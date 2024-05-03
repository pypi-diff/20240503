# Comparing `tmp/python-dali-0.8.tar.gz` & `tmp/python-dali-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dali-0.8.tar", last modified: Thu Dec  2 18:06:53 2021, max compression
+gzip compressed data, was "python-dali-0.9.tar", last modified: Thu Apr 21 08:08:54 2022, max compression
```

## Comparing `python-dali-0.8.tar` & `python-dali-0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.694086 python-dali-0.8/
--rw-rw-r--   0 steve     (1000) steve     (1000)     5898 2021-12-02 18:06:53.694086 python-dali-0.8/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)     4155 2021-12-02 18:02:17.000000 python-dali-0.8/README.rst
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.690086 python-dali-0.8/dali/
--rw-rw-r--   0 steve     (1000) steve     (1000)      118 2021-12-02 18:02:17.000000 python-dali-0.8/dali/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     8969 2021-12-02 18:02:17.000000 python-dali-0.8/dali/address.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9413 2021-12-02 18:02:17.000000 python-dali-0.8/dali/command.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.690086 python-dali-0.8/dali/device/
--rw-rw-r--   0 steve     (1000) steve     (1000)      221 2021-12-02 18:02:17.000000 python-dali-0.8/dali/device/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    19410 2021-12-02 18:02:17.000000 python-dali-0.8/dali/device/general.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.690086 python-dali-0.8/dali/driver/
--rw-rw-r--   0 steve     (1000) steve     (1000)       73 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7715 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/base.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3120 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/daliserver.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9455 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/hasseb.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    28091 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/hid.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    10891 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/tridonic.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6968 2021-12-02 18:02:17.000000 python-dali-0.8/dali/driver/unipi.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3224 2021-12-02 18:02:17.000000 python-dali-0.8/dali/exceptions.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9903 2021-12-02 18:02:17.000000 python-dali-0.8/dali/frame.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.690086 python-dali-0.8/dali/gear/
--rw-rw-r--   0 steve     (1000) steve     (1000)      335 2021-12-02 18:02:17.000000 python-dali-0.8/dali/gear/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    12529 2021-12-02 18:02:17.000000 python-dali-0.8/dali/gear/emergency.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    37444 2021-12-02 18:02:17.000000 python-dali-0.8/dali/gear/general.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     8944 2021-12-02 18:02:17.000000 python-dali-0.8/dali/gear/incandescent.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5896 2021-12-02 18:02:17.000000 python-dali-0.8/dali/gear/led.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.690086 python-dali-0.8/dali/memory/
--rw-rw-r--   0 steve     (1000) steve     (1000)      105 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    22484 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/diagnostics.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     4880 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/energy.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     4985 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/info.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    23192 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/location.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2827 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/maintenance.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6274 2021-12-02 18:02:17.000000 python-dali-0.8/dali/memory/oem.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     8138 2021-12-02 18:02:17.000000 python-dali-0.8/dali/sequences.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.694086 python-dali-0.8/dali/tests/
--rw-rw-r--   0 steve     (1000) steve     (1000)        0 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    13106 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/fakes.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5170 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/test_command.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2090 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/test_exceptions.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     8602 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/test_frame.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    24700 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/test_memory.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     4314 2021-12-02 18:02:17.000000 python-dali-0.8/dali/tests/test_sequences.py
--rw-rw-r--   0 steve     (1000) steve     (1000)       48 2021-12-02 18:02:17.000000 python-dali-0.8/dali/version.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2021-12-02 18:06:53.694086 python-dali-0.8/python_dali.egg-info/
--rw-r--r--   0 steve     (1000) steve     (1000)     5898 2021-12-02 18:06:53.000000 python-dali-0.8/python_dali.egg-info/PKG-INFO
--rw-r--r--   0 steve     (1000) steve     (1000)      964 2021-12-02 18:06:53.000000 python-dali-0.8/python_dali.egg-info/SOURCES.txt
--rw-r--r--   0 steve     (1000) steve     (1000)        1 2021-12-02 18:06:53.000000 python-dali-0.8/python_dali.egg-info/dependency_links.txt
--rw-r--r--   0 steve     (1000) steve     (1000)       31 2021-12-02 18:06:53.000000 python-dali-0.8/python_dali.egg-info/requires.txt
--rw-r--r--   0 steve     (1000) steve     (1000)        5 2021-12-02 18:06:53.000000 python-dali-0.8/python_dali.egg-info/top_level.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2021-12-02 18:06:53.694086 python-dali-0.8/setup.cfg
--rwxrwxr-x   0 steve     (1000) steve     (1000)     1065 2021-12-02 18:02:17.000000 python-dali-0.8/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.692139 python-dali-0.9/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5898 2022-04-21 08:08:54.692139 python-dali-0.9/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4155 2022-04-21 08:06:46.000000 python-dali-0.9/README.rst
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.688140 python-dali-0.9/dali/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      118 2022-04-21 08:06:46.000000 python-dali-0.9/dali/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     8969 2022-04-21 08:06:46.000000 python-dali-0.9/dali/address.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     8097 2022-04-21 08:06:46.000000 python-dali-0.9/dali/command.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.688140 python-dali-0.9/dali/device/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      221 2022-04-21 08:06:46.000000 python-dali-0.9/dali/device/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19410 2022-04-21 08:06:46.000000 python-dali-0.9/dali/device/general.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.688140 python-dali-0.9/dali/driver/
+-rw-rw-r--   0 steve     (1000) steve     (1000)       73 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7715 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/base.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3120 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/daliserver.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     9376 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/hasseb.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    28091 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/hid.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    10891 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/tridonic.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6968 2022-04-21 08:06:46.000000 python-dali-0.9/dali/driver/unipi.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3224 2022-04-21 08:06:46.000000 python-dali-0.9/dali/exceptions.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     9933 2022-04-21 08:06:46.000000 python-dali-0.9/dali/frame.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.688140 python-dali-0.9/dali/gear/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      335 2022-04-21 08:06:46.000000 python-dali-0.9/dali/gear/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    12529 2022-04-21 08:06:46.000000 python-dali-0.9/dali/gear/emergency.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    37379 2022-04-21 08:06:46.000000 python-dali-0.9/dali/gear/general.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     8944 2022-04-21 08:06:46.000000 python-dali-0.9/dali/gear/incandescent.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5896 2022-04-21 08:06:46.000000 python-dali-0.9/dali/gear/led.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.688140 python-dali-0.9/dali/memory/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      105 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    22484 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/diagnostics.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4880 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/energy.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4985 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/info.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    23192 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/location.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2827 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/maintenance.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6274 2022-04-21 08:06:46.000000 python-dali-0.9/dali/memory/oem.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     8138 2022-04-21 08:06:46.000000 python-dali-0.9/dali/sequences.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.692139 python-dali-0.9/dali/tests/
+-rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    13106 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/fakes.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5086 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/test_command.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2090 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/test_exceptions.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     8020 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/test_frame.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    24700 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/test_memory.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4314 2022-04-21 08:06:46.000000 python-dali-0.9/dali/tests/test_sequences.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)       48 2022-04-21 08:06:46.000000 python-dali-0.9/dali/version.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-04-21 08:08:54.692139 python-dali-0.9/python_dali.egg-info/
+-rw-r--r--   0 steve     (1000) steve     (1000)     5898 2022-04-21 08:08:54.000000 python-dali-0.9/python_dali.egg-info/PKG-INFO
+-rw-r--r--   0 steve     (1000) steve     (1000)      964 2022-04-21 08:08:54.000000 python-dali-0.9/python_dali.egg-info/SOURCES.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)        1 2022-04-21 08:08:54.000000 python-dali-0.9/python_dali.egg-info/dependency_links.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)       31 2022-04-21 08:08:54.000000 python-dali-0.9/python_dali.egg-info/requires.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)        5 2022-04-21 08:08:54.000000 python-dali-0.9/python_dali.egg-info/top_level.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2022-04-21 08:08:54.692139 python-dali-0.9/setup.cfg
+-rwxrwxr-x   0 steve     (1000) steve     (1000)     1065 2022-04-21 08:06:46.000000 python-dali-0.9/setup.py
```

### Comparing `python-dali-0.8/PKG-INFO` & `python-dali-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dali
-Version: 0.8
+Version: 0.9
 Summary: Interface to DALI lighting systems
 Home-page: https://github.com/sde1000/python-dali
 Author: Stephen Early
 Author-email: steve@assorted.org.uk
 License: LGPL3+
 Description: python-dali — lighting control interface
         ========================================
