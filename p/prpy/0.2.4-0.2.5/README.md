# Comparing `tmp/prpy-0.2.4.tar.gz` & `tmp/prpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prpy-0.2.4.tar", last modified: Thu Apr 11 11:02:11 2024, max compression
+gzip compressed data, was "prpy-0.2.5.tar", last modified: Fri May  3 13:14:59 2024, max compression
```

## Comparing `prpy-0.2.4.tar` & `prpy-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.186986 prpy-0.2.4/
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.154375 prpy-0.2.4/.github/
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.157996 prpy-0.2.4/.github/workflows/
--rw-r--r--   0 prouast    (501) staff       (20)     1028 2024-04-10 16:29:37.000000 prpy-0.2.4/.github/workflows/main.yml
--rw-r--r--   0 prouast    (501) staff       (20)     1830 2024-04-10 16:03:39.000000 prpy-0.2.4/.gitignore
--rw-r--r--   0 prouast    (501) staff       (20)     1058 2024-04-10 16:03:39.000000 prpy-0.2.4/LICENSE
--rw-r--r--   0 prouast    (501) staff       (20)      196 2024-04-10 16:06:46.000000 prpy-0.2.4/MANIFEST.in
--rw-r--r--   0 prouast    (501) staff       (20)     2581 2024-04-11 11:02:11.186045 prpy-0.2.4/PKG-INFO
--rw-r--r--   0 prouast    (501) staff       (20)     1148 2024-04-11 10:44:30.000000 prpy-0.2.4/README.md
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.158807 prpy-0.2.4/prpy/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     1209 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/constants.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.162979 prpy-0.2.4/prpy/ffmpeg/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/ffmpeg/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     3126 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/ffmpeg/probe.py
--rw-r--r--   0 prouast    (501) staff       (20)    16981 2024-04-11 10:45:26.000000 prpy-0.2.4/prpy/ffmpeg/readwrite.py
--rw-r--r--   0 prouast    (501) staff       (20)     3195 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/ffmpeg/utils.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.166673 prpy-0.2.4/prpy/numpy/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/numpy/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     8359 2024-04-11 10:23:49.000000 prpy-0.2.4/prpy/numpy/face.py
--rw-r--r--   0 prouast    (501) staff       (20)     7076 2024-04-11 10:46:18.000000 prpy-0.2.4/prpy/numpy/image.py
--rw-r--r--   0 prouast    (501) staff       (20)     6395 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/numpy/metric.py
--rw-r--r--   0 prouast    (501) staff       (20)    21787 2024-04-11 11:00:37.000000 prpy-0.2.4/prpy/numpy/signal.py
--rw-r--r--   0 prouast    (501) staff       (20)     7764 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/numpy/stride_tricks.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.172487 prpy-0.2.4/prpy/tensorflow/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     7554 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/image.py
--rw-r--r--   0 prouast    (501) staff       (20)     4248 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/loss.py
--rw-r--r--   0 prouast    (501) staff       (20)     3384 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/lr_schedule.py
--rw-r--r--   0 prouast    (501) staff       (20)     7660 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/model_saver.py
--rw-r--r--   0 prouast    (501) staff       (20)     8525 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/nan.py
--rw-r--r--   0 prouast    (501) staff       (20)     9844 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/optimizer.py
--rw-r--r--   0 prouast    (501) staff       (20)     3326 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/tensorflow/signal.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.173692 prpy-0.2.4/prpy/torch/
--rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/torch/__init__.py
--rw-r--r--   0 prouast    (501) staff       (20)     7582 2024-04-10 16:03:39.000000 prpy-0.2.4/prpy/torch/model_saver.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.180760 prpy-0.2.4/prpy.egg-info/
--rw-r--r--   0 prouast    (501) staff       (20)     2581 2024-04-11 11:02:11.000000 prpy-0.2.4/prpy.egg-info/PKG-INFO
--rw-r--r--   0 prouast    (501) staff       (20)      977 2024-04-11 11:02:11.000000 prpy-0.2.4/prpy.egg-info/SOURCES.txt
--rw-r--r--   0 prouast    (501) staff       (20)        1 2024-04-11 11:02:11.000000 prpy-0.2.4/prpy.egg-info/dependency_links.txt
--rw-r--r--   0 prouast    (501) staff       (20)      200 2024-04-11 11:02:11.000000 prpy-0.2.4/prpy.egg-info/requires.txt
--rw-r--r--   0 prouast    (501) staff       (20)        5 2024-04-11 11:02:11.000000 prpy-0.2.4/prpy.egg-info/top_level.txt
--rw-r--r--   0 prouast    (501) staff       (20)     1076 2024-04-10 16:07:11.000000 prpy-0.2.4/pyproject.toml
--rw-r--r--   0 prouast    (501) staff       (20)       38 2024-04-11 11:02:11.187164 prpy-0.2.4/setup.cfg
--rw-r--r--   0 prouast    (501) staff       (20)       38 2024-04-10 16:03:39.000000 prpy-0.2.4/setup.py
-drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-04-11 11:02:11.179984 prpy-0.2.4/tests/
--rw-r--r--   0 prouast    (501) staff       (20)     2101 2024-04-10 16:08:25.000000 prpy-0.2.4/tests/conftest.py
--rw-r--r--   0 prouast    (501) staff       (20)     4210 2024-04-10 16:08:34.000000 prpy-0.2.4/tests/test_ffmpeg.py
--rw-r--r--   0 prouast    (501) staff       (20)     3886 2024-04-10 16:08:54.000000 prpy-0.2.4/tests/test_numpy_face.py
--rw-r--r--   0 prouast    (501) staff       (20)     3860 2024-04-10 16:09:05.000000 prpy-0.2.4/tests/test_numpy_image.py
--rw-r--r--   0 prouast    (501) staff       (20)     2499 2024-04-10 16:09:14.000000 prpy-0.2.4/tests/test_numpy_metric.py
--rw-r--r--   0 prouast    (501) staff       (20)    13187 2024-04-10 16:09:26.000000 prpy-0.2.4/tests/test_numpy_signal.py
--rw-r--r--   0 prouast    (501) staff       (20)     2943 2024-04-10 16:10:54.000000 prpy-0.2.4/tests/test_numpy_stride_tricks.py
--rw-r--r--   0 prouast    (501) staff       (20)    29110 2024-04-10 16:09:37.000000 prpy-0.2.4/tests/test_tensorflow.py
--rw-r--r--   0 prouast    (501) staff       (20)     4434 2024-04-10 16:09:41.000000 prpy-0.2.4/tests/test_torch.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.989445 prpy-0.2.5/
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.954886 prpy-0.2.5/.github/
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.958839 prpy-0.2.5/.github/workflows/
+-rw-r--r--   0 prouast    (501) staff       (20)     1028 2024-04-10 16:29:37.000000 prpy-0.2.5/.github/workflows/main.yml
+-rw-r--r--   0 prouast    (501) staff       (20)     1830 2024-04-10 16:03:39.000000 prpy-0.2.5/.gitignore
+-rw-r--r--   0 prouast    (501) staff       (20)     1058 2024-04-10 16:03:39.000000 prpy-0.2.5/LICENSE
+-rw-r--r--   0 prouast    (501) staff       (20)      196 2024-04-10 16:06:46.000000 prpy-0.2.5/MANIFEST.in
+-rw-r--r--   0 prouast    (501) staff       (20)     2581 2024-05-03 13:14:59.988472 prpy-0.2.5/PKG-INFO
+-rw-r--r--   0 prouast    (501) staff       (20)     1148 2024-04-11 10:44:30.000000 prpy-0.2.5/README.md
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.959947 prpy-0.2.5/prpy/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     1209 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/constants.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.964427 prpy-0.2.5/prpy/ffmpeg/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/ffmpeg/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3126 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/ffmpeg/probe.py
+-rw-r--r--   0 prouast    (501) staff       (20)    17039 2024-04-13 18:42:38.000000 prpy-0.2.5/prpy/ffmpeg/readwrite.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3195 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/ffmpeg/utils.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.972590 prpy-0.2.5/prpy/numpy/
+-rw-r--r--   0 prouast    (501) staff       (20)     6148 2024-04-15 07:17:37.000000 prpy-0.2.5/prpy/numpy/.DS_Store
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-13 07:34:48.000000 prpy-0.2.5/prpy/numpy/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     8359 2024-04-12 07:55:23.000000 prpy-0.2.5/prpy/numpy/face.py
+-rw-r--r--   0 prouast    (501) staff       (20)     9066 2024-04-14 07:55:40.000000 prpy-0.2.5/prpy/numpy/image.py
+-rw-r--r--   0 prouast    (501) staff       (20)    12777 2024-04-14 08:03:16.000000 prpy-0.2.5/prpy/numpy/image_ops.c
+-rwxr-xr-x   0 prouast    (501) staff       (20)    34144 2024-04-14 07:52:52.000000 prpy-0.2.5/prpy/numpy/image_ops.cpython-310-darwin.so
+-rw-r--r--   0 prouast    (501) staff       (20)     6395 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/numpy/metric.py
+-rw-r--r--   0 prouast    (501) staff       (20)    21787 2024-04-11 11:03:30.000000 prpy-0.2.5/prpy/numpy/signal.py
+-rwxr-xr-x   0 prouast    (501) staff       (20)    33280 2024-04-13 07:09:13.000000 prpy-0.2.5/prpy/numpy/spam.cpython-310-darwin.so
+-rw-r--r--   0 prouast    (501) staff       (20)     7764 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/numpy/stride_tricks.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.976920 prpy-0.2.5/prpy/tensorflow/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7554 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/image.py
+-rw-r--r--   0 prouast    (501) staff       (20)     4248 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/loss.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3384 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/lr_schedule.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7660 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/model_saver.py
+-rw-r--r--   0 prouast    (501) staff       (20)     8525 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/nan.py
+-rw-r--r--   0 prouast    (501) staff       (20)     9844 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/optimizer.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3326 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/tensorflow/signal.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.977778 prpy-0.2.5/prpy/torch/
+-rw-r--r--   0 prouast    (501) staff       (20)     1093 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/torch/__init__.py
+-rw-r--r--   0 prouast    (501) staff       (20)     7582 2024-04-10 16:03:39.000000 prpy-0.2.5/prpy/torch/model_saver.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.983477 prpy-0.2.5/prpy.egg-info/
+-rw-r--r--   0 prouast    (501) staff       (20)     2581 2024-05-03 13:14:59.000000 prpy-0.2.5/prpy.egg-info/PKG-INFO
+-rw-r--r--   0 prouast    (501) staff       (20)     1102 2024-05-03 13:14:59.000000 prpy-0.2.5/prpy.egg-info/SOURCES.txt
+-rw-r--r--   0 prouast    (501) staff       (20)        1 2024-05-03 13:14:59.000000 prpy-0.2.5/prpy.egg-info/dependency_links.txt
+-rw-r--r--   0 prouast    (501) staff       (20)      200 2024-05-03 13:14:59.000000 prpy-0.2.5/prpy.egg-info/requires.txt
+-rw-r--r--   0 prouast    (501) staff       (20)        5 2024-05-03 13:14:59.000000 prpy-0.2.5/prpy.egg-info/top_level.txt
+-rw-r--r--   0 prouast    (501) staff       (20)     1125 2024-04-13 07:41:38.000000 prpy-0.2.5/pyproject.toml
+-rw-r--r--   0 prouast    (501) staff       (20)       38 2024-05-03 13:14:59.989631 prpy-0.2.5/setup.cfg
+-rw-r--r--   0 prouast    (501) staff       (20)      254 2024-04-13 07:41:31.000000 prpy-0.2.5/setup.py
+drwxr-xr-x   0 prouast    (501) staff       (20)        0 2024-05-03 13:14:59.982754 prpy-0.2.5/tests/
+-rw-r--r--   0 prouast    (501) staff       (20)     2101 2024-04-10 16:08:25.000000 prpy-0.2.5/tests/conftest.py
+-rw-r--r--   0 prouast    (501) staff       (20)     4210 2024-04-10 16:08:34.000000 prpy-0.2.5/tests/test_ffmpeg.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3886 2024-04-10 16:08:54.000000 prpy-0.2.5/tests/test_numpy_face.py
+-rw-r--r--   0 prouast    (501) staff       (20)     3895 2024-04-13 20:22:15.000000 prpy-0.2.5/tests/test_numpy_image.py
+-rw-r--r--   0 prouast    (501) staff       (20)     2499 2024-04-10 16:09:14.000000 prpy-0.2.5/tests/test_numpy_metric.py
+-rw-r--r--   0 prouast    (501) staff       (20)    13187 2024-04-10 16:09:26.000000 prpy-0.2.5/tests/test_numpy_signal.py
+-rw-r--r--   0 prouast    (501) staff       (20)     2943 2024-04-10 16:10:54.000000 prpy-0.2.5/tests/test_numpy_stride_tricks.py
+-rw-r--r--   0 prouast    (501) staff       (20)    29110 2024-04-10 16:09:37.000000 prpy-0.2.5/tests/test_tensorflow.py
+-rw-r--r--   0 prouast    (501) staff       (20)     4434 2024-04-10 16:09:41.000000 prpy-0.2.5/tests/test_torch.py
```

### Comparing `prpy-0.2.4/.github/workflows/main.yml` & `prpy-0.2.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/.gitignore` & `prpy-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/LICENSE` & `prpy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/PKG-INFO` & `prpy-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Collection of Python utils for signal, image, and video processing
 Author-email: Philipp Rouast <philipp@rouast.com>
 License: MIT License
 Project-URL: Repository, https://github.com/prouast/prpy.git
 Project-URL: Issues, https://github.com/prouast/prpy/issues
 Keywords: python,numpy,ffmpeg,tensorflow,torch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prpy-0.2.4/README.md` & `prpy-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/__init__.py` & `prpy-0.2.5/prpy/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/constants.py` & `prpy-0.2.5/prpy/constants.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/ffmpeg/__init__.py` & `prpy-0.2.5/prpy/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/ffmpeg/probe.py` & `prpy-0.2.5/prpy/ffmpeg/probe.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/ffmpeg/readwrite.py` & `prpy-0.2.5/prpy/ffmpeg/readwrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,16 @@
   return stream, target_n, target_w, target_h, ds_factor
 
 def _ffmpeg_output_to_numpy(
     stream: ffmpeg.nodes.FilterableStream,
     r: int,
     fps: Union[float, int, None],
     n: int,
-    w: int,
-    h: int,
+    w: Union[int, np.int64],
+    h: Union[int, np.int64],
     scale: Union[tuple, int, None] = None,
     crf: Union[int, None] = None,
     pix_fmt: str = 'bgr24',
     preserve_aspect_ratio: bool = False,
     scale_algorithm: str = 'bicubic',
     dim_deltas: tuple = (0, 0, 0)
   ) -> np.ndarray:
