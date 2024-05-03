# Comparing `tmp/matsubplots-1.1.0.tar.gz` & `tmp/matsubplots-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matsubplots-1.1.0.tar", last modified: Mon Apr 15 16:10:12 2024, max compression
+gzip compressed data, was "matsubplots-1.1.1.tar", last modified: Fri May  3 21:14:24 2024, max compression
```

## Comparing `matsubplots-1.1.0.tar` & `matsubplots-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 16:10:12.519089 matsubplots-1.1.0/
--rw-rw-rw-   0        0        0     1089 2024-04-15 16:09:00.000000 matsubplots-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     1274 2024-04-15 16:10:12.518092 matsubplots-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-04-15 16:09:00.000000 matsubplots-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 16:10:12.475412 matsubplots-1.1.0/matsubplots/
--rw-rw-rw-   0        0        0      168 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/__init__.py
--rw-rw-rw-   0        0        0     5268 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/matsubplots.py
--rw-rw-rw-   0        0        0     7514 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/orthoview.py
--rw-rw-rw-   0        0        0       23 2024-04-15 16:09:00.000000 matsubplots-1.1.0/matsubplots/version.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:10:12.515350 matsubplots-1.1.0/matsubplots.egg-info/
--rw-rw-rw-   0        0        0     1274 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 16:10:12.000000 matsubplots-1.1.0/matsubplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      312 2024-04-15 16:10:12.522087 matsubplots-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-04-15 16:09:00.000000 matsubplots-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:14:24.155451 matsubplots-1.1.1/
+-rw-rw-rw-   0        0        0     1089 2024-05-03 21:13:27.000000 matsubplots-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     1274 2024-05-03 21:14:24.154410 matsubplots-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-03 21:13:27.000000 matsubplots-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:14:24.111680 matsubplots-1.1.1/matsubplots/
+-rw-rw-rw-   0        0        0      166 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/matsubplots.py
+-rw-rw-rw-   0        0        0       23 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/version.py
+-rw-rw-rw-   0        0        0     8575 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/viewers.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:14:24.151433 matsubplots-1.1.1/matsubplots.egg-info/
+-rw-rw-rw-   0        0        0     1274 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-03 21:14:24.000000 matsubplots-1.1.1/matsubplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      312 2024-05-03 21:14:24.158450 matsubplots-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-03 21:13:27.000000 matsubplots-1.1.1/setup.py
```

### Comparing `matsubplots-1.1.0/LICENSE.md` & `matsubplots-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.1.0/PKG-INFO` & `matsubplots-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.1.0
+Version: 1.1.1
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matsubplots-1.1.0/README.md` & `matsubplots-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.1.0/matsubplots/matsubplots.py` & `matsubplots-1.1.1/matsubplots/matsubplots.py`

 * *Files identical despite different names*

### Comparing `matsubplots-1.1.0/matsubplots/orthoview.py` & `matsubplots-1.1.1/matsubplots/viewers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,86 @@
 import numpy as np
 from matplotlib.backend_bases import MouseButton
 
 
-def orthoview(axs, image, *args, backend=None, **kwargs):
-    orthoview_base(axs, image, *args, **kwargs)
-    if backend is None:
-        pass
-    elif backend.lower() == 'interactive':
-        return OrthoViewInteractive(axs, image)
-    elif backend.lower() == 'static':
-        return OrthoViewStatic(axs, image)
-    else:
-        raise NotImplementedError(backend)
-
-
-def orthoview_base(axs, image, spacing=(1,1,1), xyz=None, ijk=None, slab_thickness=None, slab_func=np.mean, **kwargs):
+def orthoview(axs, image, spacing=(1,1,1), xyz=None, ijk=None, slab_thickness=None, slab_func=np.mean, reposition=True, backend=None, **kwargs):
     axs = np.asarray(axs)
     image = np.asarray(image)
     spacing = np.asarray(spacing)
     if not (axs.size == image.ndim == spacing.size == 3):
         raise ValueError('Expected a 3D image, 3 axes, and 3 values for spacing')
     if ijk is not None and xyz is not None:
         raise ValueError('Cannot specify ijk and xyz at the same time')
