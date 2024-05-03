# Comparing `tmp/pytom3d-0.0.0rc1.tar.gz` & `tmp/pytom3d-0.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytom3d-0.0.0rc1.tar", last modified: Thu May  2 08:19:28 2024, max compression
+gzip compressed data, was "pytom3d-0.0.0rc2.tar", last modified: Thu May  2 15:43:51 2024, max compression
```

## Comparing `pytom3d-0.0.0rc1.tar` & `pytom3d-0.0.0rc2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.320021 pytom3d-0.0.0rc1/
--rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/LICENSE
--rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-02 08:19:28.320021 pytom3d-0.0.0rc1/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-02 08:15:05.000000 pytom3d-0.0.0rc1/README.md
--rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/pyproject.toml
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-02 08:19:28.320021 pytom3d-0.0.0rc1/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-02 08:19:09.000000 pytom3d-0.0.0rc1/setup.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.316021 pytom3d-0.0.0rc1/src/
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.316021 pytom3d-0.0.0rc1/src/pytom3d/
--rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/__init__.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    17041 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/core.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2688 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/scan.py
--rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/stats.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    14028 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/util.py
--rw-rw-r--   0 ale       (1000) ale       (1000)    17747 2024-05-02 08:13:47.000000 pytom3d-0.0.0rc1/src/pytom3d/viewer.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 08:19:28.316021 pytom3d-0.0.0rc1/src/pytom3d.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/requires.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-02 08:19:28.000000 pytom3d-0.0.0rc1/src/pytom3d.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 15:43:51.159714 pytom3d-0.0.0rc2/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    32473 2024-05-02 15:24:15.000000 pytom3d-0.0.0rc2/LICENSE
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-02 15:43:51.159714 pytom3d-0.0.0rc2/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      613 2024-05-02 15:24:15.000000 pytom3d-0.0.0rc2/README.md
+-rw-rw-r--   0 ale       (1000) ale       (1000)       86 2024-05-02 15:24:15.000000 pytom3d-0.0.0rc2/pyproject.toml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-02 15:43:51.159714 pytom3d-0.0.0rc2/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1123 2024-05-02 15:41:45.000000 pytom3d-0.0.0rc2/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 15:43:51.159714 pytom3d-0.0.0rc2/src/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 15:43:51.159714 pytom3d-0.0.0rc2/src/pytom3d/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2024-05-02 15:24:15.000000 pytom3d-0.0.0rc2/src/pytom3d/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    18326 2024-05-02 15:39:51.000000 pytom3d-0.0.0rc2/src/pytom3d/core.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2567 2024-05-02 15:30:31.000000 pytom3d-0.0.0rc2/src/pytom3d/scan.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2214 2024-05-02 15:24:15.000000 pytom3d-0.0.0rc2/src/pytom3d/stats.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    14028 2024-05-02 15:24:15.000000 pytom3d-0.0.0rc2/src/pytom3d/util.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    19426 2024-05-02 15:42:51.000000 pytom3d-0.0.0rc2/src/pytom3d/viewer.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-02 15:43:51.159714 pytom3d-0.0.0rc2/src/pytom3d.egg-info/
+-rw-r--r--   0 ale       (1000) ale       (1000)     1566 2024-05-02 15:43:51.000000 pytom3d-0.0.0rc2/src/pytom3d.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)      342 2024-05-02 15:43:51.000000 pytom3d-0.0.0rc2/src/pytom3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-02 15:43:51.000000 pytom3d-0.0.0rc2/src/pytom3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      112 2024-05-02 15:43:51.000000 pytom3d-0.0.0rc2/src/pytom3d.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        8 2024-05-02 15:43:51.000000 pytom3d-0.0.0rc2/src/pytom3d.egg-info/top_level.txt
```

### Comparing `pytom3d-0.0.0rc1/LICENSE` & `pytom3d-0.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc1/PKG-INFO` & `pytom3d-0.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytom3d
-Version: 0.0.0rc1
+Version: 0.0.0rc2
 Summary: PyToM-3D: Python Topography Manipulator in 3D
 Home-page: https://github.com/aletgn/pytom-3d.git
 Author: Alessandro Tognan
 Author-email: alessandro.tognan@gmail.com
 Project-URL: Bug Tracker, https://github.com/aletgn/pytom-3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pytom3d-0.0.0rc1/README.md` & `pytom3d-0.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc1/setup.py` & `pytom3d-0.0.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pytom3d",
