# Comparing `tmp/fazah-3.13.tar.gz` & `tmp/fazah-3.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazah-3.13.tar", last modified: Fri May  3 06:25:22 2024, max compression
+gzip compressed data, was "fazah-3.14.tar", last modified: Fri May  3 07:27:20 2024, max compression
```

## Comparing `fazah-3.13.tar` & `fazah-3.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:25:22.916292 fazah-3.13/
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:25:22.914332 fazah-3.13/Fazah/
--rw-r--r--   0 aidenlang   (502) staff       (20)     1219 2024-05-03 06:20:07.000000 fazah-3.13/Fazah/Fazah.py
--rw-r--r--   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:20:07.000000 fazah-3.13/Fazah/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)      387 2024-05-03 06:25:22.916069 fazah-3.13/PKG-INFO
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:25:22.915861 fazah-3.13/fazah.egg-info/
--rw-r--r--   0 aidenlang   (502) staff       (20)      387 2024-05-03 06:25:22.000000 fazah-3.13/fazah.egg-info/PKG-INFO
--rw-r--r--   0 aidenlang   (502) staff       (20)      245 2024-05-03 06:25:22.000000 fazah-3.13/fazah.egg-info/SOURCES.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 06:25:22.000000 fazah-3.13/fazah.egg-info/dependency_links.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       34 2024-05-03 06:25:22.000000 fazah-3.13/fazah.egg-info/requires.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       12 2024-05-03 06:25:22.000000 fazah-3.13/fazah.egg-info/top_level.txt
--rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 06:25:22.916336 fazah-3.13/setup.cfg
--rw-r--r--   0 aidenlang   (502) staff       (20)      516 2024-05-03 06:22:27.000000 fazah-3.13/setup.py
-drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:25:22.915162 fazah-3.13/tests/
--rw-r--r--   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:20:07.000000 fazah-3.13/tests/__init__.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1212 2024-05-03 06:20:07.000000 fazah-3.13/tests/test.openai.py
--rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.13/tests/test_gemini.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.073722 fazah-3.14/
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.072299 fazah-3.14/Fazah/
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1219 2024-05-03 06:20:07.000000 fazah-3.14/Fazah/Fazah.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:20:07.000000 fazah-3.14/Fazah/__init__.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)      387 2024-05-03 07:27:20.073551 fazah-3.14/PKG-INFO
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.073361 fazah-3.14/fazah.egg-info/
+-rw-r--r--   0 aidenlang   (502) staff       (20)      387 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/PKG-INFO
+-rw-r--r--   0 aidenlang   (502) staff       (20)      245 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/SOURCES.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)        1 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/dependency_links.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       34 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/requires.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       12 2024-05-03 07:27:20.000000 fazah-3.14/fazah.egg-info/top_level.txt
+-rw-r--r--   0 aidenlang   (502) staff       (20)       38 2024-05-03 07:27:20.073757 fazah-3.14/setup.cfg
+-rw-r--r--   0 aidenlang   (502) staff       (20)      516 2024-05-03 07:27:09.000000 fazah-3.14/setup.py
+drwxr-xr-x   0 aidenlang   (502) staff       (20)        0 2024-05-03 07:27:20.073106 fazah-3.14/tests/
+-rw-r--r--   0 aidenlang   (502) staff       (20)        0 2024-05-03 06:20:07.000000 fazah-3.14/tests/__init__.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1218 2024-05-03 06:26:06.000000 fazah-3.14/tests/test.openai.py
+-rw-r--r--   0 aidenlang   (502) staff       (20)     1320 2024-05-03 06:22:39.000000 fazah-3.14/tests/test_gemini.py
```

### Comparing `fazah-3.13/Fazah/Fazah.py` & `fazah-3.14/Fazah/Fazah.py`

 * *Files identical despite different names*

### Comparing `fazah-3.13/setup.py` & `fazah-3.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fazah',
-    version='3.13',
+    version='3.14',
     description='A library that enhances the multilingual capabilities of Large Language Models by manipulating model input, allowing responses in all languages to be equally coherent.',
     author='Aiden Lang, Will Foster',
     author_email='ajlang5@wisc.edu, wjfoster2@wisc.edu',
     packages=find_packages(),
     install_requires=[
         'deep_translator',
         'langdetect',
```

### Comparing `fazah-3.13/tests/test.openai.py` & `fazah-3.14/tests/test.openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Fazah import Fazah
+from Fazah.Fazah import Fazah
 from openai import OpenAI
 
 OPENAI_API_KEY = "sk-proj-ggVu1RBhLnYRKdOkYeZNT3BlbkFJTeyJzT4So7GBNBqgIpAU"
 client = OpenAI(api_key=OPENAI_API_KEY)
```

### Comparing `fazah-3.13/tests/test_gemini.py` & `fazah-3.14/tests/test_gemini.py`

 * *Files identical despite different names*

