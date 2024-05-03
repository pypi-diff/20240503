# Comparing `tmp/dualbounds-0.2.1.tar.gz` & `tmp/dualbounds-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualbounds-0.2.1.tar", last modified: Mon Feb 26 05:53:32 2024, max compression
+gzip compressed data, was "dualbounds-1.0.0.tar", last modified: Fri May  3 18:48:55 2024, max compression
```

## Comparing `dualbounds-0.2.1.tar` & `dualbounds-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 05:53:32.439011 dualbounds-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     3327 2024-02-26 05:53:32.439011 dualbounds-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2371 2024-01-11 14:24:27.000000 dualbounds-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 05:53:32.436011 dualbounds-0.2.1/dualbounds/
--rw-r--r--   0 root         (0) root         (0)      128 2024-02-26 05:52:43.000000 dualbounds-0.2.1/dualbounds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3833 2024-02-26 00:25:26.000000 dualbounds-0.2.1/dualbounds/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     4817 2024-02-26 05:52:43.000000 dualbounds-0.2.1/dualbounds/delta.py
--rw-r--r--   0 root         (0) root         (0)    22209 2024-02-26 00:25:26.000000 dualbounds-0.2.1/dualbounds/dist_reg.py
--rw-r--r--   0 root         (0) root         (0)     8431 2024-02-26 00:25:26.000000 dualbounds-0.2.1/dualbounds/gen_data.py
--rw-r--r--   0 root         (0) root         (0)    28419 2024-02-26 05:52:43.000000 dualbounds-0.2.1/dualbounds/generic.py
--rw-r--r--   0 root         (0) root         (0)     2517 2024-02-26 00:25:26.000000 dualbounds-0.2.1/dualbounds/interpolation.py
--rw-r--r--   0 root         (0) root         (0)    18092 2024-02-26 00:25:26.000000 dualbounds-0.2.1/dualbounds/lee.py
--rw-r--r--   0 root         (0) root         (0)    11561 2024-02-26 05:52:43.000000 dualbounds-0.2.1/dualbounds/utilities.py
--rw-r--r--   0 root         (0) root         (0)     3548 2023-12-25 04:43:42.000000 dualbounds-0.2.1/dualbounds/varcate.py
--rw-r--r--   0 root         (0) root         (0)     3247 2024-02-26 04:51:10.000000 dualbounds-0.2.1/dualbounds/varite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 05:53:32.437011 dualbounds-0.2.1/dualbounds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3327 2024-02-26 05:53:32.000000 dualbounds-0.2.1/dualbounds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2024-02-26 05:53:32.000000 dualbounds-0.2.1/dualbounds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 05:53:32.000000 dualbounds-0.2.1/dualbounds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-26 05:53:32.000000 dualbounds-0.2.1/dualbounds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-26 05:53:32.000000 dualbounds-0.2.1/dualbounds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-26 05:53:32.439011 dualbounds-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1321 2024-02-26 00:25:26.000000 dualbounds-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 05:53:32.439011 dualbounds-0.2.1/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-21 06:09:47.000000 dualbounds-0.2.1/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-12-22 19:17:19.000000 dualbounds-0.2.1/test/context.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-02-26 00:25:26.000000 dualbounds-0.2.1/test/test_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     1809 2024-02-26 05:52:43.000000 dualbounds-0.2.1/test/test_delta.py
--rw-r--r--   0 root         (0) root         (0)     3886 2024-02-26 00:25:26.000000 dualbounds-0.2.1/test/test_dist_reg.py
--rw-r--r--   0 root         (0) root         (0)     9491 2024-02-26 00:25:26.000000 dualbounds-0.2.1/test/test_generic.py
--rw-r--r--   0 root         (0) root         (0)     1092 2024-02-26 00:25:26.000000 dualbounds-0.2.1/test/test_interp.py
--rw-r--r--   0 root         (0) root         (0)    11905 2024-01-11 13:40:09.000000 dualbounds-0.2.1/test/test_lee.py
--rw-r--r--   0 root         (0) root         (0)     3552 2024-02-26 00:25:26.000000 dualbounds-0.2.1/test/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     4067 2024-02-26 00:25:26.000000 dualbounds-0.2.1/test/test_varbounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.466821 dualbounds-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     3327 2024-05-03 18:48:55.466821 dualbounds-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2371 2024-01-11 14:24:27.000000 dualbounds-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.465821 dualbounds-1.0.0/dualbounds/
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-30 02:35:02.000000 dualbounds-1.0.0/dualbounds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/delta.py
+-rw-r--r--   0 root         (0) root         (0)    24096 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/dist_reg.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/gen_data.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/generic.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/interpolation.py
+-rw-r--r--   0 root         (0) root         (0)    23650 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/lee.py
+-rw-r--r--   0 root         (0) root         (0)    13631 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/varcate.py
+-rw-r--r--   0 root         (0) root         (0)     3249 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/varite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.465821 dualbounds-1.0.0/dualbounds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3327 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 18:48:55.466821 dualbounds-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-04-30 02:35:02.000000 dualbounds-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.466821 dualbounds-1.0.0/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-21 06:09:47.000000 dualbounds-1.0.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-12-22 19:17:19.000000 dualbounds-1.0.0/test/context.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_delta.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-02-26 00:25:26.000000 dualbounds-1.0.0/test/test_dist_reg.py
+-rw-r--r--   0 root         (0) root         (0)    10928 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_generic.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2024-02-26 00:25:26.000000 dualbounds-1.0.0/test/test_interp.py
+-rw-r--r--   0 root         (0) root         (0)    13179 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_lee.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-02-26 00:25:26.000000 dualbounds-1.0.0/test/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_varbounds.py
```

### Comparing `dualbounds-0.2.1/PKG-INFO` & `dualbounds-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualbounds
-Version: 0.2.1
+Version: 1.0.0
 Summary: Dual bounds for model-agnostic inference
 Home-page: https://github.com/amspector100/dualbounds/
 Author: Asher Spector
 Author-email: amspector100@gmail.com
 License: UNKNOWN
 Description: A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://amspector100.github.io/dualbounds/ for detailed documentation and tutorials.
```

### Comparing `dualbounds-0.2.1/README.md` & `dualbounds-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dualbounds-0.2.1/dualbounds/bootstrap.py` & `dualbounds-1.0.0/dualbounds/bootstrap.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 import numpy as np
+import pandas as pd
 from scipy import stats
 from .utilities import vrange
 from .generic import DualBounds
 
 def multiplier_bootstrap(
-	samples, 
-	alpha,
-	B=1000, 
-	maxarrsize=int(1e10),
-	param='max',
-	verbose=False,
+	samples: np.array, 
+	alpha: float,
+	B: int=1000, 
+	maxarrsize: int=int(1e10),
+	param: str='max',
+	verbose: int=False,
 ):
 	"""
-	Computes a lower confidence bound on the max(mu),
-	where mu is the vector of means of ``samples``.
+	Computes multiplier bootstrap lower confidence bounds. 
+
+	Precisely, computes a lower confidence bound on
+	:math:`\max(\mu_1, \dots, \mu_d)`,
+	where :math:`\mu_i` is the mean of ``samples[i]``.
 
 	Parameters
 	----------
 	samples : np.array
 		(n,d)-shaped array where samples[i]
-		is i.i.d. with mean mui.
+		is i.i.d. with mean :math:`\mu_i`.
 	alpha : float
 		Nominal error control level.
 	B : int
 		Number of bootstrap replications
 	maxarrsize : float
-		Maximum size of an array; used to
-		save memory.
+		Maximum size of an array; used to save memory.
 	param : str
-		If param='max', computes a lower CB on max(mu).
-		Else, computes an upper CB on min(mu).
+		
+		- If param='max', computes a lower confidence bound on :math:`\max(\mu_1, \dots, \mu_d)`.
+		- Else, computes an upper confidence bound on :math:`\min(\mu_1, \dots, \mu_d)`,
+
 	verbose : bool
 		If True, shows a progress bar. Only useful
 		if ``samples`` is a very large matrix.
 
 	Returns
 	-------
 	estimate : float
-		Estimate of max(mu1, ..., mud).
+		Estimate of :math:`\max(\mu_1, \dots, \mu_d)`.
 	ci : float
-		Lower confidence bound on max(mu1, ..., mud).
+		Lower confidence bound on :math:`\max(\mu_1, \dots, \mu_d)`.
 	"""
 	if param != 'max':
 		estimate, ci = multiplier_bootstrap(
 			samples=-1 * samples, 
 			alpha=alpha, 
 			B=B, 
 			maxarrsize=maxarrsize,
@@ -94,15 +99,15 @@
 	return estimate, ci
 
 def dualbound_multiplier_bootstrap(
 	db_objects: list[DualBounds], 
 	aipw: bool=True,
 	alpha: float=0.1,
 	**kwargs,
-) -> dict:
+) -> pd.DataFrame:
 	"""
 	Combines evidence across multiple DualBounds classes
 	using the multiplier bootstrap.
 
 	Parameters
 	----------
 	db_objects : list
@@ -112,22 +117,16 @@
 		(highly recommended).
 	alpha : float
 		Nominal level, between 0 and 1.
 	kwargs : dict
 		kwargs for dualbounds.bootstrap.multiplier_bootstrap.
 	Returns
 	-------
-	Returns a dictionary with the following attributes:
-
-	estimates : np.array
-		array of lower and upper estimates. These in 
-		general may be biased.
-	cis : np.array
-		1 - alpha confidence lower/upper bounds on 
-		the partial identification bounds.
+	result : pd.DataFrame
+		dataframe of results.
 	"""
 	# Fetch summands
 	if aipw:
 		summands = [x.aipw_summands for x in db_objects]
 	else:
 		summands = [x.ipw_summands for x in db_objects]
 
@@ -147,11 +146,12 @@
 		param='min',
 		alpha=alpha/2,
 		**kwargs
 	)
 	# Return
 	estimates = np.array([lower_est, upper_est])
 	cis = np.array([lower_ci, upper_ci])
