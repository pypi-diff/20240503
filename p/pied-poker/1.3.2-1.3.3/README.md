# Comparing `tmp/pied_poker-1.3.2.tar.gz` & `tmp/pied_poker-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pied_poker-1.3.2.tar", last modified: Mon Apr 29 01:04:06 2024, max compression
+gzip compressed data, was "pied_poker-1.3.3.tar", last modified: Fri May  3 02:06:58 2024, max compression
```

## Comparing `pied_poker-1.3.2.tar` & `pied_poker-1.3.3.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.706589 pied_poker-1.3.2/
--rw-r--r--   0 ellek      (501) staff       (20)      737 2024-04-29 01:04:06.706331 pied_poker-1.3.2/PKG-INFO
--rw-r--r--   0 ellek      (501) staff       (20)    31804 2024-01-10 19:08:36.000000 pied_poker-1.3.2/README.md
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.688476 pied_poker-1.3.2/pied_poker/
--rw-r--r--   0 ellek      (501) staff       (20)      217 2024-04-26 23:52:39.000000 pied_poker-1.3.2/pied_poker/__init__.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.691446 pied_poker-1.3.2/pied_poker/card/
--rw-r--r--   0 ellek      (501) staff       (20)      164 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/card/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1846 2024-04-27 07:59:57.000000 pied_poker-1.3.2/pied_poker/card/card.py
--rw-r--r--   0 ellek      (501) staff       (20)      379 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/card/comparable.py
--rw-r--r--   0 ellek      (501) staff       (20)     2322 2024-04-27 08:03:38.000000 pied_poker-1.3.2/pied_poker/card/rank.py
--rw-r--r--   0 ellek      (501) staff       (20)      989 2024-04-27 08:03:38.000000 pied_poker-1.3.2/pied_poker/card/suit.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.692041 pied_poker-1.3.2/pied_poker/deck/
--rw-r--r--   0 ellek      (501) staff       (20)       38 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/deck/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     2450 2023-08-19 21:24:44.000000 pied_poker-1.3.2/pied_poker/deck/deck.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.696893 pied_poker-1.3.2/pied_poker/hand/
--rw-r--r--   0 ellek      (501) staff       (20)      724 2023-08-21 04:17:06.000000 pied_poker-1.3.2/pied_poker/hand/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)    10894 2023-12-23 23:23:25.000000 pied_poker-1.3.2/pied_poker/hand/base_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1061 2023-01-25 00:26:09.000000 pied_poker-1.3.2/pied_poker/hand/empty_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     3215 2023-01-30 23:07:57.000000 pied_poker-1.3.2/pied_poker/hand/flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2567 2023-01-10 07:31:28.000000 pied_poker-1.3.2/pied_poker/hand/four_of_a_kind.py
--rw-r--r--   0 ellek      (501) staff       (20)     3511 2023-06-08 21:06:49.000000 pied_poker-1.3.2/pied_poker/hand/full_house.py
--rw-r--r--   0 ellek      (501) staff       (20)     3375 2023-06-08 21:28:48.000000 pied_poker-1.3.2/pied_poker/hand/high_card.py
--rw-r--r--   0 ellek      (501) staff       (20)      853 2023-08-21 04:23:37.000000 pied_poker-1.3.2/pied_poker/hand/killer_card.py
--rw-r--r--   0 ellek      (501) staff       (20)     2913 2023-01-10 07:31:44.000000 pied_poker-1.3.2/pied_poker/hand/one_pair.py
--rw-r--r--   0 ellek      (501) staff       (20)      858 2023-12-23 23:24:38.000000 pied_poker-1.3.2/pied_poker/hand/out.py
--rw-r--r--   0 ellek      (501) staff       (20)     3318 2023-01-10 06:50:18.000000 pied_poker-1.3.2/pied_poker/hand/poker_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1953 2023-01-10 08:17:04.000000 pied_poker-1.3.2/pied_poker/hand/royal_flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2099 2023-01-10 07:31:59.000000 pied_poker-1.3.2/pied_poker/hand/straight.py
--rw-r--r--   0 ellek      (501) staff       (20)     2012 2023-01-10 08:11:25.000000 pied_poker-1.3.2/pied_poker/hand/straight_flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2853 2023-01-10 07:32:10.000000 pied_poker-1.3.2/pied_poker/hand/three_of_a_kind.py
--rw-r--r--   0 ellek      (501) staff       (20)     3493 2023-01-10 07:32:15.000000 pied_poker-1.3.2/pied_poker/hand/two_pair.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.697488 pied_poker-1.3.2/pied_poker/player/
--rw-r--r--   0 ellek      (501) staff       (20)       44 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/player/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)      840 2023-07-21 23:13:34.000000 pied_poker-1.3.2/pied_poker/player/player.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.699079 pied_poker-1.3.2/pied_poker/poker_round/
--rw-r--r--   0 ellek      (501) staff       (20)      297 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/poker_round/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     4485 2024-04-27 07:52:43.000000 pied_poker-1.3.2/pied_poker/poker_round/poker_round.py
--rw-r--r--   0 ellek      (501) staff       (20)     4728 2023-08-21 05:02:53.000000 pied_poker-1.3.2/pied_poker/poker_round/poker_round_result.py
--rw-r--r--   0 ellek      (501) staff       (20)     6794 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/poker_round/poker_round_simulation_result.py
--rw-r--r--   0 ellek      (501) staff       (20)     4628 2024-04-27 22:03:51.000000 pied_poker-1.3.2/pied_poker/poker_round/poker_round_simulator.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.700200 pied_poker-1.3.2/pied_poker/probability/
--rw-r--r--   0 ellek      (501) staff       (20)      959 2024-04-28 01:12:54.000000 pied_poker-1.3.2/pied_poker/probability/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1053 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/base_poker_event.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.704643 pied_poker-1.3.2/pied_poker/probability/events/
--rw-r--r--   0 ellek      (501) staff       (20)      980 2023-01-01 00:47:51.000000 pied_poker-1.3.2/pied_poker/probability/events/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)      861 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/community_cards_include.py
--rw-r--r--   0 ellek      (501) staff       (20)      770 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/no_tie.py
--rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_card_ranks.py
--rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_card_suits.py
--rw-r--r--   0 ellek      (501) staff       (20)     1181 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_cards.py
--rw-r--r--   0 ellek      (501) staff       (20)     1611 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1224 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_hand_or_higher.py
--rw-r--r--   0 ellek      (501) staff       (20)     2218 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_pocket_pair.py
--rw-r--r--   0 ellek      (501) staff       (20)     1520 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_has_suited_cards.py
--rw-r--r--   0 ellek      (501) staff       (20)      792 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_loses.py
--rw-r--r--   0 ellek      (501) staff       (20)     1275 2022-03-21 04:52:37.000000 pied_poker-1.3.2/pied_poker/probability/events/player_wins.py
--rw-r--r--   0 ellek      (501) staff       (20)      959 2023-01-01 00:52:22.000000 pied_poker-1.3.2/pied_poker/probability/events/player_wins_with_tie.py
--rw-r--r--   0 ellek      (501) staff       (20)      767 2023-01-01 00:43:13.000000 pied_poker-1.3.2/pied_poker/probability/events/tie.py
--rw-r--r--   0 ellek      (501) staff       (20)     1445 2024-04-29 00:54:21.000000 pied_poker-1.3.2/pied_poker/probability/probability_value.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.705927 pied_poker-1.3.2/pied_poker/visualization/
--rw-r--r--   0 ellek      (501) staff       (20)      245 2023-12-23 23:33:26.000000 pied_poker-1.3.2/pied_poker/visualization/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     8326 2023-12-28 22:01:51.000000 pied_poker-1.3.2/pied_poker/visualization/data_generator.py
--rw-r--r--   0 ellek      (501) staff       (20)     5061 2023-12-23 23:33:26.000000 pied_poker-1.3.2/pied_poker/visualization/pocket_pairs_vs_num_players.py
--rw-r--r--   0 ellek      (501) staff       (20)     6366 2023-12-23 23:33:26.000000 pied_poker-1.3.2/pied_poker/visualization/starting_card_probabilities.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-04-29 01:04:06.689973 pied_poker-1.3.2/pied_poker.egg-info/
--rw-r--r--   0 ellek      (501) staff       (20)      737 2024-04-29 01:04:06.000000 pied_poker-1.3.2/pied_poker.egg-info/PKG-INFO
--rw-r--r--   0 ellek      (501) staff       (20)     2161 2024-04-29 01:04:06.000000 pied_poker-1.3.2/pied_poker.egg-info/SOURCES.txt
--rw-r--r--   0 ellek      (501) staff       (20)        1 2024-04-29 01:04:06.000000 pied_poker-1.3.2/pied_poker.egg-info/dependency_links.txt
--rw-r--r--   0 ellek      (501) staff       (20)       50 2024-04-29 01:04:06.000000 pied_poker-1.3.2/pied_poker.egg-info/requires.txt
--rw-r--r--   0 ellek      (501) staff       (20)       11 2024-04-29 01:04:06.000000 pied_poker-1.3.2/pied_poker.egg-info/top_level.txt
--rw-r--r--   0 ellek      (501) staff       (20)       38 2024-04-29 01:04:06.706710 pied_poker-1.3.2/setup.cfg
--rw-r--r--   0 ellek      (501) staff       (20)     1275 2024-04-29 01:03:58.000000 pied_poker-1.3.2/setup.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.127386 pied_poker-1.3.3/
+-rw-r--r--   0 ellek      (501) staff       (20)      737 2024-05-03 02:06:58.127092 pied_poker-1.3.3/PKG-INFO
+-rw-r--r--   0 ellek      (501) staff       (20)    31804 2024-01-10 19:08:36.000000 pied_poker-1.3.3/README.md
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.093922 pied_poker-1.3.3/pied_poker/
+-rw-r--r--   0 ellek      (501) staff       (20)      217 2024-04-26 23:52:39.000000 pied_poker-1.3.3/pied_poker/__init__.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.098925 pied_poker-1.3.3/pied_poker/card/
+-rw-r--r--   0 ellek      (501) staff       (20)      164 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/card/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1846 2024-04-27 07:59:57.000000 pied_poker-1.3.3/pied_poker/card/card.py
+-rw-r--r--   0 ellek      (501) staff       (20)      379 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/card/comparable.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2322 2024-04-27 08:03:38.000000 pied_poker-1.3.3/pied_poker/card/rank.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1040 2024-05-03 00:06:22.000000 pied_poker-1.3.3/pied_poker/card/suit.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.100043 pied_poker-1.3.3/pied_poker/deck/
+-rw-r--r--   0 ellek      (501) staff       (20)       38 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/deck/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2450 2023-08-19 21:24:44.000000 pied_poker-1.3.3/pied_poker/deck/deck.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.107964 pied_poker-1.3.3/pied_poker/hand/
+-rw-r--r--   0 ellek      (501) staff       (20)      765 2024-05-03 00:06:22.000000 pied_poker-1.3.3/pied_poker/hand/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)    14392 2024-05-03 01:49:31.000000 pied_poker-1.3.3/pied_poker/hand/base_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1061 2023-01-25 00:26:09.000000 pied_poker-1.3.3/pied_poker/hand/empty_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3215 2023-01-30 23:07:57.000000 pied_poker-1.3.3/pied_poker/hand/flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2567 2023-01-10 07:31:28.000000 pied_poker-1.3.3/pied_poker/hand/four_of_a_kind.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3511 2023-06-08 21:06:49.000000 pied_poker-1.3.3/pied_poker/hand/full_house.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3375 2023-06-08 21:28:48.000000 pied_poker-1.3.3/pied_poker/hand/high_card.py
+-rw-r--r--   0 ellek      (501) staff       (20)      853 2023-08-21 04:23:37.000000 pied_poker-1.3.3/pied_poker/hand/killer_card.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2937 2024-05-03 00:26:44.000000 pied_poker-1.3.3/pied_poker/hand/one_pair.py
+-rw-r--r--   0 ellek      (501) staff       (20)      858 2023-12-23 23:24:38.000000 pied_poker-1.3.3/pied_poker/hand/out.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1961 2024-05-03 00:26:44.000000 pied_poker-1.3.3/pied_poker/hand/royal_flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2107 2024-05-03 00:26:44.000000 pied_poker-1.3.3/pied_poker/hand/straight.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2020 2024-05-03 00:26:44.000000 pied_poker-1.3.3/pied_poker/hand/straight_flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2877 2024-05-03 00:26:44.000000 pied_poker-1.3.3/pied_poker/hand/three_of_a_kind.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3497 2024-05-03 01:30:05.000000 pied_poker-1.3.3/pied_poker/hand/two_pair.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.108928 pied_poker-1.3.3/pied_poker/player/
+-rw-r--r--   0 ellek      (501) staff       (20)       44 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/player/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1159 2024-05-03 01:57:12.000000 pied_poker-1.3.3/pied_poker/player/player.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.111035 pied_poker-1.3.3/pied_poker/poker_round/
+-rw-r--r--   0 ellek      (501) staff       (20)      297 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/poker_round/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     4485 2024-04-27 07:52:43.000000 pied_poker-1.3.3/pied_poker/poker_round/poker_round.py
+-rw-r--r--   0 ellek      (501) staff       (20)     6693 2024-05-03 02:00:11.000000 pied_poker-1.3.3/pied_poker/poker_round/poker_round_result.py
+-rw-r--r--   0 ellek      (501) staff       (20)     6788 2024-05-03 00:06:22.000000 pied_poker-1.3.3/pied_poker/poker_round/poker_round_simulation_result.py
+-rw-r--r--   0 ellek      (501) staff       (20)     4628 2024-04-27 22:03:51.000000 pied_poker-1.3.3/pied_poker/poker_round/poker_round_simulator.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.112724 pied_poker-1.3.3/pied_poker/probability/
+-rw-r--r--   0 ellek      (501) staff       (20)      959 2024-04-28 01:12:54.000000 pied_poker-1.3.3/pied_poker/probability/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1053 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/base_poker_event.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.120045 pied_poker-1.3.3/pied_poker/probability/events/
+-rw-r--r--   0 ellek      (501) staff       (20)      980 2023-01-01 00:47:51.000000 pied_poker-1.3.3/pied_poker/probability/events/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)      861 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/community_cards_include.py
+-rw-r--r--   0 ellek      (501) staff       (20)      770 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/no_tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_card_ranks.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_card_suits.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1181 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_cards.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1611 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1224 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_hand_or_higher.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2218 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_pocket_pair.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1520 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_has_suited_cards.py
+-rw-r--r--   0 ellek      (501) staff       (20)      792 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_loses.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1275 2022-03-21 04:52:37.000000 pied_poker-1.3.3/pied_poker/probability/events/player_wins.py
+-rw-r--r--   0 ellek      (501) staff       (20)      959 2023-01-01 00:52:22.000000 pied_poker-1.3.3/pied_poker/probability/events/player_wins_with_tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)      767 2023-01-01 00:43:13.000000 pied_poker-1.3.3/pied_poker/probability/events/tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1445 2024-04-29 00:54:21.000000 pied_poker-1.3.3/pied_poker/probability/probability_value.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.123181 pied_poker-1.3.3/pied_poker/visualization/
+-rw-r--r--   0 ellek      (501) staff       (20)      245 2023-12-23 23:33:26.000000 pied_poker-1.3.3/pied_poker/visualization/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     8326 2023-12-28 22:01:51.000000 pied_poker-1.3.3/pied_poker/visualization/data_generator.py
+-rw-r--r--   0 ellek      (501) staff       (20)     5061 2023-12-23 23:33:26.000000 pied_poker-1.3.3/pied_poker/visualization/pocket_pairs_vs_num_players.py
+-rw-r--r--   0 ellek      (501) staff       (20)     6366 2023-12-23 23:33:26.000000 pied_poker-1.3.3/pied_poker/visualization/starting_card_probabilities.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2024-05-03 02:06:58.095741 pied_poker-1.3.3/pied_poker.egg-info/
+-rw-r--r--   0 ellek      (501) staff       (20)      737 2024-05-03 02:06:57.000000 pied_poker-1.3.3/pied_poker.egg-info/PKG-INFO
+-rw-r--r--   0 ellek      (501) staff       (20)     2131 2024-05-03 02:06:57.000000 pied_poker-1.3.3/pied_poker.egg-info/SOURCES.txt
+-rw-r--r--   0 ellek      (501) staff       (20)        1 2024-05-03 02:06:57.000000 pied_poker-1.3.3/pied_poker.egg-info/dependency_links.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       50 2024-05-03 02:06:57.000000 pied_poker-1.3.3/pied_poker.egg-info/requires.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       11 2024-05-03 02:06:57.000000 pied_poker-1.3.3/pied_poker.egg-info/top_level.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       38 2024-05-03 02:06:58.127505 pied_poker-1.3.3/setup.cfg
+-rw-r--r--   0 ellek      (501) staff       (20)     1275 2024-05-03 00:06:22.000000 pied_poker-1.3.3/setup.py
```

### Comparing `pied_poker-1.3.2/PKG-INFO` & `pied_poker-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pied_poker
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package to run flexible and fast poker simulations using a monte carlo style simulator.
 Home-page: https://github.com/elleklinton/PiedPoker
 Author: Ellek Linton
 Author-email: ellek@elleklinton.com
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pied_poker-1.3.2/README.md` & `pied_poker-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/card/card.py` & `pied_poker-1.3.3/pied_poker/card/card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/card/rank.py` & `pied_poker-1.3.3/pied_poker/card/rank.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/card/suit.py` & `pied_poker-1.3.3/pied_poker/card/suit.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     ALLOWED_VALUES = ['c', 'd', 'h', 's']  # clubs, diamonds, hearts, spades'
 
     def __init__(self, suit: str):
         self.__str_value__ = None
         super().__init__(suit)
 
     def __eq__(self, other):
