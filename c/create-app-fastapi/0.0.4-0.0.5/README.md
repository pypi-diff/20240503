# Comparing `tmp/create-app-fastapi-0.0.4.tar.gz` & `tmp/create-app-fastapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-app-fastapi-0.0.4.tar", last modified: Mon Apr 29 12:17:13 2024, max compression
+gzip compressed data, was "create-app-fastapi-0.0.5.tar", last modified: Fri May  3 09:16:31 2024, max compression
```

## Comparing `create-app-fastapi-0.0.4.tar` & `create-app-fastapi-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      599 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/PKG-INFO
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      599 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/PKG-INFO
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/entry_points.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-04-29 12:17:13.000000 create-app-fastapi-0.0.4/create_app_fastapi.egg-info/top_level.txt
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/projectfastapi/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.4/projectfastapi/__init__.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     3973 2024-04-29 12:17:04.000000 create-app-fastapi-0.0.4/projectfastapi/main.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     2202 2024-04-26 13:06:58.000000 create-app-fastapi-0.0.4/projectfastapi/source.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-04-29 12:17:13.268347 create-app-fastapi-0.0.4/setup.cfg
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      807 2024-04-29 12:17:00.000000 create-app-fastapi-0.0.4/setup.py
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-03 09:16:31.092927 create-app-fastapi-0.0.5/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      673 2024-05-03 09:16:31.092927 create-app-fastapi-0.0.5/PKG-INFO
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-03 09:16:31.092927 create-app-fastapi-0.0.5/create_app_fastapi.egg-info/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      673 2024-05-03 09:16:31.000000 create-app-fastapi-0.0.5/create_app_fastapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-05-03 09:16:31.000000 create-app-fastapi-0.0.5/create_app_fastapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-05-03 09:16:31.000000 create-app-fastapi-0.0.5/create_app_fastapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-05-03 09:16:31.000000 create-app-fastapi-0.0.5/create_app_fastapi.egg-info/entry_points.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-05-03 09:16:31.000000 create-app-fastapi-0.0.5/create_app_fastapi.egg-info/top_level.txt
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-03 09:16:31.092927 create-app-fastapi-0.0.5/projectfastapi/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.5/projectfastapi/__init__.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     3976 2024-05-03 09:15:32.000000 create-app-fastapi-0.0.5/projectfastapi/main.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     2202 2024-04-26 13:06:58.000000 create-app-fastapi-0.0.5/projectfastapi/source.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-05-03 09:16:31.092927 create-app-fastapi-0.0.5/setup.cfg
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      900 2024-05-03 09:14:12.000000 create-app-fastapi-0.0.5/setup.py
```

### Comparing `create-app-fastapi-0.0.4/projectfastapi/main.py` & `create-app-fastapi-0.0.5/projectfastapi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .source import getFileData
 
 def main():
 
     parser = argparse.ArgumentParser(prog ='create-app-fastapi', description="Create fastapi project") 
     parser.add_argument('name', metavar ='NAME', type = str, help ='create a project in this name')
     parser.add_argument('-v','--version',action='version',
-                    version='%(prog)s 0.0.4', help ="show program's version number and exit")
+                    version='%(prog)s 0.0.5', help ="show program's version number and exit")
     args = parser.parse_args()
 
     curdir= os.getcwd()
     platformOS= platform.system()
     threadStop= False
 
     # terminal color code
@@ -111,9 +111,8 @@
     Note: activate virtual environment before run source {GREEN}main.py{RESET}
     {GREEN}Have a nice day! {RESET}
     """)
 
     openvs= input("Open project in VS Code? (y/n): ")
     if openvs.lower() == 'y':
         run("code .")
-
-main()
+    return
```

### Comparing `create-app-fastapi-0.0.4/projectfastapi/source.py` & `create-app-fastapi-0.0.5/projectfastapi/source.py`

 * *Files identical despite different names*

