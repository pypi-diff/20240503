# Comparing `tmp/starrailcard-2.1.6.tar.gz` & `tmp/starrailcard-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.6.tar", last modified: Mon Apr 29 22:39:02 2024, max compression
+gzip compressed data, was "starrailcard-2.1.7.tar", last modified: Fri May  3 21:39:14 2024, max compression
```

## Comparing `starrailcard-2.1.6.tar` & `starrailcard-2.1.7.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.966995 starrailcard-2.1.6/
--rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.1.6/LICENSE
--rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4744 2024-04-29 22:39:02.966995 starrailcard-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.1.6/README.md
--rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 22:39:02.966995 starrailcard-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1544 2024-04-29 22:37:14.000000 starrailcard-2.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.927251 starrailcard-2.1.6/starrailcard/
--rw-rw-rw-   0        0        0     1963 2024-04-29 22:38:56.000000 starrailcard-2.1.6/starrailcard/__init__.py
--rw-rw-rw-   0        0        0    12335 2024-04-29 22:25:47.000000 starrailcard-2.1.6/starrailcard/client.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.920894 starrailcard-2.1.6/starrailcard/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.942269 starrailcard-2.1.6/starrailcard/src/api/
--rw-rw-rw-   0        0        0     2761 2024-04-29 21:42:26.000000 starrailcard-2.1.6/starrailcard/src/api/api.py
--rw-rw-rw-   0        0        0     3487 2024-04-14 22:43:00.000000 starrailcard-2.1.6/starrailcard/src/api/enka.py
--rw-rw-rw-   0        0        0    25187 2024-04-14 22:52:21.000000 starrailcard-2.1.6/starrailcard/src/api/enka_parsed.py
--rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.1.6/starrailcard/src/api/error.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.920894 starrailcard-2.1.6/starrailcard/src/assets/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.942269 starrailcard-2.1.6/starrailcard/src/assets/font/
--rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.1.6/starrailcard/src/assets/font/font_hsr.ttf
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.948270 starrailcard-2.1.6/starrailcard/src/data/
--rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/avatar.json
--rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/element.json
--rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/keys.json
--rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/paths.json
--rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/relict_sets.json
--rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/stats.json
--rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.1.6/starrailcard/src/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.949269 starrailcard-2.1.6/starrailcard/src/generator/
--rw-rw-rw-   0        0        0     6662 2024-04-20 04:28:23.000000 starrailcard-2.1.6/starrailcard/src/generator/style_profile_phone.py
--rw-rw-rw-   0        0        0    24567 2024-04-17 16:11:52.000000 starrailcard-2.1.6/starrailcard/src/generator/style_relict_score.py
--rw-rw-rw-   0        0        0    30356 2024-04-17 16:11:41.000000 starrailcard-2.1.6/starrailcard/src/generator/style_ticket.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.952782 starrailcard-2.1.6/starrailcard/src/model/
--rw-rw-rw-   0        0        0     4759 2024-04-13 14:26:08.000000 starrailcard-2.1.6/starrailcard/src/model/StarRailCard.py
--rw-rw-rw-   0        0        0    11769 2024-04-14 20:59:53.000000 starrailcard-2.1.6/starrailcard/src/model/api_mihomo.py
--rw-rw-rw-   0        0        0     4065 2024-03-13 13:47:58.000000 starrailcard-2.1.6/starrailcard/src/model/style.py
--rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.1.6/starrailcard/src/model/ukrainization_model.py
--rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.1.6/starrailcard/src/model/utils_model.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.957780 starrailcard-2.1.6/starrailcard/src/tools/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.958779 starrailcard-2.1.6/starrailcard/src/tools/calculator/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.958779 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.960779 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/
--rw-rw-rw-   0        0        0      373 2024-04-06 18:51:59.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/max.json
--rw-rw-rw-   0        0        0       49 2024-04-06 18:52:00.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-rw-rw-   0        0        0     3434 2024-04-06 18:52:00.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-rw-rw-   0        0        0    92881 2024-04-06 18:52:01.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/score.json
--rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/src/utils.py
--rw-rw-rw-   0        0        0     5747 2024-04-01 14:16:17.000000 starrailcard-2.1.6/starrailcard/src/tools/calculator/stats.py
--rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.1.6/starrailcard/src/tools/cashe.py
--rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.1.6/starrailcard/src/tools/enums.py
--rw-rw-rw-   0        0        0    10136 2024-02-23 21:20:24.000000 starrailcard-2.1.6/starrailcard/src/tools/git.py
--rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.1.6/starrailcard/src/tools/http.py
--rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.1.6/starrailcard/src/tools/json_data.py
--rw-rw-rw-   0        0        0     7017 2024-04-29 22:06:20.000000 starrailcard-2.1.6/starrailcard/src/tools/options.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.964995 starrailcard-2.1.6/starrailcard/src/tools/pill/
--rw-rw-rw-   0        0        0      199 2024-04-29 21:26:56.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/__init__.py
--rw-rw-rw-   0        0        0     3854 2024-02-22 12:55:07.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/color.py
--rw-rw-rw-   0        0        0     2330 2024-02-22 13:03:49.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/color_controle.py
--rw-rw-rw-   0        0        0     5518 2024-02-25 12:31:53.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/grandiend_v2.py
--rw-rw-rw-   0        0        0     3284 2024-02-22 12:55:28.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/grandient_v1.py
--rw-rw-rw-   0        0        0     5534 2024-04-29 22:03:56.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/image_controle.py
--rw-rw-rw-   0        0        0     5106 2024-02-22 12:55:59.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/style_editor.py
--rw-rw-rw-   0        0        0     2116 2024-02-22 13:01:14.000000 starrailcard-2.1.6/starrailcard/src/tools/pill/text_controle.py
--rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.1.6/starrailcard/src/tools/translator.py
--rw-rw-rw-   0        0        0     6585 2024-02-22 12:57:06.000000 starrailcard-2.1.6/starrailcard/src/tools/treePaths.py
--rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.1.6/starrailcard/src/tools/ukrainization.py
--rw-rw-rw-   0        0        0     6884 2024-03-18 20:19:11.000000 starrailcard-2.1.6/starrailcard/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:39:02.965995 starrailcard-2.1.6/starrailcard.egg-info/
--rw-rw-rw-   0        0        0     4744 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2011 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 22:39:02.000000 starrailcard-2.1.6/starrailcard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.979988 starrailcard-2.1.7/
+-rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4744 2024-05-03 21:39:14.978983 starrailcard-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.1.7/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:39:14.979988 starrailcard-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2024-04-29 22:37:14.000000 starrailcard-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.728308 starrailcard-2.1.7/starrailcard/
+-rw-rw-rw-   0        0        0     1967 2024-05-03 21:36:05.000000 starrailcard-2.1.7/starrailcard/__init__.py
+-rw-rw-rw-   0        0        0    12335 2024-04-29 22:25:47.000000 starrailcard-2.1.7/starrailcard/client.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.701592 starrailcard-2.1.7/starrailcard/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.771493 starrailcard-2.1.7/starrailcard/src/api/
+-rw-rw-rw-   0        0        0     2761 2024-04-29 21:42:26.000000 starrailcard-2.1.7/starrailcard/src/api/api.py
+-rw-rw-rw-   0        0        0     3487 2024-04-14 22:43:00.000000 starrailcard-2.1.7/starrailcard/src/api/enka.py
+-rw-rw-rw-   0        0        0    25187 2024-04-14 22:52:21.000000 starrailcard-2.1.7/starrailcard/src/api/enka_parsed.py
+-rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.1.7/starrailcard/src/api/error.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.700592 starrailcard-2.1.7/starrailcard/src/assets/
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.776744 starrailcard-2.1.7/starrailcard/src/assets/font/
+-rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.1.7/starrailcard/src/assets/font/font_hsr.ttf
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.807021 starrailcard-2.1.7/starrailcard/src/data/
+-rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/avatar.json
+-rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/element.json
+-rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/keys.json
+-rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/paths.json
+-rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/relict_sets.json
+-rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/stats.json
+-rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.1.7/starrailcard/src/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.822253 starrailcard-2.1.7/starrailcard/src/generator/
+-rw-rw-rw-   0        0        0     6662 2024-04-20 04:28:23.000000 starrailcard-2.1.7/starrailcard/src/generator/style_profile_phone.py
+-rw-rw-rw-   0        0        0    24567 2024-04-17 16:11:52.000000 starrailcard-2.1.7/starrailcard/src/generator/style_relict_score.py
+-rw-rw-rw-   0        0        0    30356 2024-04-17 16:11:41.000000 starrailcard-2.1.7/starrailcard/src/generator/style_ticket.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.853301 starrailcard-2.1.7/starrailcard/src/model/
+-rw-rw-rw-   0        0        0     4759 2024-04-13 14:26:08.000000 starrailcard-2.1.7/starrailcard/src/model/StarRailCard.py
+-rw-rw-rw-   0        0        0    12254 2024-05-03 18:03:39.000000 starrailcard-2.1.7/starrailcard/src/model/api_mihomo.py
+-rw-rw-rw-   0        0        0     4065 2024-03-13 13:47:58.000000 starrailcard-2.1.7/starrailcard/src/model/style.py
+-rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.1.7/starrailcard/src/model/ukrainization_model.py
+-rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.1.7/starrailcard/src/model/utils_model.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.898082 starrailcard-2.1.7/starrailcard/src/tools/
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.903716 starrailcard-2.1.7/starrailcard/src/tools/calculator/
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.908219 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.928892 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/
+-rw-rw-rw-   0        0        0      373 2024-04-06 18:51:59.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-rw-rw-   0        0        0       49 2024-04-06 18:52:00.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-rw-rw-   0        0        0     3434 2024-04-06 18:52:00.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-rw-rw-   0        0        0    92881 2024-04-06 18:52:01.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/src/utils.py
+-rw-rw-rw-   0        0        0     5802 2024-05-03 21:15:03.000000 starrailcard-2.1.7/starrailcard/src/tools/calculator/stats.py
+-rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.1.7/starrailcard/src/tools/cashe.py
+-rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.1.7/starrailcard/src/tools/enums.py
+-rw-rw-rw-   0        0        0    10136 2024-02-23 21:20:24.000000 starrailcard-2.1.7/starrailcard/src/tools/git.py
+-rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.1.7/starrailcard/src/tools/http.py
+-rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.1.7/starrailcard/src/tools/json_data.py
+-rw-rw-rw-   0        0        0     7017 2024-04-29 22:06:20.000000 starrailcard-2.1.7/starrailcard/src/tools/options.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.977480 starrailcard-2.1.7/starrailcard/src/tools/pill/
+-rw-rw-rw-   0        0        0      224 2024-05-03 21:37:45.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/__init__.py
+-rw-rw-rw-   0        0        0     3854 2024-02-22 12:55:07.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/color.py
+-rw-rw-rw-   0        0        0     2330 2024-02-22 13:03:49.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/color_controle.py
+-rw-rw-rw-   0        0        0     5367 2024-05-03 18:29:29.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/diagrama.py
+-rw-rw-rw-   0        0        0     5518 2024-02-25 12:31:53.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/grandiend_v2.py
+-rw-rw-rw-   0        0        0     3284 2024-02-22 12:55:28.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/grandient_v1.py
+-rw-rw-rw-   0        0        0     5534 2024-04-29 22:03:56.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/image_controle.py
+-rw-rw-rw-   0        0        0     5106 2024-02-22 12:55:59.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/style_editor.py
+-rw-rw-rw-   0        0        0     2116 2024-02-22 13:01:14.000000 starrailcard-2.1.7/starrailcard/src/tools/pill/text_controle.py
+-rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.1.7/starrailcard/src/tools/translator.py
+-rw-rw-rw-   0        0        0     6585 2024-02-22 12:57:06.000000 starrailcard-2.1.7/starrailcard/src/tools/treePaths.py
+-rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.1.7/starrailcard/src/tools/ukrainization.py
+-rw-rw-rw-   0        0        0     6884 2024-03-18 20:19:11.000000 starrailcard-2.1.7/starrailcard/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:39:14.977480 starrailcard-2.1.7/starrailcard.egg-info/
+-rw-rw-rw-   0        0        0     4744 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2051 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 21:39:14.000000 starrailcard-2.1.7/starrailcard.egg-info/top_level.txt
```

### Comparing `starrailcard-2.1.6/LICENSE` & `starrailcard-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/PKG-INFO` & `starrailcard-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.6
+Version: 2.1.7
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `starrailcard-2.1.6/README.md` & `starrailcard-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/pyproject.toml` & `starrailcard-2.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/setup.py` & `starrailcard-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/__init__.py` & `starrailcard-2.1.7/starrailcard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 __title__ = 'StarRailCard.py'
 __author__ = 'DeviantUa'
-__version__ = '2.1.6'
+__version__ = '2.1.7'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 from .client import *
 from .utils import *
-from .src.tools.enums import *
+from .src.tools.enums import *
+
```

