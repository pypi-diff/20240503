# Comparing `tmp/lfg_llama-1.1.1.tar.gz` & `tmp/lfg_llama-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.1.1.tar", last modified: Fri May  3 14:13:44 2024, max compression
+gzip compressed data, was "lfg_llama-1.1.2.tar", last modified: Fri May  3 14:24:42 2024, max compression
```

## Comparing `lfg_llama-1.1.1.tar` & `lfg_llama-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:13:44.219226 lfg_llama-1.1.1/
--rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 14:13:44.219022 lfg_llama-1.1.1/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1030 2024-05-03 10:03:47.000000 lfg_llama-1.1.1/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:13:44.217534 lfg_llama-1.1.1/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.1/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2173 2024-05-03 14:13:28.000000 lfg_llama-1.1.1/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:13:44.218791 lfg_llama-1.1.1/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 14:13:44.000000 lfg_llama-1.1.1/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 14:13:44.219274 lfg_llama-1.1.1/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-03 14:13:41.000000 lfg_llama-1.1.1/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:24:42.195031 lfg_llama-1.1.2/
+-rw-r--r--   0 ob907      (502) staff       (20)     1217 2024-05-03 14:24:42.194802 lfg_llama-1.1.2/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      980 2024-05-03 14:24:05.000000 lfg_llama-1.1.2/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:24:42.193287 lfg_llama-1.1.2/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.2/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     2173 2024-05-03 14:13:28.000000 lfg_llama-1.1.2/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 14:24:42.194557 lfg_llama-1.1.2/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1217 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 14:24:42.000000 lfg_llama-1.1.2/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 14:24:42.195089 lfg_llama-1.1.2/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-03 14:24:38.000000 lfg_llama-1.1.2/setup.py
```

### Comparing `lfg_llama-1.1.1/PKG-INFO` & `lfg_llama-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.1.1
+Version: 1.1.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
-![Logo](./logo.png)
+![Demo](example.gif)
 
 LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. It taps into the vast knowledge of the LLAMA3 language model (via Ollama) to understand your natural language descriptions and provide you with the most relevant commands and explanations.
 
 ## Installation
 
 ```bash
 # install pipx
@@ -52,11 +52,7 @@
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.7
 pipenv install
 ```
-
-### TODO
-
-- Use the model directly without ollama
```

### Comparing `lfg_llama-1.1.1/README.md` & `lfg_llama-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
-![Logo](./logo.png)
+![Demo](example.gif)
 
 LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. It taps into the vast knowledge of the LLAMA3 language model (via Ollama) to understand your natural language descriptions and provide you with the most relevant commands and explanations.
 
 ## Installation
 
 ```bash
 # install pipx
@@ -43,11 +43,7 @@
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.7
 pipenv install
 ```
-
-### TODO
-
-- Use the model directly without ollama
```

### Comparing `lfg_llama-1.1.1/lfg/cli.py` & `lfg_llama-1.1.2/lfg/cli.py`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.1.1/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.1.2/lfg_llama.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.1.1
+Version: 1.1.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
-![Logo](./logo.png)
+![Demo](example.gif)
 
 LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. It taps into the vast knowledge of the LLAMA3 language model (via Ollama) to understand your natural language descriptions and provide you with the most relevant commands and explanations.
 
 ## Installation
 
 ```bash
 # install pipx
@@ -52,11 +52,7 @@
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.7
 pipenv install
 ```
-
-### TODO
-
-- Use the model directly without ollama
```

