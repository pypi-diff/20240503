# Comparing `tmp/lfg_llama-1.1.0.tar.gz` & `tmp/lfg_llama-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.1.0.tar", last modified: Fri May  3 13:17:32 2024, max compression
+gzip compressed data, was "lfg_llama-1.1.1.tar", last modified: Fri May  3 14:13:44 2024, max compression
```

## Comparing `lfg_llama-1.1.0.tar` & `lfg_llama-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 13:17:32.895158 lfg_llama-1.1.0/
--rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 13:17:32.894955 lfg_llama-1.1.0/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1030 2024-05-03 10:03:47.000000 lfg_llama-1.1.0/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 13:17:32.893284 lfg_llama-1.1.0/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.0/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     1323 2024-05-03 10:00:41.000000 lfg_llama-1.1.0/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 13:17:32.894672 lfg_llama-1.1.0/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 13:17:32.895227 lfg_llama-1.1.0/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      682 2024-05-03 13:17:31.000000 lfg_llama-1.1.0/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:13:44.219226 lfg_llama-1.1.1/
+-rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 14:13:44.219022 lfg_llama-1.1.1/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1030 2024-05-03 10:03:47.000000 lfg_llama-1.1.1/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:13:44.217534 lfg_llama-1.1.1/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.1/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2173 2024-05-03 14:13:28.000000 lfg_llama-1.1.1/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:13:44.218791 lfg_llama-1.1.1/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 14:13:44.219274 lfg_llama-1.1.1/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-03 14:13:41.000000 lfg_llama-1.1.1/setup.py
```

### Comparing `lfg_llama-1.1.0/PKG-INFO` & `lfg_llama-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.1.0
+Version: 1.1.1
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

### Comparing `lfg_llama-1.1.0/README.md` & `lfg_llama-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.1.0/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.1.1/lfg_llama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.1.0
+Version: 1.1.1
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

