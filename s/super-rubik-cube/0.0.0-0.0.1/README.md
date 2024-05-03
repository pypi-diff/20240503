# Comparing `tmp/super_rubik_cube-0.0.0.tar.gz` & `tmp/super_rubik_cube-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_rubik_cube-0.0.0.tar", last modified: Fri May  3 19:55:50 2024, max compression
+gzip compressed data, was "super_rubik_cube-0.0.1.tar", last modified: Fri May  3 20:15:38 2024, max compression
```

## Comparing `super_rubik_cube-0.0.0.tar` & `super_rubik_cube-0.0.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 19:55:50.594475 super_rubik_cube-0.0.0/
--rw-rw-rw-   0        0        0      347 2024-05-03 19:55:50.593940 super_rubik_cube-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-03 19:55:50.594475 super_rubik_cube-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      541 2024-05-03 19:55:32.000000 super_rubik_cube-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:55:50.592943 super_rubik_cube-0.0.0/super_rubik_cube.egg-info/
--rw-rw-rw-   0        0        0      347 2024-05-03 19:55:50.000000 super_rubik_cube-0.0.0/super_rubik_cube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1253 2024-05-03 19:55:50.000000 super_rubik_cube-0.0.0/super_rubik_cube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 19:55:50.000000 super_rubik_cube-0.0.0/super_rubik_cube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 19:55:50.000000 super_rubik_cube-0.0.0/super_rubik_cube.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 19:55:50.572383 super_rubik_cube-0.0.0/supercube/
--rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-0.0.0/supercube/NCube.py
--rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-0.0.0/supercube/PocketCube.py
--rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-0.0.0/supercube/RubiksCube.py
--rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-0.0.0/supercube/__init__.py
--rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-0.0.0/supercube/cube.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:55:50.574381 super_rubik_cube-0.0.0/supercube/kociemba/
--rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-0.0.0/supercube/kociemba/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/build_ckociemba.py
--rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/command_line.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:55:50.581431 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/
--rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/__init__.py
--rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/color.py
--rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/coordcube.py
--rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/corner.py
--rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/cubiecube.py
--rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/edge.py
--rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/facecube.py
--rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/facelet.py
--rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/search.py
--rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:55:50.592943 super_rubik_cube-0.0.0/supercube/kociemba_2x2/
--rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/__init__.py
--rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/client_gui.py
--rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/coord.py
--rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/cubie.py
--rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/defs.py
--rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/enums.py
--rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/example.py
--rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/face.py
--rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/misc.py
--rw-rw-rw-   0        0        0     2177 2024-05-03 18:32:52.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/moves.py
--rw-rw-rw-   0        0        0     1928 2024-05-03 18:32:52.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/pruning.py
--rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/sockets.py
--rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/solver.py
--rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.0/supercube/kociemba_2x2/start_server.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:15:38.308268 super_rubik_cube-0.0.1/
+-rw-rw-rw-   0        0        0    35816 2024-05-03 20:00:15.000000 super_rubik_cube-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0    20687 2024-05-03 20:15:38.307270 super_rubik_cube-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20351 2024-05-03 20:00:15.000000 super_rubik_cube-0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 20:15:38.308268 super_rubik_cube-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0    20915 2024-05-03 20:14:51.000000 super_rubik_cube-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:15:38.306268 super_rubik_cube-0.0.1/super_rubik_cube.egg-info/
+-rw-rw-rw-   0        0        0    20687 2024-05-03 20:15:38.000000 super_rubik_cube-0.0.1/super_rubik_cube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1271 2024-05-03 20:15:38.000000 super_rubik_cube-0.0.1/super_rubik_cube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 20:15:38.000000 super_rubik_cube-0.0.1/super_rubik_cube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 20:15:38.000000 super_rubik_cube-0.0.1/super_rubik_cube.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 20:15:38.288486 super_rubik_cube-0.0.1/supercube/
+-rw-rw-rw-   0        0        0      297 2024-05-03 15:53:19.000000 super_rubik_cube-0.0.1/supercube/NCube.py
+-rw-rw-rw-   0        0        0     1215 2024-05-03 17:20:04.000000 super_rubik_cube-0.0.1/supercube/PocketCube.py
+-rw-rw-rw-   0        0        0     1207 2024-05-03 17:17:11.000000 super_rubik_cube-0.0.1/supercube/RubiksCube.py
+-rw-rw-rw-   0        0        0       96 2024-05-03 15:43:15.000000 super_rubik_cube-0.0.1/supercube/__init__.py
+-rw-rw-rw-   0        0        0    31193 2024-04-14 21:26:56.000000 super_rubik_cube-0.0.1/supercube/cube.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:15:38.290483 super_rubik_cube-0.0.1/supercube/kociemba/
+-rw-rw-rw-   0        0        0     1462 2024-05-03 17:19:32.000000 super_rubik_cube-0.0.1/supercube/kociemba/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/build_ckociemba.py
+-rw-rw-rw-   0        0        0      413 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/command_line.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:15:38.297053 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/
+-rw-rw-rw-   0        0        0        0 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/color.py
+-rw-rw-rw-   0        0        0    19234 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/coordcube.py
+-rw-rw-rw-   0        0        0      529 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/corner.py
+-rw-rw-rw-   0        0        0    20176 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/cubiecube.py
+-rw-rw-rw-   0        0        0      598 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/edge.py
+-rw-rw-rw-   0        0        0     4060 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/facecube.py
+-rw-rw-rw-   0        0        0     3178 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/facelet.py
+-rw-rw-rw-   0        0        0    13523 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/search.py
+-rw-rw-rw-   0        0        0     2485 2024-03-25 18:55:50.000000 super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 20:15:38.305268 super_rubik_cube-0.0.1/supercube/kociemba_2x2/
+-rw-rw-rw-   0        0        0        0 2024-04-02 12:07:35.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/__init__.py
+-rw-rw-rw-   0        0        0     7752 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/client_gui.py
+-rw-rw-rw-   0        0        0     1150 2024-05-03 17:23:20.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/coord.py
+-rw-rw-rw-   0        0        0     7188 2024-05-03 17:22:29.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/cubie.py
+-rw-rw-rw-   0        0        0     1122 2024-05-03 17:21:59.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/defs.py
+-rw-rw-rw-   0        0        0     2021 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/enums.py
+-rw-rw-rw-   0        0        0     2980 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/example.py
+-rw-rw-rw-   0        0        0     4874 2024-05-03 17:21:50.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/face.py
+-rw-rw-rw-   0        0        0      493 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/misc.py
+-rw-rw-rw-   0        0        0     2177 2024-05-03 18:32:52.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/moves.py
+-rw-rw-rw-   0        0        0     1928 2024-05-03 18:32:52.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/pruning.py
+-rw-rw-rw-   0        0        0     2598 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/sockets.py
+-rw-rw-rw-   0        0        0     2758 2024-05-03 17:21:32.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/solver.py
+-rw-rw-rw-   0        0        0      412 2024-03-29 20:50:57.000000 super_rubik_cube-0.0.1/supercube/kociemba_2x2/start_server.py
```

### Comparing `super_rubik_cube-0.0.0/super_rubik_cube.egg-info/SOURCES.txt` & `super_rubik_cube-0.0.1/super_rubik_cube.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 super_rubik_cube.egg-info/PKG-INFO
 super_rubik_cube.egg-info/SOURCES.txt
 super_rubik_cube.egg-info/dependency_links.txt
 super_rubik_cube.egg-info/top_level.txt
 supercube/NCube.py
 supercube/PocketCube.py
