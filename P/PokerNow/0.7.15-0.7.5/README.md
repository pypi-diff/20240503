# Comparing `tmp/pokernow-0.7.15.tar.gz` & `tmp/pokernow-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.7.15.tar", last modified: Fri May  3 00:41:35 2024, max compression
+gzip compressed data, was "pokernow-0.7.5.tar", last modified: Fri May  3 00:40:59 2024, max compression
```

## Comparing `pokernow-0.7.15.tar` & `pokernow-0.7.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:41:35.357155 pokernow-0.7.15/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.7.15/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.7.15/MANIFEST.in
--rw-rw-rw-   0        0        0    10070 2024-05-03 00:41:35.356303 pokernow-0.7.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 00:41:35.340944 pokernow-0.7.15/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.7.15/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      750 2024-05-03 00:38:17.000000 pokernow-0.7.15/PokerNow/client.py
--rw-rw-rw-   0        0        0    16335 2024-05-03 00:40:04.000000 pokernow-0.7.15/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.7.15/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:41:35.354517 pokernow-0.7.15/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10070 2024-05-03 00:41:35.000000 pokernow-0.7.15/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-03 00:41:35.000000 pokernow-0.7.15/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:41:35.000000 pokernow-0.7.15/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:41:35.000000 pokernow-0.7.15/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:41:35.000000 pokernow-0.7.15/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.7.15/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 00:41:35.357155 pokernow-0.7.15/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-05-03 00:41:31.000000 pokernow-0.7.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:40:59.426710 pokernow-0.7.5/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    10069 2024-05-03 00:40:59.425712 pokernow-0.7.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 00:40:59.411119 pokernow-0.7.5/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.7.5/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      750 2024-05-03 00:38:17.000000 pokernow-0.7.5/PokerNow/client.py
+-rw-rw-rw-   0        0        0    16335 2024-05-03 00:40:04.000000 pokernow-0.7.5/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.7.5/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:40:59.424713 pokernow-0.7.5/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10069 2024-05-03 00:40:59.000000 pokernow-0.7.5/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-03 00:40:59.000000 pokernow-0.7.5/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 00:40:59.000000 pokernow-0.7.5/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:40:59.000000 pokernow-0.7.5/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:40:59.000000 pokernow-0.7.5/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.7.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 00:40:59.427706 pokernow-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-05-03 00:40:54.000000 pokernow-0.7.5/setup.py
```

### Comparing `pokernow-0.7.15/LICENSE` & `pokernow-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.15/PKG-INFO` & `pokernow-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.7.15
+Version: 0.7.5
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.7.15/PokerNow/client.py` & `pokernow-0.7.5/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.15/PokerNow/managers.py` & `pokernow-0.7.5/PokerNow/managers.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.15/PokerNow/models.py` & `pokernow-0.7.5/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.15/PokerNow.egg-info/PKG-INFO` & `pokernow-0.7.5/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.7.15
+Version: 0.7.5
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.7.15/README.md` & `pokernow-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.15/setup.py` & `pokernow-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.7.15',
+    version='0.7.05',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