-	return dict(
-		estimates=estimates,
-		cis=cis,
+	return pd.DataFrame(
+		np.stack([estimates, cis], axis=0),
+		index=['Estimate', 'Conf. Int'],
+		columns=['Lower', 'Upper'],
 	)
```

### Comparing `dualbounds-0.2.1/dualbounds/delta.py` & `dualbounds-1.0.0/dualbounds/delta.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,66 +4,71 @@
 import ot
 from scipy import stats
 from . import utilities
 from .generic import DualBounds
 
 class DeltaDualBounds(DualBounds):
 	"""
-	Performs inference on
+	Computes generalized dual bounds via the delta method.
 
-	h(E[f(Y(0), Y(1), X)], E[z_1(Y(1), X)], E[z_0(Y(0), X)])
+	The estimand is
 
-	where h is monotone increasing in its first argument.
-	This wraps ``dualbounds.generic.DualBounds`` and applies
-	the bootstrap or delta method. 
+	:math:`h(E[f(Y(0), Y(1), X)], E[z_1(Y(1), X)], E[z_0(Y(0), X)])`
 
+	where h must be monotone increasing in its first argument. 
+	
 	Parameters
 	----------
 	h : function
 		real-valued function of fval, z0, z1, e.g.,
 		``h = lambda fval, z0, z1 : fval / z0 + z1``.
 	z0 : function
-		potentially vector-valued function of y0, x.
+		vector-valued function of y0, x.
 	z1 : function
-		potentially vector-valued function of y1, x.
+		vector-valued function of y1, x.
 	f : function
 		Function which defines the partially identified estimand.
 		Must be a function of three arguments: y0, y1, x 
 		(in that order). E.g.,
 		``f = lambda y0, y1, x : y0 <= y1``
-	X : np.array
-		(n, p)-shaped array of covariates.
-	W : np.array
-		n-length array of binary treatment indicators.
-	Y : np.array
-		n-length array of outcome measurements.
-	pis : np.array
-		n-length array of propensity scores P(W=1 | X). 
+	outcome : np.array | pd.Series
+		n-length array of outcome measurements (Y).
+	treatment : np.array | pd.Series
+		n-length array of binary treatment (W).
+	covariates : np.array | pd.Series
+		(n, p)-shaped array of covariates (X).
+	propensities : np.array | pd.Series
+		n-length array of propensity scores :math:`P(W=1 | X)`. 
 		If ``None``, will be estimated from the data.
-	Y_model : str or dist_reg.DistReg
-		One of ['ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'].
-		Alternatively, a distributional regression class inheriting 
-		from ``dist_reg.DistReg``. E.g., when ``y`` is continuous,
-		defaults to
-		``Y_model=dist_reg.CtsDistReg(
-			model_type='ridge', heterosked_model=None
-		)``.
-	W_model : str or sklearn classifier
-		Specifies how to estimate the propensity scores if ``pis`` is
-		not known.  Either a str identifier as above or an sklearn
-		classifier---see the tutorial for examples.
+	outcome_model : str | dist_reg.DistReg
+		The model for estimating the law of :math:`Y \mid X, W`.
+		Two options:
+
+		- A str identifier, e.g., 'ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'.
+		- An object inheriting from ``dist_reg.DistReg``. 
+
+		E.g., when ``outcome`` is continuous, the default is
+		``outcome_model=dist_reg.CtsDistReg(model_type='ridge')``.
+	propensity_model : str | sklearn classifier
+		How to estimate the propensity scores if they are not provided.
+		Two options:
+
+		- A str identifier, e.g., 'ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'.
+		- An sklearn classifier, e.g., ``sklearn.linear_model.LogisticRegressionCV()``.
 	discrete : bool
-		If True, treats y as a discrete variable. 
+		If True, treats the outcome as a discrete variable. 
 		Defaults to ``None`` (inferred from the data).
 	support : np.array
-		Optinal support of y, if known.
+		Optional support of the outcome, if known and discrete.
 		Defaults to ``None`` (inferred from the data).
-	**model_kwargs : dict
-		Additional kwargs for the ``DistReg`` outcome model,
-		e.g., ``eps_dist`` (for cts. y) or ``feature_transform``.
+	model_kwargs : dict
+		Additional kwargs for the ``outcome_model``, e.g.,
+		``feature_transform``. See 
+		:class:`dualbounds.dist_reg.CtsDistReg` or 
+		:class:`dualbounds.dist_reg.BinaryDistReg` for more kwargs.
 	"""
 	def __init__(
 		self, 
 		h: callable, 
 		z1: callable, 
 		z0: callable,
 		*args,
@@ -71,15 +76,15 @@
 	) -> None:
 		self.h = h
 		self.z1 = z1
 		self.z0 = z0
 		#self.h_grad = h_grad
 		super().__init__(*args, **kwargs)
 
-	def compute_final_bounds(
+	def _compute_final_bounds(
 		self, 
 		aipw: bool=True,
 		alpha: float=0.05,
 		B: int=1000
 	):
 		"""
 		Computes final bounds based on (A)IPW summands,
```

### Comparing `dualbounds-0.2.1/dualbounds/dist_reg.py` & `dualbounds-1.0.0/dualbounds/dist_reg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import numpy as np
+import pandas as pd
 import cvxpy as cp
 from scipy import stats
 import sklearn.linear_model as lm
 from . import utilities
 from .utilities import parse_dist, BatchedCategorical, vrange
 # typing
 import sklearn.base
@@ -53,14 +54,66 @@
 
 def create_folds(n, nfolds):
 	splits = np.linspace(0, n, nfolds+1).astype(int)
 	starts = splits[0:-1]
 	ends = splits[1:]
 	return starts, ends
 
+def _evaluate_model_predictions(y, haty, tol=1e-9):
+	# Preliminaries
+	n = len(y)
+	resids = y - haty
+	ybar_loo = (n * y.mean() - y) / (n-1)
+	resids_null = y - ybar_loo
+	# RMSE calculations
+	rmse = np.sqrt(np.mean(resids**2))
+	rmse_null = np.sqrt(np.mean(resids_null**2))
+	oos_r2 = 1 - rmse**2 / rmse_null**2
+	# Accuracy/likelihood/MAE calculations
+	if set(list(np.unique(y))) == set([0,1]):
+		y = y.astype(int)
+		# accuracy
+		haty_round = np.round(np.clip(haty, 0, 1)).astype(int)
+		accuracy = (haty_round == y).astype(float)
+		accuracy[haty == 0.5] = 0.5
+		accuracy = np.mean(accuracy)
+		# null model accuracy
+		null_accuracy = (np.round(ybar_loo).astype(int) == y).astype(float)
+		null_accuracy[ybar_loo == 0.5] = 0.5
+		null_accuracy = np.mean(null_accuracy)
+		# likelihood
+		haty = np.clip(haty, tol, 1-tol)
+		lls = np.log(haty) * y + np.log(1-haty) * (1 - y)
+		ybar_loo = np.clip(ybar_loo, tol, 1-tol)
+		null_lls = np.log(ybar_loo) * y + np.log(1-ybar_loo) * (1-y)
+		# take geometric mean
+		likelihood_geom = np.exp(lls.mean())
+		null_likelihood_geom = np.exp(null_lls.mean())
+		return pd.DataFrame(
+			np.array([
+				[oos_r2, 0],
+				[accuracy, null_accuracy],
+				[likelihood_geom, null_likelihood_geom]
+			]),
+			index=['Out-of-sample R^2', 'Accuracy', 'Likelihood (geom. mean)'],
+			columns=['Model', 'No covariates'],
+		)
+	else:   
+		mae = np.mean(np.abs(resids))
+		mae_null = np.mean(np.abs(resids_null))
+		return pd.DataFrame(
+			np.array([
+				[oos_r2, 0],
+				[rmse, rmse_null],
+				[mae, mae_null]
+			]),
+			index=['Out-of-sample R^2', 'RMSE', 'MAE'],
+			columns=['Model', 'No covariates'],
+		)
+
 def ridge_loo_resids(
 	features, y, ridge_cv_model
 ):
 	# Ensure we add an intercept which is unregularized
 	n, p = features.shape
 	if ridge_cv_model.fit_intercept:
 		# This is not *exact* if we fit an intercept
@@ -86,15 +139,15 @@
 
 def cross_fit_predictions(
 	W,
 	X,
 	y,
 	S=None,
 	nfolds=2,
-	train_on_selections=False,
+	train_on_selections=True,
 	model=None,
 	model_cls=None, 
 	probs_only=False,
 	verbose=False,
 	**model_kwargs
 ):
 	"""
@@ -193,14 +246,15 @@
 	Parameters
 	----------
 	how_transform : str
 		Str specifying how to transform the features before fitting
 		the underlying model. One of several options:
 
 		- 'identity': does not transform the features
+		- 'intercept': adds an intercept
 		- 'interactions' : interaction terms btwn. the treatment/covariates
 
 		The default is ``interactions``.
 	"""
 
 	def __init__(self, how_transform):
 		self.how_transform = how_transform
@@ -235,14 +289,16 @@
 		Returns
 		-------
 		features : np.array
 			(n, d)-shaped array of features.
 		"""
 		if self.how_transform in ['none', 'identity']:
 			return np.concatenate([W.reshape(-1, 1), X],axis=1)
+		elif self.how_transform in ['intercept']:
+			return np.concatenate([W.reshape(-1, 1), np.ones((len(X), 1)), X],axis=1)
 		elif self.how_transform in [
 			'int', 'interaction', 'interactions'
 		]:
 			return np.concatenate([
 				W.reshape(-1, 1), W.reshape(-1, 1) * X, X], axis=1
 			)
 		else:
@@ -632,15 +688,15 @@
 			raise ValueError(f"y must be binary; instead np.unique(y)={np.unique(y)}")
 		# fit 
 		features = self.feature_transform(W=W, X=X)
 		self.model = self.model_type(**self.model_kwargs)
 		self.model.fit(features, y)
 
 	def predict_proba(
-		self, X: np.array, W: Optional[np.array]=None
+		self, X: np.array, W: Optional[np.array]=None, margin=0.005,
 	):
 		"""
 		If W is None, returns (P(Y = 1 | W = 0, X), P(Y = 1 | W = 1, X))
 		Else, returns P(Y = 1 | W , X) 
 		"""
 		if W is not None:
 			# return predict P(Y = 1 | X, W)
@@ -652,18 +708,18 @@
 			n = len(X)
 			W0 = np.zeros(n); W1 = np.ones(n)
 			p0s, p1s = self.predict_proba(X, W=W0), self.predict_proba(X, W=W1)
 			p0s = np.minimum(1-TOL, np.maximum(TOL, p0s))
 			p1s = np.minimum(1-TOL, np.maximum(TOL, p1s))
 			# enforce monotonicity
 			if self.monotonicity:
-				flags = p0s > p1s
+				flags = p0s > p1s - margin
 				avg = (p0s[flags] + p1s[flags]) / 2
-				p0s[flags] = np.maximum(TOL, avg-TOL)
-				p1s[flags] = np.minimum(1-TOL, avg+TOL)
+				p0s[flags] = np.maximum(TOL, avg-margin)
+				p1s[flags] = np.minimum(1-TOL, avg+margin)
 			return p0s, p1s
 
 	def predict(self, X: np.array, W: Optional[np.array]=None):
 		"""
 		If W is None, returns (y0_dists, y1_dists)
 		Else, returns (y_dists) 
 		"""
@@ -683,28 +739,30 @@
 			return self.predict(X, W=W0), self.predict(X, W=W1)
 
 class MonotoneLogisticReg:
 	"""
 	A logistic regression solver which ensures that beta[0] >= 0.
 	Useful for computing Lee bounds which assume monotonicity.
 	"""
-	def __init__(self):
-		pass
+	def __init__(self, lmda: float=0.001):
+		self.lmda = lmda
 
-	def fit(self, X: np.array, y: np.array, lmda: float=1):
+	def fit(self, X: np.array, y: np.array):
+		# Set up data and losses
 		n, p = X.shape
 		sig1 = X[:, 0].std()
 		zeros = np.zeros(n)
 		beta = cp.Variable(p)
 		X1beta = X @ beta
 		term1 = cp.multiply(y, X1beta)
 		term2 = cp.log_sum_exp(cp.vstack([zeros, X1beta]), axis=0)
-		term3 = lmda * cp.sum(cp.power(beta, 2))
+		term3 = n * self.lmda * cp.sum(cp.power(beta[1:], 2))
+		# Objective and problem
 		obj = cp.Maximize(cp.sum(term1 - term2) - term3)
-		problem = cp.Problem(objective=obj, constraints=[beta[0] >= 0.1 / sig1])
+		problem = cp.Problem(objective=obj, constraints=[beta[0] >= 0])
 		try:
 			problem.solve(solver='ECOS', max_iters=100)
 		except cp.error.SolverError:
 			problem.solve(solver='ECOS', max_iters=500)
 		self.beta = beta.value
 
 	def predict_proba(self, X: np.array):
```

### Comparing `dualbounds-0.2.1/dualbounds/generic.py` & `dualbounds-1.0.0/dualbounds/generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import warnings
 import numpy as np
 import ot
 from scipy import stats
 from . import utilities, dist_reg, interpolation
 from .utilities import BatchedCategorical
+import pandas as pd
 # typing
 from scipy.stats._distn_infrastructure import rv_generic
 import sklearn.base
 from typing import Optional, Union
 
 MIN_NVALS = 7
 DISC_THRESH = 2 # treat vars. with <= DISC_THRESH values as discrete
@@ -18,25 +19,25 @@
 directly provided. Please ensure cross-fitting is
 employed correctly, else inference will be invalid
 (see https://arxiv.org/abs/2310.08115). To suppress
 this warning, set ``supress_warning=True``.
 ==================================================
 """
 
-def get_default_model(discrete, support, Y_model=None, **model_kwargs):
-	if isinstance(Y_model, dist_reg.DistReg):
-		return Y_model
-	Y_model = 'ridge' if Y_model is None else Y_model
+def get_default_model(discrete, support, outcome_model=None, **model_kwargs):
+	if isinstance(outcome_model, dist_reg.DistReg):
+		return outcome_model
+	outcome_model = 'ridge' if outcome_model is None else outcome_model
 	if not discrete:
 		return dist_reg.CtsDistReg(
-			model_type=Y_model, **model_kwargs
+			model_type=outcome_model, **model_kwargs
 		)
 	elif discrete and set(support) == set([0, 1]):
 		return dist_reg.BinaryDistReg(
-			model_type=Y_model, **model_kwargs
+			model_type=outcome_model, **model_kwargs
 		)
 	else:
 		raise NotImplementedError("Currently no default for non-binary discrete data")
 
 def infer_discrete(discrete, support, y):
 	n = len(y)
 	### Check if discrete
@@ -74,121 +75,167 @@
 		y1_min = 1.5 * y.min() - y.max() / 2
 	if y0_max is None:
 		y0_max = 1.5 * y.max() - y.min() / 2
 	if y1_max is None:
 		y1_max = 1.5 * y.max() - y.min() / 2
 	return y0_min, y1_min, y0_max, y1_max
 
-
 class DualBounds:
 	"""
-	Computes dual bounds on E[f(Y(0),Y(1), X)].
+	Computes dual bounds on :math:`E[f(Y(0),Y(1), X)].`
+
+	Here, :math:`X` are covariates and :math:`Y(0), Y(1)` are 
+	potential outcomes.
 
 	Parameters
 	----------
 	f : function
 		Function which defines the partially identified estimand.
 		Must be a function of three arguments: y0, y1, x 
 		(in that order). E.g.,
 		``f = lambda y0, y1, x : y0 <= y1``
-	X : np.array
-		(n, p)-shaped array of covariates.
-	W : np.array
-		n-length array of binary treatment indicators.
-	Y : np.array
-		n-length array of outcome measurements.
-	pis : np.array
-		n-length array of propensity scores P(W=1 | X). 
+	outcome : np.array | pd.Series
+		n-length array of outcome measurements (Y).
+	treatment : np.array | pd.Series
+		n-length array of binary treatment (W).
+	covariates : np.array | pd.Series
+		(n, p)-shaped array of covariates (X).
+	propensities : np.array | pd.Series
+		n-length array of propensity scores :math:`P(W=1 | X)`. 
 		If ``None``, will be estimated from the data.
-	Y_model : str or dist_reg.DistReg
-		One of ['ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'].
-		Alternatively, a distributional regression class inheriting 
-		from ``dist_reg.DistReg``. E.g., when ``y`` is continuous,
-		defaults to
-		``Y_model=dist_reg.CtsDistReg(
-			model_type='ridge', heterosked_model=None
-		)``.
-	W_model : str or sklearn classifier
-		Specifies how to estimate the propensity scores if ``pis`` is
-		not known.  Either a str identifier as above or an sklearn
-		classifier---see the tutorial for examples.
+	outcome_model : str | dist_reg.DistReg
+		The model for estimating the law of :math:`Y \mid X, W`.
+		Two options:
+
+		- A str identifier, e.g., 'ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'.
+		- An object inheriting from ``dist_reg.DistReg``. 
+
+		E.g., when ``outcome`` is continuous, the default is
+		``outcome_model=dist_reg.CtsDistReg(model_type='ridge')``.
+	propensity_model : str | sklearn classifier
+		How to estimate the propensity scores if they are not provided.
+		Two options:
+
+		- A str identifier, e.g., 'ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'.
+		- An sklearn classifier, e.g., ``sklearn.linear_model.LogisticRegressionCV()``.
 	discrete : bool
-		If True, treats y as a discrete variable. 
+		If True, treats the outcome as a discrete variable. 
 		Defaults to ``None`` (inferred from the data).
 	support : np.array
-		Optinal support of y, if known.
+		Optional support of the outcome, if known and discrete.
 		Defaults to ``None`` (inferred from the data).
-	**model_kwargs : dict
-		Additional kwargs for the ``DistReg`` outcome model,
-		e.g., ``eps_dist`` (for cts. y) or ``feature_transform``.
+	model_kwargs : dict
+		Additional kwargs for the ``outcome_model``, e.g.,
+		``feature_transform``. See 
+		:class:`dualbounds.dist_reg.CtsDistReg` or 
+		:class:`dualbounds.dist_reg.BinaryDistReg` for more kwargs.
+
+	Notes
+	-----
+	``DualBounds`` will do limited preprocessing to (e.g.) create 
+	dummies for discrete covariates. However, we recommended doing
+	custom preprocessing for optimal results.
 
 	Examples
 	--------
-	Here we fit DualBounds on P(Y(0) < Y(1)) based on
+	Here we fit DualBounds on :math:`P(Y(0) < Y(1))` based on
 	synthetic regression data: ::
 		import dualbounds as db
 
-		# Generate synthetic data from a heavy-tailed linear model
-		data = db.gen_data.gen_regression_data(
-			n=900, # Num. datapoints
-			p=30, # Num. covariates
-			r2=0.95, # population R^2
-			tau=3, # average treatment effect
-			interactions=True, # ensures treatment effect is heterogenous
-			eps_dist='laplace', # heavy-tailed residuals
-			sample_seed=123, # random seed
-		)
+		# Generate synthetic data
+		data = db.gen_data.gen_regression_data(n=900, p=30)
 
 		# Initialize dual bounds object
 		dbnd = db.generic.DualBounds(
 			f=lambda y0, y1, x: y0 < y1,
-			X=data['X'], # n x p covariate matrix
-			W=data['W'], # n-length treatment vector
-			y=data['y'], # n-length outcome vector
-			pis=data['pis'], # n-length propensity scores (optional)
-			Y_model='ridge', # model for Y | X, W
+			covariates=data['X'],
+			treatment=data['W'],
+			outcome=data['y'],
+			propensities=data['pis'],
+			outcome_model='ridge',
 		)
 
 		# Compute dual bounds and observe output
-		dbnd.compute_dual_bounds(
-			alpha=0.05 # nominal level
-		)
+		dbnd.fit(alpha=0.05).summary()
 	"""
 	def __init__(
 		self, 
 		f: callable,
-		X: np.array,
-		W: np.array,
-		y: np.array,
-		pis: Optional[np.array]=None,
-		Y_model: Union[str, dist_reg.DistReg]='ridge',
-		W_model: Union[str, sklearn.base.BaseEstimator]='ridge',
+		outcome: Union[np.array, pd.Series],
+		treatment: Union[np.array, pd.Series],
+		covariates: Optional[Union[np.array, pd.DataFrame]]=None,
+		propensities: Optional[Union[np.array, pd.Series]]=None,
+		outcome_model: Union[str, dist_reg.DistReg]='ridge',
+		propensity_model: Union[str, sklearn.base.BaseEstimator]='ridge',
 		discrete: Optional[np.array]=None,
 		support: Optional[np.array]=None,
 		**model_kwargs,
 	) -> None:
-		### Data
+		# Estimand
 		self.f = f
-		self.X = X
-		self.y = y
-		self.W = W
-		self.pis = pis
+
+		### Process outcome
+		self.y = outcome
+		if isinstance(self.y, pd.Series) or isinstance(self.y, pd.DataFrame):
+			self.y = self.y.values
+		if np.any(np.isnan(self.y)):
+			raise ValueError("outcome contains nans")
+		if len(self.y.shape) > 1:
+			if len(self.y.shape) == 2 and self.y.shape[1] == 1:
+				self.y = self.y.flatten()
+			else:
+				raise ValueError("outcome should be a flat array not a matrix")
 		self.n = len(self.y)
 
+		### Treatment
+		if isinstance(treatment, pd.Series) or isinstance(treatment, pd.DataFrame):
+			treatment = treatment.values.reshape(self.n)
+		self.W = utilities._binarize_variable(treatment, var_name='treatment')
+
+		### Process covariates
+		self.X = covariates
+		if self.X is None:
+			self.X = np.zeros((self.n, 1))
+		# limited preprocessing of covariates
+		if isinstance(self.X, pd.DataFrame):
+			self.X = utilities.process_covariates(self.X)
+			self.cov_names = self.X.columns
+			self.X = self.X.values
+		else:
+			if len(self.X.shape) == 1:
+				self.X = self.X.reshape(-1, 1)
+			self.cov_names = np.arange(self.X.shape[1])
+		# fill NAs if existing
+		if np.any(np.isnan(self.X)):
+			self.X = self.X.copy()
+			naninds = np.where(np.isnan(self.X))
+			self.X[naninds] = np.take(np.nanmean(self.X, axis=0), naninds[1])
+
+		### process propensities
+		self.pis = propensities
+		if isinstance(self.pis, pd.Series) or isinstance(self.pis, pd.DataFrame):
+			self.pis = self.pis.values.reshape(self.n)
+		if self.pis is not None:
+			if np.any(np.isnan(self.pis)):
+				raise ValueError(f"propensities (pis) are provided but contains missing values")
+			if np.any(self.pis < 0) or np.any(self.pis > 1):
+				raise ValueError(f"propensities (pis) do not lie within [0,1]")
+
 		### Check if discrete
 		self.discrete, self.support = infer_discrete(
 			discrete=discrete, support=support, y=self.y,
 		)
-		self.Y_model = Y_model
-		self.W_model = W_model
+		self.outcome_model = outcome_model
+		self.propensity_model = propensity_model
 		self.model_kwargs = model_kwargs
 
-		# Initialize
+		## Initialize core objects
 		self.y0_dists = None
 		self.y1_dists = None
+		self.oos_dist_preds = None
 
 	def _discretize(
 		self, 
 		ydists,
 		nvals,
 		ymin,
 		ymax,
@@ -440,87 +487,102 @@
 				lower=1,
 				**kwargs,
 			)
 			return -nu0, -nu1, -objval
 
 	def compute_dual_variables(
 		self,
-		y0_dists=None,
-		y0_vals=None,
-		y0_probs=None,
-		y1_dists=None,
-		y1_vals=None,
-		y1_probs=None,
-		verbose=True,
-		alpha=None,
-		ninterp=None,
-		nvals0=100,
-		nvals1=100,
-		interp_fn=interpolation.adaptive_interpolate,
-		y0_min=None,
-		y0_max=None,
-		y1_min=None,
-		y1_max=None,
+		y0_dists: Optional[list]=None,
+		y0_vals: Optional[np.array]=None,
+		y0_probs: Optional[np.array]=None,
+		y1_dists: Optional[list]=None,
+		y1_vals: Optional[np.array]=None,
+		y1_probs: Optional[np.array]=None,
+		verbose: bool=True,
+		alpha: Optional[float]=None,
+		ninterp: Optional[int]=None,
+		nvals0: int=100,
+		nvals1: int=100,
+		interp_fn: callable=interpolation.adaptive_interpolate,
+		y0_min: Optional[float]=None,
+		y0_max: Optional[float]=None,
+		y1_min: Optional[float]=None,
+		y1_max: Optional[float]=None,
 		**kwargs,
 	):
 		"""
-		Uses the estimated outcome model to solve the dual optimal
-		transport problem to obtain optimal dual variables.
+		Estimates dual variables using the outcome model.
+
+		We generally recommend that the user call .fit() instead of 
+		calling this function directly.
 
 		Parameters
 		----------
-		y0_dists : np.array
-			batched scipy distribution of shape (n,) where the ith
-			distribution is the conditional law of Yi(0) | Xi
-			OR 
-			list of scipy dists whose shapes add up to n.
-		y0_vals : np.array
-			(n, nvals0)-length array of values y0 can take.
+		y0_dists : list
+			The ith distribution of y0_dists represents the conditional
+			law of :math:`Y_i(0) | X_i`. There are two input formats:
+
+			- batched scipy distribution of shape (n,)
+			- list of scipy dists whose shapes add up to n.
+
+		y0_vals : list
+			Alternatively, specify a (n, nvals0)-length array
+			where ``y0_vals[i]`` is the support of :math:`Y_i(0)`.
+			Ignored if ``y0_dists`` is provided.
 		y0_probs : np.array
-			(n, nvals0)-length array where
-			y0_probs[i, j] = P(Y(0) = yvals0[j] | Xi)
-		y1_dists : np.array
-			batched scipy distribution of shape (n,) where the ith
-			distribution is the conditional law of Yi(1) | Xi
-			OR 
-			list of scipy dists whose shapes add up to n.
+			A (n, nvals0)-length array where ``y0_probs[i, j]``
+			is the estimated probability that :math:`Y_i(0)`
+			equals ``y0_vals[i, j].``
+		y1_dists : list
+			The ith distribution of y1_dists represents the conditional
+			law of :math:`Y_i(1) | X_i`. There are two input formats:
+
+			- batched scipy distribution of shape (n,)
+			- list of scipy dists whose shapes add up to n.
+
 		y1_vals : np.array
-			(n, nvals1)-length array of values y1 can take.
-			Ignored if ``y1_dists`` is provided.
+			(n, nvals1)-length array where ``y1_vals[i]`` is the support 
+			of :math:`Y_i(1)`.	Ignored if ``y1_dists`` is provided.
 		y1_probs : np.array
-			(n, nvals1)-length array where
-			y0_probs[i, j] = P(Y(1) = yvals1[j] | Xi).
-			Ignored if ``y1_dists`` is provided.
+			(n, nvals1)-length array where ``y1_probs[i, j]``
+			is the estimated probability that :math:`Y_i(1)`
+			equals ``y1_vals[i, j].``
 		nvals0 : int
 			How many values to use to discretize Y(0). 
 			Defaults to 100. Ignored for discrete Y.
 		nvals1 : int
 			How many values to use to discretize Y(1).
 			Defaults to 100. Ignored for discrete Y.
 		interp_fn : function 
 			An interpolation function with the same input/output
-			signature as ``interpolation.linear_interpolate``,
+			signature as ``interpolation.adaptive_interpolate``,
 			which is the default. Ignored for discrete Y.
 		y0_min : float
 			Minimum support for Y(0).
-			Defaults to self.y.min() - 0.5 * (self.y.max() - self.y.min())
+			Defaults to ``self.y.min() - 0.5 * (self.y.max() - self.y.min())``
 		y1_min : float
 			Minimum support for Y(1). 
-			Defaults to self.y.min() - 0.5 * (self.y.max() - self.y.min())
+			Defaults to ``self.y.min() - 0.5 * (self.y.max() - self.y.min())``
 		y0_max : float
 			Maximum support for Y(0). 
-			Defaults to self.y.max() + 0.5 * (self.y.max() - self.y.min())
+			Defaults to ``self.y.max() + 0.5 * (self.y.max() - self.y.min())``
 		y1_max : float
 			Maximum support for Y(1). 
-			Defaults to self.y.max() + 0.5 * (self.y.max() - self.y.min())
+			Defaults to ``self.y.max() + 0.5 * (self.y.max() - self.y.min())``
 		kwargs : dict
 			kwargs for ``_ensure_feasibility`` method, e.g., ``grid_size``.
+
+		Returns
+		-------
+		None
 		"""
 		### Key quantities for optimizer
 		# to ensure numerical stability, we add extra quantiles
+		if verbose:
+			print("Estimating optimal dual variables.")
 		if min([nvals0, nvals1]) <= MIN_NVALS:
 			raise ValueError(f"nvals0={nvals0}, nvals1={nvals1} must be larger than {MIN_NVALS}")
 		if self.discrete:
 			self.nvals0 = len(self.support)
 			self.nvals1 = len(self.support)
 		else:
 			self.nvals0 = nvals0
@@ -564,16 +626,14 @@
 		self.c0s = np.zeros((2, self.n))
 		self.c1s = np.zeros((2, self.n))
 		# objective values
 		self.objvals = np.zeros((2, self.n))
 		self.dxs = np.zeros((2, self.n)) # ignored, only for backward compatability
 		self.objdiffs = np.zeros((2, self.n))
 		# loop through
-		if verbose:
-			print("Estimating optimal dual variables.")
 		for i in utilities.vrange(self.n, verbose=verbose):
 			# set parameter values
 			fx = lambda y0, y1: self.f(y0=y0, y1=y1, x=self.X[i])
 			fvals = np.array(fx(
 				y0=self.y0_vals[i].reshape(-1, 1), 
 				y1=self.y1_vals[i].reshape(1, -1),
 			))
@@ -601,15 +661,15 @@
 					y1_min=y1_min,
 					y1_max=y1_max,
 					**kwargs
 				)
 
 	def _interpolate_and_ensure_feas(
 		self, yi, lower, i, y0_min, y1_min, y0_max, y1_max, **kwargs
-	):	
+	):  
 		"""
 		This is used in two places:
 		1. _compute_realized_dual_variables
 		2. Main loop of compute_dual_variables
 		"""
 		nu0x = self.nu0s[1-lower, i]
 		nu1x = self.nu1s[1-lower, i]
@@ -629,15 +689,15 @@
 			self.hatnu1s[1 - lower, i] = self.interp_fn(
 				x=y1v, y=nu1adj, newx=yi,
 			)[0]
 		else:
 			j0 = np.where(self.y0_vals[i] == yi)[0][0]
 			j1 = np.where(self.y1_vals[i] == yi)[0][0]
 			self.hatnu0s[1 - lower, i] = nu0x[j0]
-			self.hatnu1s[1 - lower, i] = nu1x[j1]	
+			self.hatnu1s[1 - lower, i] = nu1x[j1]   
 
 
 
 	def _compute_realized_dual_variables(self, y=None, **kwargs):
 		"""
 		Helper function which applies interpolation 
 		(for continuous Y) to compute realized dual variables.
@@ -684,18 +744,17 @@
 			)[self.W == 0]
 			# AIPW
 			mus = self.c1s[1-lower] + self.c0s[1-lower]
 			aipw1 = (self.hatnu1s[1-lower] - self.c1s[1-lower]) / self.pis + mus 
 			aipw0 = (self.hatnu0s[1-lower] - self.c0s[1-lower]) / (1-self.pis) + mus
 			self.aipw_summands[1-lower] = aipw1 * self.W + (1 - self.W) * aipw0
 
-	def compute_final_bounds(self, aipw=True, alpha=0.05):
+	def _compute_final_bounds(self, aipw=True, alpha=0.05):
 		"""
-		Computes final estimators/ses based on the estimated
-		dual variables.
+		Computes final results from the estimated dual variables.
 		"""
 		self._compute_ipw_summands()
 		self.estimates, self.ses, self.cis = utilities.compute_est_bounds(
 			summands=self.aipw_summands if aipw else self.ipw_summands,
 			alpha=alpha
 		)
 		return dict(
@@ -728,169 +787,187 @@
 		else:
 			y1_dists = [self.y1_dists]
 		# Compute
 		self.mu0 = np.concatenate([x.mean() for x in y0_dists])
 		self.mu1 = np.concatenate([x.mean() for x in y1_dists])
 
 	def fit_propensity_scores(
-		self, nfolds, clip=1e-2, verbose=True,
+		self, nfolds: int, clip: float=1e-2, verbose: bool=True,
 	):
 		"""
-		Performs cross-fitting to fit the propensity scores.
+		Cross-fits the propensity scores.
+
+		Parameters
+		----------
+		nfolds : int
+			Number of folds.
+		clip : float
+			Clip propensity scores to be in [clip, 1-clip].
+		verbose : bool
+			If True, prints progress reports.
+
+		Returns
+		-------
+		None
 		"""
 		# Parse model
-		if self.W_model is None:
-			self.W_model = 'ridge'
-		if isinstance(self.W_model, str):
+		if self.propensity_model is None:
+			self.propensity_model = 'ridge'
+		if isinstance(self.propensity_model, str):
 			model_cls = dist_reg.parse_model_type(
-				self.W_model, discrete=True
+				self.propensity_model, discrete=True
 			)
-			self.W_model = model_cls()
+			self.propensity_model = model_cls()
 		
 		# Loop through
 		if verbose:
 			print("Fitting propensity scores.")
 		starts, ends = dist_reg.create_folds(n=self.n, nfolds=nfolds)
 		# loop through and fit
-		self.W_model_fits = []
+		self.propensity_model_fits = []
 		self.pis = np.zeros(self.n)
 		for ii in utilities.vrange(len(starts), verbose=verbose):
 			start, end = starts[ii], ends[ii]
 			# Pick out data from the other folds
 			not_in_fold = [
 				i for i in np.arange(self.n) if i < start or i >= end
 			]
 			# Fit 
-			model_fit = copy.deepcopy(self.W_model)
+			model_fit = copy.deepcopy(self.propensity_model)
 			model_fit.fit(
 				X=self.X[not_in_fold], y=self.W[not_in_fold]
 			)
-			self.W_model_fits.append(model_fit)
+			self.propensity_model_fits.append(model_fit)
 			# Predict out of sample
 			self.pis[start:end] = model_fit.predict_proba(
 				self.X[start:end]
 			)[:, 1]
 
 		# Clip
 		self.pis = np.minimum(np.maximum(self.pis, clip), 1-clip)
 
 	def cross_fit(
 		self,
-		nfolds=5,
-		suppress_warning=False,
-		verbose=True,
+		nfolds: int=5,
+		suppress_warning: bool=False,
+		verbose: bool=True,
 	):
 		"""
-		Performs cross-fitting to fit the outcome model.
+		Cross-fits the outcome model.
 
+		Parameters
+		----------
+		nfolds : int
+			Number of folds to use in cross-fitting.
+		suppress_warning : bool
+			If True, suppresses a potential warning about cross-fitting.
+		verbose : bool
+			If True, prints progress reports.
 
 		Returns
 		-------
 		y0_dists : list
 			list of batched scipy distributions whose shapes sum to n.
 			the ith distribution is the out-of-sample estimate of
-			the conditional law of Yi(0) | X[i]
+			the conditional law of :math:`Y_i(0) | X[i]`
 		y1_dists : list
 			list of batched scipy distributions whose shapes sum to n.
 			the ith distribution is the out-of-sample estimate of
-			the conditional law of Yi(1) | X[i]
+			the conditional law of :math:`Y_i(1) | X[i]`
 		"""
 
 		# if pis not supplied: will use cross-fitting
 		if self.pis is None:
 			self.fit_propensity_scores(nfolds=nfolds, verbose=verbose)
 
 		# Fit model
 		if self.y0_dists is None or self.y1_dists is None:
 			# Note: this returns the existing model
 			# if an existing model is provided
-			self.Y_model = get_default_model(
+			self.outcome_model = get_default_model(
 				discrete=self.discrete, 
 				support=self.support,
-				Y_model=self.Y_model,
+				outcome_model=self.outcome_model,
 				**self.model_kwargs
 			)
 			if verbose:
 				print("Cross-fitting the outcome model.")
 			y_out = dist_reg.cross_fit_predictions(
 				W=self.W, X=self.X, y=self.y, 
 				nfolds=nfolds, 
-				model=self.Y_model,
+				model=self.outcome_model,
 				verbose=verbose,
 			)
-			self.y0_dists, self.y1_dists, self.model_fits, self.oos_preds = y_out
+			self.y0_dists, self.y1_dists, self.model_fits, self.oos_dist_preds = y_out
 		elif not suppress_warning:
 			warnings.warn(CROSSFIT_WARNING)
 
 		return self.y0_dists, self.y1_dists
 
-	def compute_oos_r2(self):
-		if not isinstance(self.oos_preds, list):
-			raise NotImplementedError("Only implemented for settings where self.oos_preds is a list of dists")
-		starts, ends = dist_reg.create_folds(
-			n=self.n,
-			nfolds=len(self.oos_preds)
-		)
-		self.oos_resids = np.zeros(self.n)
-		for start, end, oos_preds in zip(starts, ends, self.oos_preds):
-			self.oos_resids[start:end] = self.y[start:end] - oos_preds.mean()
-		return 1 - np.mean(self.oos_resids**2) / np.std(self.y)**2
-
+	def _compute_oos_resids(self):
+		# compute out-of-sample predictions
+		self._compute_cond_means()
+		self.oos_preds = self.mu0.copy()
+		self.oos_preds[self.W == 1] = self.mu1[self.W == 1]
+		# residuals and return
+		self.oos_resids = self.y - self.oos_preds
+		return self.oos_resids
 
-	def compute_dual_bounds(
+	def fit(
 		self,
 		nfolds: int = 5,
 		aipw: bool = True,
 		alpha: float = 0.05,
 		y0_dists: Optional[list[rv_generic]] = None,
 		y1_dists: Optional[list[rv_generic]] = None,
 		verbose: bool = True,
 		suppress_warning: bool = False,
 		**solve_kwargs,
-	) -> dict:
+	):
 		"""
-		Main function which computes dual bounds in three steps:
-		(1) cross-fitting, (2) computing optimal dual variables,
-		and (3) computing final dual bounds.
+		Main function which (1) performs cross-fitting, (2) computes 
+		optimal dual variables, and (3) computes final dual bounds.
 
 		Parameters
-		----------	
+		----------  
 		nfolds : int
 			Number of folds to use when cross-fitting. Defaults to 5.
 		alpha : float
 			Nominal coverage level. Defaults to 0.05.
 		aipw : bool
 			If true, returns AIPW estimator.
 		y0_dists : list
-			list of batched scipy distributions whose shapes sum to n.
-			the ith distribution is an out-of-sample estimate of
-			the law of Yi(0) | X[i]. This is an optional input;
-			if provided, ``Y_model`` will be ignored.
+			The ith distribution of y0_dists represents the conditional
+			law of :math:`Y_i(0) | X_i`. There are two input formats:
+
+			- batched scipy distribution of shape (n,)
+			- list of scipy dists whose shapes add up to n.
+
+			This is an optional input; if provided, ``outcome_model``
+			will be ignored.
 		y1_dists : list
-			list of batched scipy distributions whose shapes sum to n.
-			the ith distribution is an out-of-sample estimate of
-			the law of Yi(1) | X[i]. This is an optional input;
-			if provided, ``Y_model`` will be ignored.
+			The ith distribution of y1_dists represents the conditional
+			law of :math:`Y_i(1) | X_i`. There are two input formats:
+
+			- batched scipy distribution of shape (n,)
+			- list of scipy dists whose shapes add up to n.
+
+			This is an optional input; if provided, ``outcome_model``
+			will be ignored.
 		verbose : bool
 			If True, gives occasional progress reports.
-			Defaults to True.
 		suppress_warning : bool
 			If True, suppresses a warning about cross-fitting.
 		solve_kwargs : dict
 			Additional (optional) kwargs for the ``compute_dual_variables``
 			method, e.g. ``nvals0``, ``nvals1``, ``grid_size``.
 
 		Returns
 		-------
-		estimates : np.array
-			2-length array, estimates of lower/upper partial ident. bound
-		ses : np.array
-			Standard errors of ests
-		cis : np.array
-			Confidence bounds based on ests and ses. 
+		self
 		"""
 		# Fit model of W | X and Y | X if not provided
 		self.y0_dists, self.y1_dists = y0_dists, y1_dists
 		self.cross_fit(
 			nfolds=nfolds, suppress_warning=suppress_warning, verbose=verbose,
 		)
 
@@ -898,45 +975,159 @@
 		self.compute_dual_variables(
 			y0_dists=self.y0_dists,
 			y1_dists=self.y1_dists,
 			verbose=verbose,
 			**solve_kwargs,
 		)
 		# compute dual bounds
-		return self.compute_final_bounds(aipw=aipw, alpha=alpha)
+		self.alpha = alpha
+		self._compute_final_bounds(aipw=aipw, alpha=alpha)
+		return self
+
+	# def _plug_in_results(self):
+	#   pests, pses, pcis = utilities.compute_est_bounds(
+	#       summands=self.objvals,
+	#       alpha=self.alpha
+	#   )
+	#   return pd.DataFrame(
+	#       np.stack(
+	#           [pests, pses, pcis], 
+	#           axis=0
+	#       ),
+	#       index=['Estimate', 'SE', 'Conf. Int.'],
+	#       columns=['Lower', 'Upper']
+	#   )
+
+	def results(self, minval: float=-np.inf, maxval: float=np.inf):
+		"""
+		Returns a dataframe of key inferential results.
+
+		Parameters
+		----------
+		minval : float
+			Analytical lower bound on estimand used to clip results. 
+			Defaults to -np.inf.
+		maxval : float
+			Analytical upper bound on estimand used to clip results.
+			Defaults to np.inf.
+
+		Returns
+		-------
+		results : pd.DataFrame
+			DataFrame of key inferential results.
+		"""
+		self.results_ = pd.DataFrame(
+			np.stack(
+				[
+					np.clip(self.estimates, minval, maxval), 
+					self.ses,
+					np.clip(self.cis, minval, maxval),
+				], 
+				axis=0
+			),
+			index=['Estimate', 'SE', 'Conf. Int.'],
+			columns=['Lower', 'Upper']
+		)
+		return self.results_
+
+	def summary(self, minval: float=-np.inf, maxval: float=np.inf):
+		"""
+		Prints a summary of main results from the class.
+
+		Parameters
+		----------
+		minval : float
+			Analytical lower bound on estimand used to clip results. 
+			Defaults to -np.inf.
+		maxval : float
+			Analytical upper bound on estimand used to clip results.
+			Defaults to np.inf.
+
+		Returns
+		-------
+		None
+
+		Notes
+		-----
+		To access the inferential results as a pd.DataFrame, call
+		``DualBounds.results()``.
+		"""
+		print("___________________Inference_____________________")
+		print(self.results(minval=minval, maxval=maxval))
+		print()
+		print("_________________Outcome model___________________")
+		self._compute_oos_resids()
+		sumstats = dist_reg._evaluate_model_predictions(
+			y=self.y, haty=self.oos_preds
+		)
+		print(sumstats)
+		print()
+		print("_________________Treatment model_________________")
+		sumstats = dist_reg._evaluate_model_predictions(
+			y=self.W, haty=self.pis
+		)
+		print(sumstats)
+		print()
+		# print("-----------Nonrobust plug-in bounds-----------")
+		# print(self._plug_in_results())
+		# print()
+
 
 def plug_in_no_covariates(
-	y, W, f, pis=None, B=0, verbose=True, alpha=0.1, max_nvals=1000):
+	outcome: np.array, 
+	treatment: np.array, 
+	f: callable, 
+	propensities: Optional[np.array]=None,
+	B: int=0,
+	verbose: bool=True,
+	alpha: float=0.05,
+	max_nvals: int=1000,
+) -> dict:
 	"""
-	Computes plug-in bounds on E[f(Y(0),Y(1))] without using covariates.
+	Computes plug-in bounds on :math:`E[f(Y(0),Y(1))]` without using covariates.
 
 	Parameters
 	----------
-	y : np.array
-		n-length array of outcomes
-	W : np.array
-		n-length array of treatments.
+	outcome : np.array
+		n-length array of outcomes (y)
+	treatment : np.array
+		n-length array of treatments (W).
 	f : function
 		f(y0, y1, x) defines the objective.
-	pis : np.array
-		n-length array of propensity scores.
-		Default: all equal to 1/2.
+	propensities : np.array
+		n-length array of propensity scores (pis).
+		Default: all equal to treatment.mean().
 	B : int
 		Number of bootstrap replications to compute standard errors.
 		Defaults to 0 (no standard errors).
 	verbose : bool
 		Show progress bar while bootstrapping if verbose=True.
 	alpha : float
 		nominal Type I error level.
 	max_nvals : int
-		Maximum dimension of OT problem.
+		Maximum dimension of optimal transport problem.
+
+	Returns
+	-------
+	results : dict
+		Dictionary containing up to three keys:
+
+		- estimates: 2-length array of lower/upper estimates.
+		- ses: 2-length array of lower/upper standard errors.
+		- cis: 2-length array of lower/upper confidence intervals.
 	"""
+	# rename for simplicity
+	y = outcome
+	W = treatment
+	pis = propensities
+
+	# Perform analysis
 	n = len(y)
 	if pis is None:
-		pis = np.ones(n) / 2
+		pis = np.ones(n) * treatment.mean()
 	if B == 0:
 		# Dists
 		y0_vals = y[W == 0]
 		y0_probs = 1 / (1-pis[W==0]); y0_probs /= y0_probs.sum()
 		y1_vals = y[W == 1]
 		y1_probs = 1 / (pis[W==1]); y1_probs /= y1_probs.sum()
 		# Reduce dimension to prevent memory errors for huge datasets
@@ -957,24 +1148,24 @@
 			M=fvals,
 		)
 		upper = -ot.lp.emd2(
 			a=y0_probs,
 			b=y1_probs,
 			M=-fvals,
 		)
-		return np.array([lower, upper])
+		return dict(estimates=np.array([lower, upper]))
 	else:
 		# Estimates
-		ests = plug_in_no_covariates(y=y, W=W, f=f, B=0)
+		ests = plug_in_no_covariates(outcome=y, treatment=W, f=f, B=0)
 		# Bootstrap
 		bs_ests = np.zeros((B, 2))
 		for b in utilities.vrange(B, verbose=verbose):
 			inds = np.random.choice(np.arange(n), size=n, replace=True)
 			bs_ests[b] = plug_in_no_covariates(
-				y=y[inds], W=W[inds], f=f, B=0
+				outcome=y[inds], treatment=W[inds], f=f, B=0
 			)
 		# Bias
 		bias = bs_ests.mean(axis=0) - ests
 		ses = bs_ests.std(axis=0)
 		cis = ests - bias
 		cis[0] -= stats.norm.ppf(1-alpha/2) * ses[0]
 		cis[1] += stats.norm.ppf(1-alpha/2) * ses[1]
```

### Comparing `dualbounds-0.2.1/dualbounds/interpolation.py` & `dualbounds-1.0.0/dualbounds/interpolation.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 go from discrete dual variables to continuous ones.
 """
 
 import numpy as np
 import scipy as sp
 from . import utilities
 
-def adaptive_interpolate(x, y, newx):
+def adaptive_interpolate(x: np.array, y: np.array, newx: np.array):
 	"""
 	Adaptively chooses between linear and nearest-neighbor
 	interpolation.
 
 	Parameters
 	----------
 	x : np.array
@@ -29,17 +29,17 @@
 	"""
 	if len(np.unique(y)) <= 2 and len(y) > 2:
 		return nn_interpolate(x, y, newx)
 	else:
 		return linear_interpolate(x, y, newx)
 
 
-def nn_interpolate(x, y, newx):
+def nn_interpolate(x: np.array, y: np.array, newx: np.array):
 	"""
-	nearest-neighbor interpolation.
+	Nearest-neighbor interpolation.
 
 	Parameters
 	----------
 	x : np.array
 		n-length array of inputs. Must be sorted, although
 		this is not explicitly enforced to save time.
 	y : np.array
@@ -61,16 +61,18 @@
 	inds = np.stack([linds, rinds], axis=1)
 	dists = np.abs(x[inds] - newx.reshape(-1, 1))
 	nbrs = inds[(np.arange(len(newx)), np.argmin(dists, axis=1))]
 	# Return
 	return y[nbrs]
 
 
-def linear_interpolate(x, y, newx):
+def linear_interpolate(x: np.array, y: np.array, newx: np.array):
 	"""
+	Linear interpolation.
+
 	Parameters
 	----------
 	x : np.array
 		n-length array of inputs. Must be sorted, although
 		this is not explicitly enforced to save time.
 	y : np.array
 		n-length array of outputs
```

### Comparing `dualbounds-0.2.1/dualbounds/lee.py` & `dualbounds-1.0.0/dualbounds/lee.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import warnings
 import numpy as np
+import pandas as pd
 import cvxpy as cp
 from scipy import stats
 from . import utilities
 from . import dist_reg
 from .utilities import BatchedCategorical
 from . import interpolation, generic
+from typing import Optional, Union
 
-"""
-Helper functions
-"""
-def compute_cvar(dists, n, alpha, lower=True, m=1000):
+
+### Helper functions ###
+
+def compute_cvar(dists, n: int, alpha: float, lower: bool=True, m: int=1000):
 	"""
 	Computes cvar using quantile approximation with m values.
 
 	Parameters
 	----------
 	dists : stats.dist
 		scipy distribution function of shape n
 	n : int
 		Batch dimension
 	alpha : array or float	
 		float or n-length array
 	lower : bool
+		If true, computes the lower CVAR. 
+		Else computes the upper CVAR.
 	m : int
 		Number of interpolation points
 	
 	Returns
 	-------
 	cvars : array
 		n-length array.
@@ -57,20 +61,24 @@
 	y0_probs=None,
 	y1_probs=None,
 	y0_vals=None,
 	y1_vals=None,
 	m=1000,
 ):
 	"""
-	Computes semi-analytical partial ident. bounds on 
+	Helper function to compute semi-analytical Lee Bounds.
 
-	E[Y(1) - Y(0) | S(0) = S(1) = 1]
-	
-	Ulike dual bounds, this function is not at all
-	robust to model misspecification,
+
+	Unlike dual bounds, this function is not at all
+	robust to model misspecification. The estimand is 
+
+	:math:`E[Y(1) - Y(0) | S(0) = S(1) = 1]`
+
+	where :math:`Y(1), Y(0)` are potential outcomes and 
+	:math:`S(1), S(0)` are post-treatment selection events.
 
 	Parameters
 	----------
 	s0_probs : np.array
 		n-length array where s0_probs[i] = P(S(0) = 1 | Xi)
 	s1_probs : np.array
 		n-length array where s1_probs[i] = P(S(1) = 1 | Xi)
@@ -97,15 +105,16 @@
 	Returns
 	-------
 	agg_bounds : np.array
 		(2,)-length array of lower and upper bound. This integrates 
 		across all n y0_dists/y1_dists, etc.
 	cond_bounds : np.array
 		(2, n)-length array where bounds[0,i] is the ith lower bound
-		and bounds[1,i] is the ith upper bound.
+		and bounds[1,i] is the ith upper bound conditional on 
+		:math:`X_i`.
 	"""
 	# Parse arguments
 	n = s0_probs.shape[0]
 	if y0_dists is None:
 		y0_dists = BatchedCategorical(
 			vals=y0_vals, probs=y0_probs
 		)
@@ -120,42 +129,115 @@
 		raise ValueError(f"Monotonicity is violated for indices of alphas={alphas[alphas > 1]}")
 
 	# compute E[Y(1) | Y(1) >= Q(alpha), S(1)=1]
 	# (or <= depending on the value of lower)
 	cvars_lower = compute_cvar(y1_dists, n, alpha=alphas, lower=True, m=m)
 	cvars_upper = compute_cvar(y1_dists, n, alpha=1-alphas, lower=False, m=m)
 	y0ms = y0_dists.mean()
-	cond_bounds = np.stack([cvars_lower - y0ms, cvars_upper - y0ms], axis=0)
-	agg_bounds = np.mean(cond_bounds * s0_probs, axis=1) / np.mean(s0_probs)
+	cond_bounds = np.stack([cvars_lower - y0ms, cvars_upper - y0ms], axis=0) # per-X bounds
+	agg_bounds = np.mean(cond_bounds * s0_probs, axis=1) / np.mean(s0_probs) # aggregated bounds
 	return agg_bounds, cond_bounds
 
 def lee_bound_no_covariates(
-	W, S, Y,
+	outcome: np.array, 
+	treatment: np.array, 
+	selections: np.array, 
+	propensities: Optional[np.array]=None,
+	B: int=200,
+	alpha: float=0.05,
 ):
+	"""
+	Computes plug-in Lee bounds without using covariates.
+
+	Parameters
+	----------
+	outcome : np.array
+		n-length array of outcomes (y)
+	treatment : np.array
+		n-length array of treatments (W).
+	selections : np.array
+		n-length array of selection indicators (S).
+	propensities : np.array
+		n-length array of propensity scores (pis).
+		Default: all equal to treatment.mean().
+	B : int
+		Number of bootstrap replications to compute standard errors.
+		Defaults to 0 (no standard errors).
+	verbose : bool
+		Show progress bar while bootstrapping if verbose=True.
+	alpha : float
+		nominal Type I error level.
+
+	Returns
+	-------
+	results : dict
+		Dictionary containing up to three keys:
+
+		- estimates: 2-length array of lower/upper estimates.
+		- ses: 2-length array of lower/upper standard errors.
+		- cis: 2-length array of lower/upper confidence intervals.
+	"""
+	# Rename for simplicity
+	y = outcome
+	W = treatment
+	S = selections
+	pis = propensities
+	if pis is None:
+		pis = np.ones(n) * treatment.mean()
 	n = len(W)
+
 	# compute P(S | W)
 	s0_prob = np.array([np.mean(S[W == 0])])
 	s1_prob = np.array([np.mean(S[W == 1])])
 	s1_prob = np.maximum(s0_prob, s1_prob)
-	# compute P(Y(0)) and P(Y(1))
-	y0_vals = np.sort(Y[(W == 0) & (S == 1)])
-	y0_probs = np.ones(len(y0_vals)) / len(y0_vals)
-	y1_vals = np.sort(Y[(W == 1) & (S == 1)])
-	y1_probs = np.ones(len(y1_vals)) / len(y1_vals)
+
+	# compute P(Y(0))
+	flags0 = (W == 0) & (S == 1)
+	y0_vals = y[flags0]
+	y0_probs = 1 / (1-pis[flags0]); y0_probs /= y0_probs.sum()
+	inds0 = np.argsort(y0_vals)
+	y0_vals = y0_vals[inds0]; y0_probs = y0_probs[inds0]
+
+	# compute P(Y(1))
+	flags1 = (W == 1) & (S == 1)
+	y1_vals = y[flags1]
+	y1_probs = 1 / (1-pis[flags1]); y1_probs /= y1_probs.sum()
+	inds1 = np.argsort(y1_vals)
+	y1_vals = y1_vals[inds1]; y1_probs = y1_probs[inds1]
+
+	# Construct argument list
 	args = dict(
 		s0_probs=s0_prob,
 		s1_probs=s1_prob,
 		y0_probs=y0_probs.reshape(1, -1),
 		y0_vals=y0_vals.reshape(1, -1),
 		y1_probs=y1_probs.reshape(1, -1),
 		y1_vals=y1_vals.reshape(1, -1)
 	)
 	# compute lower, upper bounds
-	abnds = compute_analytical_lee_bound(**args)[1][:, 0]
-	return abnds
+	ests = compute_analytical_lee_bound(**args)[1][:, 0]
+	if B > 0:
+		bs_ests = np.zeros((B, 2))
+		for b in range(B):
+			inds = np.random.choice(n, n, replace=True)
+			bs_ests[b] = lee_bound_no_covariates(
+				treatment=W[inds], selections=S[inds], outcome=y[inds], B=0
+			)['estimates']
+		bias = bs_ests.mean(axis=0) - ests
+		ses = bs_ests.std(axis=0)
+		cis = ests - bias
+		cis[0] -= stats.norm.ppf(1-alpha/2) * ses[0]
+		cis[1] += stats.norm.ppf(1-alpha/2) * ses[1]
+		return dict(
+			estimates=ests,
+			ses=ses,
+			cis=cis,
+		)
+	else:
+		return dict(estimates=ests)
 
 def lee_delta_method_se(
 	sbetas, skappas, sgammas
 ):			
 	# estimate
 	hat_beta = sbetas.mean()
 	hat_kappa = skappas.mean()
@@ -172,68 +254,87 @@
 	])
 	# estimate
 	se = np.sqrt(grad @ hatSigma @ grad / len(sbetas))
 	return hattheta, se
 
 class LeeDualBounds(generic.DualBounds):
 	"""
-	Computes dual bounds on
+	Computes dual bounds on the ATE under selection bias.
+
+	Precisely, this class bounds 
 
-	E[Y(1) - Y(0) | S(1) = S(0) = 1]
+	:math:`E[Y(1) - Y(0) | S(0) = S(1) = 1]`
 
-	for an outcome Y and a binary post-treatment
-	selection event S. These bounds assume monotonicity,
-	i.e., S(1) >= S(0) a.s. (see Lee 2009).
+	where :math:`Y(1), Y(0)` are potential outcomes and 
+	:math:`S(1), S(0)` are post-treatment selection events.
+	These bounds assume monotonicity, i.e., 
+	:math:`S(1) \ge S(0)` a.s. (see Lee 2009).
 
 	Parameters
 	----------
-	S : np.array
-		n-length array of binary selection indicators
-	X : np.array
-		(n, p)-shaped array of covariates.
-	W : np.array
-		n-length array of treatment indicators.
-	Y : np.array
-		n-length array of outcome measurements
-	pis : np.array
-		n-length array of propensity scores P(W=1 | X). 
-		If ``None``, will be estimated from the data itself.
-	Y_model : str or dist_reg.DistReg
-		One of ['ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'].
-		Alternatively, a distributional regression class inheriting 
-		from ``dist_reg.DistReg``. E.g., when ``y`` is continuous,
-		defaults to ``Y_model=dist_reg.CtsDistReg(model_type='ridge')``.	
-	S_model : str or dist_reg.DistReg
-		One of ['logistic', 'monotone_logistic', 'randomforest', 'knn'],
-		or a class inheriting from ``dist_reg.DistReg``. Defaults to
-		``monotone_logistic``. 
-	W_model : str or sklearn classifier
-		Specifies how to estimate the propensity scores if ``pis`` is
-		not known.  Either a str identifier as above or an sklearn
-		classifier---see the tutorial for examples.
-	discrete : bool
-		If True, treats y as a discrete variable. 
-		Defaults to None (inferred from the data).
+	selections : np.array
+		n-length array-like of binary selection indicators
+	outcome : np.array | pd.Series
+		n-length array of outcome measurements (Y).
+	treatment : np.array | pd.Series
+		n-length array of binary treatment (W).
+	covariates : np.array | pd.Series
+		(n, p)-shaped array of covariates (X).
+	propensities : np.array | pd.Series
+		n-length array-like of propensity scores :math:`P(W=1 | X)`. 
+		If ``None``, will be estimated from the data.
+	outcome_model : str | dist_reg.DistReg
+		The model for estimating the law of :math:`Y \mid X, W`.
+		Two options:
+
+		- A str identifier, e.g., 'ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'.
+		- An object inheriting from ``dist_reg.DistReg``. 
+
+		E.g., when ``outcome`` is continuous, the default is
+		``outcome_model=dist_reg.CtsDistReg(model_type='ridge')``.
+	propensity_model : str | sklearn classifier
+		How to estimate the propensity scores if they are not provided.
+		Two options:
+
+		- A str identifier, e.g., 'ridge', 'lasso', 'elasticnet', 'randomforest', 'knn'.
+		- An sklearn classifier, e.g., ``sklearn.linear_model.LogisticRegressionCV()``.
+	selection_model : str | dist_reg.BinaryDistReg
+		How to estimate the selection probabilities :math:`P(S =1 | W, X)`.
+		Two options:
+
+		- A str identifier, i.e., 'monotone_logistic', 'ridge', 'lasso'.
+		- An object inheriting from ``dist_reg.BinaryDistReg``.
+
+		The default is ``monotone_logistic``. 
 	support : np.array
-		Optinal support of y, if known.
+		Optional support of the outcome, if known and discrete.
 		Defaults to ``None`` (inferred from the data).
+	model_kwargs : dict
+		Additional kwargs for the ``outcome_model``, e.g.,
+		``feature_transform``. See 
+		:class:`dualbounds.dist_reg.CtsDistReg` or 
+		:class:`dualbounds.dist_reg.BinaryDistReg` for more kwargs.
 	"""	
 
 	def __init__(
 		self,
-		S,
+		selections: Union[np.array, pd.Series],
 		*args, 
-		S_model=None,
+		selection_model: Optional[Union[str, dist_reg.BinaryDistReg]]=None,
 		**kwargs
 	):
