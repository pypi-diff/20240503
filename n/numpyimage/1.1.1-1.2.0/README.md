# Comparing `tmp/numpyimage-1.1.1.tar.gz` & `tmp/numpyimage-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyimage-1.1.1.tar", last modified: Mon Jan  9 16:52:23 2023, max compression
+gzip compressed data, was "dist/numpyimage-1.2.0.tar", last modified: Fri May  3 13:30:08 2024, max compression
```

## Comparing `numpyimage-1.1.1.tar` & `numpyimage-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-01-09 16:52:23.981810 numpyimage-1.1.1/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)    35149 2022-11-15 13:12:49.000000 numpyimage-1.1.1/LICENSE
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       25 2022-11-15 13:12:49.000000 numpyimage-1.1.1/MANIFEST.in
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     2938 2023-01-09 16:52:23.981810 numpyimage-1.1.1/PKG-INFO
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     2421 2023-01-09 14:51:41.000000 numpyimage-1.1.1/README.md
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-01-09 16:52:23.981810 numpyimage-1.1.1/npimage/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       20 2022-11-15 13:12:49.000000 numpyimage-1.1.1/npimage/__init__.py
--rwxrwxr-x   0 phelps   (253699) upramdya (11350)     8963 2023-01-09 16:45:33.000000 numpyimage-1.1.1/npimage/core.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-01-09 16:52:23.981810 numpyimage-1.1.1/npimage/filetypes/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       18 2022-11-15 13:12:49.000000 numpyimage-1.1.1/npimage/filetypes/__init__.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     2181 2022-11-15 13:12:49.000000 numpyimage-1.1.1/npimage/filetypes/pbm.py
--rwxrwxr-x   0 phelps   (253699) upramdya (11350)    30596 2022-12-13 14:06:40.000000 numpyimage-1.1.1/npimage/graphics.py
--rwxrwxr-x   0 phelps   (253699) upramdya (11350)     2444 2022-11-15 13:12:49.000000 numpyimage-1.1.1/npimage/nrrd_utils.py
--rwxrwxr-x   0 phelps   (253699) upramdya (11350)     8204 2022-12-13 14:06:40.000000 numpyimage-1.1.1/npimage/operations.py
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     1305 2022-11-15 13:12:49.000000 numpyimage-1.1.1/npimage/utils.py
-drwxrwxr-x   0 phelps   (253699) upramdya (11350)        0 2023-01-09 16:52:23.981810 numpyimage-1.1.1/numpyimage.egg-info/
--rw-rw-r--   0 phelps   (253699) upramdya (11350)     2938 2023-01-09 16:52:23.000000 numpyimage-1.1.1/numpyimage.egg-info/PKG-INFO
--rw-rw-r--   0 phelps   (253699) upramdya (11350)      396 2023-01-09 16:52:23.000000 numpyimage-1.1.1/numpyimage.egg-info/SOURCES.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)        1 2023-01-09 16:52:23.000000 numpyimage-1.1.1/numpyimage.egg-info/dependency_links.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       40 2023-01-09 16:52:23.000000 numpyimage-1.1.1/numpyimage.egg-info/requires.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)        8 2023-01-09 16:52:23.000000 numpyimage-1.1.1/numpyimage.egg-info/top_level.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       40 2022-11-15 13:12:49.000000 numpyimage-1.1.1/requirements.txt
--rw-rw-r--   0 phelps   (253699) upramdya (11350)       38 2023-01-09 16:52:23.981810 numpyimage-1.1.1/setup.cfg
--rw-rw-r--   0 phelps   (253699) upramdya (11350)      979 2023-01-09 16:50:56.000000 numpyimage-1.1.1/setup.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-05-03 13:30:08.000000 numpyimage-1.2.0/
+-rw-rw-r--   0 jasper     (501) staff       (20)    35149 2021-03-01 14:48:24.000000 numpyimage-1.2.0/LICENSE
+-rw-rw-r--   0 jasper     (501) staff       (20)       25 2022-09-19 09:39:09.000000 numpyimage-1.2.0/MANIFEST.in
+-rw-rw-r--   0 jasper     (501) staff       (20)     3243 2024-05-03 13:30:08.000000 numpyimage-1.2.0/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)     2421 2022-12-23 11:39:55.000000 numpyimage-1.2.0/README.md
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-05-03 13:30:08.000000 numpyimage-1.2.0/npimage/
+-rw-rw-r--   0 jasper     (501) staff       (20)       20 2021-03-01 14:48:24.000000 numpyimage-1.2.0/npimage/__init__.py
+-rwxrwxr-x   0 jasper     (501) staff       (20)    10664 2024-04-07 19:35:02.000000 numpyimage-1.2.0/npimage/core.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-05-03 13:30:08.000000 numpyimage-1.2.0/npimage/filetypes/
+-rw-rw-r--   0 jasper     (501) staff       (20)       18 2022-01-30 00:55:14.000000 numpyimage-1.2.0/npimage/filetypes/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     2181 2022-01-30 00:53:35.000000 numpyimage-1.2.0/npimage/filetypes/pbm.py
+-rwxrwxr-x   0 jasper     (501) staff       (20)    30596 2022-12-11 22:23:50.000000 numpyimage-1.2.0/npimage/graphics.py
+-rwxrwxr-x   0 jasper     (501) staff       (20)     2581 2024-02-27 12:41:08.000000 numpyimage-1.2.0/npimage/nrrd_utils.py
+-rwxrwxr-x   0 jasper     (501) staff       (20)    19793 2024-02-27 12:41:11.000000 numpyimage-1.2.0/npimage/operations.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     1386 2023-10-17 22:31:31.000000 numpyimage-1.2.0/npimage/utils.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2024-05-03 13:30:08.000000 numpyimage-1.2.0/numpyimage.egg-info/
+-rw-r--r--   0 jasper     (501) staff       (20)     3243 2024-05-03 13:30:08.000000 numpyimage-1.2.0/numpyimage.egg-info/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)      396 2024-05-03 13:30:08.000000 numpyimage-1.2.0/numpyimage.egg-info/SOURCES.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        1 2024-05-03 13:30:08.000000 numpyimage-1.2.0/numpyimage.egg-info/dependency_links.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)       54 2024-05-03 13:30:08.000000 numpyimage-1.2.0/numpyimage.egg-info/requires.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        8 2024-05-03 13:30:08.000000 numpyimage-1.2.0/numpyimage.egg-info/top_level.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)       54 2024-02-27 12:41:11.000000 numpyimage-1.2.0/requirements.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)       38 2024-05-03 13:30:08.000000 numpyimage-1.2.0/setup.cfg
+-rw-rw-r--   0 jasper     (501) staff       (20)      926 2024-05-03 13:29:42.000000 numpyimage-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `numpyimage-1.1.1/LICENSE` & `numpyimage-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numpyimage-1.1.1/PKG-INFO` & `numpyimage-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: numpyimage
-Version: 1.1.1
+Version: 1.2.0
 Summary: Load, save, and manipulate image files as numpy arrays
 Home-page: https://github.com/jasper-tms/npimage
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: GNU GPL v3
+Description: # npimage
+        Need to load pixel values from image files as numpy arrays, and hate having to remember whether you should use PIL, tifffile, matplotlib, or something else? Hate having to deal with the fact that those libraries all use different function names and syntaxes? Wish you could just provide a filename and get back a numpy array? This library's `core.py` does that, with `array = load(filename)`, `save(array, filename)`, and `show(array)` functions that let you easily handle a number of common image file formats without having to remember library-specific syntax. (Another choice of library to consider for accomplishing similar goals is [imageio](https://pypi.org/project/imageio/), which also supports loading videos through the FFmpeg wrapper library [pyav](https://pypi.org/project/av/).)
+        
+        Want to draw simple shapes like lines, triangles, and circles into 3D numpy arrays? Frustrated that the python libraries you can find online like `opencv` and `skimage.draw` work on 2D arrays but not 3D? I wrote some functions in `graphics.py` that do the trick in 3D. (If you know of another library that can do this, please let me know!)
+        
+        
+        ### Documentation
+        - `core.py`: load, save, or show images.
+        - `graphics.py`: draw points, lines, triangles, circles, or spheres into 2D or 3D numpy arrays representing image volumes.
+        - `nrrd_utils.py`: compress or read metadata from `.nrrd` files.
+        - `operations.py`: perform operations on images.
+        
+        For now, check each function's docstring for more. A jupyter notebook demonstrating this package's functions will come later.
+        
+        
+        ### Installation
+        
+        As is always the case in python, consider making a virtual environment (using your preference of conda, virtualenv, or virtualenvwrapper) before installing.
+        
+        **Option 1:** `pip install` from PyPI:
+        
+            pip install numpyimage
+        
+        (Unfortunately the name `npimage` was already taken on PyPI, so `pip install npimage` will get you a different package.)
+        
+        **Option 2:** `pip install` directly from GitHub:
+            
+            pip install git+https://github.com/jasper-tms/npimage.git
+        
+        **Option 3:** First `git clone` this repo and then `pip install` it from your clone:
+        
+            cd ~/repos  # Or wherever on your computer you want to download this code to
+            git clone https://github.com/jasper-tms/npimage.git
+            cd npimage
+            pip install .
+        
+        **After installing,** you can import this package in python using `import npimage` (not `import numpyimage`!)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# npimage
-Need to load pixel values from image files as numpy arrays, and hate having to remember whether you should use PIL, tifffile, matplotlib, or something else? Hate having to deal with the fact that those libraries all use different function names and syntaxes? Wish you could just provide a filename and get back a numpy array? This library's `core.py` does that, with `array = load(filename)`, `save(array, filename)`, and `show(array)` functions that let you easily handle a number of common image file formats without having to remember library-specific syntax. (Another choice of library to consider for accomplishing similar goals is [imageio](https://pypi.org/project/imageio/), which also supports loading videos through the FFmpeg wrapper library [pyav](https://pypi.org/project/av/).)
-
-Want to draw simple shapes like lines, triangles, and circles into 3D numpy arrays? Frustrated that the python libraries you can find online like `opencv` and `skimage.draw` work on 2D arrays but not 3D? I wrote some functions in `graphics.py` that do the trick in 3D. (If you know of another library that can do this, please let me know!)
-
-
-### Documentation
-- `core.py`: load, save, or show images.
-- `graphics.py`: draw points, lines, triangles, circles, or spheres into 2D or 3D numpy arrays representing image volumes.
-- `nrrd_utils.py`: compress or read metadata from `.nrrd` files.
-- `operations.py`: perform operations on images.
-
-For now, check each function's docstring for more. A jupyter notebook demonstrating this package's functions will come later.
-
-
-### Installation
-
-As is always the case in python, consider making a virtual environment (using your preference of conda, virtualenv, or virtualenvwrapper) before installing.
-
-**Option 1:** `pip install` from PyPI:
-
-    pip install numpyimage
-
-(Unfortunately the name `npimage` was already taken on PyPI, so `pip install npimage` will get you a different package.)
-
-**Option 2:** `pip install` directly from GitHub:
-    
-    pip install git+https://github.com/jasper-tms/npimage.git
-
-**Option 3:** First `git clone` this repo and then `pip install` it from your clone:
-
-    cd ~/repos  # Or wherever on your computer you want to download this code to
-    git clone https://github.com/jasper-tms/npimage.git
-    cd npimage
-    pip install .
-
-**After installing,** you can import this package in python using `import npimage` (not `import numpyimage`!)
```

