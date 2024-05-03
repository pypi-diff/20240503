# Comparing `tmp/nndp-0.0.9.tar.gz` & `tmp/nndp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nndp-0.0.9.tar", last modified: Thu Apr 18 20:01:52 2024, max compression
+gzip compressed data, was "nndp-0.1.0.tar", last modified: Fri May  3 14:44:52 2024, max compression
```

## Comparing `nndp-0.0.9.tar` & `nndp-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 20:01:52.716621 nndp-0.0.9/
--rwxr-xr-x   0 mbarrera (10656) users      (100)     1098 2023-02-26 23:27:51.000000 nndp-0.0.9/LICENSE
--rw-r--r--   0 mbarrera (10656) users      (100)     4448 2024-04-18 20:01:52.713624 nndp-0.0.9/PKG-INFO
--rw-r--r--   0 mbarrera (10656) users      (100)     2702 2024-04-17 12:06:41.000000 nndp-0.0.9/README.md
--rw-r--r--   0 mbarrera (10656) users      (100)      663 2024-04-18 20:00:27.000000 nndp-0.0.9/pyproject.toml
--rw-r--r--   0 mbarrera (10656) users      (100)       38 2024-04-18 20:01:52.716628 nndp-0.0.9/setup.cfg
-drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 20:01:52.647621 nndp-0.0.9/src/
-drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 20:01:52.662621 nndp-0.0.9/src/nndp/
--rwxr-xr-x   0 mbarrera (10656) users      (100)       66 2024-04-18 20:00:28.000000 nndp-0.0.9/src/nndp/__init__.py
-drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 20:01:52.698622 nndp-0.0.9/src/nndp/agnostic/
--rw-r--r--   0 mbarrera (10656) users      (100)      126 2024-04-13 14:51:09.000000 nndp-0.0.9/src/nndp/agnostic/__init__.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)      370 2024-04-13 13:34:40.000000 nndp-0.0.9/src/nndp/agnostic/analysis.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)      266 2024-04-12 18:32:39.000000 nndp-0.0.9/src/nndp/agnostic/model.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)      949 2024-04-12 18:32:37.000000 nndp-0.0.9/src/nndp/agnostic/policy.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)     1821 2024-04-13 13:34:41.000000 nndp-0.0.9/src/nndp/agnostic/samplers.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)     6324 2024-04-18 19:37:37.000000 nndp-0.0.9/src/nndp/agnostic/train.py
-drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 20:01:52.706623 nndp-0.0.9/src/nndp/core/
--rw-r--r--   0 mbarrera (10656) users      (100)       20 2024-04-18 19:37:34.000000 nndp-0.0.9/src/nndp/core/__init__.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)     5111 2024-04-18 19:59:31.000000 nndp-0.0.9/src/nndp/core/policy_function.py
--rwxr-xr-x   0 mbarrera (10656) users      (100)     7492 2024-04-18 19:59:31.000000 nndp-0.0.9/src/nndp/core/train.py
-drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 20:01:52.709629 nndp-0.0.9/src/nndp.egg-info/
--rw-r--r--   0 mbarrera (10656) users      (100)     4448 2024-04-18 20:01:52.000000 nndp-0.0.9/src/nndp.egg-info/PKG-INFO
--rw-r--r--   0 mbarrera (10656) users      (100)      466 2024-04-18 20:01:52.000000 nndp-0.0.9/src/nndp.egg-info/SOURCES.txt
--rw-r--r--   0 mbarrera (10656) users      (100)        1 2024-04-18 20:01:52.000000 nndp-0.0.9/src/nndp.egg-info/dependency_links.txt
--rw-r--r--   0 mbarrera (10656) users      (100)      108 2024-04-18 20:01:52.000000 nndp-0.0.9/src/nndp.egg-info/requires.txt
--rw-r--r--   0 mbarrera (10656) users      (100)        5 2024-04-18 20:01:52.000000 nndp-0.0.9/src/nndp.egg-info/top_level.txt
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-05-03 14:44:52.708732 nndp-0.1.0/
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     1098 2023-02-26 23:27:51.000000 nndp-0.1.0/LICENSE
+-rw-r--r--   0 mbarrera (10656) users      (100)     4448 2024-05-03 14:44:52.706731 nndp-0.1.0/PKG-INFO
+-rw-r--r--   0 mbarrera (10656) users      (100)     2702 2024-04-17 12:06:41.000000 nndp-0.1.0/README.md
+-rw-r--r--   0 mbarrera (10656) users      (100)      663 2024-05-03 14:44:16.000000 nndp-0.1.0/pyproject.toml
+-rw-r--r--   0 mbarrera (10656) users      (100)       38 2024-05-03 14:44:52.709729 nndp-0.1.0/setup.cfg
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-05-03 14:44:52.650728 nndp-0.1.0/src/
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-05-03 14:44:52.661739 nndp-0.1.0/src/nndp/
+-rwxr-xr-x   0 mbarrera (10656) users      (100)       66 2024-05-03 14:40:46.000000 nndp-0.1.0/src/nndp/__init__.py
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-05-03 14:44:52.691732 nndp-0.1.0/src/nndp/agnostic/
+-rw-r--r--   0 mbarrera (10656) users      (100)      126 2024-04-13 14:51:09.000000 nndp-0.1.0/src/nndp/agnostic/__init__.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)      370 2024-04-13 13:34:40.000000 nndp-0.1.0/src/nndp/agnostic/analysis.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)      266 2024-04-12 18:32:39.000000 nndp-0.1.0/src/nndp/agnostic/model.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)      949 2024-04-12 18:32:37.000000 nndp-0.1.0/src/nndp/agnostic/policy.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     1821 2024-04-13 13:34:41.000000 nndp-0.1.0/src/nndp/agnostic/samplers.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     6324 2024-04-18 19:37:37.000000 nndp-0.1.0/src/nndp/agnostic/train.py
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-05-03 14:44:52.699733 nndp-0.1.0/src/nndp/core/
+-rw-r--r--   0 mbarrera (10656) users      (100)       50 2024-05-03 14:40:42.000000 nndp-0.1.0/src/nndp/core/__init__.py
+-rw-r--r--   0 mbarrera (10656) users      (100)     7253 2024-05-03 14:41:30.000000 nndp-0.1.0/src/nndp/core/neural_network.py
+-rw-r--r--   0 mbarrera (10656) users      (100)     7862 2024-05-03 14:40:44.000000 nndp-0.1.0/src/nndp/core/train.py
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-05-03 14:44:52.702737 nndp-0.1.0/src/nndp.egg-info/
+-rw-r--r--   0 mbarrera (10656) users      (100)     4448 2024-05-03 14:44:52.000000 nndp-0.1.0/src/nndp.egg-info/PKG-INFO
+-rw-r--r--   0 mbarrera (10656) users      (100)      465 2024-05-03 14:44:52.000000 nndp-0.1.0/src/nndp.egg-info/SOURCES.txt
+-rw-r--r--   0 mbarrera (10656) users      (100)        1 2024-05-03 14:44:52.000000 nndp-0.1.0/src/nndp.egg-info/dependency_links.txt
+-rw-r--r--   0 mbarrera (10656) users      (100)      108 2024-05-03 14:44:52.000000 nndp-0.1.0/src/nndp.egg-info/requires.txt
+-rw-r--r--   0 mbarrera (10656) users      (100)        5 2024-05-03 14:44:52.000000 nndp-0.1.0/src/nndp.egg-info/top_level.txt
```

### Comparing `nndp-0.0.9/LICENSE` & `nndp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nndp-0.0.9/PKG-INFO` & `nndp-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nndp
-Version: 0.0.9
+Version: 0.1.0
 Summary: Dynamic Programming using Neural Networks
 Author-email: Marc de la Barrera <marc.delabarrera@gmail.com>, Tim de Silva <tdesilva@mit.edu>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `nndp-0.0.9/README.md` & `nndp-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nndp-0.0.9/pyproject.toml` & `nndp-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "nndp"
-version = "0.0.9"
+version = "0.1.0"
 description = "Dynamic Programming using Neural Networks"
 readme = "README.md"
 authors = [{ name = "Marc de la Barrera", email = "marc.delabarrera@gmail.com" }, { name = "Tim de Silva", email = "tdesilva@mit.edu" }]
 license = { file = "LICENSE" }
 keywords = ["economics"]
 dependencies = [
     "numpy >= 1.20.0",
```

