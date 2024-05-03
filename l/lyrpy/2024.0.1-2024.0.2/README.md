# Comparing `tmp/lyrpy-2024.0.1.tar.gz` & `tmp/lyrpy-2024.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrpy-2024.0.1.tar", last modified: Fri May  3 11:14:22 2024, max compression
+gzip compressed data, was "lyrpy-2024.0.2.tar", last modified: Fri May  3 11:21:20 2024, max compression
```

## Comparing `lyrpy-2024.0.1.tar` & `lyrpy-2024.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 11:14:22.972858 lyrpy-2024.0.1/
--rw-rw-rw-   0        0        0     1096 2024-04-30 15:41:00.000000 lyrpy-2024.0.1/LICENSE
--rw-rw-rw-   0        0        0     2015 2024-05-03 11:14:22.972858 lyrpy-2024.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-04-30 15:40:42.000000 lyrpy-2024.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 11:14:22.921069 lyrpy-2024.0.1/data/
--rw-rw-rw-   0        0        0       14 2024-04-30 09:32:36.000000 lyrpy-2024.0.1/data/text.txt
--rw-rw-rw-   0        0        0     1517 2024-05-03 11:13:36.000000 lyrpy-2024.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-03 11:14:22.973834 lyrpy-2024.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1740 2024-05-03 09:53:47.000000 lyrpy-2024.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 11:14:22.916187 lyrpy-2024.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 11:14:22.967977 lyrpy-2024.0.1/src/lyr/
--rw-rw-rw-   0        0        0    13852 2024-04-29 12:56:27.000000 lyrpy-2024.0.1/src/lyr/LUConsole.py
--rw-rw-rw-   0        0        0     1108 2024-04-29 12:56:27.000000 lyrpy-2024.0.1/src/lyr/LUConst.py
--rw-rw-rw-   0        0        0     6524 2024-04-29 12:56:27.000000 lyrpy-2024.0.1/src/lyr/LUDateTime.py
--rw-rw-rw-   0        0        0    18997 2024-04-30 11:55:59.000000 lyrpy-2024.0.1/src/lyr/LUDecotators.py
--rw-rw-rw-   0        0        0     3102 2024-04-29 12:56:27.000000 lyrpy-2024.0.1/src/lyr/LUDict.py
--rw-rw-rw-   0        0        0     1667 2024-04-29 12:57:13.000000 lyrpy-2024.0.1/src/lyr/LUDoc.py
--rw-rw-rw-   0        0        0     2117 2024-04-29 13:00:17.000000 lyrpy-2024.0.1/src/lyr/LUErrors.py
--rw-rw-rw-   0        0        0    48481 2024-04-29 13:04:38.000000 lyrpy-2024.0.1/src/lyr/LUFile.py
--rw-rw-rw-   0        0        0    18915 2024-04-29 13:08:41.000000 lyrpy-2024.0.1/src/lyr/LUFileUtils.py
--rw-rw-rw-   0        0        0    81725 2024-04-29 13:15:05.000000 lyrpy-2024.0.1/src/lyr/LULog.py
--rw-rw-rw-   0        0        0     7641 2024-04-29 13:15:05.000000 lyrpy-2024.0.1/src/lyr/LUNetwork.py
--rw-rw-rw-   0        0        0     6248 2024-04-29 13:15:05.000000 lyrpy-2024.0.1/src/lyr/LUNumUtils.py
--rw-rw-rw-   0        0        0     5940 2024-04-29 13:15:05.000000 lyrpy-2024.0.1/src/lyr/LUObjects.py
--rw-rw-rw-   0        0        0    29161 2024-04-30 11:43:32.000000 lyrpy-2024.0.1/src/lyr/LUObjectsYT.py
--rw-rw-rw-   0        0        0    14655 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUParserARG.py
--rw-rw-rw-   0        0        0    11006 2024-04-30 11:58:21.000000 lyrpy-2024.0.1/src/lyr/LUParserINI.py
--rw-rw-rw-   0        0        0    19443 2024-04-18 15:59:45.000000 lyrpy-2024.0.1/src/lyr/LUParserREG.py
--rw-rw-rw-   0        0        0     3248 2024-04-18 15:59:45.000000 lyrpy-2024.0.1/src/lyr/LUProc.py
--rw-rw-rw-   0        0        0     4068 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUQThread.py
--rw-rw-rw-   0        0        0     5448 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUQTimer.py
--rw-rw-rw-   0        0        0    31451 2024-04-30 11:58:21.000000 lyrpy-2024.0.1/src/lyr/LUSheduler.py
--rw-rw-rw-   0        0        0     9312 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUStrDecode.py
--rw-rw-rw-   0        0        0    24575 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUStrUtils.py
--rw-rw-rw-   0        0        0     3085 2024-04-28 11:44:29.000000 lyrpy-2024.0.1/src/lyr/LUSupport.py
--rw-rw-rw-   0        0        0     6072 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUThread.py
--rw-rw-rw-   0        0        0     4020 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUTimer.py
--rw-rw-rw-   0        0        0    12254 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUVersion.py
--rw-rw-rw-   0        0        0     6300 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUYouTube.py
--rw-rw-rw-   0        0        0    27518 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUos.py
--rw-rw-rw-   0        0        0     1103 2024-04-30 12:04:24.000000 lyrpy-2024.0.1/src/lyr/LUsys.py
--rw-rw-rw-   0        0        0      498 2024-04-29 09:06:02.000000 lyrpy-2024.0.1/src/lyr/__init__.py
--rw-rw-rw-   0        0        0      410 2024-04-29 12:47:14.000000 lyrpy-2024.0.1/src/lyr/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 11:14:22.971880 lyrpy-2024.0.1/src/lyrpy.egg-info/
--rw-rw-rw-   0        0        0     2015 2024-05-03 11:14:22.000000 lyrpy-2024.0.1/src/lyrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2024-05-03 11:14:22.000000 lyrpy-2024.0.1/src/lyrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 11:14:22.000000 lyrpy-2024.0.1/src/lyrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-03 11:14:22.000000 lyrpy-2024.0.1/src/lyrpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 11:21:20.920446 lyrpy-2024.0.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-30 15:41:00.000000 lyrpy-2024.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2084 2024-05-03 11:21:20.919470 lyrpy-2024.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-30 15:40:42.000000 lyrpy-2024.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 11:21:20.895058 lyrpy-2024.0.2/data/
+-rw-rw-rw-   0        0        0       14 2024-04-30 09:32:36.000000 lyrpy-2024.0.2/data/text.txt
+-rw-rw-rw-   0        0        0     1519 2024-05-03 11:21:10.000000 lyrpy-2024.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-03 11:21:20.920446 lyrpy-2024.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1740 2024-05-03 09:53:47.000000 lyrpy-2024.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:21:20.891154 lyrpy-2024.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 11:21:20.915564 lyrpy-2024.0.2/src/lyr/
+-rw-rw-rw-   0        0        0    13852 2024-04-29 12:56:27.000000 lyrpy-2024.0.2/src/lyr/LUConsole.py
+-rw-rw-rw-   0        0        0     1108 2024-04-29 12:56:27.000000 lyrpy-2024.0.2/src/lyr/LUConst.py
+-rw-rw-rw-   0        0        0     6524 2024-04-29 12:56:27.000000 lyrpy-2024.0.2/src/lyr/LUDateTime.py
+-rw-rw-rw-   0        0        0    18997 2024-04-30 11:55:59.000000 lyrpy-2024.0.2/src/lyr/LUDecotators.py
+-rw-rw-rw-   0        0        0     3102 2024-04-29 12:56:27.000000 lyrpy-2024.0.2/src/lyr/LUDict.py
+-rw-rw-rw-   0        0        0     1667 2024-04-29 12:57:13.000000 lyrpy-2024.0.2/src/lyr/LUDoc.py
+-rw-rw-rw-   0        0        0     2117 2024-04-29 13:00:17.000000 lyrpy-2024.0.2/src/lyr/LUErrors.py
+-rw-rw-rw-   0        0        0    48481 2024-04-29 13:04:38.000000 lyrpy-2024.0.2/src/lyr/LUFile.py
+-rw-rw-rw-   0        0        0    18915 2024-04-29 13:08:41.000000 lyrpy-2024.0.2/src/lyr/LUFileUtils.py
+-rw-rw-rw-   0        0        0    81725 2024-04-29 13:15:05.000000 lyrpy-2024.0.2/src/lyr/LULog.py
+-rw-rw-rw-   0        0        0     7641 2024-04-29 13:15:05.000000 lyrpy-2024.0.2/src/lyr/LUNetwork.py
+-rw-rw-rw-   0        0        0     6248 2024-04-29 13:15:05.000000 lyrpy-2024.0.2/src/lyr/LUNumUtils.py
+-rw-rw-rw-   0        0        0     5940 2024-04-29 13:15:05.000000 lyrpy-2024.0.2/src/lyr/LUObjects.py
+-rw-rw-rw-   0        0        0    29161 2024-04-30 11:43:32.000000 lyrpy-2024.0.2/src/lyr/LUObjectsYT.py
+-rw-rw-rw-   0        0        0    14655 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUParserARG.py
+-rw-rw-rw-   0        0        0    11006 2024-04-30 11:58:21.000000 lyrpy-2024.0.2/src/lyr/LUParserINI.py
+-rw-rw-rw-   0        0        0    19443 2024-04-18 15:59:45.000000 lyrpy-2024.0.2/src/lyr/LUParserREG.py
+-rw-rw-rw-   0        0        0     3248 2024-04-18 15:59:45.000000 lyrpy-2024.0.2/src/lyr/LUProc.py
+-rw-rw-rw-   0        0        0     4068 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUQThread.py
+-rw-rw-rw-   0        0        0     5448 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUQTimer.py
+-rw-rw-rw-   0        0        0    31451 2024-04-30 11:58:21.000000 lyrpy-2024.0.2/src/lyr/LUSheduler.py
+-rw-rw-rw-   0        0        0     9312 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUStrDecode.py
+-rw-rw-rw-   0        0        0    24575 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUStrUtils.py
+-rw-rw-rw-   0        0        0     3085 2024-04-28 11:44:29.000000 lyrpy-2024.0.2/src/lyr/LUSupport.py
+-rw-rw-rw-   0        0        0     6072 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUThread.py
+-rw-rw-rw-   0        0        0     4020 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUTimer.py
+-rw-rw-rw-   0        0        0    12254 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUVersion.py
+-rw-rw-rw-   0        0        0     6300 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUYouTube.py
+-rw-rw-rw-   0        0        0    27518 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUos.py
+-rw-rw-rw-   0        0        0     1103 2024-04-30 12:04:24.000000 lyrpy-2024.0.2/src/lyr/LUsys.py
+-rw-rw-rw-   0        0        0      498 2024-04-29 09:06:02.000000 lyrpy-2024.0.2/src/lyr/__init__.py
+-rw-rw-rw-   0        0        0      410 2024-04-29 12:47:14.000000 lyrpy-2024.0.2/src/lyr/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:21:20.919470 lyrpy-2024.0.2/src/lyrpy.egg-info/
+-rw-rw-rw-   0        0        0     2084 2024-05-03 11:21:20.000000 lyrpy-2024.0.2/src/lyrpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2024-05-03 11:21:20.000000 lyrpy-2024.0.2/src/lyrpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 11:21:20.000000 lyrpy-2024.0.2/src/lyrpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-03 11:21:20.000000 lyrpy-2024.0.2/src/lyrpy.egg-info/top_level.txt
```

### Comparing `lyrpy-2024.0.1/LICENSE` & `lyrpy-2024.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/PKG-INFO` & `lyrpy-2024.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrpy
-Version: 2024.0.1
+Version: 2024.0.2
 Summary: lyrpy
 Author: Lisitsin Y.R.
 Author-email: lisitsinyr <lisitsinyr@gmail.com>
 License: ﻿Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,14 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Repository, https://github.com/lisitsinyr/TOOLS_PY.git
 Keywords: tools,py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lyrpy-2024.0.1/pyproject.toml` & `lyrpy-2024.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lyrpy"
