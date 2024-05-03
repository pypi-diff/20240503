# Comparing `tmp/mypypi9-0.7.8.tar.gz` & `tmp/mypypi9-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypypi9-0.7.8.tar", last modified: Sat Apr 27 06:21:56 2024, max compression
+gzip compressed data, was "mypypi9-0.7.9.tar", last modified: Sat Apr 27 06:24:47 2024, max compression
```

## Comparing `mypypi9-0.7.8.tar` & `mypypi9-0.7.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 06:21:56.017000 mypypi9-0.7.8/
--rw-rw-rw-   0        0        0     1088 2022-08-26 12:36:15.000000 mypypi9-0.7.8/LICENSE
--rw-rw-rw-   0        0        0      416 2024-04-27 06:21:56.001000 mypypi9-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0       28 2022-08-26 12:36:16.000000 mypypi9-0.7.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 06:21:55.900000 mypypi9-0.7.8/myPYPI9/
--rw-rw-rw-   0        0        0       42 2024-03-21 02:09:48.000000 mypypi9-0.7.8/myPYPI9/__init__.py
--rw-rw-rw-   0        0        0      836 2022-08-26 12:36:32.000000 mypypi9-0.7.8/myPYPI9/prime_numbers.py
--rw-rw-rw-   0        0        0      836 2023-04-05 18:18:42.000000 mypypi9-0.7.8/myPYPI9/prime_numbersNew.py
-drwxrwxrwx   0        0        0        0 2024-04-27 06:21:55.991000 mypypi9-0.7.8/myPYPI9.egg-info/
--rw-rw-rw-   0        0        0      416 2024-04-27 06:21:55.000000 mypypi9-0.7.8/myPYPI9.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-27 06:21:55.000000 mypypi9-0.7.8/myPYPI9.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 06:21:55.000000 mypypi9-0.7.8/myPYPI9.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 06:21:55.000000 mypypi9-0.7.8/myPYPI9.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 06:21:56.015000 mypypi9-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-04-27 06:05:19.000000 mypypi9-0.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 06:21:55.972000 mypypi9-0.7.8/tests/
--rw-rw-rw-   0        0        0      179 2024-03-21 02:10:56.000000 mypypi9-0.7.8/tests/test_prime.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:24:47.086000 mypypi9-0.7.9/
+-rw-rw-rw-   0        0        0     1088 2022-08-26 12:36:15.000000 mypypi9-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-04-27 06:24:47.071000 mypypi9-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2022-08-26 12:36:16.000000 mypypi9-0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 06:24:46.960000 mypypi9-0.7.9/myPYPI9/
+-rw-rw-rw-   0        0        0       42 2024-03-21 02:09:48.000000 mypypi9-0.7.9/myPYPI9/__init__.py
+-rw-rw-rw-   0        0        0      836 2022-08-26 12:36:32.000000 mypypi9-0.7.9/myPYPI9/prime_numbers.py
+-rw-rw-rw-   0        0        0      836 2023-04-05 18:18:42.000000 mypypi9-0.7.9/myPYPI9/prime_numbersNew.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:24:47.062000 mypypi9-0.7.9/myPYPI9.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-04-27 06:24:46.000000 mypypi9-0.7.9/myPYPI9.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-27 06:24:46.000000 mypypi9-0.7.9/myPYPI9.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 06:24:46.000000 mypypi9-0.7.9/myPYPI9.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 06:24:46.000000 mypypi9-0.7.9/myPYPI9.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-27 06:24:47.084000 mypypi9-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-04-27 06:24:37.000000 mypypi9-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 06:24:47.043000 mypypi9-0.7.9/tests/
+-rw-rw-rw-   0        0        0      179 2024-03-21 02:10:56.000000 mypypi9-0.7.9/tests/test_prime.py
```

### Comparing `mypypi9-0.7.8/LICENSE` & `mypypi9-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypypi9-0.7.8/myPYPI9/prime_numbers.py` & `mypypi9-0.7.9/myPYPI9/prime_numbers.py`

 * *Files identical despite different names*

### Comparing `mypypi9-0.7.8/myPYPI9/prime_numbersNew.py` & `mypypi9-0.7.9/myPYPI9/prime_numbersNew.py`

 * *Files identical despite different names*

### Comparing `mypypi9-0.7.8/setup.py` & `mypypi9-0.7.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="myPYPI9", #package name Replace with your own username
-    version="0.7.8",
+    version="0.7.9",
     author="spacenet2300",
     author_email="endersu@outlook.com",
     description="Create A small package to work with prime numbers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/clement-bonnet/medium-first-package",
     # url="https://github.com/myNKUST/myprimelib9b.git",
```

