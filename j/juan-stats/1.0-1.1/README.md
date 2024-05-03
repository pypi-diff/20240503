# Comparing `tmp/juan-stats-1.0.tar.gz` & `tmp/juan_stats-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juan-stats-1.0.tar", last modified: Fri May  3 04:58:56 2024, max compression
+gzip compressed data, was "juan_stats-1.1.tar", last modified: Fri May  3 05:41:37 2024, max compression
```

## Comparing `juan-stats-1.0.tar` & `juan_stats-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 04:58:56.427305 juan-stats-1.0/
--rw-rw-rw-   0        0        0      163 2024-05-03 04:58:56.426305 juan-stats-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 04:58:56.417927 juan-stats-1.0/juan-stats/
--rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan-stats-1.0/juan-stats/Binomialdistribution.py
--rw-rw-rw-   0        0        0     3800 2024-05-03 04:52:53.000000 juan-stats-1.0/juan-stats/Gaussiandistribution.py
--rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan-stats-1.0/juan-stats/Generaldistribution.py
--rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan-stats-1.0/juan-stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 04:58:56.425299 juan-stats-1.0/juan_stats.egg-info/
--rw-rw-rw-   0        0        0      163 2024-05-03 04:58:56.000000 juan-stats-1.0/juan_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-03 04:58:56.000000 juan-stats-1.0/juan_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 04:58:56.000000 juan-stats-1.0/juan_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-03 04:58:56.000000 juan-stats-1.0/juan_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-03 04:58:56.000000 juan-stats-1.0/juan_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 04:58:56.427305 juan-stats-1.0/setup.cfg
--rw-rw-rw-   0        0        0      255 2024-05-03 04:58:49.000000 juan-stats-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:41:37.544866 juan_stats-1.1/
+-rw-rw-rw-   0        0        0      163 2024-05-03 05:41:37.543859 juan_stats-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 05:41:37.533479 juan_stats-1.1/juan_stats/
+-rw-rw-rw-   0        0        0     4851 2024-05-03 04:52:53.000000 juan_stats-1.1/juan_stats/Binomialdistribution.py
+-rw-rw-rw-   0        0        0     3800 2024-05-03 04:52:53.000000 juan_stats-1.1/juan_stats/Gaussiandistribution.py
+-rw-rw-rw-   0        0        0      953 2024-05-03 04:52:53.000000 juan_stats-1.1/juan_stats/Generaldistribution.py
+-rw-rw-rw-   0        0        0       88 2024-05-03 04:52:53.000000 juan_stats-1.1/juan_stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:41:37.541945 juan_stats-1.1/juan_stats.egg-info/
+-rw-rw-rw-   0        0        0      163 2024-05-03 05:41:37.000000 juan_stats-1.1/juan_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-03 05:41:37.000000 juan_stats-1.1/juan_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 05:41:37.000000 juan_stats-1.1/juan_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-03 04:58:56.000000 juan_stats-1.1/juan_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-03 05:41:37.000000 juan_stats-1.1/juan_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 05:41:37.544866 juan_stats-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      255 2024-05-03 05:40:42.000000 juan_stats-1.1/setup.py
```

### Comparing `juan-stats-1.0/juan-stats/Binomialdistribution.py` & `juan_stats-1.1/juan_stats/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `juan-stats-1.0/juan-stats/Gaussiandistribution.py` & `juan_stats-1.1/juan_stats/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `juan-stats-1.0/juan-stats/Generaldistribution.py` & `juan_stats-1.1/juan_stats/Generaldistribution.py`

 * *Files identical despite different names*