@@ -119,15 +119,15 @@
         
         - Ferdinand Keil
         
         
         Copyright
         ---------
         
-        python-dali is Copyright (C) 2013–2021 Stephen Early <steve@assorted.org.uk>
+        python-dali is Copyright (C) 2013–2022 Stephen Early <steve@assorted.org.uk>
         and other contributors.
         
         It is distributed under the terms of the GNU Lesser General Public
         License as published by the Free Software Foundation, either version 3
         of the License, or (at your option) any later version.
         
         This program is distributed in the hope that it will be useful, but
```

### Comparing `python-dali-0.8/README.rst` & `python-dali-0.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 - Ferdinand Keil
 
 
 Copyright
 ---------
 
-python-dali is Copyright (C) 2013–2021 Stephen Early <steve@assorted.org.uk>
+python-dali is Copyright (C) 2013–2022 Stephen Early <steve@assorted.org.uk>
 and other contributors.
 
 It is distributed under the terms of the GNU Lesser General Public
 License as published by the Free Software Foundation, either version 3
 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but
```

### Comparing `python-dali-0.8/dali/address.py` & `python-dali-0.9/dali/address.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/command.py` & `python-dali-0.9/dali/command.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Declaration of base types for dali commands and their responses."""
 
 from dali import address
 from dali import frame
 from dali.exceptions import MissingResponse
 from dali.exceptions import ResponseError
-import warnings
 
 
 class _CommandTracker(type):
     """Metaclass keeping track of all the types of Command we understand.
 
     Commands that have names starting with '_' are treated as abstract
     base classes that will never be instantiated because they do not
