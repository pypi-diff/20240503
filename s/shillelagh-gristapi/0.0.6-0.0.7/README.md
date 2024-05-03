# Comparing `tmp/shillelagh-gristapi-0.0.6.tar.gz` & `tmp/shillelagh_gristapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-gristapi-0.0.6.tar", last modified: Mon Apr  1 19:14:54 2024, max compression
+gzip compressed data, was "shillelagh_gristapi-0.0.7.tar", last modified: Fri May  3 10:31:56 2024, max compression
```

## Comparing `shillelagh-gristapi-0.0.6.tar` & `shillelagh_gristapi-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)    11357 2024-03-30 21:29:03.000000 shillelagh-gristapi-0.0.6/LICENSE.txt
--rw-r--r--   0 qleroy    (1000) qleroy    (1000)     3441 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/PKG-INFO
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     2819 2024-04-01 19:09:33.000000 shillelagh-gristapi-0.0.6/README.md
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      870 2024-04-01 19:14:29.000000 shillelagh-gristapi-0.0.6/pyproject.toml
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       38 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/setup.cfg
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.136668 shillelagh-gristapi-0.0.6/src/
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.140668 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        0 2024-03-23 05:41:01.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__init__.py
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      175 2024-03-23 08:32:37.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     6995 2024-03-23 05:41:01.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8234 2024-03-31 03:49:10.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8992 2024-03-31 03:49:05.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/grist.py
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/
--rw-r--r--   0 qleroy    (1000) qleroy    (1000)     3441 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/PKG-INFO
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      588 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/SOURCES.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        1 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/dependency_links.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       67 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/entry_points.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       35 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/requires.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       20 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/top_level.txt
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/tests/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     1515 2024-03-31 03:27:06.000000 shillelagh-gristapi-0.0.6/tests/test_grist.py
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-05-03 10:31:56.180016 shillelagh_gristapi-0.0.7/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)    11357 2024-03-30 21:29:03.000000 shillelagh_gristapi-0.0.7/LICENSE.txt
+-rw-r--r--   0 qleroy    (1000) qleroy    (1000)     3441 2024-05-03 10:31:56.180016 shillelagh_gristapi-0.0.7/PKG-INFO
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     2819 2024-04-01 19:19:33.000000 shillelagh_gristapi-0.0.7/README.md
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      870 2024-05-03 10:31:22.000000 shillelagh_gristapi-0.0.7/pyproject.toml
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       38 2024-05-03 10:31:56.180016 shillelagh_gristapi-0.0.7/setup.cfg
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-05-03 10:31:56.172016 shillelagh_gristapi-0.0.7/src/
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-05-03 10:31:56.176016 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      390 2024-05-03 10:11:43.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__init__.py
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-05-03 10:31:56.176016 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__pycache__/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      566 2024-05-03 10:13:09.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     6995 2024-03-23 05:41:01.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8295 2024-05-03 10:13:09.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     9070 2024-05-03 10:11:43.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/grist.py
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-05-03 10:31:56.176016 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/
+-rw-r--r--   0 qleroy    (1000) qleroy    (1000)     3441 2024-05-03 10:31:56.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/PKG-INFO
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      588 2024-05-03 10:31:56.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        1 2024-05-03 10:31:56.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       67 2024-05-03 10:31:56.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/entry_points.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       35 2024-05-03 10:31:56.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/requires.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       20 2024-05-03 10:31:56.000000 shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/top_level.txt
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-05-03 10:31:56.176016 shillelagh_gristapi-0.0.7/tests/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     1515 2024-03-31 03:27:06.000000 shillelagh_gristapi-0.0.7/tests/test_grist.py
```

### Comparing `shillelagh-gristapi-0.0.6/LICENSE.txt` & `shillelagh_gristapi-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.6/PKG-INFO` & `shillelagh_gristapi-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh-gristapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shillelagh adapter for querying Grist Documents.
 Author-email: Quentin Leroy <quentin.n.leroy@gmail.com>
 Project-URL: Homepage, https://github.com/qleroy/shillelagh-gristapi
 Project-URL: Issues, https://github.com/qleroy/shillelagh-gristapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,15 +87,15 @@
 To make the `shillelagh-gristapi` plugin available, add the following to your `requirements-local.txt` file:
 
 ```python
 shillelagh
 shillelagh-gristapi
 ```
 
-SqlAlechmy URI
+SqlAlchemy URI
 
 ```txt
 shillelagh+safe://
 ```
 
 Engine parameters
```

### Comparing `shillelagh-gristapi-0.0.6/README.md` & `shillelagh_gristapi-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 To make the `shillelagh-gristapi` plugin available, add the following to your `requirements-local.txt` file:
 
 ```python
 shillelagh
 shillelagh-gristapi
 ```
 
-SqlAlechmy URI
+SqlAlchemy URI
 
 ```txt
 shillelagh+safe://
 ```
 
 Engine parameters
```

### Comparing `shillelagh-gristapi-0.0.6/pyproject.toml` & `shillelagh_gristapi-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shillelagh-gristapi"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = ["requests >=2.31.0", "shillelagh >=1.2.6"]
 authors = [{ name = "Quentin Leroy", email = "quentin.n.leroy@gmail.com" }]
 description = "Shillelagh adapter for querying Grist Documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc` & `shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc` & `shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Mar 31 03:49:05 2024 UTC, .py size: 8992 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,515 +1,519 @@
-00000000: 6f0d 0d0a 0000 0000 31dd 0866 2023 0000  o.......1..f #..
+00000000: 6f0d 0d0a 0000 0000 5fb8 3466 6e23 0000  o......._.4fn#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
+00000020: 0004 0000 0040 0000 0073 4401 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d01 5a01  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6404 6c0a 5a0a 6401 6404 6c0b  ..d.d.l.Z.d.d.l.
 00000070: 5a0b 6401 6404 6c0c 5a0d 6401 6404 6c0e  Z.d.d.l.Z.d.d.l.