-    left = 0
+    bounds = []
+    cbounds = []
     for i, ax in enumerate(axs.ravel()):
         if xyz is not None:
             j = round(xyz[::-1][i] / spacing[::-1][i] + (image.shape[i] - 1) / 2)
         elif ijk is not None:
             j = ijk[i]
         else:
             j = image.shape[i] // 2
         thickness = 1 if slab_thickness is None else round(slab_thickness / spacing[i])
         j0 = np.maximum(j - thickness // 2, 0)
         j1 = j - (-thickness // 2)
         slice_ = slab_func(np.rollaxis(image, i)[j0:j1], axis=0)
         aspect = np.divide(*spacing[::-1][np.arange(spacing.size) != i])
-        bounds = ax.get_position().bounds
-        width = bounds[2] * (slice_.shape[1] / slice_.shape[0]) / aspect
-        ax.set_position((bounds[0] - left, bounds[1], width, bounds[3]))
+        bounds.append([])
+        bounds[-1].append(ax.get_position().bounds)
         im = ax.imshow(slice_, aspect=aspect, **kwargs)
-        left += bounds[2] - width
+        bounds[-1].append(ax.get_position().bounds)
         if hasattr(ax, 'cax'):
-            if ax is axs.ravel()[-1]:
-                bounds = ax.cax.get_position().bounds
-                ax.cax.set_position((bounds[0] - left, bounds[1], bounds[2], bounds[3]))
             ax.get_figure().colorbar(im, cax=ax.cax)
+            cbounds.append(ax.cax.get_position().bounds)
+    if reposition:
+        _, _, w00, _ = bounds[0][0]
+        l01, b01, w01, h01 = bounds[0][1]
+        l0, b0, w0, h0 = l01, b01, w01, h01
+        _, _, w10, _ = bounds[1][0]
+        l11, b11, w11, h11 = bounds[1][1]
+        l1, b1, w1, h1 = l11, b11, w11, h11
+        _, _, w20, _ = bounds[2][0]
+        l21, b21, w21, h21 = bounds[2][1]
+        l2, b2, w2, h2 = l21, b21, w21, h21
+        lshift = (w00 - w01) / 2
+        lshift += (w10 - w11) / 2
+        if w1 < w0:
+            w0 = w1
+            h0 *= w0 / w01
+            b0 += (h01 - h0) / 2
+            lshift += w01 - w0
+            axs[0].set_position((l0, b0, w0, h0))
+            axs[1].set_position((l1 - lshift, b1, w1, h1))
+        else:
+            w1 = w0
+            h1 *= w1 / w11
+            b1 += (h11 - h1) / 2
+            axs[1].set_position((l1 - lshift, b1, w1, h1))
+            lshift += w11 - w1
+        lshift += (w10 - w11) / 2
+        w2 *= h1 / h2
+        h2 = h1
+        b2 = b1
+        lshift += (w20 - w21) / 2
+        axs[2].set_position((l2 - lshift, b2, w2, h2))
+        lshift += (w20 - w21) / 2
+        lshift += w21 - w2
+        if cbounds:
+            cl, cb, cw, ch = cbounds[2]
+            ch2 = max(h0, h1, h2)
+            cb2 = cb + (ch - ch2) / 2
+            ax.cax.set_position((cl - lshift, cb2, cw, ch2))
+    if backend is None:
+        pass
+    elif backend.lower() == 'interactive':
+        return OrthoViewInteractive(axs, image)
+    elif backend.lower() == 'static':
+        return OrthoViewStatic(axs, image)
+    else:
+        raise NotImplementedError(backend)
 
 
 class OrthoView:
 
     alignments = (0, 0), (0, 1), (1, 1)
     colors = '#ff0000', '#00ff00', '#ffff00'
     indices = (1, 2), (0, 2), (0, 1)
```

### Comparing `matsubplots-1.1.0/matsubplots.egg-info/PKG-INFO` & `matsubplots-1.1.1/matsubplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.1.0
+Version: 1.1.1
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matsubplots-1.1.0/setup.py` & `matsubplots-1.1.1/setup.py`

 * *Files identical despite different names*