-    version="0.0.0rc1",
+    version="0.0.0rc2",
     description="PyToM-3D: Python Topography Manipulator in 3D",
     long_description=long_description,
     long_description_content_type="text/markdown",
         
     author="Alessandro Tognan",
     author_email="alessandro.tognan@gmail.com",
     url="https://github.com/aletgn/pytom-3d.git",
```

### Comparing `pytom3d-0.0.0rc1/src/pytom3d/core.py` & `pytom3d-0.0.0rc2/src/pytom3d/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,49 @@
         List[Tuple]
             A list containing information about the filtering event.
 
         """
         self.P = self.P[indices, :]
         return [(len(self.history_), self.filter_points.__name__), ("indices", indices)]
 
+    def pick_points(self, axis: int, loc: float, tol: float = 1e-3) -> Tuple[np.ndarray]:
+        """
+        Pick points based on proximity to a specified location along a given axis.
+
+        Parameters
+        ----------
+        axis : int
+            The axis along which to pick points. 0 for x-axis, 1 for y-axis.
+        loc : float
+            The location along the specified axis to which points are compared.
+        tol : float, optional
+            The tolerance value for proximity. Default is 1e-3.
+
+        Returns
+        -------
+        picked_locs : array_like
+            Array of locations of the picked points.
+        picked_coords : array_like
+            Array of coordinates (along the other axis) of the picked points.
+        picked_values : array_like
+            Array of values of the picked points.
+
+        """
+        assert axis < 2
+
+        pick = np.where((np.abs(self.P[:, axis] - loc) < tol))[0]
+        picked_points = self.P[pick]
+        sorted_index = np.argsort(picked_points[:, 1-axis])
+        picked_points = picked_points[sorted_index]
+        picked_locs = picked_points[:, axis]
+        picked_coords = picked_points[:, 1-axis]
+        picked_values = picked_points[:, 2]
+
+        return picked_locs, picked_coords, picked_values
+    
     @update
     def translate(self, v: np.ndarray = np.array([0, 0, 0]), aux: bool = False) -> List[Tuple]:
         """
         Translate the data points by the given vector.
 
         Parameters
         ----------
```

### Comparing `pytom3d-0.0.0rc1/src/pytom3d/scan.py` & `pytom3d-0.0.0rc2/src/pytom3d/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,14 @@
             self.line = "-"
 
         try:
             self.alpha = kwargs.pop("alpha")
         except KeyError:
             self.alpha = 0.3
 
-        try:
-            self.err_bar = kwargs.pop("err_bar")
-        except KeyError:
-            self.err_bar = False
-
     def config_aspect(self, color, line, alpha):
         self.color = color
         self.line = line
         self.alpha = alpha
 
     def load_file(self, reader: callable, path: str, **kwargs: Dict['str', Any]) -> None:
         """
```

### Comparing `pytom3d-0.0.0rc1/src/pytom3d/stats.py` & `pytom3d-0.0.0rc2/src/pytom3d/stats.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc1/src/pytom3d/util.py` & `pytom3d-0.0.0rc2/src/pytom3d/util.py`

 * *Files identical despite different names*

### Comparing `pytom3d-0.0.0rc1/src/pytom3d/viewer.py` & `pytom3d-0.0.0rc2/src/pytom3d/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,14 +208,19 @@
 
         if reference is not None:
             ax.scatter3D(reference.P[:, 0], reference.P[:, 1], reference.P[:, 2], s=2, alpha=1)
 
         ax.axis('tight')
         plt.show()
 
+    def contour(self, topography):
+        fig, ax = plt.subplots(dpi=300)
+        ax.tricontourf(topography.P[:, 0], topography.P[:, 1], topography.P[:, 2])
+        plt.show()
+
 
 class PostViewer:
 
     def __init__(self, **kwargs) -> None:
 
         try:
             self.name = kwargs.pop("name")
@@ -293,46 +298,100 @@
         None
             This function does not return anything. It only sets the instance attributes for color bar limits.
 
         """
         self.mean_lim =  cbar_bounds(bot[2], top[2])
         self.std_lim = cbar_bounds(bot[3], top[3])
 
