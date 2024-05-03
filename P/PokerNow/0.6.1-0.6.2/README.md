# Comparing `tmp/pokernow-0.6.1.tar.gz` & `tmp/pokernow-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.6.1.tar", last modified: Fri May  3 00:06:31 2024, max compression
+gzip compressed data, was "pokernow-0.6.2.tar", last modified: Fri May  3 00:11:49 2024, max compression
```

## Comparing `pokernow-0.6.1.tar` & `pokernow-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:06:31.961824 pokernow-0.6.1/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.6.1/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10069 2024-05-03 00:06:31.961824 pokernow-0.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 00:06:31.949024 pokernow-0.6.1/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.6.1/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.6.1/PokerNow/client.py
--rw-rw-rw-   0        0        0     9545 2024-05-03 00:04:51.000000 pokernow-0.6.1/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.6.1/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:06:31.960820 pokernow-0.6.1/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10069 2024-05-03 00:06:31.000000 pokernow-0.6.1/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-03 00:06:31.000000 pokernow-0.6.1/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:06:31.000000 pokernow-0.6.1/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:06:31.000000 pokernow-0.6.1/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:06:31.000000 pokernow-0.6.1/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.6.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 00:06:31.961824 pokernow-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-05-03 00:06:17.000000 pokernow-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:11:49.733039 pokernow-0.6.2/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    10069 2024-05-03 00:11:49.733039 pokernow-0.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 00:11:49.715047 pokernow-0.6.2/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.6.2/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.6.2/PokerNow/client.py
+-rw-rw-rw-   0        0        0     9401 2024-05-03 00:11:21.000000 pokernow-0.6.2/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.6.2/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-03 00:11:49.732042 pokernow-0.6.2/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10069 2024-05-03 00:11:49.000000 pokernow-0.6.2/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-03 00:11:49.000000 pokernow-0.6.2/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 00:11:49.000000 pokernow-0.6.2/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:11:49.000000 pokernow-0.6.2/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 00:11:49.000000 pokernow-0.6.2/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 00:11:49.733039 pokernow-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-03 00:11:35.000000 pokernow-0.6.2/setup.py
```

### Comparing `pokernow-0.6.1/LICENSE` & `pokernow-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.1/PKG-INFO` & `pokernow-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.6.1/PokerNow/client.py` & `pokernow-0.6.2/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.1/PokerNow/managers.py` & `pokernow-0.6.2/PokerNow/managers.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,16 @@
             pot_size=self.parse_stack_value(self.element_helper.get_text('.table-pot-size .main-value')),
             community_cards=self.get_community_cards(),
             players=self.get_players_info(),
             dealer_position=self.get_dealer_position(),
             current_player=self.get_current_player(),
             blinds=self.get_blinds(),
             winners=self.get_winners(),
-            is_your_turn=self.is_your_turn() 
+            is_your_turn=self.is_your_turn(),
+            available_actions=self.get_available_actions()
         )
 
     def is_your_turn(self):
         try:
             action_signal = self.element_helper.get_element('.action-signal')
             if action_signal and action_signal.text:
                 return action_signal.text.strip() == 'Your Turn'
@@ -127,24 +128,20 @@
         return stack_value.strip()
 
 class ActionHelper:
     def __init__(self, element_helper):
         self.element_helper = element_helper
 
     def get_available_actions(self):
-        available_actions = {}
-        for action_name, selector in {
-            'Call': '.game-decisions-ctn .button-1.call',
-            'Raise': '.game-decisions-ctn .button-1.raise',
-            'Check': '.game-decisions-ctn .button-1.check',
-            'Fold': '.game-decisions-ctn .button-1.fold'
-        }.items():
-            element = self.element_helper.get_element(selector)
-            if element and element.is_displayed() and not element.get_attribute('disabled'):
-                available_actions[action_name] = element
+        available_actions = []
+        action_elements = self.element_helper.get_elements('.game-decisions-ctn .button-1')
+        for element in action_elements:
+            action_text = element.text.strip().lower()
+            if action_text in ['fold', 'call', 'raise', 'check']:
+                available_actions.append(action_text)
         return available_actions
 
     def perform_action(self, action, amount=None):
         available_actions = self.get_available_actions()
         if action == 'Raise' and available_actions.get('Raise'):
             self.handle_raise(amount)
         elif action in available_actions:
```

### Comparing `pokernow-0.6.1/PokerNow/models.py` & `pokernow-0.6.2/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.1/PokerNow.egg-info/PKG-INFO` & `pokernow-0.6.2/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.6.1/README.md` & `pokernow-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.6.1/setup.py` & `pokernow-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.6.1',
+    version='0.6.2',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