@@ -187,23 +186,14 @@
 
     # 16-bit frames may be interpreted differently if they are
     # preceded by the EnableDeviceType command.  If a command needs
     # EnableDeviceType(foo) to be sent first, override devicetype to
     # foo.  This parameter is ignored for all other frame lengths.
     devicetype = 0
 
-    # devicetype used to be called "_devicetype".  This property is
-    # here for compatibility with older code that relied on this.  It
-    # will be removed in release 0.9
-    @property
-    def _devicetype(self):
-        warnings.warn("'_devicetype' has been renamed to 'devicetype'",
-                      DeprecationWarning, stacklevel=2)
-        return self.devicetype
-
     def __init__(self, f):
         assert isinstance(f, frame.ForwardFrame)
         self._data = f
 
     _framesizes = {}
 
     @classmethod
@@ -241,42 +231,18 @@
 
     @property
     def frame(self):
         """The forward frame to be transmitted for this command."""
         return self._data
 
     @property
-    def is_config(self):
-        """Is this a configuration command?  (Does it need repeating to
-        take effect?)
-
-        Use of this property is deprecated: access the "sendtwice"
-        attribute directly. This property will be removed in release 0.9.
-        """
-        warnings.warn("Access 'sendtwice' directly instead of using 'is_config'",
-                      DeprecationWarning, stacklevel=2)
-        return self.sendtwice
-
-    @property
     def is_query(self):
         """Does this command return a result?"""
         return self.response is not None
 
