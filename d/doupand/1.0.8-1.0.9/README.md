# Comparing `tmp/doupand-1.0.8.tar.gz` & `tmp/doupand-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doupand-1.0.8.tar", last modified: Fri Apr 26 14:56:54 2024, max compression
+gzip compressed data, was "doupand-1.0.9.tar", last modified: Fri May  3 14:52:49 2024, max compression
```

## Comparing `doupand-1.0.8.tar` & `doupand-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:56:54.403118 doupand-1.0.8/
--rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.8/LICENSE
--rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-04-26 14:56:54.402933 doupand-1.0.8/PKG-INFO
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:56:54.400290 doupand-1.0.8/doupand/
--rw-r--r--   0 tongjun    (501) staff       (20)      134 2024-04-26 14:56:51.000000 doupand-1.0.8/doupand/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:56:54.401694 doupand-1.0.8/doupand/api/
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.8/doupand/api/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)     3413 2024-04-26 14:47:06.000000 doupand-1.0.8/doupand/api/client.py
--rw-r--r--   0 tongjun    (501) staff       (20)       54 2024-04-26 14:44:18.000000 doupand-1.0.8/doupand/api/dp_url.csv
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:56:54.402592 doupand-1.0.8/doupand/utils/
--rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.8/doupand/utils/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.8/doupand/utils/cons.py
--rw-r--r--   0 tongjun    (501) staff       (20)       71 2024-04-26 14:52:16.000000 doupand-1.0.8/doupand/utils/dp_tk.csv
--rw-r--r--   0 tongjun    (501) staff       (20)      701 2024-04-26 14:54:25.000000 doupand-1.0.8/doupand/utils/userauth.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-04-26 14:56:54.400942 doupand-1.0.8/doupand.egg-info/
--rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-04-26 14:56:54.000000 doupand-1.0.8/doupand.egg-info/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)      357 2024-04-26 14:56:54.000000 doupand-1.0.8/doupand.egg-info/SOURCES.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2024-04-26 14:56:54.000000 doupand-1.0.8/doupand.egg-info/dependency_links.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       16 2024-04-26 14:56:54.000000 doupand-1.0.8/doupand.egg-info/requires.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        8 2024-04-26 14:56:54.000000 doupand-1.0.8/doupand.egg-info/top_level.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       38 2024-04-26 14:56:54.403168 doupand-1.0.8/setup.cfg
--rw-r--r--   0 tongjun    (501) staff       (20)     2400 2024-04-26 14:56:51.000000 doupand-1.0.8/setup.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.518100 doupand-1.0.9/
+-rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.9/LICENSE
+-rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-05-03 14:52:49.517936 doupand-1.0.9/PKG-INFO
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.515765 doupand-1.0.9/doupand/
+-rw-r--r--   0 tongjun    (501) staff       (20)      134 2024-05-03 14:50:41.000000 doupand-1.0.9/doupand/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.517085 doupand-1.0.9/doupand/api/
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.9/doupand/api/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)     3362 2024-05-03 14:50:41.000000 doupand-1.0.9/doupand/api/client.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.517603 doupand-1.0.9/doupand/utils/
+-rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.9/doupand/utils/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.9/doupand/utils/cons.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      701 2024-04-26 14:54:25.000000 doupand-1.0.9/doupand/utils/userauth.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2024-05-03 14:52:49.516677 doupand-1.0.9/doupand.egg-info/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2039 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)      310 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/SOURCES.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/dependency_links.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       16 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/requires.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        8 2024-05-03 14:52:49.000000 doupand-1.0.9/doupand.egg-info/top_level.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       38 2024-05-03 14:52:49.518152 doupand-1.0.9/setup.cfg
+-rw-r--r--   0 tongjun    (501) staff       (20)     2400 2024-05-03 14:52:30.000000 doupand-1.0.9/setup.py
```

### Comparing `doupand-1.0.8/LICENSE` & `doupand-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `doupand-1.0.8/PKG-INFO` & `doupand-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.8/doupand/api/client.py` & `doupand-1.0.9/doupand/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 __all__ = ['data_reader']
 
 
 class DataReader:
     __token = ''
     __http_url = ''
-    # __distribution_url = 'http://api.doupand.com'
-    __distribution_url = 'http://127.0.0.1:7001'
+    __distribution_url = 'http://api.doupand.com'
 
     def __init__(self, token='', timeout=15):
         """
         :param token: API的TOKEN，用于用户认证
         :param timeout:
         """
         self.__token = token
```

### Comparing `doupand-1.0.8/doupand/utils/userauth.py` & `doupand-1.0.9/doupand/utils/userauth.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.8/doupand.egg-info/PKG-INFO` & `doupand-1.0.9/doupand.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.8/setup.py` & `doupand-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
 """
 
 setup(
     name='doupand',
-    version="1.0.8",
+    version="1.0.9",
     description='A simple and easy-to-use financial data interface library built for normal investors!',
     long_description=long_desc,
     author='DouBro',
     author_email='doupand@163.com',
     packages=find_packages(),
     platforms=["all"],
     license='BSD',
```

