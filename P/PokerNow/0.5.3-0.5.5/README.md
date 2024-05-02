# Comparing `tmp/pokernow-0.5.3.tar.gz` & `tmp/pokernow-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.5.3.tar", last modified: Thu May  2 21:29:49 2024, max compression
+gzip compressed data, was "pokernow-0.5.5.tar", last modified: Thu May  2 23:39:17 2024, max compression
```

## Comparing `pokernow-0.5.3.tar` & `pokernow-0.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 21:29:49.816314 pokernow-0.5.3/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0    10069 2024-05-02 21:29:49.812750 pokernow-0.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 21:29:49.791101 pokernow-0.5.3/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.5.3/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.5.3/PokerNow/client.py
--rw-rw-rw-   0        0        0     9526 2024-05-02 21:29:25.000000 pokernow-0.5.3/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.5.3/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:29:49.811230 pokernow-0.5.3/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10069 2024-05-02 21:29:49.000000 pokernow-0.5.3/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-02 21:29:49.000000 pokernow-0.5.3/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 21:29:49.000000 pokernow-0.5.3/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 21:29:49.000000 pokernow-0.5.3/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 21:29:49.000000 pokernow-0.5.3/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.5.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 21:29:49.816314 pokernow-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-05-02 21:29:46.000000 pokernow-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:39:17.509498 pokernow-0.5.5/
+-rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    10069 2024-05-02 23:39:17.509498 pokernow-0.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 23:39:17.498390 pokernow-0.5.5/PokerNow/
+-rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.5.5/PokerNow/__init__.py
+-rw-rw-rw-   0        0        0      697 2024-04-26 00:39:39.000000 pokernow-0.5.5/PokerNow/client.py
+-rw-rw-rw-   0        0        0     9494 2024-05-02 23:38:40.000000 pokernow-0.5.5/PokerNow/managers.py
+-rw-rw-rw-   0        0        0     1750 2024-05-01 20:02:08.000000 pokernow-0.5.5/PokerNow/models.py
+drwxrwxrwx   0        0        0        0 2024-05-02 23:39:17.508486 pokernow-0.5.5/PokerNow.egg-info/
+-rw-rw-rw-   0        0        0    10069 2024-05-02 23:39:17.000000 pokernow-0.5.5/PokerNow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-05-02 23:39:17.000000 pokernow-0.5.5/PokerNow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 23:39:17.000000 pokernow-0.5.5/PokerNow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 23:39:17.000000 pokernow-0.5.5/PokerNow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 23:39:17.000000 pokernow-0.5.5/PokerNow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 23:39:17.509498 pokernow-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-02 23:39:14.000000 pokernow-0.5.5/setup.py
```

### Comparing `pokernow-0.5.3/LICENSE` & `pokernow-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.3/PKG-INFO` & `pokernow-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.5.3
+Version: 0.5.5
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.5.3/PokerNow/client.py` & `pokernow-0.5.5/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.3/PokerNow/managers.py` & `pokernow-0.5.5/PokerNow/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,20 +40,21 @@
             winners=self.get_winners(),
             is_your_turn=self.is_your_turn() 
         )
 
     def is_your_turn(self):
         try:
             action_signal = self.element_helper.get_element('.action-signal')
-            if action_signal:
+            if action_signal and action_signal.text:
                 return action_signal.text.strip() == 'Your Turn'
             else:
                 return False
         except NoSuchElementException:
             return False
+            
     def get_winners(self):
         winners = []
         try:
             winner_elements = self.element_helper.get_elements('.table-player.winner')
             for winner_element in winner_elements:
                 # Extract the winner's name
                 name = self.element_helper.get_text('.table-player-name a', winner_element)
@@ -74,31 +75,30 @@
     def get_community_cards(self):
         card_elements = self.element_helper.get_elements('.table-cards .card-container')
         return [Card.parse_card_class(card.get_attribute('class')) for card in card_elements]
 
     def get_players_info(self):
         players = []
         for player_element in self.element_helper.get_elements('.table-player'):
-            # Extract hand message if available
             hand_message = self.element_helper.get_text('.player-hand-message .name', player_element)
 
-            # Check if the player is all-in
             stack_element = self.element_helper.get_element('.table-player-stack', player_element)
-            is_all_in = 'All In' in stack_element.text if stack_element else False
+            is_all_in = 'All In' in stack_element.text if stack_element and stack_element.text else False
 
             players.append(PlayerInfo(
                 name=self.element_helper.get_text('.table-player-name a', player_element),
                 stack=self.parse_stack_value(self.element_helper.get_text('.table-player-stack .chips-value', player_element)) if not is_all_in else 'All In',
                 bet_value=self.parse_stack_value(self.element_helper.get_text('.table-player-bet-value .chips-value', player_element)),
                 cards=self.get_player_cards(player_element),
                 status=self.get_player_status(player_element),
                 hand_message=hand_message
             ))
         return players
 
+
     def get_player_status(self, player_element):
         class_list = player_element.get_attribute('class').split()
         if 'decision-current' in class_list:
             return PlayerState.CURRENT
         if 'fold' in class_list:
             return PlayerState.FOLDED
         if 'offline' in class_list:
```

### Comparing `pokernow-0.5.3/PokerNow/models.py` & `pokernow-0.5.5/PokerNow/models.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.3/PokerNow.egg-info/PKG-INFO` & `pokernow-0.5.5/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.5.3
+Version: 0.5.5
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.5.3/README.md` & `pokernow-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.5.3/setup.py` & `pokernow-0.5.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.5.3',
+    version='0.5.5',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