### Comparing `starrailcard-2.1.6/starrailcard/client.py` & `starrailcard-2.1.7/starrailcard/client.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/api/api.py` & `starrailcard-2.1.7/starrailcard/src/api/api.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/api/enka.py` & `starrailcard-2.1.7/starrailcard/src/api/enka.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/api/enka_parsed.py` & `starrailcard-2.1.7/starrailcard/src/api/enka_parsed.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.1.7/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/data/avatar.json` & `starrailcard-2.1.7/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/data/relict_sets.json` & `starrailcard-2.1.7/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/data/stats.json` & `starrailcard-2.1.7/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/data/weapons.json` & `starrailcard-2.1.7/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.1.7/starrailcard/src/generator/style_profile_phone.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.1.7/starrailcard/src/generator/style_relict_score.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.1.7/starrailcard/src/generator/style_ticket.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.1.7/starrailcard/src/model/StarRailCard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.1.7/starrailcard/src/model/api_mihomo.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,14 +246,31 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #self.icon = MAIN_LINK.format(icon = self.icon)
 
         if UA_LANG:
             self.name = TranslateDataManager._data.stats.get(self.field, self.name)
             
+class CharacterProperties(BaseModel):
+    type: Optional[str]
+    field: Optional[str]
+    name: Optional[str]
+    icon: Optional[str]
+    value: float
+    display: Optional[str]
+    percent: bool
+    
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        #self.icon = MAIN_LINK.format(icon = self.icon)
+
+        if UA_LANG:
+            self.name = TranslateDataManager._data.stats.get(self.field, self.name)            
+
+        
 class Character(BaseModel):
     id: Optional[str]
     name: Optional[str]
     rarity: int
     rank: int
     level: int
     promotion: int
