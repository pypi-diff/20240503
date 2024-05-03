# Comparing `tmp/libsrg_apps-0.1.0.tar.gz` & `tmp/libsrg_apps-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg_apps-0.1.0.tar", max compression
+gzip compressed data, was "libsrg_apps-1.0.0.tar", max compression
```

## Comparing `libsrg_apps-0.1.0.tar` & `libsrg_apps-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6179 2024-05-02 19:07:58.823920 libsrg_apps-0.1.0/README.md
--rwxr-xr-x   0        0        0    15705 2024-04-09 15:09:14.551097 libsrg_apps-0.1.0/libsrg_apps/ReZFS.py
--rwxr-xr-x   0        0        0     7024 2023-10-05 17:56:35.188332 libsrg_apps-0.1.0/libsrg_apps/Stage0.py
--rw-r--r--   0        0        0        0 2024-05-02 19:09:02.278580 libsrg_apps-0.1.0/libsrg_apps/__init__.py
--rwxr-xr-x   0        0        0    26598 2024-04-09 15:09:14.543097 libsrg_apps-0.1.0/libsrg_apps/ztool.py
--rw-r--r--   0        0        0      694 2024-05-02 19:52:42.089631 libsrg_apps-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 libsrg_apps-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1154 2024-05-02 20:58:57.454367 libsrg_apps-1.0.0/README.md
+-rwxr-xr-x   0        0        0    15705 2024-04-09 15:09:14.551097 libsrg_apps-1.0.0/libsrg_apps/ReZFS.py
+-rwxr-xr-x   0        0        0     7024 2023-10-05 17:56:35.188332 libsrg_apps-1.0.0/libsrg_apps/Stage0.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:09:02.278580 libsrg_apps-1.0.0/libsrg_apps/__init__.py
+-rwxr-xr-x   0        0        0    26598 2024-04-09 15:09:14.543097 libsrg_apps-1.0.0/libsrg_apps/ztool.py
+-rw-r--r--   0        0        0      694 2024-05-02 20:59:10.203300 libsrg_apps-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 libsrg_apps-1.0.0/PKG-INFO
```

### Comparing `libsrg_apps-0.1.0/libsrg_apps/ReZFS.py` & `libsrg_apps-1.0.0/libsrg_apps/ReZFS.py`

 * *Files identical despite different names*

### Comparing `libsrg_apps-0.1.0/libsrg_apps/Stage0.py` & `libsrg_apps-1.0.0/libsrg_apps/Stage0.py`

 * *Files identical despite different names*

### Comparing `libsrg_apps-0.1.0/libsrg_apps/ztool.py` & `libsrg_apps-1.0.0/libsrg_apps/ztool.py`

 * *Files identical despite different names*

### Comparing `libsrg_apps-0.1.0/pyproject.toml` & `libsrg_apps-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg-apps"
-version = "0.1.0"
+version = "1.0.0"
 description = "This is a handful of applications migrated out of lilbsrg."
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

