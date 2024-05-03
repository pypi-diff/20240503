# Comparing `tmp/fpp_sle-0.2.3.tar.gz` & `tmp/fpp_sle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpp_sle-0.2.3.tar", max compression
+gzip compressed data, was "fpp_sle-0.3.0.tar", max compression
```

## Comparing `fpp_sle-0.2.3.tar` & `fpp_sle-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-01-10 07:54:12.444742 fpp_sle-0.2.3/LICENSE
--rw-r--r--   0        0        0     3499 2024-01-10 07:54:12.444742 fpp_sle-0.2.3/README.md
--rw-r--r--   0        0        0     2822 2024-01-10 07:54:26.544926 fpp_sle-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      150 2024-01-10 07:54:12.444742 fpp_sle-0.2.3/src/fpp_sle/__init__.py
--rw-r--r--   0        0        0       43 2024-01-10 07:54:12.444742 fpp_sle-0.2.3/src/fpp_sle/__main__.py
--rw-r--r--   0        0        0      195 2024-01-10 07:54:12.448742 fpp_sle-0.2.3/src/fpp_sle/fpp/__init__.py
--rw-r--r--   0        0        0     3698 2024-01-10 07:54:12.448742 fpp_sle-0.2.3/src/fpp_sle/fpp/forcing_generators.py
--rw-r--r--   0        0        0     8443 2024-01-10 07:54:12.448742 fpp_sle-0.2.3/src/fpp_sle/fpp/get_arrival_times.py
--rw-r--r--   0        0        0      323 2024-01-10 07:54:12.448742 fpp_sle-0.2.3/src/fpp_sle/sde/__init__.py
--rw-r--r--   0        0        0     8884 2024-01-10 07:54:12.448742 fpp_sle-0.2.3/src/fpp_sle/sde/runge_kutta_sde.py
--rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 fpp_sle-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3482 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/README.md
+-rw-r--r--   0        0        0     2830 2024-05-03 06:59:34.222982 fpp_sle-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/__main__.py
+-rw-r--r--   0        0        0      195 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/fpp/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/fpp/forcing_generators.py
+-rw-r--r--   0        0        0     8443 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/fpp/get_arrival_times.py
+-rw-r--r--   0        0        0      323 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/sde/__init__.py
+-rw-r--r--   0        0        0     8884 2024-05-03 06:59:20.650998 fpp_sle-0.3.0/src/fpp_sle/sde/runge_kutta_sde.py
+-rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 fpp_sle-0.3.0/PKG-INFO
```

### Comparing `fpp_sle-0.2.3/LICENSE` & `fpp_sle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fpp_sle-0.2.3/README.md` & `fpp_sle-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 </div>
 
 ## Install
 
 The package is publised on [PyPI] and installable via `pip`:
 
-```sh
+```bash
 pip install fpp-sle
 ```
 
 ## Usage
 
 See the [examples.py] script for working examples. The main classes and functions this
 package provide is
@@ -56,30 +56,30 @@
 
   This module holds different implementations of stochastic differential equations. See
   the docstring of the individual functions for explanations.
 
 ## Contributing
 
 To contribute to the project, clone and install the full development version (uses
-[poetry] for dependencies). There is also a `.rtx.toml` file that installs and sets up
-an appropriate virtual environment if [rtx](https://github.com/jdx/rtx) is available on
-your system (it's really good, check it out!).
+[poetry] for dependencies). There is also a `.mise.toml` file that installs and sets up
+an appropriate virtual environment if [mise](https://mise.jdx.dev/) is available on your
+system.
 
-```sh
+```bash
 git clone https://github.com/uit-cosmo/fpp-sle.git
 cd fpp-sle
-# Set up a virtual environment, for example with rtx
-rtx i
+# Set up a virtual environment, for example with mise
+mise i  # optional
 poetry install
 pre-commit install
 ```
 
 Before committing new changes to a branch you may run command
 