+        if other is None:
+            return False
         return self.value == other.value
 
     def __hash__(self):
         if self.value == 'c':
             return 0
         if self.value == 'd':
             return 1
```

### Comparing `pied_poker-1.3.2/pied_poker/deck/deck.py` & `pied_poker-1.3.3/pied_poker/deck/deck.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/__init__.py` & `pied_poker-1.3.3/pied_poker/hand/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pied_poker.hand.base_hand import BaseHand
+from pied_poker.hand.base_hand import BaseHand as PokerHand # For backwards compatibility
 from pied_poker.hand.flush import Flush
 from pied_poker.hand.four_of_a_kind import FourOfAKind
 from pied_poker.hand.full_house import FullHouse
 from pied_poker.hand.high_card import HighCard
 from pied_poker.hand.one_pair import OnePair
 from pied_poker.hand.royal_flush import RoyalFlush
 from pied_poker.hand.straight import Straight
 from pied_poker.hand.straight_flush import StraightFlush
 from pied_poker.hand.three_of_a_kind import ThreeOfAKind
 from pied_poker.hand.two_pair import TwoPair
-from pied_poker.hand.poker_hand import PokerHand
 from pied_poker.hand.empty_hand import EmptyHand
 from pied_poker.hand.out import Out
 from pied_poker.hand.killer_card import KillerCard
