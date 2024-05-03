# Comparing `tmp/codenerix-lib-1.0.8.tar.gz` & `tmp/codenerix-lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codenerix-lib-1.0.8.tar", last modified: Fri May 10 06:56:54 2019, max compression
+gzip compressed data, was "dist/codenerix-lib-1.0.9.tar", last modified: Fri May 10 07:14:03 2019, max compression
```

## Comparing `codenerix-lib-1.0.8.tar` & `codenerix-lib-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      110 2018-11-28 18:18:47.000000 codenerix-lib-1.0.8/MANIFEST.in
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       38 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/setup.cfg
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2017-01-31 16:52:43.000000 codenerix-lib-1.0.8/LICENSE
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      444 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/top_level.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2018-11-28 18:29:28.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       23 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2028 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1396 2018-11-28 18:29:09.000000 codenerix-lib-1.0.8/setup.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      848 2018-11-28 18:24:50.000000 codenerix-lib-1.0.8/README.rst
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2028 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/PKG-INFO
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2019-05-10 06:56:54.000000 codenerix-lib-1.0.8/codenerix_lib/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6161 2017-11-28 23:22:48.000000 codenerix-lib-1.0.8/codenerix_lib/timeout.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      101 2019-05-10 06:56:53.000000 codenerix-lib-1.0.8/codenerix_lib/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1944 2019-04-02 13:13:06.000000 codenerix-lib-1.0.8/codenerix_lib/memorytracer.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11669 2019-05-10 06:56:43.000000 codenerix-lib-1.0.8/codenerix_lib/debugger.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3812 2017-12-18 12:03:26.000000 codenerix-lib-1.0.8/codenerix_lib/pylock.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2890 2018-11-26 06:24:20.000000 codenerix-lib-1.0.8/codenerix_lib/cryptography.py
--rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)     2144 2018-11-28 18:26:26.000000 codenerix-lib-1.0.8/codenerix_lib/colors.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      110 2018-11-28 18:18:47.000000 codenerix-lib-1.0.9/MANIFEST.in
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       38 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/setup.cfg
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2017-01-31 16:52:43.000000 codenerix-lib-1.0.9/LICENSE
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      444 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/top_level.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2018-11-28 18:29:28.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       23 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2028 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1396 2018-11-28 18:29:09.000000 codenerix-lib-1.0.9/setup.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      848 2018-11-28 18:24:50.000000 codenerix-lib-1.0.9/README.rst
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2028 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/PKG-INFO
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2019-05-10 07:14:03.000000 codenerix-lib-1.0.9/codenerix_lib/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6161 2017-11-28 23:22:48.000000 codenerix-lib-1.0.9/codenerix_lib/timeout.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      101 2019-05-10 07:14:02.000000 codenerix-lib-1.0.9/codenerix_lib/__init__.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1944 2019-04-02 13:13:06.000000 codenerix-lib-1.0.9/codenerix_lib/memorytracer.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11731 2019-05-10 07:13:54.000000 codenerix-lib-1.0.9/codenerix_lib/debugger.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3812 2017-12-18 12:03:26.000000 codenerix-lib-1.0.9/codenerix_lib/pylock.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2890 2018-11-26 06:24:20.000000 codenerix-lib-1.0.9/codenerix_lib/cryptography.py
+-rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)     2144 2018-11-28 18:26:26.000000 codenerix-lib-1.0.9/codenerix_lib/colors.py
```

### Comparing `codenerix-lib-1.0.8/LICENSE` & `codenerix-lib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/codenerix_lib.egg-info/PKG-INFO` & `codenerix-lib-1.0.9/codenerix_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: codenerix-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Basic libraries used by CODENERIX.
 Home-page: https://github.com/codenerix/codenerix-lib
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>
 Author-email: UNKNOWN
 License: Apache License Version 2.0
 Description: =============
         codenerix-lib
```

### Comparing `codenerix-lib-1.0.8/setup.py` & `codenerix-lib-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/README.rst` & `codenerix-lib-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/PKG-INFO` & `codenerix-lib-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: codenerix-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Basic libraries used by CODENERIX.
 Home-page: https://github.com/codenerix/codenerix-lib
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>
 Author-email: UNKNOWN
 License: Apache License Version 2.0
 Description: =============
         codenerix-lib
```

### Comparing `codenerix-lib-1.0.8/codenerix_lib/timeout.py` & `codenerix-lib-1.0.9/codenerix_lib/timeout.py`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/codenerix_lib/memorytracer.py` & `codenerix-lib-1.0.9/codenerix_lib/memorytracer.py`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/codenerix_lib/debugger.py` & `codenerix-lib-1.0.9/codenerix_lib/debugger.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from os import getcwd
 from time import time
 from datetime import datetime
 from inspect import currentframe
 
 from .colors import colors
 
-__version__ = "2019051000"
+__version__ = "2019051001"
 
 __all__ = ['Debugger', 'lineno', '__FILE__', '__LINE__']
 
 
 def lineno():
     '''
     Returns the current line number in our program.
@@ -249,14 +249,17 @@
         self.debug_with_style(msg, "INFO", "cyan", "info", show_line_info, header=header, tail=tail)
 
     def error(self, msg, header=True, tail=True, show_line_info=True):
         self.debug_with_style(msg, "ERROR", "red", "error", show_line_info, header=header, tail=tail)
 
     def warningerror(self, msg, header, prefix, color, tail, line=None, filename=None, kind=None):
 
+        # Save original color
+        original_color = color
+
         # Retrieve the name of the class
         clname = self.__class__.__name__
 
         # Retrieve tabular
         if 'tabular' in self.__indebug:
             tabular = self.__indebug['tabular']
         else:
```

### Comparing `codenerix-lib-1.0.8/codenerix_lib/pylock.py` & `codenerix-lib-1.0.9/codenerix_lib/pylock.py`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/codenerix_lib/cryptography.py` & `codenerix-lib-1.0.9/codenerix_lib/cryptography.py`

 * *Files identical despite different names*

### Comparing `codenerix-lib-1.0.8/codenerix_lib/colors.py` & `codenerix-lib-1.0.9/codenerix_lib/colors.py`

 * *Files identical despite different names*