-		self.S = S
-		self.S_model = S_model
+		# Main initialization
 		kwargs['f'] = None
 		super().__init__(*args, **kwargs)
-
+		# Initialization for S
+		self.selection_model = selection_model
+		if isinstance(selections, pd.Series) or isinstance(selections, pd.DataFrame):
+			selections = selections.values.reshape(self.n)
+		self.S = utilities._binarize_variable(selections, var_name='selections')
+	
 	def _ensure_feasibility(
 		self,
 		i,
 		nu0,
 		nu1,
 		lower,
 		ymin,
@@ -302,37 +403,54 @@
 		verbose=False,
 		nvals=100,
 		ymin=None,
 		ymax=None,
 		**kwargs,
 	):
 		"""
+		Estimates dual variables using the outcome model.
+
+		We generally recommend that the user call .fit() instead of 
+		calling this function directly.
+
 		Parameters
 		----------
 		s0_probs : np.array
-			n-length array where s0_probs[i] = P(S(0) = 1 | Xi)
+			n-length array where s0_probs[i] = :math:`P(S_i(0) = 1 | X_i)`.
 		s1_probs : np.array
-			n-length array where s1_probs[i] = P(S(1) = 1 | Xi)
-		y1_dists : np.array
-			batched scipy distribution of shape (n,) where the ith
-			distribution is the conditional law of Yi(1) | S(1) = 1, Xi
-			OR 
-			list of scipy dists whose shapes add up to n.
+			n-length array where s1_probs[i] = :math:`P(S_i(1) = 1 | X_i)`.
+		y1_dists : list
+			The ith distribution of y1_dists represents the conditional
+			law of :math:`Y_i(1) | X_i, S_i(1) =1`. There are two input formats:
+
+			- batched scipy distribution of shape (n,)
+			- list of scipy dists whose shapes add up to n.
+
 		y1_vals : np.array
-			Optional (n, nvals1)-length array of values y1 can take.
-			Ignored if ``y1_dists`` is provided.
+			(n, nvals1)-length array where ``y1_vals[i]`` is the support 
+			of :math:`Y_i(1)`.	Ignored if ``y1_dists`` is provided.
 		y1_probs : np.array
-			Optional (n, nvals1)-length array where
-			y1_probs[i, j] = P(Y(1) = yvals1[j] | S(1) = 1, Xi).
-			Ignored if ``y1_dists`` is provided.
+			(n, nvals1)-length array where ``y1_probs[i, j]``
+			is the estimated probability that :math:`Y_i(1)`
+			equals ``y1_vals[i, j].``
+		verbose : bool
+			If True, prints progress reports.
+		nvals : int
+			Number of values to use when discretizing Y(1).
+		ymin : float
+			Minimum value of Y(1) to use numerically.
+		ymax : float
+			Maximum value of Y(1) to use numerically.
 		kwargs : dict
 			kwargs for _ensure_feasibility method.
 			Includes ymin, ymax, grid_size.
 		"""
 		# Constants for solver