```

### Comparing `pied_poker-1.3.2/pied_poker/hand/empty_hand.py` & `pied_poker-1.3.3/pied_poker/hand/empty_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/flush.py` & `pied_poker-1.3.3/pied_poker/hand/flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/four_of_a_kind.py` & `pied_poker-1.3.3/pied_poker/hand/four_of_a_kind.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/full_house.py` & `pied_poker-1.3.3/pied_poker/hand/full_house.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/high_card.py` & `pied_poker-1.3.3/pied_poker/hand/high_card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/killer_card.py` & `pied_poker-1.3.3/pied_poker/hand/killer_card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/one_pair.py` & `pied_poker-1.3.3/pied_poker/hand/one_pair.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,42 +30,42 @@
     def cards_not_in_hand(self):
         return [c for c in self.cards_sorted if c.rank not in self.ranks_pair][:3]
 
     def __eq__(self, other):
         if super().__eq__(other):  # Same class of hand
             if self.ranks_pair[0] == other.ranks_pair[0]:  # Same pair
                 # If have same pair, we delegate to HighCard to determine the winner on the rest of the cards at stake
-                return BaseHand(self.cards_not_in_hand).as_hand(HighCard) == BaseHand(other.cards_not_in_hand).as_hand(HighCard)
+                return BaseHand(self.cards_not_in_hand).__as_hand__(HighCard) == BaseHand(other.cards_not_in_hand).__as_hand__(HighCard)
         return False
 
     def __gt__(self, other):
         if super().__gt__(other):
             return True
         elif super().__lt__(other):
             return False
         else:
             if self.ranks_pair[0] > other.ranks_pair[0]:
                 return True
             elif self.ranks_pair[0] == other.ranks_pair[0]:
                 # If have same pair, we delegate to HighCard to determine the winner on the rest of the cards at stake
