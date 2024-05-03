# Comparing `tmp/gpytorch_mogp-0.1.0.tar.gz` & `tmp/gpytorch_mogp-0.1.1.tar.gz`

## Comparing `gpytorch_mogp-0.1.0.tar` & `gpytorch_mogp-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0   414111 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/examples/comparison_with_rapid_models.ipynb
--rw-r--r--   0        0        0   149282 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/examples/gpytorch-mogp.png
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/examples/multioutput_gp_regression.py
--rw-r--r--   0        0        0   148734 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/examples/rapid-models.png
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/kernels/__init__.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/kernels/multioutput_kernel.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/likelihoods/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/likelihoods/multioutput_gaussian_likelihood.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/likelihoods/noise_models.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/utils/__init__.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/utils/blocks.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/src/gpytorch_mogp/utils/covariance.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/LICENSE
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/README.md
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0   414111 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/examples/comparison_with_rapid_models.ipynb
+-rw-r--r--   0        0        0   149282 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/examples/gpytorch-mogp.png
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/examples/multioutput_gp_regression.py
+-rw-r--r--   0        0        0   148734 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/examples/rapid-models.png
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/kernels/__init__.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/kernels/multioutput_kernel.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/likelihoods/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/likelihoods/multioutput_gaussian_likelihood.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/likelihoods/noise_models.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/utils/__init__.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/utils/blocks.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/src/gpytorch_mogp/utils/covariance.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/README.md
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10553 2020-02-02 00:00:00.000000 gpytorch_mogp-0.1.1/PKG-INFO
```

### Comparing `gpytorch_mogp-0.1.0/examples/comparison_with_rapid_models.ipynb` & `gpytorch_mogp-0.1.1/examples/comparison_with_rapid_models.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/examples/gpytorch-mogp.png` & `gpytorch_mogp-0.1.1/examples/gpytorch-mogp.png`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/examples/multioutput_gp_regression.py` & `gpytorch_mogp-0.1.1/examples/multioutput_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/examples/rapid-models.png` & `gpytorch_mogp-0.1.1/examples/rapid-models.png`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/src/gpytorch_mogp/kernels/multioutput_kernel.py` & `gpytorch_mogp-0.1.1/src/gpytorch_mogp/kernels/multioutput_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/src/gpytorch_mogp/likelihoods/multioutput_gaussian_likelihood.py` & `gpytorch_mogp-0.1.1/src/gpytorch_mogp/likelihoods/multioutput_gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/src/gpytorch_mogp/likelihoods/noise_models.py` & `gpytorch_mogp-0.1.1/src/gpytorch_mogp/likelihoods/noise_models.py`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/src/gpytorch_mogp/utils/blocks.py` & `gpytorch_mogp-0.1.1/src/gpytorch_mogp/utils/blocks.py`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/src/gpytorch_mogp/utils/covariance.py` & `gpytorch_mogp-0.1.1/src/gpytorch_mogp/utils/covariance.py`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/.gitignore` & `gpytorch_mogp-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/LICENSE` & `gpytorch_mogp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpytorch_mogp-0.1.0/README.md` & `gpytorch_mogp-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # gpytorch-mogp
 
-[![PyPI - Version](https://img.shields.io/pypi/v/gpytorch-mogp-new.svg)](https://pypi.org/project/gpytorch-mogp-new)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gpytorch-mogp-new.svg)](https://pypi.org/project/gpytorch-mogp-new)
+[![PyPI - Version](https://img.shields.io/pypi/v/gpytorch-mogp.svg)](https://pypi.org/project/gpytorch-mogp)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gpytorch-mogp.svg)](https://pypi.org/project/gpytorch-mogp)
 
 `gpytorch-mogp` is a Python package that extends [GPyTorch](https://gpytorch.ai/) to support Multiple-Output Gaussian
 processes where the correlation between the outputs is known.
 
 > **Note:** The package is currently in an early stage of development. Expect bugs and breaking changes in future
 > versions. Please create an issue if you encounter any problems or have any suggestions.
```

### Comparing `gpytorch_mogp-0.1.0/pyproject.toml` & `gpytorch_mogp-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gpytorch-mogp"
 description = "A package which extends GPyTorch with correlated multi-output GPs"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 requires-python = ">=3.11"
 license = "MIT"
 authors = [
     { name = "Magnus Kristiansen", email = "magnus.kristiansen@dnv.com" },
 ]
 classifiers = [
```

### Comparing `gpytorch_mogp-0.1.0/PKG-INFO` & `gpytorch_mogp-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gpytorch-mogp
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package which extends GPyTorch with correlated multi-output GPs
 Project-URL: Documentation, https://github.com/magkri/gpytorch-mogp#readme
 Project-URL: Issues, https://github.com/magkri/gpytorch-mogp/issues
 Project-URL: Source, https://github.com/magkri/gpytorch-mogp
 Author-email: Magnus Kristiansen <magnus.kristiansen@dnv.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -25,16 +25,16 @@
 Provides-Extra: examples
 Requires-Dist: jupyter>=1.0.0; extra == 'examples'
 Requires-Dist: matplotlib>=3.8.4; extra == 'examples'
 Description-Content-Type: text/markdown
 
 # gpytorch-mogp
 
-[![PyPI - Version](https://img.shields.io/pypi/v/gpytorch-mogp-new.svg)](https://pypi.org/project/gpytorch-mogp-new)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gpytorch-mogp-new.svg)](https://pypi.org/project/gpytorch-mogp-new)
+[![PyPI - Version](https://img.shields.io/pypi/v/gpytorch-mogp.svg)](https://pypi.org/project/gpytorch-mogp)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gpytorch-mogp.svg)](https://pypi.org/project/gpytorch-mogp)
 
 `gpytorch-mogp` is a Python package that extends [GPyTorch](https://gpytorch.ai/) to support Multiple-Output Gaussian
 processes where the correlation between the outputs is known.
 
 > **Note:** The package is currently in an early stage of development. Expect bugs and breaking changes in future
 > versions. Please create an issue if you encounter any problems or have any suggestions.
```