-version = "2024.0.1"
+version = "2024.0.2"
 requires-python = ">=3.8"
 authors = [
   { name="lisitsinyr", email="lisitsinyr@gmail.com" },
 ]
 description = "lyrpy"
 readme = "README.md"
 license = {file = "LICENSE"}
@@ -40,14 +40,14 @@
 # Issues = "https://github.com/me/spam/issues"
 # Repository = "https://github.com/me/spam.git"
 # Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 # Documentation = "https://readthedocs.org"
 
 # Homepage = "https://github.com/lisitsinyr/TOOLS_PY"
 # Issues = "https://github.com/lisitsinyr/TOOLS_PY/issues"
-# Repository = "git@github.com:lisitsinyr/TOOLS_PY.git"
+Repository = "https://github.com/lisitsinyr/TOOLS_PY.git"
 # Changelog = "https://github.com/lisitsinyr/TOOLS_PY/blob/main/README.md"
 # Documentation = "https://readthedocs.org"
```

### Comparing `lyrpy-2024.0.1/setup.py` & `lyrpy-2024.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUConsole.py` & `lyrpy-2024.0.2/src/lyr/LUConsole.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUConst.py` & `lyrpy-2024.0.2/src/lyr/LUConst.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUDateTime.py` & `lyrpy-2024.0.2/src/lyr/LUDateTime.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUDecotators.py` & `lyrpy-2024.0.2/src/lyr/LUDecotators.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUDict.py` & `lyrpy-2024.0.2/src/lyr/LUDict.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUDoc.py` & `lyrpy-2024.0.2/src/lyr/LUDoc.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUErrors.py` & `lyrpy-2024.0.2/src/lyr/LUErrors.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUFile.py` & `lyrpy-2024.0.2/src/lyr/LUFile.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUFileUtils.py` & `lyrpy-2024.0.2/src/lyr/LUFileUtils.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LULog.py` & `lyrpy-2024.0.2/src/lyr/LULog.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUNetwork.py` & `lyrpy-2024.0.2/src/lyr/LUNetwork.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUNumUtils.py` & `lyrpy-2024.0.2/src/lyr/LUNumUtils.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUObjects.py` & `lyrpy-2024.0.2/src/lyr/LUObjects.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUObjectsYT.py` & `lyrpy-2024.0.2/src/lyr/LUObjectsYT.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUParserARG.py` & `lyrpy-2024.0.2/src/lyr/LUParserARG.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUParserINI.py` & `lyrpy-2024.0.2/src/lyr/LUParserINI.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUParserREG.py` & `lyrpy-2024.0.2/src/lyr/LUParserREG.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUProc.py` & `lyrpy-2024.0.2/src/lyr/LUProc.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUQThread.py` & `lyrpy-2024.0.2/src/lyr/LUQThread.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUQTimer.py` & `lyrpy-2024.0.2/src/lyr/LUQTimer.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUSheduler.py` & `lyrpy-2024.0.2/src/lyr/LUSheduler.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUStrDecode.py` & `lyrpy-2024.0.2/src/lyr/LUStrDecode.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUStrUtils.py` & `lyrpy-2024.0.2/src/lyr/LUStrUtils.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUSupport.py` & `lyrpy-2024.0.2/src/lyr/LUSupport.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUThread.py` & `lyrpy-2024.0.2/src/lyr/LUThread.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUTimer.py` & `lyrpy-2024.0.2/src/lyr/LUTimer.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUVersion.py` & `lyrpy-2024.0.2/src/lyr/LUVersion.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUYouTube.py` & `lyrpy-2024.0.2/src/lyr/LUYouTube.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUos.py` & `lyrpy-2024.0.2/src/lyr/LUos.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyr/LUsys.py` & `lyrpy-2024.0.2/src/lyr/LUsys.py`

 * *Files identical despite different names*

### Comparing `lyrpy-2024.0.1/src/lyrpy.egg-info/PKG-INFO` & `lyrpy-2024.0.2/src/lyrpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrpy
-Version: 2024.0.1
+Version: 2024.0.2
 Summary: lyrpy
 Author: Lisitsin Y.R.
 Author-email: lisitsinyr <lisitsinyr@gmail.com>
 License: ﻿Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,14 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Repository, https://github.com/lisitsinyr/TOOLS_PY.git
 Keywords: tools,py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lyrpy-2024.0.1/src/lyrpy.egg-info/SOURCES.txt` & `lyrpy-2024.0.2/src/lyrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