-                return BaseHand(self.cards_not_in_hand).as_hand(HighCard) > BaseHand(other.cards_not_in_hand).as_hand(HighCard)
+                return BaseHand(self.cards_not_in_hand).__as_hand__(HighCard) > BaseHand(other.cards_not_in_hand).__as_hand__(HighCard)
 
         return False
 
     def __lt__(self, other):
         if super().__gt__(other):
             return False
         if super().__lt__(other):
             return True
         else:
             if self.ranks_pair[0] < other.ranks_pair[0]:
                 return True
             elif self.ranks_pair[0] == other.ranks_pair[0]:
                 # If have same pair, we delegate to HighCard to determine the winner on the rest of the cards at stake
-                return BaseHand(self.cards_not_in_hand).as_hand(HighCard) < BaseHand(other.cards_not_in_hand).as_hand(HighCard)
+                return BaseHand(self.cards_not_in_hand).__as_hand__(HighCard) < BaseHand(other.cards_not_in_hand).__as_hand__(HighCard)
 
         return False
 
     def __hash__(self):
         return hash(str(self))
 
     def __hand_outs__(self, out_cards: Set[Card]) -> List[Card]:
```

### Comparing `pied_poker-1.3.2/pied_poker/hand/out.py` & `pied_poker-1.3.3/pied_poker/hand/out.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/hand/royal_flush.py` & `pied_poker-1.3.3/pied_poker/hand/royal_flush.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def __hash__(self):
         return hash(str(self))
 
     def __hand_outs__(self, out_cards: Set[Card]) -> List[Card]:
         rv = []
 
