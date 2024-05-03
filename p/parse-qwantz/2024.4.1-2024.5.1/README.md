# Comparing `tmp/parse_qwantz-2024.4.1.tar.gz` & `tmp/parse_qwantz-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_qwantz-2024.4.1.tar", last modified: Tue Apr  9 19:46:59 2024, max compression
+gzip compressed data, was "parse_qwantz-2024.5.1.tar", last modified: Fri May  3 09:31:02 2024, max compression
```

## Comparing `parse_qwantz-2024.4.1.tar` & `parse_qwantz-2024.5.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-04-09 19:46:59.680179 parse_qwantz-2024.4.1/
--rw-rw-r--   0 janek     (1000) janek     (1000)     1054 2023-01-31 20:45:07.000000 parse_qwantz-2024.4.1/LICENSE
--rw-rw-r--   0 janek     (1000) janek     (1000)       83 2023-09-28 16:35:47.000000 parse_qwantz-2024.4.1/MANIFEST.in
--rw-r--r--   0 janek     (1000) janek     (1000)     4045 2024-04-09 19:46:59.680179 parse_qwantz-2024.4.1/PKG-INFO
--rw-rw-r--   0 janek     (1000) janek     (1000)     3157 2023-10-06 19:26:41.000000 parse_qwantz-2024.4.1/README.md
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-04-09 19:46:59.676179 parse_qwantz-2024.4.1/parse_qwantz/
--rw-rw-r--   0 janek     (1000) janek     (1000)       68 2023-10-02 19:10:15.000000 parse_qwantz-2024.4.1/parse_qwantz/__init__.py
--rw-rw-r--   0 janek     (1000) janek     (1000)       72 2023-01-31 20:45:07.000000 parse_qwantz-2024.4.1/parse_qwantz/__main__.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     3520 2023-08-28 21:24:27.000000 parse_qwantz-2024.4.1/parse_qwantz/box.py
--rw-rw-r--   0 janek     (1000) janek     (1000)    19650 2024-04-09 19:40:53.000000 parse_qwantz-2024.4.1/parse_qwantz/char_variants.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     2675 2023-10-31 10:18:06.000000 parse_qwantz-2024.4.1/parse_qwantz/cli.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     1198 2023-03-31 23:11:32.000000 parse_qwantz-2024.4.1/parse_qwantz/color_logs.py
--rw-rw-r--   0 janek     (1000) janek     (1000)      693 2023-10-06 19:26:31.000000 parse_qwantz-2024.4.1/parse_qwantz/colors.py
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-04-09 19:46:59.676179 parse_qwantz-2024.4.1/parse_qwantz/data/
--rw-rw-r--   0 janek     (1000) janek     (1000)   197439 2024-04-02 20:10:01.000000 parse_qwantz-2024.4.1/parse_qwantz/data/panel_overrides.json
--rw-rw-r--   0 janek     (1000) janek     (1000)     2045 2023-08-23 20:40:34.000000 parse_qwantz-2024.4.1/parse_qwantz/detect_thought.py
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-04-09 19:46:59.676179 parse_qwantz-2024.4.1/parse_qwantz/dict/
--rw-rw-r--   0 janek     (1000) janek     (1000)   190919 2023-11-01 19:17:30.000000 parse_qwantz-2024.4.1/parse_qwantz/dict/html-words.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)     4361 2024-01-10 18:08:05.000000 parse_qwantz-2024.4.1/parse_qwantz/dict/manual-additions.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       38 2023-11-01 20:59:54.000000 parse_qwantz-2024.4.1/parse_qwantz/dict/manual-removed.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)   213425 2023-11-01 19:18:11.000000 parse_qwantz-2024.4.1/parse_qwantz/dict/unambiguous-qwantz.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)     4016 2024-02-07 17:17:43.000000 parse_qwantz-2024.4.1/parse_qwantz/elements.py
--rw-rw-r--   0 janek     (1000) janek     (1000)    15671 2024-04-02 20:04:46.000000 parse_qwantz-2024.4.1/parse_qwantz/fonts.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     1849 2024-01-02 21:24:36.000000 parse_qwantz-2024.4.1/parse_qwantz/hyphens.py
--rw-rw-r--   0 janek     (1000) janek     (1000)      270 2023-08-24 19:09:24.000000 parse_qwantz-2024.4.1/parse_qwantz/image_viewer.py
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-04-09 19:46:59.680179 parse_qwantz-2024.4.1/parse_qwantz/img/
--rw-rw-r--   0 janek     (1000) janek     (1000)    15240 2023-10-10 20:29:02.000000 parse_qwantz-2024.4.1/parse_qwantz/img/ask-professor-science.svg
--rw-rw-r--   0 janek     (1000) janek     (1000)  1066287 2023-10-11 21:59:03.000000 parse_qwantz-2024.4.1/parse_qwantz/img/blank.svg
--rw-rw-r--   0 janek     (1000) janek     (1000)     1688 2023-02-11 21:19:49.000000 parse_qwantz-2024.4.1/parse_qwantz/img/italic13.png
--rw-rw-r--   0 janek     (1000) janek     (1000)    16964 2023-01-28 22:23:52.000000 parse_qwantz-2024.4.1/parse_qwantz/img/mask.png
--rw-rw-r--   0 janek     (1000) janek     (1000)     1146 2023-02-18 23:33:01.000000 parse_qwantz-2024.4.1/parse_qwantz/img/regular10.png
--rw-rw-r--   0 janek     (1000) janek     (1000)     1277 2023-02-11 21:19:49.000000 parse_qwantz-2024.4.1/parse_qwantz/img/regular11.png
--rw-rw-r--   0 janek     (1000) janek     (1000)     1360 2023-02-11 21:19:49.000000 parse_qwantz-2024.4.1/parse_qwantz/img/regular12.png
--rw-rw-r--   0 janek     (1000) janek     (1000)     1351 2024-04-02 20:04:11.000000 parse_qwantz-2024.4.1/parse_qwantz/img/regular13.png
--rw-rw-r--   0 janek     (1000) janek     (1000)      947 2023-02-11 21:19:49.000000 parse_qwantz-2024.4.1/parse_qwantz/img/regular8.png
--rw-rw-r--   0 janek     (1000) janek     (1000)      991 2024-02-26 20:14:44.000000 parse_qwantz-2024.4.1/parse_qwantz/img/regular9.png
--rw-rw-r--   0 janek     (1000) janek     (1000)     1166 2023-03-14 16:35:52.000000 parse_qwantz-2024.4.1/parse_qwantz/img/serif13.png
--rw-rw-r--   0 janek     (1000) janek     (1000)     2116 2023-10-05 19:29:23.000000 parse_qwantz-2024.4.1/parse_qwantz/lines.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     2796 2023-10-31 10:18:06.000000 parse_qwantz-2024.4.1/parse_qwantz/main.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     5758 2023-11-28 11:21:10.000000 parse_qwantz-2024.4.1/parse_qwantz/match_blocks.py
--rw-rw-r--   0 janek     (1000) janek     (1000)    18324 2024-01-19 20:38:13.000000 parse_qwantz-2024.4.1/parse_qwantz/match_lines.py
--rw-rw-r--   0 janek     (1000) janek     (1000)      557 2023-08-23 20:40:34.000000 parse_qwantz-2024.4.1/parse_qwantz/match_thought.py
--rw-rw-r--   0 janek     (1000) janek     (1000)      477 2023-03-29 21:30:27.000000 parse_qwantz-2024.4.1/parse_qwantz/panel_overrides.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     1962 2023-10-06 19:26:31.000000 parse_qwantz-2024.4.1/parse_qwantz/panels.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     9734 2024-02-27 21:37:22.000000 parse_qwantz-2024.4.1/parse_qwantz/parser.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     2458 2023-10-05 17:25:02.000000 parse_qwantz-2024.4.1/parse_qwantz/pixels.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     1755 2023-10-06 19:26:31.000000 parse_qwantz-2024.4.1/parse_qwantz/prepare_image.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     1416 2023-03-05 08:20:05.000000 parse_qwantz-2024.4.1/parse_qwantz/shape.py
--rw-rw-r--   0 janek     (1000) janek     (1000)      985 2023-10-05 18:23:15.000000 parse_qwantz-2024.4.1/parse_qwantz/simple_image.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     5206 2023-10-11 22:03:41.000000 parse_qwantz-2024.4.1/parse_qwantz/svg_gen.py
--rw-rw-r--   0 janek     (1000) janek     (1000)    11114 2024-02-24 22:37:53.000000 parse_qwantz-2024.4.1/parse_qwantz/text_blocks.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     8398 2023-10-05 19:23:42.000000 parse_qwantz-2024.4.1/parse_qwantz/text_lines.py
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-04-09 19:46:59.680179 parse_qwantz-2024.4.1/parse_qwantz.egg-info/
--rw-r--r--   0 janek     (1000) janek     (1000)     4045 2024-04-09 19:46:59.000000 parse_qwantz-2024.4.1/parse_qwantz.egg-info/PKG-INFO
--rw-rw-r--   0 janek     (1000) janek     (1000)     1482 2024-04-09 19:46:59.000000 parse_qwantz-2024.4.1/parse_qwantz.egg-info/SOURCES.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)        1 2024-04-09 19:46:59.000000 parse_qwantz-2024.4.1/parse_qwantz.egg-info/dependency_links.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       50 2024-04-09 19:46:59.000000 parse_qwantz-2024.4.1/parse_qwantz.egg-info/entry_points.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       27 2024-04-09 19:46:59.000000 parse_qwantz-2024.4.1/parse_qwantz.egg-info/requires.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       13 2024-04-09 19:46:59.000000 parse_qwantz-2024.4.1/parse_qwantz.egg-info/top_level.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)      998 2024-04-09 19:45:03.000000 parse_qwantz-2024.4.1/pyproject.toml
--rw-rw-r--   0 janek     (1000) janek     (1000)       38 2024-04-09 19:46:59.680179 parse_qwantz-2024.4.1/setup.cfg
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-05-03 09:31:02.749754 parse_qwantz-2024.5.1/
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1054 2023-01-31 20:45:07.000000 parse_qwantz-2024.5.1/LICENSE
+-rw-rw-r--   0 janek     (1000) janek     (1000)       83 2023-09-28 16:35:47.000000 parse_qwantz-2024.5.1/MANIFEST.in
+-rw-r--r--   0 janek     (1000) janek     (1000)     4045 2024-05-03 09:31:02.749754 parse_qwantz-2024.5.1/PKG-INFO
+-rw-rw-r--   0 janek     (1000) janek     (1000)     3157 2023-10-06 19:26:41.000000 parse_qwantz-2024.5.1/README.md
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-05-03 09:31:02.745753 parse_qwantz-2024.5.1/parse_qwantz/
+-rw-rw-r--   0 janek     (1000) janek     (1000)       68 2023-10-02 19:10:15.000000 parse_qwantz-2024.5.1/parse_qwantz/__init__.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)       72 2023-01-31 20:45:07.000000 parse_qwantz-2024.5.1/parse_qwantz/__main__.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     3520 2023-08-28 21:24:27.000000 parse_qwantz-2024.5.1/parse_qwantz/box.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)    19650 2024-04-09 19:40:53.000000 parse_qwantz-2024.5.1/parse_qwantz/char_variants.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     2675 2023-10-31 10:18:06.000000 parse_qwantz-2024.5.1/parse_qwantz/cli.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1198 2023-03-31 23:11:32.000000 parse_qwantz-2024.5.1/parse_qwantz/color_logs.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)      693 2023-10-06 19:26:31.000000 parse_qwantz-2024.5.1/parse_qwantz/colors.py
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-05-03 09:31:02.745753 parse_qwantz-2024.5.1/parse_qwantz/data/
+-rw-rw-r--   0 janek     (1000) janek     (1000)   196912 2024-05-03 09:28:02.000000 parse_qwantz-2024.5.1/parse_qwantz/data/panel_overrides.json
+-rw-rw-r--   0 janek     (1000) janek     (1000)     2045 2023-08-23 20:40:34.000000 parse_qwantz-2024.5.1/parse_qwantz/detect_thought.py
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-05-03 09:31:02.745753 parse_qwantz-2024.5.1/parse_qwantz/dict/
+-rw-rw-r--   0 janek     (1000) janek     (1000)   190919 2023-11-01 19:17:30.000000 parse_qwantz-2024.5.1/parse_qwantz/dict/html-words.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)     4361 2024-01-10 18:08:05.000000 parse_qwantz-2024.5.1/parse_qwantz/dict/manual-additions.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       38 2023-11-01 20:59:54.000000 parse_qwantz-2024.5.1/parse_qwantz/dict/manual-removed.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)   213425 2023-11-01 19:18:11.000000 parse_qwantz-2024.5.1/parse_qwantz/dict/unambiguous-qwantz.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)     4016 2024-02-07 17:17:43.000000 parse_qwantz-2024.5.1/parse_qwantz/elements.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)    15671 2024-04-02 20:04:46.000000 parse_qwantz-2024.5.1/parse_qwantz/fonts.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1849 2024-01-02 21:24:36.000000 parse_qwantz-2024.5.1/parse_qwantz/hyphens.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)      270 2023-08-24 19:09:24.000000 parse_qwantz-2024.5.1/parse_qwantz/image_viewer.py
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-05-03 09:31:02.749754 parse_qwantz-2024.5.1/parse_qwantz/img/
+-rw-rw-r--   0 janek     (1000) janek     (1000)    15240 2023-10-10 20:29:02.000000 parse_qwantz-2024.5.1/parse_qwantz/img/ask-professor-science.svg
+-rw-rw-r--   0 janek     (1000) janek     (1000)  1066287 2023-10-11 21:59:03.000000 parse_qwantz-2024.5.1/parse_qwantz/img/blank.svg
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1688 2023-02-11 21:19:49.000000 parse_qwantz-2024.5.1/parse_qwantz/img/italic13.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)    16964 2023-01-28 22:23:52.000000 parse_qwantz-2024.5.1/parse_qwantz/img/mask.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1146 2023-02-18 23:33:01.000000 parse_qwantz-2024.5.1/parse_qwantz/img/regular10.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1277 2023-02-11 21:19:49.000000 parse_qwantz-2024.5.1/parse_qwantz/img/regular11.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1360 2023-02-11 21:19:49.000000 parse_qwantz-2024.5.1/parse_qwantz/img/regular12.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1351 2024-04-02 20:04:11.000000 parse_qwantz-2024.5.1/parse_qwantz/img/regular13.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)      947 2023-02-11 21:19:49.000000 parse_qwantz-2024.5.1/parse_qwantz/img/regular8.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)      991 2024-02-26 20:14:44.000000 parse_qwantz-2024.5.1/parse_qwantz/img/regular9.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1166 2023-03-14 16:35:52.000000 parse_qwantz-2024.5.1/parse_qwantz/img/serif13.png
+-rw-rw-r--   0 janek     (1000) janek     (1000)     2116 2023-10-05 19:29:23.000000 parse_qwantz-2024.5.1/parse_qwantz/lines.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     2796 2023-10-31 10:18:06.000000 parse_qwantz-2024.5.1/parse_qwantz/main.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     5758 2023-11-28 11:21:10.000000 parse_qwantz-2024.5.1/parse_qwantz/match_blocks.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)    18324 2024-01-19 20:38:13.000000 parse_qwantz-2024.5.1/parse_qwantz/match_lines.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)      557 2023-08-23 20:40:34.000000 parse_qwantz-2024.5.1/parse_qwantz/match_thought.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)      477 2023-03-29 21:30:27.000000 parse_qwantz-2024.5.1/parse_qwantz/panel_overrides.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1962 2023-10-06 19:26:31.000000 parse_qwantz-2024.5.1/parse_qwantz/panels.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     9734 2024-02-27 21:37:22.000000 parse_qwantz-2024.5.1/parse_qwantz/parser.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     2458 2023-10-05 17:25:02.000000 parse_qwantz-2024.5.1/parse_qwantz/pixels.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1755 2023-10-06 19:26:31.000000 parse_qwantz-2024.5.1/parse_qwantz/prepare_image.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1416 2023-03-05 08:20:05.000000 parse_qwantz-2024.5.1/parse_qwantz/shape.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)      985 2023-10-05 18:23:15.000000 parse_qwantz-2024.5.1/parse_qwantz/simple_image.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     5206 2023-10-11 22:03:41.000000 parse_qwantz-2024.5.1/parse_qwantz/svg_gen.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)    11114 2024-02-24 22:37:53.000000 parse_qwantz-2024.5.1/parse_qwantz/text_blocks.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     8398 2023-10-05 19:23:42.000000 parse_qwantz-2024.5.1/parse_qwantz/text_lines.py
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-05-03 09:31:02.749754 parse_qwantz-2024.5.1/parse_qwantz.egg-info/
+-rw-r--r--   0 janek     (1000) janek     (1000)     4045 2024-05-03 09:31:02.000000 parse_qwantz-2024.5.1/parse_qwantz.egg-info/PKG-INFO
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1482 2024-05-03 09:31:02.000000 parse_qwantz-2024.5.1/parse_qwantz.egg-info/SOURCES.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)        1 2024-05-03 09:31:02.000000 parse_qwantz-2024.5.1/parse_qwantz.egg-info/dependency_links.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       50 2024-05-03 09:31:02.000000 parse_qwantz-2024.5.1/parse_qwantz.egg-info/entry_points.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       27 2024-05-03 09:31:02.000000 parse_qwantz-2024.5.1/parse_qwantz.egg-info/requires.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       13 2024-05-03 09:31:02.000000 parse_qwantz-2024.5.1/parse_qwantz.egg-info/top_level.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)      998 2024-05-03 09:30:12.000000 parse_qwantz-2024.5.1/pyproject.toml
+-rw-rw-r--   0 janek     (1000) janek     (1000)       38 2024-05-03 09:31:02.749754 parse_qwantz-2024.5.1/setup.cfg
```

### Comparing `parse_qwantz-2024.4.1/LICENSE` & `parse_qwantz-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/PKG-INFO` & `parse_qwantz-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_qwantz
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Transcript generator for Dinosaur Comics
 Author-email: Jan Szejko <jan.szejko@gmail.com>
 Project-URL: homepage, https://github.com/janek37/parse_qwantz
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `parse_qwantz-2024.4.1/README.md` & `parse_qwantz-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/box.py` & `parse_qwantz-2024.5.1/parse_qwantz/box.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/char_variants.py` & `parse_qwantz-2024.5.1/parse_qwantz/char_variants.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/cli.py` & `parse_qwantz-2024.5.1/parse_qwantz/cli.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/color_logs.py` & `parse_qwantz-2024.5.1/parse_qwantz/color_logs.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/colors.py` & `parse_qwantz-2024.5.1/parse_qwantz/colors.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/data/panel_overrides.json` & `parse_qwantz-2024.5.1/parse_qwantz/data/panel_overrides.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9919786096256684%*

 * *Differences: {"'cc8ed6d551a36f086d490bf4bfc750aa'": "OrderedDict([('comic_id', 2656), ('file_name', "*

 * *                                       "'comic2-2666.png'), ('panels', OrderedDict([('2', "*

 * *                                       "['Narrator: BUT THAT NIGHT:', 'Off panel: ▹rrrring "*

 * *                                       "rrrrrring◃', 'T-Rex: WHAAAAAAAT']), ('6', ['Narrator: THAT "*

 * *                                       "NIGHT:', 'Off panel: ▹bzzzzzzzzzzzzzzzzzzzzzzzzzzz◃', "*

 * *                                       "' […]*

```diff
@@ -2979,24 +2979,14 @@
             "6": [
                 "English: PLEASE NOTE THAT WHEN DESCRIBING A MEAL OR OTHER ELEMENT RELATED TO HOSPITALITY, NONE OF THESE WORDS APPLY AND YOU MUST INSTEAD USE THE PHRASE \"FIT FOR A KING\".",
                 "T-Rex: ...",
                 "T-Rex: ...I hereby RETIRE FROM WORDS"
             ]
         }
     },