-00000080: 5a0e 6401 6404 6c0f 5a0f 6401 6405 6c10  Z.d.d.l.Z.d.d.l.
-00000090: 6d11 5a11 0100 6401 6406 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
-000000a0: 6d14 5a14 6d15 5a15 6d16 5a16 6d17 5a17  m.Z.m.Z.m.Z.m.Z.
-000000b0: 6d18 5a18 6d19 5a19 6d1a 5a1a 0100 6401  m.Z.m.Z.m.Z...d.
-000000c0: 6407 6c1b 6d1c 5a1c 6d1d 5a1d 0100 6401  d.l.m.Z.m.Z...d.
-000000d0: 6408 6c1e 6d1f 5a1f 6d20 5a20 0100 650a  d.l.m.Z.m Z ..e.
-000000e0: a021 a100 5a22 650b a023 6409 a101 728b  .!..Z"e..#d...r.
-000000f0: 650b a023 6409 a101 a024 a100 640a 7600  e..#d....$..d.v.
-00000100: 728b 650a 6a25 650a 6a26 640b 8d01 0100  r.e.j%e.j&d.....
-00000110: 650a a027 a100 5a28 6528 a029 650a 6a26  e..'..Z(e(.)e.j&
-00000120: a101 0100 650a a02a 640c a101 5a2b 6528  ....e..*d...Z+e(
-00000130: a02c 652b a101 0100 6522 a02d 6528 a101  .,e+....e".-e(..
-00000140: 0100 6e07 650a 6a25 650a 6a2e 640b 8d01  ..n.e.j%e.j.d...
-00000150: 0100 4700 640d 640e 8400 640e 6511 8303  ..G.d.d...d.e...
-00000160: 5a2f 6404 5300 290f 7a1f 0a41 6e20 6164  Z/d.S.).z..An ad
-00000170: 6170 7465 7220 666f 7220 7468 6520 4772  apter for the Gr
-00000180: 6973 7420 4150 492e 0ae9 0000 0000 2902  ist API.......).
-00000190: da04 6461 7465 da08 6461 7465 7469 6d65  ..date..datetime
-000001a0: 2906 da03 416e 79da 0444 6963 74da 0849  )...Any..Dict..I
-000001b0: 7465 7261 746f 72da 044c 6973 74da 084f  terator..List..O
-000001c0: 7074 696f 6e61 6cda 0554 7570 6c65 4e29  ptional..TupleN)
-000001d0: 01da 0741 6461 7074 6572 2908 da07 426f  ...Adapter)...Bo
-000001e0: 6f6c 6561 6eda 0444 6174 65da 0844 6174  olean..Date..Dat
-000001f0: 6554 696d 65da 0546 6965 6c64 da05 466c  eTime..Field..Fl
-00000200: 6f61 74da 0749 6e74 6567 6572 da05 4f72  oat..Integer..Or
-00000210: 6465 72da 0653 7472 696e 6729 02da 0646  der..String)...F
-00000220: 696c 7465 72da 0552 616e 6765 2902 da0e  ilter..Range)...
-00000230: 5265 7175 6573 7465 644f 7264 6572 da03  RequestedOrder..
-00000240: 526f 77da 0544 4542 5547 2902 da04 7472  Row..DEBUG)...tr
-00000250: 7565 da01 3129 01da 056c 6576 656c 7a29  ue..1)...levelz)
-00000260: 2528 6173 6374 696d 6529 7320 2d20 2528  %(asctime)s - %(
-00000270: 6c65 7665 6c6e 616d 6529 7320 2d20 2528  levelname)s - %(
-00000280: 6d65 7373 6167 6529 7363 0000 0000 0000  message)sc......
-00000290: 0000 0000 0000 0000 0000 0b00 0000 0000  ................
-000002a0: 0000 73a2 0100 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000002b0: 015a 0364 025a 0465 0564 2564 0365 0664  .Z.d.Z.e.d%d.e.d
-000002c0: 0465 0764 0565 0864 0665 0965 0719 0066  .e.d.e.d.e.e...f
-000002d0: 0864 0764 0884 0583 015a 0a65 0564 0365  .d.d.....Z.e.d.e
-000002e0: 0664 0665 0b65 0619 0066 0464 0964 0a84  .d.e.e...f.d.d..
-000002f0: 0483 015a 0c09 0b09 0b09 0b64 2664 0365  ...Z.......d&d.e
-00000300: 0664 0c65 0965 0619 0064 0d65 0965 0619  .d.e.e...d.e.e..
-00000310: 0064 0e65 0965 0619 0066 0887 0066 0164  .d.e.e...f...f.d
-00000320: 0f64 1084 0d5a 0d64 2764 1164 1284 045a  .d...Z.d'd.d...Z
-00000330: 0e64 0665 0f65 0665 1066 0219 0066 0264  .d.e.e.e.f...f.d
-00000340: 1364 1484 045a 1164 0665 0f65 0665 1066  .d...Z.d.e.e.e.f
-00000350: 0219 0066 0264 1564 1684 045a 1264 1765  ...f.d.d...Z.d.e
-00000360: 0f65 0665 1366 0219 0064 1865 1465 0b65  .e.e.f...d.e.e.e
-00000370: 0665 1566 0219 0019 0064 0665 1665 1719  .e.f.....d.e.e..
-00000380: 0066 0664 1964 1a84 045a 1864 1765 0f65  .f.d.d...Z.d.e.e
-00000390: 0665 1366 0219 0064 1865 1465 0b65 0665  .e.f...d.e.e.e.e
-000003a0: 1566 0219 0019 0064 0665 1665 1719 0066  .f.....d.e.e...f
-000003b0: 0664 1b64 1c84 045a 1964 1765 0f65 0665  .d.d...Z.d.e.e.e
-000003c0: 1366 0219 0064 1865 1465 0b65 0665 1566  .f...d.e.e.e.e.f
-000003d0: 0219 0019 0064 0665 1665 1719 0066 0664  .....d.e.e...f.d
-000003e0: 1d64 1e84 045a 1a64 0665 0f65 0665 1066  .d...Z.d.e.e.e.f
-000003f0: 0219 0066 0264 1f64 2084 045a 1b64 0665  ...f.d.d ..Z.d.e
-00000400: 0f65 0665 0866 0219 0066 0264 2164 2284  .e.e.f...f.d!d".
-00000410: 045a 1c64 1765 0f65 0665 1366 0219 0064  .Z.d.e.e.e.f...d
-00000420: 1865 1465 0b65 0665 1566 0219 0019 0064  .e.e.e.e.f.....d
-00000430: 0665 1665 1719 0066 0664 2364 2484 045a  .e.e...f.d#d$..Z
-00000440: 1d87 0004 005a 1e53 0029 28da 0847 7269  .....Z.S.)(..Gri
-00000450: 7374 4150 497a 270a 2020 2020 416e 2061  stAPIz'.    An a
-00000460: 6461 7074 6572 2066 6f72 2074 6865 2047  dapter for the G
-00000470: 7269 7374 2041 5049 2e0a 2020 2020 54da  rist API..    T.
-00000480: 0375 7269 da04 6661 7374 da06 6b77 6172  .uri..fast..kwar
-00000490: 6773 da06 7265 7475 726e 6302 0000 0000  gs..returnc.....
-000004a0: 0000 0000 0000 0004 0000 0008 0000 004b  ...............K
-000004b0: 0000 0073 4200 0000 7400 a001 6401 7c00  ...sB...t...d.|.
-000004c0: 9b02 6402 7c01 9b02 6403 7c02 9b02 9d06  ..d.|...d.|.....
-000004d0: a101 0100 7402 6a03 a004 7c00 a101 7d03  ....t.j...|...}.
-000004e0: 7400 a001 6404 7c03 9b02 9d02 a101 0100  t...d.|.........
-000004f0: 7c03 6a05 6405 6b02 5300 2906 4e7a 0d73  |.j.d.k.S.).Nz.s
-00000500: 7570 706f 7274 7320 7572 693d 7a06 2066  upports uri=z. f
-00000510: 6173 743d 7a08 206b 7761 7267 733d 7a10  ast=z. kwargs=z.
-00000520: 7375 7070 6f72 7473 2070 6172 7365 643d  supports parsed=
-00000530: da05 6772 6973 7429 06da 066c 6f67 6765  ..grist)...logge
-00000540: 72da 0564 6562 7567 da06 7572 6c6c 6962  r..debug..urllib
-00000550: da05 7061 7273 65da 0875 726c 7061 7273  ..parse..urlpars
-00000560: 65da 0673 6368 656d 6529 0472 1c00 0000  e..scheme).r....
-00000570: 721d 0000 0072 1e00 0000 da06 7061 7273  r....r......pars
-00000580: 6564 a900 7228 0000 00fa 522f 686f 6d65  ed..r(....R/home
-00000590: 2f71 6c65 726f 792f 6772 6973 742f 7368  /qleroy/grist/sh
-000005a0: 696c 6c65 6c61 6768 2f73 6869 6c6c 656c  illelagh/shillel
-000005b0: 6167 682d 6772 6973 7461 7069 2f73 7263  agh-gristapi/src
-000005c0: 2f73 6869 6c6c 656c 6167 685f 6772 6973  /shillelagh_gris
-000005d0: 7461 7069 2f67 7269 7374 2e70 79da 0873  tapi/grist.py..s
-000005e0: 7570 706f 7274 7341 0000 0073 0800 0000  upportsA...s....
-000005f0: 1c02 0c01 1001 0a01 7a11 4772 6973 7441  ........z.GristA
-00000600: 5049 2e73 7570 706f 7274 7363 0100 0000  PI.supportsc....
-00000610: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000620: 4300 0000 7306 0000 007c 0066 0153 00a9  C...s....|.f.S..
-00000630: 014e 7228 0000 0029 0172 1c00 0000 7228  .Nr(...).r....r(
-00000640: 0000 0072 2800 0000 7229 0000 00da 0970  ...r(...r).....p
-00000650: 6172 7365 5f75 7269 4800 0000 7302 0000  arse_uriH...s...
-00000660: 0006 027a 1247 7269 7374 4150 492e 7061  ...z.GristAPI.pa
-00000670: 7273 655f 7572 694e da06 6f72 675f 6964  rse_uriN..org_id
-00000680: da06 7365 7276 6572 da07 6170 695f 6b65  ..server..api_ke
-00000690: 7963 0500 0000 0000 0000 0000 0000 0800  yc..............
-000006a0: 0000 0500 0000 0300 0000 73f4 0000 0074  ..........s....t
-000006b0: 0083 00a0 01a1 0001 0074 026a 03a0 047c  .........t.j...|
-000006c0: 01a1 017d 0574 026a 03a0 057c 056a 06a1  ...}.t.j...|.j..
-000006d0: 017d 067c 056a 07a0 0864 01a1 017d 0764  .}.|.j...d...}.d
-000006e0: 007c 005f 0974 0a7c 0783 0164 026b 0472  .|._.t.|...d.k.r
-000006f0: 267c 0764 0219 007c 005f 097c 056a 0b7c  &|.d...|._.|.j.|
-00000700: 005f 0c74 0da0 0e64 037c 006a 0c9b 029d  ._.t...d.|.j....
-00000710: 02a1 0101 007c 0473 3b7c 0664 0419 0064  .....|.s;|.d...d
-00000720: 0519 007d 047c 0373 437c 0664 0619 0064  ...}.|.sC|.d...d
-00000730: 0519 007d 037c 0273 4b7c 0664 0719 0064  ...}.|.sK|.d...d
-00000740: 0519 007d 027c 027c 005f 0f64 0864 097c  ...}.|.|._.d.d.|
-00000750: 049b 009d 0269 017c 005f 107c 037c 005f  .....i.|._.|.|._
-00000760: 1174 126a 1364 0a64 0b64 0c64 0d8d 037c  .t.j.d.d.d.d...|
-00000770: 005f 147c 006a 0c72 747c 006a 0972 6e7c  ._.|.j.rt|.j.rn|
-00000780: 00a0 15a1 0001 0064 0053 007c 00a0 16a1  .......d.S.|....
-00000790: 0001 0064 0053 007c 00a0 17a1 0001 0064  ...d.S.|.......d
-000007a0: 0053 0029 0e4e fa01 2fe9 0100 0000 7a15  .S.).N../.....z.
-000007b0: 5f5f 696e 6974 5f5f 2073 656c 662e 646f  __init__ self.do
-000007c0: 635f 6964 3dda 036b 6579 7201 0000 0072  c_id=..keyr....r
-000007d0: 2e00 0000 722d 0000 00da 0d41 7574 686f  ....r-.....Autho
-000007e0: 7269 7a61 7469 6f6e 7a07 4265 6172 6572  rizationz.Bearer
-000007f0: 20da 0b67 7269 7374 5f63 6163 6865 da06   ..grist_cache..
-00000800: 7371 6c69 7465 e9b4 0000 0029 03da 0a63  sqlite.....)...c
-00000810: 6163 6865 5f6e 616d 65da 0762 6163 6b65  ache_name..backe
-00000820: 6e64 da0c 6578 7069 7265 5f61 6674 6572  nd..expire_after
-00000830: 2918 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
-00000840: 745f 5f72 2300 0000 7224 0000 0072 2500  t__r#...r$...r%.
-00000850: 0000 da08 7061 7273 655f 7173 da05 7175  ....parse_qs..qu
-00000860: 6572 79da 0470 6174 68da 0573 706c 6974  ery..path..split
-00000870: da08 7461 626c 655f 6964 da03 6c65 6eda  ..table_id..len.
-00000880: 066e 6574 6c6f 63da 0664 6f63 5f69 6472  .netloc..doc_idr
-00000890: 2100 0000 7222 0000 0072 2d00 0000 da07  !...r"...r-.....
-000008a0: 6865 6164 6572 7372 2e00 0000 da0e 7265  headersr......re
-000008b0: 7175 6573 7473 5f63 6163 6865 da0d 4361  quests_cache..Ca
-000008c0: 6368 6564 5365 7373 696f 6eda 085f 7365  chedSession.._se
-000008d0: 7373 696f 6eda 115f 7365 745f 636f 6c75  ssion.._set_colu
-000008e0: 6d6e 735f 6461 7461 da13 5f73 6574 5f63  mns_data.._set_c
-000008f0: 6f6c 756d 6e73 5f74 6162 6c65 73da 115f  olumns_tables.._
-00000900: 7365 745f 636f 6c75 6d6e 735f 646f 6373  set_columns_docs
-00000910: 2908 da04 7365 6c66 721c 0000 0072 2d00  )...selfr....r-.
-00000920: 0000 722e 0000 0072 2f00 0000 7227 0000  ..r....r/...r'..
-00000930: 00da 0c71 7565 7279 5f73 7472 696e 67da  ...query_string.
-00000940: 0a73 706c 6974 5f70 6174 68a9 01da 095f  .split_path...._
-00000950: 5f63 6c61 7373 5f5f 7228 0000 0072 2900  _class__r(...r).
-00000960: 0000 723b 0000 004c 0000 0073 3800 0000  ..r;...L...s8...
-00000970: 0a07 0c02 0e01 0c02 0601 0c01 0a01 0801  ................
-00000980: 1201 0401 0c01 0401 0c01 0401 0c01 0601  ................
-00000990: 1001 0601 0402 0201 0201 0201 08fd 0606  ................
-000009a0: 0601 0c01 0c02 0c02 7a11 4772 6973 7441  ........z.GristA
-000009b0: 5049 2e5f 5f69 6e69 745f 5f63 0100 0000  PI.__init__c....
-000009c0: 0000 0000 0000 0000 0500 0000 0600 0000  ................
-000009d0: 0300 0000 73b2 0000 0074 00a0 0164 017c  ....s....t...d.|
-000009e0: 006a 029b 029d 02a1 0101 007c 006a 039b  .j.........|.j..
-000009f0: 0064 027c 006a 049b 0064 037c 006a 029b  .d.|.j...d.|.j..
-00000a00: 0064 049d 067d 0174 056a 067c 017c 006a  .d...}.t.j.|.|.j
-00000a10: 0764 058d 027d 027c 02a0 08a1 0064 0619  .d...}.|.....d..
-00000a20: 007d 0364 0764 0884 0089 0087 0066 0164  .}.d.d.......f.d
-00000a30: 0964 0a84 087c 0344 0083 017d 0464 0b64  .d...|.D...}.d.d
-00000a40: 0c84 007c 0444 0083 017c 005f 0964 0d64  ...|.D...|._.d.d
-00000a50: 0c84 007c 006a 09a0 0aa1 0044 0083 017c  ...|.j.....D...|
-00000a60: 005f 0b74 0c74 0d6a 0e64 0e8d 017c 006a  ._.t.t.j.d...|.j
-00000a70: 0964 0f3c 0074 00a0 0164 107c 006a 099b  .d.<.t...d.|.j..
-00000a80: 029d 02a1 0101 0064 1153 0029 127a 810a  .......d.S.).z..
-00000a90: 2020 2020 2020 2020 4361 6c6c 2074 6f0a          Call to.
-00000aa0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00000ab0: 7375 7070 6f72 742e 6765 7467 7269 7374  support.getgrist
-00000ac0: 2e63 6f6d 2f61 7069 2f23 7461 672f 636f  .com/api/#tag/co
-00000ad0: 6c75 6d6e 732f 6f70 6572 6174 696f 6e2f  lumns/operation/
-00000ae0: 6c69 7374 436f 6c75 6d6e 730a 2020 2020  listColumns.    
-00000af0: 2020 2020 746f 2073 6574 2063 6f6c 756d      to set colum
-00000b00: 6e20 7479 7065 730a 2020 2020 2020 2020  n types.        
-00000b10: 7a20 5f73 6574 5f63 6f6c 756d 6e73 5f64  z _set_columns_d
-00000b20: 6174 6120 7365 6c66 2e74 6162 6c65 5f69  ata self.table_i
-00000b30: 643d fa0a 2f61 7069 2f64 6f63 732f fa08  d=../api/docs/..
-00000b40: 2f74 6162 6c65 732f 7a08 2f63 6f6c 756d  /tables/z./colum
-00000b50: 6e73 a901 7244 0000 00da 0763 6f6c 756d  ns..rD.....colum
-00000b60: 6e73 6301 0000 0000 0000 0000 0000 0001  nsc.............
-00000b70: 0000 0005 0000 0053 0000 0073 0a01 0000  .......S...s....
-00000b80: 7c00 6401 6b02 720a 7400 7401 6a02 6402  |.d.k.r.t.t.j.d.
-00000b90: 8d01 5300 7c00 6403 6b02 7214 7403 7401  ..S.|.d.k.r.t.t.
-00000ba0: 6a02 6402 8d01 5300 7c00 6404 6b02 721e  j.d...S.|.d.k.r.
-00000bb0: 7404 7401 6a02 6402 8d01 5300 7c00 6405  t.t.j.d...S.|.d.
-00000bc0: 6b02 7228 7405 7401 6a02 6402 8d01 5300  k.r(t.t.j.d...S.
-00000bd0: 7c00 6406 6b02 7232 7400 7401 6a02 6402  |.d.k.r2t.t.j.d.
-00000be0: 8d01 5300 7c00 6407 6b02 723c 7400 7401  ..S.|.d.k.r<t.t.
-00000bf0: 6a02 6402 8d01 5300 7c00 6408 6b02 7249  j.d...S.|.d.k.rI
-00000c00: 7406 7407 6701 6409 7401 6a02 640a 8d03  t.t.g.d.t.j.d...
-00000c10: 5300 7c00 a008 640b a101 7257 7409 7407  S.|...d...rWt.t.
-00000c20: 6701 6409 7401 6a02 640a 8d03 5300 7c00  g.d.t.j.d...S.|.
-00000c30: a008 640c a101 7262 7400 7401 6a02 6402  ..d...rbt.t.j.d.
-00000c40: 8d01 5300 7c00 a008 640d a101 726d 7400  ..S.|...d...rmt.
-00000c50: 7401 6a02 6402 8d01 5300 7c00 640e 6b02  t.j.d...S.|.d.k.
-00000c60: 7277 7400 7401 6a02 6402 8d01 5300 740a  rwt.t.j.d...S.t.
-00000c70: a00b 640f 7c00 9b02 9d02 a101 0100 7400  ..d.|.........t.
-00000c80: 7401 6a02 6402 8d01 5300 2910 4eda 0454  t.j.d...S.).N..T
-00000c90: 6578 74a9 01da 056f 7264 6572 da03 496e  ext....order..In
-00000ca0: 74da 074e 756d 6572 6963 da04 426f 6f6c  t..Numeric..Bool
-00000cb0: da06 4368 6f69 6365 da0a 4368 6f69 6365  ..Choice..Choice
-00000cc0: 4c69 7374 720c 0000 0046 2903 da07 6669  Listr....F)...fi
-00000cd0: 6c74 6572 73da 0565 7861 6374 7256 0000  lters..exactrV..
-00000ce0: 007a 0944 6174 6554 696d 653a 7a04 5265  .z.DateTime:z.Re
-00000cf0: 663a 7a08 5265 664c 6973 743a da0b 4174  f:z.RefList:..At
-00000d00: 7461 6368 6d65 6e74 737a 0574 7970 653d  tachmentsz.type=
-00000d10: 290c 7212 0000 0072 1100 0000 da03 414e  ).r....r......AN
-00000d20: 5972 1000 0000 720f 0000 0072 0b00 0000  Yr....r....r....
-00000d30: 720c 0000 0072 1400 0000 da0a 7374 6172  r....r......star
-00000d40: 7473 7769 7468 720d 0000 0072 2100 0000  tswithr....r!...
-00000d50: 7222 0000 0029 01da 0474 7970 6572 2800  r"...)...typer(.
-00000d60: 0000 7228 0000 0072 2900 0000 da07 6765  ..r(...r).....ge
-00000d70: 7474 7970 6582 0000 0073 3000 0000 0801  ttype....s0.....
-00000d80: 0c01 0801 0c01 0801 0c01 0801 0c01 0801  ................
-00000d90: 0c01 0801 0c01 0801 1201 0a01 1201 0a01  ................
-00000da0: 0c01 0a01 0c01 0801 0c01 1002 0c01 7a2b  ..............z+
-00000db0: 4772 6973 7441 5049 2e5f 7365 745f 636f  GristAPI._set_co
-00000dc0: 6c75 6d6e 735f 6461 7461 2e3c 6c6f 6361  lumns_data.<loca
-00000dd0: 6c73 3e2e 6765 7474 7970 6563 0100 0000  ls>.gettypec....
-00000de0: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00000df0: 1300 0000 7324 0000 0067 007c 005d 0e7d  ....s$...g.|.].}
-00000e00: 017c 0164 0019 0088 007c 0164 0119 0064  .|.d.....|.d...d
-00000e10: 0219 0083 0166 0291 0271 0253 0029 03da  .....f...q.S.)..
-00000e20: 0269 64da 0666 6965 6c64 7372 6100 0000  .id..fieldsra...
-00000e30: 7228 0000 0029 02da 022e 30da 0163 a901  r(...)....0..c..
-00000e40: 7262 0000 0072 2800 0000 7229 0000 00da  rb...r(...r)....
-00000e50: 0a3c 6c69 7374 636f 6d70 3e9d 0000 0073  .<listcomp>....s
-00000e60: 0200 0000 2400 7a2e 4772 6973 7441 5049  ....$.z.GristAPI
-00000e70: 2e5f 7365 745f 636f 6c75 6d6e 735f 6461  ._set_columns_da
-00000e80: 7461 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ta.<locals>.<lis
-00000e90: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
-00000ea0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-00000eb0: 1a00 0000 6900 7c00 5d09 7d01 7c01 6400  ....i.|.].}.|.d.
-00000ec0: 1900 7c01 6401 1900 9302 7102 5300 2902  ..|.d.....q.S.).
-00000ed0: 7201 0000 0072 3100 0000 7228 0000 0029  r....r1...r(...)
-00000ee0: 0272 6500 0000 da02 6c74 7228 0000 0072  .re.....ltr(...r
-00000ef0: 2800 0000 7229 0000 00da 0a3c 6469 6374  (...r).....<dict
-00000f00: 636f 6d70 3e9e 0000 0073 0200 0000 1a00  comp>....s......
-00000f10: 7a2e 4772 6973 7441 5049 2e5f 7365 745f  z.GristAPI._set_
-00000f20: 636f 6c75 6d6e 735f 6461 7461 2e3c 6c6f  columns_data.<lo
-00000f30: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00000f40: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000f50: 0005 0000 0053 0000 0073 2600 0000 6900  .....S...s&...i.
-00000f60: 7c00 5d0f 5c02 7d01 7d02 7400 7c02 8301  |.].\.}.}.t.|...
-00000f70: 7401 7402 6602 7600 7202 7c01 7c02 9302  t.t.f.v.r.|.|...
-00000f80: 7102 5300 7228 0000 0029 0372 6100 0000  q.S.r(...).ra...
-00000f90: 720c 0000 0072 0d00 0000 2903 7265 0000  r....r....).re..
-00000fa0: 00da 016b da01 7672 2800 0000 7228 0000  ...k..vr(...r(..
-00000fb0: 0072 2900 0000 726a 0000 009f 0000 0073  .r)...rj.......s
-00000fc0: 0400 0000 0600 2001 7255 0000 0072 6300  ...... .rU...rc.
-00000fd0: 0000 7a1f 5f73 6574 5f63 6f6c 756d 6e73  ..z._set_columns
-00000fe0: 5f64 6174 6120 7365 6c66 2e63 6f6c 756d  _data self.colum
-00000ff0: 6e73 3d4e 290f 7221 0000 0072 2200 0000  ns=N).r!...r"...
-00001000: 7240 0000 0072 2e00 0000 7243 0000 00da  r@...r....rC....
-00001010: 0872 6571 7565 7374 73da 0367 6574 7244  .requests..getrD
-00001020: 0000 00da 046a 736f 6e72 5300 0000 da05  .....jsonrS.....
-00001030: 6974 656d 73da 1263 6f6c 756d 6e73 5f64  items..columns_d
-00001040: 6174 6573 7469 6d65 7372 1000 0000 7211  atestimesr....r.
-00001050: 0000 0072 5f00 0000 2905 724b 0000 00da  ...r_...).rK....
-00001060: 0375 726c da08 7265 7370 6f6e 7365 7253  .url..responserS
-00001070: 0000 00da 0a6c 6162 656c 7479 7065 7372  .....labeltypesr
-00001080: 2800 0000 7267 0000 0072 2900 0000 7248  (...rg...r)...rH
-00001090: 0000 0076 0000 0073 1800 0000 1206 1c01  ...v...s........
-000010a0: 1002 0c01 0802 121b 1001 0601 0801 08ff  ................
-000010b0: 1203 1602 7a1a 4772 6973 7441 5049 2e5f  ....z.GristAPI._
-000010c0: 7365 745f 636f 6c75 6d6e 735f 6461 7461  set_columns_data
-000010d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000010e0: 0004 0000 0043 0000 0073 1600 0000 6401  .....C...s....d.
-000010f0: 7400 7401 6a02 6402 8d01 6901 7c00 5f03  t.t.j.d...i.|._.
-00001100: 6400 5300 2903 4e72 6300 0000 7255 0000  d.S.).Nrc...rU..
-00001110: 0029 0472 1200 0000 7211 0000 0072 5f00  .).r....r....r_.
-00001120: 0000 7253 0000 00a9 0172 4b00 0000 7228  ..rS.....rK...r(
-00001130: 0000 0072 2800 0000 7229 0000 0072 4900  ...r(...r)...rI.
-00001140: 0000 a600 0000 7304 0000 000c 020a ff7a  ......s........z
-00001150: 1c47 7269 7374 4150 492e 5f73 6574 5f63  .GristAPI._set_c
-00001160: 6f6c 756d 6e73 5f74 6162 6c65 7363 0100  olumns_tablesc..
-00001170: 0000 0000 0000 0000 0000 0100 0000 0a00  ................
-00001180: 0000 4300 0000 735c 0000 0074 0074 016a  ..C...s\...t.t.j
-00001190: 0264 018d 0174 0374 016a 0264 018d 0174  .d...t.t.j.d...t
-000011a0: 0374 016a 0264 018d 0174 0374 016a 0264  .t.j.d...t.t.j.d
-000011b0: 018d 0174 0374 016a 0264 018d 0174 0374  ...t.t.j.d...t.t
-000011c0: 016a 0264 018d 0174 0374 016a 0264 018d  .j.d...t.t.j.d..
-000011d0: 0174 0374 016a 0264 018d 0164 029c 087c  .t.t.j.d...d...|
-000011e0: 005f 0464 0053 0029 034e 7255 0000 00a9  ._.d.S.).NrU....
-000011f0: 0872 6300 0000 da04 6e61 6d65 da06 6163  .rc.....name..ac
-00001200: 6365 7373 da09 6f72 6744 6f6d 6169 6e72  cess..orgDomainr
-00001210: 4300 0000 da08 646f 635f 6e61 6d65 da0d  C.....doc_name..
-00001220: 646f 635f 6372 6561 7465 6441 74da 0d64  doc_createdAt..d
-00001230: 6f63 5f75 7064 6174 6564 4174 2905 7210  oc_updatedAt).r.
-00001240: 0000 0072 1100 0000 725f 0000 0072 1200  ...r....r_...r..
-00001250: 0000 7253 0000 0072 7500 0000 7228 0000  ..rS...ru...r(..
-00001260: 0072 2800 0000 7229 0000 0072 4a00 0000  .r(...r)...rJ...
-00001270: ab00 0000 7312 0000 000a 020a 010a 010a  ....s...........
-00001280: 010a 010a 010a 010a 010c f87a 1a47 7269  ...........z.Gri
-00001290: 7374 4150 492e 5f73 6574 5f63 6f6c 756d  stAPI._set_colum
-000012a0: 6e73 5f64 6f63 73da 0662 6f75 6e64 7372  ns_docs..boundsr
-000012b0: 5600 0000 6303 0000 0000 0000 0000 0000  V...c...........
-000012c0: 000c 0000 0006 0000 006b 0000 0073 2a01  .........k...s*.
-000012d0: 0000 8100 7400 a001 6401 a101 0100 7c00  ....t...d.....|.
-000012e0: 6a02 9b00 6402 7c00 6a03 9b00 6403 7c00  j...d.|.j...d.|.
-000012f0: 6a04 9b00 6404 9d06 7d04 7400 a001 6405  j...d...}.t...d.
-00001300: 7c04 9b02 9d02 a101 0100 7405 6a06 7c04  |.........t.j.|.
-00001310: 7c00 6a07 6406 8d02 7d05 7c05 a008 a100  |.j.d...}.|.....
-00001320: 6407 1900 7d06 7c06 4400 5d66 7d07 7c07  d...}.|.D.]f}.|.
-00001330: 6408 1900 7d08 7400 a001 6409 7c08 9b02  d...}.t...d.|...
-00001340: 9d02 a101 0100 7400 a001 640a 7c00 6a09  ......t...d.|.j.
-00001350: 9b02 9d02 a101 0100 6900 7d09 7c07 640b  ........i.}.|.d.
-00001360: 1900 7c09 640b 3c00 7c08 a00a a100 4400  ..|.d.<.|.....D.
-00001370: 5d3f 5c02 7d0a 7d0b 740b 7c00 6a09 7c0a  ]?\.}.}.t.|.j.|.
-00001380: 1900 740c 8302 7267 7c0b 640c 7501 7267  ..t...rg|.d.u.rg
-00001390: 740d a00e 740f 7c0b 8301 a101 7d0b 6e23  t...t.|.....}.n#
-000013a0: 740b 7c00 6a09 7c0a 1900 7410 8302 727b  t.|.j.|...t...r{
-000013b0: 7c0b 640c 7501 727b 7411 a00e 740f 7c0b  |.d.u.r{t...t.|.
-000013c0: 8301 a101 7d0b 6e0f 740b 7c0b 7412 8302  ....}.n.t.|.t...
-000013d0: 728a 640d a013 640e 640f 8400 7c0b 4400  r.d...d.d...|.D.
-000013e0: 8301 a101 7d0b 7c0b 7c09 7c0a 3c00 714f  ....}.|.|.|.<.qO
-000013f0: 7c09 5600 0100 712c 640c 5300 2910 7a82  |.V...q,d.S.).z.
-00001400: 0a20 2020 2020 2020 2043 616c 6c20 746f  .        Call to
-00001410: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-00001420: 2f73 7570 706f 7274 2e67 6574 6772 6973  /support.getgris
-00001430: 742e 636f 6d2f 6170 692f 2374 6167 2f72  t.com/api/#tag/r
-00001440: 6563 6f72 6473 2f6f 7065 7261 7469 6f6e  ecords/operation
-00001450: 2f6c 6973 7452 6563 6f72 6473 0a20 2020  /listRecords.   
-00001460: 2020 2020 2059 6965 6c64 7320 6120 726f       Yields a ro
-00001470: 7720 6f66 2064 6174 610a 2020 2020 2020  w of data.      
-00001480: 2020 da0b 6665 7463 685f 7461 626c 6572    ..fetch_tabler
-00001490: 5000 0000 7251 0000 007a 082f 7265 636f  P...rQ...z./reco
-000014a0: 7264 737a 1066 6574 6368 5f74 6162 6c65  rdsz.fetch_table
-000014b0: 2075 726c 3d72 5200 0000 da07 7265 636f   url=rR.....reco
-000014c0: 7264 7372 6400 0000 7a06 6669 656c 643d  rdsrd...z.field=
-000014d0: 7a0d 7365 6c66 2e63 6f6c 756d 6e73 3d72  z.self.columns=r
-000014e0: 6300 0000 4efa 012c 6301 0000 0000 0000  c...N..,c.......
-000014f0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001500: 0073 1400 0000 6700 7c00 5d06 7d01 7400  .s....g.|.].}.t.
-00001510: 7c01 8301 9102 7102 5300 7228 0000 0029  |.....q.S.r(...)
-00001520: 01da 0373 7472 2902 7265 0000 00da 0469  ...str).re.....i
-00001530: 7465 6d72 2800 0000 7228 0000 0072 2900  temr(...r(...r).
-00001540: 0000 7268 0000 00d4 0000 0073 0200 0000  ..rh.......s....
-00001550: 1400 7a28 4772 6973 7441 5049 2e66 6574  ..z(GristAPI.fet
-00001560: 6368 5f74 6162 6c65 2e3c 6c6f 6361 6c73  ch_table.<locals
-00001570: 3e2e 3c6c 6973 7463 6f6d 703e 2914 7221  >.<listcomp>).r!
-00001580: 0000 0072 2200 0000 722e 0000 0072 4300  ...r"...r....rC.
-00001590: 0000 7240 0000 0072 6d00 0000 726e 0000  ..r@...rm...rn..
-000015a0: 0072 4400 0000 726f 0000 0072 5300 0000  .rD...ro...rS...
-000015b0: 7270 0000 00da 0a69 7369 6e73 7461 6e63  rp.....isinstanc
-000015c0: 6572 0c00 0000 7202 0000 00da 0d66 726f  er....r......fro
-000015d0: 6d74 696d 6573 7461 6d70 da03 696e 7472  mtimestamp..intr
-000015e0: 0d00 0000 7203 0000 00da 046c 6973 74da  ....r......list.
-000015f0: 046a 6f69 6e29 0c72 4b00 0000 727d 0000  .join).rK...r}..
-00001600: 0072 5600 0000 721e 0000 0072 7200 0000  .rV...r....rr...
-00001610: 7273 0000 0072 7f00 0000 da06 7265 636f  rs...r......reco
-00001620: 7264 da05 6669 656c 64da 0166 726b 0000  rd..field..frk..
-00001630: 0072 6c00 0000 7228 0000 0072 2800 0000  .rl...r(...r(...
-00001640: 7229 0000 0072 7e00 0000 b700 0000 732c  r)...r~.......s,
-00001650: 0000 0002 800a 0b1c 0110 0110 020c 0108  ................
-00001660: 0108 0110 0112 0104 010c 0110 0118 0110  ................
-00001670: 0118 0110 010a 0114 010a 0108 0104 f27a  ...............z
-00001680: 1447 7269 7374 4150 492e 6665 7463 685f  .GristAPI.fetch_
-00001690: 7461 626c 6563 0300 0000 0000 0000 0000  tablec..........
-000016a0: 0000 0800 0000 0400 0000 6b00 0000 734e  ..........k...sN
-000016b0: 0000 0081 007c 006a 009b 0064 017c 006a  .....|.j...d.|.j
-000016c0: 019b 0064 029d 047d 0474 026a 037c 047c  ...d...}.t.j.|.|
-000016d0: 006a 0464 038d 027d 057c 05a0 05a1 0064  .j.d...}.|.....d
-000016e0: 0419 007d 067c 0644 005d 097d 0764 057c  ...}.|.D.].}.d.|
-000016f0: 0764 0519 0069 0156 0001 0071 1b64 0653  .d...i.V...q.d.S
-00001700: 0029 077a 7d0a 2020 2020 2020 2020 4361  .).z}.        Ca
-00001710: 6c6c 2074 6f0a 2020 2020 2020 2020 6874  ll to.        ht
-00001720: 7470 733a 2f2f 7375 7070 6f72 742e 6765  tps://support.ge
-00001730: 7467 7269 7374 2e63 6f6d 2f61 7069 2f23  tgrist.com/api/#
-00001740: 7461 672f 7461 626c 6573 2f6f 7065 7261  tag/tables/opera
-00001750: 7469 6f6e 2f6c 6973 7454 6162 6c65 730a  tion/listTables.
-00001760: 2020 2020 2020 2020 5969 656c 6473 2061          Yields a
-00001770: 2074 6162 6c65 5f69 640a 2020 2020 2020   table_id.      
-00001780: 2020 7250 0000 007a 072f 7461 626c 6573    rP...z./tables
-00001790: 7252 0000 00da 0674 6162 6c65 7372 6300  rR.....tablesrc.
-000017a0: 0000 4e29 0672 2e00 0000 7243 0000 0072  ..N).r....rC...r
-000017b0: 6d00 0000 726e 0000 0072 4400 0000 726f  m...rn...rD...ro
-000017c0: 0000 0029 0872 4b00 0000 727d 0000 0072  ...).rK...r}...r
-000017d0: 5600 0000 721e 0000 0072 7200 0000 7273  V...r....rr...rs
-000017e0: 0000 0072 8b00 0000 da05 7461 626c 6572  ...r......tabler
-000017f0: 2800 0000 7228 0000 0072 2900 0000 da0f  (...r(...r).....
-00001800: 6665 7463 685f 7461 626c 655f 6964 73d8  fetch_table_ids.
-00001810: 0000 0073 0e00 0000 0280 140b 1002 0c01  ...s............
-00001820: 0801 1001 04ff 7a18 4772 6973 7441 5049  ......z.GristAPI
-00001830: 2e66 6574 6368 5f74 6162 6c65 5f69 6473  .fetch_table_ids
-00001840: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
-00001850: 000b 0000 006b 0000 0073 8200 0000 8100  .....k...s......
-00001860: 7c00 6a00 9b00 6401 7c00 6a01 9b00 6402  |.j...d.|.j...d.
-00001870: 9d04 7d04 7402 6a03 7c04 7c00 6a04 6403  ..}.t.j.|.|.j.d.
-00001880: 8d02 7d05 7c05 a005 a100 7d06 7c06 4400  ..}.|.....}.|.D.
-00001890: 5d25 7d07 7c07 6404 1900 4400 5d1e 7d08  ]%}.|.d...D.].}.
-000018a0: 7c07 6405 1900 7c07 6406 1900 7c07 6407  |.d...|.d...|.d.
-000018b0: 1900 7c07 6408 1900 7c08 6405 1900 7c08  ..|.d...|.d...|.
-000018c0: 6406 1900 7c08 6409 1900 7c08 640a 1900  d...|.d...|.d...
-000018d0: 640b 9c08 5600 0100 711f 7119 640c 5300  d...V...q.q.d.S.
-000018e0: 290d 7a83 0a20 2020 2020 2020 2043 616c  ).z..        Cal
-000018f0: 6c20 746f 0a20 2020 2020 2020 2068 7474  l to.        htt
-00001900: 7073 3a2f 2f73 7570 706f 7274 2e67 6574  ps://support.get
-00001910: 6772 6973 742e 636f 6d2f 6170 692f 2374  grist.com/api/#t
-00001920: 6167 2f77 6f72 6b73 7061 6365 732f 6f70  ag/workspaces/op
-00001930: 6572 6174 696f 6e2f 6c69 7374 576f 726b  eration/listWork
-00001940: 7370 6163 6573 0a20 2020 2020 2020 2059  spaces.        Y
-00001950: 6965 6c64 7320 6120 646f 635f 6964 0a20  ields a doc_id. 
-00001960: 2020 2020 2020 207a 0a2f 6170 692f 6f72         z./api/or
-00001970: 6773 2f7a 0b2f 776f 726b 7370 6163 6573  gs/z./workspaces
-00001980: 7252 0000 00da 0464 6f63 7372 6300 0000  rR.....docsrc...
-00001990: 7277 0000 0072 7800 0000 7279 0000 00da  rw...rx...ry....
-000019a0: 0963 7265 6174 6564 4174 da09 7570 6461  .createdAt..upda
-000019b0: 7465 6441 7472 7600 0000 4e29 0672 2e00  tedAtrv...N).r..
-000019c0: 0000 722d 0000 0072 6d00 0000 726e 0000  ..r-...rm...rn..
-000019d0: 0072 4400 0000 726f 0000 0029 0972 4b00  .rD...ro...).rK.
-000019e0: 0000 727d 0000 0072 5600 0000 721e 0000  ..r}...rV...r...
-000019f0: 0072 7200 0000 7273 0000 00da 0a77 6f72  .rr...rs.....wor
-00001a00: 6b73 7061 6365 73da 0977 6f72 6b73 7061  kspaces..workspa
-00001a10: 6365 da03 646f 6372 2800 0000 7228 0000  ce..docr(...r(..
-00001a20: 0072 2900 0000 da0e 6665 7463 685f 646f  .r).....fetch_do
-00001a30: 6373 5f69 6473 ea00 0000 7322 0000 0002  cs_ids....s"....
-00001a40: 8014 0b10 0208 0108 010c 0106 0206 0106  ................
-00001a50: 0106 0106 0106 0106 0106 010a f802 ff04  ................
-00001a60: ff7a 1747 7269 7374 4150 492e 6665 7463  .z.GristAPI.fetc
-00001a70: 685f 646f 6373 5f69 6473 6301 0000 0000  h_docs_idsc.....
-00001a80: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001a90: 0000 0073 0600 0000 7c00 6a00 5300 722b  ...s....|.j.S.r+
-00001aa0: 0000 0029 0172 5300 0000 7275 0000 0072  ...).rS...ru...r
-00001ab0: 2800 0000 7228 0000 0072 2900 0000 da0b  (...r(...r).....
-00001ac0: 6765 745f 636f 6c75 6d6e 7306 0100 0073  get_columns....s
-00001ad0: 0200 0000 0601 7a14 4772 6973 7441 5049  ......z.GristAPI
-00001ae0: 2e67 6574 5f63 6f6c 756d 6e73 6301 0000  .get_columnsc...
-00001af0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00001b00: 0043 0000 0073 0400 0000 6900 5300 722b  .C...s....i.S.r+
-00001b10: 0000 0072 2800 0000 7275 0000 0072 2800  ...r(...ru...r(.
-00001b20: 0000 7228 0000 0072 2900 0000 da0c 6765  ..r(...r).....ge
-00001b30: 745f 6d65 7461 6461 7461 0901 0000 7302  t_metadata....s.
-00001b40: 0000 0004 017a 1547 7269 7374 4150 492e  .....z.GristAPI.
-00001b50: 6765 745f 6d65 7461 6461 7461 6303 0000  get_metadatac...
-00001b60: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00001b70: 004b 0000 0073 7e00 0000 7c00 6a00 7230  .K...s~...|.j.r0
-00001b80: 7c00 6a01 721d 7402 a003 6401 7c00 6a00  |.j.r.t...d.|.j.
-00001b90: 9b02 6402 7c00 6a01 9b00 9d04 a101 0100  ..d.|.j.........
-00001ba0: 7c00 6a04 7c01 7c02 6602 6900 7c03 a401  |.j.|.|.f.i.|...
-00001bb0: 8e01 5300 7402 a003 6403 7c00 6a00 9b02  ..S.t...d.|.j...
-00001bc0: 9d02 a101 0100 7c00 6a05 7c01 7c02 6602  ......|.j.|.|.f.
-00001bd0: 6900 7c03 a401 8e01 5300 7402 a003 6404  i.|.....S.t...d.
-00001be0: a101 0100 7c00 6a06 7c01 7c02 6602 6900  ....|.j.|.|.f.i.
-00001bf0: 7c03 a401 8e01 5300 2905 4e7a 2167 6574  |.....S.).Nz!get
-00001c00: 5f72 6f77 7320 6665 7463 685f 7461 626c  _rows fetch_tabl
-00001c10: 6520 7365 6c66 2e64 6f63 5f69 643d da01  e self.doc_id=..
-00001c20: 207a 2567 6574 5f72 6f77 7320 6665 7463   z%get_rows fetc
-00001c30: 685f 7461 626c 655f 6964 7320 7365 6c66  h_table_ids self
-00001c40: 2e64 6f63 5f69 643d 7a17 6765 745f 726f  .doc_id=z.get_ro
-00001c50: 7773 2066 6574 6368 5f64 6f63 735f 6964  ws fetch_docs_id
-00001c60: 7329 0772 4300 0000 7240 0000 0072 2100  s).rC...r@...r!.
-00001c70: 0000 7222 0000 0072 7e00 0000 728d 0000  ..r"...r~...r...
-00001c80: 0072 9400 0000 2904 724b 0000 0072 7d00  .r....).rK...r}.
-00001c90: 0000 7256 0000 0072 1e00 0000 7228 0000  ..rV...r....r(..
-00001ca0: 0072 2800 0000 7229 0000 00da 0867 6574  .r(...r).....get
-00001cb0: 5f72 6f77 730c 0100 0073 1000 0000 0606  _rows....s......
-00001cc0: 0601 1a01 1401 1202 1401 0a02 1401 7a11  ..............z.
-00001cd0: 4772 6973 7441 5049 2e67 6574 5f72 6f77  GristAPI.get_row
-00001ce0: 7329 0154 2903 4e4e 4e29 0272 1f00 0000  s).T).NNN).r....
-00001cf0: 4e29 1fda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00001d00: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00001d10: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00001d20: da04 7361 6665 da0c 7374 6174 6963 6d65  ..safe..staticme
-00001d30: 7468 6f64 7281 0000 00da 0462 6f6f 6c72  thodr......boolr
-00001d40: 0400 0000 7208 0000 0072 2a00 0000 7209  ....r....r*...r.
-00001d50: 0000 0072 2c00 0000 723b 0000 0072 4800  ...r,...r;...rH.
-00001d60: 0000 7205 0000 0072 0e00 0000 7249 0000  ..r....r....rI..
-00001d70: 0072 4a00 0000 7213 0000 0072 0700 0000  .rJ...r....r....
-00001d80: 7215 0000 0072 0600 0000 7216 0000 0072  r....r....r....r
-00001d90: 7e00 0000 728d 0000 0072 9400 0000 7295  ~...r....r....r.
-00001da0: 0000 0072 9600 0000 7298 0000 00da 0d5f  ...r....r......_
-00001db0: 5f63 6c61 7373 6365 6c6c 5f5f 7228 0000  _classcell__r(..
-00001dc0: 0072 2800 0000 724e 0000 0072 2900 0000  .r(...rN...r)...
-00001dd0: 721b 0000 0039 0000 0073 6800 0000 0800  r....9...sh.....
-00001de0: 0401 0405 0202 2201 0206 1801 0206 0201  ......".........
-00001df0: 0201 04fb 0202 02fe 0603 02fd 0604 02fc  ................
-00001e00: 0605 0efb 0a2a 1630 1605 020c 0a02 02fe  .....*.0........
-00001e10: 0e03 02fd 0605 0afb 0221 0a02 02fe 0e03  .........!......
-00001e20: 02fd 0605 0afb 0212 0a02 02fe 0e03 02fd  ................
-00001e30: 0605 0afb 161c 1603 0203 0a02 02fe 0e03  ................
-00001e40: 02fd 0605 12fb 721b 0000 0029 3072 9c00  ......r....)0r..
-00001e50: 0000 7203 0000 0072 0200 0000 da06 7479  ..r....r......ty
-00001e60: 7069 6e67 7204 0000 0072 0500 0000 7206  pingr....r....r.
-00001e70: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00001e80: 0000 da07 6c6f 6767 696e 67da 026f 73da  ....logging..os.
-00001e90: 0c75 726c 6c69 622e 7061 7273 6572 2300  .urllib.parser#.
-00001ea0: 0000 726d 0000 0072 4500 0000 da18 7368  ..rm...rE.....sh
-00001eb0: 696c 6c65 6c61 6768 2e61 6461 7074 6572  illelagh.adapter
-00001ec0: 732e 6261 7365 720a 0000 00da 1173 6869  s.baser......shi
-00001ed0: 6c6c 656c 6167 682e 6669 656c 6473 720b  llelagh.fieldsr.
-00001ee0: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00001ef0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00001f00: 0072 1200 0000 da12 7368 696c 6c65 6c61  .r......shillela
-00001f10: 6768 2e66 696c 7465 7273 7213 0000 0072  gh.filtersr....r
-00001f20: 1400 0000 da11 7368 696c 6c65 6c61 6768  ......shillelagh
-00001f30: 2e74 7970 696e 6772 1500 0000 7216 0000  .typingr....r...
-00001f40: 00da 0967 6574 4c6f 6767 6572 7221 0000  ...getLoggerr!..
-00001f50: 00da 0667 6574 656e 76da 056c 6f77 6572  ...getenv..lower
-00001f60: da0b 6261 7369 6343 6f6e 6669 6772 1700  ..basicConfigr..
-00001f70: 0000 da0d 5374 7265 616d 4861 6e64 6c65  ....StreamHandle
-00001f80: 72da 0e73 7464 6f75 745f 6861 6e64 6c65  r..stdout_handle
-00001f90: 72da 0873 6574 4c65 7665 6cda 0946 6f72  r..setLevel..For
-00001fa0: 6d61 7474 6572 da09 666f 726d 6174 7465  matter..formatte
-00001fb0: 72da 0c73 6574 466f 726d 6174 7465 72da  r..setFormatter.
-00001fc0: 0a61 6464 4861 6e64 6c65 72da 0545 5252  .addHandler..ERR
-00001fd0: 4f52 721b 0000 0072 2800 0000 7228 0000  ORr....r(...r(..
-00001fe0: 0072 2800 0000 7229 0000 00da 083c 6d6f  .r(...r).....<mo
-00001ff0: 6475 6c65 3e01 0000 0073 2c00 0000 0401  dule>....s,.....
-00002000: 1003 2004 0808 0801 0801 0802 0801 0c02  .. .............
-00002010: 2801 100a 1004 0805 1c02 0e01 0801 0c01  (...............
-00002020: 0a01 0a01 0c01 0e02 1403                 ..........
+00000080: 5a0e 6401 6404 6c0f 5a0f 6405 6406 6c10  Z.d.d.l.Z.d.d.l.
+00000090: 6d11 5a11 0100 6401 6407 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
+000000a0: 0100 6401 6408 6c14 6d15 5a15 6d16 5a16  ..d.d.l.m.Z.m.Z.
+000000b0: 6d17 5a17 6d18 5a18 6d19 5a19 6d1a 5a1a  m.Z.m.Z.m.Z.m.Z.
+000000c0: 6d1b 5a1b 6d1c 5a1c 0100 6401 6409 6c1d  m.Z.m.Z...d.d.l.
+000000d0: 6d1e 5a1e 6d1f 5a1f 0100 6401 640a 6c20  m.Z.m.Z...d.d.l 
+000000e0: 6d21 5a21 6d22 5a22 0100 650a a023 a100  m!Z!m"Z"..e..#..
+000000f0: 5a24 650b a025 640b a101 7291 650b a025  Z$e..%d...r.e..%
+00000100: 640b a101 a026 a100 640c 7600 7291 650a  d....&..d.v.r.e.
+00000110: 6a27 650a 6a28 640d 8d01 0100 650a a029  j'e.j(d.....e..)
+00000120: a100 5a2a 652a a02b 650a 6a28 a101 0100  ..Z*e*.+e.j(....
+00000130: 650a a02c 640e a101 5a2d 652a a02e 652d  e..,d...Z-e*..e-
+00000140: a101 0100 6524 a02f 652a a101 0100 6e07  ....e$./e*....n.
+00000150: 650a 6a27 650a 6a30 640d 8d01 0100 4700  e.j'e.j0d.....G.
+00000160: 640f 6410 8400 6410 6513 8303 5a31 6404  d.d...d.e...Z1d.
+00000170: 5300 2911 7a1f 0a41 6e20 6164 6170 7465  S.).z..An adapte
+00000180: 7220 666f 7220 7468 6520 4772 6973 7420  r for the Grist 
+00000190: 4150 492e 0ae9 0000 0000 2902 da04 6461  API.......)...da
+000001a0: 7465 da08 6461 7465 7469 6d65 2906 da03  te..datetime)...
+000001b0: 416e 79da 0444 6963 74da 0849 7465 7261  Any..Dict..Itera
+000001c0: 746f 72da 044c 6973 74da 084f 7074 696f  tor..List..Optio
+000001d0: 6e61 6cda 0554 7570 6c65 4ee9 0100 0000  nal..TupleN.....
+000001e0: 2901 da15 7265 7175 6573 745f 6361 6368  )...request_cach
+000001f0: 655f 6261 636b 656e 6429 01da 0741 6461  e_backend)...Ada
+00000200: 7074 6572 2908 da07 426f 6f6c 6561 6eda  pter)...Boolean.
+00000210: 0444 6174 65da 0844 6174 6554 696d 65da  .Date..DateTime.
+00000220: 0546 6965 6c64 da05 466c 6f61 74da 0749  .Field..Float..I
+00000230: 6e74 6567 6572 da05 4f72 6465 72da 0653  nteger..Order..S
+00000240: 7472 696e 6729 02da 0646 696c 7465 72da  tring)...Filter.
+00000250: 0552 616e 6765 2902 da0e 5265 7175 6573  .Range)...Reques
+00000260: 7465 644f 7264 6572 da03 526f 77da 0544  tedOrder..Row..D
+00000270: 4542 5547 2902 da04 7472 7565 da01 3129  EBUG)...true..1)
+00000280: 01da 056c 6576 656c 7a29 2528 6173 6374  ...levelz)%(asct
+00000290: 696d 6529 7320 2d20 2528 6c65 7665 6c6e  ime)s - %(leveln
+000002a0: 616d 6529 7320 2d20 2528 6d65 7373 6167  ame)s - %(messag
+000002b0: 6529 7363 0000 0000 0000 0000 0000 0000  e)sc............
+000002c0: 0000 0000 0b00 0000 0000 0000 73a2 0100  ............s...
+000002d0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+000002e0: 0465 0564 2564 0365 0664 0465 0764 0565  .e.d%d.e.d.e.d.e
+000002f0: 0864 0665 0965 0719 0066 0864 0764 0884  .d.e.e...f.d.d..
+00000300: 0583 015a 0a65 0564 0365 0664 0665 0b65  ...Z.e.d.e.d.e.e
+00000310: 0619 0066 0464 0964 0a84 0483 015a 0c09  ...f.d.d.....Z..
+00000320: 0b09 0b09 0b64 2664 0365 0664 0c65 0965  .....d&d.e.d.e.e
+00000330: 0619 0064 0d65 0965 0619 0064 0e65 0965  ...d.e.e...d.e.e
+00000340: 0619 0066 0887 0066 0164 0f64 1084 0d5a  ...f...f.d.d...Z
+00000350: 0d64 2764 1164 1284 045a 0e64 0665 0f65  .d'd.d...Z.d.e.e
+00000360: 0665 1066 0219 0066 0264 1364 1484 045a  .e.f...f.d.d...Z
+00000370: 1164 0665 0f65 0665 1066 0219 0066 0264  .d.e.e.e.f...f.d
+00000380: 1564 1684 045a 1264 1765 0f65 0665 1366  .d...Z.d.e.e.e.f
+00000390: 0219 0064 1865 1465 0b65 0665 1566 0219  ...d.e.e.e.e.f..
+000003a0: 0019 0064 0665 1665 1719 0066 0664 1964  ...d.e.e...f.d.d
+000003b0: 1a84 045a 1864 1765 0f65 0665 1366 0219  ...Z.d.e.e.e.f..
+000003c0: 0064 1865 1465 0b65 0665 1566 0219 0019  .d.e.e.e.e.f....
+000003d0: 0064 0665 1665 1719 0066 0664 1b64 1c84  .d.e.e...f.d.d..
+000003e0: 045a 1964 1765 0f65 0665 1366 0219 0064  .Z.d.e.e.e.f...d
+000003f0: 1865 1465 0b65 0665 1566 0219 0019 0064  .e.e.e.e.f.....d
+00000400: 0665 1665 1719 0066 0664 1d64 1e84 045a  .e.e...f.d.d...Z
+00000410: 1a64 0665 0f65 0665 1066 0219 0066 0264  .d.e.e.e.f...f.d
+00000420: 1f64 2084 045a 1b64 0665 0f65 0665 0866  .d ..Z.d.e.e.e.f
+00000430: 0219 0066 0264 2164 2284 045a 1c64 1765  ...f.d!d"..Z.d.e
+00000440: 0f65 0665 1366 0219 0064 1865 1465 0b65  .e.e.f...d.e.e.e
+00000450: 0665 1566 0219 0019 0064 0665 1665 1719  .e.f.....d.e.e..
+00000460: 0066 0664 2364 2484 045a 1d87 0004 005a  .f.d#d$..Z.....Z
+00000470: 1e53 0029 28da 0847 7269 7374 4150 497a  .S.)(..GristAPIz
+00000480: 270a 2020 2020 416e 2061 6461 7074 6572  '.    An adapter
+00000490: 2066 6f72 2074 6865 2047 7269 7374 2041   for the Grist A
+000004a0: 5049 2e0a 2020 2020 54da 0375 7269 da04  PI..    T..uri..
+000004b0: 6661 7374 da06 6b77 6172 6773 da06 7265  fast..kwargs..re
+000004c0: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+000004d0: 0004 0000 0008 0000 004b 0000 0073 4200  .........K...sB.
+000004e0: 0000 7400 a001 6401 7c00 9b02 6402 7c01  ..t...d.|...d.|.
+000004f0: 9b02 6403 7c02 9b02 9d06 a101 0100 7402  ..d.|.........t.
+00000500: 6a03 a004 7c00 a101 7d03 7400 a001 6404  j...|...}.t...d.
+00000510: 7c03 9b02 9d02 a101 0100 7c03 6a05 6405  |.........|.j.d.
+00000520: 6b02 5300 2906 4e7a 0d73 7570 706f 7274  k.S.).Nz.support
+00000530: 7320 7572 693d 7a06 2066 6173 743d 7a08  s uri=z. fast=z.
+00000540: 206b 7761 7267 733d 7a10 7375 7070 6f72   kwargs=z.suppor
+00000550: 7473 2070 6172 7365 643d da05 6772 6973  ts parsed=..gris
+00000560: 7429 06da 066c 6f67 6765 72da 0564 6562  t)...logger..deb
+00000570: 7567 da06 7572 6c6c 6962 da05 7061 7273  ug..urllib..pars
+00000580: 65da 0875 726c 7061 7273 65da 0673 6368  e..urlparse..sch
+00000590: 656d 6529 0472 1e00 0000 721f 0000 0072  eme).r....r....r
+000005a0: 2000 0000 da06 7061 7273 6564 a900 722a   .....parsed..r*
+000005b0: 0000 00fa 522f 686f 6d65 2f71 6c65 726f  ....R/home/qlero
+000005c0: 792f 6772 6973 742f 7368 696c 6c65 6c61  y/grist/shillela
+000005d0: 6768 2f73 6869 6c6c 656c 6167 682d 6772  gh/shillelagh-gr
+000005e0: 6973 7461 7069 2f73 7263 2f73 6869 6c6c  istapi/src/shill
+000005f0: 656c 6167 685f 6772 6973 7461 7069 2f67  elagh_gristapi/g
+00000600: 7269 7374 2e70 79da 0873 7570 706f 7274  rist.py..support
+00000610: 7343 0000 0073 0800 0000 1c02 0c01 1001  sC...s..........
+00000620: 0a01 7a11 4772 6973 7441 5049 2e73 7570  ..z.GristAPI.sup
+00000630: 706f 7274 7363 0100 0000 0000 0000 0000  portsc..........
+00000640: 0000 0100 0000 0100 0000 4300 0000 7306  ..........C...s.
+00000650: 0000 007c 0066 0153 00a9 014e 722a 0000  ...|.f.S...Nr*..
+00000660: 0029 0172 1e00 0000 722a 0000 0072 2a00  .).r....r*...r*.
+00000670: 0000 722b 0000 00da 0970 6172 7365 5f75  ..r+.....parse_u
+00000680: 7269 4a00 0000 7302 0000 0006 027a 1247  riJ...s......z.G
+00000690: 7269 7374 4150 492e 7061 7273 655f 7572  ristAPI.parse_ur
+000006a0: 694e da06 6f72 675f 6964 da06 7365 7276  iN..org_id..serv
+000006b0: 6572 da07 6170 695f 6b65 7963 0500 0000  er..api_keyc....
+000006c0: 0000 0000 0000 0000 0900 0000 0500 0000  ................
+000006d0: 0300 0000 73fa 0000 0074 0083 00a0 01a1  ....s....t......
+000006e0: 0001 0074 026a 03a0 047c 01a1 017d 0574  ...t.j...|...}.t
+000006f0: 026a 03a0 057c 056a 06a1 017d 067c 056a  .j...|.j...}.|.j
+00000700: 07a0 0864 01a1 017d 0764 007c 005f 0974  ...d...}.d.|._.t
+00000710: 0a7c 0783 0164 026b 0472 267c 0764 0219  .|...d.k.r&|.d..
+00000720: 007c 005f 097c 056a 0b7c 005f 0c74 0da0  .|._.|.j.|._.t..
+00000730: 0e64 037c 006a 0c9b 029d 02a1 0101 007c  .d.|.j.........|
+00000740: 0473 3b7c 0664 0419 0064 0519 007d 047c  .s;|.d...d...}.|
+00000750: 0373 437c 0664 0619 0064 0519 007d 037c  .sC|.d...d...}.|
+00000760: 0273 4b7c 0664 0719 0064 0519 007d 027c  .sK|.d...d...}.|
+00000770: 027c 005f 0f64 0864 097c 049b 009d 0269  .|._.d.d.|.....i
+00000780: 017c 005f 107c 037c 005f 1174 1283 007d  .|._.|.|._.t...}
+00000790: 0874 136a 1464 0a7c 0864 0b64 0c8d 037c  .t.j.d.|.d.d...|
+000007a0: 005f 157c 006a 0c72 777c 006a 0972 717c  ._.|.j.rw|.j.rq|
+000007b0: 00a0 16a1 0001 0064 0053 007c 00a0 17a1  .......d.S.|....
+000007c0: 0001 0064 0053 007c 00a0 18a1 0001 0064  ...d.S.|.......d
+000007d0: 0053 0029 0d4e fa01 2f72 0a00 0000 7a15  .S.).N../r....z.
+000007e0: 5f5f 696e 6974 5f5f 2073 656c 662e 646f  __init__ self.do
+000007f0: 635f 6964 3dda 036b 6579 7201 0000 0072  c_id=..keyr....r
+00000800: 3000 0000 722f 0000 00da 0d41 7574 686f  0...r/.....Autho
+00000810: 7269 7a61 7469 6f6e 7a07 4265 6172 6572  rizationz.Bearer
+00000820: 205a 0b67 7269 7374 5f63 6163 6865 e9b4   Z.grist_cache..
+00000830: 0000 0029 03da 0a63 6163 6865 5f6e 616d  ...)...cache_nam
+00000840: 65da 0762 6163 6b65 6e64 da0c 6578 7069  e..backend..expi
+00000850: 7265 5f61 6674 6572 2919 da05 7375 7065  re_after)...supe
+00000860: 72da 085f 5f69 6e69 745f 5f72 2500 0000  r..__init__r%...
+00000870: 7226 0000 0072 2700 0000 da08 7061 7273  r&...r'.....pars
+00000880: 655f 7173 da05 7175 6572 79da 0470 6174  e_qs..query..pat
+00000890: 68da 0573 706c 6974 da08 7461 626c 655f  h..split..table_
+000008a0: 6964 da03 6c65 6eda 066e 6574 6c6f 63da  id..len..netloc.
+000008b0: 0664 6f63 5f69 6472 2300 0000 7224 0000  .doc_idr#...r$..
+000008c0: 0072 2f00 0000 da07 6865 6164 6572 7372  .r/.....headersr
+000008d0: 3000 0000 720b 0000 00da 0e72 6571 7565  0...r......reque
+000008e0: 7374 735f 6361 6368 65da 0d43 6163 6865  sts_cache..Cache
+000008f0: 6453 6573 7369 6f6e da08 5f73 6573 7369  dSession.._sessi
+00000900: 6f6e da11 5f73 6574 5f63 6f6c 756d 6e73  on.._set_columns
+00000910: 5f64 6174 61da 135f 7365 745f 636f 6c75  _data.._set_colu
+00000920: 6d6e 735f 7461 626c 6573 da11 5f73 6574  mns_tables.._set
+00000930: 5f63 6f6c 756d 6e73 5f64 6f63 7329 09da  _columns_docs)..
+00000940: 0473 656c 6672 1e00 0000 722f 0000 0072  .selfr....r/...r
+00000950: 3000 0000 7231 0000 0072 2900 0000 da0c  0...r1...r).....
+00000960: 7175 6572 795f 7374 7269 6e67 5a0a 7370  query_stringZ.sp
+00000970: 6c69 745f 7061 7468 7237 0000 00a9 01da  lit_pathr7......
+00000980: 095f 5f63 6c61 7373 5f5f 722a 0000 0072  .__class__r*...r
+00000990: 2b00 0000 723a 0000 004e 0000 0073 3a00  +...r:...N...s:.
+000009a0: 0000 0a07 0c02 0e01 0c02 0601 0c01 0a01  ................
+000009b0: 0801 1201 0401 0c01 0401 0c01 0401 0c01  ................
+000009c0: 0601 1001 0601 0602 0401 0201 0201 0201  ................
+000009d0: 08fd 0606 0601 0c01 0c02 0c02 7a11 4772  ............z.Gr
+000009e0: 6973 7441 5049 2e5f 5f69 6e69 745f 5f63  istAPI.__init__c
+000009f0: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00000a00: 0600 0000 0300 0000 73b2 0000 0074 00a0  ........s....t..
+00000a10: 0164 017c 006a 029b 029d 02a1 0101 007c  .d.|.j.........|
+00000a20: 006a 039b 0064 027c 006a 049b 0064 037c  .j...d.|.j...d.|
+00000a30: 006a 029b 0064 049d 067d 0174 056a 067c  .j...d...}.t.j.|
+00000a40: 017c 006a 0764 058d 027d 027c 02a0 08a1  .|.j.d...}.|....
+00000a50: 0064 0619 007d 0364 0764 0884 0089 0087  .d...}.d.d......
+00000a60: 0066 0164 0964 0a84 087c 0344 0083 017d  .f.d.d...|.D...}
+00000a70: 0464 0b64 0c84 007c 0444 0083 017c 005f  .d.d...|.D...|._
+00000a80: 0964 0d64 0c84 007c 006a 09a0 0aa1 0044  .d.d...|.j.....D
+00000a90: 0083 017c 005f 0b74 0c74 0d6a 0e64 0e8d  ...|._.t.t.j.d..
+00000aa0: 017c 006a 0964 0f3c 0074 00a0 0164 107c  .|.j.d.<.t...d.|
+00000ab0: 006a 099b 029d 02a1 0101 0064 1153 0029  .j.........d.S.)
+00000ac0: 127a 810a 2020 2020 2020 2020 4361 6c6c  .z..        Call
+00000ad0: 2074 6f0a 2020 2020 2020 2020 6874 7470   to.        http
+00000ae0: 733a 2f2f 7375 7070 6f72 742e 6765 7467  s://support.getg
+00000af0: 7269 7374 2e63 6f6d 2f61 7069 2f23 7461  rist.com/api/#ta
+00000b00: 672f 636f 6c75 6d6e 732f 6f70 6572 6174  g/columns/operat
+00000b10: 696f 6e2f 6c69 7374 436f 6c75 6d6e 730a  ion/listColumns.
+00000b20: 2020 2020 2020 2020 746f 2073 6574 2063          to set c
+00000b30: 6f6c 756d 6e20 7479 7065 730a 2020 2020  olumn types.    
+00000b40: 2020 2020 7a20 5f73 6574 5f63 6f6c 756d      z _set_colum
+00000b50: 6e73 5f64 6174 6120 7365 6c66 2e74 6162  ns_data self.tab
+00000b60: 6c65 5f69 643d fa0a 2f61 7069 2f64 6f63  le_id=../api/doc
+00000b70: 732f fa08 2f74 6162 6c65 732f 7a08 2f63  s/../tables/z./c
+00000b80: 6f6c 756d 6e73 a901 7243 0000 00da 0763  olumns..rC.....c
+00000b90: 6f6c 756d 6e73 6301 0000 0000 0000 0000  olumnsc.........
+00000ba0: 0000 0001 0000 0005 0000 0053 0000 0073  ...........S...s
+00000bb0: 0a01 0000 7c00 6401 6b02 720a 7400 7401  ....|.d.k.r.t.t.
+00000bc0: 6a02 6402 8d01 5300 7c00 6403 6b02 7214  j.d...S.|.d.k.r.
+00000bd0: 7403 7401 6a02 6402 8d01 5300 7c00 6404  t.t.j.d...S.|.d.
+00000be0: 6b02 721e 7404 7401 6a02 6402 8d01 5300  k.r.t.t.j.d...S.
+00000bf0: 7c00 6405 6b02 7228 7405 7401 6a02 6402  |.d.k.r(t.t.j.d.
+00000c00: 8d01 5300 7c00 6406 6b02 7232 7400 7401  ..S.|.d.k.r2t.t.
+00000c10: 6a02 6402 8d01 5300 7c00 6407 6b02 723c  j.d...S.|.d.k.r<
+00000c20: 7400 7401 6a02 6402 8d01 5300 7c00 6408  t.t.j.d...S.|.d.
+00000c30: 6b02 7249 7406 7407 6701 6409 7401 6a02  k.rIt.t.g.d.t.j.
+00000c40: 640a 8d03 5300 7c00 a008 640b a101 7257  d...S.|...d...rW
+00000c50: 7409 7407 6701 6409 7401 6a02 640a 8d03  t.t.g.d.t.j.d...
+00000c60: 5300 7c00 a008 640c a101 7262 7400 7401  S.|...d...rbt.t.
+00000c70: 6a02 6402 8d01 5300 7c00 a008 640d a101  j.d...S.|...d...
+00000c80: 726d 7400 7401 6a02 6402 8d01 5300 7c00  rmt.t.j.d...S.|.
+00000c90: 640e 6b02 7277 7400 7401 6a02 6402 8d01  d.k.rwt.t.j.d...
+00000ca0: 5300 740a a00b 640f 7c00 9b02 9d02 a101  S.t...d.|.......
+00000cb0: 0100 7400 7401 6a02 6402 8d01 5300 2910  ..t.t.j.d...S.).
+00000cc0: 4eda 0454 6578 74a9 01da 056f 7264 6572  N..Text....order
+00000cd0: da03 496e 74da 074e 756d 6572 6963 da04  ..Int..Numeric..
+00000ce0: 426f 6f6c 5a06 4368 6f69 6365 5a0a 4368  BoolZ.ChoiceZ.Ch
+00000cf0: 6f69 6365 4c69 7374 720e 0000 0046 2903  oiceListr....F).
+00000d00: da07 6669 6c74 6572 73da 0565 7861 6374  ..filters..exact
+00000d10: 7254 0000 007a 0944 6174 6554 696d 653a  rT...z.DateTime:
+00000d20: 7a04 5265 663a 7a08 5265 664c 6973 743a  z.Ref:z.RefList:
+00000d30: 5a0b 4174 7461 6368 6d65 6e74 737a 0574  Z.Attachmentsz.t
+00000d40: 7970 653d 290c 7214 0000 0072 1300 0000  ype=).r....r....
+00000d50: da03 414e 5972 1200 0000 7211 0000 0072  ..ANYr....r....r
+00000d60: 0d00 0000 720e 0000 0072 1600 0000 da0a  ....r....r......
+00000d70: 7374 6172 7473 7769 7468 720f 0000 0072  startswithr....r
+00000d80: 2300 0000 7224 0000 0029 01da 0474 7970  #...r$...)...typ
+00000d90: 6572 2a00 0000 722a 0000 0072 2b00 0000  er*...r*...r+...
+00000da0: da07 6765 7474 7970 6585 0000 0073 3000  ..gettype....s0.
+00000db0: 0000 0801 0c01 0801 0c01 0801 0c01 0801  ................
+00000dc0: 0c01 0801 0c01 0801 0c01 0801 1201 0a01  ................
+00000dd0: 1201 0a01 0c01 0a01 0c01 0801 0c01 1002  ................
+00000de0: 0c01 7a2b 4772 6973 7441 5049 2e5f 7365  ..z+GristAPI._se
+00000df0: 745f 636f 6c75 6d6e 735f 6461 7461 2e3c  t_columns_data.<
+00000e00: 6c6f 6361 6c73 3e2e 6765 7474 7970 6563  locals>.gettypec
+00000e10: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000e20: 0600 0000 1300 0000 7324 0000 0067 007c  ........s$...g.|
+00000e30: 005d 0e7d 017c 0164 0019 0088 007c 0164  .].}.|.d.....|.d
+00000e40: 0119 0064 0219 0083 0166 0291 0271 0253  ...d.....f...q.S
+00000e50: 0029 03da 0269 64da 0666 6965 6c64 7372  .)...id..fieldsr
+00000e60: 5c00 0000 722a 0000 0029 02da 022e 30da  \...r*...)....0.
+00000e70: 0163 a901 725d 0000 0072 2a00 0000 722b  .c..r]...r*...r+
+00000e80: 0000 00da 0a3c 6c69 7374 636f 6d70 3ea0  .....<listcomp>.
+00000e90: 0000 0073 0200 0000 2400 7a2e 4772 6973  ...s....$.z.Gris
+00000ea0: 7441 5049 2e5f 7365 745f 636f 6c75 6d6e  tAPI._set_column
+00000eb0: 735f 6461 7461 2e3c 6c6f 6361 6c73 3e2e  s_data.<locals>.
+00000ec0: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+00000ed0: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00000ee0: 0000 0073 1a00 0000 6900 7c00 5d09 7d01  ...s....i.|.].}.
+00000ef0: 7c01 6400 1900 7c01 6401 1900 9302 7102  |.d...|.d.....q.
+00000f00: 5300 2902 7201 0000 0072 0a00 0000 722a  S.).r....r....r*
+00000f10: 0000 0029 0272 6000 0000 da02 6c74 722a  ...).r`.....ltr*
+00000f20: 0000 0072 2a00 0000 722b 0000 00da 0a3c  ...r*...r+.....<
+00000f30: 6469 6374 636f 6d70 3ea1 0000 0073 0200  dictcomp>....s..
+00000f40: 0000 1a00 7a2e 4772 6973 7441 5049 2e5f  ....z.GristAPI._
+00000f50: 7365 745f 636f 6c75 6d6e 735f 6461 7461  set_columns_data
+00000f60: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000f70: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00000f80: 0003 0000 0005 0000 0053 0000 0073 2600  .........S...s&.
+00000f90: 0000 6900 7c00 5d0f 5c02 7d01 7d02 7400  ..i.|.].\.}.}.t.
+00000fa0: 7c02 8301 7401 7402 6602 7600 7202 7c01  |...t.t.f.v.r.|.
+00000fb0: 7c02 9302 7102 5300 722a 0000 0029 0372  |...q.S.r*...).r
+00000fc0: 5c00 0000 720e 0000 0072 0f00 0000 2903  \...r....r....).
+00000fd0: 7260 0000 00da 016b da01 7672 2a00 0000  r`.....k..vr*...
+00000fe0: 722a 0000 0072 2b00 0000 7265 0000 00a2  r*...r+...re....
+00000ff0: 0000 0073 0400 0000 0600 2001 7253 0000  ...s...... .rS..
+00001000: 0072 5e00 0000 7a1f 5f73 6574 5f63 6f6c  .r^...z._set_col
+00001010: 756d 6e73 5f64 6174 6120 7365 6c66 2e63  umns_data self.c
+00001020: 6f6c 756d 6e73 3d4e 290f 7223 0000 0072  olumns=N).r#...r
+00001030: 2400 0000 723f 0000 0072 3000 0000 7242  $...r?...r0...rB
+00001040: 0000 00da 0872 6571 7565 7374 73da 0367  .....requests..g
+00001050: 6574 7243 0000 00da 046a 736f 6e72 5100  etrC.....jsonrQ.
+00001060: 0000 da05 6974 656d 735a 1263 6f6c 756d  ....itemsZ.colum
+00001070: 6e73 5f64 6174 6573 7469 6d65 7372 1200  ns_datestimesr..
+00001080: 0000 7213 0000 0072 5a00 0000 2905 724a  ..r....rZ...).rJ
+00001090: 0000 00da 0375 726c da08 7265 7370 6f6e  .....url..respon
+000010a0: 7365 7251 0000 005a 0a6c 6162 656c 7479  serQ...Z.labelty
+000010b0: 7065 7372 2a00 0000 7262 0000 0072 2b00  pesr*...rb...r+.
+000010c0: 0000 7247 0000 0079 0000 0073 1800 0000  ..rG...y...s....
+000010d0: 1206 1c01 1002 0c01 0802 121b 1001 0601  ................
+000010e0: 0801 08ff 1203 1602 7a1a 4772 6973 7441  ........z.GristA
+000010f0: 5049 2e5f 7365 745f 636f 6c75 6d6e 735f  PI._set_columns_
+00001100: 6461 7461 6301 0000 0000 0000 0000 0000  datac...........
+00001110: 0001 0000 0004 0000 0043 0000 0073 1600  .........C...s..
+00001120: 0000 6401 7400 7401 6a02 6402 8d01 6901  ..d.t.t.j.d...i.
+00001130: 7c00 5f03 6400 5300 2903 4e72 5e00 0000  |._.d.S.).Nr^...
+00001140: 7253 0000 0029 0472 1400 0000 7213 0000  rS...).r....r...
+00001150: 0072 5a00 0000 7251 0000 00a9 0172 4a00  .rZ...rQ.....rJ.
+00001160: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
+00001170: 0072 4800 0000 a900 0000 7304 0000 000c  .rH.......s.....
+00001180: 020a ff7a 1c47 7269 7374 4150 492e 5f73  ...z.GristAPI._s
+00001190: 6574 5f63 6f6c 756d 6e73 5f74 6162 6c65  et_columns_table
+000011a0: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+000011b0: 0000 0a00 0000 4300 0000 735c 0000 0074  ......C...s\...t
+000011c0: 0074 016a 0264 018d 0174 0374 016a 0264  .t.j.d...t.t.j.d
+000011d0: 018d 0174 0374 016a 0264 018d 0174 0374  ...t.t.j.d...t.t
+000011e0: 016a 0264 018d 0174 0374 016a 0264 018d  .j.d...t.t.j.d..
+000011f0: 0174 0374 016a 0264 018d 0174 0374 016a  .t.t.j.d...t.t.j
+00001200: 0264 018d 0174 0374 016a 0264 018d 0164  .d...t.t.j.d...d
+00001210: 029c 087c 005f 0464 0053 0029 034e 7253  ...|._.d.S.).NrS
+00001220: 0000 00a9 0872 5e00 0000 da04 6e61 6d65  .....r^.....name
+00001230: da06 6163 6365 7373 da09 6f72 6744 6f6d  ..access..orgDom
+00001240: 6169 6e72 4200 0000 5a08 646f 635f 6e61  ainrB...Z.doc_na
+00001250: 6d65 5a0d 646f 635f 6372 6561 7465 6441  meZ.doc_createdA
+00001260: 745a 0d64 6f63 5f75 7064 6174 6564 4174  tZ.doc_updatedAt
+00001270: 2905 7212 0000 0072 1300 0000 725a 0000  ).r....r....rZ..
+00001280: 0072 1400 0000 7251 0000 0072 6e00 0000  .r....rQ...rn...
+00001290: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
+000012a0: 4900 0000 ae00 0000 7312 0000 000a 020a  I.......s.......
+000012b0: 010a 010a 010a 010a 010a 010a 010c f87a  ...............z
+000012c0: 1a47 7269 7374 4150 492e 5f73 6574 5f63  .GristAPI._set_c
+000012d0: 6f6c 756d 6e73 5f64 6f63 73da 0662 6f75  olumns_docs..bou
+000012e0: 6e64 7372 5400 0000 6303 0000 0000 0000  ndsrT...c.......
+000012f0: 0000 0000 000c 0000 0006 0000 006b 0000  .............k..
+00001300: 0073 2a01 0000 8100 7400 a001 6401 a101  .s*.....t...d...
+00001310: 0100 7c00 6a02 9b00 6402 7c00 6a03 9b00  ..|.j...d.|.j...
+00001320: 6403 7c00 6a04 9b00 6404 9d06 7d04 7400  d.|.j...d...}.t.
+00001330: a001 6405 7c04 9b02 9d02 a101 0100 7405  ..d.|.........t.
+00001340: 6a06 7c04 7c00 6a07 6406 8d02 7d05 7c05  j.|.|.j.d...}.|.
+00001350: a008 a100 6407 1900 7d06 7c06 4400 5d66  ....d...}.|.D.]f
+00001360: 7d07 7c07 6408 1900 7d08 7400 a001 6409  }.|.d...}.t...d.
+00001370: 7c08 9b02 9d02 a101 0100 7400 a001 640a  |.........t...d.
+00001380: 7c00 6a09 9b02 9d02 a101 0100 6900 7d09  |.j.........i.}.
+00001390: 7c07 640b 1900 7c09 640b 3c00 7c08 a00a  |.d...|.d.<.|...
+000013a0: a100 4400 5d3f 5c02 7d0a 7d0b 740b 7c00  ..D.]?\.}.}.t.|.
+000013b0: 6a09 7c0a 1900 740c 8302 7267 7c0b 640c  j.|...t...rg|.d.
+000013c0: 7501 7267 740d a00e 740f 7c0b 8301 a101  u.rgt...t.|.....
+000013d0: 7d0b 6e23 740b 7c00 6a09 7c0a 1900 7410  }.n#t.|.j.|...t.
+000013e0: 8302 727b 7c0b 640c 7501 727b 7411 a00e  ..r{|.d.u.r{t...
+000013f0: 740f 7c0b 8301 a101 7d0b 6e0f 740b 7c0b  t.|.....}.n.t.|.
+00001400: 7412 8302 728a 640d a013 640e 640f 8400  t...r.d...d.d...
+00001410: 7c0b 4400 8301 a101 7d0b 7c0b 7c09 7c0a  |.D.....}.|.|.|.
+00001420: 3c00 714f 7c09 5600 0100 712c 640c 5300  <.qO|.V...q,d.S.
+00001430: 2910 7a82 0a20 2020 2020 2020 2043 616c  ).z..        Cal
+00001440: 6c20 746f 0a20 2020 2020 2020 2068 7474  l to.        htt
+00001450: 7073 3a2f 2f73 7570 706f 7274 2e67 6574  ps://support.get
+00001460: 6772 6973 742e 636f 6d2f 6170 692f 2374  grist.com/api/#t
+00001470: 6167 2f72 6563 6f72 6473 2f6f 7065 7261  ag/records/opera
+00001480: 7469 6f6e 2f6c 6973 7452 6563 6f72 6473  tion/listRecords
+00001490: 0a20 2020 2020 2020 2059 6965 6c64 7320  .        Yields 
+000014a0: 6120 726f 7720 6f66 2064 6174 610a 2020  a row of data.  
+000014b0: 2020 2020 2020 da0b 6665 7463 685f 7461        ..fetch_ta
+000014c0: 626c 6572 4e00 0000 724f 0000 007a 082f  blerN...rO...z./
+000014d0: 7265 636f 7264 737a 1066 6574 6368 5f74  recordsz.fetch_t
+000014e0: 6162 6c65 2075 726c 3d72 5000 0000 da07  able url=rP.....
+000014f0: 7265 636f 7264 7372 5f00 0000 7a06 6669  recordsr_...z.fi
+00001500: 656c 643d 7a0d 7365 6c66 2e63 6f6c 756d  eld=z.self.colum
+00001510: 6e73 3d72 5e00 0000 4efa 012c 6301 0000  ns=r^...N..,c...
+00001520: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00001530: 0053 0000 0073 1400 0000 6700 7c00 5d06  .S...s....g.|.].
+00001540: 7d01 7400 7c01 8301 9102 7102 5300 722a  }.t.|.....q.S.r*
+00001550: 0000 0029 01da 0373 7472 2902 7260 0000  ...)...str).r`..
+00001560: 00da 0469 7465 6d72 2a00 0000 722a 0000  ...itemr*...r*..
+00001570: 0072 2b00 0000 7263 0000 00d7 0000 0073  .r+...rc.......s
+00001580: 0200 0000 1400 7a28 4772 6973 7441 5049  ......z(GristAPI
+00001590: 2e66 6574 6368 5f74 6162 6c65 2e3c 6c6f  .fetch_table.<lo
+000015a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000015b0: 2914 7223 0000 0072 2400 0000 7230 0000  ).r#...r$...r0..
+000015c0: 0072 4200 0000 723f 0000 0072 6800 0000  .rB...r?...rh...
+000015d0: 7269 0000 0072 4300 0000 726a 0000 0072  ri...rC...rj...r
+000015e0: 5100 0000 726b 0000 00da 0a69 7369 6e73  Q...rk.....isins
+000015f0: 7461 6e63 6572 0e00 0000 7202 0000 00da  tancer....r.....
+00001600: 0d66 726f 6d74 696d 6573 7461 6d70 da03  .fromtimestamp..
+00001610: 696e 7472 0f00 0000 7203 0000 00da 046c  intr....r......l
+00001620: 6973 74da 046a 6f69 6e29 0c72 4a00 0000  ist..join).rJ...
+00001630: 7273 0000 0072 5400 0000 7220 0000 0072  rs...rT...r ...r
+00001640: 6c00 0000 726d 0000 0072 7500 0000 da06  l...rm...ru.....
+00001650: 7265 636f 7264 da05 6669 656c 64da 0166  record..field..f
+00001660: 7266 0000 0072 6700 0000 722a 0000 0072  rf...rg...r*...r
+00001670: 2a00 0000 722b 0000 0072 7400 0000 ba00  *...r+...rt.....
+00001680: 0000 732c 0000 0002 800a 0b1c 0110 0110  ..s,............
+00001690: 020c 0108 0108 0110 0112 0104 010c 0110  ................
+000016a0: 0118 0110 0118 0110 010a 0114 010a 0108  ................
+000016b0: 0104 f27a 1447 7269 7374 4150 492e 6665  ...z.GristAPI.fe
+000016c0: 7463 685f 7461 626c 6563 0300 0000 0000  tch_tablec......
+000016d0: 0000 0000 0000 0800 0000 0400 0000 6b00  ..............k.
+000016e0: 0000 734e 0000 0081 007c 006a 009b 0064  ..sN.....|.j...d
+000016f0: 017c 006a 019b 0064 029d 047d 0474 026a  .|.j...d...}.t.j
+00001700: 037c 047c 006a 0464 038d 027d 057c 05a0  .|.|.j.d...}.|..
+00001710: 05a1 0064 0419 007d 067c 0644 005d 097d  ...d...}.|.D.].}
+00001720: 0764 057c 0764 0519 0069 0156 0001 0071  .d.|.d...i.V...q
+00001730: 1b64 0653 0029 077a 7d0a 2020 2020 2020  .d.S.).z}.      
+00001740: 2020 4361 6c6c 2074 6f0a 2020 2020 2020    Call to.      
+00001750: 2020 6874 7470 733a 2f2f 7375 7070 6f72    https://suppor
+00001760: 742e 6765 7467 7269 7374 2e63 6f6d 2f61  t.getgrist.com/a
+00001770: 7069 2f23 7461 672f 7461 626c 6573 2f6f  pi/#tag/tables/o
+00001780: 7065 7261 7469 6f6e 2f6c 6973 7454 6162  peration/listTab
+00001790: 6c65 730a 2020 2020 2020 2020 5969 656c  les.        Yiel
+000017a0: 6473 2061 2074 6162 6c65 5f69 640a 2020  ds a table_id.  
+000017b0: 2020 2020 2020 724e 0000 007a 072f 7461        rN...z./ta
+000017c0: 626c 6573 7250 0000 00da 0674 6162 6c65  blesrP.....table
+000017d0: 7372 5e00 0000 4e29 0672 3000 0000 7242  sr^...N).r0...rB
+000017e0: 0000 0072 6800 0000 7269 0000 0072 4300  ...rh...ri...rC.
+000017f0: 0000 726a 0000 0029 0872 4a00 0000 7273  ..rj...).rJ...rs
+00001800: 0000 0072 5400 0000 7220 0000 0072 6c00  ...rT...r ...rl.
+00001810: 0000 726d 0000 0072 8100 0000 da05 7461  ..rm...r......ta
+00001820: 626c 6572 2a00 0000 722a 0000 0072 2b00  bler*...r*...r+.
+00001830: 0000 da0f 6665 7463 685f 7461 626c 655f  ....fetch_table_
+00001840: 6964 73db 0000 0073 0e00 0000 0280 140b  ids....s........
+00001850: 1002 0c01 0801 1001 04ff 7a18 4772 6973  ..........z.Gris
+00001860: 7441 5049 2e66 6574 6368 5f74 6162 6c65  tAPI.fetch_table
+00001870: 5f69 6473 6303 0000 0000 0000 0000 0000  _idsc...........
+00001880: 0009 0000 000b 0000 006b 0000 0073 8200  .........k...s..
+00001890: 0000 8100 7c00 6a00 9b00 6401 7c00 6a01  ....|.j...d.|.j.
+000018a0: 9b00 6402 9d04 7d04 7402 6a03 7c04 7c00  ..d...}.t.j.|.|.
+000018b0: 6a04 6403 8d02 7d05 7c05 a005 a100 7d06  j.d...}.|.....}.
+000018c0: 7c06 4400 5d25 7d07 7c07 6404 1900 4400  |.D.]%}.|.d...D.
+000018d0: 5d1e 7d08 7c07 6405 1900 7c07 6406 1900  ].}.|.d...|.d...
+000018e0: 7c07 6407 1900 7c07 6408 1900 7c08 6405  |.d...|.d...|.d.
+000018f0: 1900 7c08 6406 1900 7c08 6409 1900 7c08  ..|.d...|.d...|.
+00001900: 640a 1900 640b 9c08 5600 0100 711f 7119  d...d...V...q.q.
+00001910: 640c 5300 290d 7a83 0a20 2020 2020 2020  d.S.).z..       
+00001920: 2043 616c 6c20 746f 0a20 2020 2020 2020   Call to.       
+00001930: 2068 7474 7073 3a2f 2f73 7570 706f 7274   https://support
+00001940: 2e67 6574 6772 6973 742e 636f 6d2f 6170  .getgrist.com/ap
+00001950: 692f 2374 6167 2f77 6f72 6b73 7061 6365  i/#tag/workspace
+00001960: 732f 6f70 6572 6174 696f 6e2f 6c69 7374  s/operation/list
+00001970: 576f 726b 7370 6163 6573 0a20 2020 2020  Workspaces.     
+00001980: 2020 2059 6965 6c64 7320 6120 646f 635f     Yields a doc_
+00001990: 6964 0a20 2020 2020 2020 207a 0a2f 6170  id.        z./ap
+000019a0: 692f 6f72 6773 2f7a 0b2f 776f 726b 7370  i/orgs/z./worksp
+000019b0: 6163 6573 7250 0000 00da 0464 6f63 7372  acesrP.....docsr
+000019c0: 5e00 0000 7270 0000 0072 7100 0000 7272  ^...rp...rq...rr
+000019d0: 0000 005a 0963 7265 6174 6564 4174 5a09  ...Z.createdAtZ.
+000019e0: 7570 6461 7465 6441 7472 6f00 0000 4e29  updatedAtro...N)
+000019f0: 0672 3000 0000 722f 0000 0072 6800 0000  .r0...r/...rh...
+00001a00: 7269 0000 0072 4300 0000 726a 0000 0029  ri...rC...rj...)
+00001a10: 0972 4a00 0000 7273 0000 0072 5400 0000  .rJ...rs...rT...
+00001a20: 7220 0000 0072 6c00 0000 726d 0000 005a  r ...rl...rm...Z
+00001a30: 0a77 6f72 6b73 7061 6365 735a 0977 6f72  .workspacesZ.wor
+00001a40: 6b73 7061 6365 da03 646f 6372 2a00 0000  kspace..docr*...
+00001a50: 722a 0000 0072 2b00 0000 da0e 6665 7463  r*...r+.....fetc
+00001a60: 685f 646f 6373 5f69 6473 ed00 0000 7322  h_docs_ids....s"
+00001a70: 0000 0002 8014 0b10 0208 0108 010c 0106  ................
+00001a80: 0206 0106 0106 0106 0106 0106 0106 010a  ................
+00001a90: f802 ff04 ff7a 1747 7269 7374 4150 492e  .....z.GristAPI.
+00001aa0: 6665 7463 685f 646f 6373 5f69 6473 6301  fetch_docs_idsc.
+00001ab0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00001ac0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+00001ad0: 5300 722d 0000 0029 0172 5100 0000 726e  S.r-...).rQ...rn
+00001ae0: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
+00001af0: 0000 da0b 6765 745f 636f 6c75 6d6e 7309  ....get_columns.
+00001b00: 0100 0073 0200 0000 0601 7a14 4772 6973  ...s......z.Gris
+00001b10: 7441 5049 2e67 6574 5f63 6f6c 756d 6e73  tAPI.get_columns
+00001b20: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001b30: 0001 0000 0043 0000 0073 0400 0000 6900  .....C...s....i.
+00001b40: 5300 722d 0000 0072 2a00 0000 726e 0000  S.r-...r*...rn..
+00001b50: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
+00001b60: da0c 6765 745f 6d65 7461 6461 7461 0c01  ..get_metadata..
+00001b70: 0000 7302 0000 0004 017a 1547 7269 7374  ..s......z.Grist
+00001b80: 4150 492e 6765 745f 6d65 7461 6461 7461  API.get_metadata
+00001b90: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00001ba0: 0006 0000 004b 0000 0073 7e00 0000 7c00  .....K...s~...|.
+00001bb0: 6a00 7230 7c00 6a01 721d 7402 a003 6401  j.r0|.j.r.t...d.
+00001bc0: 7c00 6a00 9b02 6402 7c00 6a01 9b00 9d04  |.j...d.|.j.....
+00001bd0: a101 0100 7c00 6a04 7c01 7c02 6602 6900  ....|.j.|.|.f.i.
+00001be0: 7c03 a401 8e01 5300 7402 a003 6403 7c00  |.....S.t...d.|.
+00001bf0: 6a00 9b02 9d02 a101 0100 7c00 6a05 7c01  j.........|.j.|.
+00001c00: 7c02 6602 6900 7c03 a401 8e01 5300 7402  |.f.i.|.....S.t.
+00001c10: a003 6404 a101 0100 7c00 6a06 7c01 7c02  ..d.....|.j.|.|.
+00001c20: 6602 6900 7c03 a401 8e01 5300 2905 4e7a  f.i.|.....S.).Nz
+00001c30: 2167 6574 5f72 6f77 7320 6665 7463 685f  !get_rows fetch_
+00001c40: 7461 626c 6520 7365 6c66 2e64 6f63 5f69  table self.doc_i
+00001c50: 643d da01 207a 2567 6574 5f72 6f77 7320  d=.. z%get_rows 
+00001c60: 6665 7463 685f 7461 626c 655f 6964 7320  fetch_table_ids 
+00001c70: 7365 6c66 2e64 6f63 5f69 643d 7a17 6765  self.doc_id=z.ge
+00001c80: 745f 726f 7773 2066 6574 6368 5f64 6f63  t_rows fetch_doc
+00001c90: 735f 6964 7329 0772 4200 0000 723f 0000  s_ids).rB...r?..
+00001ca0: 0072 2300 0000 7224 0000 0072 7400 0000  .r#...r$...rt...
+00001cb0: 7283 0000 0072 8600 0000 2904 724a 0000  r....r....).rJ..
+00001cc0: 0072 7300 0000 7254 0000 0072 2000 0000  .rs...rT...r ...
+00001cd0: 722a 0000 0072 2a00 0000 722b 0000 00da  r*...r*...r+....
+00001ce0: 0867 6574 5f72 6f77 730f 0100 0073 1000  .get_rows....s..
+00001cf0: 0000 0606 0601 1a01 1401 1202 1401 0a02  ................
+00001d00: 1401 7a11 4772 6973 7441 5049 2e67 6574  ..z.GristAPI.get
+00001d10: 5f72 6f77 7329 0154 2903 4e4e 4e29 0272  _rows).T).NNN).r
+00001d20: 2100 0000 4e29 1fda 085f 5f6e 616d 655f  !...N)...__name_
+00001d30: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001d40: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00001d50: 6f63 5f5f da04 7361 6665 da0c 7374 6174  oc__..safe..stat
+00001d60: 6963 6d65 7468 6f64 7277 0000 00da 0462  icmethodrw.....b
+00001d70: 6f6f 6c72 0400 0000 7208 0000 0072 2c00  oolr....r....r,.
+00001d80: 0000 7209 0000 0072 2e00 0000 723a 0000  ..r....r....r:..
+00001d90: 0072 4700 0000 7205 0000 0072 1000 0000  .rG...r....r....
+00001da0: 7248 0000 0072 4900 0000 7215 0000 0072  rH...rI...r....r
+00001db0: 0700 0000 7217 0000 0072 0600 0000 7218  ....r....r....r.
+00001dc0: 0000 0072 7400 0000 7283 0000 0072 8600  ...rt...r....r..
+00001dd0: 0000 7287 0000 0072 8800 0000 728a 0000  ..r....r....r...
+00001de0: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00001df0: 722a 0000 0072 2a00 0000 724c 0000 0072  r*...r*...rL...r
+00001e00: 2b00 0000 721d 0000 003b 0000 0073 6800  +...r....;...sh.
+00001e10: 0000 0800 0401 0405 0202 2201 0206 1801  ..........".....
+00001e20: 0206 0201 0201 04fb 0202 02fe 0603 02fd  ................
+00001e30: 0604 02fc 0605 0efb 0a2b 1630 1605 020c  .........+.0....
+00001e40: 0a02 02fe 0e03 02fd 0605 0afb 0221 0a02  .............!..
+00001e50: 02fe 0e03 02fd 0605 0afb 0212 0a02 02fe  ................
+00001e60: 0e03 02fd 0605 0afb 161c 1603 0203 0a02  ................
+00001e70: 02fe 0e03 02fd 0605 12fb 721d 0000 0029  ..........r....)
+00001e80: 3272 8e00 0000 7203 0000 0072 0200 0000  2r....r....r....
+00001e90: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
+00001ea0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00001eb0: 0072 0900 0000 da07 6c6f 6767 696e 67da  .r......logging.
+00001ec0: 026f 73da 0c75 726c 6c69 622e 7061 7273  .os..urllib.pars
+00001ed0: 6572 2500 0000 7268 0000 0072 4400 0000  er%...rh...rD...
+00001ee0: da00 720b 0000 00da 1873 6869 6c6c 656c  ..r......shillel
+00001ef0: 6167 682e 6164 6170 7465 7273 2e62 6173  agh.adapters.bas
+00001f00: 6572 0c00 0000 da11 7368 696c 6c65 6c61  er......shillela
+00001f10: 6768 2e66 6965 6c64 7372 0d00 0000 720e  gh.fieldsr....r.
+00001f20: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00001f30: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00001f40: 00da 1273 6869 6c6c 656c 6167 682e 6669  ...shillelagh.fi
+00001f50: 6c74 6572 7372 1500 0000 7216 0000 00da  ltersr....r.....
+00001f60: 1173 6869 6c6c 656c 6167 682e 7479 7069  .shillelagh.typi
+00001f70: 6e67 7217 0000 0072 1800 0000 da09 6765  ngr....r......ge
+00001f80: 744c 6f67 6765 7272 2300 0000 da06 6765  tLoggerr#.....ge
+00001f90: 7465 6e76 da05 6c6f 7765 72da 0b62 6173  tenv..lower..bas
+00001fa0: 6963 436f 6e66 6967 7219 0000 00da 0d53  icConfigr......S
+00001fb0: 7472 6561 6d48 616e 646c 6572 5a0e 7374  treamHandlerZ.st
+00001fc0: 646f 7574 5f68 616e 646c 6572 da08 7365  dout_handler..se
+00001fd0: 744c 6576 656c da09 466f 726d 6174 7465  tLevel..Formatte
+00001fe0: 72da 0966 6f72 6d61 7474 6572 da0c 7365  r..formatter..se
+00001ff0: 7446 6f72 6d61 7474 6572 da0a 6164 6448  tFormatter..addH
+00002000: 616e 646c 6572 da05 4552 524f 5272 1d00  andler..ERRORr..
+00002010: 0000 722a 0000 0072 2a00 0000 722a 0000  ..r*...r*...r*..
+00002020: 0072 2b00 0000 da08 3c6d 6f64 756c 653e  .r+.....<module>
+00002030: 0100 0000 732e 0000 0004 0110 0320 0408  ....s........ ..
+00002040: 0808 0108 0108 0208 010c 020c 0228 0110  .............(..
+00002050: 0a10 0408 051c 020e 0108 010c 010a 010a  ................
+00002060: 010c 010e 0214 03                        .......
```

