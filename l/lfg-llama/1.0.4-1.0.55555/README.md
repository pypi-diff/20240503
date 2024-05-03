# Comparing `tmp/lfg_llama-1.0.4.tar.gz` & `tmp/lfg_llama-1.0.55555.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.0.4.tar", last modified: Fri May  3 09:50:52 2024, max compression
+gzip compressed data, was "lfg_llama-1.0.55555.tar", last modified: Fri May  3 09:52:35 2024, max compression
```

## Comparing `lfg_llama-1.0.4.tar` & `lfg_llama-1.0.55555.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:50:52.929122 lfg_llama-1.0.4/
--rw-r--r--   0 ob907      (502) staff       (20)     1037 2024-05-03 09:50:52.928921 lfg_llama-1.0.4/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      800 2024-05-03 09:50:39.000000 lfg_llama-1.0.4/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:50:52.926981 lfg_llama-1.0.4/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.4/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     1341 2024-05-03 09:49:44.000000 lfg_llama-1.0.4/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:50:52.928642 lfg_llama-1.0.4/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1037 2024-05-03 09:50:52.000000 lfg_llama-1.0.4/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 09:50:52.000000 lfg_llama-1.0.4/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 09:50:52.000000 lfg_llama-1.0.4/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 09:50:52.000000 lfg_llama-1.0.4/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 09:50:52.000000 lfg_llama-1.0.4/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 09:50:52.000000 lfg_llama-1.0.4/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 09:50:52.929194 lfg_llama-1.0.4/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      682 2024-05-03 09:50:01.000000 lfg_llama-1.0.4/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:52:35.025997 lfg_llama-1.0.55555/
+-rw-r--r--   0 ob907      (502) staff       (20)     1041 2024-05-03 09:52:35.025784 lfg_llama-1.0.55555/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      800 2024-05-03 09:50:39.000000 lfg_llama-1.0.55555/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:52:35.024502 lfg_llama-1.0.55555/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.55555/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     1268 2024-05-03 09:51:31.000000 lfg_llama-1.0.55555/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-03 09:52:35.025543 lfg_llama-1.0.55555/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1041 2024-05-03 09:52:34.000000 lfg_llama-1.0.55555/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-03 09:52:35.000000 lfg_llama-1.0.55555/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-03 09:52:34.000000 lfg_llama-1.0.55555/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-03 09:52:34.000000 lfg_llama-1.0.55555/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-03 09:52:34.000000 lfg_llama-1.0.55555/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-03 09:52:34.000000 lfg_llama-1.0.55555/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-03 09:52:35.026049 lfg_llama-1.0.55555/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      686 2024-05-03 09:52:29.000000 lfg_llama-1.0.55555/setup.py
```

### Comparing `lfg_llama-1.0.4/PKG-INFO` & `lfg_llama-1.0.55555/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.0.4
+Version: 1.0.55555
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

### Comparing `lfg_llama-1.0.4/README.md` & `lfg_llama-1.0.55555/README.md`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.0.4/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.0.55555/lfg_llama.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.0.4
+Version: 1.0.55555
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

### Comparing `lfg_llama-1.0.4/setup.py` & `lfg_llama-1.0.55555/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         install_requires = map(lambda s: s.strip(), req_txt.readlines()[2:])
 
     return list(install_requires)
 
 
 setup(
     name="lfg-llama",
-    version="1.0.4",
+    version="1.0.55555",
     description="LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bjarne Oeverli",
     author_email="bjarneocodes@gmail.com",
     packages=find_packages(),
     install_requires=["groq"],
```

