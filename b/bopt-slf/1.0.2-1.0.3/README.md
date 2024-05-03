# Comparing `tmp/bopt_slf-1.0.2.tar.gz` & `tmp/bopt_slf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bopt_slf-1.0.2.tar", last modified: Fri Apr 19 03:43:03 2024, max compression
+gzip compressed data, was "bopt_slf-1.0.3.tar", last modified: Fri May  3 06:39:04 2024, max compression
```

## Comparing `bopt_slf-1.0.2.tar` & `bopt_slf-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.503899 bopt_slf-1.0.2/
--rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bopt_slf-1.0.2/LICENSE.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      524 2024-04-19 03:43:03.503663 bopt_slf-1.0.2/PKG-INFO
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.498293 bopt_slf-1.0.2/bopt_slf/
--rw-r--r--   0 javiermorlet   (501) staff       (20)       58 2024-04-19 03:36:26.000000 bopt_slf-1.0.2/bopt_slf/__init__.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.499722 bopt_slf-1.0.2/bopt_slf/core/
--rw-r--r--   0 javiermorlet   (501) staff       (20)       20 2024-03-23 19:00:17.000000 bopt_slf-1.0.2/bopt_slf/core/__init__.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)    12626 2024-04-16 08:07:37.000000 bopt_slf-1.0.2/bopt_slf/core/main.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.503206 bopt_slf-1.0.2/bopt_slf/utils/
--rw-r--r--   0 javiermorlet   (501) staff       (20)     2256 2024-04-05 04:58:08.000000 bopt_slf-1.0.2/bopt_slf/utils/Acq_fun.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     4235 2024-04-16 03:10:41.000000 bopt_slf-1.0.2/bopt_slf/utils/Aux.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     7155 2024-04-16 07:45:00.000000 bopt_slf-1.0.2/bopt_slf/utils/Dimension_reduction.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)    12137 2024-04-11 07:20:37.000000 bopt_slf-1.0.2/bopt_slf/utils/Initialize.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     3814 2024-04-11 09:08:18.000000 bopt_slf-1.0.2/bopt_slf/utils/Models.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     4748 2024-04-16 03:36:53.000000 bopt_slf-1.0.2/bopt_slf/utils/Plotting.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     3890 2024-04-05 05:04:38.000000 bopt_slf-1.0.2/bopt_slf/utils/Querry_points.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     5908 2024-04-12 09:39:36.000000 bopt_slf-1.0.2/bopt_slf/utils/Set_level_filtration.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     1187 2024-03-17 16:50:23.000000 bopt_slf-1.0.2/bopt_slf/utils/Update.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)      614 2024-04-05 04:49:31.000000 bopt_slf-1.0.2/bopt_slf/utils/__init__.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.499054 bopt_slf-1.0.2/bopt_slf.egg-info/
--rw-r--r--   0 javiermorlet   (501) staff       (20)      524 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/PKG-INFO
--rw-r--r--   0 javiermorlet   (501) staff       (20)      538 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/SOURCES.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/dependency_links.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/requires.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        9 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/top_level.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-04-19 03:43:03.503952 bopt_slf-1.0.2/setup.cfg
--rw-r--r--   0 javiermorlet   (501) staff       (20)      595 2024-04-05 04:56:21.000000 bopt_slf-1.0.2/setup.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-05-03 06:39:04.315936 bopt_slf-1.0.3/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bopt_slf-1.0.3/LICENSE.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      524 2024-05-03 06:39:04.315697 bopt_slf-1.0.3/PKG-INFO
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      663 2024-05-03 03:21:20.000000 bopt_slf-1.0.3/README.md
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-05-03 06:39:04.310970 bopt_slf-1.0.3/bopt_slf/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       58 2024-04-19 03:36:26.000000 bopt_slf-1.0.3/bopt_slf/__init__.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-05-03 06:39:04.312270 bopt_slf-1.0.3/bopt_slf/core/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       20 2024-03-23 19:00:17.000000 bopt_slf-1.0.3/bopt_slf/core/__init__.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     9985 2024-05-01 10:37:39.000000 bopt_slf-1.0.3/bopt_slf/core/main.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-05-03 06:39:04.315300 bopt_slf-1.0.3/bopt_slf/utils/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     2256 2024-04-05 04:58:08.000000 bopt_slf-1.0.3/bopt_slf/utils/Acq_fun.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     5123 2024-05-01 10:45:07.000000 bopt_slf-1.0.3/bopt_slf/utils/Aux.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     7683 2024-05-01 10:03:46.000000 bopt_slf-1.0.3/bopt_slf/utils/Dimension_reduction.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)    14472 2024-05-01 10:37:44.000000 bopt_slf-1.0.3/bopt_slf/utils/Initialize.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     3773 2024-04-25 08:36:05.000000 bopt_slf-1.0.3/bopt_slf/utils/Models.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     4748 2024-04-16 03:36:53.000000 bopt_slf-1.0.3/bopt_slf/utils/Plotting.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     3731 2024-04-25 05:13:47.000000 bopt_slf-1.0.3/bopt_slf/utils/Querry_points.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     5323 2024-05-03 06:22:06.000000 bopt_slf-1.0.3/bopt_slf/utils/Set_level_filtration.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     1187 2024-03-17 16:50:23.000000 bopt_slf-1.0.3/bopt_slf/utils/Update.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      656 2024-05-03 03:08:38.000000 bopt_slf-1.0.3/bopt_slf/utils/__init__.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-05-03 06:39:04.311751 bopt_slf-1.0.3/bopt_slf.egg-info/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      524 2024-05-03 06:39:04.000000 bopt_slf-1.0.3/bopt_slf.egg-info/PKG-INFO
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      548 2024-05-03 06:39:04.000000 bopt_slf-1.0.3/bopt_slf.egg-info/SOURCES.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-05-03 06:39:04.000000 bopt_slf-1.0.3/bopt_slf.egg-info/dependency_links.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-05-03 06:39:04.000000 bopt_slf-1.0.3/bopt_slf.egg-info/requires.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        9 2024-05-03 06:39:04.000000 bopt_slf-1.0.3/bopt_slf.egg-info/top_level.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-05-03 06:39:04.315985 bopt_slf-1.0.3/setup.cfg
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      595 2024-04-23 13:07:36.000000 bopt_slf-1.0.3/setup.py
```

### Comparing `bopt_slf-1.0.2/LICENSE.txt` & `bopt_slf-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.2/PKG-INFO` & `bopt_slf-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bopt_slf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
 Author: Javier Morlet-Espinosa
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Acq_fun.py` & `bopt_slf-1.0.3/bopt_slf/utils/Acq_fun.py`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Aux.py` & `bopt_slf-1.0.3/bopt_slf/utils/Aux.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import multiprocess as mp
 import numpy as np
 
 # *******************************************************
 
 def Errors(n_x, n_y, design_type, surrogate, constraints_method, AF_name):
 
-    valid_var_type = ["continuous", "discrete", "categorical"]
+    valid_var_type = ["continuous", "integer", "categorical"]
     valid_design_type = ["random", "LHS", "Sobol", "Halton", "Mesh"]
     valid_surrogate_name = ["GP", "SGP"]
     valid_constraints_method = ["PoF", "GPC"]
     valid_af_names = ['UCB', 'EI', 'PI']
 
     if n_x <= 0 and n_y <= 0:
         raise ValueError("Not valid variable type, valid names are:", *valid_var_type)
@@ -35,28 +35,28 @@
 
     if enc_cat != None:
         x_conv = []
         for i in range(len(enc_cat)):
             ix_cat = (dims - n_c)
             x_conv.append(enc_cat[i].inverse_transform(x[:,ix_cat+i].reshape(-1,1)))
         x_conv = np.array(x_conv).reshape(-1,1)
-        x_eval = np.hstack((x[:, :ix_cat], np.asarray(x_conv,object)))
+        x_eval = np.hstack((x[:, :ix_cat], np.asarray(x_conv, object)))
     else:
         x_eval = x
     
     return x_eval
 
 # *******************************************************
 
-def Eval_fun(x, n_elements, parallelization, jobs, function):
+def Eval_fun(x, n_elements, jobs, function):
 
-    if parallelization == "no":
+    if jobs == 1:
         x_new = np.array(x).reshape(1,-1)
         z_new = function(x_new)
-    elif parallelization == "yes":
+    else:
         x_new = [x[i].reshape(1,-1) for i in range(n_elements)]
         with mp.Pool(jobs) as pool:
             z_new = pool.map(function, x_new)
         
     return z_new
 
 # *******************************************************
@@ -68,42 +68,77 @@
     elif constraints_method == "GPC":
         data = [eval(const[i]['constraint'], None, {"x": x}) for i in range(n_const)]
 
     return np.array(data).reshape(-1, n_const)
 
 # *******************************************************
 
+def Best_values(x, z, sense):
+
+    if sense == "maximize":
+        ix_best = np.argmax(z)
+        z_best = np.max(z)
+    elif sense == "minimize":
+        ix_best = np.argmin(z)
+        z_best = np.min(z)
+    x_best = x[ix_best]
+
+    return x_best, z_best
+
+# *******************************************************
+
 def Regret(z_true, x, n_elements, model):
     # Return an average of the reward
     z_pred, _ = model.predict(x)
     rt = [(z_true[i] - z_pred[i]) for i in range(n_elements)]
     rt = sum(rt)
 
     return rt/n_elements
 
 # *******************************************************
 
-def Print_results(x, enc_cat):
+def Print_header(names, x_symb_names, dims):
+
+    if names is None:
+        header = 'ite  ' +  '  f      ' + str(x_symb_names[0])
+    else:
+        header = 'ite  ' +  '  f      ' + str(names[0])
+    for i in range(1, dims):
+        if names is None:
+            header += '      ' + str(x_symb_names[i])
+        else:
+            header += '      ' + str(names[i])
+    
+    return header
+
+# *******************************************************
+
+def Print_results(x, z, n_c, dims, enc_cat):
+
+    x_eval = Data_eval(x.reshape(1,-1), n_c, dims, enc_cat)
 
     if enc_cat is None:
-        x = x.reshape(-1)
+        x = x_eval.reshape(-1)
         x_print = ["%.5f" % value if 1e-3 < abs(value) < 1e3 else "%0.1e" % value for value in x]
     else:
+        x = x_eval
         x = x[0]
         x_print = [] 
         for value in x:
             if type(value) == str:
                 x_print.append(value)
             elif type(value) == float:
                 if 1e-3 < abs(value) < 1e3:
                     x_print.append("%.5f" % value)
                 else:
                     x_print.append("%0.1e" % value)
+    
+    z_print = "%.5f" % z if 1e-3 < abs(z) < 1e3 else "%0.1e" % z
         
-    return x_print
+    return x_print, z_print
 
 # *******************************************************
 
 def Create_results(x_best, z_best, x, z, x_l, x_u, dims, max_iter, points, design, af_params, constraints_method, rt, models_const, model):
 
     res = {'x_best': x_best, 'f_best': z_best, 
            'x_init': x[0:points], 'f_init': z[0:points],
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Dimension_reduction.py` & `bopt_slf-1.0.3/bopt_slf/utils/Dimension_reduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,18 +203,28 @@
         model_names = np.arange(len(model))
         model = dict(zip(model_names, list(model.values())))
 
     return model
 
 # *******************************************************
 
-def Red_bounds(mesh, x_l, x_u, n_x, dims, dims_red, problem_type, reducer):
+def Red_bounds(x_l, x_u, y_v, n_x, n_y, dims, dims_red, problem_type, reducer):
 
     if reducer is None:
         x_l_red = x_l
         x_u_red = x_u
     else:
-        x_mesh_red = Reduce(mesh, n_x, dims, problem_type, reducer)
+        if problem_type == "Continuous":
+            lists = [[x_l[i], x_u[i]] for i in range(dims)]
+        elif problem_type == "Mixed":
+            lists_x = [[x_l[i], x_u[i]] for i in range(n_x)]
+            lists_y = [[y_v[i][0], y_v[i][-1]] for i in range(n_y)]
+            lists = np.vstack((lists_x, lists_y)).tolist()
+        elif problem_type == "Discrete":
+            lists = [[y_v[i][0], y_v[i][-1]] for i in range(dims)]
+        mesh = np.meshgrid(*lists)
+        x_mesh = np.array(mesh).T.reshape(-1, dims)
+        x_mesh_red = Reduce(x_mesh, n_x, dims, problem_type, reducer)
         x_l_red = np.array([x_mesh_red[0,i] for i in range(dims_red)])
         x_u_red = np.array([x_mesh_red[-1,i] for i in range(dims_red)])
 
     return x_l_red, x_u_red
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Initialize.py` & `bopt_slf-1.0.3/bopt_slf/utils/Initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # *******************************************************
 # Import libraries
 
+import time
 import numpy as np
+import multiprocess as mp
 from scipy.stats import qmc
 from sklearn.preprocessing import OrdinalEncoder
-import time
+from GPy.kern import RBF
+from ..utils.Aux import Data_eval
+from ..utils.Models import Kernel_discovery
 
 # *******************************************************
 
 def Space(domain):
 
     """ 
     Gets an array for the lower and upper bounds of the continuous variables, and a tuple for the discrete variables.
@@ -30,15 +34,15 @@
             names.append(domain[i]['name'])
         except:
             names = 0
         if domain[i]['type'] == "continuous":
             n_x += 1
             x_l.append(domain[i]['domain'][0])
             x_u.append(domain[i]['domain'][1])
-        elif domain[i]['type'] == "discrete":
+        elif domain[i]['type'] == "integer":
             n_d += 1
             dis_val.append(domain[i]['domain'])
         elif domain[i]['type'] == "categorical":
             n_c += 1
             enc_cat.append(OrdinalEncoder())
             X = domain[i]['domain']
             X = [[(X[i])] for i in range(len(X))]
@@ -84,70 +88,35 @@
 
 # *******************************************************
 
 def Get_constraints(constraints, constraints_method):
 
     "Transforms tuple of constraints into list"
 
-    n_const = len(constraints)
-
-    if constraints_method == "PoF":
-        symbols = ['<=', '>=']
-        const = []
-        for i in range(n_const):
-            for s in symbols:
-                try:
-                    index_const = constraints[i]['constraint'].index(s)
-                    const.append(constraints[i]['constraint'][:index_const-1])
-                except:
-                    pass
-    elif constraints_method == "GPC":
-        const = constraints
+    if constraints is None:
+        const, n_const = None, None
+    else:
+        n_const = len(constraints)
+        if constraints_method == "PoF":
+            symbols = ['<=', '>=']
+            const = []
+            for i in range(n_const):
+                for s in symbols:
+                    try:
+                        index_const = constraints[i]['constraint'].index(s)
+                        const.append(constraints[i]['constraint'][:index_const-1])
+                    except:
+                        pass
+        elif constraints_method == "GPC":
+            const = constraints
     
     return const, n_const
 
 # *******************************************************
 
-def Times_fun(fun, x):
-
-    """ 
-    Generates the number of points of the mesh or grid, depending on the cost of the evaluation of the function, and the dimensions of the problem
-    """
-    
-    start = time.time()
-    f_eval = fun(x.reshape(1,-1))
-    end = time.time()
-    
-    return (end - start), f_eval
-
-# *******************************************************
-
-def Points_initial_design(times, dims, design, c_param = 50):
-
-    if times <= 1:
-        exp_param = 0.25
-    else: 
-        exp_param = 0.95
-    
-    points_D = int(c_param - c_param/(1+(1/times)**exp_param))
-
-    if design == "Mesh":
-        points_D = int(np.ceil(points_D)**(1/dims))
-    elif design == "Sobol":
-        points_D = int(np.ceil(np.sqrt(points_D))**2)
-    else:
-        pass
-
-    if points_D < 3:
-        points_D = int(3)
-
-    return points_D
-
-# *******************************************************
-
 def x_Generator(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, design_type):
 
     def Random_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type):
 
         def Bounds_y(y_v, n_y):
 
             y_l = []
@@ -170,15 +139,15 @@
             return np.random.uniform(x_l, x_u, size=(points, dims))
         
         def Y_rand(y_v, n_y, points):
 
             y_l, y_u, flag = Bounds_y(y_v, n_y)
 
             if flag == 1:
-                y_rand = np.random.randint(y_l, y_u, size=(points, dims))
+                y_rand = np.random.randint(y_l, y_u, size=(points, n_y))
             elif flag == 0:
                 size_y = [len(y_v[i]) for i in range(n_y)]
                 l = [np.repeat(1/size_y[i], size_y[i]) for i in range(n_y)]
                 sample = [np.random.choice(y_v[i], p=l[i], size=(points, 1)).reshape(-1) for i in range(n_y)]
                 y_rand = np.array(sample).T
             else:
                 pass
@@ -188,15 +157,15 @@
         if problem_type == "Continuous":
             variables = X_rand(x_l, x_u, dims, points)
         elif problem_type == "Mixed":
             x_variables = X_rand(x_l, x_u, n_x, points)
             y_variables = Y_rand(y_v, n_y, points)
             variables = np.hstack((x_variables, y_variables))
         elif problem_type == "Discrete":
-            variables = Y_rand(y_v, dims, points)[0]
+            variables = Y_rand(y_v, dims, points)
         else:
             pass
 
         return variables
     
     def QMC_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, design_type):
 
@@ -333,48 +302,150 @@
 
     # Main program
     if design_type == "random":
         variables = Random_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type)
     elif design_type == "LHS":
         variables = QMC_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, "LHS")
     elif design_type == "Sobol":
-        points = int(np.ceil(np.sqrt(points))**2)
         variables = QMC_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, "Sobol")
     elif design_type == "Halton":
         variables = QMC_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, "Halton")
     elif design_type == "Mesh":
         variables = Mesh_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type)
     else:
         pass
     
     return variables
 
+# ******************************************************* 
+
+def Get_x_and_z(fun, x_0, z_0, x_l, x_u, y_v, n_x, n_y, n_c, dims, enc_cat, p_design, design, problem_type):
+
+# *************************
+
+    def Times_fun(fun, x):
+
+        """ 
+        Generates the number of points of the mesh or grid, depending on the cost of the evaluation of the function, and the dimensions of the problem
+        """
+        
+        start = time.time()
+        f_eval = fun(x.reshape(1,-1))
+        end = time.time()
+        
+        return (end - start), f_eval
+
+# *************************
+
+    def Points_initial_design(times, dims, design, c_param = 50):
+
+        """ 
+        Generates the number of initial points of the design
+        """
+
+        if times <= 1:
+            exp_param = 0.25
+        else: 
+            exp_param = 0.95
+        points_D = int(c_param - c_param/(1+(1/times)**exp_param))
+        # Adjust points if design is Mesh or Sobol. 
+        if design == "Mesh":
+            points_D = int(np.ceil(points_D)**(1/dims))
+        elif design == "Sobol":
+            points_D = int(np.ceil(np.sqrt(points_D))**2)
+        else:
+            pass
+        if points_D < 3:
+            points_D = int(3)
+
+        return points_D
+    
+    if x_0 is None:
+        # Evaluate an arbitrary point to determine the computation time of the function
+        x_trial = x_Generator(x_l, x_u, y_v, n_x, n_y, dims, 1, problem_type, "random")
+        x_eval = Data_eval(x_trial, n_c, dims, enc_cat)
+        times, z_trial = Times_fun(fun, x_eval)
+        if p_design == None:
+            p_design = Points_initial_design(times, dims, design)
+        x_0 = x_Generator(x_l, x_u, y_v, n_x, n_y, dims, p_design, problem_type, design)
+        x_eval = Data_eval(x_0, n_c, dims, enc_cat)
+        z_0 = fun(x_eval).reshape(-1,1)
+        x, z = np.vstack((x_0, x_trial)), np.vstack((z_0, z_trial))
+    else:
+        x = x_0
+        if z_0 is None:
+            x_eval = Data_eval(x_0, n_c, dims, enc_cat)
+            z = fun(x_eval).reshape(-1,1)
+        else:
+            p_design = len(z_0)
+            z = z_0
+    
+    return x, z
+
 # *******************************************************
 
 def Bounds(x_l, x_u, dims):
 
     bnds = np.sort(np.array([[x_l[i], x_u[i]] for i in range(dims)]))
     return tuple(map(tuple, bnds))
 
 # *******************************************************
 
-def Points_mesh(dims, r1=9):
+def Get_kernel(x_red, z, dims_red, kern_discovery, kern_discovery_evals, surrogate, kernel):
+
+    if kern_discovery == "yes":
+        model = Kernel_discovery(x_red, z, dims_red, surrogate, kern_discovery_evals)
+        kernel_ = model.kern
+    elif kern_discovery == "no" and kernel is None:
+        kernel_ = RBF(input_dim=dims_red, variance=1.0, lengthscale=1.0)
+    else:
+        kernel_ = kernel
+
+    return kernel_
+
+# *******************************************************
+
+def Points_mesh(dims, r1=10):
 
     """ 
     Generates the points mesh
     """
-    points = int(np.ceil(2**r1)**(1/dims))
-
+    points = int(np.ceil(2**(r1/dims)))
     if points < 3:
         points = 3
 
     return points
 
 # *******************************************************
 
+def Percentile_q(max_iter):
+
+    q0 = 25
+    qf = 75
+    delta_q = (qf-q0)/max_iter
+    q_inc = q0
+    q = q0
+
+    return q, q_inc, delta_q
+
+# *******************************************************
+
+def Num_jobs(n_jobs):
+
+    if n_jobs == -1:
+        jobs = mp.cpu_count()
+    elif n_jobs == None:
+        jobs = 1
+    else:
+        jobs = n_jobs
+    
+    return jobs
+
+# *******************************************************
+
 def AF_params(z, xi, xi_decay, iters, AF_name, sense):
 
     if xi_decay == "yes":
         xi_decay = (1/xi)**(1/iters)
     elif xi_decay == "no":
         xi_decay = 1
     else:
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Models.py` & `bopt_slf-1.0.3/bopt_slf/utils/Models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def Select_model(x, z, kernel, surrogate):
 
     if surrogate == "GP":
         model = GPy.models.GPRegression(x, z, kernel)
     elif surrogate == "SGP":
         model = GPy.models.SparseGPRegression(x, z, kernel)
     else:
-        raise ValueError('Not valid surrogate model')
+        pass
     
     return model
 
 # *******************************************************
 
 def Train_model(model, n_restarts):
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Plotting.py` & `bopt_slf-1.0.3/bopt_slf/utils/Plotting.py`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Querry_points.py` & `bopt_slf-1.0.3/bopt_slf/utils/Querry_points.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,74 +29,70 @@
         Sigma = []
 
         if dims == 1:
             for i in range(n_elements):
                 var = np.var(matrix[i]/np.sqrt(len(matrix[i])), axis=0)
                 if var == 0:
                     Sigma.append(1e-6)
