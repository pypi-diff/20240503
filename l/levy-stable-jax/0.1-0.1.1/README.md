# Comparing `tmp/levy_stable_jax-0.1.tar.gz` & `tmp/levy_stable_jax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levy_stable_jax-0.1.tar", max compression
+gzip compressed data, was "levy_stable_jax-0.1.1.tar", max compression
```

## Comparing `levy_stable_jax-0.1.tar` & `levy_stable_jax-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-10-22 07:47:03.747679 levy_stable_jax-0.1/LICENSE
--rw-r--r--   0        0        0     1211 2024-05-03 13:48:05.485542 levy_stable_jax-0.1/README.md
--rw-r--r--   0        0        0     2609 2024-04-26 18:20:38.105714 levy_stable_jax-0.1/pyproject.toml
--rw-r--r--   0        0        0      336 2024-05-03 13:29:34.962247 levy_stable_jax-0.1/src/levy_stable_jax/__init__.py
--rw-r--r--   0        0        0      708 2024-04-24 12:12:58.006634 levy_stable_jax-0.1/src/levy_stable_jax/_cache.py
--rw-r--r--   0        0        0     4270 2024-05-03 11:58:27.607858 levy_stable_jax-0.1/src/levy_stable_jax/_generate_data.py
--rw-r--r--   0        0        0      975 2024-05-03 13:51:24.346392 levy_stable_jax-0.1/src/levy_stable_jax/_interp.py
--rw-r--r--   0        0        0      559 2024-05-03 13:29:34.962247 levy_stable_jax-0.1/src/levy_stable_jax/_typing.py
--rw-r--r--   0        0        0     7742 2024-05-03 13:50:38.658201 levy_stable_jax-0.1/src/levy_stable_jax/_utils.py
--rw-r--r--   0        0        0    12470 2024-05-03 13:43:26.840236 levy_stable_jax-0.1/src/levy_stable_jax/distribution.py
--rw-r--r--   0        0        0     4556 2024-05-03 13:29:34.966248 levy_stable_jax-0.1/src/levy_stable_jax/estimation.py
--rw-r--r--   0        0        0  6464128 2024-05-03 13:29:34.994248 levy_stable_jax-0.1/src/levy_stable_jax/logpdf.npy
--rw-r--r--   0        0        0     6069 2024-05-03 13:31:25.623373 levy_stable_jax-0.1/src/levy_stable_jax/pymc.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 levy_stable_jax-0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-22 07:47:03.747679 levy_stable_jax-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1232 2024-05-03 14:13:46.602439 levy_stable_jax-0.1.1/README.md
+-rw-r--r--   0        0        0     2365 2024-05-03 14:12:44.162493 levy_stable_jax-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      336 2024-05-03 13:29:34.962247 levy_stable_jax-0.1.1/src/levy_stable_jax/__init__.py
+-rw-r--r--   0        0        0      708 2024-04-24 12:12:58.006634 levy_stable_jax-0.1.1/src/levy_stable_jax/_cache.py
+-rw-r--r--   0        0        0     4270 2024-05-03 11:58:27.607858 levy_stable_jax-0.1.1/src/levy_stable_jax/_generate_data.py
+-rw-r--r--   0        0        0      975 2024-05-03 13:51:24.346392 levy_stable_jax-0.1.1/src/levy_stable_jax/_interp.py
+-rw-r--r--   0        0        0      559 2024-05-03 13:29:34.962247 levy_stable_jax-0.1.1/src/levy_stable_jax/_typing.py
+-rw-r--r--   0        0        0     7742 2024-05-03 13:50:38.658201 levy_stable_jax-0.1.1/src/levy_stable_jax/_utils.py
+-rw-r--r--   0        0        0    12470 2024-05-03 13:43:26.840236 levy_stable_jax-0.1.1/src/levy_stable_jax/distribution.py
+-rw-r--r--   0        0        0     4556 2024-05-03 13:29:34.966248 levy_stable_jax-0.1.1/src/levy_stable_jax/estimation.py
+-rw-r--r--   0        0        0  6464128 2024-05-03 13:29:34.994248 levy_stable_jax-0.1.1/src/levy_stable_jax/logpdf.npy
+-rw-r--r--   0        0        0     6069 2024-05-03 13:31:25.623373 levy_stable_jax-0.1.1/src/levy_stable_jax/pymc.py
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 levy_stable_jax-0.1.1/PKG-INFO
```

### Comparing `levy_stable_jax-0.1/LICENSE` & `levy_stable_jax-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/README.md` & `levy_stable_jax-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 ## Commands (development only)
 
 
 Setting up the test environment
 
 ```
 pip install .[dev]
+make lint
+make test
+
 
 ```