+		if verbose:
+			print("Estimating optimal dual variables.")
 		n = s0_probs.shape[0]
 		self.nvals0 = 2 # because S is binary
 		if self.discrete:
 			self.nvals1 = len(self.support) + 1
 		else:
 			self.nvals1 = nvals
 		self.interp_fn = interpolation.linear_interpolate
@@ -393,15 +511,15 @@
 			fvals = (
 				s0_vals * self.y1_vals_adj[i].reshape(1, -1)
 			).astype(float)
 			# below is the max val. used instead of inf to relax 
 			# constraints. this provably has no effect compared
 			# to using np.inf, but allows the use of ot instead
 			# of cvxpy, leading to a substantial speedup.
-			max_fval = np.abs(fvals).max() * 1e5
+			max_fval = np.abs(fvals).max() * 1e7
 			# helpful concatenation
 			probs0 = np.array([1 - s0_probs[i], s0_probs[i]])
 			# solve 
 			for lower in [1, 0]:
 				# Relax constraints due to monotonicity
 				fvals[1][0] = max_fval if lower else -max_fval
 				nu0x, nu1x, objval = self._solve_single_instance(
@@ -449,123 +567,146 @@
 					)[0]
 				if self.discrete and S[i] == 1:
 					j = np.argmin(np.abs(self.y1_vals_adj[i][1:] - y[i]))
 					self.hatnu1s[1 - lower, i] = nu1x[j+1]
 
 	def cross_fit(
 		self,
-		nfolds=5,
-		suppress_warning=False,
-		verbose=True,
+		nfolds: int=5,
+		suppress_warning: bool=False,
+		verbose: bool=True,
 	):
 		"""
-		Performs cross-fitting to estimate the outcome and selection models.
+		Cross-fits the outcome and selection models.
+
+		Parameters
+		----------
+		nfolds : int
+			Number of folds to use in cross-fitting.
+		suppress_warning : bool
+			If True, suppresses the warning about manual crossfitting.
+		verbose : bool
+			If True, prints progress reports.
 
 		Returns
 		-------
 		s0_probs : np.array
-			n-length array where s0_probs[i] = P(S(0) = 1 | Xi)
+			n-length array where s0_probs[i] = :math:`P(S_i(0) = 1 | X_i)`.
 		s1_probs : np.array
-			n-length array where s1_probs[i] = P(S(1) = 1 | Xi)
+			n-length array where s1_probs[i] = :math:`P(S_i(1) = 1 | X_i)`.
 		y0_dists : np.array
 			list of batched scipy distributions whose shapes sum to n.
-			the ith dist. is the conditional law of Yi(0) | S(0) = 1, Xi
-		y1_dists : np.array
+			the ith dist. is the conditional law of :math:`Y_i(0) | S_i(0) = 1, X_i`.
+		y1_dists : list
 			list of batched scipy distributions whose shapes sum to n.
-			the ith dist. is the conditional law of Yi(1) | S(1) = 1, Xi
-		suppress_warning : bool
-			If True, suppresses the warning about manual crossfitting.
+			the ith dist. is the conditional law of :math:`Y_i(1) | S_i(1) = 1, X_i`.
 		"""
 		# estimate selection probs
 		if self.s0_probs is None or self.s1_probs is None:
-			if self.S_model is None:
-				self.S_model = 'monotone_logistic'
-			self.S_model = generic.get_default_model(
-				Y_model=self.S_model, support=set([0,1]), 
-				discrete=True, monotonicity=True, 
+			if self.selection_model is None:
+				self.selection_model = 'monotone_logistic'
+			self.selection_model = generic.get_default_model(
+				outcome_model=self.selection_model, 
+				# the following args are ignored if selection_model already
+				# inherits from dist_reg.DistReg class
+				support=set([0,1]), 
+				discrete=True,
+				monotonicity=True, 
+				how_transform='intercept',
 			)
 			if verbose:
 				print("Cross-fitting the selection model.")
 			sout = dist_reg.cross_fit_predictions(
 				W=self.W, X=self.X, y=self.S, 
 				nfolds=nfolds, 
-				model=self.S_model,
+				model=self.selection_model,
 				verbose=verbose,
 				probs_only=True,
 			)
-			self.s0_probs, self.s1_probs, self.S_model_fits, self.S_oos_preds = sout
+			self.s0_probs, self.s1_probs, self.selection_model_fits, self.S_oos_preds = sout
 		elif not suppress_warning:
 			warnings.warn(
 				generic.CROSSFIT_WARNING.replace("y0_", "s0_").replace("y1_", "s1_")
 			)
 
 		# Estimate outcome model
 		if self.y0_dists is None or self.y1_dists is None:
-			self.Y_model = generic.get_default_model(
-				discrete=self.discrete, support=self.support, Y_model=self.Y_model,
+			self.outcome_model = generic.get_default_model(
+				discrete=self.discrete, support=self.support, outcome_model=self.outcome_model,
 			)
 			if verbose:
 				print("Cross-fitting the outcome model.")
 			yout = dist_reg.cross_fit_predictions(
 				W=self.W, X=self.X, S=self.S, y=self.y, 
 				nfolds=nfolds, 
-				model=self.Y_model,
+				model=self.outcome_model,
 				verbose=verbose,
 			)
-			self.y0_dists, self.y1_dists, self.model_fits, self.oos_preds = yout
+			self.y0_dists, self.y1_dists, self.model_fits, self.oos_dist_preds = yout
 		elif not suppress_warning:
 			warnings.warn(generic.CROSSFIT_WARNING)
 
 		# return
 		return self.s0_probs, self.s1_probs, self.y0_dists, self.y1_dists
 
 
-	def compute_dual_bounds(
+	def fit(
 		self,
 		nfolds=5,
 		alpha=0.05,
 		aipw=True,
 		s0_probs=None,
 		s1_probs=None,
 		y0_dists=None,
 		y1_dists=None,
 		suppress_warning=False,
 		verbose=True,
 		**solve_kwargs,
 	):
 		"""
+		Main function which (1) performs cross-fitting, (2) computes 
+		optimal dual variables, and (3) computes final dual bounds.
+
 		Parameters
 		----------
 		nfolds : int
 			Number of folds to use when cross-fitting. Defaults to 5,
 		alpha : float
 			Nominal coverage level. Defaults to 0.05.
 		aipw : bool
 			If true, returns AIPW estimator.
 		s0_probs : np.array
-			Optional n-length array where s0_probs[i] = P(S(0) = 1 | Xi).
+			Optional n-length array where s0_probs[i] = 
+			:math:`P(S_i(0) = 1 | X_i)`.
 			If not provided, will be estimated from the data.
 		s1_probs : np.array
-			Optional n-length array where s1_probs[i] = P(S(1) = 1 | Xi).
+			Optional n-length array where s1_probs[i] = 
+			:math:`P(S_i(1) = 1 | X_i)`.
 			If not provided, will be estimated from the data.
-		y0_dists : list
-			Optional list of n scipy distributions, where the ith
-			distribution is the conditional law of Yi(0) | S(0) = 1, Xi.
+		y0_dists : np.array
+			Optional list of batched scipy distributions whose shapes sum to n.
+			the ith dist. is the conditional law of 
+			:math:`Y_i(0) | S_i(0) = 1, X_i`.
 			If not provided, will be estimated from the data.
 		y1_dists : np.array
-			Optional list of n scipy distributions, where  the ith
-			distribution is the conditional law of Yi(1) | S(1) = 1, Xi.
+			Optional list of batched scipy distributions whose shapes sum to n.
+			The ith dist. is the conditional law of 
+			:math:`Y_i(1) | S_i(1) = 1, X_i`.
 			If not provided, will be estimated from the data.
 		suppress_warning : bool
 			If True, suppresses warning about cross-fitting.
 		verbose : bool
 			If True, gives occasional progress reports..
 		solve_kwargs : dict
 			kwargs to self.compute_dual_variables(), 
 			e.g., ``verbose``, ``nvals``, ``grid_size``
+
+		Returns
+		-------
+		self : object
 		"""
 		# Save data
 		self.s0_probs, self.s1_probs = s0_probs, s1_probs
 		self.y0_dists, self.y1_dists = y0_dists, y1_dists
 
 		# if pis not supplied: will use cross-fitting
 		if self.pis is None:
@@ -584,26 +725,28 @@
 			ymin=self.y.min(),
 			ymax=self.y.max(),
 			verbose=verbose,
 			**solve_kwargs,
 		)
 
 		# compute dual bounds
-		return self.compute_final_bounds(aipw=aipw, alpha=alpha)
+		self._compute_final_bounds(aipw=aipw, alpha=alpha)
+		return self
 
-
-	def compute_final_bounds(self, aipw=True, alpha=0.05):
+	def _compute_final_bounds(self, aipw=True, alpha=0.05):
 		"""
 		Computes final bounds based in (A)IPW summands,
 		using the delta method for E[Y(1) - Y(0) | S(1) = S(0) = 1].
 		"""
 		self._compute_ipw_summands()
 		summands = self.aipw_summands if aipw else self.ipw_summands
 		self._compute_cond_means()
 		self.y0s0_cond_means = self.mu0 * self.s0_probs
+		self.s_probs = self.s0_probs.copy()
+		self.s_probs[self.W == 1] = self.s1_probs[self.W == 1]
 		ests = []
 		ses = []
 		bounds = []
 		scale = stats.norm.ppf(1-alpha/2)
 		# kappa = E[Y(0) S(0)]
 		skappas = (1 - self.W) * (self.y * self.S - self.y0s0_cond_means) 
 		skappas = skappas / (1-self.pis)
@@ -629,8 +772,44 @@
 		self.estimates = np.array(ests)
 		self.ses = np.array(ses)
 		self.cis = np.array(bounds)
 		return dict(
 			estimates=self.estimates,
 			ses=self.ses,
 			cis=self.cis
-		)
+		)
+
+	def summary(self, minval=-np.inf, maxval=np.inf):
+		"""
+		Prints a summary of main results from the class.
+
+		Parameters
+		----------
+		minval : float
+			Analytical lower bound on estimand used to clip results. 
+			Defaults to -np.inf.
+		maxval : float
+			Analytical upper bound on estimand used to clip results.
+			Defaults to np.inf.
+		"""
+		print("___________________Inference_____________________")
+		print(self.results(minval=minval, maxval=maxval))
+		print()
+		print("________________Selection model__________________")
+		sumstats = dist_reg._evaluate_model_predictions(
+			y=self.S, haty=self.s_probs
+		)
+		print(sumstats)
+		print()
+		print("_________________Outcome model___________________")
+		self._compute_oos_resids()
+		sumstats = dist_reg._evaluate_model_predictions(
+			y=self.y[self.S == 1], haty=self.oos_preds[self.S == 1],
+		)
+		print(sumstats)
+		print()
+		print("________________Treatment model__________________")
+		sumstats = dist_reg._evaluate_model_predictions(
+			y=self.W, haty=self.pis
+		)
+		print(sumstats)
+		print()
```

### Comparing `dualbounds-0.2.1/dualbounds/utilities.py` & `dualbounds-1.0.0/dualbounds/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import sys
 import time
 import numpy as np
+import pandas as pd
 from scipy import stats
 from multiprocessing import Pool
 from functools import partial
 from itertools import product
 from tqdm.auto import tqdm
+from typing import Optional, Union
 
 def elapsed(t0):
 	return np.around(time.time() - t0, 2)
 
 def vrange(n, verbose=False):
 	if not verbose:
 		return range(n)
@@ -20,14 +22,71 @@
 def haslength(x):
 	try:
 		len(x)
 		return True
 	except:
 		return False
 
+def floatable(x):
+	try:
+		float(x)
+		return True
+	except:
+		return False
+
+### For processing data
+def _binarize_variable(x: np.array, var_name: str):
+	"""
+	Converts x to a binary r.v. and raises an error
+	if it contains more than 2 values.
+	"""
+	# Check if nans
+	if np.any(np.isnan(x)):
+		raise ValueError(f"{var_name} has missing values.")
+
+	# Check if binary
+	vals = set(list(np.unique(x)))
+	if len(vals) > 2:
+		raise ValueError(f"{var_name} is not binary and takes {len(vals)} values.")
+	elif len(vals - set([0,1])) == 0:
+		return x.astype(int)
+	else:
+		print(f"For {var_name}, replacing {vals[0]} with 0 and {vals[1]} with 1.")
+		return (x == list(vals)[1]).astype(int)
+
+def process_covariates(data: pd.DataFrame):
+	"""
+	Performs rudimentary pre-processing of covariates.
+
+	Parameters
+	----------
+	data : pd.DataFrame
+		Dataframe of covariates.
+
+	Returns
+	-------
+	processed : pd.DataFrame
+		DataFrame of preprocessed covariates.
+	"""
+	cts_covs = []
+	discrete_covs = []
+	for c in data.columns:
+		if np.all(data[c].apply(floatable)):
+			cts_covs.append(c)
+		else:
+			discrete_covs.append(c)
+
+	# Get dummies and return
+	return pd.get_dummies(
+		data[discrete_covs + cts_covs],
+		columns=discrete_covs,
+		dummy_na=True,
+		drop_first=True,
+	).astype(float)
+
 ### Multiprocessing helper
 def _one_arg_function(list_of_inputs, args, func, kwargs):
 	"""
 	Globally-defined helper function for pickling in multiprocessing.
 	:param list of inputs: List of inputs to a function
 	:param args: Names/args for those inputs
 	:param func: A function
@@ -56,24 +115,25 @@
 		A dictionary of arguments to func which do not change in each
 		of the processes spawned, defaults to {}.
 	num_processes : int
 		The maximum number of processes spawned, defaults to 1.
 	kwargs : dict
 		Each key should correspond to an argument to func and should
 		map to a list of different arguments.
+
 	Returns
 	-------
 	outputs : list
 		List of outputs for each input, in the order of the inputs.
+	
 	Examples
 	--------
 	If we are varying inputs 'a' and 'b', we might have
-	``apply_pool(
-		func=my_func, a=[1,2], b=[5]
-	)``
+		>> apply_pool_factorial(func=my_func, a=[1,2], b=[5])
+
 	which would return ``[my_func(a=1, b=5), my_func(a=2,b=5)]``.
 	"""
 	# Construct input sequence 
 	args = sorted(kwargs.keys())
 	kwarg_prod = list(product(*[kwargs[x] for x in args]))
 	# Prepare to send this to apply pool
 	final_kwargs = {}
@@ -107,18 +167,17 @@
 	Returns
 	-------
 	outputs : list
 		List of outputs for each input, in the order of the inputs.
 	Examples
 	--------
 	If we are varying inputs 'a' and 'b', we might have
-	``apply_pool(
-		func=my_func, a=[1,3,5], b=[2,4,6]
-	)``
-	which would return ``[my_func(a=1, b=2), my_func(a=3,b=4), my_func(a=5,b=6)]``.
+		>> apply_pool(func=my_func, a=[1,3,5], b=[2,4,6])
+
+	which returns ``[my_func(a=1, b=2), my_func(a=3,b=4), my_func(a=5,b=6)]``.
 	"""
 
 	# Construct input sequence
 	args = sorted(kwargs.keys())
 	num_inputs = len(kwargs[args[0]])
 	for arg in args:
 		if len(kwargs[arg]) != num_inputs:
@@ -143,14 +202,16 @@
 		with Pool(num_processes) as thepool:
 			all_outputs = thepool.map(partial_func, inputs)
 
 	return all_outputs
 
 def compute_est_bounds(summands, alpha=0.05):
 	"""
+	Helper function to compute confidence intervals.
+
 	Parameters
 	----------
 	summands : np.array
 		(2, n)-shaped array
 
 	Returns
 	-------
@@ -193,40 +254,60 @@
 		self.loc = loc
 		self.scale = scale
 
 	def rvs(self, size):
 		return self.loc + self.scale * np.ones(size)
 
 class BatchedCategorical:
-	
+	"""
+	Batched discrete (categorical) distribution.
+
+	This class supports the small set of operations
+	needed by the ``DualBounds`` class.
+
+	Parameters
+	----------
+	vals : np.array
+		(n, nvals)-shaped array of supports.
+	probs : np.array
+		(n, nvals)-shaped array of probabilities.
+	"""
 	def __init__(
 		self, vals, probs
 	):
-		"""
-		Parameters
-		----------
-		vals : (n, nvals)-shaped array
-		probs : (n, nvals)-shaped array. probs.sum(axis=1) == 1.
-		"""
 		# sort
 		self.n, self.nvals = vals.shape
 		self.vals, self.probs = _sort_disc_dist(vals=vals, probs=probs)
 		self.cumprobs = np.cumsum(self.probs, axis=1)
 		# validate args
 		if np.any(self.probs < 0):
 			raise ValueError("probs must be nonnegative")
 		if np.any(np.abs(self.probs.sum(axis=1)-1) > 1e-5):
 			raise ValueError("probs.sum(axis=1) must equal 1")
 	
 	def mean(self):
+		"""
+		Returns
+		-------
+		mu : np.array
+			n-length mean of discrete distributions.
+		"""
 		return np.sum(self.vals * self.probs, axis=1)
 	
 	def ppf(self, q):
 		"""
-		q : (m,n)-shaped array.
+		Parameters
+		----------
+		q : np.array
+			(m,n)-shaped array of desired quantiles, between 0 and 1.
+
+		Returns
+		-------
+		quantile_values : np.array
+			The desired quantile values of the categorical distributions.
 		"""
 		m = q.shape[0]
 		if len(q.shape) == 1:
 			q = np.stack([q for _ in range(self.n)], axis=1)
 		# use a for loop to save memory
 		qvals = np.zeros((m, self.n))
 		for i in range(self.n):
@@ -242,15 +323,14 @@
 			n-length array of a single RV drawn from each categorical.
 		"""
 		u = np.random.uniform(size=(self.n, 1))
 		inds = (u < self.cumprobs).argmax(axis=1)
 		return self.vals[(np.arange(self.n), inds)]
 
 
-
 def _convert_to_cat(bern_dist, n):
 	"""
 	Convert bernoulli dist. object to BatchedCategorical
 	"""
 	vals = np.zeros((n, 2)); vals[:, 1] += 1
 	probs = bern_dist.mean()
 	return BatchedCategorical(
@@ -314,60 +394,73 @@
 			probs = probs[~np.isnan(probs)]
 		return vals, probs
 	
 def adjust_support_size(
 	vals, probs, new_nvals, ymin, ymax
 ):
 	"""
-	Adjust categorical distribution to have a support of size new_nvals.
+	Adjust categorical distribution to have support of size ``new_nvals``.
 	
 	Parameters
 	----------
 	vals : np.array
 		(n, nvals)-length array of support. vals[i] must be sorted for each i.
 	probs : np.array
-		(n, nvals)-length array of probabilities
+		(n, nvals)-length array of probabilities of original distributions.
 	new_nvals : int
 		Desired size of support.
 	ymin : float
-		Minimum value for support
+		Minimum value for support.
 	ymax : float
-		Maximum value for support
+		Maximum value for support.
+
+	Returns
+	-------
+	new_vals : np.array
+		(n, new_nvals)-array of supports.
+	new_probs : np.array
+		(n, new_nvals)-array of probabilities.
 	"""
 	n, nvals = vals.shape
 	new_vals = np.zeros((n, new_nvals))
 	new_probs = np.zeros((n, new_nvals))
 	for i in range(n):
 		new_vals[i], new_probs[i] = _adjust_support_size_unbatched(
 			vals[i], probs[i], new_nvals, ymin=ymin, ymax=ymax,
 		)
 	return new_vals, new_probs
-def weighted_quantile(values, weights, quantiles, old_style=True):
+
+def weighted_quantile(values, weights, quantiles, _old_style=True):
 	"""
 	Very close to numpy.percentile, but supports weights.
 
 	Parameters
 	----------
 	values : np.array
 		n-length array of data
 	weights : np.array
 		n-length array of sample weights
 	quantiles : array-like
-		desired quantiles
+		d-length array of desired quantiles
+
+	Returns
+	-------
+	results : np.array
+		d-length array of weighted quantiles.
 	"""
 	if np.any(quantiles < 0) or np.any(quantiles > 1):
 		raise ValueError("Quantiles must be in [0,1]")
 
 	# Sort values
 	sorter = np.argsort(values)
 	values = values[sorter]
 	weights = weights[sorter]
 	# Compute quantiles
 	cdf = np.cumsum(weights) - 0.5 * weights
-	if old_style:
+	if _old_style:
 		cdf -= cdf[0]
 		cdf /= cdf[-1]
 	else:
 		cdf /= np.sum(weights)
 	# Interp + return
 	return np.interp(quantiles, cdf, values)
```

### Comparing `dualbounds-0.2.1/dualbounds/varcate.py` & `dualbounds-1.0.0/dualbounds/varcate.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,22 +68,19 @@
 	])
 	# estimate
 	se = np.sqrt(grad @ hatSigma @ grad / len(shx))
 	return hattheta, se
 
 class VarCATEDualBounds(generic.DualBounds):
 	"""
-	Class for computing lower bounds on 
-	
-	Var(E[Y(1) - Y(0) | X]).
-
-	This class has the same signature as 
-	``generic.DualBounds`` except it only
-	provides lower bounds and the input
-	``f`` will be ignored.
+	Computes lower bounds on :math:`Var(E[Y(1) - Y(0) | X]).`
+
+	This class has the same signature as ``generic.DualBounds``
+	except it only provides lower bounds and the input ``f``
+	will be ignored.
 	"""
 
 	def __init__(self, *args, **kwargs):
 		# Initialize with no f function
 		kwargs['f'] = None
 		super().__init__(*args, **kwargs)
 
@@ -98,22 +95,22 @@
 
 	def _compute_realized_dual_variables(self):
 		raise NotImplementedError()
 
 	def compute_dual_variables(self, *args, **kwargs):
 		""" 
 		In this case, the optimal dual variables are simply 
-		the estimated CATE.
+		the estimated CATE, so this function does nothing.
 		"""
 		pass
 
 	def _compute_ipw_summands(self):
 		pass
 
-	def compute_final_bounds(self, aipw=True, alpha=0.05):
+	def _compute_final_bounds(self, aipw=True, alpha=0.05):
 		self._compute_cond_means()
 		self.cates = self.mu1 - self.mu0 
 		#### We have to use the 6-d delta method
 		# The notation uses h(X) = hat E[Y(1) - Y(0) | X]
 		# 1. AIPW terms for h(X) * Y(1)
 		self.shxy1 = self.W * self.cates * (self.y - self.mu1)
 		self.shxy1 = self.shxy1 / self.pis + self.cates * self.mu1
@@ -125,22 +122,20 @@
 		# 4. AIPW terms for Y(1)
 		self.sy1 = self.W * (self.y - self.mu1) / self.pis + self.mu1
 		# 5. AIPW terms for Y(0)
 		self.sy0 = (1 - self.W ) * (self.y - self.mu0)
 		self.sy0 = self.sy0 / (1 - self.pis) + self.mu0
 		# 6. AIPW terms for h(X)^2
 		self.shx2 = self.cates**2
-		self.estimate, self.se = varcate_delta_method_se(
+		estimate, se = varcate_delta_method_se(
 			shxy1=self.shxy1, 
 			shxy0=self.shxy0, 
 			shx=self.shx, 
 			sy1=self.sy1, 
 			sy0=self.sy0, 
 			shx2=self.shx2,
 		)
 		scale = stats.norm.ppf(1-alpha)
-		self.lower_ci = self.estimate - scale * self.se
-		return dict(
-			estimate=self.estimate,
-			se=self.se,
-			lower_ci=self.lower_ci
-		)
+		lower_ci = estimate - scale * se
+		self.estimates = np.array([estimate, np.nan])
+		self.ses = np.array([se, np.nan])
+		self.cis = np.array([lower_ci, np.nan])
```

### Comparing `dualbounds-0.2.1/dualbounds/varite.py` & `dualbounds-1.0.0/dualbounds/varite.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 def compute_analytical_varite_bound(
 	n,
 	y0_dists,
 	y1_dists,
 	reps=100,
 ):
 	"""
-	Computes semi-analytical bounds on
-
-	Var(Y(0) - Y(1)).
+	Semi-analytical bounds on :math:`Var(Y(0) - Y(1))`.
 
 	Unlike dual bounds, this function is not
-	robust to model misspecification, 
+	robust to model misspecification.
 	
 	Parameters
 	----------
 	n : int
 		Number of observations.
 	y0_dists : stats.rv_continuous / stats.rv_discrete
 		batched scipy distribution of shape (n,) where the ith
@@ -68,29 +66,27 @@
 	)
 	# estimate
 	se = np.sqrt(grad @ hatSigma @ grad / len(sbetas))
 	return hattheta, se
 
 class VarITEDualBounds(DualBounds):
 	"""
-	Computes dual bounds on 
-
-	Var(Y(1) - Y(0)).
+	Computes dual bounds on :math:`Var(Y(1) - Y(0)).`
 
 	The signature of this class is identical to 
 	the ``generic.DualBounds`` class.  However, 
 	the input ``f`` will be ignored.
 	"""
 
 	def __init__(self, *args, **kwargs):
 		# Initialize with correct f function
 		kwargs['f'] = lambda y0, y1, x: (y0-y1)**2
 		super().__init__(*args, **kwargs)
 
