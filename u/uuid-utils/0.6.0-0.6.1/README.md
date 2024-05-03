# Comparing `tmp/uuid_utils-0.6.0.tar.gz` & `tmp/uuid_utils-0.6.1.tar.gz`

## Comparing `uuid_utils-0.6.0.tar` & `uuid_utils-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 uuid_utils-0.6.0/Cargo.toml
--rw-r--r--   0     1001      127     7872 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      703 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/.gitignore
--rw-r--r--   0     1001      127     1487 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/LICENSE.md
--rw-r--r--   0     1001      127      410 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/Makefile
--rw-r--r--   0     1001      127     3048 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/README.md
--rw-r--r--   0     1001      127      201 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/benchmarks/README.md
--rw-r--r--   0     1001      127     1137 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/benchmarks/bench_generator.py
--rw-r--r--   0     1001      127     1331 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/benchmarks/bench_parser.py
--rw-r--r--   0     1001      127      622 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/python/uuid_utils/__init__.py
--rw-r--r--   0     1001      127     6057 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/python/uuid_utils/__init__.pyi
--rw-r--r--   0     1001      127     1617 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/python/uuid_utils/compat/__init__.py
--rw-r--r--   0     1001      127     1425 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/python/uuid_utils/compat/__init__.pyi
--rw-r--r--   0     1001      127        0 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/python/uuid_utils/py.typed
--rw-r--r--   0     1001      127       68 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/requirements.txt
--rw-r--r--   0     1001      127    12408 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/src/lib.rs
--rw-r--r--   0     1001      127        0 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/tests/__init__.py
--rw-r--r--   0     1001      127        0 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/tests/test_compat/__init__.py
--rw-r--r--   0     1001      127      603 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/tests/test_compat/test_compat.py
--rw-r--r--   0     1001      127     5649 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/tests/test_uuid.py
--rw-r--r--   0     1001      127    12942 2023-11-03 12:03:54.000000 uuid_utils-0.6.0/Cargo.lock
--rw-r--r--   0     1001      127     1392 2023-11-03 12:03:49.000000 uuid_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 uuid_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 uuid_utils-0.6.1/Cargo.toml
+-rw-r--r--   0     1001      127     7913 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      703 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/.gitignore
+-rw-r--r--   0     1001      127     1487 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/LICENSE.md
+-rw-r--r--   0     1001      127      410 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/Makefile
+-rw-r--r--   0     1001      127     3048 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/README.md
+-rw-r--r--   0     1001      127      201 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/benchmarks/README.md
+-rw-r--r--   0     1001      127     1137 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/benchmarks/bench_generator.py
+-rw-r--r--   0     1001      127     1331 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/benchmarks/bench_parser.py
+-rw-r--r--   0     1001      127      622 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/python/uuid_utils/__init__.py
+-rw-r--r--   0     1001      127     6057 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/python/uuid_utils/__init__.pyi
+-rw-r--r--   0     1001      127     1617 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/python/uuid_utils/compat/__init__.py
+-rw-r--r--   0     1001      127     1425 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/python/uuid_utils/compat/__init__.pyi
+-rw-r--r--   0     1001      127        0 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/python/uuid_utils/py.typed
+-rw-r--r--   0     1001      127       68 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/requirements.txt
+-rw-r--r--   0     1001      127    12408 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/src/lib.rs
+-rw-r--r--   0     1001      127        0 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/tests/__init__.py
+-rw-r--r--   0     1001      127        0 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/tests/test_compat/__init__.py
+-rw-r--r--   0     1001      127      603 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/tests/test_compat/test_compat.py
+-rw-r--r--   0     1001      127     5649 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/tests/test_uuid.py
+-rw-r--r--   0     1001      127    12942 2023-11-06 09:30:20.000000 uuid_utils-0.6.1/Cargo.lock
+-rw-r--r--   0     1001      127     1392 2023-11-06 09:30:12.000000 uuid_utils-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 uuid_utils-0.6.1/PKG-INFO
```

### Comparing `uuid_utils-0.6.0/.github/workflows/ci.yml` & `uuid_utils-0.6.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [lint, linux, windows, macos, sdist]
+    needs: [lint, linux, linux-cross, musllinux, musllinux-cross, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `uuid_utils-0.6.0/.gitignore` & `uuid_utils-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/LICENSE.md` & `uuid_utils-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/README.md` & `uuid_utils-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/benchmarks/bench_generator.py` & `uuid_utils-0.6.1/benchmarks/bench_generator.py`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/benchmarks/bench_parser.py` & `uuid_utils-0.6.1/benchmarks/bench_parser.py`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/python/uuid_utils/__init__.py` & `uuid_utils-0.6.1/python/uuid_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/python/uuid_utils/__init__.pyi` & `uuid_utils-0.6.1/python/uuid_utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/python/uuid_utils/compat/__init__.py` & `uuid_utils-0.6.1/python/uuid_utils/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/python/uuid_utils/compat/__init__.pyi` & `uuid_utils-0.6.1/python/uuid_utils/compat/__init__.pyi`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/src/lib.rs` & `uuid_utils-0.6.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/tests/test_compat/test_compat.py` & `uuid_utils-0.6.1/tests/test_compat/test_compat.py`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/tests/test_uuid.py` & `uuid_utils-0.6.1/tests/test_uuid.py`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/Cargo.lock` & `uuid_utils-0.6.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
  "md-5",
  "rand",
  "sha1_smol",
 ]
 
 [[package]]
 name = "uuid-utils"
-version = "0.6.0"
+version = "0.6.1"
 dependencies = [
  "mac_address",
  "pyo3",
  "rand",
  "uuid",
 ]
```

### Comparing `uuid_utils-0.6.0/pyproject.toml` & `uuid_utils-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uuid_utils-0.6.0/PKG-INFO` & `uuid_utils-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uuid_utils
-Version: 0.6.0
+Version: 0.6.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uuid_utils Version: 0.6.0 Classifier: Development
+Metadata-Version: 2.1 Name: uuid_utils Version: 0.6.1 Classifier: Development
 Status :: 3 - Alpha Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Rust Classifier: Intended
```

