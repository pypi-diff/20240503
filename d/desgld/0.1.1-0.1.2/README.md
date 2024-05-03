# Comparing `tmp/desgld-0.1.1.tar.gz` & `tmp/desgld-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desgld-0.1.1.tar", last modified: Mon Apr 29 23:03:37 2024, max compression
+gzip compressed data, was "desgld-0.1.2.tar", last modified: Fri May  3 02:02:19 2024, max compression
```

## Comparing `desgld-0.1.1.tar` & `desgld-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-04-29 23:03:37.443501 desgld-0.1.1/
--rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.1/LICENSE
--rw-r--r--   0 macpc      (501) staff       (20)      504 2024-04-29 23:03:37.443205 desgld-0.1.1/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.1/README.md
--rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.1/pyproject.toml
--rw-r--r--   0 macpc      (501) staff       (20)       38 2024-04-29 23:03:37.443550 desgld-0.1.1/setup.cfg
--rw-r--r--   0 macpc      (501) staff       (20)      618 2024-04-29 23:03:04.000000 desgld-0.1.1/setup.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-04-29 23:03:37.440045 desgld-0.1.1/src/
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-04-29 23:03:37.441715 desgld-0.1.1/src/desgld/
--rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.1/src/desgld/__init__.py
--rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-04-29 21:40:38.000000 desgld-0.1.1/src/desgld/desgld_alg.py
--rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-04-29 20:32:35.000000 desgld-0.1.1/src/desgld/evaluation.py
--rw-r--r--   0 macpc      (501) staff       (20)     4185 2024-04-29 20:32:35.000000 desgld-0.1.1/src/desgld/network.py
-drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-04-29 23:03:37.442773 desgld-0.1.1/src/desgld.egg-info/
--rw-r--r--   0 macpc      (501) staff       (20)      504 2024-04-29 23:03:37.000000 desgld-0.1.1/src/desgld.egg-info/PKG-INFO
--rw-r--r--   0 macpc      (501) staff       (20)      305 2024-04-29 23:03:37.000000 desgld-0.1.1/src/desgld.egg-info/SOURCES.txt
--rw-r--r--   0 macpc      (501) staff       (20)        1 2024-04-29 23:03:37.000000 desgld-0.1.1/src/desgld.egg-info/dependency_links.txt
--rw-r--r--   0 macpc      (501) staff       (20)       78 2024-04-29 23:03:37.000000 desgld-0.1.1/src/desgld.egg-info/requires.txt
--rw-r--r--   0 macpc      (501) staff       (20)        7 2024-04-29 23:03:37.000000 desgld-0.1.1/src/desgld.egg-info/top_level.txt
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.345304 desgld-0.1.2/
+-rw-r--r--   0 macpc      (501) staff       (20)     1079 2024-04-29 20:32:35.000000 desgld-0.1.2/LICENSE
+-rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 02:02:19.344982 desgld-0.1.2/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      228 2024-04-29 22:08:43.000000 desgld-0.1.2/README.md
+-rw-r--r--   0 macpc      (501) staff       (20)       79 2024-04-29 20:32:35.000000 desgld-0.1.2/pyproject.toml
+-rw-r--r--   0 macpc      (501) staff       (20)       38 2024-05-03 02:02:19.345365 desgld-0.1.2/setup.cfg
+-rw-r--r--   0 macpc      (501) staff       (20)      708 2024-05-03 02:01:04.000000 desgld-0.1.2/setup.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.341569 desgld-0.1.2/src/
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.343384 desgld-0.1.2/src/desgld/
+-rw-r--r--   0 macpc      (501) staff       (20)      273 2024-04-29 20:32:35.000000 desgld-0.1.2/src/desgld/__init__.py
+-rw-r--r--   0 macpc      (501) staff       (20)    11597 2024-04-29 21:40:38.000000 desgld-0.1.2/src/desgld/desgld_alg.py
+-rw-r--r--   0 macpc      (501) staff       (20)     5454 2024-04-29 20:32:35.000000 desgld-0.1.2/src/desgld/evaluation.py
+-rw-r--r--   0 macpc      (501) staff       (20)     8050 2024-05-02 23:28:18.000000 desgld-0.1.2/src/desgld/network.py
+drwxr-xr-x   0 macpc      (501) staff       (20)        0 2024-05-03 02:02:19.344473 desgld-0.1.2/src/desgld.egg-info/
+-rw-r--r--   0 macpc      (501) staff       (20)      773 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/PKG-INFO
+-rw-r--r--   0 macpc      (501) staff       (20)      305 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/SOURCES.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        1 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/dependency_links.txt
+-rw-r--r--   0 macpc      (501) staff       (20)       78 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/requires.txt
+-rw-r--r--   0 macpc      (501) staff       (20)        7 2024-05-03 02:02:19.000000 desgld-0.1.2/src/desgld.egg-info/top_level.txt
```

### Comparing `desgld-0.1.1/LICENSE` & `desgld-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `desgld-0.1.1/setup.py` & `desgld-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 requirements_dev = ["black", "isort", "flake8", "pre-commit"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="desgld",
-    version="0.1.1",
+    version="0.1.2",
     description="Package for decentralized stochastic gradient descent",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://github.com/mrislambd/desgld_package.git",
     author="Rafiq Islam",
     packages=["desgld"],
     package_dir={"": "src"},
     install_requires=requirements,
     extras_require={"dev": requirements_dev},
 )
```

### Comparing `desgld-0.1.1/src/desgld/desgld_alg.py` & `desgld-0.1.2/src/desgld/desgld_alg.py`

 * *Files identical despite different names*

### Comparing `desgld-0.1.1/src/desgld/evaluation.py` & `desgld-0.1.2/src/desgld/evaluation.py`

 * *Files identical despite different names*