-    "9423cfde3a675c2c7c81f748e5e41e30": {
-        "comic_id": 359,
-        "file_name": "comic2-379.png",
-        "panels": {
-            "3": [
-                "T-Rex: All of the functions are there: e\u02e3, \u03c0r\u00b2, i\u00b2, even some old-school guys like abs(x). Anyway, poor e\u02e3 is alone in a corner, acting all morose. His good friend 2\u02e3 comes over and says, \u201cWhat's the problem? Come on, integrate yourself into the party!\u201d And e\u02e3 looks at him and he says, \u201cWhy? It's not going to make a difference!\u201d",
-                "T-Rex: Hah hah!"
-            ]
-        }
-    },
     "94633aa9d294ad409952628e8d9fba77": {
         "comic_id": 368,
         "file_name": "comic2-400.png",
         "panels": {
             "2": [
                 "T-Rex: ...things would be different!",
                 "T-Rex: \u301astarts daydreaming\u301b"
@@ -4210,14 +4200,31 @@
             "6": [
                 "Movie poster: THE \u25d6GUY\u25d7 WHO KEPT TAKING \u25d6BITES\u25d7 OUT OF \u25d6ANIMALS\u25d7",
                 "Movie poster: Once In a Lifetime Comes a Movie (In The German Expressionist Tradition) In Which A Dinosaur Takes Cartoony Bites out of Cows and Then Tries to Avoid Punishment for That.\u2122",
                 "Movie poster: \u201c\u25d6BITINGLY\u25d7 hilarious!\u201d --Everyone??"
             ]
         }
     },
+    "cc8ed6d551a36f086d490bf4bfc750aa": {
+        "comic_id": 2656,
+        "file_name": "comic2-2666.png",
+        "panels": {
+            "2": [
+                "Narrator: BUT THAT NIGHT:",
+                "Off panel: \u25b9rrrring rrrrrring\u25c3",
+                "T-Rex: WHAAAAAAAT"
+            ],
+            "6": [
+                "Narrator: THAT NIGHT:",
+                "Off panel: \u25b9bzzzzzzzzzzzzzzzzzzzzzzzzzzz\u25c3",
+                "T-Rex: Oh wow, the ghost of my noisy CPU fan that died fifteen years ago!",
+                "T-Rex: The afterlife sure is awesome and definitely not full of garbage at all!!"
+            ]
+        }
+    },
     "ce0dcb22e51bd95ce96e2967a95dc435": {
         "comic_id": 3101,
         "file_name": "comic2-3106.png",
         "panels": {
             "6": [
                 "Banner: BEING A BACHELOR IS EASY",
                 "T-Rex: As hunting and gathering was dominant for over 90% of our history, odds are we've ALREADY solved your housekeeping problem!",
@@ -4429,31 +4436,14 @@
             "6": [
                 "Narrator: TELEPATHIC HOTTIE CHAT:",
                 "T-Rex: \u301athinks\u301b Hey baby do u like to kiss on dudes?? bc IM A DUDE",
                 "T-Rex: \u301athinks in a different font\u301b SEND TO: all hotties / REGIONS: all / FLAGS: important, must-read, NOT A JOKE"
             ]
         }
     },
-    "d7e1efc131d8b6294412112269623126": {
-        "comic_id": 2656,
-        "file_name": "comic2-2666.png",
-        "panels": {
-            "2": [
-                "Narrator: BUT THAT NIGHT:",
-                "Off panel: \u25b9rrrring rrrrrring\u25c3",
-                "T-Rex: WHAAAAAAAT"
-            ],
-            "6": [
-                "Narrator: THAT NIGHT:",
-                "Off panel: \u25b9bzzzzzzzzzzzzzzzzzzzzzzzzzzz\u25c3",
-                "T-Rex: Oh wow, the ghost of my noisy CPU fan that died fifteen years ago!",
-                "T-Rex: The afterlife sure is awesome and definitely not full of garbage at all!!"
-            ]
-        }
-    },
     "d84fd25b92cce70472dac22eeb6d6455": {
         "comic_id": 952,
         "file_name": "comic2-984.png",
         "panels": {
             "6": [
                 "Off panel: Well look at YOU, Mr. \"I write a book about a tugboat that employs superseded scientific theories for locomotion\"!",
                 "T-Rex: Yes! Look at me! at me and buy my story and find out if Tuggy saves us all!",
```

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/detect_thought.py` & `parse_qwantz-2024.5.1/parse_qwantz/detect_thought.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/dict/html-words.txt` & `parse_qwantz-2024.5.1/parse_qwantz/dict/html-words.txt`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/dict/manual-additions.txt` & `parse_qwantz-2024.5.1/parse_qwantz/dict/manual-additions.txt`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/dict/unambiguous-qwantz.txt` & `parse_qwantz-2024.5.1/parse_qwantz/dict/unambiguous-qwantz.txt`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/elements.py` & `parse_qwantz-2024.5.1/parse_qwantz/elements.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/fonts.py` & `parse_qwantz-2024.5.1/parse_qwantz/fonts.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/hyphens.py` & `parse_qwantz-2024.5.1/parse_qwantz/hyphens.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/ask-professor-science.svg` & `parse_qwantz-2024.5.1/parse_qwantz/img/ask-professor-science.svg`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/blank.svg` & `parse_qwantz-2024.5.1/parse_qwantz/img/blank.svg`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/italic13.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/italic13.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/mask.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/mask.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/regular10.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/regular10.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/regular11.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/regular11.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/regular12.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/regular12.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/regular13.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/regular13.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/regular8.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/regular8.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/regular9.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/regular9.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/img/serif13.png` & `parse_qwantz-2024.5.1/parse_qwantz/img/serif13.png`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/lines.py` & `parse_qwantz-2024.5.1/parse_qwantz/lines.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/main.py` & `parse_qwantz-2024.5.1/parse_qwantz/main.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/match_blocks.py` & `parse_qwantz-2024.5.1/parse_qwantz/match_blocks.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/match_lines.py` & `parse_qwantz-2024.5.1/parse_qwantz/match_lines.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/match_thought.py` & `parse_qwantz-2024.5.1/parse_qwantz/match_thought.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/panels.py` & `parse_qwantz-2024.5.1/parse_qwantz/panels.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/parser.py` & `parse_qwantz-2024.5.1/parse_qwantz/parser.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/pixels.py` & `parse_qwantz-2024.5.1/parse_qwantz/pixels.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/prepare_image.py` & `parse_qwantz-2024.5.1/parse_qwantz/prepare_image.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/shape.py` & `parse_qwantz-2024.5.1/parse_qwantz/shape.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/simple_image.py` & `parse_qwantz-2024.5.1/parse_qwantz/simple_image.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/svg_gen.py` & `parse_qwantz-2024.5.1/parse_qwantz/svg_gen.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/text_blocks.py` & `parse_qwantz-2024.5.1/parse_qwantz/text_blocks.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz/text_lines.py` & `parse_qwantz-2024.5.1/parse_qwantz/text_lines.py`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/parse_qwantz.egg-info/PKG-INFO` & `parse_qwantz-2024.5.1/parse_qwantz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_qwantz
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Transcript generator for Dinosaur Comics
 Author-email: Jan Szejko <jan.szejko@gmail.com>
 Project-URL: homepage, https://github.com/janek37/parse_qwantz
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `parse_qwantz-2024.4.1/parse_qwantz.egg-info/SOURCES.txt` & `parse_qwantz-2024.5.1/parse_qwantz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parse_qwantz-2024.4.1/pyproject.toml` & `parse_qwantz-2024.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "parse_qwantz"
 authors = [{name = "Jan Szejko", email = "jan.szejko@gmail.com"}]
-version = "2024.4.1"
+version = "2024.5.1"
 description = "Transcript generator for Dinosaur Comics"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
     "Environment :: Console",
```