### Comparing `nndp-0.0.9/src/nndp/agnostic/policy.py` & `nndp-0.1.0/src/nndp/agnostic/policy.py`

 * *Files identical despite different names*

### Comparing `nndp-0.0.9/src/nndp/agnostic/samplers.py` & `nndp-0.1.0/src/nndp/agnostic/samplers.py`

 * *Files identical despite different names*

### Comparing `nndp-0.0.9/src/nndp/agnostic/train.py` & `nndp-0.1.0/src/nndp/agnostic/train.py`

 * *Files identical despite different names*

### Comparing `nndp-0.0.9/src/nndp/core/train.py` & `nndp-0.1.0/src/nndp/core/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from jax._src.prng import PRNGKeyArray
 from jax._src.basearray import Array
 from typing import Callable
 import jax.numpy as jnp
 from jax.tree_util import Partial
 import optax
 
+
+@Partial(jax.jit, static_argnames=['policy','nn','u','m', 'N_simul', 'T'])
 def evaluate_policy(key:PRNGKeyArray,
                     policy: Callable[[Array, Array], Array],
+                    params: dict,
+                    nn: Callable,
                     u: Callable[[Array, Array], Array],
                     m: Callable[[PRNGKeyArray, Array, Array], Array], 
                     s0: Array,
                     T: int,
                     N_simul: int=1
                     ) -> Array:
     '''
@@ -34,23 +38,24 @@
         E(\sum_{t=0}^T \beta^t u(action_t, state_t) | state_0 = s0(k))
     '''
     K = s0.shape[0]
     state = jnp.repeat(s0, repeats = N_simul, axis = 0)
     V = jnp.zeros((K * N_simul, 1))
     key, *subkey = jax.random.split(key, (T + 1))
     for t in range(T):