-                    P.append(1/(1e-6))
                     chi.append(1.4)
                 else:
                     Sigma.append(var)
                     var_inv = 1/var
-                    P.append(var_inv)
                     y = matrix[i] - mu[i]
                     dist = [(y[j]*np.sqrt(var_inv)) for j in range(len(y))]
                     chi.append(np.percentile(dist, 95))
         else:                
             for i in range(n_elements):
                 if (len(matrix[i]) < 3):
                     cov = np.eye(dims)
                     Sigma.append(cov)
-                    P.append(cov)
                     chi.append(1.4)
                 else:
                     # Covariance matrix
                     cov = np.cov(matrix[i].T)
-                    # Check if the covariance matrix is singular, if so, add a small value to the diagonal
+                    # Check if the covariance matrix is singular. If so, add a small value to the diagonal
                     if np.linalg.det(cov) == 0:
                         cov = cov + 1e-6*np.eye(dims)
                         # Inverse of the covariance matrix
                     cov_inv = np.linalg.inv(cov)
                     y = matrix[i]-mu[i].T
                     dist = [np.sqrt(y[j].T@cov_inv@y[j]) for j in range(len(y))]
                     Sigma.append(cov_inv)
-                    P.append(cov)
                     chi.append(np.percentile(dist, 95))
 
