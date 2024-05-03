# Comparing `tmp/constrained_linear_regression-0.0.4.tar.gz` & `tmp/constrained_linear_regression-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrained_linear_regression-0.0.4.tar", last modified: Wed Aug 24 18:02:57 2022, max compression
+gzip compressed data, was "constrained_linear_regression-0.0.5.tar", last modified: Fri May  3 07:01:10 2024, max compression
```

## Comparing `constrained_linear_regression-0.0.4.tar` & `constrained_linear_regression-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-08-24 18:02:57.386806 constrained_linear_regression-0.0.4/
--rw-rw-rw-   0        0        0     2950 2022-08-24 18:02:57.385806 constrained_linear_regression-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1974 2021-09-30 23:10:27.000000 constrained_linear_regression-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-08-24 18:02:57.357806 constrained_linear_regression-0.0.4/constrained_linear_regression/
--rw-rw-rw-   0        0        0     5616 2022-08-24 17:59:09.000000 constrained_linear_regression-0.0.4/constrained_linear_regression/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-24 18:02:57.382806 constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/
--rw-rw-rw-   0        0        0     2950 2022-08-24 18:02:57.000000 constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2022-08-24 18:02:57.000000 constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-24 18:02:57.000000 constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-08-24 18:02:57.000000 constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2022-08-24 18:02:57.000000 constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-24 18:02:57.386806 constrained_linear_regression-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      967 2022-08-24 18:02:11.000000 constrained_linear_regression-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:01:10.250746 constrained_linear_regression-0.0.5/
+-rw-rw-rw-   0        0        0     2537 2024-05-03 07:01:10.245746 constrained_linear_regression-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1974 2021-09-30 23:10:27.000000 constrained_linear_regression-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 07:01:10.196747 constrained_linear_regression-0.0.5/constrained_linear_regression/
+-rw-rw-rw-   0        0        0      121 2024-05-03 06:46:46.000000 constrained_linear_regression-0.0.5/constrained_linear_regression/__init__.py
+-rw-rw-rw-   0        0        0     2064 2024-05-03 06:56:11.000000 constrained_linear_regression-0.0.5/constrained_linear_regression/base.py
+-rw-rw-rw-   0        0        0     3696 2024-05-03 06:46:47.000000 constrained_linear_regression-0.0.5/constrained_linear_regression/constrained_linear_regression.py
+-rw-rw-rw-   0        0        0     2818 2024-05-03 06:56:29.000000 constrained_linear_regression-0.0.5/constrained_linear_regression/matrix_constrained_linear_regression.py
+-rw-rw-rw-   0        0        0     5545 2024-05-03 06:56:11.000000 constrained_linear_regression-0.0.5/constrained_linear_regression/multi_constrained_linear_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:01:10.242747 constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/
+-rw-rw-rw-   0        0        0     2537 2024-05-03 07:01:10.000000 constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-05-03 07:01:10.000000 constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 07:01:10.000000 constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-03 07:01:10.000000 constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-03 07:01:10.000000 constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 07:01:10.250746 constrained_linear_regression-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      962 2024-05-03 06:59:38.000000 constrained_linear_regression-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 07:01:10.238750 constrained_linear_regression-0.0.5/tests/
+-rw-rw-rw-   0        0        0      769 2024-05-03 06:43:48.000000 constrained_linear_regression-0.0.5/tests/test_clr_basic.py
+-rw-rw-rw-   0        0        0     1947 2024-05-03 06:46:47.000000 constrained_linear_regression-0.0.5/tests/test_clr_multi.py
+-rw-rw-rw-   0        0        0     2136 2024-05-03 06:46:46.000000 constrained_linear_regression-0.0.5/tests/test_shape_check.py
```

### Comparing `constrained_linear_regression-0.0.4/PKG-INFO` & `constrained_linear_regression-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 Metadata-Version: 2.1
 Name: constrained_linear_regression
-Version: 0.0.4
+Version: 0.0.5
 Summary: Constrained linear regression in scikit-learn style
 Home-page: https://github.com/avidale/constrained-linear-regression
 Author: David Dale
 Author-email: dale.david@mail.ru
 License: MIT
