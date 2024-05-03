# Comparing `tmp/atlantisfastapi-6.0.1.tar.gz` & `tmp/atlantisfastapi-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantisfastapi-6.0.1.tar", last modified: Wed Apr  3 14:51:15 2024, max compression
+gzip compressed data, was "atlantisfastapi-7.0.0.tar", last modified: Fri May  3 10:27:11 2024, max compression
```

## Comparing `atlantisfastapi-6.0.1.tar` & `atlantisfastapi-7.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:15.094753 atlantisfastapi-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 14:51:15.094753 atlantisfastapi-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:15.090753 atlantisfastapi-6.0.1/atlantisfastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/atlantisfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:15.090753 atlantisfastapi-6.0.1/atlantisfastapi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/atlantisfastapi/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:15.090753 atlantisfastapi-6.0.1/atlantisfastapi/lib/security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/atlantisfastapi/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/atlantisfastapi/lib/security/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:15.090753 atlantisfastapi-6.0.1/atlantisfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 14:51:15.000000 atlantisfastapi-6.0.1/atlantisfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-03 14:51:15.000000 atlantisfastapi-6.0.1/atlantisfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:51:15.000000 atlantisfastapi-6.0.1/atlantisfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 14:51:15.000000 atlantisfastapi-6.0.1/atlantisfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 14:51:15.000000 atlantisfastapi-6.0.1/atlantisfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:51:15.098753 atlantisfastapi-6.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:15.090753 atlantisfastapi-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-03 14:50:21.000000 atlantisfastapi-6.0.1/tests/test_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:27:11.670227 atlantisfastapi-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 10:27:11.670227 atlantisfastapi-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:27:11.662227 atlantisfastapi-7.0.0/atlantisfastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/atlantisfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:27:11.662227 atlantisfastapi-7.0.0/atlantisfastapi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/atlantisfastapi/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:27:11.666227 atlantisfastapi-7.0.0/atlantisfastapi/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/atlantisfastapi/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/atlantisfastapi/lib/security/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:27:11.666227 atlantisfastapi-7.0.0/atlantisfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-03 10:27:11.000000 atlantisfastapi-7.0.0/atlantisfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-03 10:27:11.000000 atlantisfastapi-7.0.0/atlantisfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:27:11.000000 atlantisfastapi-7.0.0/atlantisfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 10:27:11.000000 atlantisfastapi-7.0.0/atlantisfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 10:27:11.000000 atlantisfastapi-7.0.0/atlantisfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:27:11.670227 atlantisfastapi-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:27:11.666227 atlantisfastapi-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-03 10:26:06.000000 atlantisfastapi-7.0.0/tests/test_finder.py
```

### Comparing `atlantisfastapi-6.0.1/PKG-INFO` & `atlantisfastapi-7.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: atlantisfastapi
-Version: 6.0.1
+Version: 7.0.0
 Summary: atlantisfastapi
 Author-email: Atlantis Labs <r00tail@protonmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: coderfastapi~=4.2.2
-Requires-Dist: atlantiscore~=7.0
+Requires-Dist: coderfastapi~=5.0.0
+Requires-Dist: atlantiscore~=9.0
 Provides-Extra: test
 Requires-Dist: pytest~=7.4; extra == "test"
 Requires-Dist: pytest-asyncio~=0.21; extra == "test"
 Requires-Dist: pytest-cov~=4.1; extra == "test"
 Requires-Dist: pytest-mock~=3.11; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=3.3; extra == "test"
 Provides-Extra: dev
```

### Comparing `atlantisfastapi-6.0.1/atlantisfastapi/__init__.py` & `atlantisfastapi-7.0.0/atlantisfastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantisfastapi-6.0.1/atlantisfastapi/lib/security/http.py` & `atlantisfastapi-7.0.0/atlantisfastapi/lib/security/http.py`

 * *Files identical despite different names*

### Comparing `atlantisfastapi-6.0.1/atlantisfastapi.egg-info/PKG-INFO` & `atlantisfastapi-7.0.0/atlantisfastapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: atlantisfastapi
-Version: 6.0.1
+Version: 7.0.0
 Summary: atlantisfastapi
 Author-email: Atlantis Labs <r00tail@protonmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: coderfastapi~=4.2.2
-Requires-Dist: atlantiscore~=7.0
+Requires-Dist: coderfastapi~=5.0.0
+Requires-Dist: atlantiscore~=9.0
 Provides-Extra: test
 Requires-Dist: pytest~=7.4; extra == "test"
 Requires-Dist: pytest-asyncio~=0.21; extra == "test"
 Requires-Dist: pytest-cov~=4.1; extra == "test"
 Requires-Dist: pytest-mock~=3.11; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=3.3; extra == "test"
 Provides-Extra: dev
```

### Comparing `atlantisfastapi-6.0.1/pyproject.toml` & `atlantisfastapi-7.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlantisfastapi"
-version = "6.0.1"
+version = "7.0.0"
 description = "atlantisfastapi"
 readme = "README.md"
 authors = [{ name = "Atlantis Labs", email = "r00tail@protonmail.com" }]
 dependencies = [
-    'coderfastapi ~= 4.2.2',
-    "atlantiscore ~= 7.0",
+    'coderfastapi ~= 5.0.0',
+    "atlantiscore ~= 9.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest ~= 7.4",
     "pytest-asyncio ~= 0.21",
     "pytest-cov ~= 4.1",
@@ -22,15 +22,15 @@
     "pytest-xdist[psutil] ~= 3.3",
 ]
 dev = [
     'black ~= 23.9'
 ]
 
 [tool.bumpver]
-current_version = "6.0.1"
+current_version = "7.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `atlantisfastapi-6.0.1/tests/test_finder.py` & `atlantisfastapi-7.0.0/tests/test_finder.py`

 * *Files identical despite different names*