-        return mu, Sigma, P, chi
+        return mu, Sigma, chi
 
     def Constrains(x, n_elements, mu, P, chi):
 
+        # lambda function for the constrains
+        def Constraint_lambify(fun):
+
+            lam = lambda x: fun(*x)
+            return lam
+
         const = []
 
         for i in range(n_elements):
             y = (x-mu[i])
             dist = y.T*P[i]*y
             const.append(sp.LessThan(dist[0], chi[i]))
             
         const_lamb = [sp.lambdify(x, (const[i].rhs - const[i].lhs), 'numpy') for i in range(n_elements)]
-        # lambda function for the constrains
-        def Constraint_lambify(fun):
-
-            lam = lambda x: fun(*x)
-            return lam
-
         constraints = [Constraint_lambify(const_lamb[i]) for i in range(n_elements)]
         
         return constraints
     
     # Main program
     # Check if the initial database is empty
     if x_matrix is None:
         raise ValueError('Initial database is empty')
     # Compute the confidence region
-    mu, Sigma, P, chi = Mahalanobis_distance(x_matrix, n_elements)
+    mu, Sigma, chi = Mahalanobis_distance(x_matrix, n_elements)
     # Define the constrains
     constraints = Constrains(x, n_elements, mu, Sigma, chi)
     # Define the optimization problem
     x_opt = []
     for i in range(n_elements):
         res = minimize(Acquisition_function_opt, x0=mu[i], args=(af_params, sense, model, models_const), method='SLSQP', bounds=bounds, constraints={'type': 'ineq', 'fun': constraints[i]})
