# Comparing `tmp/comic-parser-0.0.2.tar.gz` & `tmp/comic_parser-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comic-parser-0.0.2.tar", last modified: Fri Apr 12 11:54:57 2024, max compression
+gzip compressed data, was "comic_parser-1.0.tar", last modified: Fri May  3 08:17:25 2024, max compression
```

## Comparing `comic-parser-0.0.2.tar` & `comic_parser-1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.856152 comic-parser-0.0.2/
--rw-rw-rw-   0        0        0     1095 2024-04-08 12:22:08.000000 comic-parser-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1757 2024-04-12 11:54:57.854158 comic-parser-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-30 08:39:04.000000 comic-parser-0.0.2/README.md
--rw-rw-rw-   0        0        0      735 2024-04-12 11:54:28.000000 comic-parser-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 11:54:57.856152 comic-parser-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.812222 comic-parser-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.823373 comic-parser-0.0.2/src/comicParser/
--rw-rw-rw-   0        0        0      153 2024-04-12 11:20:55.000000 comic-parser-0.0.2/src/comicParser/__init__.py
--rw-rw-rw-   0        0        0      784 2024-04-12 11:40:37.000000 comic-parser-0.0.2/src/comicParser/comicParser.py
-drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.851959 comic-parser-0.0.2/src/comic_parser.egg-info/
--rw-rw-rw-   0        0        0     1757 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 08:17:25.084686 comic_parser-1.0/
+-rw-rw-rw-   0        0        0     1095 2024-04-08 12:22:08.000000 comic_parser-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      706 2024-05-03 08:17:25.081694 comic_parser-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-30 08:39:04.000000 comic_parser-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 08:17:25.050776 comic_parser-1.0/comicParser/
+-rw-rw-rw-   0        0        0      141 2024-05-03 08:14:03.000000 comic_parser-1.0/comicParser/__init__.py
+-rw-rw-rw-   0        0        0     3429 2024-05-03 08:14:03.000000 comic_parser-1.0/comicParser/comicParser.py
+-rw-rw-rw-   0        0        0       82 2024-05-03 08:14:03.000000 comic_parser-1.0/comicParser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:17:25.079699 comic_parser-1.0/comic_parser.egg-info/
+-rw-rw-rw-   0        0        0      706 2024-05-03 08:17:24.000000 comic_parser-1.0/comic_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-03 08:17:25.000000 comic_parser-1.0/comic_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 08:17:24.000000 comic_parser-1.0/comic_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-03 08:17:24.000000 comic_parser-1.0/comic_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 08:17:24.000000 comic_parser-1.0/comic_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-05-03 08:17:24.000000 comic_parser-1.0/comic_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-03 08:17:24.000000 comic_parser-1.0/comic_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 08:17:25.084686 comic_parser-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1514 2024-05-03 08:17:02.000000 comic_parser-1.0/setup.py
```

### Comparing `comic-parser-0.0.2/LICENSE.txt` & `comic_parser-1.0/LICENSE.txt`

 * *Files identical despite different names*

