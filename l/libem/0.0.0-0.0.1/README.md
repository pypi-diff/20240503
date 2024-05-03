# Comparing `tmp/libem-0.0.0.tar.gz` & `tmp/libem-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.0.tar", last modified: Wed May  1 03:13:27 2024, max compression
+gzip compressed data, was "libem-0.0.1.tar", last modified: Fri May  3 09:46:18 2024, max compression
```

## Comparing `libem-0.0.0.tar` & `libem-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,42 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-01 03:13:27.919441 libem-0.0.0/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.0/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-01 03:13:27.919334 libem-0.0.0/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)       36 2024-05-01 02:16:29.000000 libem-0.0.0/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-01 03:13:27.918693 libem-0.0.0/benchmark/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 02:59:47.000000 libem-0.0.0/benchmark/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-01 03:13:27.919138 libem-0.0.0/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-01 03:13:27.000000 libem-0.0.0/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      210 2024-05-01 03:13:27.000000 libem-0.0.0/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-01 03:13:27.000000 libem-0.0.0/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)       30 2024-05-01 03:13:27.000000 libem-0.0.0/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-01 03:13:27.000000 libem-0.0.0/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-01 03:13:27.919225 libem-0.0.0/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 03:03:29.000000 libem-0.0.0/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-01 03:13:27.919473 libem-0.0.0/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      421 2024-05-01 02:58:52.000000 libem-0.0.0/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.852364 libem-0.0.1/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.1/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-03 09:46:18.852248 libem-0.0.1/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)      212 2024-05-03 05:42:27.000000 libem-0.0.1/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.848492 libem-0.0.1/benchmark/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 02:59:47.000000 libem-0.0.1/benchmark/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.848562 libem-0.0.1/eval/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:23:30.000000 libem-0.0.1/eval/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.849524 libem-0.0.1/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      350 2024-05-03 08:56:58.000000 libem-0.0.1/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.850879 libem-0.0.1/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)      104 2024-05-03 09:12:55.000000 libem-0.0.1/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1542 2024-05-03 09:32:13.000000 libem-0.0.1/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.1/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.1/libem/browse/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      364 2024-05-03 08:56:38.000000 libem-0.0.1/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.851259 libem-0.0.1/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.1/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2357 2024-05-03 09:44:29.000000 libem-0.0.1/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)      240 2024-05-03 06:53:59.000000 libem-0.0.1/libem/core/struct.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.851797 libem-0.0.1/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:10:31.000000 libem-0.0.1/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      352 2024-05-03 09:41:15.000000 libem-0.0.1/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.1/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.1/libem/match/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      141 2024-05-03 06:50:11.000000 libem-0.0.1/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.852069 libem-0.0.1/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:13:20.000000 libem-0.0.1/libem/prepare/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 19:12:22.000000 libem-0.0.1/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.1/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-02 20:20:44.000000 libem-0.0.1/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      235 2024-05-02 20:19:34.000000 libem-0.0.1/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.850299 libem-0.0.1/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)      659 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       27 2024-05-03 09:46:18.000000 libem-0.0.1/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-03 09:46:18.852136 libem-0.0.1/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-01 03:03:29.000000 libem-0.0.1/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-03 09:46:18.852395 libem-0.0.1/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      421 2024-05-03 09:45:46.000000 libem-0.0.1/setup.py
```

### Comparing `libem-0.0.0/LICENSE` & `libem-0.0.1/LICENSE`

 * *Files identical despite different names*

