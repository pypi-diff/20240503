# Comparing `tmp/ssb_konjunk-0.0.4.tar.gz` & `tmp/ssb_konjunk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_konjunk-0.0.4.tar", max compression
+gzip compressed data, was "ssb_konjunk-0.0.5.tar", max compression
```

## Comparing `ssb_konjunk-0.0.4.tar` & `ssb_konjunk-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1073 2024-03-11 12:35:30.620894 ssb_konjunk-0.0.4/LICENSE
--rw-r--r--   0        0        0     2901 2024-03-11 12:35:30.620894 ssb_konjunk-0.0.4/README.md
--rw-r--r--   0        0        0     4085 2024-03-11 12:35:39.028892 ssb_konjunk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       19 2024-03-11 12:35:30.624894 ssb_konjunk-0.0.4/src/ssb_konjunk/__init__.py
--rw-r--r--   0        0        0      213 2024-03-11 12:35:30.624894 ssb_konjunk-0.0.4/src/ssb_konjunk/__main__.py
--rw-r--r--   0        0        0      466 2024-03-11 12:35:30.624894 ssb_konjunk-0.0.4/src/ssb_konjunk/_functions.py
--rw-r--r--   0        0        0      992 2024-03-11 12:35:30.624894 ssb_konjunk-0.0.4/src/ssb_konjunk/functions.py
--rw-r--r--   0        0        0     7069 2024-03-11 12:35:39.028892 ssb_konjunk-0.0.4/src/ssb_konjunk/prompts.py
--rw-r--r--   0        0        0        0 2024-03-11 12:35:30.624894 ssb_konjunk-0.0.4/src/ssb_konjunk/py.typed
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 ssb_konjunk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-03 08:43:28.163441 ssb_konjunk-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2901 2024-05-03 08:43:28.163441 ssb_konjunk-0.0.5/README.md
+-rw-r--r--   0        0        0     4088 2024-05-03 08:43:37.903423 ssb_konjunk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/__main__.py
+-rw-r--r--   0        0        0      466 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/_functions.py
+-rw-r--r--   0        0        0      627 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/data_formating.py
+-rw-r--r--   0        0        0      992 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/functions.py
+-rw-r--r--   0        0        0     7069 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/prompts.py
+-rw-r--r--   0        0        0        0 2024-05-03 08:43:28.167441 ssb_konjunk-0.0.5/src/ssb_konjunk/py.typed
+-rw-r--r--   0        0        0     3771 1970-01-01 00:00:00.000000 ssb_konjunk-0.0.5/PKG-INFO
```

### Comparing `ssb_konjunk-0.0.4/LICENSE` & `ssb_konjunk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_konjunk-0.0.4/README.md` & `ssb_konjunk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ssb_konjunk-0.0.4/pyproject.toml` & `ssb_konjunk-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ssb-konjunk"
-version = "0.0.4"
+version = "0.0.5"
 description = "SSB Konjunk"
 authors = ["Edvard Garmannslund <ged@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-konjunk"
 repository = "https://github.com/statisticsnorway/ssb-konjunk"
 documentation = "https://statisticsnorway.github.io/ssb-konjunk"
 classifiers = ["Development Status :: 1 - Planning"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-konjunk/releases"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 click = ">=8.0.1"
 pandas = "^2.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pygments = ">=2.10.0"
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
@@ -32,15 +32,15 @@
 sphinx = ">=6.2.1"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-autodoc-typehints = ">=1.24.0"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = { extras = ["colors"], version = ">=0.15.10" }
 myst-parser = { version = ">=0.16.1" }
-pandas-stubs = "^2.1.4.231227"
+pandas-stubs = ">=2.1.4.231227"
 
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.poetry.scripts]
 ssb-konjunk = "ssb_konjunk.__main__:main"
@@ -65,15 +65,15 @@
 show_column_numbers = true
 show_error_context = true
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
-target-version = "py39"  # Minimum Python version supported
+target-version = "py310"  # Minimum Python version supported
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 extend-exclude = [
     "__pycache__",
     "old",
     ".ipynb_checkpoints",
     "noxfile.py",
     "docs/conf.py",
```

### Comparing `ssb_konjunk-0.0.4/src/ssb_konjunk/functions.py` & `ssb_konjunk-0.0.5/src/ssb_konjunk/functions.py`

 * *Files identical despite different names*

### Comparing `ssb_konjunk-0.0.4/src/ssb_konjunk/prompts.py` & `ssb_konjunk-0.0.5/src/ssb_konjunk/prompts.py`

 * *Files identical despite different names*

### Comparing `ssb_konjunk-0.0.4/PKG-INFO` & `ssb_konjunk-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ssb-konjunk
-Version: 0.0.4
+Version: 0.0.5
 Summary: SSB Konjunk
 Home-page: https://github.com/statisticsnorway/ssb-konjunk
 License: MIT
 Author: Edvard Garmannslund
 Author-email: ged@ssb.no
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-konjunk/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/ssb-konjunk
```

