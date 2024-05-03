# Comparing `tmp/mymorsecode-0.1.0.tar.gz` & `tmp/mymorsecode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymorsecode-0.1.0.tar", max compression
+gzip compressed data, was "mymorsecode-0.2.0.tar", max compression
```

## Comparing `mymorsecode-0.1.0.tar` & `mymorsecode-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2024-05-03 15:08:38.424611 mymorsecode-0.1.0/LICENSE
--rw-r--r--   0        0        0       11 2024-05-03 15:06:25.053376 mymorsecode-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-03 15:01:12.596031 mymorsecode-0.1.0/mymorsecode/__init__.py
--rw-r--r--   0        0        0      336 2024-05-03 15:10:52.390855 mymorsecode-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 mymorsecode-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-03 15:08:38.424611 mymorsecode-0.2.0/LICENSE
+-rw-r--r--   0        0        0       11 2024-05-03 15:06:25.053376 mymorsecode-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 15:01:12.596031 mymorsecode-0.2.0/mymorsecode/__init__.py
+-rw-r--r--   0        0        0      352 2024-05-03 15:13:15.724213 mymorsecode-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 mymorsecode-0.2.0/PKG-INFO
```

### Comparing `mymorsecode-0.1.0/LICENSE` & `mymorsecode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mymorsecode-0.1.0/PKG-INFO` & `mymorsecode-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: mymorsecode
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/tct123/morsecode
+License: MIT
 Author: tct123
 Author-email: 42028373+tct123@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/tct123/morsecode
```

