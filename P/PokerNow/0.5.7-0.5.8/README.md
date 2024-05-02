# Comparing `tmp/pokernow-0.5.7.tar.gz` & `tmp/pokernow-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.5.7.tar", last modified: Thu May  2 23:45:47 2024, max compression
+gzip compressed data, was "pokernow-0.5.8.tar", last modified: Thu May  2 23:52:29 2024, max compression
```

## Comparing `pokernow-0.5.7.tar` & `pokernow-0.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 23:45:47.808909 pokernow-0.5.7/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.5.7/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0    10069 2024-05-02 23:45:47.807912 pokernow-0.5.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 23:45:47.796743 pokernow-0.5.7/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.5.7/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.5.7/PokerNow/client.py
--rw-rw-rw-   0        0        0     9511 2024-05-02 23:45:24.000000 pokernow-0.5.7/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.5.7/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-02 23:45:47.806902 pokernow-0.5.7/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10069 2024-05-02 23:45:47.000000 pokernow-0.5.7/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-02 23:45:47.000000 pokernow-0.5.7/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 23:45:47.000000 pokernow-0.5.7/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 23:45:47.000000 pokernow-0.5.7/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 23:45:47.000000 pokernow-0.5.7/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.5.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 23:45:47.808909 pokernow-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-05-02 23:45:36.000000 pokernow-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:52:29.229354 pokernow-0.5.8/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.5.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    10069 2024-05-02 23:52:29.228357 pokernow-0.5.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 23:52:29.217607 pokernow-0.5.8/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.5.8/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.5.8/PokerNow/client.py
+-rw-rw-rw-   0        0        0     9570 2024-05-02 23:52:04.000000 pokernow-0.5.8/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.5.8/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:52:29.228357 pokernow-0.5.8/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10069 2024-05-02 23:52:29.000000 pokernow-0.5.8/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-02 23:52:29.000000 pokernow-0.5.8/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 23:52:29.000000 pokernow-0.5.8/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 23:52:29.000000 pokernow-0.5.8/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 23:52:29.000000 pokernow-0.5.8/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 23:52:29.229354 pokernow-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-02 23:52:20.000000 pokernow-0.5.8/setup.py
```

### Comparing `pokernow-0.5.7/LICENSE` & `pokernow-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.7/PKG-INFO` & `pokernow-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.5.7
+Version: 0.5.8
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.5.7/PokerNow/client.py` & `pokernow-0.5.8/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.7/PokerNow/managers.py` & `pokernow-0.5.8/PokerNow/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,18 @@
             self.driver.find_element(By.CSS_SELECTOR, selector)
             return True
         except NoSuchElementException:
             return False
 
     def get_text(self, selector, context=None):
         try:
-            element = context.find_element(By.CSS_SELECTOR, selector) if context else self.driver.find_element(By.CSS_SELECTOR, selector)
+            if context:
+                element = context.find_element(By.CSS_SELECTOR, selector)
+            else:
+                element = self.driver.find_element(By.CSS_SELECTOR, selector)
             return element.text.strip()
         except NoSuchElementException:
             return ""
 
     def get_element(self, selector):
         try:
             return self.driver.find_element(By.CSS_SELECTOR, selector)
```

### Comparing `pokernow-0.5.7/PokerNow/models.py` & `pokernow-0.5.8/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.7/PokerNow.egg-info/PKG-INFO` & `pokernow-0.5.8/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.5.7
+Version: 0.5.8
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.5.7/README.md` & `pokernow-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.7/setup.py` & `pokernow-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.5.7',
+    version='0.5.8',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

