# Comparing `tmp/monisha-0.0.64.tar.gz` & `tmp/monisha-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.64.tar", last modified: Wed May  1 06:17:16 2024, max compression
+gzip compressed data, was "monisha-0.0.65.tar", last modified: Fri May  3 12:19:06 2024, max compression
```

## Comparing `monisha-0.0.64.tar` & `monisha-0.0.65.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:16.586695 monisha-0.0.64/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 06:17:05.000000 monisha-0.0.64/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:16.578694 monisha-0.0.64/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:16.582695 monisha-0.0.64/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/functions/function18.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:16.582695 monisha-0.0.64/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-01 06:17:05.000000 monisha-0.0.64/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-01 06:17:16.586695 monisha-0.0.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 06:17:05.000000 monisha-0.0.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:17:16.586695 monisha-0.0.64/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-01 06:17:16.000000 monisha-0.0.64/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-01 06:17:16.000000 monisha-0.0.64/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:17:16.000000 monisha-0.0.64/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 06:17:16.000000 monisha-0.0.64/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 06:17:16.000000 monisha-0.0.64/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:17:16.586695 monisha-0.0.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-01 06:17:05.000000 monisha-0.0.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.250053 monisha-0.0.65/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 12:19:02.000000 monisha-0.0.65/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.242053 monisha-0.0.65/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.246053 monisha-0.0.65/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/functions/function19.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.250053 monisha-0.0.65/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-03 12:19:02.000000 monisha-0.0.65/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 12:19:06.250053 monisha-0.0.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 12:19:02.000000 monisha-0.0.65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:19:06.250053 monisha-0.0.65/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 12:19:06.000000 monisha-0.0.65/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:19:06.250053 monisha-0.0.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 12:19:02.000000 monisha-0.0.65/setup.py
```

### Comparing `monisha-0.0.64/LICENSE` & `monisha-0.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/__init__.py` & `monisha-0.0.65/Monisha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.64"
+version = "0.0.65"
 
 install = ["hachoir"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

### Comparing `monisha-0.0.64/Monisha/functions/__init__.py` & `monisha-0.0.65/Monisha/functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 from .function07 import Cmd, Wosd
 from .function18 import Metadatas
 from .function15 import Location
 from .function17 import Filename
 from .function09 import Storage
 from .function16 import FMagic
 from .function10 import Fonts
+from .function19 import views
 from .function11 import con2s
 from .function12 import YKeys
 from .function05 import Doxo
 from .function13 import Guid
 from .function08 import Num
```

### Comparing `monisha-0.0.64/Monisha/functions/function01.py` & `monisha-0.0.65/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function02.py` & `monisha-0.0.65/Monisha/functions/function02.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from ..scripts import Humon, Scripted
 #=============================================================================
 
 def Dbytes(sizes, second=Scripted.DATA01):
-    if not sizes or (sizes == Scripted.DATA02):
+    if not sizes or sizes == Scripted.DATA02 or sizes < 0:
         return Scripted.DATA09
     nomos = 0
-    POWEO = 2**10
+    POWEO = 1024
     POWER = Humon.DATA01
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
     ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
     return ouing
 
 #=============================================================================
 
 def Hbytes(sizes, second=Scripted.DATA01):
-    if not sizes or (sizes == Scripted.DATA02):
+    if not sizes or sizes == Scripted.DATA02 or sizes < 0:
         return Scripted.DATA08
     nomos = 0
-    POWEO = 2**10
+    POWEO = 1024
     POWER = Humon.DATA02
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
     ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
     return ouing
 
 #=============================================================================
 
 def Gbytes(sizes, second=Scripted.DATA01):
-    if not sizes or (sizes == Scripted.DATA02):
+    if not sizes or sizes == Scripted.DATA02 or sizes < 0:
         return Scripted.DATA01
     nomos = 0
-    POWEO = 2**10
+    POWEO = 1024
     POWER = Humon.DATA01
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
     ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
     return ouing
```

### Comparing `monisha-0.0.64/Monisha/functions/function03.py` & `monisha-0.0.65/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function04.py` & `monisha-0.0.65/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function06.py` & `monisha-0.0.65/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function07.py` & `monisha-0.0.65/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function10.py` & `monisha-0.0.65/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function14.py` & `monisha-0.0.65/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function15.py` & `monisha-0.0.65/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function16.py` & `monisha-0.0.65/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function17.py` & `monisha-0.0.65/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/functions/function18.py` & `monisha-0.0.65/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.64/Monisha/scripts/es.py` & `monisha-0.0.65/Monisha/scripts/es.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,20 @@
     DATA05 = "ABRAHAM"
     DATA06 = "DOWNLOAD"
     DATA07 = "DOWNLOADS"
     DATA08 = "TEMPORARY"
 
 #=======================================================================================
 
+class Numeo(object):
+
+    DATA01 = ["", "K", "M", "B", "T", "Qa", "Qu", "S", "Oc", "No"]
+
+#=======================================================================================
+
 class Strine(object):
 
     DATA01 = "0123456789"
     DATA02 = "abcdefghijklmnopqrstuvwxyz"
     DATA03 = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
     DATA04 = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
```

### Comparing `monisha-0.0.64/PKG-INFO` & `monisha-0.0.65/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.64
+Version: 0.0.65
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.64 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.65 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.64/monisha.egg-info/PKG-INFO` & `monisha-0.0.65/monisha.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.64
+Version: 0.0.65
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.64 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.65 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.64/monisha.egg-info/SOURCES.txt` & `monisha-0.0.65/monisha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 Monisha/functions/function12.py
 Monisha/functions/function13.py
 Monisha/functions/function14.py
 Monisha/functions/function15.py
 Monisha/functions/function16.py
 Monisha/functions/function17.py
 Monisha/functions/function18.py
+Monisha/functions/function19.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
```

### Comparing `monisha-0.0.64/setup.py` & `monisha-0.0.65/setup.py`

 * *Files identical despite different names*