-        for straight_flush_out in self.as_hand(StraightFlush).__hand_outs__({*out_cards}, True):
-            hand = BaseHand(self.cards_sorted + [straight_flush_out]).as_hand(RoyalFlush)
+        for straight_flush_out in self.__as_hand__(StraightFlush).__hand_outs__({*out_cards}, True):
+            hand = BaseHand(self.cards_sorted + [straight_flush_out]).__as_hand__(RoyalFlush)
             if hand.is_hand:
                 rv.append(straight_flush_out)
                 out_cards.update({straight_flush_out})
         return rv
```

### Comparing `pied_poker-1.3.2/pied_poker/hand/straight.py` & `pied_poker-1.3.3/pied_poker/hand/straight.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     
     def __hand_outs__(self, out_cards: Set[Card]) -> List[Card]:
         # TODO: this could maybe be more efficient, probably don't need to iterate over all cards here
         rv = []
         for card in Deck.ALL_CARDS:
             if card not in self.cards_set and card not in out_cards:
                 newHand = BaseHand(self.cards_sorted + [card]).as_best_hand()
-                if newHand.as_hand(Straight).is_hand or newHand.as_hand(RoyalFlush).is_hand:
+                if newHand.__as_hand__(Straight).is_hand or newHand.__as_hand__(RoyalFlush).is_hand:
                     rv.append(card)
                     out_cards.update([card])
         return rv