-	def compute_final_bounds(self, aipw=True, alpha=0.05):
+	def _compute_final_bounds(self, aipw=True, alpha=0.05):
 		"""
 		Computes final bounds based in (A)IPW summands,
 		using the delta method for Var(Y(1) - Y(0)).
 		"""
 		self._compute_ipw_summands()
 		summands = self.aipw_summands if aipw else self.ipw_summands
 		self._compute_cond_means()
```

### Comparing `dualbounds-0.2.1/dualbounds.egg-info/PKG-INFO` & `dualbounds-1.0.0/dualbounds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dualbounds
-Version: 0.2.1
+Version: 1.0.0
 Summary: Dual bounds for model-agnostic inference
 Home-page: https://github.com/amspector100/dualbounds/
 Author: Asher Spector
 Author-email: amspector100@gmail.com
 License: UNKNOWN
 Description: A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://amspector100.github.io/dualbounds/ for detailed documentation and tutorials.
```

### Comparing `dualbounds-0.2.1/dualbounds.egg-info/SOURCES.txt` & `dualbounds-1.0.0/dualbounds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dualbounds-0.2.1/setup.py` & `dualbounds-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,12 +34,13 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
         "numpy>=1.17.4",
         "scipy>=1.12.0",
         "scikit-learn>=1.4.1",