-    def scan_view(self, *scan: List) -> None:
+    def scan_view(self, swap: bool = False, *scan: List) -> None:
         """
-        Visualize scan data.
+        Plot scan data.
 
         Parameters
         ----------
+        swap : bool, optional
+            If True, swap x and y axes in the plot. Default is False.
         *scan : List
-            Variable number of scan objects. Each scan object should have attributes x, y, and y_err.
-            If y_err is not available, the function will plot only x and y.
+            List of scan data to plot. Each scan data should be provided as a list-like object.
 
         Returns
         -------
         None
-            This function does not return anything. It simply displays the plot.
 
         """
         fig, ax = plt.subplots(dpi=300)
+        for s in scan:
+            if swap:
+                ax.plot(s.y, s.x)
+
+            else:
+                ax.plot(s.x, s.y)
+
+            plt.show()
 
+    def scan_view_and_fill(self, swap: bool = False, *scan: List) -> None:
+        """
+        Plot scan data with filled error regions.
+
+        Parameters
+        ----------
+        swap : bool, optional
+            If True, swap x and y axes in the plot. Default is False.
+        *scan : List
+            List of scan data to plot. Each scan data should be provided as a list-like object.
+
+        Returns
+        -------
+        None
+
+        """
+        fig, ax = plt.subplots(dpi=300)
         for s in scan:
-            if s.err_bar:
-                try:
-                    ax.errorbar(s.x, s.y, s.y_err, fmt="-o", markersize=3, capsize=3, capthick=1, linewidth=0.8)
-                except KeyError:
-                    ax.plot(s.x, s.y)
+            if swap:
+                if s.y_err is not None:
+                    ax.fill_betweenx(s.x, s.y-s.y_err, s.y+s.y_err, alpha=0.5, edgecolor="none")
+                ax.plot(s.y, s.x)
+
             else:
-                try:
+                if s.y_err is not None:
                     ax.fill_between(s.x, s.y-s.y_err, s.y+s.y_err, alpha=0.5, edgecolor="none")
-                    ax.plot(s.x, s.y)
-                except KeyError:
-                    ax.plot(s.x, s.y)
+                ax.plot(s.x, s.y)
 
-        plt.show()
+            plt.show()
+
+    def scan_view_and_bar(self, swap: bool = False, *scan: List) -> None:
+        """
+        Plot scan data with error bars.
+
+        Parameters
+        ----------
+        swap : bool, optional
+            If True, swap x and y axes in the plot. Default is False.
+        *scan : List
+            List of scan data to plot. Each scan data should be provided as a list-like object.
+
+        Returns
+        -------
+        None
+
+        """
+        fig, ax = plt.subplots(dpi=300)
+        for s in scan:
+            if swap:
+                if s.y_err is not None:
+                    ax.errorbar(s.y, s.x, xerr=s.y_err, yerr=None, fmt="-o",
+                                markersize=3, capsize=3, capthick=1, linewidth=0.8)
+                pass
+
+            else:
+                if s.y_err is not None:
+                    ax.errorbar(s.x, s.y, xerr=None, yerr=s.y_err, fmt="-o",
+                                markersize=3, capsize=3, capthick=1, linewidth=0.8)
+
+            plt.show()
 
     def contour_and_scan_2(self, top_cnt, bot_cnt, top_scan = None, bot_scan = None) -> None:
         """
         Plot contour and scan data.
 
         Parameters
         ----------
```

### Comparing `pytom3d-0.0.0rc1/src/pytom3d.egg-info/PKG-INFO` & `pytom3d-0.0.0rc2/src/pytom3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytom3d
-Version: 0.0.0rc1
+Version: 0.0.0rc2
 Summary: PyToM-3D: Python Topography Manipulator in 3D
 Home-page: https://github.com/aletgn/pytom-3d.git
 Author: Alessandro Tognan
 Author-email: alessandro.tognan@gmail.com
 Project-URL: Bug Tracker, https://github.com/aletgn/pytom-3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

