# Comparing `tmp/flatpack-3.4.7.tar.gz` & `tmp/flatpack-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.7.tar", last modified: Thu May  2 14:43:57 2024, max compression
+gzip compressed data, was "flatpack-3.4.8.tar", last modified: Thu May  2 14:59:36 2024, max compression
```

## Comparing `flatpack-3.4.7.tar` & `flatpack-3.4.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.305091 flatpack-3.4.7/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.7/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:43:57.304801 flatpack-3.4.7/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.7/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.301780 flatpack-3.4.7/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.7/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.7/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.303219 flatpack-3.4.7/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.7/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.7/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.7/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-02 14:38:54.000000 flatpack-3.4.7/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26234 2024-05-02 10:00:01.000000 flatpack-3.4.7/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.304016 flatpack-3.4.7/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.7/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.7/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.7/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.7/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:43:57.304406 flatpack-3.4.7/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 14:43:57.000000 flatpack-3.4.7/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 14:43:57.305164 flatpack-3.4.7/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 14:31:49.000000 flatpack-3.4.7/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.216545 flatpack-3.4.8/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.8/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:59:36.216280 flatpack-3.4.8/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.8/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.213283 flatpack-3.4.8/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.8/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.8/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.214770 flatpack-3.4.8/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.8/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.8/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.8/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-02 14:38:54.000000 flatpack-3.4.8/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26624 2024-05-02 14:58:46.000000 flatpack-3.4.8/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.215589 flatpack-3.4.8/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.8/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.8/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.8/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.8/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 14:59:36.215935 flatpack-3.4.8/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 14:59:36.000000 flatpack-3.4.8/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 14:59:36.216601 flatpack-3.4.8/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 14:56:51.000000 flatpack-3.4.8/setup.py
```

### Comparing `flatpack-3.4.7/LICENSE` & `flatpack-3.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/PKG-INFO` & `flatpack-3.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.7
+Version: 3.4.8
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.7/README.md` & `flatpack-3.4.8/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/agent_manager.py` & `flatpack-3.4.8/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/datasets.py` & `flatpack-3.4.8/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.4.8/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/instructions.py` & `flatpack-3.4.8/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/main.py` & `flatpack-3.4.8/flatpack/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -633,18 +633,32 @@
 
 def fpk_cli_handle_unbox(args, session):
     if not args.input:
         print("❌ Please specify a flatpack for the unbox command.")
         return
 
     directory_name = args.input
-    if not args.local and directory_name not in fpk_fetch_github_dirs(session):
+    existing_dirs = fpk_fetch_github_dirs(session)
+
+    if directory_name not in existing_dirs:
         print(f"❌ The flatpack '{directory_name}' does not exist.")
         return
 
+    fpk_display_disclaimer(directory_name)
+
+    while True:
+        user_response = input().strip().upper()
+        if user_response == "YES":
+            break
+        elif user_response == "NO":
+            print("❌ Installation aborted by user.")
+            return
+        else:
+            print("❌ Invalid input. Please type 'YES' to accept or 'NO' to decline.")
+
     if args.local:
         local_directory_path = Path(directory_name)
         if not local_directory_path.exists() or not local_directory_path.is_dir():
             print(f"❌ Local directory does not exist: '{directory_name}'.")
             return
         toml_path = local_directory_path / 'flatpack.toml'
         if not toml_path.exists():
```

### Comparing `flatpack-3.4.7/flatpack/modules/lstm.py` & `flatpack-3.4.8/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/modules/rnn.py` & `flatpack-3.4.8/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/parsers.py` & `flatpack-3.4.8/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack/vector_manager.py` & `flatpack-3.4.8/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.8/flatpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.7
+Version: 3.4.8
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.4.7/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.8/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.7/setup.py` & `flatpack-3.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.7",
+    version="3.4.8",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
```

