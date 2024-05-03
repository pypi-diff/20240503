# Comparing `tmp/pokernow-0.7.265.tar.gz` & `tmp/pokernow-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokernow-0.7.265.tar", last modified: Fri May  3 00:48:17 2024, max compression
+gzip compressed data, was "pokernow-0.7.5.tar", last modified: Fri May  3 00:40:59 2024, max compression
```

## Comparing `pokernow-0.7.265.tar` & `pokernow-0.7.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:48:17.675338 pokernow-0.7.265/
--rw-rw-rw-   0        0        0     1064 2024-04-24 19:41:53.000000 pokernow-0.7.265/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-24 19:41:42.000000 pokernow-0.7.265/MANIFEST.in
--rw-rw-rw-   0        0        0    10071 2024-05-03 00:48:17.674341 pokernow-0.7.265/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 00:48:17.658384 pokernow-0.7.265/PokerNow/
--rw-rw-rw-   0        0        0      341 2024-04-26 00:33:11.000000 pokernow-0.7.265/PokerNow/__init__.py
--rw-rw-rw-   0        0        0      750 2024-05-03 00:38:17.000000 pokernow-0.7.265/PokerNow/client.py
--rw-rw-rw-   0        0        0    16439 2024-05-03 00:46:49.000000 pokernow-0.7.265/PokerNow/managers.py
--rw-rw-rw-   0        0        0     1826 2024-05-03 00:47:43.000000 pokernow-0.7.265/PokerNow/models.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:48:17.673344 pokernow-0.7.265/PokerNow.egg-info/
--rw-rw-rw-   0        0        0    10071 2024-05-03 00:48:17.000000 pokernow-0.7.265/PokerNow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-03 00:48:17.000000 pokernow-0.7.265/PokerNow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:48:17.000000 pokernow-0.7.265/PokerNow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:48:17.000000 pokernow-0.7.265/PokerNow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:48:17.000000 pokernow-0.7.265/PokerNow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9199 2024-04-24 20:09:28.000000 pokernow-0.7.265/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 00:48:17.675338 pokernow-0.7.265/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-03 00:48:12.000000 pokernow-0.7.265/setup.py
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

### Comparing `pokernow-0.7.265/LICENSE` & `pokernow-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.265/PKG-INFO` & `pokernow-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.7.265
+Version: 0.7.5
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.7.265/PokerNow/client.py` & `pokernow-0.7.5/PokerNow/client.py`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.265/PokerNow/managers.py` & `pokernow-0.7.5/PokerNow/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,37 +102,33 @@
         print(f"Found {len(card_elements)} card elements") # Debug print
         community_cards = [Card.parse_card_class(card.get_attribute('class')) for card in card_elements]
         print(f"Community cards: {community_cards}") # Debug print
         print("Leaving get_community_cards()") # Debug print
         return community_cards
 
     def get_players_info(self):
-        print("Entering get_players_info()")  # Debug print
+        print("Entering get_players_info()") # Debug print
         players = []
         for player_element in self.element_helper.get_elements('.table-player'):
             hand_message = self.element_helper.get_text('.player-hand-message .name', player_element)
 
             stack_element = self.element_helper.get_element('.table-player-stack', player_element)
             is_all_in = 'All In' in stack_element.text if stack_element and stack_element.text else False
 
-            name = self.element_helper.get_text('.table-player-name a', player_element)
-            stack_value = self.element_helper.get_text('.table-player-stack .chips-value', player_element)
-            bet_value = self.element_helper.get_text('.table-player-bet-value .chips-value', player_element)
-
             player_info = PlayerInfo(
-                name=name,
-                stack=self.parse_stack_value(stack_value) if not is_all_in else 'All In',
-                bet_value=self.parse_stack_value(bet_value),
+                name=self.element_helper.get_text('.table-player-name a', player_element),
+                stack=self.parse_stack_value(self.element_helper.get_text('.table-player-stack .chips-value', player_element)) if not is_all_in else 'All In',
+                bet_value=self.parse_stack_value(self.element_helper.get_text('.table-player-bet-value .chips-value', player_element)),
                 cards=self.get_player_cards(player_element),
                 status=self.get_player_status(player_element),
                 hand_message=hand_message
             )
-            print(f"Player info: {player_info}")  # Debug print
+            print(f"Player info: {player_info}") # Debug print
             players.append(player_info)
-        print("Leaving get_players_info()")  # Debug print
+        print("Leaving get_players_info()") # Debug print
         return players
 
     def get_player_status(self, player_element):
         print("Entering get_player_status()") # Debug print
         class_list = player_element.get_attribute('class').split()
         if 'decision-current' in class_list:
             status = PlayerState.CURRENT
```

### Comparing `pokernow-0.7.265/PokerNow/models.py` & `pokernow-0.7.5/PokerNow/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,24 @@
                 rank = rank_dict.get(rank, rank)
             elif part in ["card-c", "card-d", "card-h", "card-s"]:
                 suit_dict = {"card-c": "Clubs", "card-d": "Diamonds", "card-h": "Hearts", "card-s": "Spades"}
                 suit = suit_dict.get(part)
         return f'{rank} of {suit}' if rank and suit else 'Unknown Card'
         
 class GameState:
-    def __init__(self, game_type, pot_size, community_cards, players, dealer_position, current_player, blinds, winners=None, is_your_turn=False, available_actions=None):
+    def __init__(self, game_type, pot_size, community_cards, players, dealer_position, current_player, blinds, winners=None, is_your_turn=False):
         self.game_type = game_type
         self.pot_size = pot_size
         self.community_cards = community_cards
         self.players = players
         self.dealer_position = dealer_position
         self.current_player = current_player
         self.blinds = blinds
         self.winners = winners
         self.is_your_turn = is_your_turn
-        self.available_actions = available_actions
 
 class PlayerInfo:
     def __init__(self, name, stack, bet_value, cards, status, hand_message=''):
         self.name = name
         self.stack = stack
         self.bet_value = bet_value
         self.cards = cards
```

### Comparing `pokernow-0.7.265/PokerNow.egg-info/PKG-INFO` & `pokernow-0.7.5/PokerNow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PokerNow
-Version: 0.7.265
+Version: 0.7.5
 Summary: A Python client for interacting with PokerNow games via the web.
 Home-page: https://github.com/Zehmosu/PokerNow/
 Author: Zehm
 Author-email: mrtentacleshasallthetalent@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Games/Entertainment
```

### Comparing `pokernow-0.7.265/README.md` & `pokernow-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pokernow-0.7.265/setup.py` & `pokernow-0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PokerNow',
-    version='0.7.265',
+    version='0.7.05',
     author='Zehm',
     author_email='mrtentacleshasallthetalent@gmail.com',
     description='A Python client for interacting with PokerNow games via the web.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zehmosu/PokerNow/',
     packages=find_packages(),
```

