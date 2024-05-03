# Comparing `tmp/bigluo-0.1.0.tar.gz` & `tmp/bigluo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigluo-0.1.0.tar", last modified: Fri May  3 17:28:27 2024, max compression
+gzip compressed data, was "bigluo-0.1.1.tar", last modified: Fri May  3 17:29:02 2024, max compression
```

## Comparing `bigluo-0.1.0.tar` & `bigluo-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rnthking   (501) staff       (20)        0 2024-05-03 17:28:27.637969 bigluo-0.1.0/
--rw-r--r--   0 rnthking   (501) staff       (20)       50 2024-05-03 17:28:27.637747 bigluo-0.1.0/PKG-INFO
--rw-r--r--   0 rnthking   (501) staff       (20)       59 2024-05-03 17:17:58.000000 bigluo-0.1.0/README.md
-drwxr-xr-x   0 rnthking   (501) staff       (20)        0 2024-05-03 17:28:27.636577 bigluo-0.1.0/bgtest/
--rw-r--r--   0 rnthking   (501) staff       (20)       24 2024-05-03 17:19:43.000000 bigluo-0.1.0/bgtest/__init__.py
--rw-r--r--   0 rnthking   (501) staff       (20)       55 2024-05-03 17:18:49.000000 bigluo-0.1.0/bgtest/main.py
-drwxr-xr-x   0 rnthking   (501) staff       (20)        0 2024-05-03 17:28:27.637526 bigluo-0.1.0/bigluo.egg-info/
--rw-r--r--   0 rnthking   (501) staff       (20)       50 2024-05-03 17:28:27.000000 bigluo-0.1.0/bigluo.egg-info/PKG-INFO
--rw-r--r--   0 rnthking   (501) staff       (20)      205 2024-05-03 17:28:27.000000 bigluo-0.1.0/bigluo.egg-info/SOURCES.txt
--rw-r--r--   0 rnthking   (501) staff       (20)        1 2024-05-03 17:28:27.000000 bigluo-0.1.0/bigluo.egg-info/dependency_links.txt
--rw-r--r--   0 rnthking   (501) staff       (20)       40 2024-05-03 17:28:27.000000 bigluo-0.1.0/bigluo.egg-info/entry_points.txt
--rw-r--r--   0 rnthking   (501) staff       (20)        7 2024-05-03 17:28:27.000000 bigluo-0.1.0/bigluo.egg-info/top_level.txt
--rw-r--r--   0 rnthking   (501) staff       (20)       38 2024-05-03 17:28:27.638013 bigluo-0.1.0/setup.cfg
--rw-r--r--   0 rnthking   (501) staff       (20)      339 2024-05-03 17:28:09.000000 bigluo-0.1.0/setup.py
+drwxr-xr-x   0 rnthking   (501) staff       (20)        0 2024-05-03 17:29:02.506993 bigluo-0.1.1/
+-rw-r--r--   0 rnthking   (501) staff       (20)       50 2024-05-03 17:29:02.506744 bigluo-0.1.1/PKG-INFO
+-rw-r--r--   0 rnthking   (501) staff       (20)       59 2024-05-03 17:17:58.000000 bigluo-0.1.1/README.md
+drwxr-xr-x   0 rnthking   (501) staff       (20)        0 2024-05-03 17:29:02.505267 bigluo-0.1.1/bgtest/
+-rw-r--r--   0 rnthking   (501) staff       (20)       24 2024-05-03 17:19:43.000000 bigluo-0.1.1/bgtest/__init__.py
+-rw-r--r--   0 rnthking   (501) staff       (20)       55 2024-05-03 17:18:49.000000 bigluo-0.1.1/bgtest/main.py
+drwxr-xr-x   0 rnthking   (501) staff       (20)        0 2024-05-03 17:29:02.506523 bigluo-0.1.1/bigluo.egg-info/
+-rw-r--r--   0 rnthking   (501) staff       (20)       50 2024-05-03 17:29:02.000000 bigluo-0.1.1/bigluo.egg-info/PKG-INFO
+-rw-r--r--   0 rnthking   (501) staff       (20)      205 2024-05-03 17:29:02.000000 bigluo-0.1.1/bigluo.egg-info/SOURCES.txt
+-rw-r--r--   0 rnthking   (501) staff       (20)        1 2024-05-03 17:29:02.000000 bigluo-0.1.1/bigluo.egg-info/dependency_links.txt
+-rw-r--r--   0 rnthking   (501) staff       (20)       40 2024-05-03 17:29:02.000000 bigluo-0.1.1/bigluo.egg-info/entry_points.txt
+-rw-r--r--   0 rnthking   (501) staff       (20)        7 2024-05-03 17:29:02.000000 bigluo-0.1.1/bigluo.egg-info/top_level.txt
+-rw-r--r--   0 rnthking   (501) staff       (20)       38 2024-05-03 17:29:02.507052 bigluo-0.1.1/setup.cfg
+-rw-r--r--   0 rnthking   (501) staff       (20)      339 2024-05-03 17:29:00.000000 bigluo-0.1.1/setup.py
```

