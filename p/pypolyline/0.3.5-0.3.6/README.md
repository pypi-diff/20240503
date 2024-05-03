# Comparing `tmp/pypolyline-0.3.5.tar.gz` & `tmp/pypolyline-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypolyline-0.3.5.tar", last modified: Sun Oct  1 15:28:57 2023, max compression
+gzip compressed data, was "pypolyline-0.3.6.tar", last modified: Wed Oct  4 13:52:51 2023, max compression
```

## Comparing `pypolyline-0.3.5.tar` & `pypolyline-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.151954 pypolyline-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.147953 pypolyline-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-01 15:28:43.000000 pypolyline-0.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.147953 pypolyline-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2023-10-01 15:28:43.000000 pypolyline-0.3.5/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-10-01 15:28:43.000000 pypolyline-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-10-01 15:28:43.000000 pypolyline-0.3.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-10-01 15:28:57.151954 pypolyline-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-10-01 15:28:43.000000 pypolyline-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.147953 pypolyline-0.3.5/benches/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-10-01 15:28:43.000000 pypolyline-0.3.5/benches/benchmark_cgg.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-10-01 15:28:43.000000 pypolyline-0.3.5/benches/benchmark_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-01 15:28:43.000000 pypolyline-0.3.5/benches/benchmark_rust.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-01 15:28:43.000000 pypolyline-0.3.5/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-01 15:28:43.000000 pypolyline-0.3.5/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-01 15:28:43.000000 pypolyline-0.3.5/pypolyline_p.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-01 15:28:43.000000 pypolyline-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-01 15:28:57.151954 pypolyline-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-10-01 15:28:43.000000 pypolyline-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.147953 pypolyline-0.3.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-01 15:28:57.000000 pypolyline-0.3.5/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.147953 pypolyline-0.3.5/src/pypolyline/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-01 15:28:43.000000 pypolyline-0.3.5/src/pypolyline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2023-10-01 15:28:43.000000 pypolyline-0.3.5/src/pypolyline/cutil.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-01 15:28:43.000000 pypolyline-0.3.5/src/pypolyline/pypolyline_p.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-01 15:28:43.000000 pypolyline-0.3.5/src/pypolyline/stdbool.h
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-10-01 15:28:43.000000 pypolyline-0.3.5/src/pypolyline/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.151954 pypolyline-0.3.5/src/pypolyline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-10-01 15:28:57.000000 pypolyline-0.3.5/src/pypolyline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-01 15:28:57.000000 pypolyline-0.3.5/src/pypolyline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-01 15:28:57.000000 pypolyline-0.3.5/src/pypolyline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-01 15:28:57.000000 pypolyline-0.3.5/src/pypolyline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-01 15:28:57.000000 pypolyline-0.3.5/src/pypolyline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-01 15:28:57.151954 pypolyline-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2023-10-01 15:28:43.000000 pypolyline-0.3.5/tests/test_pypolyline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2023-10-04 13:52:37.000000 pypolyline-0.3.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-10-04 13:52:37.000000 pypolyline-0.3.6/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-10-04 13:52:37.000000 pypolyline-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2023-10-04 13:52:37.000000 pypolyline-0.3.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-10-04 13:52:51.293583 pypolyline-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-10-04 13:52:37.000000 pypolyline-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/benches/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2023-10-04 13:52:37.000000 pypolyline-0.3.6/benches/benchmark_cgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-10-04 13:52:37.000000 pypolyline-0.3.6/benches/benchmark_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-04 13:52:37.000000 pypolyline-0.3.6/benches/benchmark_rust.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-04 13:52:37.000000 pypolyline-0.3.6/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-04 13:52:37.000000 pypolyline-0.3.6/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-04 13:52:37.000000 pypolyline-0.3.6/pypolyline_p.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-04 13:52:37.000000 pypolyline-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 13:52:51.293583 pypolyline-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-10-04 13:52:37.000000 pypolyline-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-04 13:52:51.000000 pypolyline-0.3.6/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/src/pypolyline/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-04 13:52:37.000000 pypolyline-0.3.6/src/pypolyline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2023-10-04 13:52:37.000000 pypolyline-0.3.6/src/pypolyline/cutil.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-04 13:52:37.000000 pypolyline-0.3.6/src/pypolyline/pypolyline_p.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-04 13:52:37.000000 pypolyline-0.3.6/src/pypolyline/stdbool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-10-04 13:52:37.000000 pypolyline-0.3.6/src/pypolyline/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/src/pypolyline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-10-04 13:52:51.000000 pypolyline-0.3.6/src/pypolyline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-04 13:52:51.000000 pypolyline-0.3.6/src/pypolyline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 13:52:51.000000 pypolyline-0.3.6/src/pypolyline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-04 13:52:51.000000 pypolyline-0.3.6/src/pypolyline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-04 13:52:51.000000 pypolyline-0.3.6/src/pypolyline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 13:52:51.293583 pypolyline-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2023-10-04 13:52:37.000000 pypolyline-0.3.6/tests/test_pypolyline.py
```

### Comparing `pypolyline-0.3.5/.github/workflows/wheels.yml` & `pypolyline-0.3.6/.github/workflows/wheels.yml`

 * *Files 5% similar despite different names*

```diff
@@ -25,31 +25,31 @@
     needs: get_latest_lib_tag
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         include:
         - os: ubuntu-latest
