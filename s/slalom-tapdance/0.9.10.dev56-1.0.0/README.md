# Comparing `tmp/slalom_tapdance-0.9.10.dev56.tar.gz` & `tmp/slalom_tapdance-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-0.9.10.dev56.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.0.tar", max compression
```

## Comparing `slalom_tapdance-0.9.10.dev56.tar` & `slalom_tapdance-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-02 16:25:14.818699 slalom_tapdance-0.9.10.dev56/LICENSE
--rw-r--r--   0        0        0     1221 2024-05-02 16:25:29.790791 slalom_tapdance-0.9.10.dev56/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/install_helper.py
--rw-r--r--   0        0        0    37120 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/states.py
--rw-r--r--   0        0        0    11850 2024-05-02 16:25:14.822699 slalom_tapdance-0.9.10.dev56/tapdance/syncs.py
--rw-r--r--   0        0        0     1358 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev56/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-02 21:37:39.179500 slalom_tapdance-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1213 2024-05-02 21:37:39.179500 slalom_tapdance-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-02 21:37:39.179500 slalom_tapdance-1.0.0/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-02 21:37:39.179500 slalom_tapdance-1.0.0/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-02 21:37:39.179500 slalom_tapdance-1.0.0/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-02 21:37:39.179500 slalom_tapdance-1.0.0/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-02 21:37:39.183500 slalom_tapdance-1.0.0/tapdance/install_helper.py
+-rw-r--r--   0        0        0    37120 2024-05-02 21:37:39.183500 slalom_tapdance-1.0.0/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-02 21:37:39.183500 slalom_tapdance-1.0.0/tapdance/states.py
+-rw-r--r--   0        0        0    11850 2024-05-02 21:37:39.183500 slalom_tapdance-1.0.0/tapdance/syncs.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.0/PKG-INFO
```

### Comparing `slalom_tapdance-0.9.10.dev56/LICENSE` & `slalom_tapdance-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/pyproject.toml` & `slalom_tapdance-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "0.9.10-dev.56"
+version = "1.0.0"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/cli.py` & `slalom_tapdance-1.0.0/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/config.py` & `slalom_tapdance-1.0.0/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/docker.py` & `slalom_tapdance-1.0.0/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/install_helper.py` & `slalom_tapdance-1.0.0/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/plans.py` & `slalom_tapdance-1.0.0/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/states.py` & `slalom_tapdance-1.0.0/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/tapdance/syncs.py` & `slalom_tapdance-1.0.0/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev56/PKG-INFO` & `slalom_tapdance-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 0.9.10.dev56
+Version: 1.0.0
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