-    @property
-    def _response(self):
-        """If this command returns a result, use this class for the response.
-
-        This property is provided for compatibility with old code.
-        Access the "response" attribute directly. This property will
-        be removed in release 0.9.
-        """
-        warnings.warn("Access 'response' directly instead of using '_response'",
-                      DeprecationWarning, stacklevel=2)
-        return self.response
-
     @staticmethod
     def _check_destination(destination):
         """Check that a valid destination has been specified.
 
         destination can be a dali.bus.Device object with
         address_obj attribute, a dali.address.Address object with
         add_to_frame method, or an integer which will be wrapped in a
```

### Comparing `python-dali-0.8/dali/device/general.py` & `python-dali-0.9/dali/device/general.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/driver/base.py` & `python-dali-0.9/dali/driver/base.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/driver/daliserver.py` & `python-dali-0.9/dali/driver/daliserver.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/driver/hasseb.py` & `python-dali-0.9/dali/driver/hasseb.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 from dali.sequences import sleep as sequence_sleep
 from dali.sequences import progress as sequence_progress
 
 import dali.gear.general as gear
 
 import time
 
-import hidapi
-
-hidapi.hid_init()
+import hid
 
 HASSEB_USB_VENDOR = 0x04cc
 HASSEB_USB_PRODUCT = 0x0802
 
 HASSEB_READ_FIRMWARE_VERSION    = 0x02
 HASSEB_CONFIGURE_DEVICE         = 0x05
 HASSEB_DALI_FRAME               = 0X07
@@ -78,15 +76,19 @@
     sn = 0
     send_message = None
     _pending = None
     _response_message = None
 
     def __init__(self, path=None):
         try:
-            self.device = hidapi.hid_open(HASSEB_USB_VENDOR, HASSEB_USB_PRODUCT, None) if not bool(path) else hidapi.hid_open_path(path)
+            self.device = hid.device()
+            if path:
+                self.device.open_path(path)
+            else:
+                self.device.open(HASSEB_USB_VENDOR, HASSEB_USB_PRODUCT)
             self.device_found = 1
         except:
             self.device_found = None
 
     def run_sequence(self, seq, progress_cb=None):
         from dali.gear.general import EnableDeviceType
 
@@ -121,15 +123,15 @@
             self.sn = 1
         frame_length = 16
         if command.is_query:
             expect_reply = 1
         else:
             expect_reply = 0
         transmitter_settling_time = 0
-        if command.is_config:
+        if command.sendtwice:
             send_twice = 10 # 10 ms delay between messages
         else:
             send_twice = 0
         frame = command.frame.as_byte_sequence
         byte_a, byte_b = frame
         data = struct.pack('BBBBBBBBBB', 0xAA, HASSEB_DALI_FRAME, self.sn,
                            frame_length, expect_reply,
@@ -174,24 +176,24 @@
         time.sleep(0.02)    # a delay between sent messages need to be at lest 22*417 µs
         self._response_message = None
         data = self.construct(command)
         self.send_message = struct.pack('BB', data[7], data[8])
         if command.response is not None:
             self._pending = command
             self._response_message = None
-            hidapi.hid_write(self.device, data)
+            self.device.write(data)
             self.wait_for_response()
             return command.response(self.extract(self._response_message))
         else:
             self._pending = None
-            hidapi.hid_write(self.device, data)
+            self.device.write(data)
             return
 
     def receive(self):
-        data = hidapi.hid_read(self.device, 10)
+        data = self.device.read(10)
         frame = self.extract(data)
         if isinstance(frame, HassebDALIUSBNoDataAvailable):
             return
         elif isinstance(frame, BackwardFrame) or isinstance(frame, HassebDALIUSBNoAnswer):
             if self._pending and isinstance(frame, BackwardFrame):
                 self._response_message = data
                 self._pending = None
@@ -202,41 +204,41 @@
 
     def readFirmwareVersion(self):
         self.sn = self.sn + 1
         if self.sn > 255:
             self.sn = 1
         data = struct.pack('BBBBBBBBBB', 0xAA, HASSEB_READ_FIRMWARE_VERSION,
                             self.sn, 0, 0, 0, 0, 0, 0, 0)
-        hidapi.hid_write(self.device, data)
-        data = hidapi.hid_read(self.device, 10)
+        self.device.write(data)
+        data = self.device.read(10)
         for i in range(0,100):
             if len(data)==10:
                 if data[1] != HASSEB_READ_FIRMWARE_VERSION:
-                    data = hidapi.hid_read(self.device, 10)
+                    data = self.device.read(10)
                 else:
                     return f"{data[3]}.{data[4]}"
             else:
-                data = hidapi.hid_read(self.device, 10)
+                data = self.device.read(10)
         return f"VERSION_ERROR"
 
     def enableSniffing(self):
         self.sn = self.sn + 1
         if self.sn > 255:
             self.sn = 1
         data = struct.pack('BBBBBBBBBB', 0xAA, HASSEB_CONFIGURE_DEVICE,
                             self.sn, 0x01, 0, 0, 0, 0, 0, 0)
-        hidapi.hid_write(self.device, data)
+        self.device.write(data)
 
     def disableSniffing(self):
         self.sn = self.sn + 1
         if self.sn > 255:
             self.sn = 1
         data = struct.pack('BBBBBBBBBB', 0xAA, HASSEB_CONFIGURE_DEVICE,
                             self.sn, 0, 0, 0, 0, 0, 0, 0)
-        hidapi.hid_write(self.device, data)
+        self.device.write(data)
 
 
 class AsyncHassebDALIUSBDriver(HassebDALIUSBDriver, AsyncDALIDriver):
     """Asynchronous ``DALIDriver`` implementation for Hasseb DALI USB device.
        Using asynchronous driver requires a separate thread for receiving
        DALI messages. receive() function needs to be called continously
        from the thread. You can also define an event processor function which