### Comparing `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/grist.py` & `shillelagh_gristapi-0.0.7/src/shillelagh_gristapi/grist.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import logging
 import os
 import urllib.parse
 
 import requests
 import requests_cache
 
+from . import request_cache_backend
+
 from shillelagh.adapters.base import Adapter
 from shillelagh.fields import (
     Boolean,
     Date,
     DateTime,
     Field,
     Float,
@@ -97,17 +99,18 @@
             server = query_string["server"][0]
         if not org_id:
             org_id = query_string["org_id"][0]
         self.org_id = org_id
         self.headers = {"Authorization": f"Bearer {api_key}"}
         self.server = server
 
+        backend = request_cache_backend()
         self._session = requests_cache.CachedSession(
             cache_name="grist_cache",
-            backend="sqlite",
+            backend=backend,
             expire_after=180,
         )
 
         if self.doc_id:
             if self.table_id:
                 self._set_columns_data()
             else:
```

### Comparing `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/PKG-INFO` & `shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh-gristapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Shillelagh adapter for querying Grist Documents.
 Author-email: Quentin Leroy <quentin.n.leroy@gmail.com>
 Project-URL: Homepage, https://github.com/qleroy/shillelagh-gristapi
 Project-URL: Issues, https://github.com/qleroy/shillelagh-gristapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,15 +87,15 @@
 To make the `shillelagh-gristapi` plugin available, add the following to your `requirements-local.txt` file:
 
 ```python
 shillelagh
 shillelagh-gristapi
 ```
 
-SqlAlechmy URI
+SqlAlchemy URI
 
 ```txt
 shillelagh+safe://
 ```
 
 Engine parameters
```

### Comparing `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/SOURCES.txt` & `shillelagh_gristapi-0.0.7/src/shillelagh_gristapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.6/tests/test_grist.py` & `shillelagh_gristapi-0.0.7/tests/test_grist.py`

 * *Files identical despite different names*

