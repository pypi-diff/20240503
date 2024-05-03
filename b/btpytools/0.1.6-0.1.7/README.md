# Comparing `tmp/btpytools-0.1.6.tar.gz` & `tmp/btpytools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btpytools-0.1.6.tar", last modified: Thu Jan  6 14:36:11 2022, max compression
+gzip compressed data, was "btpytools-0.1.7.tar", last modified: Thu Jan  6 14:44:53 2022, max compression
```

## Comparing `btpytools-0.1.6.tar` & `btpytools-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-06 14:36:11.132627 btpytools-0.1.6/
--rw-rw-r--   0 rob       (1000) rob       (1000)    34523 2021-06-23 14:50:37.000000 btpytools-0.1.6/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)     3152 2022-01-06 14:36:11.132627 btpytools-0.1.6/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     1908 2021-06-24 14:33:27.000000 btpytools-0.1.6/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-06 14:36:11.132627 btpytools-0.1.6/btpytools/
--rw-rw-r--   0 rob       (1000) rob       (1000)       50 2022-01-06 14:35:07.000000 btpytools-0.1.6/btpytools/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)      673 2022-01-06 13:30:41.000000 btpytools-0.1.6/btpytools/brainreg_bt.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     6492 2022-01-06 13:30:41.000000 btpytools-0.1.6/btpytools/compressRawData.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     1517 2022-01-06 13:30:41.000000 btpytools-0.1.6/btpytools/recipe.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)      801 2022-01-06 13:30:41.000000 btpytools-0.1.6/btpytools/summariseAcquisitions.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)     8456 2022-01-06 13:30:41.000000 btpytools-0.1.6/btpytools/tools.py
--rwxrwxr-x   0 rob       (1000) rob       (1000)    10387 2022-01-06 14:36:10.000000 btpytools-0.1.6/btpytools/transferToServer.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-06 14:36:11.132627 btpytools-0.1.6/btpytools.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)        2 2021-06-24 14:04:23.000000 btpytools-0.1.6/btpytools.egg-info/.gitignore
--rw-r--r--   0 rob       (1000) rob       (1000)     3152 2022-01-06 14:36:11.000000 btpytools-0.1.6/btpytools.egg-info/PKG-INFO
--rw-r--r--   0 rob       (1000) rob       (1000)      446 2022-01-06 14:36:11.000000 btpytools-0.1.6/btpytools.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-01-06 14:36:11.000000 btpytools-0.1.6/btpytools.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)      172 2022-01-06 14:36:11.000000 btpytools-0.1.6/btpytools.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        7 2022-01-06 14:36:11.000000 btpytools-0.1.6/btpytools.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       10 2022-01-06 14:36:11.000000 btpytools-0.1.6/btpytools.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)     1093 2022-01-06 14:36:11.132627 btpytools-0.1.6/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)      115 2021-06-24 13:12:55.000000 btpytools-0.1.6/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-06 14:44:53.896511 btpytools-0.1.7/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    34523 2021-06-23 14:50:37.000000 btpytools-0.1.7/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)     3152 2022-01-06 14:44:53.896511 btpytools-0.1.7/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1908 2021-06-24 14:33:27.000000 btpytools-0.1.7/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-06 14:44:53.896511 btpytools-0.1.7/btpytools/
+-rw-rw-r--   0 rob       (1000) rob       (1000)       50 2022-01-06 14:44:01.000000 btpytools-0.1.7/btpytools/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)      673 2022-01-06 13:30:41.000000 btpytools-0.1.7/btpytools/brainreg_bt.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     6492 2022-01-06 13:30:41.000000 btpytools-0.1.7/btpytools/compressRawData.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1517 2022-01-06 13:30:41.000000 btpytools-0.1.7/btpytools/recipe.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)      801 2022-01-06 13:30:41.000000 btpytools-0.1.7/btpytools/summariseAcquisitions.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)     8456 2022-01-06 13:30:41.000000 btpytools-0.1.7/btpytools/tools.py
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    10387 2022-01-06 14:43:24.000000 btpytools-0.1.7/btpytools/transferToServer.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-01-06 14:44:53.896511 btpytools-0.1.7/btpytools.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)        2 2021-06-24 14:04:23.000000 btpytools-0.1.7/btpytools.egg-info/.gitignore
+-rw-r--r--   0 rob       (1000) rob       (1000)     3152 2022-01-06 14:44:53.000000 btpytools-0.1.7/btpytools.egg-info/PKG-INFO
+-rw-r--r--   0 rob       (1000) rob       (1000)      446 2022-01-06 14:44:53.000000 btpytools-0.1.7/btpytools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-01-06 14:44:53.000000 btpytools-0.1.7/btpytools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)      172 2022-01-06 14:44:53.000000 btpytools-0.1.7/btpytools.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        7 2022-01-06 14:44:53.000000 btpytools-0.1.7/btpytools.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       10 2022-01-06 14:44:53.000000 btpytools-0.1.7/btpytools.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1093 2022-01-06 14:44:53.896511 btpytools-0.1.7/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)      115 2021-06-24 13:12:55.000000 btpytools-0.1.7/setup.py
```

### Comparing `btpytools-0.1.6/LICENSE` & `btpytools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/PKG-INFO` & `btpytools-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btpytools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Helper functions for BakingTray and StitchIt
 Home-page: https://github.com/SainsburyWellcomeCentre/btpytools
 Author: Rob Campbell
 Author-email: rob.campbell@ucl.ac.uk
 License: UNKNOWN
 Project-URL: Source, https://bakingtray.mouse.vision
 Description: # StitchIt Python Tools