-        x_opt.append(res.x)        
+        x_opt.append(res.x)
 
     return x_opt
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Set_level_filtration.py` & `bopt_slf-1.0.3/bopt_slf/utils/Set_level_filtration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Create class for the querry points using Gaussian Process, UCB and Set-level filtration
-# Each querry point is a connected component of the matrix of points x in the domain adove the level set
+# Find connected component of the matrix of points x in the domain adove the level set
 
 # *******************************************************
 # Import libraries
 import numpy as np
 from itertools import product, permutations
 
 # *******************************************************
@@ -20,15 +19,15 @@
         elif sense == "minimize":
             data_matrix = np.array([score < level])[0]
         # Reshape the data
         data_matrix = data_matrix.reshape(*[p_x]*dims)
 
         return data_matrix.astype(int), x.reshape(*[p_x]*dims, dims)
 
-    def Find_connected_elements(nodes, matrix):
+    def Find_connected_elements_dfs(nodes, matrix):
         # Number of dimensions
         D = [nodes.shape[i] for i in range(dims)]
         D0 = D[0]
         # Define the neighbors
         s_neg = [-1]
         s_pos = [1]
         for i in range(dims-1):
@@ -70,15 +69,15 @@
         connected_elements = []
         level = np.percentile(np.concatenate(score), q)
         if level == 0:
             level = np.mean(np.concatenate(score))
         #
         for j in range(n_elements):
             x_flitred = Filtration(x[j], score[j], p_x[j], dims, level, sense)
