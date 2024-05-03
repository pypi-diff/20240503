# Comparing `tmp/pokernow-0.6.45.tar.gz` & `tmp/pokernow-0.6.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.6.45.tar", last modified: Fri May  3 00:18:23 2024, max compression
+gzip compressed data, was "pokernow-0.6.55.tar", last modified: Fri May  3 00:20:18 2024, max compression
```

## Comparing `pokernow-0.6.45.tar` & `pokernow-0.6.55.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:18:23.083037 pokernow-0.6.45/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.6.45/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.6.45/MANIFEST.in
--rw-rw-rw-   0        0        0    10070 2024-05-03 00:18:23.082038 pokernow-0.6.45/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 00:18:23.066766 pokernow-0.6.45/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.6.45/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.6.45/PokerNow/client.py
--rw-rw-rw-   0        0        0     9727 2024-05-03 00:17:28.000000 pokernow-0.6.45/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.6.45/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:18:23.080528 pokernow-0.6.45/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10070 2024-05-03 00:18:22.000000 pokernow-0.6.45/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-03 00:18:23.000000 pokernow-0.6.45/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:18:22.000000 pokernow-0.6.45/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:18:22.000000 pokernow-0.6.45/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:18:22.000000 pokernow-0.6.45/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.6.45/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 00:18:23.083037 pokernow-0.6.45/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-05-03 00:18:00.000000 pokernow-0.6.45/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:20:18.886231 pokernow-0.6.55/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.6.55/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.6.55/MANIFEST.in
+-rw-rw-rw-   0        0        0    10070 2024-05-03 00:20:18.885234 pokernow-0.6.55/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 00:20:18.871273 pokernow-0.6.55/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.6.55/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.6.55/PokerNow/client.py
+-rw-rw-rw-   0        0        0     9935 2024-05-03 00:19:54.000000 pokernow-0.6.55/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.6.55/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:20:18.884223 pokernow-0.6.55/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10070 2024-05-03 00:20:18.000000 pokernow-0.6.55/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-03 00:20:18.000000 pokernow-0.6.55/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 00:20:18.000000 pokernow-0.6.55/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:20:18.000000 pokernow-0.6.55/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:20:18.000000 pokernow-0.6.55/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.6.55/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 00:20:18.886231 pokernow-0.6.55/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-05-03 00:20:07.000000 pokernow-0.6.55/setup.py
```

### Comparing `pokernow-0.6.45/LICENSE` & `pokernow-0.6.55/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.45/PKG-INFO` & `pokernow-0.6.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.6.45
+Version: 0.6.55
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.6.45/PokerNow/client.py` & `pokernow-0.6.55/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.45/PokerNow/managers.py` & `pokernow-0.6.55/PokerNow/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pickle
+import traceback
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.common.exceptions import NoSuchElementException, TimeoutException
 from selenium.webdriver.support import expected_conditions as EC
 from .models import Card, GameState, PlayerInfo, PlayerState
 
 class CookieManager:
@@ -212,13 +213,17 @@
             print(f"Trying to find element with selector: {selector}")
             element = self.driver.find_element(By.CSS_SELECTOR, selector)
             print(f"Found element with selector: {selector}")
             return element
         except NoSuchElementException:
             print(f"Element with selector '{selector}' not found.")
             return None
+        except Exception as e:
+            print(f"An error occurred while trying to find element with selector '{selector}':")
+            traceback.print_exc()
+            return None
 
     def get_elements(self, selector):
         try:
             return self.driver.find_elements(By.CSS_SELECTOR, selector)
         except NoSuchElementException:
             return []
```

### Comparing `pokernow-0.6.45/PokerNow/models.py` & `pokernow-0.6.55/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.45/PokerNow.egg-info/PKG-INFO` & `pokernow-0.6.55/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.6.45
+Version: 0.6.55
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.6.45/README.md` & `pokernow-0.6.55/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.45/setup.py` & `pokernow-0.6.55/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.6.45',
+    version='0.6.55',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