@@ -266,15 +283,15 @@
     skills: List[Skill]
     skill_trees: List[SkillTree]
     light_cone: Optional[LightCone]
     relics: Optional[List[Relic]]
     relic_sets: Optional[List[RelicSet]]
     attributes: List[CharacterAttributes]
     additions: List[CharacterAttributes]
-    properties: Optional[List[CharacterAttributes]]
+    properties: Optional[List[CharacterProperties]]
     pos: list
     
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #self.icon = MAIN_LINK.format(icon = self.icon)
         #self.preview = MAIN_LINK.format(icon = self.preview)
         #self.portrait = MAIN_LINK.format(icon = self.portrait)
```

### Comparing `starrailcard-2.1.6/starrailcard/src/model/style.py` & `starrailcard-2.1.7/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/model/utils_model.py` & `starrailcard-2.1.7/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.1.7/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.1.7/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.1.7/starrailcard/src/tools/calculator/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,17 @@
             self.result["total_score"]["count"] += self.result["score"][key]["count"]
         
         self.result["total_score"]["count"] = round(self.result["total_score"]["count"] /2, 1)
         self.result["total_score"]["rank"] = {"name": utils.get_relic_full_score_text(self.result["total_score"]["count"]), "color": utils.get_total_score_color(self.result["total_score"]["count"])}
          
         return self.result
 