-            connected_elements.append(Find_connected_elements(x_flitred[0], x_flitred[1])) 
+            connected_elements.append(Find_connected_elements_dfs(x_flitred[0], x_flitred[1])) 
 
         connected_elements = [x for x in connected_elements if x != []]
         connected_elements = Flatten(connected_elements)
         n_connected_elements = len(connected_elements)
 
         return connected_elements, n_connected_elements
     
@@ -90,52 +89,47 @@
 
         score_all = np.concatenate(score)
         mesh_all = np.concatenate(mesh)
         scores_lst = []
         scores_mean = []
 
         for i in range(n_elements):
-            #connected_elements[0]
             scores_lst.append(np.array([Replace_val(x[i][j], mesh_all, score_all) for j in range(len(x[i]))]))
 
         for i in range(n_elements):
             if len(scores_lst[i].shape) == 1:
                 scores_mean.append(np.mean([np.mean(scores_lst[i][j]) for j in range(len(scores_lst[i]))]))
-                #for j in range(len(scores_lst[i])):
-                #    scores_mean.append(np.mean(scores_lst[i][j]))
             else:
                 scores_mean.append(np.mean(scores_lst[i]))
-            #except:
-            #    print(scores_lst)
-            #    print('Todo: Broadcast error with numpy mean function to be solved')
                 
         if sense == "maximize":
             sorted = np.sort(scores_mean)[::-1][:jobs]
         elif sense == "minimize":
             sorted = np.sort(scores_mean)[:jobs]
         l = np.array([np.where(scores_mean == sorted[i]) for i in range(len(sorted))]).reshape(-1)