@@ -199,16 +199,16 @@
   Returns:
     frames: The video frames in shape (n, h, w, c)
   """
   assert isinstance(stream, ffmpeg.nodes.FilterableStream)
   assert isinstance(r, int)
   assert fps is None or isinstance(fps, (float, int))
   assert isinstance(n, int)
-  assert isinstance(w, int)
-  assert isinstance(h, int)
+  assert isinstance(w, (int, np.int64))
+  assert isinstance(h, (int, np.int64))
   assert crf is None or isinstance(crf, int)
   assert isinstance(pix_fmt, str)
   assert isinstance(dim_deltas, tuple) and len(dim_deltas) == 3 and all(isinstance(i, int) for i in dim_deltas)
   if crf is None:
     # Run stream straight to raw video
     stream = stream.output("pipe:", vsync=0, format="rawvideo", pix_fmt=pix_fmt)
     stream = stream.global_args("-loglevel", "panic", "-hide_banner", "-nostdin", "-nostats")
```

### Comparing `prpy-0.2.4/prpy/ffmpeg/utils.py` & `prpy-0.2.5/prpy/ffmpeg/utils.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/numpy/__init__.py` & `prpy-0.2.5/prpy/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/numpy/face.py` & `prpy-0.2.5/prpy/numpy/face.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/numpy/image.py` & `prpy-0.2.5/prpy/numpy/image.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,40 +15,43 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
+import logging
 from typing import Union
 
+from .image_ops import resample_bilinear_op, resample_box_op, reduce_roi_op
+
 def crop_slice_resize(
     inputs: np.ndarray,
     target_size: Union[int, tuple, list], 
     roi: Union[tuple, list, None] = None,
     target_idxs: Union[tuple, list, np.ndarray, None] = None,
     preserve_aspect_ratio: bool = False,
     keepdims: bool = True,
     library: str = 'PIL',
     scale_algorithm: str = 'bicubic'
   ) -> np.ndarray:
   """Crop, slice, and resize image(s) with all same settings.
 
   Args:
-    inputs: The inputs as uint8 shape (h, w, 3) or (n_frames, h, w, 3)
+    inputs: The inputs of shape (h, w, 3) or (n_frames, h, w, 3)
     target_size: The target size; scalar or (H, W) if preserve_aspect_ratio=False
     roi: The region of interest in format (x0, y0, x1, y1). Use None to keep all.
     target_idxs: The frame indices to be used. Use None to keep all.
     preserve_aspect_ratio: Preserve the aspect ratio?
     keepdims: If True, always keep n_frames dim. Otherwise, may drop n_frames dim.
     library: The library to use. `cv2` or `PIL` (return np ndarray), or `tf` (returns tf Tensor)
     scale_algorithm: The algorithm used for scaling.
       Supports: bicubic, bilinear, area (not for PIL!), lanczos. Default: bicubic
   Returns:
-    result: The processed frame(s) as float32 shape (h, w, 3) or (n_frames, h, w, 3)
+    result: The processed frame(s) of shape (h_new, w_new, 3) or (n_frames_new, h_new, w_new, 3)
   """
   assert isinstance(inputs, np.ndarray) and (len(inputs.shape) == 3 or len(inputs.shape) == 4)
   assert isinstance(target_size, int) or (isinstance(target_size, (tuple, list)) and len(target_size) == 2 and all(isinstance(i, int) for i in target_size))
   assert roi is None or (isinstance(roi, (tuple, list)) and len(roi) == 4 and all(isinstance(i, (int, np.int64)) for i in roi) and roi[2] > roi[0] and roi[3] > roi[1])
   assert target_idxs is None or isinstance(target_idxs, np.ndarray) or (isinstance(target_idxs, (tuple, list)) and all(isinstance(i, int) for i in target_idxs))
   assert isinstance(preserve_aspect_ratio, bool)
   assert isinstance(keepdims, bool)
@@ -82,17 +85,17 @@
     return out_size
   out_size = _out_size(in_shape, target_height, target_width, preserve_aspect_ratio)
   # Distinguish between different cases
   if out_size == (in_shape[1], in_shape[2]):
     # No resizing necessary
     if library == 'tf':
       import tensorflow as tf
-      out = tf.convert_to_tensor(inputs, dtype=tf.float32)
+      out = tf.convert_to_tensor(inputs)
     else:
-      out = inputs.astype(np.float32) 
+      out = inputs
   else:
     # Resize to out_size
     if library == 'tf':
       import tensorflow as tf
       # https://www.tensorflow.org/api_docs/python/tf/image/ResizeMethod
       mapping = {"bicubic": "bicubic", "bilinear": "bilinear", "lanczos": "lanczos3", "area": "area"}
       try:
@@ -102,15 +105,15 @@
       out = tf.image.resize(
         images=inputs, size=(target_height, target_width),
         preserve_aspect_ratio=preserve_aspect_ratio,
         method=library_algorithm, antialias=False)
     elif library == 'PIL':
       from PIL import Image
       # https://pillow.readthedocs.io/en/stable/releasenotes/2.7.0.html#image-resizing-filters
-      mapping = {"bicubic": Image.BICUBIC, "bilinear": Image.BILINEAR, "lanczos": Image.LANCZOS}
+      mapping = {"bicubic": Image.BICUBIC, "bilinear": Image.BILINEAR, "lanczos": Image.LANCZOS, "box": Image.BOX}
       try:
         library_algorithm = mapping[scale_algorithm]
       except KeyError:
         raise ValueError("Scaling algorithm {} is not supported by {}".format(scale_algorithm, library))
       # PIL requires (width, height)
       out_size = (out_size[1], out_size[0])
       out = np.asarray([
@@ -123,19 +126,74 @@
         library_algorithm = mapping[scale_algorithm]
       except KeyError:
         raise ValueError("Scaling algorithm {} is not supported by {}".format(scale_algorithm, library))
       # cv2 requires (width, height)
       out_size = (out_size[1], out_size[0])
       out = np.asarray([
         cv2.resize(src=f, dsize=out_size, interpolation=library_algorithm) for f in inputs])
+    elif library == 'prpy':
+      if scale_algorithm == 'bilinear':
+        if inputs.shape[1] / target_height > 2 and inputs.shape[2] / target_width > 2:
+          logging.debug("Switching from bilinear to box by default because we are downsampling significantly.")
+          out = resample_box(im=inputs, size=(target_height, target_width))
+        else:
+          out = resample_bilinear(im=inputs, size=(target_height, target_width))
+      elif scale_algorithm == 'box':
+        out = resample_box(im=inputs, size=(target_height, target_width))
+      else:
+        raise ValueError("Scaling algorithm {} is not supported by {}".format(scale_algorithm, library))
     else:
       raise ValueError("Library {} not supported".format(library))
   if keepdims and len(out.shape) == 3 and len(inputs_shape) == 4:
     # Add temporal dim back - might have been lost when slicing
     newaxis = tf.newaxis if library == 'tf' else np.newaxis
     out = out[newaxis,:,:,:]
   elif not keepdims and len(out.shape) == 4:
     # Remove temporal dim if necessary
     squeeze = tf.squeeze if library == 'tf' else np.squeeze
     if out.shape[0] == 1:
       out = squeeze(out, axis=0)
   return out
+
+def resample_bilinear(
+    im: np.ndarray,
+    size: Union[int, tuple]
+  ):
+  """Compute bilinear resampling with batch dimension
+  
+  Args:
+    im: The image(s) to be resized. Shape (n, h, w, c) or (h, w, c)
+    size: The new size either as scalar or (new_h, new_w)
+  Returns:
+    out: The resized image(s). Shape (n, new_h, new_w, c) or (new_h, new_w, c)
+  """
+  if isinstance(size, int): size = (size, size)
+  return resample_bilinear_op(im, size)
+
+def resample_box(
+    im: np.ndarray,
+    size: Union[int, tuple]
+  ):
+  """Compute box resampling with batch dimension
+  
+  Args:
+    im: The image(s) to be resized. Shape (n, h, w, c) or (h, w, c)
+    size: The new size either as scalar or (new_h, new_w)
+  Returns:
+    out: The resized image(s). Shape (n, new_h, new_w, c) or (new_h, new_w, c)
+  """
+  if isinstance(size, int): size = (size, size)
+  return resample_box_op(im, size)
+
+def reduce_roi(
+    video: np.ndarray,
+    roi: np.ndarray
+  ) -> np.ndarray:
+  """Reduce the spatial dimensions of a video by mean using ROI.
+
+  Args:
+    video: The video to be reduced. Shape (n, h, w, 3)
+    roi: The roi in form (x0, y0, x1, y1). Shape (n, 4) 
+  Returns:
+    out: The reduced vals. Shape (n, 3)
+  """
+  return reduce_roi_op(video, roi)
```

### Comparing `prpy-0.2.4/prpy/numpy/metric.py` & `prpy-0.2.5/prpy/numpy/metric.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/numpy/signal.py` & `prpy-0.2.5/prpy/numpy/signal.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/numpy/stride_tricks.py` & `prpy-0.2.5/prpy/numpy/stride_tricks.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/__init__.py` & `prpy-0.2.5/prpy/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/image.py` & `prpy-0.2.5/prpy/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/loss.py` & `prpy-0.2.5/prpy/tensorflow/loss.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/lr_schedule.py` & `prpy-0.2.5/prpy/tensorflow/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/model_saver.py` & `prpy-0.2.5/prpy/tensorflow/model_saver.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/nan.py` & `prpy-0.2.5/prpy/tensorflow/nan.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/optimizer.py` & `prpy-0.2.5/prpy/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/tensorflow/signal.py` & `prpy-0.2.5/prpy/tensorflow/signal.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/torch/__init__.py` & `prpy-0.2.5/prpy/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy/torch/model_saver.py` & `prpy-0.2.5/prpy/torch/model_saver.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/prpy.egg-info/PKG-INFO` & `prpy-0.2.5/prpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Collection of Python utils for signal, image, and video processing
 Author-email: Philipp Rouast <philipp@rouast.com>
 License: MIT License
 Project-URL: Repository, https://github.com/prouast/prpy.git
 Project-URL: Issues, https://github.com/prouast/prpy/issues
 Keywords: python,numpy,ffmpeg,tensorflow,torch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prpy-0.2.4/prpy.egg-info/SOURCES.txt` & `prpy-0.2.5/prpy.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -12,19 +12,23 @@
 prpy.egg-info/dependency_links.txt
 prpy.egg-info/requires.txt
 prpy.egg-info/top_level.txt
 prpy/ffmpeg/__init__.py
 prpy/ffmpeg/probe.py
 prpy/ffmpeg/readwrite.py
 prpy/ffmpeg/utils.py
+prpy/numpy/.DS_Store
 prpy/numpy/__init__.py
 prpy/numpy/face.py
 prpy/numpy/image.py
+prpy/numpy/image_ops.c
+prpy/numpy/image_ops.cpython-310-darwin.so
 prpy/numpy/metric.py
 prpy/numpy/signal.py
+prpy/numpy/spam.cpython-310-darwin.so
 prpy/numpy/stride_tricks.py
 prpy/tensorflow/__init__.py
 prpy/tensorflow/image.py
 prpy/tensorflow/loss.py
 prpy/tensorflow/lr_schedule.py
 prpy/tensorflow/model_saver.py
 prpy/tensorflow/nan.py
```

### Comparing `prpy-0.2.4/pyproject.toml` & `prpy-0.2.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61", "setuptools-scm"]
+requires = ["setuptools>=61", "setuptools-scm", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prpy"
 authors = [
     {name = "Philipp Rouast", email = "philipp@rouast.com"},
 ]
@@ -30,8 +30,11 @@
 torch = ["torch==2.1.0"]
 test = ["pytest", "flake8"]
 
 [project.urls]
 Repository = "https://github.com/prouast/prpy.git"
 Issues = "https://github.com/prouast/prpy/issues"
 
+[tools.setuptools]
+packages = ["prpy"]
+
 [tool.setuptools_scm]
```

### Comparing `prpy-0.2.4/tests/conftest.py` & `prpy-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_ffmpeg.py` & `prpy-0.2.5/tests/test_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_numpy_face.py` & `prpy-0.2.5/tests/test_numpy_face.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_numpy_image.py` & `prpy-0.2.5/tests/test_numpy_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 import tensorflow as tf
 
 @pytest.mark.parametrize("target_size", [6, 3, (6, 12)])
 @pytest.mark.parametrize("n_frames", [None, 3])
 @pytest.mark.parametrize("roi", [(2, 2, 7, 7), [2, 2, 7, 7], None])
 @pytest.mark.parametrize("target_idxs", [None, [0, 2], (0, 2), np.asarray([0, 2])])
 @pytest.mark.parametrize("preserve_aspect_ratio", [True, False])
-@pytest.mark.parametrize("library", ["cv2", "tf", "PIL"])
-@pytest.mark.parametrize("scale_algorithm", ["bicubic", "area", "lanczos", "bilinear"])
+@pytest.mark.parametrize("library", ["cv2", "tf", "PIL"]) # TODO: Test prpy
+@pytest.mark.parametrize("scale_algorithm", ["bicubic", "area", "lanczos", "bilinear"]) # TODO: Test box
 @pytest.mark.parametrize("keepdims", [True, False])
 def test_crop_slice_resize(target_size, n_frames, roi, target_idxs, preserve_aspect_ratio, library, scale_algorithm, keepdims):
   if (n_frames is None and target_idxs is not None) or \
      (library == "PIL" and scale_algorithm == "area"):
     pytest.skip("Skip because parameter combination does not work")
   if n_frames is None:
     images_in = np.random.uniform(size=(8, 12, 3), low=0, high=255)
```

### Comparing `prpy-0.2.4/tests/test_numpy_metric.py` & `prpy-0.2.5/tests/test_numpy_metric.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_numpy_signal.py` & `prpy-0.2.5/tests/test_numpy_signal.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_numpy_stride_tricks.py` & `prpy-0.2.5/tests/test_numpy_stride_tricks.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_tensorflow.py` & `prpy-0.2.5/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `prpy-0.2.4/tests/test_torch.py` & `prpy-0.2.5/tests/test_torch.py`

 * *Files identical despite different names*