-        action = policy(state)
+        action = policy(state, params, nn)
         V += u(state, action) 
         state = m(subkey[t], state, action)
     V = V.reshape(K, -1)
     return jnp.mean(V, axis = 1, keepdims = True)                    
 
 def train_step(key:PRNGKeyArray,
                params:dict,
-               policy:Callable[[Array, Array], Array],
+               policy:Callable[[Array, dict, Callable], Array],
+               nn: Callable[[Array], Array],
                u:Callable[[Array, Array], Array],
                m:Callable[[PRNGKeyArray, Array, Array], Array], 
                s0:Array,
                T:int,
                N_simul:int,
                optimizer,
                opt_state
@@ -77,29 +82,32 @@
     ----------
     params: updated neutral network parameters
     opt_state: updated state of optimizer
     value: objective function value at previous step
     '''
     value, grads = jax.value_and_grad(lambda params: -jnp.mean(
         evaluate_policy(key = key, 
-                       policy = Partial(policy, params = params),
+                       policy = policy,
+                       params = params, 
+                        nn= nn,
                        u = u,
                        m = m,
                        s0 = s0,
                        T = T,
                        N_simul = N_simul)
         )
     )(params)
     updates, opt_state = optimizer.update(grads, opt_state)
     params = optax.apply_updates(params, updates)
     return params, opt_state, value
 
 def train(key:PRNGKeyArray,
           params:dict,
-          policy:Callable[[Array, Array], Array],
+          policy:Callable[[Array, dict, Callable], Array],
+          nn: Callable[[Array], Array],
           u:Callable[[Array, Array], Array],
           m:Callable[[PRNGKeyArray, Array, Array], Array], 
           F:Callable[[Array, Array], Array],
           T:int,
           N_simul:int,
           batch_size:int,
           N_iter:int,
@@ -131,14 +139,15 @@
     for i in range(N_iter):
         key, subkey = jax.random.split(key)
         s0 = F(key = subkey, N = batch_size)
         key, subkey = jax.random.split(key)
         params, opt_state, value = train_step(key = subkey, 
                                               params = params, 
                                               policy = policy, 
+                                              nn = nn,
                                               u = u, 
                                               m = m, 
                                               s0 = s0, 
                                               T = T, 
                                               N_simul = N_simul, 
                                               optimizer = optimizer, 
                                               opt_state = opt_state)
```

### Comparing `nndp-0.0.9/src/nndp.egg-info/PKG-INFO` & `nndp-0.1.0/src/nndp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nndp
-Version: 0.0.9
+Version: 0.1.0
 Summary: Dynamic Programming using Neural Networks
 Author-email: Marc de la Barrera <marc.delabarrera@gmail.com>, Tim de Silva <tdesilva@mit.edu>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

