# Comparing `tmp/fazah-3.14.tar.gz` & `tmp/fazah-3.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazah-3.14.tar", last modified: Fri May  3 07:27:20 2024, max compression
+gzip compressed data, was "fazah-3.15.tar", last modified: Fri May  3 07:37:33 2024, max compression
```

## Comparing `fazah-3.14.tar` & `fazah-3.15.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.073722 fazah-3.14/
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.072299 fazah-3.14/Fazah/
--rw-r--r--   0 aidenlang   (502) staff       (20)     1219 2024-05-03 06:20:07.000000 fazah-3.14/Fazah/Fazah.py
--rw-r--r--   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:20:07.000000 fazah-3.14/Fazah/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)      387 2024-05-03 07:27:20.073551 fazah-3.14/PKG-INFO
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.073361 fazah-3.14/fazah.egg-info/
--rw-r--r--   0 aidenlang   (502) staff       (20)      387 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/PKG-INFO
--rw-r--r--   0 aidenlang   (502) staff       (20)      245 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/SOURCES.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/dependency_links.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       34 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/requires.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       12 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/top_level.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 07:27:20.073757 fazah-3.14/setup.cfg
--rw-r--r--   0 aidenlang   (502) staff       (20)      516 2024-05-03 07:27:09.000000 fazah-3.14/setup.py
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.073106 fazah-3.14/tests/
--rw-r--r--   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:20:07.000000 fazah-3.14/tests/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.14/tests/test.openai.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.14/tests/test_gemini.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:37:33.483087 fazah-3.15/
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:37:33.481641 fazah-3.15/Fazah/
+-rw-r--r--   0 aidenlang   (502) staff       (20)       19 2024-05-03 07:37:08.000000 fazah-3.15/Fazah/__init__.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1219 2024-05-03 07:37:24.000000 fazah-3.15/Fazah/fazah.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 07:37:33.482899 fazah-3.15/PKG-INFO
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:37:33.482736 fazah-3.15/fazah.egg-info/
+-rw-r--r--   0 aidenlang   (502) staff       (20)      365 2024-05-03 07:37:33.000000 fazah-3.15/fazah.egg-info/PKG-INFO
+-rw-r--r--   0 aidenlang   (502) staff       (20)      227 2024-05-03 07:37:33.000000 fazah-3.15/fazah.egg-info/SOURCES.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 07:37:33.000000 fazah-3.15/fazah.egg-info/dependency_links.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       27 2024-05-03 07:37:33.000000 fazah-3.15/fazah.egg-info/requires.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        6 2024-05-03 07:37:33.000000 fazah-3.15/fazah.egg-info/top_level.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 07:37:33.483125 fazah-3.15/setup.cfg
+-rw-r--r--   0 aidenlang   (502) staff       (20)      496 2024-05-03 07:36:42.000000 fazah-3.15/setup.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:37:33.482403 fazah-3.15/tests/
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.15/tests/test.openai.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.15/tests/test_gemini.py
```

### Comparing `fazah-3.14/Fazah/Fazah.py` & `fazah-3.15/Fazah/fazah.py`

 * *Files identical despite different names*

### Comparing `fazah-3.14/tests/test.openai.py` & `fazah-3.15/tests/test.openai.py`

 * *Files identical despite different names*

### Comparing `fazah-3.14/tests/test_gemini.py` & `fazah-3.15/tests/test_gemini.py`

 * *Files identical despite different names*