```

### Comparing `super_rubik_cube-0.0.0/supercube/PocketCube.py` & `super_rubik_cube-0.0.1/supercube/PocketCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/RubiksCube.py` & `super_rubik_cube-0.0.1/supercube/RubiksCube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/cube.py` & `super_rubik_cube-0.0.1/supercube/cube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/__init__.py` & `super_rubik_cube-0.0.1/supercube/kociemba/__init__.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/build_ckociemba.py` & `super_rubik_cube-0.0.1/supercube/kociemba/build_ckociemba.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/coordcube.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/coordcube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/corner.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/corner.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/cubiecube.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/cubiecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/edge.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/edge.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/facecube.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/facecube.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/facelet.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/facelet.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/search.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/search.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba/pykociemba/tools.py` & `super_rubik_cube-0.0.1/supercube/kociemba/pykociemba/tools.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/client_gui.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/client_gui.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/coord.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/coord.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/cubie.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/cubie.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/defs.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/defs.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/enums.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/enums.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/example.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/example.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/face.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/face.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/moves.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/moves.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/pruning.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/pruning.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/sockets.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/sockets.py`

 * *Files identical despite different names*

### Comparing `super_rubik_cube-0.0.0/supercube/kociemba_2x2/solver.py` & `super_rubik_cube-0.0.1/supercube/kociemba_2x2/solver.py`

 * *Files identical despite different names*

