# Comparing `tmp/hrbdataproject-2.0.tar.gz` & `tmp/hrbdataproject-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbdataproject-2.0.tar", last modified: Fri May  3 15:45:51 2024, max compression
+gzip compressed data, was "hrbdataproject-2.1.tar", last modified: Fri May  3 15:53:27 2024, max compression
```

## Comparing `hrbdataproject-2.0.tar` & `hrbdataproject-2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:45:51.342197 hrbdataproject-2.0/
--rw-rw-rw-   0        0        0      385 2024-05-03 15:45:51.342197 hrbdataproject-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 15:45:51.333358 hrbdataproject-2.0/hrbdataproject/
--rw-rw-rw-   0        0        0      125 2024-05-03 09:51:07.000000 hrbdataproject-2.0/hrbdataproject/__init__.py
--rw-rw-rw-   0        0        0     7267 2024-05-03 15:43:43.000000 hrbdataproject-2.0/hrbdataproject/data_quality_checks.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:45:51.340490 hrbdataproject-2.0/hrbdataproject.egg-info/
--rw-rw-rw-   0        0        0      385 2024-05-03 15:45:51.000000 hrbdataproject-2.0/hrbdataproject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-03 15:45:51.000000 hrbdataproject-2.0/hrbdataproject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:45:51.000000 hrbdataproject-2.0/hrbdataproject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-03 15:45:51.000000 hrbdataproject-2.0/hrbdataproject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 15:45:51.344677 hrbdataproject-2.0/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-03 15:44:00.000000 hrbdataproject-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:53:27.591410 hrbdataproject-2.1/
+-rw-rw-rw-   0        0        0      367 2024-05-03 15:53:27.591410 hrbdataproject-2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 15:53:27.591410 hrbdataproject-2.1/hrbdataproject/
+-rw-rw-rw-   0        0        0      125 2024-05-03 09:51:07.000000 hrbdataproject-2.1/hrbdataproject/__init__.py
+-rw-rw-rw-   0        0        0     7267 2024-05-03 15:43:43.000000 hrbdataproject-2.1/hrbdataproject/data_quality_checks.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:53:27.591410 hrbdataproject-2.1/hrbdataproject.egg-info/
+-rw-rw-rw-   0        0        0      367 2024-05-03 15:53:27.000000 hrbdataproject-2.1/hrbdataproject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-03 15:53:27.000000 hrbdataproject-2.1/hrbdataproject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:53:27.000000 hrbdataproject-2.1/hrbdataproject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 15:53:27.000000 hrbdataproject-2.1/hrbdataproject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:53:27.591410 hrbdataproject-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      581 2024-05-03 15:53:23.000000 hrbdataproject-2.1/setup.py
```

### Comparing `hrbdataproject-2.0/hrbdataproject/data_quality_checks.py` & `hrbdataproject-2.1/hrbdataproject/data_quality_checks.py`

 * *Files identical despite different names*

### Comparing `hrbdataproject-2.0/setup.py` & `hrbdataproject-2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hrbdataproject',
-    version='2.0',
+    version='2.1',
     packages=find_packages(),
     #py_modules=['data_quality_checks'],  # Specify the individual Python file here
     description='A library for data quality checks in Databricks notebooks',
     author='Harun Raseed Basheer',
     author_email='harun.raseed093@gmail.com',
-    url='https://github.com/harun_raseed_basheer/my_data_quality_library',
+    url='https://github.com/harunraseed/hrbdataproject',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
 )
```

