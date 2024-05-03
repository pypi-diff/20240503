# Comparing `tmp/random_file_generator-0.0.1.tar.gz` & `tmp/random_file_generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random_file_generator-0.0.1.tar", last modified: Fri May  3 10:38:05 2024, max compression
+gzip compressed data, was "random_file_generator-0.0.2.tar", last modified: Fri May  3 10:41:45 2024, max compression
```

## Comparing `random_file_generator-0.0.1.tar` & `random_file_generator-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nishithkashyap   (501) staff       (20)        0 2024-05-03 10:38:05.827415 random_file_generator-0.0.1/
--rw-r--r--   0 nishithkashyap   (501) staff       (20)     1071 2024-05-03 09:49:56.000000 random_file_generator-0.0.1/LICENSE
--rw-r--r--   0 nishithkashyap   (501) staff       (20)      293 2024-05-03 10:38:05.826479 random_file_generator-0.0.1/PKG-INFO
--rw-r--r--   0 nishithkashyap   (501) staff       (20)      832 2024-05-03 10:15:41.000000 random_file_generator-0.0.1/README.md
-drwxr-xr-x   0 nishithkashyap   (501) staff       (20)        0 2024-05-03 10:38:05.823686 random_file_generator-0.0.1/random-file-generator/
--rw-r--r--   0 nishithkashyap   (501) staff       (20)     1151 2024-05-03 10:12:01.000000 random_file_generator-0.0.1/random-file-generator/__init__.py
-drwxr-xr-x   0 nishithkashyap   (501) staff       (20)        0 2024-05-03 10:38:05.825712 random_file_generator-0.0.1/random_file_generator.egg-info/
--rw-r--r--   0 nishithkashyap   (501) staff       (20)      293 2024-05-03 10:38:05.000000 random_file_generator-0.0.1/random_file_generator.egg-info/PKG-INFO
--rw-r--r--   0 nishithkashyap   (501) staff       (20)      240 2024-05-03 10:38:05.000000 random_file_generator-0.0.1/random_file_generator.egg-info/SOURCES.txt
--rw-r--r--   0 nishithkashyap   (501) staff       (20)        1 2024-05-03 10:38:05.000000 random_file_generator-0.0.1/random_file_generator.egg-info/dependency_links.txt
--rw-r--r--   0 nishithkashyap   (501) staff       (20)       22 2024-05-03 10:38:05.000000 random_file_generator-0.0.1/random_file_generator.egg-info/top_level.txt
--rw-r--r--   0 nishithkashyap   (501) staff       (20)       38 2024-05-03 10:38:05.827604 random_file_generator-0.0.1/setup.cfg
--rw-r--r--   0 nishithkashyap   (501) staff       (20)      408 2024-05-03 10:35:45.000000 random_file_generator-0.0.1/setup.py
+drwxr-xr-x   0 nishithkashyap   (501) staff       (20)        0 2024-05-03 10:41:45.867927 random_file_generator-0.0.2/
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)     1071 2024-05-03 09:49:56.000000 random_file_generator-0.0.2/LICENSE
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)     1167 2024-05-03 10:41:45.867435 random_file_generator-0.0.2/PKG-INFO
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)      832 2024-05-03 10:15:41.000000 random_file_generator-0.0.2/README.md
+drwxr-xr-x   0 nishithkashyap   (501) staff       (20)        0 2024-05-03 10:41:45.865274 random_file_generator-0.0.2/random-file-generator/
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)     1151 2024-05-03 10:12:01.000000 random_file_generator-0.0.2/random-file-generator/__init__.py
+drwxr-xr-x   0 nishithkashyap   (501) staff       (20)        0 2024-05-03 10:41:45.866852 random_file_generator-0.0.2/random_file_generator.egg-info/
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)     1167 2024-05-03 10:41:45.000000 random_file_generator-0.0.2/random_file_generator.egg-info/PKG-INFO
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)      240 2024-05-03 10:41:45.000000 random_file_generator-0.0.2/random_file_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)        1 2024-05-03 10:41:45.000000 random_file_generator-0.0.2/random_file_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)       22 2024-05-03 10:41:45.000000 random_file_generator-0.0.2/random_file_generator.egg-info/top_level.txt
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)       38 2024-05-03 10:41:45.868074 random_file_generator-0.0.2/setup.cfg
+-rw-r--r--   0 nishithkashyap   (501) staff       (20)      566 2024-05-03 10:40:30.000000 random_file_generator-0.0.2/setup.py
```

### Comparing `random_file_generator-0.0.1/LICENSE` & `random_file_generator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `random_file_generator-0.0.1/README.md` & `random_file_generator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `random_file_generator-0.0.1/random-file-generator/__init__.py` & `random_file_generator-0.0.2/random-file-generator/__init__.py`

 * *Files identical despite different names*

