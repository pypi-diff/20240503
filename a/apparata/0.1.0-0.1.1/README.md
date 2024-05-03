# Comparing `tmp/apparata-0.1.0.tar.gz` & `tmp/apparata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apparata-0.1.0.tar", last modified: Fri May  3 16:28:59 2024, max compression
+gzip compressed data, was "apparata-0.1.1.tar", last modified: Fri May  3 17:31:58 2024, max compression
```

## Comparing `apparata-0.1.0.tar` & `apparata-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nishantgerald   (501) staff       (20)        0 2024-05-03 16:28:59.264848 apparata-0.1.0/
--rw-r--r--   0 nishantgerald   (501) staff       (20)      183 2024-05-03 16:28:59.264678 apparata-0.1.0/PKG-INFO
--rw-r--r--   0 nishantgerald   (501) staff       (20)      917 2024-05-03 03:44:25.000000 apparata-0.1.0/README.md
-drwxr-xr-x   0 nishantgerald   (501) staff       (20)        0 2024-05-03 16:28:59.263614 apparata-0.1.0/apparata/
--rw-r--r--   0 nishantgerald   (501) staff       (20)       24 2024-05-03 16:15:25.000000 apparata-0.1.0/apparata/__init__.py
--rw-r--r--   0 nishantgerald   (501) staff       (20)     3042 2024-05-03 16:19:23.000000 apparata-0.1.0/apparata/apparata.py
-drwxr-xr-x   0 nishantgerald   (501) staff       (20)        0 2024-05-03 16:28:59.264472 apparata-0.1.0/apparata.egg-info/
--rw-r--r--   0 nishantgerald   (501) staff       (20)      183 2024-05-03 16:28:59.000000 apparata-0.1.0/apparata.egg-info/PKG-INFO
--rw-r--r--   0 nishantgerald   (501) staff       (20)      219 2024-05-03 16:28:59.000000 apparata-0.1.0/apparata.egg-info/SOURCES.txt
--rw-r--r--   0 nishantgerald   (501) staff       (20)        1 2024-05-03 16:28:59.000000 apparata-0.1.0/apparata.egg-info/dependency_links.txt
--rw-r--r--   0 nishantgerald   (501) staff       (20)       13 2024-05-03 16:28:59.000000 apparata-0.1.0/apparata.egg-info/requires.txt
--rw-r--r--   0 nishantgerald   (501) staff       (20)        9 2024-05-03 16:28:59.000000 apparata-0.1.0/apparata.egg-info/top_level.txt
--rw-r--r--   0 nishantgerald   (501) staff       (20)       38 2024-05-03 16:28:59.264904 apparata-0.1.0/setup.cfg
--rw-r--r--   0 nishantgerald   (501) staff       (20)      302 2024-05-03 16:23:25.000000 apparata-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:31:58.450625 apparata-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-03 17:31:58.450625 apparata-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-03 17:31:54.000000 apparata-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:31:58.450625 apparata-0.1.1/apparata/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 17:31:54.000000 apparata-0.1.1/apparata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-03 17:31:54.000000 apparata-0.1.1/apparata/apparata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:31:58.450625 apparata-0.1.1/apparata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-03 17:31:58.000000 apparata-0.1.1/apparata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-03 17:31:58.000000 apparata-0.1.1/apparata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:31:58.000000 apparata-0.1.1/apparata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 17:31:58.000000 apparata-0.1.1/apparata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 17:31:58.000000 apparata-0.1.1/apparata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:31:58.450625 apparata-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 17:31:54.000000 apparata-0.1.1/setup.py
```

### Comparing `apparata-0.1.0/README.md` & `apparata-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,21 @@
 * Last names
 * Addresses
 * Phone numbers
 * Datetimes
 * Emails
 * Latitudes and longitudes
 
+## How to Install Apparata
+```bash
+pip install apparata
+```
+
 ## How to Use Apparata
 
 To use Apparata, simply import the script into your Python program and call the desired function. For example, to generate a random number with 10 digits, you would use the following code:
 
 ```python
 import apparata
 
 number = apparata.generate_numbers(10)
 ```
-
```

### Comparing `apparata-0.1.0/apparata/apparata.py` & `apparata-0.1.1/apparata/apparata.py`

 * *Files identical despite different names*

