# Comparing `tmp/PathMePy-0.5.2.tar.gz` & `tmp/PathMePy-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PathMePy-0.5.2.tar", last modified: Sun Apr 14 17:02:29 2024, max compression
+gzip compressed data, was "PathMePy-0.5.3.tar", last modified: Fri May  3 12:09:20 2024, max compression
```

## Comparing `PathMePy-0.5.2.tar` & `PathMePy-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 17:02:29.041976 PathMePy-0.5.2/
--rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-0.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1349 2024-04-14 17:02:29.038977 PathMePy-0.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 17:02:29.001001 PathMePy-0.5.2/PathMePy/
--rw-rw-rw-   0        0        0     1718 2024-04-10 16:49:09.000000 PathMePy-0.5.2/PathMePy/PathMePy.py
--rw-rw-rw-   0        0        0      173 2024-04-14 17:02:00.000000 PathMePy-0.5.2/PathMePy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 17:02:29.035983 PathMePy-0.5.2/PathMePy.egg-info/
--rw-rw-rw-   0        0        0     1349 2024-04-14 17:02:28.000000 PathMePy-0.5.2/PathMePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-14 17:02:28.000000 PathMePy-0.5.2/PathMePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 17:02:28.000000 PathMePy-0.5.2/PathMePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 17:02:28.000000 PathMePy-0.5.2/PathMePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      976 2024-04-14 12:33:38.000000 PathMePy-0.5.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 17:02:29.042976 PathMePy-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1421 2024-04-14 17:02:11.000000 PathMePy-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:09:20.067054 PathMePy-0.5.3/
+-rw-rw-rw-   0        0        0      404 2024-05-03 12:09:20.063145 PathMePy-0.5.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 12:09:20.022137 PathMePy-0.5.3/PathMePy/
+-rw-rw-rw-   0        0        0     1907 2024-05-03 11:59:27.000000 PathMePy-0.5.3/PathMePy/PathMePy.py
+-rw-rw-rw-   0        0        0      173 2024-04-14 17:02:00.000000 PathMePy-0.5.3/PathMePy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 12:09:20.058262 PathMePy-0.5.3/PathMePy.egg-info/
+-rw-rw-rw-   0        0        0      404 2024-05-03 12:09:19.000000 PathMePy-0.5.3/PathMePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-03 12:09:19.000000 PathMePy-0.5.3/PathMePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 12:09:19.000000 PathMePy-0.5.3/PathMePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 12:09:19.000000 PathMePy-0.5.3/PathMePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 12:09:20.067054 PathMePy-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      503 2024-05-03 12:09:09.000000 PathMePy-0.5.3/setup.py
```

### Comparing `PathMePy-0.5.2/PathMePy/PathMePy.py` & `PathMePy-0.5.3/PathMePy/PathMePy.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 def IsAlreadyOnPath(path):
     if path in Current_Path_Formated:
         return True
     else:
         return False
 
 def UserScriptFolderIsAlreadyOnPath():
-    if site.getusersitepackages().replace('site-packages', 'Scripts') in Current_Path_Formated:
+    if platform.system() == "Windows":
+        path = site.getusersitepackages().replace('site-packages', 'Scripts')
+    else:
+        path = "~/.local/bin"
+    if path in Current_Path_Formated:
         return True
     else:
         return False
 
 def PathMePyDir(path):
     path = os.path.abspath(path)
     if not os.path.exists(path):
@@ -35,14 +39,17 @@
         os.system('export PATH=$PATH:' + path)
     elif platform.system() == "Windows" :
         os.system('set Path="%Path%;' + path + '"')
     elif platform.system() == "Linux":
         os.system('export PATH=$PATH:' + path)
 
 def PathMePyUserScriptFolder():
-    path = site.getusersitepackages().replace('site-packages', 'Scripts')
+    if platform.system() == "Windows":
+        path = site.getusersitepackages().replace('site-packages', 'Scripts')
+    else:
+        path = "~/.local/bin"
     if platform.system() != "Windows" and platform.system() != "Linux" :
         os.system('export PATH=$PATH:' + path)
     if platform.system() == "Windows" :
         os.system('set Path="%Path%;' + path + '"')
     elif platform.system() == "Linux":
         os.system('export PATH=$PATH:' + path)
```