```

### Comparing `pied_poker-1.3.2/pied_poker/hand/straight_flush.py` & `pied_poker-1.3.3/pied_poker/hand/straight_flush.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             return self.straight_flush[0] < other.straight_flush[0]
 
     def __hash__(self):
         return hash(str(self))
 
     def __hand_outs__(self, out_cards: Set[Card], include_higher_hand_outs=False) -> List[Card]:
         rv = []
-        for flushOut in self.as_hand(Flush).__hand_outs__({*out_cards}, True):
-            newHand = BaseHand(self.cards_sorted + [flushOut]).as_hand(StraightFlush)
+        for flushOut in self.__as_hand__(Flush).__hand_outs__({*out_cards}, True):
+            newHand = BaseHand(self.cards_sorted + [flushOut]).__as_hand__(StraightFlush)
             if newHand.is_hand and flushOut not in out_cards:
                 if newHand.__class__.hand_rank == StraightFlush.hand_rank or \
                         (newHand.hand_rank > self.hand_rank and include_higher_hand_outs):
                     rv.append(flushOut)
                     out_cards.update([flushOut])
         return rv
```

### Comparing `pied_poker-1.3.2/pied_poker/hand/three_of_a_kind.py` & `pied_poker-1.3.3/pied_poker/hand/three_of_a_kind.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,42 +29,42 @@
     def cards_not_in_hand(self):
         return [c for c in self.cards_sorted if c.rank not in self.ranks_triple][:2]
 
     def __eq__(self, other):
         if super().__eq__(other):  # Same class of hand
             if self.ranks_triple[0] == other.ranks_triple[0]:  # Same triple
                 # If have same triple, we delegate to HighCard to determine the winner on the rest of the cards at stake
-                return BaseHand(self.cards_not_in_hand).as_hand(HighCard) == BaseHand(other.cards_not_in_hand).as_hand(HighCard)
+                return BaseHand(self.cards_not_in_hand).__as_hand__(HighCard) == BaseHand(other.cards_not_in_hand).__as_hand__(HighCard)
         return False
 
     def __gt__(self, other):
         if super().__gt__(other):
             return True
         elif super().__lt__(other):
             return False
         else:
             if self.ranks_triple[0] > other.ranks_triple[0]:
                 return True
             elif self.ranks_triple[0] < other.ranks_triple[0]:
                 return False
             else:  # Same trip card_internals, delegate to HighCard to determine winner
-                return BaseHand(self.cards_not_in_hand).as_hand(HighCard) > BaseHand(other.cards_not_in_hand).as_hand(HighCard)
+                return BaseHand(self.cards_not_in_hand).__as_hand__(HighCard) > BaseHand(other.cards_not_in_hand).__as_hand__(HighCard)
 
     def __lt__(self, other):
         if super().__gt__(other):
             return False
         if super().__lt__(other):
             return True
         else:
             if self.ranks_triple[0] < other.ranks_triple[0]:
                 return True
             elif self.ranks_triple[0] > other.ranks_triple[0]:
                 return False
             else:  # Same trip card_internals, delegate to HighCard to determine winner
-                return BaseHand(self.cards_not_in_hand).as_hand(HighCard) < BaseHand(other.cards_not_in_hand).as_hand(HighCard)
+                return BaseHand(self.cards_not_in_hand).__as_hand__(HighCard) < BaseHand(other.cards_not_in_hand).__as_hand__(HighCard)
 
     def __hash__(self):
         return hash(str(self))
 
     def __hand_outs__(self, out_cards: Set[Card]) -> List[Card]:
         rv = []
         for c in self.ranks_pair:
```

### Comparing `pied_poker-1.3.2/pied_poker/hand/two_pair.py` & `pied_poker-1.3.3/pied_poker/hand/two_pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     @property
     def is_hand(self):
         return len(self.ranks_pair) >= 2
 
     @property
     def cards_in_hand(self):
-        return [c for c in self.cards_sorted if c.rank in self.ranks_pair]
+        return [c for c in self.cards_sorted if c.rank in self.ranks_pair[:2]]
 
     @property
     def cards_not_in_hand(self):
         # Only take the first high card_internals since 2 pair takes up 4/5 cards
         return [c for c in self.cards_sorted if c.rank not in self.ranks_pair][:1]
 
     def __eq__(self, other):
```

### Comparing `pied_poker-1.3.2/pied_poker/player/player.py` & `pied_poker-1.3.3/pied_poker/player/player.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 from typing import List
 
 from pied_poker.card.card import Card
-from pied_poker.hand.poker_hand import PokerHand
+from pied_poker.hand.base_hand import BaseHand
 
 
 class Player:
-    def __init__(self, name: str, cards: List[Card] = None, hand: PokerHand = None):
+    def __init__(self, name: str, cards: List[Card] = None, hand: BaseHand = None):
         self.name = name
         self.cards: List[Card] = cards if cards else []
         self.hand = hand
 
     def poker_hand(self, community_cards: List[Card]):
-        self.hand = PokerHand(self.cards + community_cards)
+        self.hand = BaseHand(self.cards + community_cards)
         self.hand = self.hand.as_best_hand()
         return self.hand
 
+    def add_community_cards(self, *cards: Card):
+        for card in cards:
+            self.hand.add_card(card)
+        self.hand = self.hand.as_best_hand()
+
+    def remove_community_card(self, *cards: Card):
+        for card in cards:
+            self.hand.remove_card(card)
+        self.hand = self.hand.as_best_hand()
+
     def __str__(self):
         return self.__repr__()
 
     def __repr__(self):
         if self.hand is not None:
             return f'{self.name}: {self.hand}'
         return f'{self.name}: {self.cards}'
```

### Comparing `pied_poker-1.3.2/pied_poker/poker_round/poker_round.py` & `pied_poker-1.3.3/pied_poker/poker_round/poker_round.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/poker_round/poker_round_result.py` & `pied_poker-1.3.3/pied_poker/poker_round/poker_round_result.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,18 +10,58 @@
 class PokerRoundResult:
     def __init__(self, players: List[Player], community_cards: List[Card]):
         self.player_one = players[0]
         self.players_ranked = sorted(players, reverse=True, key=lambda p: p.poker_hand(community_cards))
         self.community_cards = community_cards
         self.winners = set([p for p in self.players_ranked if p.hand == self.players_ranked[0].hand])
         self.player_during_round: Dict[Player, Player] = {}
+
         for p in players:
             self.player_during_round[p] = p
 
-        self.__check_unique_cards__()
+        all_player_cards = [card for player in self.players_ranked for card in player.cards]
+        self.player_cards_set: Set[Card] = set(all_player_cards)
+        self.community_cards_set: Set[Card] = set(community_cards)
+
+        if len(self.player_cards_set) != len(all_player_cards):
+            raise ValueError('Error! Duplicate player cards detected')
+        elif len(self.community_cards_set) != len(community_cards):
+            raise ValueError('Error! Duplicate community cards detected')
+
+    def add_community_card(self, *cards: Card):
+        for c in cards:
+            if c in self.community_cards_set:
+                raise ValueError(f'cannot add {c} to community cards, already in community cards')
+            if c in self.player_cards_set:
+                raise ValueError(f'cannot add {c} to community cards, already in player cards')
+
+        self.community_cards.append(*cards)
+        self.community_cards_set.add(*cards)
+
+        for p in self.players_ranked:
+            p.add_community_cards(*cards)
+
+        self.players_ranked = sorted(self.players_ranked, reverse=True, key=lambda p: p.hand)
+        self.winners = set([p for p in self.players_ranked if p.hand == self.players_ranked[0].hand])
+
+    def remove_community_card(self, *cards: Card):
+        for c in cards:
+            if c not in self.community_cards_set:
+                raise ValueError(f'cannot remove {c} from community cards, not in community cards')
+            if c in self.player_cards_set:
+                raise ValueError(f'cannot remove {c} from community cards, in player cards')
+
+        self.community_cards = [c for c in self.community_cards if c not in cards]
+        self.community_cards_set.remove(*cards)
+
+        for p in self.players_ranked:
+            p.remove_community_card(*cards)
+
+        self.players_ranked = sorted(self.players_ranked, reverse=True, key=lambda p: p.hand)
+        self.winners = set([p for p in self.players_ranked if p.hand == self.players_ranked[0].hand])
 
     def outs(self, player: Player, should_include_equal_hand_outs=True) -> List[Out]:
         """
         All the possible one-carded outs that the player could have that are better than their current hand.
 
         By default, "outs" equal to the current hand rank are enabled, so for example, if the current best winning hand
         is ThreeOfAKind, but the player has a possible out with a stronger ThreeOfAKind, that out would only be returned
```

### Comparing `pied_poker-1.3.2/pied_poker/poker_round/poker_round_simulation_result.py` & `pied_poker-1.3.3/pied_poker/poker_round/poker_round_simulation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 
 import pied_poker.probability.base_poker_event as base_poker_event
 import pied_poker.probability.probability_value as probability_value
 import pied_poker.poker_round.poker_round_result as round_result
 import pied_poker.probability.events.player_has_hand as player_has_hand
 import pied_poker.probability.events.player_wins as player_wins
-import pied_poker.hand.poker_hand as poker_hand
+import pied_poker.hand.base_hand as base_hand
 import pied_poker.player as player
 
 
 class PokerRoundSimulationResult:
     def __init__(self, simulation_rounds: List[round_result.PokerRoundResult]):
         """
         An object to store the results of a poker simulation and compute probabilities based on those events.