+        "pandas",
         "POT",
         "cvxpy",
         "tqdm",
     ],
 )
```

### Comparing `dualbounds-0.2.1/test/context.py` & `dualbounds-1.0.0/test/context.py`

 * *Files identical despite different names*

### Comparing `dualbounds-0.2.1/test/test_bootstrap.py` & `dualbounds-1.0.0/test/test_bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,21 @@
 
 	def test_multiplier_bootstrap_db_no_error(self):
 		# Fit two dualbounds objects
 		data = db.gen_data.gen_regression_data(n=200, p=5)
 		db_objects = []
 		for Y_model in ['ridge', 'knn']:
 			gdb = db.generic.DualBounds(
-				y=data['y'], X=data['X'], W=data['W'], pis=data['pis'],
-				Y_model=Y_model,
+				outcome=data['y'], 
+				covariates=data['X'], 
+				treatment=data['W'], 
+				propensities=data['pis'],
+				outcome_model=Y_model,
 				f=lambda y0, y1, x: (y1 < y0).astype(float) 
 			)
-			gdb.compute_dual_bounds(nfolds=2)
+			gdb.fit(nfolds=2)
 			db_objects.append(gdb)
 
 		# Run mult bootstrap
 		bootstrap.dualbound_multiplier_bootstrap(
 			db_objects, alpha=0.1, B=100
 		)
```

### Comparing `dualbounds-0.2.1/test/test_dist_reg.py` & `dualbounds-1.0.0/test/test_dist_reg.py`

 * *Files identical despite different names*

### Comparing `dualbounds-0.2.1/test/test_generic.py` & `dualbounds-1.0.0/test/test_generic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import numpy as np
+import pandas as pd
 import scipy as sp
 from scipy import stats
 import unittest
 import pytest
 import os
 import sys
 import sklearn.ensemble
@@ -48,18 +49,18 @@
 			upper = np.std(y1 - y0u)**2
 			mu2 = (y1_dists.mean() - y0_dists.mean())**2
 			# create dualbound.
 			# the input data is a dummy variable that does nothing
 			nvals = 2000
 			vdb = db.generic.DualBounds(
 				f=lambda y0, y1, x: (y0-y1)**2,
-				X=np.zeros(1),
-				W=np.zeros(1),
-				pis=np.ones(1) * 1/2,
-				y=np.zeros(1),
+				covariates=np.zeros(1),
+				treatment=np.zeros(1),
+				propensities=np.ones(1) * 1/2,
+				outcome=np.zeros(1),
 				discrete=discrete,
 				support=support,
 			)
 			vdb.compute_dual_variables(
 				y0_dists=y0_dists_input, 
 				y1_dists=y1_dists_input, 
 				y0_min=np.min(y0l),
@@ -99,18 +100,18 @@
 			lambda y0, y1, x: y0 <= y1,
 			lambda y0, y1, x: (y0 <= 0) * (y1 <= 0),
 		]
 		# Test the size of objdiffs is small on average
 		for f in fs:
 			gdb = db.generic.DualBounds(
 				f=f,
-				X=X,
-				W=W,
-				pis=pis,
-				y=Y,
+				covariates=X,
+				treatment=W,
+				propensities=pis,
+				outcome=Y,
 			)
 			gdb.compute_dual_variables(
 				y0_dists=y0_dists, 
 				y1_dists=y1_dists,
 				nvals0=nvals,
 				nvals1=nvals,
 			)
@@ -160,26 +161,28 @@
 			mt_exps,
 			sigma_model_types,
 			sigma_model_exps,
 			eps_dists
 		):
 			gdb = db.generic.DualBounds(
 				f=f, 
-				X=data['X'], W=data['W'], 
-				y=data['y'], pis=data['pis'], 
-				Y_model=model,
+				covariates=data['X'], 
+				treatment=data['W'], 
+				outcome=data['y'],
+				propensities=data['pis'], 
+				outcome_model=model,
 				heterosked_model=sigma_model,
 				eps_dist=eps_dist,
 			)
-			gdb.compute_dual_bounds(nfolds=3, alpha=0.05)
+			gdb.fit(nfolds=3, alpha=0.05).summary()
 			# Check the correct class for the main model
 			Ym = gdb.model_fits[0].model
 			self.assertTrue(
 				isinstance(Ym, mt_exp),
-				f"fit Y_model {Ym} with W_model={model} is not of type {mt_exp}"
+				f"fit outcome_model {Ym} with propensity_model={model} is not of type {mt_exp}"
 			)
 			# Check correct class for the heteroskedastic model
 			if sigma_model_exp is not None:
 				Ym2 = gdb.model_fits[0].sigma2_model
 				self.assertTrue(
 					isinstance(Ym2, sigma_model_exp),
 					f"sigma_model {Ym2} with heterosked_model={sigma_model} is not of type {sigma_model_exp}"
@@ -200,55 +203,99 @@
 			db.dist_reg.parse_model_type(mt, discrete=True) for mt in model_types
 		]
 		model_types.append(db.dist_reg.BinaryDistReg(model_type='ridge'))
 		expected_mts.append(lm.LogisticRegressionCV)
 		for model_type, mt_exp in zip(model_types, expected_mts):
 			gdb = db.generic.DualBounds(
 				f=f, 
-				X=data['X'], W=data['W'], 
-				y=data['y'], pis=data['pis'], 
-				Y_model=model_type,
+				covariates=data['X'], 
+				treatment=data['W'], 
+				outcome=data['y'],
+				propensities=data['pis'], 
+				outcome_model=model_type,
 			)
-			gdb.compute_dual_bounds(nfolds=3, alpha=0.05)
+			gdb.fit(nfolds=3, alpha=0.05).summary()
 			# Check the correct model type
 			Ym = gdb.model_fits[0].model
 			self.assertTrue(
 				isinstance(Ym, mt_exp),
-				f"fit model {mt_exp} with Y_model={model_type} is not of type {mt_exp}"
+				f"fit model {mt_exp} with outcome_model={model_type} is not of type {mt_exp}"
 			)
 
 
 	def test_fit_propensity_scores(self):
 		"""
-		Same as above but for W_model
+		Same as above but for propensity_model
 		"""
 		data = gen_data.gen_regression_data(n=300, p=3, eps_dist='gaussian', r2=0)
 		f = lambda y0, y1, x : y0 <= y1
-		W_models = ['ridge', 'lasso', 'knn', 'rf']
+		propensity_models = ['ridge', 'lasso', 'knn', 'rf']
 		expecteds = [
-			db.dist_reg.parse_model_type(wm, discrete=True) for wm in W_models
+			db.dist_reg.parse_model_type(wm, discrete=True) for wm in propensity_models
 		]
-		W_models.append(sklearn.ensemble.AdaBoostClassifier(algorithm='SAMME'))
+		propensity_models.append(sklearn.ensemble.AdaBoostClassifier(algorithm='SAMME'))
 		expecteds.append(sklearn.ensemble.AdaBoostClassifier)
-		for W_model, expected in zip(W_models, expecteds):
+		for propensity_model, expected in zip(propensity_models, expecteds):
 			gdb = db.generic.DualBounds(
 				f=f,
-				X=data['X'], W=data['W'], y=data['y'],
-				pis=None, # to be estimated 
-				Y_model='ridge',
-				W_model=W_model,
+				covariates=data['X'], treatment=data['W'], outcome=data['y'],
+				propensities=None, # to be estimated 
+				outcome_model='ridge',
+				propensity_model=propensity_model,
 			)
-			gdb.compute_dual_bounds(nfolds=3)
+			gdb.fit(nfolds=3).summary()
 			# Check the correct class
-			Wm = gdb.W_model_fits[0]
+			Wm = gdb.propensity_model_fits[0]
 			self.assertTrue(
 				isinstance(Wm, expected),
-				f"fit W_model {Wm} with W_model={W_model} is not of type {expected}"
+				f"fit propensity_model {Wm} with propensity_model={propensity_model} is not of type {expected}"
 			)
 
