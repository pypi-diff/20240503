# Comparing `tmp/lfg_llama-1.0.6.tar.gz` & `tmp/lfg_llama-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.0.6.tar", last modified: Fri May  3 09:54:18 2024, max compression
+gzip compressed data, was "lfg_llama-1.1.0.tar", last modified: Fri May  3 13:17:32 2024, max compression
```

## Comparing `lfg_llama-1.0.6.tar` & `lfg_llama-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:54:18.431796 lfg_llama-1.0.6/
--rw-r--r--   0 ob907      (502) staff       (20)     1037 2024-05-03 09:54:18.431601 lfg_llama-1.0.6/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      800 2024-05-03 09:50:39.000000 lfg_llama-1.0.6/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:54:18.429909 lfg_llama-1.0.6/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.6/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     1323 2024-05-03 09:54:00.000000 lfg_llama-1.0.6/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:54:18.431262 lfg_llama-1.0.6/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1037 2024-05-03 09:54:18.000000 lfg_llama-1.0.6/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 09:54:18.000000 lfg_llama-1.0.6/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 09:54:18.000000 lfg_llama-1.0.6/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 09:54:18.000000 lfg_llama-1.0.6/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 09:54:18.000000 lfg_llama-1.0.6/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 09:54:18.000000 lfg_llama-1.0.6/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 09:54:18.431955 lfg_llama-1.0.6/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      682 2024-05-03 09:54:15.000000 lfg_llama-1.0.6/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 13:17:32.895158 lfg_llama-1.1.0/
+-rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 13:17:32.894955 lfg_llama-1.1.0/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1030 2024-05-03 10:03:47.000000 lfg_llama-1.1.0/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 13:17:32.893284 lfg_llama-1.1.0/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.1.0/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     1323 2024-05-03 10:00:41.000000 lfg_llama-1.1.0/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 13:17:32.894672 lfg_llama-1.1.0/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1267 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 13:17:32.000000 lfg_llama-1.1.0/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 13:17:32.895227 lfg_llama-1.1.0/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      682 2024-05-03 13:17:31.000000 lfg_llama-1.1.0/setup.py
```

### Comparing `lfg_llama-1.0.6/README.md` & `lfg_llama-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,24 @@
 # restart your terminal
 # install LFG
 pipx install lfg-llama
 ```
 
 ## Usage
 
+This executable is using Groq, that means you need and [API token](https://console.groq.com/keys).
+
+Add the token to your .bashrc/.zshrc and reload your terminal.
+
+```
+export GROQ_API_KEY=1337
+```
+
+Now you can use the executable
+
 ```bash
 lfg kill port 3000
 
 # Kill process listening on port 3000
 lsof -i :3000 | xargs kill
 
 ```
```

### Comparing `lfg_llama-1.0.6/lfg/cli.py` & `lfg_llama-1.1.0/lfg/cli.py`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.0.6/setup.py` & `lfg_llama-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         install_requires = map(lambda s: s.strip(), req_txt.readlines()[2:])
 
     return list(install_requires)
 
 
 setup(
     name="lfg-llama",
-    version="1.0.6",
+    version="1.1.0",
     description="LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bjarne Oeverli",
     author_email="bjarneocodes@gmail.com",
     packages=find_packages(),
     install_requires=["groq"],
```

