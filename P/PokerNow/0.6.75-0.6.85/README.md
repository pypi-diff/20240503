# Comparing `tmp/pokernow-0.6.75.tar.gz` & `tmp/pokernow-0.6.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.6.75.tar", last modified: Fri May  3 00:26:42 2024, max compression
+gzip compressed data, was "pokernow-0.6.85.tar", last modified: Fri May  3 00:30:20 2024, max compression
```

## Comparing `pokernow-0.6.75.tar` & `pokernow-0.6.85.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:26:42.395943 pokernow-0.6.75/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.6.75/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.6.75/MANIFEST.in
--rw-rw-rw-   0        0        0    10070 2024-05-03 00:26:42.390976 pokernow-0.6.75/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 00:26:42.377641 pokernow-0.6.75/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.6.75/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.6.75/PokerNow/client.py
--rw-rw-rw-   0        0        0     9960 2024-05-03 00:25:36.000000 pokernow-0.6.75/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.6.75/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:26:42.389979 pokernow-0.6.75/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10070 2024-05-03 00:26:42.000000 pokernow-0.6.75/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-03 00:26:42.000000 pokernow-0.6.75/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:26:42.000000 pokernow-0.6.75/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:26:42.000000 pokernow-0.6.75/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:26:42.000000 pokernow-0.6.75/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.6.75/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 00:26:42.396940 pokernow-0.6.75/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-05-03 00:26:31.000000 pokernow-0.6.75/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:30:20.702699 pokernow-0.6.85/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.6.85/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.6.85/MANIFEST.in
+-rw-rw-rw-   0        0        0    10070 2024-05-03 00:30:20.701492 pokernow-0.6.85/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 00:30:20.689006 pokernow-0.6.85/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.6.85/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.6.85/PokerNow/client.py
+-rw-rw-rw-   0        0        0    10018 2024-05-03 00:29:48.000000 pokernow-0.6.85/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.6.85/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:30:20.701492 pokernow-0.6.85/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10070 2024-05-03 00:30:20.000000 pokernow-0.6.85/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-03 00:30:20.000000 pokernow-0.6.85/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 00:30:20.000000 pokernow-0.6.85/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:30:20.000000 pokernow-0.6.85/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:30:20.000000 pokernow-0.6.85/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.6.85/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 00:30:20.702699 pokernow-0.6.85/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-05-03 00:29:56.000000 pokernow-0.6.85/setup.py
```

### Comparing `pokernow-0.6.75/LICENSE` & `pokernow-0.6.85/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.75/PKG-INFO` & `pokernow-0.6.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.6.75
+Version: 0.6.85
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.6.75/PokerNow/client.py` & `pokernow-0.6.85/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.75/PokerNow/managers.py` & `pokernow-0.6.85/PokerNow/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
                 bet_value=self.parse_stack_value(self.element_helper.get_text('.table-player-bet-value .chips-value', player_element)),
                 cards=self.get_player_cards(player_element),
                 status=self.get_player_status(player_element),
                 hand_message=hand_message
             ))
         return players
 
-
     def get_player_status(self, player_element):
         class_list = player_element.get_attribute('class').split()
         if 'decision-current' in class_list:
             return PlayerState.CURRENT
         if 'fold' in class_list:
             return PlayerState.FOLDED
         if 'offline' in class_list:
@@ -207,14 +206,15 @@
             return element.text.strip()
         except NoSuchElementException:
             return ""
 
     def get_element(self, selector):
         try:
             print(f"Trying to find element with selector: {selector}")
+            print(f"Arguments received: self, {selector}")
             element = self.driver.find_element(By.CSS_SELECTOR, selector)
             print(f"Found element with selector: {selector}")
             return element
         except NoSuchElementException:
             print(f"Element with selector '{selector}' not found.")
             return None
         except Exception as e:
```

### Comparing `pokernow-0.6.75/PokerNow/models.py` & `pokernow-0.6.85/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.75/PokerNow.egg-info/PKG-INFO` & `pokernow-0.6.85/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.6.75
+Version: 0.6.85
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.6.75/README.md` & `pokernow-0.6.85/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.75/setup.py` & `pokernow-0.6.85/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.6.75',
+    version='0.6.85',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