@@ -276,13 +278,13 @@
 def SyncHassebDALIUSBDriverFactory():
     """Enumerates Hasseb DALI masters and instantiates `SyncHassebDALIUSBDriver`s
     for each one of them.
     """
 
     hasseb_dali_drivers = []
 
-    hasseb_hid_devices = hidapi.hid_enumerate(HASSEB_USB_VENDOR, HASSEB_USB_PRODUCT)
+    hasseb_hid_devices = hid.enumerate(HASSEB_USB_VENDOR, HASSEB_USB_PRODUCT)
     for hasseb_hid_device in hasseb_hid_devices:
         logging.getLogger("SyncHassebDALIUSBDriverFactory").debug("device found, path is {}".format(hasseb_hid_device.path))
         hasseb_dali_drivers.append(SyncHassebDALIUSBDriver(hasseb_hid_device.path))
 
-    return hasseb_dali_drivers
+    return hasseb_dali_drivers
```

### Comparing `python-dali-0.8/dali/driver/hid.py` & `python-dali-0.9/dali/driver/hid.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/driver/tridonic.py` & `python-dali-0.9/dali/driver/tridonic.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/driver/unipi.py` & `python-dali-0.9/dali/driver/unipi.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/exceptions.py` & `python-dali-0.9/dali/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/frame.py` & `python-dali-0.9/dali/frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     A Frame consists of one start bit, n data bits, and one stop
     condition.  The most significant bit is always transmitted first.
 
     Instances of this object are mutable.
     """
 
-    def __init__(self, bits, data=0, new_exceptions=False):
+    def __init__(self, bits, data=0, new_exceptions=True):
         """Initialise a Frame with the supplied number of data bits.
 
         :parameter bits: the number of data bits in the Frame
         :parameter data: initial data for the Frame as an integer or
         an iterable sequence of integers
         """
         if not isinstance(bits, int):
@@ -28,17 +28,17 @@
             self._data = data
         else:
             if new_exceptions:
                 self._data = int.from_bytes(data, 'big')
             else:
                 warnings.warn("Frame() will raise ValueError in the future "
                               "when an invalid initialisation sequence is "
-                              "passed, instead of TypeError. Pass "
-                              "new_exceptions=True to Frame() to use "
-                              "the new behaviour now.",
+                              "passed, instead of TypeError. Passing "
+                              "new_exceptions=False to Frame() will not be "
+                              "possible in the next release.",
                               DeprecationWarning, stacklevel=2)
                 try:
                     self._data = int.from_bytes(data, 'big')
                 except ValueError:
                     raise TypeError(
                         "data must be a sequence of integers all in the "
                         "range 0..255 or an integer")
@@ -182,30 +182,30 @@
         If the frame is not an exact multiple of 8 bits long, the
         first byte in the string will contain fewer than 8 bits.
         """
         return self._data.to_bytes(
             (len(self) // 8) + (1 if len(self) % 8 else 0),
             'big')
 
-    def pack_len(self, l, new_exceptions=False):
+    def pack_len(self, l, new_exceptions=True):
         """The contents of the frame represented as a fixed length byte string.
 
         The least significant bit of the frame is aligned to the end
         of the byte string.  The start of the byte string is padded with zeroes.
 
         If the frame will not fit in the byte string, raises
         ValueError (with new_exceptions=False) or OverflowError (with
         new_exceptions=True).
         """
         if new_exceptions:
             return self._data.to_bytes(l, 'big')
         warnings.warn("Frame.pack_len() will raise OverflowError in the "
                       "future when an invalid length is passed, instead of "
-                      "ValueError. Pass new_exceptions=True to use "
-                      "the new behaviour now.",
+                      "ValueError. Passing new_exceptions=False will not be "
+                      "possible in the next release.",
                       DeprecationWarning, stacklevel=2)
         try:
             return self._data.to_bytes(l, 'big')
         except OverflowError:
             raise ValueError(
                 f"Frame length {len(self)} will not fit in {l} bytes")
```

### Comparing `python-dali-0.8/dali/gear/emergency.py` & `python-dali-0.9/dali/gear/emergency.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/gear/general.py` & `python-dali-0.9/dali/gear/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -1011,16 +1011,15 @@
         else:
             if len(args) != 0:
                 raise TypeError(
                     "{}.__init__() takes exactly 1 arguments ({} given)".format(
                         self.__class__.__name__, len(args) + 1))
             param = 0
         self.param = param
-        super().__init__(frame.ForwardFrame(16, (self._cmdval, self.param),
-                                            new_exceptions=True))
+        super().__init__(frame.ForwardFrame(16, (self._cmdval, self.param)))
 
     # dict of frame[15:8] to cls
     _opcodes = {}
 
     @classmethod
     def _register_subclass(cls, subclass):
         if subclass.__name__[0] == '_':
```

### Comparing `python-dali-0.8/dali/gear/incandescent.py` & `python-dali-0.9/dali/gear/incandescent.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/gear/led.py` & `python-dali-0.9/dali/gear/led.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/memory/diagnostics.py` & `python-dali-0.9/dali/memory/diagnostics.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/memory/energy.py` & `python-dali-0.9/dali/memory/energy.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/memory/info.py` & `python-dali-0.9/dali/memory/info.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/memory/location.py` & `python-dali-0.9/dali/memory/location.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/memory/maintenance.py` & `python-dali-0.9/dali/memory/maintenance.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/memory/oem.py` & `python-dali-0.9/dali/memory/oem.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/sequences.py` & `python-dali-0.9/dali/sequences.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/tests/fakes.py` & `python-dali-0.9/dali/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/tests/test_command.py` & `python-dali-0.9/dali/tests/test_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                         'intendedAttr: %s' % (obj, intendedAttr))
 
     def test_test_coverage(self):
         """all command classes are covered by test pattern"""
         seen = {}
         for fs, d, dt in _test_pattern():
             c = command.from_frame(
-                frame.ForwardFrame(fs, d, new_exceptions=True), devicetype=dt)
+                frame.ForwardFrame(fs, d), devicetype=dt)
             seen[c.__class__] = True
         for cls in command.Command._commands:
             self.assertTrue(
                 cls in seen,
                 'class {} not covered by tests'.format(cls.__name__)
             )
 