```

### Comparing `levy_stable_jax-0.1/pyproject.toml` & `levy_stable_jax-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,51 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
+[project]
+name = "levy-stable-jax"
+version = "0.1.1"
+authors = [
+    {name = "Tim Hunter", email = "tjhunter@cs.stanford.edu"},
+]
+license = { text = "Apache 2 License" }
+description = "Implementation of the Lévy stable distributions for Jax."
+readme = "README.md"
+requires-python = ">=3.9"
+keywords = ["levy", "stable", "jax", "probability", "statistics"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+dependencies = [
+    "jax>=0.3",
+    "jaxopt>=0.8",
+    "numpy>=1.19",
+    "scipy>=1.5",    
+]
+
+[project.urls]
+Homepage = "https://github.com/tjhunter/levy-stable-jax"
+Documentation = "https://github.com/tjhunter/levy-stable-jax"
+Repository = "https://github.com/tjhunter/levy-stable-jax"
+
 [tool.poetry]
 packages = [{include = "levy_stable_jax", from="src"}]
 name = "levy-stable-jax"
-version = "0.1"
+version = "0.1.1"
 authors = ["Tim Hunter <tjhunter@cs.stanford.edu>"]
-description = "Implementation of the Lévy stable distributions for Jax."
+description = "Implementation of the Lévy alpha-stable distributions for Jax."
 readme = "README.md"
-license = "MIT"
+license = "Apache 2.0"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 jax = "^0.4"
 numpy = "^1.19" 
 scipy = "^1.5"
@@ -42,81 +73,25 @@
 numpyro = "^0.14.0"
 sphinx = "^7.3.7"
 sphinx-rtd-theme = "^2.0.0"
 mkdocs-material = "^9.5.19"
 mkdocstrings = {extras = ["python"], version = "^0.24.3"}
 pytkdocs = {version = "^0.16.1", extras = ["numpy-style"]}
 
-[project]
-name = "levy-stable-jax"
-version = "0.1"
-authors = [
-    {name = "Tim Hunter", email = "tjhunter@cs.stanford.edu"},
-]
-description = "Implementation of the Lévy stable distributions for Jax."
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
-dependencies = [
-    "jax>=0.3",
-    "jaxopt>=0.8",
-    "numpy>=1.19",
-    "scipy>=1.5",    
-]
-
-[project.optional-dependencies]
-dev = [
-    "black==23.10",
-    "mypy==1.6.1",
-    "ruff==0.1.1",
-]
-test = [
-    "pytest-cov~=4.1.0",
-    "pytest~=7.4.0",
-    "hypothesis~=6.88.0",
-    "absl-py==2.0.0",
-    "scikit-learn~=1.3.1",
-]
 
 [tool.pytest.ini_options]
 #addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
 minversion = "7.0"
 testpaths = [
     "tests",
 ]
 pythonpath = [
     "src",
 ]
 
-[tool.hatch.build.targets.wheel]
-sources = ["src"]
-
-[tool.hatch.build.targets.sdist]
-include = [
-  "src/*",
-]
-exclude = [
-]
-
-[tool.hatch.env]
-requires = [
-    "hatch-mkdocs",
-]
-
-[tool.hatch.env.collectors.mkdocs.docs]
-path = "mkdocs.yml"
 
 [tool.coverage.run]
 source = ["src"]
 
 [tool.ruff]
 
 line-length = 100
```

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/_cache.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/_cache.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/_generate_data.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/_generate_data.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/_interp.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/_interp.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/_typing.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/_typing.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/_utils.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/_utils.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/distribution.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/distribution.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/estimation.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/estimation.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/logpdf.npy` & `levy_stable_jax-0.1.1/src/levy_stable_jax/logpdf.npy`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/src/levy_stable_jax/pymc.py` & `levy_stable_jax-0.1.1/src/levy_stable_jax/pymc.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1/PKG-INFO` & `levy_stable_jax-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: levy-stable-jax
-Version: 0.1
-Summary: Implementation of the Lévy stable distributions for Jax.
-License: MIT
+Version: 0.1.1
+Summary: Implementation of the Lévy alpha-stable distributions for Jax.
+License: Apache 2.0
 Author: Tim Hunter
 Author-email: tjhunter@cs.stanford.edu
 Requires-Python: >=3.10,<3.13
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jax (>=0.4,<0.5)
 Requires-Dist: numpy (>=1.19,<2.0)
 Requires-Dist: scipy (>=1.5,<2.0)
@@ -44,9 +44,12 @@
 ## Commands (development only)
 
 
 Setting up the test environment
 
 ```
 pip install .[dev]
+make lint
+make test
+
 
 ```
```