+        #print(l)
+        try:
+            l = Flatten(l)
+            l = list(set(l))
+        except:
+            l = l
         connected_elements = [x[i] for i in l]
         n_connected_elements = len(connected_elements)
 
         return connected_elements, n_connected_elements
     
+    # Main
     score = [Acq_fun(mesh[i], af_params, constraints_method, model, models_const) for i in range(len(mesh))]
     n_elements = len(mesh)
-    q_D = []
-    flag = 0
-    
-    for q in range(q0, 0, -5):
-        if sense == "maximize":
-            connected_elements, n_connected_elements = List_of_elements(mesh, score, p_mesh, n_elements, dims, q, sense)
-            q_D.append([q, connected_elements, n_connected_elements])
-        elif sense == "minimize":
-            connected_elements, n_connected_elements = List_of_elements(mesh, score, p_mesh, n_elements, dims, 100-q, sense)
-            q_D.append([100-q, connected_elements, n_connected_elements])
-        if n_connected_elements < jobs:
-            flag = 1
-            break
-
-    if flag == 0:
-        q, connected_elements, n_connected_elements = q_D[0][0], q_D[0][1], q_D[0][2]
+    # 
+    if sense == "maximize":
+        connected_elements, n_connected_elements = List_of_elements(mesh, score, p_mesh, n_elements, dims, q0, sense)
+    elif sense == "minimize":
+        connected_elements, n_connected_elements = List_of_elements(mesh, score, p_mesh, n_elements, dims, 100-q0, sense)
+    else:
+        pass
+    #  
+    if n_connected_elements > jobs:
         connected_elements, n_connected_elements = Reduce_num_elements(connected_elements, mesh, score, n_connected_elements, jobs, sense)