+	def test_from_pd(self):
+		# Sample data
+		for eps_dist in ['gaussian', 'bernoulli']:
+			data = gen_data.gen_regression_data(n=50, p=5, eps_dist='bernoulli', r2=0)
+
+			# Method 1
+			f = lambda y0, y1, x: y1 - y0
+			gdb1 = db.generic.DualBounds(
+				f=f,
+				outcome=pd.Series(data['y']),
+				treatment=pd.Series(data['W']),
+				covariates=pd.DataFrame(data['X']),
+				propensities=pd.Series(data['pis']),
+			).fit()
+
+			# Method 2
+			gdb2 = db.generic.DualBounds(
+				f=f,
+				covariates=data['X'],
+				outcome=data['y'],
+				treatment=data['W'],
+				propensities=data['pis'],
+			)
+
+			# Test equality
+			self.assertTrue(
+				gdb1.X.shape == gdb2.X.shape,
+				"using pandas changes the shape of the covariates"
+			)
+			for expected, out, name in zip(
+				[gdb2.y, gdb2.W, gdb2.pis],
+				[gdb1.y, gdb1.W, gdb1.pis],
+				['y', 'W', 'pis'],
+			):
+				np.testing.assert_array_almost_equal(
+					expected,
+					out,
+					decimal=8,
+					err_msg=f"Using pandas initialization changes {name} values."
+				)
+
+
 	def test_plug_in_no_covariates(self):
 		np.random.seed(123)
 		## DGP
 		n, reps = 300, 100
 		mu0 = np.zeros(n)
 		mu1 = np.random.randn(n)
 		y0_dists = stats.norm(loc=mu0)
@@ -265,28 +312,28 @@
 		oracles = np.zeros((reps, 2))
 		for r in range(reps):
 			# Observed Y(1), Y()
 			W = np.random.binomial(1, pis, size=n)
 			y = y1.copy(); y[W == 0] = y0[W==0]
 			# Naive estimator
 			naive[r] = db.generic.plug_in_no_covariates(
-				y=y, W=W, f=f, pis=None, max_nvals=n
-			)
+				outcome=y, treatment=W, f=f, propensities=None, max_nvals=n
+			)['estimates']
 			# Oracle estimator
 			oracles[r] = db.generic.plug_in_no_covariates(
-				y=np.concatenate([y1, y0]), 
-				W=np.concatenate([np.ones(n), np.zeros(n)]), 
+				outcome=np.concatenate([y1, y0]), 
+				treatment=np.concatenate([np.ones(n), np.zeros(n)]), 
 				f=f,
-				pis=None,
+				propensities=None,
 				max_nvals=2*n,
-			)
+			)['estimates']
 			# Real estimator
 			ests[r] = db.generic.plug_in_no_covariates(
-				y=y, W=W, f=f, pis=pis, max_nvals=n
-			)
+				outcome=y, treatment=W, f=f, propensities=pis, max_nvals=n
+			)['estimates']
 
 		# Take averages
 		naive_mu = naive.mean(axis=0)
 		est_mu = ests.mean(axis=0)
 		oracle_mu = oracles.mean(axis=0)
 
 		# Test inaccuracy of naive method
```

### Comparing `dualbounds-0.2.1/test/test_interp.py` & `dualbounds-1.0.0/test/test_interp.py`

 * *Files identical despite different names*

### Comparing `dualbounds-0.2.1/test/test_lee.py` & `dualbounds-1.0.0/test/test_lee.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import numpy as np
+import pandas as pd
 import scipy as sp
 from scipy import stats
 import unittest
 import pytest
 import os
 import sys
 import sklearn.linear_model as lm
@@ -216,15 +217,15 @@
 		args = dict(
 			s0_probs=s0_probs, s1_probs=s1_probs, y1_dists=y1_dists,
 		)
 		# analytical solution
 		_, expected = lee.compute_analytical_lee_bound(**args, y0_dists=y0_dists)
 		# analytical bounds based on linear programming
 		ldb = lee.LeeDualBounds(
-			y=y, X=None, W=None, S=np.random.binomial(1, 0.5, n),
+			outcome=y, treatment=np.ones(n), selections=np.random.binomial(1, 0.5, n),
 		)
 		ldb.compute_dual_variables(
 			**args, ymin=-10, ymax=10, nvals=nvals
 		)
 		lp_bounds = ldb.objvals - ldb.dxs - y0_dists.mean() * s0_probs
 		lp_bounds = lp_bounds / s0_probs
 		np.testing.assert_array_almost_equal(
@@ -280,15 +281,15 @@
 
 			# analytical solution
 			_, abounds = lee.compute_analytical_lee_bound(**args, y0_dists=y0_dists)
 			# convert to E[Y(1) S(0)]
 			expected = np.mean(abounds * s0_probs + s0_probs * y0_dists.mean(), axis=1)
 			# compute dual variables
 			ldb = lee.LeeDualBounds(
-				y=Y[0], S=S[0], W=W[0], X=None, pis=pis
+				outcome=Y[0], selections=S[0], treatment=W[0], X=None, propensities=pis
 			)
 			ldb.y0_dists = y0_dists
 			ldb.s0_probs = s0_probs
 			ldb.compute_dual_variables(**args, ymin=-5, ymax=5)
 			# compute IPW/AIPW summands
 			ipws = []
 			aipws = []
@@ -308,55 +309,95 @@
 				np.testing.assert_array_almost_equal(
 					ests,
 					expected,
 					decimal=2,
 					err_msg=f"{method} bounds do not agree with analytical bounds",
 				)
 
+	def test_from_pd(self):
+		# Sample data
+		data = db.gen_data.gen_lee_bound_data(n=50, p=5, eps_dist='bernoulli', r2=0)
+
+		# Method 1
+		ldb1 = db.lee.LeeDualBounds(
+			covariates=pd.DataFrame(data['X']),
+			outcome=pd.Series(data['y']),
+			treatment=pd.Series(data['W']),
+			selections=pd.Series(data['S']),
+			propensities=pd.DataFrame(data['pis']),
+		)
+
+		# Method 2
+		ldb2 = db.lee.LeeDualBounds(
+			covariates=data['X'],
+			outcome=data['y'],
+			treatment=data['W'],
+			selections=data['S'],
+			propensities=data['pis'],
+		)
+
+		# Test equality
+		self.assertTrue(
+			ldb1.X.shape == ldb2.X.shape,
+			"LeeDualBounds init. from pandas changes the shape of the covariates"
+		)
+		for expected, out, name in zip(
+			[ldb2.y, ldb2.W, ldb2.pis, ldb2.S],
+			[ldb1.y, ldb1.W, ldb1.pis, ldb1.S],
+			['y', 'W', 'pis', 'S'],
+		):
+			np.testing.assert_array_almost_equal(
+				expected,
+				out,
+				decimal=8,
+				err_msg=f"LeeDualBounds init. from pandas changes {name} values."
+			)
+
+
 	def test_model_type_inputs(self):
 		"""
 		Tests that the various model classes don't error and give
 		the correct underlying model type.
 		"""
 		data = db.gen_data.gen_lee_bound_data(
 			n=500, p=3, r2=0, dgp_seed=1, sample_seed=1,
 		)
 
-		for Y_model, S_model, W_model, pis in zip(
+		for outcome_model, selection_model, propensity_model, pis in zip(
 			['rf', 'ridge', 'knn', 'elastic'],
 			['monotone_logistic', 'knn', 'logistic', 'rf'],
 			[None, None, 'knn', 'logistic'],
 			[data['pis'], data['pis'], None, None]
 		):
 			ldb = lee.LeeDualBounds(
-				y=data['y'], W=data['W'], S=data['S'], X=data['X'], pis=pis,
-				Y_model=Y_model, S_model=S_model, W_model=W_model,
+				outcome=data['y'], treatment=data['W'], selections=data['S'], covariates=data['X'], pis=pis,
+				outcome_model=outcome_model, selection_model=selection_model, propensity_model=propensity_model,
 			)
-			ldb.compute_dual_bounds(nfolds=3)
+			ldb.fit(nfolds=3).summary()
 			# Test y-model is correct
 			Ym = ldb.model_fits[0].model
-			Y_exp = db.dist_reg.parse_model_type(Y_model, discrete=False)
+			Y_exp = db.dist_reg.parse_model_type(outcome_model, discrete=False)
 			self.assertTrue(
 				isinstance(Ym, Y_exp),
-				f"fit model {Ym} with Y_model={Y_model} is not of type {Y_exp}"
+				f"fit model {Ym} with outcome_model={outcome_model} is not of type {Y_exp}"
 			)
 			# Test s-model is correct
-			Sm = ldb.S_model_fits[0].model
-			S_exp = db.dist_reg.parse_model_type(S_model, discrete=True)
+			Sm = ldb.selection_model_fits[0].model
+			S_exp = db.dist_reg.parse_model_type(selection_model, discrete=True)
 			self.assertTrue(
 				isinstance(Sm, S_exp),
-				f"fit model {Sm} with S_model={S_model} is not of type {S_exp}"
+				f"fit model {Sm} with selection_model={selection_model} is not of type {S_exp}"
 			)
 			# Test pi model is correct if fit
 			if pis is None:
-				Wm = ldb.W_model_fits[0]
-				W_exp = db.dist_reg.parse_model_type(W_model, discrete=True)
+				Wm = ldb.propensity_model_fits[0]
+				W_exp = db.dist_reg.parse_model_type(propensity_model, discrete=True)
 				self.assertTrue(
 					isinstance(Wm, W_exp),
-					f"fit model {Wm} with S_model={W_model} is not of type {W_exp}"
+					f"fit model {Wm} with selection_model={propensity_model} is not of type {W_exp}"
 				)
 
 
 	@pytest.mark.slow
 	def test_lee_consistency(self):
 		n = 10000
 		p = 3
@@ -373,22 +414,22 @@
 				y0_dists=data['_y0_dists_4input'], 
 				y1_dists=data['_y1_dists_4input'],
 			)
 			## Ground truth
 			expected, _ = lee.compute_analytical_lee_bound(**oracle_args)
 			## Oracle test
 			ldb_oracle = lee.LeeDualBounds(
-				y=data['y'], W=data['W'], S=data['S'], X=data['X'], pis=data['pis'],
+				outcome=data['y'], treatment=data['W'], selections=data['S'], covariates=data['X'], propensities=data['pis'],
 			)
-			est_oracle = ldb_oracle.compute_dual_bounds(**oracle_args, suppress_warning=True)['estimates']
+			est_oracle = ldb_oracle.fit(**oracle_args, suppress_warning=True).estimates
 			## Actual dual bounds
 			ldb = lee.LeeDualBounds(
-				y=data['y'], W=data['W'], S=data['S'], X=data['X'], pis=data['pis'],
+				outcome=data['y'], treatment=data['W'], selections=data['S'], covariates=data['X'], propensities=data['pis'],
 			)
-			est_actual = ldb.compute_dual_bounds(nfolds=3)['estimates']
+			est_actual = ldb.fit(nfolds=3).estimates
 			for est, name in zip([est_oracle, est_actual], ['Oracle', 'Dual']):
 				np.testing.assert_array_almost_equal(
 					est,
 					expected,
 					decimal=1,
 					err_msg=f"{name} Lee bound is not consistent with n={n}"
 				)
```

### Comparing `dualbounds-0.2.1/test/test_utils.py` & `dualbounds-1.0.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dualbounds-0.2.1/test/test_varbounds.py` & `dualbounds-1.0.0/test/test_varbounds.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,17 +31,20 @@
 				n=n, 
 				y0_dists=data['y0_dists'], y1_dists=data['y1_dists'],
 				reps=10,
 			)
 
 			# Compute vdb
 			vdb = db.varite.VarITEDualBounds(
-				X=data['X'], y=data['y'], W=data['W'], pis=data['pis'],
+				covariates=data['X'],
+				outcome=data['y'],
+				treatment=data['W'],
+				propensities=data['pis'],
 			)
-			ests = vdb.compute_dual_bounds(nfolds=3)['estimates']
+			ests = vdb.fit(nfolds=3).estimates
 
 			# test accuracy
 			np.testing.assert_array_almost_equal(
 				np.array([lower, upper]),
 				ests,
 				decimal=1,
 				err_msg=f"Var(ITE) bounds are not consistent, n={n}"
@@ -60,17 +63,21 @@
 	def test_no_error(self):
 		""" This tests if the code runs without error for continuous Y. """
 		for eps_dist in ['gaussian', 'bernoulli']:
 			data = gen_data.gen_regression_data(
 				n=200, p=10, eps_dist=eps_dist, sample_seed=123
 			)
 			vdb = db.varite.VarITEDualBounds(
-				X=data['X'], y=data['y'], W=data['W'], pis=data['pis'],
+				covariates=data['X'],
+				outcome=data['y'],
+				treatment=data['W'],
+				propensities=data['pis'],
 			)
-			output = vdb.compute_dual_bounds(nfolds=3)
+			vdb.fit(nfolds=3).summary()
+
 
 class TestVarCATE(unittest.TestCase):
 
 	def test_varcate_delta_method_se(self):
 		""" Tests that we correctly estimate the SE. """
 		context._run_se_computation_test(
 			dim=6,
@@ -87,43 +94,43 @@
 		Just tests that the discrete case runs without errors.
 		The LogisticCV solver is slow so we don't check consistency.
 		"""
 		data = db.gen_data.gen_lee_bound_data(
 			n=200, p=5, eps_dist='bernoulli',
 		)
 		vdb = db.varcate.VarCATEDualBounds(
-			X=data['X'], y=data['y'], W=data['W'], pis=data['pis'],
+			covariates=data['X'], outcome=data['y'], treatment=data['W'], propensities=data['pis'],
 		)
-		vdb.compute_dual_bounds(nfolds=3)
+		vdb.fit(nfolds=3).summary()
 
 
 	def test_varcate_consistency(self):
 		for eps_dist, r2 in zip(
 			['gaussian', 'expon'], [0.9, 0.5, 0.0]
 		):
 			data = db.gen_data.gen_lee_bound_data(
 				n=300000, p=5, r2=r2, tau=2, dgp_seed=1, sample_seed=1,
 				eps_dist=eps_dist,
 				interactions=True,
 			)
 			expected = data['cates'].std()**2
 			## Oracle
 			vdb_oracle = db.varcate.VarCATEDualBounds(
-				X=data['X'], y=data['y'], W=data['W'], pis=data['pis'],
+				covariates=data['X'], outcome=data['y'], treatment=data['W'], propensities=data['pis'],
 			)
-			est_oracle = vdb_oracle.compute_dual_bounds(
+			est_oracle = vdb_oracle.fit(
 				y0_dists=data['y0_dists'], y1_dists=data['y1_dists'], 
 				suppress_warning=True,
-			)['estimate']
+			).estimates[0]
 			## Actual
 			vdb = db.varcate.VarCATEDualBounds(
-				X=data['X'], y=data['y'], W=data['W'], pis=data['pis'],
-				Y_model=db.dist_reg.CtsDistReg(eps_dist='gaussian')
+				covariates=data['X'], outcome=data['y'], treatment=data['W'], propensities=data['pis'],
+				outcome_model=db.dist_reg.CtsDistReg(eps_dist='gaussian')
 			)
-			est_actual = vdb.compute_dual_bounds(nfolds=3)['estimate']
+			est_actual = vdb.fit(nfolds=3).estimates[0]
 			for est, name in zip([est_oracle, est_actual], ['oracle', 'est']):
 				np.testing.assert_array_almost_equal(
 					est,
 					expected,
 					decimal=2,
 					err_msg=f"VarCATE {name} is inaccurate (r2={r2}, eps_dist={eps_dist})"
 				)
```