### Comparing `numpyimage-1.1.1/README.md` & `numpyimage-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `numpyimage-1.1.1/npimage/core.py` & `numpyimage-1.2.0/npimage/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -106,30 +106,32 @@
         return data
 
 open = load  # Function name alias
 read = load  # Function name alias
 imread = load  # Function name alias
 
 
-def save(data, filename, dim_order='zyx', metadata=None, compress=False):
+def save(data, filename, overwrite=False, dim_order='zyx', metadata=None, compress=False):
     """
     Save a numpy array to file with a file type specified by the
     filename extension.
 
     As is typical for Python, the input array is assumed to have
      dimensions ordered as zyx for 3D images, yx for 1-channel 2D
      images, or yxc for multi-channel 2D images.
     Set dim_order='xy' if your array is a 3D image in in xyz order,
      a 1-channel 2D image in xy order, or a multi-channel 2D image
      in xyc order.
 
     `compress` only matters when saving in `.nrrd` format
     """
-    while filename.endswith('/'):
-        filename = filename[:-1]
+    filename = filename.rstrip('/')
+    if os.path.exists(filename) and not overwrite:
+        raise Exception(f'File {filename} already exists. '
+                        'Set overwrite=True to overwrite.')
     extension = filename.split('.')[-1]
     assert extension in supported_extensions, f'Filetype {extension} not supported'
 
     if compress and extension != 'nrrd':
         print('WARNING: compress argument is ignored because not saving as '
               '.nrrd. Whether or not compression occurs now will depend on '
               'the format you are saving to.')
