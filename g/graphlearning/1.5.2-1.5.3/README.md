# Comparing `tmp/graphlearning-1.5.2.tar.gz` & `tmp/graphlearning-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlearning-1.5.2.tar", last modified: Wed May  1 20:50:56 2024, max compression
+gzip compressed data, was "graphlearning-1.5.3.tar", last modified: Fri May  3 02:14:02 2024, max compression
```

## Comparing `graphlearning-1.5.2.tar` & `graphlearning-1.5.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.137328 graphlearning-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-01 20:50:41.000000 graphlearning-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 20:50:41.000000 graphlearning-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-01 20:50:56.137328 graphlearning-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-01 20:50:41.000000 graphlearning-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.133328 graphlearning-1.5.2/c_code/
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/cextensions.c
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/hjsolvers.c
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/hjsolvers.h
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/lp_iterate.c
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/lp_iterate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/maj_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/maj_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/maj_simple_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mbo_convolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mbo_speedy_volume_preserving.c
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/memory_allocation.c
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/memory_allocation.h
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mnist_benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/mnist_benchmark.h
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-01 20:50:41.000000 graphlearning-1.5.2/c_code/vector_operations.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.133328 graphlearning-1.5.2/graphlearning/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23366 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    77849 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/trainsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22463 2024-05-01 20:50:41.000000 graphlearning-1.5.2/graphlearning/weightmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:50:56.137328 graphlearning-1.5.2/graphlearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 20:50:56.000000 graphlearning-1.5.2/graphlearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-01 20:50:42.000000 graphlearning-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:50:56.137328 graphlearning-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-01 20:50:42.000000 graphlearning-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.119960 graphlearning-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 02:13:47.000000 graphlearning-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:13:47.000000 graphlearning-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-03 02:14:02.119960 graphlearning-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-03 02:13:47.000000 graphlearning-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.115960 graphlearning-1.5.3/c_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/cextensions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/hjsolvers.c
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/hjsolvers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/lp_iterate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/lp_iterate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/maj_dijkstra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/maj_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/maj_simple_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mbo_convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mbo_speedy_volume_preserving.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/memory_allocation.c
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/memory_allocation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mnist_benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mnist_benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/vector_operations.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.119960 graphlearning-1.5.3/graphlearning/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23417 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77849 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/trainsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22463 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/weightmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.119960 graphlearning-1.5.3/graphlearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-03 02:13:48.000000 graphlearning-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:14:02.119960 graphlearning-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-03 02:13:48.000000 graphlearning-1.5.3/setup.py
```

### Comparing `graphlearning-1.5.2/LICENSE` & `graphlearning-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/PKG-INFO` & `graphlearning-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.2
+Version: 1.5.3
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.2/README.md` & `graphlearning-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/cextensions.c` & `graphlearning-1.5.3/c_code/cextensions.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/hjsolvers.c` & `graphlearning-1.5.3/c_code/hjsolvers.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/hjsolvers.h` & `graphlearning-1.5.3/c_code/hjsolvers.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/lp_iterate.c` & `graphlearning-1.5.3/c_code/lp_iterate.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/lp_iterate.h` & `graphlearning-1.5.3/c_code/lp_iterate.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/maj_dijkstra.h` & `graphlearning-1.5.3/c_code/maj_dijkstra.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/maj_implicit_heap.h` & `graphlearning-1.5.3/c_code/maj_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/maj_simple_implicit_heap.h` & `graphlearning-1.5.3/c_code/maj_simple_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/mbo_convolution.h` & `graphlearning-1.5.3/c_code/mbo_convolution.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/mbo_speedy_volume_preserving.c` & `graphlearning-1.5.3/c_code/mbo_speedy_volume_preserving.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/memory_allocation.c` & `graphlearning-1.5.3/c_code/memory_allocation.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/mnist_benchmark.c` & `graphlearning-1.5.3/c_code/mnist_benchmark.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/mnist_benchmark.h` & `graphlearning-1.5.3/c_code/mnist_benchmark.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/c_code/vector_operations.h` & `graphlearning-1.5.3/c_code/vector_operations.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/active_learning.py` & `graphlearning-1.5.3/graphlearning/active_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,16 +291,16 @@
             self.storage = 'full'
         else:
             self.storage = 'trunc'
         
         
     def compute(self, u, candidate_ind):
         if self.storage == 'full':
