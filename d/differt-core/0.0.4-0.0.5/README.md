# Comparing `tmp/differt_core-0.0.4.tar.gz` & `tmp/differt_core-0.0.5.tar.gz`

## Comparing `differt_core-0.0.4.tar` & `differt_core-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 differt_core-0.0.4/differt-core/Cargo.toml
--rw-r--r--   0     1001      127     2681 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/.gitignore
--rw-r--r--   0     1001      127     1073 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/LICENSE.md
--rw-r--r--   0     1001      127      123 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/README.md
--rw-r--r--   0     1001      127      101 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/differt_core.pyi
--rw-r--r--   0     1001      127       14 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/requirements.txt
--rw-r--r--   0     1001      127     3516 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/src/lib.rs
--rw-r--r--   0     1001      127    15207 2023-11-14 16:12:07.000000 differt_core-0.0.4/differt-core/Cargo.lock
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 differt_core-0.0.4/pyproject.toml
--rw-r--r--   0     1001      127      123 2023-11-14 16:12:07.000000 differt_core-0.0.4/README.md
--rw-r--r--   0     1001      127     1073 2023-11-14 16:12:07.000000 differt_core-0.0.4/LICENSE.md
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 differt_core-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 differt_core-0.0.5/differt-core/Cargo.toml
+-rw-r--r--   0     1001      127     2681 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/.gitignore
+-rw-r--r--   0     1001      127     1073 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/LICENSE.md
+-rw-r--r--   0     1001      127      123 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/README.md
+-rw-r--r--   0     1001      127      101 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/differt_core.pyi
+-rw-r--r--   0     1001      127       14 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/requirements.txt
+-rw-r--r--   0     1001      127     3507 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/src/lib.rs
+-rw-r--r--   0     1001      127    15207 2023-11-14 16:42:31.000000 differt_core-0.0.5/differt-core/Cargo.lock
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 differt_core-0.0.5/pyproject.toml
+-rw-r--r--   0     1001      127      123 2023-11-14 16:42:31.000000 differt_core-0.0.5/README.md
+-rw-r--r--   0     1001      127     1073 2023-11-14 16:42:31.000000 differt_core-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 differt_core-0.0.5/PKG-INFO
```

### Comparing `differt_core-0.0.4/differt-core/.github/workflows/CI.yml` & `differt_core-0.0.5/differt-core/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `differt_core-0.0.4/differt-core/.gitignore` & `differt_core-0.0.5/differt-core/.gitignore`

 * *Files identical despite different names*

### Comparing `differt_core-0.0.4/differt-core/LICENSE.md` & `differt_core-0.0.5/differt-core/LICENSE.md`

 * *Files identical despite different names*

### Comparing `differt_core-0.0.4/differt-core/src/lib.rs` & `differt_core-0.0.5/differt-core/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 use numpy::ndarray::{s, Array2};
 use numpy::{IntoPyArray, PyArray2};
 use pyo3::prelude::*;
 
+const VERSION: &str = "0.0.5";
 
-const VERSION: &'static str = "0.0.4";
-
-/// Formats the sum of two numbers as string.
+/// Generate an array of path num_candidates.
 #[pyfunction]
 fn generate_path_candidates(py: Python<'_>, num_primitives: u32, order: u32) -> &PyArray2<u32> {
     if order == 0 {
         // One path of size 0
-        return Array2::default((1, 0)).into_pyarray(py);
+        return Array2::default((0, 1)).into_pyarray(py);
     } else if num_primitives == 0 {
         // Zero path of size order
-        return Array2::default((0, order as usize)).into_pyarray(py);
+        return Array2::default((order as usize, 0)).into_pyarray(py);
     } else if order == 1 {
         let mut path_candidates = Array2::default((1, num_primitives as usize));
 
-        for i in 0..num_primitives {
-            path_candidates[(0, i as usize)] = i;
+        for j in 0..num_primitives {
+            path_candidates[(0, j as usize)] = j;
         }
         return path_candidates.into_pyarray(py);
     }
     let num_choices = (num_primitives - 1) as usize;
     let num_candidates_per_batch = num_choices.pow(order - 1);
     let num_candidates = (num_primitives as usize) * num_candidates_per_batch;
 
@@ -60,17 +59,17 @@
     use super::*;
 
     use rstest::rstest;
 
     use pyo3::{types::IntoPyDict, Python};
 
     #[rstest]
-    #[case(0, 0, "np.empty((1, 0), dtype=np.uint32)")]
-    #[case(3, 0, "np.empty((1, 0), dtype=np.uint32)")]
-    #[case(0, 3, "np.empty((0, 3), dtype=np.uint32)")]
+    #[case(0, 0, "np.empty((0, 1), dtype=np.uint32)")]
+    #[case(3, 0, "np.empty((0, 1), dtype=np.uint32)")]
+    #[case(0, 3, "np.empty((3, 0), dtype=np.uint32)")]
     #[case(9, 1, "np.arange(9, dtype=np.uint32).reshape(1, 9)")]
     #[case(3, 1, "np.array([[0, 1, 2]], dtype=np.uint32)")]
     #[case(
         3,
         2,
         "np.array([[0, 1], [0, 2], [1, 0], [1, 2], [2, 0], [2, 1]], dtype=np.uint32).T"
     )]
```

### Comparing `differt_core-0.0.4/differt-core/Cargo.lock` & `differt_core-0.0.5/differt-core/Cargo.lock`

 * *Files identical despite different names*

### Comparing `differt_core-0.0.4/pyproject.toml` & `differt_core-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `differt_core-0.0.4/LICENSE.md` & `differt_core-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `differt_core-0.0.4/PKG-INFO` & `differt_core-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: differt-core
-Version: 0.0.4
+Version: 0.0.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE.md
 Author-email: Jérome Eertmans <jeertmans@icloud.com>
 Requires-Python: >=3.9
```

