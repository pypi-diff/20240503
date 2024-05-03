# Comparing `tmp/precommend-0.3.0.tar.gz` & `tmp/precommend-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precommend-0.3.0.tar", last modified: Tue Apr 23 13:21:01 2024, max compression
+gzip compressed data, was "precommend-0.3.1.tar", last modified: Fri May  3 11:25:53 2024, max compression
```

## Comparing `precommend-0.3.0.tar` & `precommend-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.229344 precommend-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.221344 precommend-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:20:54.000000 precommend-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.221344 precommend-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 13:20:54.000000 precommend-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 13:20:54.000000 precommend-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 13:20:54.000000 precommend-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-23 13:20:54.000000 precommend-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 13:20:54.000000 precommend-0.3.0/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-23 13:20:54.000000 precommend-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 13:20:54.000000 precommend-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-23 13:21:01.229344 precommend-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 13:20:54.000000 precommend-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-23 13:20:54.000000 precommend-0.3.0/bump_identify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/precommend/
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 13:20:54.000000 precommend-0.3.0/precommend/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/precommend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 13:21:01.000000 precommend-0.3.0/precommend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-23 13:20:54.000000 precommend-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:21:01.229344 precommend-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 13:20:54.000000 precommend-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 13:20:54.000000 precommend-0.3.0/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.221344 precommend-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/cpp/test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/generic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/generic/.github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/generic/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/generic/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/generic/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/generic/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:21:01.225344 precommend-0.3.0/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/python/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/data/python/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 13:20:54.000000 precommend-0.3.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.339240 precommend-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 11:25:48.000000 precommend-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.339240 precommend-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 11:25:48.000000 precommend-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-03 11:25:48.000000 precommend-0.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-03 11:25:48.000000 precommend-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-03 11:25:48.000000 precommend-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 11:25:48.000000 precommend-0.3.1/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 11:25:48.000000 precommend-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 11:25:48.000000 precommend-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-03 11:25:53.343241 precommend-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-03 11:25:48.000000 precommend-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 11:25:48.000000 precommend-0.3.1/bump_identify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.339240 precommend-0.3.1/precommend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-03 11:25:48.000000 precommend-0.3.1/precommend/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 11:25:48.000000 precommend-0.3.1/precommend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-03 11:25:48.000000 precommend-0.3.1/precommend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-03 11:25:48.000000 precommend-0.3.1/precommend/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-03 11:25:48.000000 precommend-0.3.1/precommend/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/precommend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 11:25:53.000000 precommend-0.3.1/precommend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-03 11:25:48.000000 precommend-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:25:53.343241 precommend-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 11:25:48.000000 precommend-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-03 11:25:48.000000 precommend-0.3.1/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.335240 precommend-0.3.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/tests/data/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/cpp/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/tests/data/generic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/tests/data/generic/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/generic/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/tests/data/generic/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/generic/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/generic/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:53.343241 precommend-0.3.1/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/python/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/data/python/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-03 11:25:48.000000 precommend-0.3.1/tests/test_core.py
```

### Comparing `precommend-0.3.0/.github/workflows/ci.yml` & `precommend-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/.github/workflows/pypi.yml` & `precommend-0.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/.gitignore` & `precommend-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/.pre-commit-config.yaml` & `precommend-0.3.1/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 
 repos:
   - repo: local
     hooks:
       - id: synchronize-files
         name: Synchronize files within the repository
         entry: python sync.py
-        language: system
+        language: python
         always_run: true
         pass_filenames: false
       - id: bump-precommit-and-identify
         name: Bump versions of pre-commit and identify
         entry: python bump_identify.py
-        language: system
+        language: python
+        additional_dependencies: [requests]
         always_run: true
         pass_filenames: false
 
   - repo: https://github.com/psf/black
-    rev: 24.4.0
+    rev: 24.4.2
     hooks:
       - id: black  # Run Black - the uncompromising Python code formatter
       - id: black-jupyter  # Run Black - the uncompromising Python code formatter (Jupyter version)
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
@@ -76,22 +77,25 @@
       - id: setup-cfg-fmt  # Automatically format/sanitize setup.cfg
 
   - repo: https://github.com/citation-file-format/cffconvert
     rev: main
     hooks:
       - id: validate-cff # Validate CFF format
 
