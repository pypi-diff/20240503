# Comparing `tmp/navel-0.2.42.tar.gz` & `tmp/navel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navel-0.2.42.tar", last modified: Wed Feb 21 17:15:34 2024, max compression
+gzip compressed data, was "navel-0.3.0.tar", last modified: Fri May  3 14:29:13 2024, max compression
```

## Comparing `navel-0.2.42.tar` & `navel-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-02-21 17:15:34.505715 navel-0.2.42/
--rw-r--r--   0 builder   (1000) builder   (1000)        0 2024-02-15 17:43:50.000000 navel-0.2.42/LICENSE
--rw-r--r--   0 builder   (1000) builder   (1000)      443 2024-02-21 17:15:34.501715 navel-0.2.42/PKG-INFO
--rw-r--r--   0 builder   (1000) builder   (1000)      688 2024-02-15 17:43:50.000000 navel-0.2.42/pyproject.toml
--rw-r--r--   0 builder   (1000) builder   (1000)       38 2024-02-21 17:15:34.505715 navel-0.2.42/setup.cfg
-drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-02-21 17:15:34.469713 navel-0.2.42/src/
-drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-02-21 17:15:34.485714 navel-0.2.42/src/navel/
--rw-r--r--   0 builder   (1000) builder   (1000)      334 2024-02-21 16:27:08.000000 navel-0.2.42/src/navel/__init__.py
--rw-r--r--   0 builder   (1000) builder   (1000)     2111 2024-02-21 16:27:08.000000 navel-0.2.42/src/navel/_async.py
--rw-r--r--   0 builder   (1000) builder   (1000)     7207 2024-02-15 17:43:50.000000 navel-0.2.42/src/navel/_data_structs.py
--rw-r--r--   0 builder   (1000) builder   (1000)     4733 2024-02-21 16:27:08.000000 navel-0.2.42/src/navel/_interface.py
--rw-r--r--   0 builder   (1000) builder   (1000)    28166 2024-02-21 16:27:08.000000 navel-0.2.42/src/navel/_messages.py
-drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-02-21 17:15:34.497715 navel-0.2.42/src/navel/_pyproto/
--rw-r--r--   0 builder   (1000) builder   (1000)        0 2024-02-21 17:14:12.000000 navel-0.2.42/src/navel/_pyproto/__init__.py
--rw-r--r--   0 builder   (1000) builder   (1000)     2866 2024-02-21 17:14:12.000000 navel-0.2.42/src/navel/_pyproto/config_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     2243 2024-02-21 17:14:13.000000 navel-0.2.42/src/navel/_pyproto/coord_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     1905 2024-02-21 17:14:13.000000 navel-0.2.42/src/navel/_pyproto/klframe_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     3443 2024-02-21 17:14:13.000000 navel-0.2.42/src/navel/_pyproto/payload_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     3268 2024-02-21 17:14:13.000000 navel-0.2.42/src/navel/_pyproto/perc_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     1288 2024-02-21 17:14:14.000000 navel-0.2.42/src/navel/_pyproto/speech_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     1014 2024-02-21 17:14:14.000000 navel-0.2.42/src/navel/_pyproto/sys_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     1025 2024-02-21 17:14:14.000000 navel-0.2.42/src/navel/_pyproto/uuid_pb2.py
--rw-r--r--   0 builder   (1000) builder   (1000)     2063 2024-02-15 17:43:50.000000 navel-0.2.42/src/navel/_socket_coms.py
--rw-r--r--   0 builder   (1000) builder   (1000)       73 2024-02-21 17:14:11.000000 navel-0.2.42/src/navel/_version.py
-drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-02-21 17:15:34.501715 navel-0.2.42/src/navel.egg-info/
--rw-r--r--   0 builder   (1000) builder   (1000)      443 2024-02-21 17:15:34.000000 navel-0.2.42/src/navel.egg-info/PKG-INFO
--rw-r--r--   0 builder   (1000) builder   (1000)      685 2024-02-21 17:15:34.000000 navel-0.2.42/src/navel.egg-info/SOURCES.txt
--rw-r--r--   0 builder   (1000) builder   (1000)        1 2024-02-21 17:15:34.000000 navel-0.2.42/src/navel.egg-info/dependency_links.txt
--rw-r--r--   0 builder   (1000) builder   (1000)       19 2024-02-21 17:15:34.000000 navel-0.2.42/src/navel.egg-info/requires.txt
--rw-r--r--   0 builder   (1000) builder   (1000)        6 2024-02-21 17:15:34.000000 navel-0.2.42/src/navel.egg-info/top_level.txt
-drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-02-21 17:15:34.501715 navel-0.2.42/tests/
--rw-r--r--   0 builder   (1000) builder   (1000)      531 2024-02-15 17:43:50.000000 navel-0.2.42/tests/test_app_running.py
--rw-r--r--   0 builder   (1000) builder   (1000)      804 2024-02-15 17:43:50.000000 navel-0.2.42/tests/test_async.py
+drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-05-03 14:29:13.217614 navel-0.3.0/
+-rw-r--r--   0 builder   (1000) builder   (1000)        0 2024-02-15 17:43:50.000000 navel-0.3.0/LICENSE
+-rw-r--r--   0 builder   (1000) builder   (1000)      442 2024-05-03 14:29:13.213614 navel-0.3.0/PKG-INFO
+-rw-r--r--   0 builder   (1000) builder   (1000)      688 2024-02-15 17:43:50.000000 navel-0.3.0/pyproject.toml
+-rw-r--r--   0 builder   (1000) builder   (1000)       38 2024-05-03 14:29:13.217614 navel-0.3.0/setup.cfg
+drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-05-03 14:29:13.181612 navel-0.3.0/src/
+drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-05-03 14:29:13.193613 navel-0.3.0/src/navel/
+-rw-r--r--   0 builder   (1000) builder   (1000)      334 2024-02-21 16:27:08.000000 navel-0.3.0/src/navel/__init__.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     2111 2024-02-21 16:27:08.000000 navel-0.3.0/src/navel/_async.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     7213 2024-03-05 17:33:08.000000 navel-0.3.0/src/navel/_data_structs.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     4733 2024-02-21 16:27:08.000000 navel-0.3.0/src/navel/_interface.py
+-rw-r--r--   0 builder   (1000) builder   (1000)    28163 2024-02-29 11:40:03.000000 navel-0.3.0/src/navel/_messages.py
+drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-05-03 14:29:13.209614 navel-0.3.0/src/navel/_pyproto/
+-rw-r--r--   0 builder   (1000) builder   (1000)        0 2024-05-03 14:27:37.000000 navel-0.3.0/src/navel/_pyproto/__init__.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     2866 2024-05-03 14:27:37.000000 navel-0.3.0/src/navel/_pyproto/config_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     2243 2024-05-03 14:27:38.000000 navel-0.3.0/src/navel/_pyproto/coord_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     1905 2024-05-03 14:27:38.000000 navel-0.3.0/src/navel/_pyproto/klframe_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     3443 2024-05-03 14:27:38.000000 navel-0.3.0/src/navel/_pyproto/payload_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     3268 2024-05-03 14:27:38.000000 navel-0.3.0/src/navel/_pyproto/perc_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     1288 2024-05-03 14:27:38.000000 navel-0.3.0/src/navel/_pyproto/speech_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     1014 2024-05-03 14:27:39.000000 navel-0.3.0/src/navel/_pyproto/sys_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     1025 2024-05-03 14:27:39.000000 navel-0.3.0/src/navel/_pyproto/uuid_pb2.py
+-rw-r--r--   0 builder   (1000) builder   (1000)     2063 2024-02-15 17:43:50.000000 navel-0.3.0/src/navel/_socket_coms.py
+-rw-r--r--   0 builder   (1000) builder   (1000)       72 2024-05-03 14:27:36.000000 navel-0.3.0/src/navel/_version.py
+drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-05-03 14:29:13.213614 navel-0.3.0/src/navel.egg-info/
+-rw-r--r--   0 builder   (1000) builder   (1000)      442 2024-05-03 14:29:13.000000 navel-0.3.0/src/navel.egg-info/PKG-INFO
+-rw-r--r--   0 builder   (1000) builder   (1000)      685 2024-05-03 14:29:13.000000 navel-0.3.0/src/navel.egg-info/SOURCES.txt
+-rw-r--r--   0 builder   (1000) builder   (1000)        1 2024-05-03 14:29:13.000000 navel-0.3.0/src/navel.egg-info/dependency_links.txt
+-rw-r--r--   0 builder   (1000) builder   (1000)       19 2024-05-03 14:29:13.000000 navel-0.3.0/src/navel.egg-info/requires.txt
+-rw-r--r--   0 builder   (1000) builder   (1000)        6 2024-05-03 14:29:13.000000 navel-0.3.0/src/navel.egg-info/top_level.txt
+drwxr-xr-x   0 builder   (1000) builder   (1000)        0 2024-05-03 14:29:13.213614 navel-0.3.0/tests/
+-rw-r--r--   0 builder   (1000) builder   (1000)      531 2024-02-15 17:43:50.000000 navel-0.3.0/tests/test_app_running.py
+-rw-r--r--   0 builder   (1000) builder   (1000)      804 2024-02-15 17:43:50.000000 navel-0.3.0/tests/test_async.py
```

### Comparing `navel-0.2.42/pyproject.toml` & `navel-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_async.py` & `navel-0.3.0/src/navel/_async.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_data_structs.py` & `navel-0.3.0/src/navel/_data_structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             Defaults to None.
         gaze (CartVec3d): Vector describing persons direction of gaze.
             Defaults to None.
         facial_expression (PersonFacialExpression): Person's facial expression.
             Defaults to None.
         dist_mm (float): Distance from robot to person (mm).
             Defaults to None.