@@ -172,18 +174,61 @@
 
     if extension in ['raw', 'vol']:
         raise NotImplementedError
 
     if extension == 'zarr':
         raise NotImplementedError
 
+
 write = save  # Function name alias
 to_file = save  # Function name alias
 
 
+def save_video(data, filename, overwrite=False, dim_order='yx', time_axis=0,
+               framerate=30, crf=23, compression_speed='medium'):
+    """
+    Save a 3D numpy array as a video, with a specified axis as the time axis.
+
+    Follows the PyAV cookbook section on generating video from numpy arrays:
+    https://pyav.basswood-io.com/docs/develop/cookbook/numpy.html#generating-video
+    """
+    if not data.ndim == 3:
+        raise ValueError('Input data must be a 3D numpy array.')
+    try:
+        import av
+    except ImportError:
+        raise ImportError('To save videos, you must have PyAV installed. '
+                          'You can install it with "pip install av".')
+    data = np.moveaxis(data, time_axis, 0)
+    if 'xy' in dim_order:
+        data = data.swapaxes(1, 2)
+    n_frames = data.shape[0]
+
+    if os.path.exists(filename) and not overwrite:
+        raise Exception(f'File {filename} already exists. '
+                        'Set overwrite=True to overwrite.')
+    container = av.open(filename, mode='w')
+
+    stream = container.add_stream('libx264', rate=framerate)
+    stream.pix_fmt = 'yuv420p'
+    stream.options = {'crf': str(crf), 'preset': compression_speed}
+    stream.height = data.shape[1]
+    stream.width = data.shape[2]
+
+    for frame_i in range(n_frames):
+        frame = av.VideoFrame.from_ndarray(data[frame_i], format='gray')
+        for packet in stream.encode(frame):
+            container.mux(packet)
+
+    for packet in stream.encode():
+        container.mux(packet)
+
+    container.close()
+
+
 def show(data, dim_order='yx', mode='PIL', **kwargs):
     """
     Display a numpy array of pixel values as an image. Supported types:
       1-channel (grayscale) : data.shape must be (y, x)
       3-channel (RGB)       : data.shape must be (y, x, 3)
       4-channel (RGBA)  : data.shape must be (y, x, 4)
```

### Comparing `numpyimage-1.1.1/npimage/filetypes/pbm.py` & `numpyimage-1.2.0/npimage/filetypes/pbm.py`

 * *Files identical despite different names*

### Comparing `numpyimage-1.1.1/npimage/graphics.py` & `numpyimage-1.2.0/npimage/graphics.py`

 * *Files identical despite different names*

### Comparing `numpyimage-1.1.1/npimage/nrrd_utils.py` & `numpyimage-1.2.0/npimage/nrrd_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,22 +34,27 @@
                 os.rename(fn, fn_moved)
             else:
                 print(f'Overwriting {fn} with a compressed version of itself.')
 
             nrrd.write(fn, data, header=header)
 
 
-def read_headers(*fn_patterns):
+def read_headers(*fn_patterns, verbose=True):
+    headers = dict()
     if len(fn_patterns) == 0:
         fn_patterns = ['*.nrrd']
-        print('Reading headers of all nrrd files in this directory.\n')
+        if verbose:
+            print('Reading headers of all nrrd files in this directory.')
     for fn_pattern in fn_patterns:
-        for fn in glob.glob(fn_pattern):
-            print(fn)
-            print(nrrd.read_header(fn), '\n')
+        for fn in sorted(glob.glob(fn_pattern)):
+            if verbose:
+                print(f'Reading header of {fn}')
+            headers[fn] = nrrd.read_header(fn)
+
+    return headers
 
 
 if __name__ == '__main__':
     l = locals()
     public_functions = [f for f in l if callable(l[f]) and f[0] != '_']
     if len(sys.argv) <= 1 or not sys.argv[1] in public_functions:
         from inspect import signature
```

### Comparing `numpyimage-1.1.1/npimage/utils.py` & `numpyimage-1.2.0/npimage/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
 
-def iround(n):
+def iround(n, output_dtype=int):
     # This rounds to the nearest integer, rounding values ending in .5 up
     # (toward positive infinity)
-    return np.floor(n + 0.5).astype(int)
+    return np.floor(n + 0.5).astype(output_dtype)
 
     # "For values exactly halfway between rounded decimal values, NumPy.round
     # rounds to the nearest even value. Thus 1.5 and 2.5 round to 2.0, -0.5 and
     # 0.5 round to 0.0, etc."
     # I think this convention is potentially problematic for graphics
     # applications, that is, it could break watertightness of shapes that are
     # supposed to be watertight, so I'm not using it here.
     #return np.round(n).astype(int)
 
 
-def ifloor(n):
-    return np.floor(n).astype(int)
+def ifloor(n, output_dtype=int):
+    return np.floor(n).astype(output_dtype)
 
 
-def iceil(n):
-    return np.ceil(n).astype(int)
+def iceil(n, output_dtype=int):
+    return np.ceil(n).astype(output_dtype)
 
 
 def eq(a, b, tolerance=1e-8):
     """
     Test if two objects have an absolute difference less than a small value.
     Useful for testing for "equivalence" of floats which are not be stored to
     infinite precision.