-  - repo: https://github.com/lovesegfault/beautysh
-    rev: v6.2.1
+  - repo: https://github.com/pecigonzalo/pre-commit-shfmt
+    rev: v2.2.0
     hooks:
-      - id: beautysh  # Beautify Bash scripts
+      - id: shell-fmt-go  # Format Bash scripts
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject  # Validate the contents of pyproject.toml
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
     rev: 0.28.2
     hooks:
       - id: check-readthedocs  # Validate the given .readthedocs.yml file
       - id: check-dependabot  # Validate the given dependabot.yml file
+
+ci:
+  skip: [bump-precommit-and-identify]
```

### Comparing `precommend-0.3.0/LICENSE.md` & `precommend-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/PKG-INFO` & `precommend-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.3.0
+Version: 0.3.1
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `precommend-0.3.0/README.md` & `precommend-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/bump_identify.py` & `precommend-0.3.1/bump_identify.py`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/precommend/.pre-commit-config.yaml` & `precommend-0.3.1/precommend/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 
 repos:
   - repo: local
     hooks:
       - id: synchronize-files
         name: Synchronize files within the repository
         entry: python sync.py
-        language: system
+        language: python
         always_run: true
         pass_filenames: false
       - id: bump-precommit-and-identify
         name: Bump versions of pre-commit and identify
         entry: python bump_identify.py
-        language: system
+        language: python
+        additional_dependencies: [requests]
         always_run: true
         pass_filenames: false
 
   - repo: https://github.com/psf/black
-    rev: 24.4.0
+    rev: 24.4.2
     hooks:
       - id: black  # Run Black - the uncompromising Python code formatter
       - id: black-jupyter  # Run Black - the uncompromising Python code formatter (Jupyter version)
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
@@ -76,22 +77,25 @@
       - id: setup-cfg-fmt  # Automatically format/sanitize setup.cfg
 
   - repo: https://github.com/citation-file-format/cffconvert
     rev: main
     hooks:
       - id: validate-cff # Validate CFF format
 
-  - repo: https://github.com/lovesegfault/beautysh
-    rev: v6.2.1
+  - repo: https://github.com/pecigonzalo/pre-commit-shfmt
+    rev: v2.2.0
     hooks:
-      - id: beautysh  # Beautify Bash scripts
+      - id: shell-fmt-go  # Format Bash scripts
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.16
     hooks:
       - id: validate-pyproject  # Validate the contents of pyproject.toml
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
     rev: 0.28.2
     hooks:
       - id: check-readthedocs  # Validate the given .readthedocs.yml file
       - id: check-dependabot  # Validate the given dependabot.yml file
+
+ci:
+  skip: [bump-precommit-and-identify]
```

### Comparing `precommend-0.3.0/precommend/__main__.py` & `precommend-0.3.1/precommend/__main__.py`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/precommend/core.py` & `precommend-0.3.1/precommend/core.py`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/precommend/rules.py` & `precommend-0.3.1/precommend/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 @rule
 def actionlint(ctx):
     if ctx.directory_exists(".github/workflows"):
         return "actionlint"
 
 
 @rule
-def beautysh(ctx):
-    if ctx.tag_exists("bash"):
-        return "beautysh"
+def shell_fmt_go(ctx):
+    if ctx.tag_exists("shell") or ctx.tag_exists("bash"):
+        return "shell-fmt-go"
 
 
 @rule
 def black(ctx):
     if ctx.tag_exists("jupyter"):
         return "black-jupyter"
     if ctx.tag_exists("python"):
```

### Comparing `precommend-0.3.0/precommend.egg-info/PKG-INFO` & `precommend-0.3.1/precommend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precommend
-Version: 0.3.0
+Version: 0.3.1
 Summary: Opinionated initialization of pre-commit configurations
 Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `precommend-0.3.0/precommend.egg-info/SOURCES.txt` & `precommend-0.3.1/precommend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/pyproject.toml` & `precommend-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `precommend-0.3.0/tests/test_core.py` & `precommend-0.3.1/tests/test_core.py`

 * *Files identical despite different names*

