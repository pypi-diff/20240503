# Comparing `tmp/vcmtools-0.1.tar.gz` & `tmp/vcmtools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcmtools-0.1.tar", last modified: Fri May  3 07:47:32 2024, max compression
+gzip compressed data, was "vcmtools-0.2.tar", last modified: Fri May  3 09:06:03 2024, max compression
```

## Comparing `vcmtools-0.1.tar` & `vcmtools-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 07:47:32.546085 vcmtools-0.1/
--rw-rw-rw-   0        0        0     1085 2024-04-19 14:35:49.000000 vcmtools-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       80 2024-05-03 07:47:32.546085 vcmtools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1793 2024-04-19 17:30:32.000000 vcmtools-0.1/README.rst
--rw-rw-rw-   0        0        0        0 2024-04-19 15:13:18.000000 vcmtools-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 07:47:32.546085 vcmtools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      161 2024-05-03 07:45:13.000000 vcmtools-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:47:32.530474 vcmtools-0.1/vcmtools/
--rw-rw-rw-   0        0        0        0 2024-04-19 18:02:56.000000 vcmtools-0.1/vcmtools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 07:47:32.530474 vcmtools-0.1/vcmtools.egg-info/
--rw-rw-rw-   0        0        0       80 2024-05-03 07:47:32.000000 vcmtools-0.1/vcmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-03 07:47:32.000000 vcmtools-0.1/vcmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 07:47:32.000000 vcmtools-0.1/vcmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 07:47:32.000000 vcmtools-0.1/vcmtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 09:06:03.439600 vcmtools-0.2/
+-rw-rw-rw-   0        0        0     1085 2024-04-19 14:35:49.000000 vcmtools-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       80 2024-05-03 09:06:03.439600 vcmtools-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1793 2024-04-19 17:30:32.000000 vcmtools-0.2/README.rst
+-rw-rw-rw-   0        0        0        0 2024-04-19 15:13:18.000000 vcmtools-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 09:06:03.439600 vcmtools-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      161 2024-05-03 09:05:54.000000 vcmtools-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:06:03.398507 vcmtools-0.2/vcmtools/
+-rw-rw-rw-   0        0        0        0 2024-04-19 18:02:56.000000 vcmtools-0.2/vcmtools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 09:06:03.398507 vcmtools-0.2/vcmtools.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-05-03 09:06:03.000000 vcmtools-0.2/vcmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-03 09:06:03.000000 vcmtools-0.2/vcmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 09:06:03.000000 vcmtools-0.2/vcmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 09:06:03.000000 vcmtools-0.2/vcmtools.egg-info/top_level.txt
```

### Comparing `vcmtools-0.1/LICENSE.txt` & `vcmtools-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vcmtools-0.1/README.rst` & `vcmtools-0.2/README.rst`

 * *Files identical despite different names*

