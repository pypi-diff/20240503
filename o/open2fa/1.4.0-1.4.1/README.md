# Comparing `tmp/open2fa-1.4.0-py3-none-any.whl.zip` & `tmp/open2fa-1.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20670 bytes, number of entries: 17
+Zip file size: 20678 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      113 b- defN 24-Feb-12 01:03 open2fa/__init__.py
 -rw-r--r--  2.0 unx    10069 b- defN 24-Mar-25 23:32 open2fa/cli.py
 -rw-r--r--  2.0 unx     4747 b- defN 24-Apr-27 23:38 open2fa/cli_utils.py
 -rw-r--r--  2.0 unx     4334 b- defN 24-Mar-24 22:21 open2fa/common.py
 -rw-r--r--  2.0 unx      660 b- defN 24-Apr-11 22:49 open2fa/config.py
 -rw-r--r--  2.0 unx      923 b- defN 24-Mar-21 19:32 open2fa/ex.py
 -rw-r--r--  2.0 unx    17991 b- defN 24-Apr-28 22:53 open2fa/main.py
 -rw-r--r--  2.0 unx     1814 b- defN 24-Apr-28 22:58 open2fa/msgs.py
 -rw-r--r--  2.0 unx     2248 b- defN 24-Apr-16 18:10 open2fa/totp.py
 -rw-r--r--  2.0 unx     2139 b- defN 24-Mar-21 19:36 open2fa/utils.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-28 23:02 open2fa/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    11088 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/RECORD
-17 files, 58652 bytes uncompressed, 18600 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-03 02:32 open2fa/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11097 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 24-May-03 02:34 open2fa-1.4.1.dist-info/RECORD
+17 files, 58661 bytes uncompressed, 18608 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: open2fa/utils.py
 Comment: 
 
 Filename: open2fa/version.py
 Comment: 
 
-Filename: open2fa-1.4.0.dist-info/LICENSE
+Filename: open2fa-1.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: open2fa-1.4.0.dist-info/METADATA
+Filename: open2fa-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: open2fa-1.4.0.dist-info/WHEEL
+Filename: open2fa-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: open2fa-1.4.0.dist-info/entry_points.txt
+Filename: open2fa-1.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: open2fa-1.4.0.dist-info/top_level.txt
+Filename: open2fa-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: open2fa-1.4.0.dist-info/RECORD
+Filename: open2fa-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## open2fa/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.4.0"
+__version__ = "1.4.1"
```

## Comparing `open2fa-1.4.0.dist-info/LICENSE` & `open2fa-1.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `open2fa-1.4.0.dist-info/METADATA` & `open2fa-1.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open2fa
-Version: 1.4.0
+Version: 1.4.1
 Summary: A 2FA CLI tool for generating 2FA codes using TOTP secrets, with an optional SECURE remote api, and an optional web ui enabling 2FA code generation from any device
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://open2fa.liberfy.ai
 Project-URL: Repository, https://github.com/cc-d/open2fa
 Project-URL: Issues, https://github.com/cc-d/open2fa/issues
 Project-URL: Server, https://github.com/cc-d/open2fa-server
 Project-URL: Documentation, https://github.com/cc-d/open2fa
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: logfunc <=2.4.3
 Requires-Dist: cryptography <=41.0.7
-Requires-Dist: pyshared >=1.1
+Requires-Dist: pyshared <1.6.0,>=1.5.8
 Requires-Dist: base58 ==2.1.1
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pytest-mock ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
```

## Comparing `open2fa-1.4.0.dist-info/RECORD` & `open2fa-1.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 open2fa/common.py,sha256=44pDlWVJhfGbCW_TczO7Urc_0JFpynfEkP6FJYd6r-Y,4334
 open2fa/config.py,sha256=VixFalMSdS2vOtVhs6D2Jh1-wIeo98fMvD1BZIJbJog,660
 open2fa/ex.py,sha256=nc_q0UdNdbk-KFR0XmcQbpdhtqbs1SnWcus4XzqAq70,923
 open2fa/main.py,sha256=CWU1iJC2Gt78I8AdL_BAB7VH5Ad3GYUS3smhbdbWEq8,17991
 open2fa/msgs.py,sha256=xdQ_tdhopmJz2qJqVkdk-0QCwLFkoNo5y7UBeUl0rno,1814
 open2fa/totp.py,sha256=WKZXQlGlaa7eZK5SR3yBIfUq6PhDAUJpWAiwWJewmMY,2248
 open2fa/utils.py,sha256=j6Nom2zc51aDsY79d1sW6qmSyXrGirIa0cP7AE_wNDg,2139
-open2fa/version.py,sha256=8UhoYEXHs1Oai7BW_ExBmuwWnRI-yMG_u1fQAXMizHQ,22
-open2fa-1.4.0.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-open2fa-1.4.0.dist-info/METADATA,sha256=U6aenzSOPNuBxUy4g2PiGATQdbg4kpUq62-EwUOQ8Cw,11088
-open2fa-1.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-open2fa-1.4.0.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
-open2fa-1.4.0.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
-open2fa-1.4.0.dist-info/RECORD,,
+open2fa/version.py,sha256=BqOI5y46o1G1RWC9bF1DPL-YM68lGYPmZt1pn6FZFZs,22
+open2fa-1.4.1.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+open2fa-1.4.1.dist-info/METADATA,sha256=PIShID3i4qUYFROzoi2R3BJBVy8TI6yAg1aLMN5F88Y,11097
+open2fa-1.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+open2fa-1.4.1.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
+open2fa-1.4.1.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
+open2fa-1.4.1.dist-info/RECORD,,
```