@@ -67,25 +67,25 @@
                 self.assertIsInstance(cls.response(None), command.Response)
             self.assertHasAttr(cls, "sendtwice")
             self.assertIsInstance(cls.sendtwice, bool)
 
     def test_roundtrip(self):
         """all frames survive command.from_frame()"""
         for fs, d, dt in _test_pattern():
-            f = frame.ForwardFrame(fs, d, new_exceptions=True)
+            f = frame.ForwardFrame(fs, d)
             c = command.from_frame(f, dt)
             nf = c.frame
             self.assertEqual(
                 f, nf, 'frame {} failed command round-trip; command {} '
                 'became {}'.format(str(f), str(c), str(nf)))
 
     def test_str(self):
         """command objects can be converted to strings"""
         for fs, d, dt in _test_pattern():
-            f = frame.ForwardFrame(fs, d, new_exceptions=True)
+            f = frame.ForwardFrame(fs, d)
             self.assertIsInstance(str(command.from_frame(f, dt)),
                                   str)
 
     def test_with_integer_destination(self):
         """commands accept integer destination"""
         self.assertEqual(
             generalgear.DAPC(5, 100).destination,
@@ -95,15 +95,15 @@
         self.assertRaises(ValueError, generalgear.Off, -1)
         self.assertRaises(ValueError, generalgear.Off, 64)
         self.assertRaises(ValueError, generalgear.Off, None)
 
     def test_response(self):
         """responses act sensibly"""
         for fs, d, dt in _test_pattern():
-            f = frame.ForwardFrame(fs, d, new_exceptions=True)
+            f = frame.ForwardFrame(fs, d)
             c = command.from_frame(f, dt)
             if c.response:
                 self.assertRaises(TypeError, lambda: c.response('wibble'))
                 self.assertHasAttr(
                     c.response(None), 'raw_value')
 
     def test_queryextendedversionnumber(self):
```

### Comparing `python-dali-0.8/dali/tests/test_exceptions.py` & `python-dali-0.9/dali/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/tests/test_frame.py` & `python-dali-0.9/dali/tests/test_frame.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.assertRaises(ValueError, frame.Frame, 16, 0x1ffff)
         self.assertRaises(ValueError, frame.Frame, 16, -1)
         self.assertEqual(len(frame.Frame(16, 0xffff)), 16)
         self.assertEqual(len(frame.Frame(256, 1 << 255)), 256)
 
     def test_frame_init_data(self):
         """frames can be initialised with integer or iterable data"""
-        # In release 0.8, Frame defaults to new_exceptions=False
+        # In release 0.9, Frame defaults to new_exceptions=True
         with self.assertWarns(DeprecationWarning):
             self.assertEqual(
                 frame.Frame(16, 0xffff),
                 frame.Frame(16, (0xff, 0xff), new_exceptions=False)
             )
             self.assertNotEqual(
                 frame.Frame(16, 0xffff),
@@ -30,29 +30,27 @@
             self.assertEqual(
                 frame.Frame(16, 0xffff),
                 frame.Frame(16, (0, 0, 0xff, 0xff), new_exceptions=False)
             )
             self.assertRaises(TypeError, frame.Frame, 24, (0x100, 0xff),
                               new_exceptions=False)
 
-        # In release 0.9, Frame will default to new_exceptions=True
         self.assertEqual(
             frame.Frame(16, 0xffff),
-            frame.Frame(16, (0xff, 0xff), new_exceptions=True)
+            frame.Frame(16, (0xff, 0xff))
         )
         self.assertNotEqual(
             frame.Frame(16, 0xffff),
-            frame.Frame(16, (0xff, 0xfe), new_exceptions=True)
+            frame.Frame(16, (0xff, 0xfe))
         )
         self.assertEqual(
             frame.Frame(16, 0xffff),
-            frame.Frame(16, (0, 0, 0xff, 0xff), new_exceptions=True)
+            frame.Frame(16, (0, 0, 0xff, 0xff))
         )
-        self.assertRaises(ValueError, frame.Frame, 24, (0x100, 0xff),
-                          new_exceptions=True)
+        self.assertRaises(ValueError, frame.Frame, 24, (0x100, 0xff))
 
         # In release 0.10 (or whatever we decide to call it), passing
         # any value for new_exceptions will cause a warning, and in
         # the release after that new_exceptions will be removed
 
     def test_comparisons(self):
         """frame comparisons"""
@@ -62,15 +60,15 @@
         self.assertEqual(frame.Frame(1) == frame.Frame(2), False)
         self.assertEqual(frame.Frame(1) != frame.Frame(2), True)
 
     def test_read(self):
         """frames return correct values when read using index"""
         # Frame will be 0001 0010 0011 0100 0101 0110
         # Index:        3210 9876 5432 1098 7654 3210
-        f = frame.Frame(24, (0x12, 0x34, 0x56), new_exceptions=True)
+        f = frame.Frame(24, (0x12, 0x34, 0x56))
         self.assertEqual(f[0], False)
         self.assertEqual(f[1], True)
         self.assertEqual(f[20], True)
         self.assertRaises(IndexError, lambda: f[24])
         self.assertRaises(IndexError, lambda: f[-1])
         self.assertRaises(TypeError, lambda: f['wibble'])
         self.assertRaises(TypeError, lambda: f[3:0:2])
@@ -139,27 +137,26 @@
     def test_as_integer(self):
         """returning frame as integer works as expected"""
         self.assertEqual(frame.Frame(32, 0x12345678).as_integer, 0x12345678)
 
     def test_as_byte_sequence(self):
         """constructing frames from byte sequence works as expected"""
         f = frame.Frame(29, 0x12345678)
-        self.assertEqual(frame.Frame(29, f.as_byte_sequence,
-                                     new_exceptions=True), f)
+        self.assertEqual(frame.Frame(29, f.as_byte_sequence), f)
 
     def test_pack(self):
         """frame packing return expected byte strings"""
         f = frame.Frame(28, 0x2345678)
         self.assertEqual(f.pack, b'\x02\x34\x56\x78')
         f = frame.Frame(16, 0xaa55)
         self.assertEqual(f.pack, b'\xaa\x55')
 
     def test_pack_len(self):
         """frame packing with length returns expected byte strings"""
-        # In release 0.8, pack_len defaults to new_exceptions=False
+        # In release 0.9, pack_len defaults to new_exceptions=True
         with self.assertWarns(DeprecationWarning):
             f = frame.Frame(28, 0x2345678)
             self.assertRaises(ValueError, lambda: f.pack_len(
                 3, new_exceptions=False))
             self.assertEqual(f.pack_len(4, new_exceptions=False),
                              b'\x02\x34\x56\x78')
             self.assertEqual(f.pack_len(5, new_exceptions=False),
@@ -168,29 +165,22 @@
             self.assertRaises(ValueError, lambda: f.pack_len(
                 0, new_exceptions=False))
             self.assertEqual(f.pack_len(2, new_exceptions=False),
                              b'\xaa\x55')
             self.assertEqual(f.pack_len(4, new_exceptions=False),
                              b'\x00\x00\xaa\x55')
 
-        # In release 0.9, pack_len will default to new_exceptions=True
         f = frame.Frame(28, 0x2345678)
-        self.assertRaises(OverflowError, lambda: f.pack_len(
-            3, new_exceptions=True))
-        self.assertEqual(f.pack_len(4, new_exceptions=True),
-                         b'\x02\x34\x56\x78')
-        self.assertEqual(f.pack_len(5, new_exceptions=True),
-                         b'\x00\x02\x34\x56\x78')
+        self.assertRaises(OverflowError, lambda: f.pack_len(3))
+        self.assertEqual(f.pack_len(4), b'\x02\x34\x56\x78')
+        self.assertEqual(f.pack_len(5), b'\x00\x02\x34\x56\x78')
         f = frame.Frame(16, 0xaa55)
-        self.assertRaises(OverflowError, lambda: f.pack_len(
-            0, new_exceptions=True))
-        self.assertEqual(f.pack_len(2, new_exceptions=True),
-                         b'\xaa\x55')
-        self.assertEqual(f.pack_len(4, new_exceptions=True),
-                         b'\x00\x00\xaa\x55')
+        self.assertRaises(OverflowError, lambda: f.pack_len(0))
+        self.assertEqual(f.pack_len(2), b'\xaa\x55')
+        self.assertEqual(f.pack_len(4), b'\x00\x00\xaa\x55')
 
         # In release 0.10 (or whatever we decide to call it), passing
         # any value for new_exceptions will cause a warning, and in
         # the release after that new_exceptions will be removed
 
     def test_contains(self):
         """frame __contains__ method works as expected"""
```

### Comparing `python-dali-0.8/dali/tests/test_memory.py` & `python-dali-0.9/dali/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/dali/tests/test_sequences.py` & `python-dali-0.9/dali/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/python_dali.egg-info/PKG-INFO` & `python-dali-0.9/python_dali.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dali
-Version: 0.8
+Version: 0.9
 Summary: Interface to DALI lighting systems
 Home-page: https://github.com/sde1000/python-dali
 Author: Stephen Early
 Author-email: steve@assorted.org.uk
 License: LGPL3+
 Description: python-dali — lighting control interface
         ========================================
@@ -119,15 +119,15 @@
         
         - Ferdinand Keil
         
         
         Copyright
         ---------
         
-        python-dali is Copyright (C) 2013–2021 Stephen Early <steve@assorted.org.uk>
+        python-dali is Copyright (C) 2013–2022 Stephen Early <steve@assorted.org.uk>
         and other contributors.
         
         It is distributed under the terms of the GNU Lesser General Public
         License as published by the Free Software Foundation, either version 3
         of the License, or (at your option) any later version.
         
         This program is distributed in the hope that it will be useful, but
```

### Comparing `python-dali-0.8/python_dali.egg-info/SOURCES.txt` & `python-dali-0.9/python_dali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-dali-0.8/setup.py` & `python-dali-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='python-dali',
-    version='0.8',
+    version='0.9',
     description='Interface to DALI lighting systems',
     long_description=readme(),
     long_description_content_type='text/x-rst',
     author='Stephen Early',
     author_email='steve@assorted.org.uk',
     url='https://github.com/sde1000/python-dali',
     packages=[
```

