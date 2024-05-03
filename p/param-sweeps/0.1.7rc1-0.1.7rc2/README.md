# Comparing `tmp/param_sweeps-0.1.7rc1.tar.gz` & `tmp/param_sweeps-0.1.7rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "param_sweeps-0.1.7rc1.tar", max compression
+gzip compressed data, was "param_sweeps-0.1.7rc2.tar", max compression
```

## Comparing `param_sweeps-0.1.7rc1.tar` & `param_sweeps-0.1.7rc2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1093 2024-04-28 20:40:55.138491 param_sweeps-0.1.7rc1/LICENSE
--rw-r--r--   0        0        0      267 2024-04-28 20:46:48.524927 param_sweeps-0.1.7rc1/param_sweeps/__init__.py
--rw-r--r--   0        0        0      572 2024-04-23 21:33:39.731115 param_sweeps-0.1.7rc1/param_sweeps/constants.py
--rw-r--r--   0        0        0     8151 2024-04-23 21:33:39.731115 param_sweeps-0.1.7rc1/param_sweeps/driver.py
--rw-r--r--   0        0        0     3230 2024-04-23 21:33:39.732216 param_sweeps-0.1.7rc1/param_sweeps/generate.py
--rw-r--r--   0        0        0      967 2024-04-23 21:33:39.732216 param_sweeps-0.1.7rc1/param_sweeps/sample_driver.py
--rw-r--r--   0        0        0     2683 2024-04-28 20:46:48.519489 param_sweeps-0.1.7rc1/pyproject.toml
--rw-r--r--   0        0        0     1153 2024-04-23 21:33:39.730041 param_sweeps-0.1.7rc1/README.md
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 param_sweeps-0.1.7rc1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-28 20:40:55.138491 param_sweeps-0.1.7rc2/LICENSE
+-rw-r--r--   0        0        0      267 2024-05-03 01:36:19.608726 param_sweeps-0.1.7rc2/param_sweeps/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-23 21:33:39.731115 param_sweeps-0.1.7rc2/param_sweeps/constants.py
+-rw-r--r--   0        0        0     8151 2024-04-23 21:33:39.731115 param_sweeps-0.1.7rc2/param_sweeps/driver.py
+-rw-r--r--   0        0        0     3230 2024-04-23 21:33:39.732216 param_sweeps-0.1.7rc2/param_sweeps/generate.py
+-rw-r--r--   0        0        0      967 2024-04-23 21:33:39.732216 param_sweeps-0.1.7rc2/param_sweeps/sample_driver.py
+-rw-r--r--   0        0        0     2512 2024-05-03 01:36:19.603227 param_sweeps-0.1.7rc2/pyproject.toml
+-rw-r--r--   0        0        0     2796 2024-05-02 04:21:01.466596 param_sweeps-0.1.7rc2/README.md
+-rw-r--r--   0        0        0      740 2024-05-02 04:21:01.466596 param_sweeps-0.1.7rc2/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     4067 1970-01-01 00:00:00.000000 param_sweeps-0.1.7rc2/PKG-INFO
```

### Comparing `param_sweeps-0.1.7rc1/LICENSE` & `param_sweeps-0.1.7rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7rc1/param_sweeps/constants.py` & `param_sweeps-0.1.7rc2/param_sweeps/constants.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7rc1/param_sweeps/driver.py` & `param_sweeps-0.1.7rc2/param_sweeps/driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7rc1/param_sweeps/generate.py` & `param_sweeps-0.1.7rc2/param_sweeps/generate.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7rc1/param_sweeps/sample_driver.py` & `param_sweeps-0.1.7rc2/param_sweeps/sample_driver.py`

 * *Files identical despite different names*

### Comparing `param_sweeps-0.1.7rc1/pyproject.toml` & `param_sweeps-0.1.7rc2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "param-sweeps"
-version = "0.1.7-rc.1"
+version = "0.1.7-rc.2"
 
 description = "Parameter sweeper for ui.json powered applications"
 license = "MIT"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = ["Benjamin Kary <benjamink@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/param-sweeps"
 #documentatio  = "https://mirageoscience-param-sweeps.readthedocs-hosted.com/"
@@ -50,20 +50,15 @@
 Pygments = "*"
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 tomli = "*"
 
 [tool.isort]
-# settings for compatibility between ``isort`` and ``black`` formatting
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-line_length = 88
+profile = "black"
 
 [tool.black]
 # defaults are just fine
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
```

