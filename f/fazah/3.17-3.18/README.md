# Comparing `tmp/fazah-3.17.tar.gz` & `tmp/fazah-3.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazah-3.17.tar", last modified: Fri May  3 20:19:17 2024, max compression
+gzip compressed data, was "fazah-3.18.tar", last modified: Fri May  3 20:23:45 2024, max compression
```

## Comparing `fazah-3.17.tar` & `fazah-3.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:19:17.311575 fazah-3.17/
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:19:17.309981 fazah-3.17/Fazah/
--rw-r--r--   0 aidenlang   (502) staff       (20)       19 2024-05-03 20:18:52.000000 fazah-3.17/Fazah/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1222 2024-05-03 20:18:11.000000 fazah-3.17/Fazah/fazah.py
--rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 20:19:17.311370 fazah-3.17/PKG-INFO
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:19:17.311148 fazah-3.17/fazah.egg-info/
--rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 20:19:17.000000 fazah-3.17/fazah.egg-info/PKG-INFO
--rw-r--r--   0 aidenlang   (502) staff       (20)      227 2024-05-03 20:19:17.000000 fazah-3.17/fazah.egg-info/SOURCES.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 20:19:17.000000 fazah-3.17/fazah.egg-info/dependency_links.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       27 2024-05-03 20:19:17.000000 fazah-3.17/fazah.egg-info/requires.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        6 2024-05-03 20:19:17.000000 fazah-3.17/fazah.egg-info/top_level.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 20:19:17.311614 fazah-3.17/setup.cfg
--rw-r--r--   0 aidenlang   (502) staff       (20)      496 2024-05-03 20:17:46.000000 fazah-3.17/setup.py
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:19:17.310894 fazah-3.17/tests/
--rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.17/tests/test.openai.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.17/tests/test_gemini.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:23:45.881854 fazah-3.18/
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:23:45.879810 fazah-3.18/Fazah/
+-rw-r--r--   0 aidenlang   (502) staff       (20)       71 2024-05-03 20:22:51.000000 fazah-3.18/Fazah/__init__.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1222 2024-05-03 20:23:26.000000 fazah-3.18/Fazah/fazah.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 20:23:45.881657 fazah-3.18/PKG-INFO
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:23:45.881435 fazah-3.18/fazah.egg-info/
+-rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 20:23:45.000000 fazah-3.18/fazah.egg-info/PKG-INFO
+-rw-r--r--   0 aidenlang   (502) staff       (20)      227 2024-05-03 20:23:45.000000 fazah-3.18/fazah.egg-info/SOURCES.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 20:23:45.000000 fazah-3.18/fazah.egg-info/dependency_links.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       27 2024-05-03 20:23:45.000000 fazah-3.18/fazah.egg-info/requires.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        6 2024-05-03 20:23:45.000000 fazah-3.18/fazah.egg-info/top_level.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 20:23:45.881896 fazah-3.18/setup.cfg
+-rw-r--r--   0 aidenlang   (502) staff       (20)      496 2024-05-03 20:23:06.000000 fazah-3.18/setup.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 20:23:45.881136 fazah-3.18/tests/
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.18/tests/test.openai.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.18/tests/test_gemini.py
```

### Comparing `fazah-3.17/Fazah/fazah.py` & `fazah-3.18/Fazah/fazah.py`

 * *Files identical despite different names*

### Comparing `fazah-3.17/tests/test.openai.py` & `fazah-3.18/tests/test.openai.py`

 * *Files identical despite different names*

### Comparing `fazah-3.17/tests/test_gemini.py` & `fazah-3.18/tests/test_gemini.py`

 * *Files identical despite different names*

