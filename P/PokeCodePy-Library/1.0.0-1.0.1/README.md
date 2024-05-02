# Comparing `tmp/pokecodepy_library-1.0.0.tar.gz` & `tmp/pokecodepy_library-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokecodepy_library-1.0.0.tar", last modified: Thu May  2 02:15:23 2024, max compression
+gzip compressed data, was "pokecodepy_library-1.0.1.tar", last modified: Thu May  2 03:08:19 2024, max compression
```

## Comparing `pokecodepy_library-1.0.0.tar` & `pokecodepy_library-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 02:15:23.751067 pokecodepy_library-1.0.0/
--rw-rw-rw-   0        0        0      245 2024-05-02 02:15:23.747037 pokecodepy_library-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 02:15:23.669380 pokecodepy_library-1.0.0/PokeCodePy_Library/
--rw-rw-rw-   0        0        0       43 2024-05-02 02:04:32.000000 pokecodepy_library-1.0.0/PokeCodePy_Library/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-02 02:15:11.000000 pokecodepy_library-1.0.0/PokeCodePy_Library/main.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 11:51:28.000000 pokecodepy_library-1.0.0/PokeCodePy_Library/pokemon.csv
--rw-rw-rw-   0        0        0      806 2024-05-02 02:12:24.000000 pokecodepy_library-1.0.0/PokeCodePy_Library/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:15:23.742767 pokecodepy_library-1.0.0/PokeCodePy_Library.egg-info/
--rw-rw-rw-   0        0        0      245 2024-05-02 02:15:23.000000 pokecodepy_library-1.0.0/PokeCodePy_Library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-05-02 02:15:23.000000 pokecodepy_library-1.0.0/PokeCodePy_Library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 02:15:23.000000 pokecodepy_library-1.0.0/PokeCodePy_Library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 02:15:23.000000 pokecodepy_library-1.0.0/PokeCodePy_Library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-02 02:15:23.000000 pokecodepy_library-1.0.0/PokeCodePy_Library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1017 2024-05-02 01:51:47.000000 pokecodepy_library-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 02:15:23.752152 pokecodepy_library-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      439 2024-05-02 01:47:32.000000 pokecodepy_library-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 03:08:19.587863 pokecodepy_library-1.0.1/
+-rw-rw-rw-   0        0        0      245 2024-05-02 03:08:19.585682 pokecodepy_library-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 03:08:19.512484 pokecodepy_library-1.0.1/PokeCodePy_Library/
+-rw-rw-rw-   0        0        0       43 2024-05-02 02:04:32.000000 pokecodepy_library-1.0.1/PokeCodePy_Library/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 11:51:28.000000 pokecodepy_library-1.0.1/PokeCodePy_Library/pokemon.csv
+-rw-rw-rw-   0        0        0      806 2024-05-02 02:12:24.000000 pokecodepy_library-1.0.1/PokeCodePy_Library/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-02 03:08:19.580819 pokecodepy_library-1.0.1/PokeCodePy_Library.egg-info/
+-rw-rw-rw-   0        0        0      245 2024-05-02 03:08:19.000000 pokecodepy_library-1.0.1/PokeCodePy_Library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-05-02 03:08:19.000000 pokecodepy_library-1.0.1/PokeCodePy_Library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 03:08:19.000000 pokecodepy_library-1.0.1/PokeCodePy_Library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 03:08:19.000000 pokecodepy_library-1.0.1/PokeCodePy_Library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-02 03:08:19.000000 pokecodepy_library-1.0.1/PokeCodePy_Library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1017 2024-05-02 01:51:47.000000 pokecodepy_library-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 03:08:19.588868 pokecodepy_library-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      439 2024-05-02 03:07:23.000000 pokecodepy_library-1.0.1/setup.py
```

### Comparing `pokecodepy_library-1.0.0/PokeCodePy_Library/pokemon.csv` & `pokecodepy_library-1.0.1/PokeCodePy_Library/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokecodepy_library-1.0.0/PokeCodePy_Library/random_pokemon.py` & `pokecodepy_library-1.0.1/PokeCodePy_Library/random_pokemon.py`

 * *Files identical despite different names*

### Comparing `pokecodepy_library-1.0.0/README.md` & `pokecodepy_library-1.0.1/README.md`

 * *Files identical despite different names*