```

### Comparing `btpytools-0.1.6/README.md` & `btpytools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/btpytools/brainreg_bt.py` & `btpytools-0.1.7/btpytools/brainreg_bt.py`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/btpytools/compressRawData.py` & `btpytools-0.1.7/btpytools/compressRawData.py`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/btpytools/recipe.py` & `btpytools-0.1.7/btpytools/recipe.py`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/btpytools/summariseAcquisitions.py` & `btpytools-0.1.7/btpytools/summariseAcquisitions.py`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/btpytools/tools.py` & `btpytools-0.1.7/btpytools/tools.py`

 * *Files identical despite different names*

### Comparing `btpytools-0.1.6/btpytools/transferToServer.py` & `btpytools-0.1.7/btpytools/transferToServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     if not main_rsync_switch.startswith("-"):
         main_rsync_switch = "-%s" % main_rsync_switch
 
     # Append "n" for dry-run rsync mode if the user asked for this with the -s flag at CLI
     if args.simulate:
         main_rsync_switch += "n"
 
-    source_dirs = args.paths[1:-1]  # One or more files or folders to copy
+    source_dirs = args.paths[0:-1]  # One or more files or folders to copy
     destination_dir = args.paths[-1]  # Where we will copy to
 
     # Bail out if any of the supplied paths do not exist
     if check_directories(source_dirs, destination_dir):
         exit()
 
     # Remove trailing slash from data directories that don't contain data sub-directories
```

### Comparing `btpytools-0.1.6/btpytools.egg-info/PKG-INFO` & `btpytools-0.1.7/btpytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btpytools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Helper functions for BakingTray and StitchIt
 Home-page: https://github.com/SainsburyWellcomeCentre/btpytools
 Author: Rob Campbell
 Author-email: rob.campbell@ucl.ac.uk
 License: UNKNOWN
 Project-URL: Source, https://bakingtray.mouse.vision
 Description: # StitchIt Python Tools
```

### Comparing `btpytools-0.1.6/setup.cfg` & `btpytools-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_file = LICENSE
 name = btpytools
-version = 0.1.6
+version = 0.1.7
 author = Rob Campbell
 author_email = rob.campbell@ucl.ac.uk
 description = Helper functions for BakingTray and StitchIt
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/SainsburyWellcomeCentre/btpytools
 project_urls =
```