-Description: # constrained-linear-regression
-        [![PyPI version](https://badge.fury.io/py/constrained-linear-regression.svg)](https://badge.fury.io/py/constrained-linear-regression)
-        
-        This is a Python implementation of constrained linear regression in scikit-learn style. 
-        The current version supports upper and lower bound for each slope coefficient.
-        
-        It was developed after this question https://stackoverflow.com/questions/50410037
-        
-        Installation:
-        ```pip install constrained-linear-regression```
-        
-        You can use this model, for example, if you want all coefficients to be non-negative:
-        
-        ```Python
-        from constrained_linear_regression import ConstrainedLinearRegression
-        from sklearn.datasets import load_boston
-        from sklearn.linear_model import LinearRegression
-        X, y = load_boston(return_X_y=True)
-        model = ConstrainedLinearRegression(nonnegative=True)
-        model.fit(X, y)
-        print(model.intercept_)
-        print(model.coef_)
-        ```
-        The output will be like
-        ```commandline
-        -36.99292986145538
-        [0.         0.05286515 0.         4.12512386 0.         8.04017956
-         0.         0.         0.         0.         0.         0.02273805
-         0.        ]
-        ```
-        You can also impose arbitrary bounds for any coefficients you choose 
-        ```Python
-        model = ConstrainedLinearRegression()
-        min_coef = np.repeat(-np.inf, X.shape[1])
-        min_coef[0] = 0
-        min_coef[4] = -1
-        max_coef = np.repeat(4, X.shape[1])
-        max_coef[3] = 2
-        model.fit(X, y, max_coef=max_coef, min_coef=min_coef)
-        print(model.intercept_)
-        print(model.coef_)
-        ```
-        The output will be 
-        ```commandline
-        24.060175576410515
-        [ 0.          0.04504673 -0.0354073   2.         -1.          4.
-         -0.01343263 -1.17231216  0.2183103  -0.01375266 -0.7747823   0.01122374
-         -0.56678676]
-        ```
-        
-        You can also set coefficients `lasso` and `ridge` if you want to apply the 
-        corresponding penalties. For `lasso`, however, the output might not be exactly 
-        equal to the result of `sklearn.linear_model.Lasso` due to the difference
-        in the optimization algorithm.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: scikit-learn
+Requires-Dist: numpy
+
+# constrained-linear-regression
+[![PyPI version](https://badge.fury.io/py/constrained-linear-regression.svg)](https://badge.fury.io/py/constrained-linear-regression)
+
+This is a Python implementation of constrained linear regression in scikit-learn style. 
+The current version supports upper and lower bound for each slope coefficient.
+
+It was developed after this question https://stackoverflow.com/questions/50410037
+
+Installation:
+```pip install constrained-linear-regression```
+
+You can use this model, for example, if you want all coefficients to be non-negative:
+
+```Python
+from constrained_linear_regression import ConstrainedLinearRegression
+from sklearn.datasets import load_boston
+from sklearn.linear_model import LinearRegression
+X, y = load_boston(return_X_y=True)
+model = ConstrainedLinearRegression(nonnegative=True)
+model.fit(X, y)
+print(model.intercept_)
+print(model.coef_)
+```
+The output will be like
+```commandline
+-36.99292986145538
+[0.         0.05286515 0.         4.12512386 0.         8.04017956
+ 0.         0.         0.         0.         0.         0.02273805
+ 0.        ]
+```
+You can also impose arbitrary bounds for any coefficients you choose 
+```Python
+model = ConstrainedLinearRegression()
+min_coef = np.repeat(-np.inf, X.shape[1])
+min_coef[0] = 0
+min_coef[4] = -1
+max_coef = np.repeat(4, X.shape[1])
+max_coef[3] = 2
+model.fit(X, y, max_coef=max_coef, min_coef=min_coef)
+print(model.intercept_)
+print(model.coef_)
+```
+The output will be 
+```commandline
+24.060175576410515
+[ 0.          0.04504673 -0.0354073   2.         -1.          4.
+ -0.01343263 -1.17231216  0.2183103  -0.01375266 -0.7747823   0.01122374
+ -0.56678676]
+```
+
+You can also set coefficients `lasso` and `ridge` if you want to apply the 
+corresponding penalties. For `lasso`, however, the output might not be exactly 
+equal to the result of `sklearn.linear_model.Lasso` due to the difference
+in the optimization algorithm.
```

### Comparing `constrained_linear_regression-0.0.4/README.md` & `constrained_linear_regression-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `constrained_linear_regression-0.0.4/constrained_linear_regression.egg-info/PKG-INFO` & `constrained_linear_regression-0.0.5/constrained_linear_regression.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 Metadata-Version: 2.1
-Name: constrained-linear-regression
-Version: 0.0.4
+Name: constrained_linear_regression
+Version: 0.0.5
 Summary: Constrained linear regression in scikit-learn style
 Home-page: https://github.com/avidale/constrained-linear-regression
 Author: David Dale
 Author-email: dale.david@mail.ru
 License: MIT
-Description: # constrained-linear-regression
-        [![PyPI version](https://badge.fury.io/py/constrained-linear-regression.svg)](https://badge.fury.io/py/constrained-linear-regression)
-        
-        This is a Python implementation of constrained linear regression in scikit-learn style. 
-        The current version supports upper and lower bound for each slope coefficient.
-        
-        It was developed after this question https://stackoverflow.com/questions/50410037
-        
-        Installation:
-        ```pip install constrained-linear-regression```
-        
-        You can use this model, for example, if you want all coefficients to be non-negative:
-        
-        ```Python
-        from constrained_linear_regression import ConstrainedLinearRegression
-        from sklearn.datasets import load_boston
-        from sklearn.linear_model import LinearRegression
-        X, y = load_boston(return_X_y=True)
-        model = ConstrainedLinearRegression(nonnegative=True)
-        model.fit(X, y)
-        print(model.intercept_)
-        print(model.coef_)
-        ```
-        The output will be like
-        ```commandline
-        -36.99292986145538
-        [0.         0.05286515 0.         4.12512386 0.         8.04017956
-         0.         0.         0.         0.         0.         0.02273805
-         0.        ]
-        ```
-        You can also impose arbitrary bounds for any coefficients you choose 
-        ```Python
-        model = ConstrainedLinearRegression()
-        min_coef = np.repeat(-np.inf, X.shape[1])
-        min_coef[0] = 0
-        min_coef[4] = -1
-        max_coef = np.repeat(4, X.shape[1])
-        max_coef[3] = 2
-        model.fit(X, y, max_coef=max_coef, min_coef=min_coef)
-        print(model.intercept_)
-        print(model.coef_)
-        ```
-        The output will be 
-        ```commandline
-        24.060175576410515
-        [ 0.          0.04504673 -0.0354073   2.         -1.          4.
-         -0.01343263 -1.17231216  0.2183103  -0.01375266 -0.7747823   0.01122374
-         -0.56678676]
-        ```
-        
-        You can also set coefficients `lasso` and `ridge` if you want to apply the 
-        corresponding penalties. For `lasso`, however, the output might not be exactly 
-        equal to the result of `sklearn.linear_model.Lasso` due to the difference
-        in the optimization algorithm.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: scikit-learn
+Requires-Dist: numpy
+
+# constrained-linear-regression
+[![PyPI version](https://badge.fury.io/py/constrained-linear-regression.svg)](https://badge.fury.io/py/constrained-linear-regression)
+
+This is a Python implementation of constrained linear regression in scikit-learn style. 
+The current version supports upper and lower bound for each slope coefficient.
+
+It was developed after this question https://stackoverflow.com/questions/50410037
+
+Installation:
+```pip install constrained-linear-regression```
+
+You can use this model, for example, if you want all coefficients to be non-negative:
+
+```Python
+from constrained_linear_regression import ConstrainedLinearRegression
+from sklearn.datasets import load_boston
+from sklearn.linear_model import LinearRegression
+X, y = load_boston(return_X_y=True)
+model = ConstrainedLinearRegression(nonnegative=True)
+model.fit(X, y)
+print(model.intercept_)
+print(model.coef_)
+```
+The output will be like
+```commandline
+-36.99292986145538
+[0.         0.05286515 0.         4.12512386 0.         8.04017956
+ 0.         0.         0.         0.         0.         0.02273805
+ 0.        ]
+```
+You can also impose arbitrary bounds for any coefficients you choose 
+```Python
+model = ConstrainedLinearRegression()
+min_coef = np.repeat(-np.inf, X.shape[1])
+min_coef[0] = 0
+min_coef[4] = -1
+max_coef = np.repeat(4, X.shape[1])
+max_coef[3] = 2
+model.fit(X, y, max_coef=max_coef, min_coef=min_coef)
+print(model.intercept_)
+print(model.coef_)
+```
+The output will be 
+```commandline
+24.060175576410515
+[ 0.          0.04504673 -0.0354073   2.         -1.          4.
+ -0.01343263 -1.17231216  0.2183103  -0.01375266 -0.7747823   0.01122374
+ -0.56678676]
+```
+
+You can also set coefficients `lasso` and `ridge` if you want to apply the 
+corresponding penalties. For `lasso`, however, the output might not be exactly 
+equal to the result of `sklearn.linear_model.Lasso` due to the difference
+in the optimization algorithm.
```

### Comparing `constrained_linear_regression-0.0.4/setup.py` & `constrained_linear_regression-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = description
 if os.path.exists("README.md"):
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 setuptools.setup(
     name="constrained_linear_regression",
-    version="0.0.4",
+    version="0.0.5",
     author="David Dale",
     author_email="dale.david@mail.ru",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/avidale/constrained-linear-regression",
     packages=setuptools.find_packages(),
@@ -21,11 +21,11 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'scikit-learn<=1.1',
-        'numpy',
+        "scikit-learn",
+        "numpy",
     ],
 )
```