-```sh
+```bash
 nox
 ```
 
 to run the full test suite. You will need [Poetry], [nox] and [nox-poetry] installed for
 this.
 
 [pypi]: https://pypi.org/
```

### Comparing `fpp_sle-0.2.3/pyproject.toml` & `fpp_sle-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fpp-sle"
-version = "0.2.3"
+version = "0.3.0"
 description = "Implements FPP and SLE algorithms"
 authors = ["engeir <engeir@pm.me>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "fpp_sle", from = "src" }]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -15,31 +15,31 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<3.13"
 numpy = "^1.20.2"
 numba = ">=0.53.1,<0.59.0"
 superposed-pulses = "^1.2"
 importlib-metadata = ">=5,<7"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.10,<24.0"
-bandit = "1.7.5"
+bandit = "1.7.6"
 mypy = ">=0.982,<1.7"
 pre-commit = ">=2.19,<4.0"
 pre-commit-hooks = "^4.2.0"
 pytest = "^7.1.2"
 isort = "^5.10.1"
 darglint = "^1.8.1"
 cosmoplots = ">=0.1.6,<0.4.0"
-ruff = "^0.1.1"
+ruff = ">=0.1.1,<0.5.0"
 pydocstringformatter = "^0.7.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `fpp_sle-0.2.3/src/fpp_sle/fpp/forcing_generators.py` & `fpp_sle-0.3.0/src/fpp_sle/fpp/forcing_generators.py`

 * *Files identical despite different names*

### Comparing `fpp_sle-0.2.3/src/fpp_sle/fpp/get_arrival_times.py` & `fpp_sle-0.3.0/src/fpp_sle/fpp/get_arrival_times.py`

 * *Files identical despite different names*

### Comparing `fpp_sle-0.2.3/src/fpp_sle/sde/runge_kutta_sde.py` & `fpp_sle-0.3.0/src/fpp_sle/sde/runge_kutta_sde.py`

 * *Files identical despite different names*

### Comparing `fpp_sle-0.2.3/PKG-INFO` & `fpp_sle-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fpp-sle
-Version: 0.2.3
+Version: 0.3.0
 Summary: Implements FPP and SLE algorithms
 License: GPL-3.0-or-later
 Author: engeir
 Author-email: engeir@pm.me
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: importlib-metadata (>=5,<7)
 Requires-Dist: numba (>=0.53.1,<0.59.0)
 Requires-Dist: numpy (>=1.20.2,<2.0.0)
 Requires-Dist: superposed-pulses (>=1.2,<2.0)
 Description-Content-Type: text/markdown
 
@@ -37,15 +38,15 @@
 
 </div>
 
 ## Install
 
 The package is publised on [PyPI] and installable via `pip`:
 
-```sh
+```bash
 pip install fpp-sle
 ```
 
 ## Usage
 
 See the [examples.py] script for working examples. The main classes and functions this
 package provide is
@@ -80,30 +81,30 @@
 
   This module holds different implementations of stochastic differential equations. See
   the docstring of the individual functions for explanations.
 
 ## Contributing
 
 To contribute to the project, clone and install the full development version (uses
-[poetry] for dependencies). There is also a `.rtx.toml` file that installs and sets up
-an appropriate virtual environment if [rtx](https://github.com/jdx/rtx) is available on
-your system (it's really good, check it out!).
+[poetry] for dependencies). There is also a `.mise.toml` file that installs and sets up
+an appropriate virtual environment if [mise](https://mise.jdx.dev/) is available on your
+system.
 
-```sh
+```bash
 git clone https://github.com/uit-cosmo/fpp-sle.git
 cd fpp-sle
-# Set up a virtual environment, for example with rtx
-rtx i
+# Set up a virtual environment, for example with mise
+mise i  # optional
 poetry install
 pre-commit install
 ```
 
 Before committing new changes to a branch you may run command
 
-```sh
+```bash
 nox
 ```
 
 to run the full test suite. You will need [Poetry], [nox] and [nox-poetry] installed for
 this.
 
 [pypi]: https://pypi.org/
```

