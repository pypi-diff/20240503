# Comparing `tmp/OpenGeodeWeb-Viewer-0.1.1rc2.tar.gz` & `tmp/opengeodeweb_viewer-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenGeodeWeb-Viewer-0.1.1rc2.tar", last modified: Wed Mar 13 10:32:04 2024, max compression
+gzip compressed data, was "opengeodeweb_viewer-0.1.2rc1.tar", last modified: Fri May  3 10:03:40 2024, max compression
```

## Comparing `OpenGeodeWeb-Viewer-0.1.1rc2.tar` & `opengeodeweb_viewer-0.1.2rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.992474 OpenGeodeWeb-Viewer-0.1.1rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-13 10:32:04.992474 OpenGeodeWeb-Viewer-0.1.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 10:32:04.992474 OpenGeodeWeb-Viewer-0.1.1rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.984474 OpenGeodeWeb-Viewer-0.1.1rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.988474 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-13 10:32:04.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-13 10:32:04.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:32:04.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 10:32:04.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-13 10:32:04.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-13 10:32:04.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.988474 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.984474 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.988474 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/apply_textures.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/create_object_pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/create_visualization.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/delete_object_pipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/get_point_position.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/point_size.json
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/reset.json
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/reset_camera.json
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/set_color.json
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/set_vertex_attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/toggle_edge_visibility.json
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/toggle_object_visibility.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/toggle_point_visibility.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/update_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/vtk_override_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/vtk_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/vtkw_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:32:04.988474 OpenGeodeWeb-Viewer-0.1.1rc2/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-13 10:31:54.000000 OpenGeodeWeb-Viewer-0.1.1rc2/src/tests/test_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.140978 opengeodeweb_viewer-0.1.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-03 10:03:40.140978 opengeodeweb_viewer-0.1.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 10:03:31.000000 opengeodeweb_viewer-0.1.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:03:40.140978 opengeodeweb_viewer-0.1.2rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.132978 opengeodeweb_viewer-0.1.2rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.140978 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-03 10:03:40.000000 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-03 10:03:40.000000 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:03:40.000000 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 10:03:40.000000 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-03 10:03:40.000000 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 10:03:40.000000 opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.136978 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.132978 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.140978 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/apply_textures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/create_object_pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/create_visualization.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/delete_object_pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/get_point_position.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/point_size.json
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/reset.json
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/reset_camera.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/set_color.json
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/set_vertex_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/toggle_edge_visibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/toggle_object_visibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/toggle_point_visibility.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/update_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/vtk_override_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/vtk_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/vtkw_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:40.140978 opengeodeweb_viewer-0.1.2rc1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-03 10:03:30.000000 opengeodeweb_viewer-0.1.2rc1/src/tests/test_protocol.py
```

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/LICENSE` & `opengeodeweb_viewer-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/PKG-INFO` & `opengeodeweb_viewer-0.1.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Viewer
-Version: 0.1.1rc2
+Version: 0.1.2rc1
 Summary: OpenGeodeWeb-Viewer is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/pyproject.toml` & `opengeodeweb_viewer-0.1.2rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Viewer"
-version = "0.1.1-rc.2"
+version = "0.1.2-rc.1"
 dynamic = ["dependencies"]
 authors = [
   { name="Geode-solutions", email="team-web@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Viewer is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/requirements.txt` & `opengeodeweb_viewer-0.1.2rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO` & `opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Viewer
-Version: 0.1.1rc2
+Version: 0.1.2rc1
 Summary: OpenGeodeWeb-Viewer is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/OpenGeodeWeb_Viewer.egg-info/SOURCES.txt` & `opengeodeweb_viewer-0.1.2rc1/src/OpenGeodeWeb_Viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/config.py` & `opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/config.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/rpc/schemas/apply_textures.json` & `opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/rpc/schemas/apply_textures.json`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/vtk_override_protocols.py` & `opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/vtk_override_protocols.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/vtk_protocol.py` & `opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/vtk_protocol.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/opengeodeweb_viewer/vtkw_server.py` & `opengeodeweb_viewer-0.1.2rc1/src/opengeodeweb_viewer/vtkw_server.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/tests/conftest.py` & `opengeodeweb_viewer-0.1.2rc1/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.1.1rc2/src/tests/test_protocol.py` & `opengeodeweb_viewer-0.1.2rc1/src/tests/test_protocol.py`

 * *Files identical despite different names*