-            col_norms = np.linalg.norm(self.C, axis=0)**2.
-            diag_terms = self.gamma2 + self.C.diagonal()
+            col_norms = np.linalg.norm(self.C[:,candidate_ind], axis=0)**2.
+            diag_terms = self.gamma2 + self.C.diagonal()[candidate_ind]
         else:
             Cavk = self.C @ self.V[candidate_ind,:].T
             col_norms = np.linalg.norm(Cavk, axis=0)**2.
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
             
         return col_norms / diag_terms
 
@@ -376,16 +376,16 @@
             self.storage = 'full'
         else:
             self.storage = 'trunc'
         
         
     def compute(self, u, candidate_ind):
         if self.storage == 'full':
-            col_sums = np.sum(self.C, axis=0)**2.
-            diag_terms = selg.gamma2 + self.C.diagonal()
+            col_sums = np.sum(self.C[:, candidate_ind], axis=0)**2.
+            diag_terms = self.gamma2 + self.C.diagonal()[candidate_ind]
         else:
             Cavk = self.C @ self.V[candidate_ind,:].T
             col_sums = np.sum(Cavk, axis=0)**2.
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
             
         return col_sums/ diag_terms
 
@@ -461,15 +461,15 @@
         self.unc_sampling = unc_sampling(unc_method=unc_method)
         if self.V is None:
             self.storage = 'full'
         else:
             self.storage = 'trunc'
         
     def compute(self, u, candidate_ind):
-        unc_terms = self.unc_sampling.compute_values(active_learning, u)
+        unc_terms = self.unc_sampling.compute(u, candidate_ind)
         if self.storage == 'full':
             col_norms = np.linalg.norm(self.C, axis=0)
             diag_terms = self.gamma2 + self.C.diagonal()
         else:
             Cavk = self.C @ self.V[candidate_ind,:].T
             col_norms = np.linalg.norm(Cavk, axis=0)
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
@@ -541,22 +541,22 @@
     Journal on Selected Areas in Information Theory 1, 167–177 (May 2020).
     """
     def __init__(self, C, V=None, gamma2=0.1**2., unc_method='smallest_margin'):
         assert (C.shape[0] == C.shape[1]) or (V is not None)
         self.C = C.copy()
         self.V = V
         self.gamma2 = gamma2
-        self.unc_sampling = unc_sampling(method=unc_method)
+        self.unc_sampling = unc_sampling(unc_method=unc_method)
         if self.V is None:
             self.storage = 'full'
         else:
             self.storage = 'trunc'
         
     def compute(self, u, candidate_ind):
-        unc_terms = self.unc_sampling.compute_values(active_learning, u)
+        unc_terms = self.unc_sampling.compute(u, candidate_ind)
         if self.storage == 'full':
             col_norms = np.linalg.norm(self.C, axis=0)**2.
             diag_terms = self.gamma2 + self.C.diagonal()
         else:
             Cavk = self.C @ self.V[candidate_ind,:].T
             col_norms = np.linalg.norm(Cavk, axis=0)**2.
             diag_terms = (self.gamma2 + np.array([np.inner(self.V[k,:], Cavk[:, i]) for i,k in enumerate(candidate_ind)]))
```

### Comparing `graphlearning-1.5.2/graphlearning/clustering.py` & `graphlearning-1.5.3/graphlearning/clustering.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/datasets.py` & `graphlearning-1.5.3/graphlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/graph.py` & `graphlearning-1.5.3/graphlearning/graph.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/ssl.py` & `graphlearning-1.5.3/graphlearning/ssl.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/trainsets.py` & `graphlearning-1.5.3/graphlearning/trainsets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/utils.py` & `graphlearning-1.5.3/graphlearning/utils.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning/weightmatrix.py` & `graphlearning-1.5.3/graphlearning/weightmatrix.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/graphlearning.egg-info/PKG-INFO` & `graphlearning-1.5.3/graphlearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.2
+Version: 1.5.3
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.2/graphlearning.egg-info/SOURCES.txt` & `graphlearning-1.5.3/graphlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.2/pyproject.toml` & `graphlearning-1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools]
 packages = ['graphlearning']
 
 
 [project]
 name = "graphlearning"
-version = "1.5.2"
+version = "1.5.3"
 authors = [
   { name="Jeff Calder", email="jwcalder@umn.edu" },
 ]
 description = "Python package for graph-based clustering and semi-supervised learning"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.6"
```

### Comparing `graphlearning-1.5.2/setup.py` & `graphlearning-1.5.3/setup.py`

 * *Files identical despite different names*