```

### Comparing `numpyimage-1.1.1/numpyimage.egg-info/PKG-INFO` & `numpyimage-1.2.0/numpyimage.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: numpyimage
-Version: 1.1.1
+Version: 1.2.0
 Summary: Load, save, and manipulate image files as numpy arrays
 Home-page: https://github.com/jasper-tms/npimage
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: GNU GPL v3
+Description: # npimage
+        Need to load pixel values from image files as numpy arrays, and hate having to remember whether you should use PIL, tifffile, matplotlib, or something else? Hate having to deal with the fact that those libraries all use different function names and syntaxes? Wish you could just provide a filename and get back a numpy array? This library's `core.py` does that, with `array = load(filename)`, `save(array, filename)`, and `show(array)` functions that let you easily handle a number of common image file formats without having to remember library-specific syntax. (Another choice of library to consider for accomplishing similar goals is [imageio](https://pypi.org/project/imageio/), which also supports loading videos through the FFmpeg wrapper library [pyav](https://pypi.org/project/av/).)
+        
+        Want to draw simple shapes like lines, triangles, and circles into 3D numpy arrays? Frustrated that the python libraries you can find online like `opencv` and `skimage.draw` work on 2D arrays but not 3D? I wrote some functions in `graphics.py` that do the trick in 3D. (If you know of another library that can do this, please let me know!)
+        
+        
+        ### Documentation
+        - `core.py`: load, save, or show images.
+        - `graphics.py`: draw points, lines, triangles, circles, or spheres into 2D or 3D numpy arrays representing image volumes.
+        - `nrrd_utils.py`: compress or read metadata from `.nrrd` files.
+        - `operations.py`: perform operations on images.
+        
+        For now, check each function's docstring for more. A jupyter notebook demonstrating this package's functions will come later.
+        
+        
+        ### Installation
+        
+        As is always the case in python, consider making a virtual environment (using your preference of conda, virtualenv, or virtualenvwrapper) before installing.
+        
+        **Option 1:** `pip install` from PyPI:
+        
+            pip install numpyimage
+        
+        (Unfortunately the name `npimage` was already taken on PyPI, so `pip install npimage` will get you a different package.)
+        
+        **Option 2:** `pip install` directly from GitHub:
+            
+            pip install git+https://github.com/jasper-tms/npimage.git
+        
+        **Option 3:** First `git clone` this repo and then `pip install` it from your clone:
+        
+            cd ~/repos  # Or wherever on your computer you want to download this code to
+            git clone https://github.com/jasper-tms/npimage.git
+            cd npimage
+            pip install .
+        
+        **After installing,** you can import this package in python using `import npimage` (not `import numpyimage`!)
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# npimage
-Need to load pixel values from image files as numpy arrays, and hate having to remember whether you should use PIL, tifffile, matplotlib, or something else? Hate having to deal with the fact that those libraries all use different function names and syntaxes? Wish you could just provide a filename and get back a numpy array? This library's `core.py` does that, with `array = load(filename)`, `save(array, filename)`, and `show(array)` functions that let you easily handle a number of common image file formats without having to remember library-specific syntax. (Another choice of library to consider for accomplishing similar goals is [imageio](https://pypi.org/project/imageio/), which also supports loading videos through the FFmpeg wrapper library [pyav](https://pypi.org/project/av/).)
-
-Want to draw simple shapes like lines, triangles, and circles into 3D numpy arrays? Frustrated that the python libraries you can find online like `opencv` and `skimage.draw` work on 2D arrays but not 3D? I wrote some functions in `graphics.py` that do the trick in 3D. (If you know of another library that can do this, please let me know!)
-
-
-### Documentation
-- `core.py`: load, save, or show images.
-- `graphics.py`: draw points, lines, triangles, circles, or spheres into 2D or 3D numpy arrays representing image volumes.
-- `nrrd_utils.py`: compress or read metadata from `.nrrd` files.
-- `operations.py`: perform operations on images.
-
-For now, check each function's docstring for more. A jupyter notebook demonstrating this package's functions will come later.
-
-
-### Installation
-
-As is always the case in python, consider making a virtual environment (using your preference of conda, virtualenv, or virtualenvwrapper) before installing.
-
-**Option 1:** `pip install` from PyPI:
-
-    pip install numpyimage
-
-(Unfortunately the name `npimage` was already taken on PyPI, so `pip install npimage` will get you a different package.)
-
-**Option 2:** `pip install` directly from GitHub:
-    
-    pip install git+https://github.com/jasper-tms/npimage.git
-
-**Option 3:** First `git clone` this repo and then `pip install` it from your clone:
-
-    cd ~/repos  # Or wherever on your computer you want to download this code to
-    git clone https://github.com/jasper-tms/npimage.git
-    cd npimage
-    pip install .
-
-**After installing,** you can import this package in python using `import npimage` (not `import numpyimage`!)
```

### Comparing `numpyimage-1.1.1/setup.py` & `numpyimage-1.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
     requirements = [l for l in requirements if not l.startswith('#')]
 
 setuptools.setup(
     name="numpyimage",
-    version="1.1.1",
+    version="1.2.0",
     author="Jasper Phelps",
     author_email="jasper.s.phelps@gmail.com",
     description="Load, save, and manipulate image files as numpy arrays",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasper-tms/npimage",
     license='GNU GPL v3',
     packages=setuptools.find_packages(),
-    #package_data={'npimage': ['requirements.txt']},
     classifiers=[
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=requirements
```

