# Comparing `tmp/trame-vtklocal-0.1.0.tar.gz` & `tmp/trame-vtklocal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtklocal-0.1.0.tar", last modified: Fri Apr 19 17:06:38 2024, max compression
+gzip compressed data, was "trame-vtklocal-0.2.0.tar", last modified: Thu May  2 23:22:16 2024, max compression
```

## Comparing `trame-vtklocal-0.1.0.tar` & `trame-vtklocal-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.369640 trame-vtklocal-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      583 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2238 2024-04-19 17:06:38.369640 trame-vtklocal-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1478 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      896 2024-04-19 17:06:38.369640 trame-vtklocal-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame/modules/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame/widgets/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame_vtklocal/
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame_vtklocal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame_vtklocal/module/
--rw-r--r--   0 root         (0) root         (0)      873 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame_vtklocal/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4331 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame_vtklocal/module/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.361640 trame-vtklocal-0.1.0/trame_vtklocal/module/serve/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame_vtklocal/module/serve/js/
--rw-r--r--   0 root         (0) root         (0)     4135 2024-04-19 17:06:34.000000 trame-vtklocal-0.1.0/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js
--rw-r--r--   0 root         (0) root         (0)     1620 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame_vtklocal/module/wasm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame_vtklocal/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame_vtklocal/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1694 2024-04-19 17:06:14.000000 trame-vtklocal-0.1.0/trame_vtklocal/widgets/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:06:38.365640 trame-vtklocal-0.1.0/trame_vtklocal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2238 2024-04-19 17:06:38.000000 trame-vtklocal-0.1.0/trame_vtklocal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-19 17:06:38.000000 trame-vtklocal-0.1.0/trame_vtklocal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 17:06:38.000000 trame-vtklocal-0.1.0/trame_vtklocal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-19 17:06:38.000000 trame-vtklocal-0.1.0/trame_vtklocal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 17:06:38.000000 trame-vtklocal-0.1.0/trame_vtklocal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      896 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.640755 trame-vtklocal-0.2.0/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame/modules/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame/widgets/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame_vtklocal/
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame_vtklocal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame_vtklocal/module/
+-rw-r--r--   0 root         (0) root         (0)      873 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame_vtklocal/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4331 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame_vtklocal/module/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.640755 trame-vtklocal-0.2.0/trame_vtklocal/module/serve/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame_vtklocal/module/serve/js/
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-02 23:22:13.000000 trame-vtklocal-0.2.0/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame_vtklocal/module/wasm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame_vtklocal/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame_vtklocal/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-05-02 23:21:53.000000 trame-vtklocal-0.2.0/trame_vtklocal/widgets/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 23:22:16.644755 trame-vtklocal-0.2.0/trame_vtklocal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-02 23:22:16.000000 trame-vtklocal-0.2.0/trame_vtklocal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-02 23:22:16.000000 trame-vtklocal-0.2.0/trame_vtklocal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 23:22:16.000000 trame-vtklocal-0.2.0/trame_vtklocal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-02 23:22:16.000000 trame-vtklocal-0.2.0/trame_vtklocal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-02 23:22:16.000000 trame-vtklocal-0.2.0/trame_vtklocal.egg-info/top_level.txt
```

### Comparing `trame-vtklocal-0.1.0/LICENSE` & `trame-vtklocal-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.1.0/PKG-INFO` & `trame-vtklocal-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtklocal
-Version: 0.1.0
+Version: 0.2.0
 Summary: VTK Local Rendering using WASM
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -71,7 +71,11 @@
     # We need a VTK that has its wasm counterpart
     # This is the first version available with it
     # For ParaView (not yet supported), VTK don't need to be installed
     pip install "vtk==9.3.20240418.dev0" --extra-index-url https://wheels.vtk.org
 
     # regular trame app
     python ./examples/vtk/cone.py 
+
+
+Some example are meant to test and validate WASM rendering.
+Some will default for remote rendering but if you want to force them to use WASM just run `export USE_WASM=1` before executing them.
```

### Comparing `trame-vtklocal-0.1.0/README.rst` & `trame-vtklocal-0.2.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -52,7 +52,11 @@
     # We need a VTK that has its wasm counterpart
     # This is the first version available with it
     # For ParaView (not yet supported), VTK don't need to be installed
     pip install "vtk==9.3.20240418.dev0" --extra-index-url https://wheels.vtk.org
 
     # regular trame app
     python ./examples/vtk/cone.py 
+
+
+Some example are meant to test and validate WASM rendering.
+Some will default for remote rendering but if you want to force them to use WASM just run `export USE_WASM=1` before executing them.
```

### Comparing `trame-vtklocal-0.1.0/setup.cfg` & `trame-vtklocal-0.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtklocal
-version = 0.1.0
+version = 0.2.0
 description = VTK Local Rendering using WASM
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-vtklocal-0.1.0/trame_vtklocal/module/__init__.py` & `trame-vtklocal-0.2.0/trame_vtklocal/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.1.0/trame_vtklocal/module/protocol.py` & `trame-vtklocal-0.2.0/trame_vtklocal/module/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.1.0/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js` & `trame-vtklocal-0.2.0/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.1.0/trame_vtklocal/module/wasm.py` & `trame-vtklocal-0.2.0/trame_vtklocal/module/wasm.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.1.0/trame_vtklocal.egg-info/PKG-INFO` & `trame-vtklocal-0.2.0/trame_vtklocal.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtklocal
-Version: 0.1.0
+Version: 0.2.0
 Summary: VTK Local Rendering using WASM
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -71,7 +71,11 @@
     # We need a VTK that has its wasm counterpart
     # This is the first version available with it
     # For ParaView (not yet supported), VTK don't need to be installed
     pip install "vtk==9.3.20240418.dev0" --extra-index-url https://wheels.vtk.org
 
     # regular trame app
     python ./examples/vtk/cone.py 
+
+
+Some example are meant to test and validate WASM rendering.
+Some will default for remote rendering but if you want to force them to use WASM just run `export USE_WASM=1` before executing them.
```

### Comparing `trame-vtklocal-0.1.0/trame_vtklocal.egg-info/SOURCES.txt` & `trame-vtklocal-0.2.0/trame_vtklocal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