-          pybuilds: cp3{7,8,9,10,11}-manylinux_x86_64
+          pybuilds: cp3{7,8,9,10,11,12}-manylinux_x86_64
           arch: x86_64
           id: linux
         - os: ubuntu-latest
-          pybuilds: cp3{7,8,9,10,11}-manylinux_aarch64
+          pybuilds: cp3{7,8,9,10,11,12}-manylinux_aarch64
           arch: aarch64
           id: linux_arm64
         - os: macos-latest
-          pybuilds: cp3{7,8,9,10,11}-macosx_x86_64
+          pybuilds: cp3{7,8,9,10,11,12}-macosx_x86_64
           arch: x86_64
           id: macos_x86
         - os: macos-latest
-          pybuilds: cp3{8,9,10,11}-macosx_arm64
+          pybuilds: cp3{8,9,10,11,12}-macosx_arm64
           arch: arm64
           id: macos_arm64
         - os: windows-latest
-          pybuilds: cp3{7,8,9,10,11}-win_amd64
+          pybuilds: cp3{7,8,9,10,11,12}-win_amd64
           arch: x86_64
           id: windows
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # Optional, use if you use setuptools_scm
```

### Comparing `pypolyline-0.3.5/PKG-INFO` & `pypolyline-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypolyline
-Version: 0.3.5
+Version: 0.3.6
 Summary: Fast Google Polyline encoding and decoding using Rust FFI
 Author-email: Stephan Hügel <urschrei@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Stephan Hügel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pypolyline-0.3.5/README.md` & `pypolyline-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/benchmarks.py` & `pypolyline-0.3.6/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/license.txt` & `pypolyline-0.3.6/license.txt`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/pyproject.toml` & `pypolyline-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/setup.py` & `pypolyline-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/src/pypolyline/cutil.pyx` & `pypolyline-0.3.6/src/pypolyline/cutil.pyx`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/src/pypolyline/util.py` & `pypolyline-0.3.6/src/pypolyline/util.py`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/src/pypolyline.egg-info/PKG-INFO` & `pypolyline-0.3.6/src/pypolyline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypolyline
-Version: 0.3.5
+Version: 0.3.6
 Summary: Fast Google Polyline encoding and decoding using Rust FFI
 Author-email: Stephan Hügel <urschrei@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Stephan Hügel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pypolyline-0.3.5/src/pypolyline.egg-info/SOURCES.txt` & `pypolyline-0.3.6/src/pypolyline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypolyline-0.3.5/tests/test_pypolyline.py` & `pypolyline-0.3.6/tests/test_pypolyline.py`

 * *Files identical despite different names*

