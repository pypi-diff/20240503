# Comparing `tmp/armenian_latin_to_armenian_hy-0.0.2.tar.gz` & `tmp/armenian_latin_to_armenian_hy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armenian_latin_to_armenian_hy-0.0.2.tar", last modified: Thu May  2 23:46:39 2024, max compression
+gzip compressed data, was "armenian_latin_to_armenian_hy-0.0.3.tar", last modified: Fri May  3 18:24:19 2024, max compression
```

## Comparing `armenian_latin_to_armenian_hy-0.0.2.tar` & `armenian_latin_to_armenian_hy-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 haykeminyan   (501) staff       (20)        0 2024-05-02 23:46:39.626385 armenian_latin_to_armenian_hy-0.0.2/
--rw-r--r--   0 haykeminyan   (501) staff       (20)      516 2024-05-02 23:46:39.626162 armenian_latin_to_armenian_hy-0.0.2/PKG-INFO
--rw-r--r--   0 haykeminyan   (501) staff       (20)      166 2024-05-02 23:19:50.000000 armenian_latin_to_armenian_hy-0.0.2/README.md
-drwxr-xr-x   0 haykeminyan   (501) staff       (20)        0 2024-05-02 23:46:39.625988 armenian_latin_to_armenian_hy-0.0.2/armenian_latin_to_armenian_hy.egg-info/
--rw-r--r--   0 haykeminyan   (501) staff       (20)      516 2024-05-02 23:46:39.000000 armenian_latin_to_armenian_hy-0.0.2/armenian_latin_to_armenian_hy.egg-info/PKG-INFO
--rw-r--r--   0 haykeminyan   (501) staff       (20)      256 2024-05-02 23:46:39.000000 armenian_latin_to_armenian_hy-0.0.2/armenian_latin_to_armenian_hy.egg-info/SOURCES.txt
--rw-r--r--   0 haykeminyan   (501) staff       (20)        1 2024-05-02 23:46:39.000000 armenian_latin_to_armenian_hy-0.0.2/armenian_latin_to_armenian_hy.egg-info/dependency_links.txt
--rw-r--r--   0 haykeminyan   (501) staff       (20)       53 2024-05-02 23:46:39.000000 armenian_latin_to_armenian_hy-0.0.2/armenian_latin_to_armenian_hy.egg-info/top_level.txt
--rw-r--r--   0 haykeminyan   (501) staff       (20)    16942 2024-05-02 22:22:06.000000 armenian_latin_to_armenian_hy-0.0.2/armenian_transliterate.py
--rw-r--r--   0 haykeminyan   (501) staff       (20)       38 2024-05-02 23:46:39.626426 armenian_latin_to_armenian_hy-0.0.2/setup.cfg
--rw-r--r--   0 haykeminyan   (501) staff       (20)      594 2024-05-02 23:43:26.000000 armenian_latin_to_armenian_hy-0.0.2/setup.py
+drwxr-xr-x   0 haykeminyan   (501) staff       (20)        0 2024-05-03 18:24:19.447313 armenian_latin_to_armenian_hy-0.0.3/
+-rw-r--r--   0 haykeminyan   (501) staff       (20)      671 2024-05-03 18:24:19.447085 armenian_latin_to_armenian_hy-0.0.3/PKG-INFO
+-rw-r--r--   0 haykeminyan   (501) staff       (20)      321 2024-05-03 18:24:12.000000 armenian_latin_to_armenian_hy-0.0.3/README.md
+drwxr-xr-x   0 haykeminyan   (501) staff       (20)        0 2024-05-03 18:24:19.446680 armenian_latin_to_armenian_hy-0.0.3/armenian_latin_to_armenian_hy.egg-info/
+-rw-r--r--   0 haykeminyan   (501) staff       (20)      671 2024-05-03 18:24:19.000000 armenian_latin_to_armenian_hy-0.0.3/armenian_latin_to_armenian_hy.egg-info/PKG-INFO
+-rw-r--r--   0 haykeminyan   (501) staff       (20)      256 2024-05-03 18:24:19.000000 armenian_latin_to_armenian_hy-0.0.3/armenian_latin_to_armenian_hy.egg-info/SOURCES.txt
+-rw-r--r--   0 haykeminyan   (501) staff       (20)        1 2024-05-03 18:24:19.000000 armenian_latin_to_armenian_hy-0.0.3/armenian_latin_to_armenian_hy.egg-info/dependency_links.txt
+-rw-r--r--   0 haykeminyan   (501) staff       (20)       53 2024-05-03 18:24:19.000000 armenian_latin_to_armenian_hy-0.0.3/armenian_latin_to_armenian_hy.egg-info/top_level.txt
+-rw-r--r--   0 haykeminyan   (501) staff       (20)    17500 2024-05-03 18:22:20.000000 armenian_latin_to_armenian_hy-0.0.3/armenian_transliterate.py
+-rw-r--r--   0 haykeminyan   (501) staff       (20)       38 2024-05-03 18:24:19.447361 armenian_latin_to_armenian_hy-0.0.3/setup.cfg
+-rw-r--r--   0 haykeminyan   (501) staff       (20)      594 2024-05-03 18:24:12.000000 armenian_latin_to_armenian_hy-0.0.3/setup.py
```

### Comparing `armenian_latin_to_armenian_hy-0.0.2/setup.py` & `armenian_latin_to_armenian_hy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md') as file:
 	description = file.read()
 
 
 setup(
 	name="armenian_latin_to_armenian_hy",
-	version="0.0.2",
+	version="0.0.3",
 	description="Transliteration from Latin Armenian language to Armenian",
 	py_modules=["armenian_latin_to_armenian_hy", "armenian_transliterate"],
 	packages=find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
```