+        
 
     return connected_elements, n_connected_elements
```

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/Update.py` & `bopt_slf-1.0.3/bopt_slf/utils/Update.py`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.2/bopt_slf/utils/__init__.py` & `bopt_slf-1.0.3/bopt_slf/utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from .Acq_fun import UCB, PI, EI, PoF, Prob_GPC, AF
-from .Aux import Errors, Data_eval, Eval_fun, Eval_const, Regret, Print_results, Create_results
+from .Aux import Errors, Data_eval, Eval_fun, Eval_const, Best_values, Regret, Print_results, Print_header, Create_results
 from .Dimension_reduction import Trans_data_to_pandas, Reduce, Inverse, Train_reducer, Train_inverter, Find_reducer, Find_inverter, Red_bounds
-from .Initialize import Space, Problem_type, Get_constraints, Times_fun, Points_initial_design, x_Generator, Bounds, Points_mesh, AF_params
+from .Initialize import Space, Problem_type, Get_constraints, x_Generator, Get_x_and_z, Bounds, Get_kernel, Points_mesh, Percentile_q, Num_jobs, AF_params
 from .Models import Select_model, Train_model, Train_models_const, Kernel_discovery
 from .Querry_points import Querry
 from .Set_level_filtration import Slf
 from .Update import Up_mesh
```

### Comparing `bopt_slf-1.0.2/bopt_slf.egg-info/PKG-INFO` & `bopt_slf-1.0.3/bopt_slf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bopt-slf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
 Author: Javier Morlet-Espinosa
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
```

### Comparing `bopt_slf-1.0.2/bopt_slf.egg-info/SOURCES.txt` & `bopt_slf-1.0.3/bopt_slf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+README.md
 setup.py
 bopt_slf/__init__.py
 bopt_slf.egg-info/PKG-INFO
 bopt_slf.egg-info/SOURCES.txt
 bopt_slf.egg-info/dependency_links.txt
 bopt_slf.egg-info/requires.txt
 bopt_slf.egg-info/top_level.txt
```

### Comparing `bopt_slf-1.0.2/setup.py` & `bopt_slf-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='bopt_slf',
-    version='1.0.2',
+    version='1.0.3',
     description='Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems',
     author='Javier Morlet-Espinosa',
     author_email='a00833961@tec.mx',
     packages = find_packages(),
     install_requires=[
         'numpy>=1.23.5',
         'sympy>=1.11.1',
```