@@ -98,15 +98,15 @@
         :type player: player.Player
         :return: None
         :rtype: None
         """
         hand_names = []
         hand_probabilities = []
 
-        for hand_type in reversed(poker_hand.PokerHand.ALL_HANDS_RANKED):
+        for hand_type in reversed(base_hand.BaseHand.ALL_HANDS_RANKED):
             p = self.probability_of(player_has_hand.PlayerHasHand(hand_type, player))
             hand_names.append(hand_type.__name__ + f' ({p.__percent_str__})')
             hand_probabilities.append(p.probability)
 
         self.__plot_barplot__(hand_probabilities, hand_names, 'Hand Type Probabilities')
 
     def visualize_winner_distribution(self):
@@ -145,15 +145,15 @@
                 winning_hand_counts[hand_str] = hand_count
                 total_hands += 1
 
         hand_names = []
         hand_probabilities = []
         last_cumulative_probability = 0
 
-        for hand_type in reversed(poker_hand.PokerHand.ALL_HANDS_RANKED):
+        for hand_type in reversed(base_hand.BaseHand.ALL_HANDS_RANKED):
             hand_str = hand_type.__name__
             hand_count = winning_hand_counts.get(hand_str, 0)
             if cumulative:
                 hand_p = hand_count / (total_hands if total_hands > 0 else 1)
                 hand_p += last_cumulative_probability
                 last_cumulative_probability = hand_p
             else:
```

### Comparing `pied_poker-1.3.2/pied_poker/poker_round/poker_round_simulator.py` & `pied_poker-1.3.3/pied_poker/poker_round/poker_round_simulator.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/__init__.py` & `pied_poker-1.3.3/pied_poker/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/base_poker_event.py` & `pied_poker-1.3.3/pied_poker/probability/base_poker_event.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/__init__.py` & `pied_poker-1.3.3/pied_poker/probability/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/community_cards_include.py` & `pied_poker-1.3.3/pied_poker/probability/events/community_cards_include.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/no_tie.py` & `pied_poker-1.3.3/pied_poker/probability/events/no_tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_card_ranks.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_card_ranks.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_card_suits.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_card_suits.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_cards.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_cards.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_hand.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_hand_or_higher.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_hand_or_higher.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_pocket_pair.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_pocket_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_has_suited_cards.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_has_suited_cards.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_loses.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_loses.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_wins.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_wins.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/player_wins_with_tie.py` & `pied_poker-1.3.3/pied_poker/probability/events/player_wins_with_tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/events/tie.py` & `pied_poker-1.3.3/pied_poker/probability/events/tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/probability/probability_value.py` & `pied_poker-1.3.3/pied_poker/probability/probability_value.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/visualization/data_generator.py` & `pied_poker-1.3.3/pied_poker/visualization/data_generator.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/visualization/pocket_pairs_vs_num_players.py` & `pied_poker-1.3.3/pied_poker/visualization/pocket_pairs_vs_num_players.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker/visualization/starting_card_probabilities.py` & `pied_poker-1.3.3/pied_poker/visualization/starting_card_probabilities.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.3.2/pied_poker.egg-info/PKG-INFO` & `pied_poker-1.3.3/pied_poker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pied-poker
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package to run flexible and fast poker simulations using a monte carlo style simulator.
 Home-page: https://github.com/elleklinton/PiedPoker
 Author: Ellek Linton
 Author-email: ellek@elleklinton.com
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pied_poker-1.3.2/pied_poker.egg-info/SOURCES.txt` & `pied_poker-1.3.3/pied_poker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 pied_poker/hand/flush.py
 pied_poker/hand/four_of_a_kind.py
 pied_poker/hand/full_house.py
 pied_poker/hand/high_card.py
 pied_poker/hand/killer_card.py
 pied_poker/hand/one_pair.py
 pied_poker/hand/out.py
-pied_poker/hand/poker_hand.py
 pied_poker/hand/royal_flush.py
 pied_poker/hand/straight.py
 pied_poker/hand/straight_flush.py
 pied_poker/hand/three_of_a_kind.py
 pied_poker/hand/two_pair.py
 pied_poker/player/__init__.py
 pied_poker/player/player.py
```

### Comparing `pied_poker-1.3.2/setup.py` & `pied_poker-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name='pied_poker',
-    version='1.3.2',
+    version='1.3.3',
     description='A Python package to run flexible and fast poker simulations using a monte carlo style simulator.',
     long_description='A Python package to run flexible and fast poker simulations using a monte carlo style simulator.',
     url='https://github.com/elleklinton/PiedPoker',
     author='Ellek Linton',
     author_email='ellek@elleklinton.com',
     license='GNU LGPLv3',
     packages=['pied_poker',
```