-        
+    async def get_score(self):
+        return self.score
+    
     async def update_score(self, charter_id = None):
         
         for key in _PATH_FILE_NAME:
             if key == "score":
                 data = await get_score(_LINK_SCORE)
                 if not charter_id is None:
                     if data.get(str(charter_id)) is None:
```

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/cashe.py` & `starrailcard-2.1.7/starrailcard/src/tools/cashe.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/enums.py` & `starrailcard-2.1.7/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/git.py` & `starrailcard-2.1.7/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/http.py` & `starrailcard-2.1.7/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/json_data.py` & `starrailcard-2.1.7/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/options.py` & `starrailcard-2.1.7/starrailcard/src/tools/options.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/color.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/color_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/grandiend_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/image_controle.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/image_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.1.7/starrailcard/src/tools/pill/text_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/translator.py` & `starrailcard-2.1.7/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/treePaths.py` & `starrailcard-2.1.7/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.1.7/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard/utils.py` & `starrailcard-2.1.7/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.6/starrailcard.egg-info/PKG-INFO` & `starrailcard-2.1.7/starrailcard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.6
+Version: 2.1.7
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `starrailcard-2.1.6/starrailcard.egg-info/SOURCES.txt` & `starrailcard-2.1.7/starrailcard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,13 @@
 starrailcard/src/tools/calculator/src/assets/max.json
 starrailcard/src/tools/calculator/src/assets/relic_id.json
 starrailcard/src/tools/calculator/src/assets/rolls.json
 starrailcard/src/tools/calculator/src/assets/score.json
 starrailcard/src/tools/pill/__init__.py
 starrailcard/src/tools/pill/color.py
 starrailcard/src/tools/pill/color_controle.py
+starrailcard/src/tools/pill/diagrama.py
 starrailcard/src/tools/pill/grandiend_v2.py
 starrailcard/src/tools/pill/grandient_v1.py
 starrailcard/src/tools/pill/image_controle.py
 starrailcard/src/tools/pill/style_editor.py
 starrailcard/src/tools/pill/text_controle.py
```