-        g_overlap (float): How much person is staring at robot, 0 = not
+        gaze_overlap (float): How much person is staring at robot, 0 = not
             looking at robot, 1 = looking directly at robot.
             Defaults to None.
         g_eye_left (CartSys3d): A list of the position of left eye in all coord
             frames. This might be out of frame, then sys is CoordSystem.UNDEFINED.
             Defaults to None.
         g_eye_right (CartSys3d): A list of the position of right eye in all
             coord frames. This might be out of frame, then sys is
@@ -199,15 +199,15 @@
     uuid: float | None = None
     face: Bbox2d | None = None
     landmarks: PersonLandmarks | None = None
     head_position: Bryan | None = None
     gaze: CartVec3d | None = None
     facial_expression: PersonFacialExpression | None = None
     dist_mm: float | None = None
-    g_overlap: float | None = None
+    gaze_overlap: float | None = None
     g_eye_left: CartSys3d | None = None
     g_eye_right: CartSys3d | None = None
     g_nose: CartSys3d | None = None
     g_head_position: CartSys3d | None = None
     g_gaze: CartSys3d | None = None
```

### Comparing `navel-0.2.42/src/navel/_interface.py` & `navel-0.3.0/src/navel/_interface.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_messages.py` & `navel-0.3.0/src/navel/_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,15 +714,15 @@
                 in seconds. Defaults to 1.
 
         Raises:
             ConnectionAbortedError: If socket connection is lost
             TimeoutError: If timeout is triggered.
 
         Returns:
-            Awaitable[ds.PerceptionData]: The received perception data.
+            Awaitable[PerceptionData]: The received perception data.
         """
         start = time.time()
         match = None
         while time.time() - start < timeout:
             try:
                 msg = self._perc_sock.recv()
             except BlockingIOError:
```

### Comparing `navel-0.2.42/src/navel/_pyproto/config_pb2.py` & `navel-0.3.0/src/navel/_pyproto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/coord_pb2.py` & `navel-0.3.0/src/navel/_pyproto/coord_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/klframe_pb2.py` & `navel-0.3.0/src/navel/_pyproto/klframe_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/payload_pb2.py` & `navel-0.3.0/src/navel/_pyproto/payload_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/perc_pb2.py` & `navel-0.3.0/src/navel/_pyproto/perc_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/speech_pb2.py` & `navel-0.3.0/src/navel/_pyproto/speech_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/sys_pb2.py` & `navel-0.3.0/src/navel/_pyproto/sys_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_pyproto/uuid_pb2.py` & `navel-0.3.0/src/navel/_pyproto/uuid_pb2.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel/_socket_coms.py` & `navel-0.3.0/src/navel/_socket_coms.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/src/navel.egg-info/SOURCES.txt` & `navel-0.3.0/src/navel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/tests/test_app_running.py` & `navel-0.3.0/tests/test_app_running.py`

 * *Files identical despite different names*

### Comparing `navel-0.2.42/tests/test_async.py` & `navel-0.3.0/tests/test_async.py`

 * *Files identical despite different names*

