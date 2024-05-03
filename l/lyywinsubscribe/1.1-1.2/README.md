# Comparing `tmp/lyywinsubscribe-1.1.tar.gz` & `tmp/lyywinsubscribe-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyywinsubscribe-1.1.tar", last modified: Fri May  3 15:41:49 2024, max compression
+gzip compressed data, was "lyywinsubscribe-1.2.tar", last modified: Fri May  3 15:42:44 2024, max compression
```

## Comparing `lyywinsubscribe-1.1.tar` & `lyywinsubscribe-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:41:49.806611 lyywinsubscribe-1.1/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyywinsubscribe-1.1/LICENSE
--rw-rw-rw-   0        0        0      152 2024-05-03 15:41:49.806611 lyywinsubscribe-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyywinsubscribe-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 15:41:49.805607 lyywinsubscribe-1.1/lyywinsubscribe.egg-info/
--rw-rw-rw-   0        0        0      152 2024-05-03 15:41:49.000000 lyywinsubscribe-1.1/lyywinsubscribe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-03 15:41:49.000000 lyywinsubscribe-1.1/lyywinsubscribe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:41:49.000000 lyywinsubscribe-1.1/lyywinsubscribe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 15:41:49.000000 lyywinsubscribe-1.1/lyywinsubscribe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-03 15:41:49.000000 lyywinsubscribe-1.1/lyywinsubscribe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1343 2024-05-02 12:53:18.000000 lyywinsubscribe-1.1/lyywinsubscribe.py
--rw-rw-rw-   0        0        0       42 2024-05-03 15:41:49.806611 lyywinsubscribe-1.1/setup.cfg
--rw-rw-rw-   0        0        0      277 2024-05-03 15:41:48.000000 lyywinsubscribe-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:42:44.827267 lyywinsubscribe-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyywinsubscribe-1.2/LICENSE
+-rw-rw-rw-   0        0        0      152 2024-05-03 15:42:44.826251 lyywinsubscribe-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyywinsubscribe-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:42:44.825249 lyywinsubscribe-1.2/lyywinsubscribe.egg-info/
+-rw-rw-rw-   0        0        0      152 2024-05-03 15:42:44.000000 lyywinsubscribe-1.2/lyywinsubscribe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-03 15:42:44.000000 lyywinsubscribe-1.2/lyywinsubscribe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:42:44.000000 lyywinsubscribe-1.2/lyywinsubscribe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 15:42:44.000000 lyywinsubscribe-1.2/lyywinsubscribe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-03 15:42:44.000000 lyywinsubscribe-1.2/lyywinsubscribe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10162 2024-05-03 15:42:30.000000 lyywinsubscribe-1.2/lyywinsubscribe.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:42:44.827267 lyywinsubscribe-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      277 2024-05-03 15:42:43.000000 lyywinsubscribe-1.2/setup.py
```

### Comparing `lyywinsubscribe-1.1/LICENSE` & `lyywinsubscribe-1.2/LICENSE`

 * *Files identical despite different names*

