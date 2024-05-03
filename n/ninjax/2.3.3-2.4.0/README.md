# Comparing `tmp/ninjax-2.3.3.tar.gz` & `tmp/ninjax-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjax-2.3.3.tar", last modified: Mon Feb  5 01:40:55 2024, max compression
+gzip compressed data, was "ninjax-2.4.0.tar", last modified: Fri May  3 01:12:06 2024, max compression
```

## Comparing `ninjax-2.3.3.tar` & `ninjax-2.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-05 01:40:55.914459 ninjax-2.3.3/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2023-11-19 22:35:43.000000 ninjax-2.3.3/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9589 2024-02-05 01:40:55.914459 ninjax-2.3.3/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9178 2023-11-29 00:44:38.000000 ninjax-2.3.3/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-05 01:40:55.910459 ninjax-2.3.3/ninjax/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      493 2023-12-04 20:45:03.000000 ninjax-2.3.3/ninjax/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    21315 2024-02-05 01:40:52.000000 ninjax-2.3.3/ninjax/ninjax.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-05 01:40:55.910459 ninjax-2.3.3/ninjax.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9589 2024-02-05 01:40:55.000000 ninjax-2.3.3/ninjax.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      394 2024-02-05 01:40:55.000000 ninjax-2.3.3/ninjax.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-02-05 01:40:55.000000 ninjax-2.3.3/ninjax.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        4 2024-02-05 01:40:55.000000 ninjax-2.3.3/ninjax.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2024-02-05 01:40:55.000000 ninjax-2.3.3/ninjax.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-02-05 01:40:55.914459 ninjax-2.3.3/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      800 2024-02-05 01:40:52.000000 ninjax-2.3.3/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-05 01:40:55.914459 ninjax-2.3.3/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1959 2023-11-26 03:13:56.000000 ninjax-2.3.3/tests/test_attrs.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1020 2023-12-05 21:38:21.000000 ninjax-2.3.3/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1138 2023-11-29 00:10:03.000000 ninjax-2.3.3/tests/test_cond.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3608 2023-12-05 21:36:48.000000 ninjax-2.3.3/tests/test_grad.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2428 2023-11-29 00:16:02.000000 ninjax-2.3.3/tests/test_init.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2528 2023-12-04 20:45:06.000000 ninjax-2.3.3/tests/test_jit.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1751 2023-11-29 00:28:06.000000 ninjax-2.3.3/tests/test_module.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1435 2023-12-05 21:04:09.000000 ninjax-2.3.3/tests/test_scan.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1278 2023-11-29 00:14:22.000000 ninjax-2.3.3/tests/test_variable.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.420701 ninjax-2.4.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2023-11-19 22:35:43.000000 ninjax-2.4.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9160 2024-05-03 01:12:06.420701 ninjax-2.4.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     8749 2024-05-03 01:12:04.000000 ninjax-2.4.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.408701 ninjax-2.4.0/ninjax/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      493 2023-12-04 20:45:03.000000 ninjax-2.4.0/ninjax/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    22614 2024-05-03 01:12:04.000000 ninjax-2.4.0/ninjax/ninjax.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.408701 ninjax-2.4.0/ninjax.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9160 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      394 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        4 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-03 01:12:06.420701 ninjax-2.4.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      800 2024-02-05 01:40:52.000000 ninjax-2.4.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.420701 ninjax-2.4.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1959 2023-11-26 03:13:56.000000 ninjax-2.4.0/tests/test_attrs.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1020 2023-12-05 21:38:21.000000 ninjax-2.4.0/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1138 2023-11-29 00:10:03.000000 ninjax-2.4.0/tests/test_cond.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3608 2023-12-05 21:36:48.000000 ninjax-2.4.0/tests/test_grad.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2428 2023-11-29 00:16:02.000000 ninjax-2.4.0/tests/test_init.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2528 2023-12-04 20:45:06.000000 ninjax-2.4.0/tests/test_jit.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1751 2023-11-29 00:28:06.000000 ninjax-2.4.0/tests/test_module.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1435 2023-12-05 21:04:09.000000 ninjax-2.4.0/tests/test_scan.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1278 2023-11-29 00:14:22.000000 ninjax-2.4.0/tests/test_variable.py
```

### Comparing `ninjax-2.3.3/LICENSE` & `ninjax-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/PKG-INFO` & `ninjax-2.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,43 @@
-Metadata-Version: 2.1
-Name: ninjax
-Version: 2.3.3
-Summary: Flexible Modules for JAX
-Home-page: http://github.com/danijar/ninjax
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI](https://img.shields.io/pypi/v/ninjax.svg)](https://pypi.python.org/pypi/ninjax/#history)
 
 # 🥷  Ninjax: Flexible Modules for JAX
 
-Ninjax is a general module system for [JAX][jax]. It gives the user complete
-and transparent control over updating the state of each module, bringing the
-flexibility of PyTorch and TensorFlow to JAX. Moreover, Ninjax makes it easy to
-mix and match modules from different libraries, such as [Flax][flax] and
-[Haiku][flax].
+Ninjax is a general and practical module system for [JAX][jax]. It gives users
+full and transparent control over updating the state of each module, bringing
+flexibility to JAX and enabling new use cases.
+
+## Overview
+
+Ninjax provides a simple and general `nj.Module` class.
+
+- Modules can store state for things like model parameters, Adam momentum
+  buffer, BatchNorm statistics, recurrent state, etc.
+
+- Modules can read and write their state entries. For example, this allows
+  modules to have train methods, because they can update their parameters from
+  the inside.
+
+- Any method can initialize, read, and write state entries. This avoids the
+  need for a special `build()` method or `@compact` decorator used in Flax.
+
+- Ninjax makes it easy to mix and match modules from different libraries, such
+  as [Flax][flax] and [Haiku][flax].
+
+- Instead of PyTrees, Ninjax state is a flat `dict` that maps
+  string keys like `/net/layer1/weights` to `jnp.array`s. This makes it easy
+  to iterate over, modify, and save or load state.
+
+- Modules can specify typed hyperparameters using the [dataclass][dataclass]
+  syntax.
 
 [jax]: https://github.com/google/jax
 [flax]: https://github.com/google/flax
 [haiku]: https://github.com/deepmind/dm-haiku
-
-## Motivation
-
-Existing deep learning libraries for JAX provide modules, but those modules
-only specify neural networks and cannot easily implement training logic.
-Orchestrating training all in one place, outside of the modules, is fine for
-simple code bases. But it becomes a problem when there are many modules with
-their own training logic and optimizers.
-
-Ninjax solves this problem by giving each `nj.Module` full read and write
-access to its state. This means modules can have train functions to
-implement custom training logic, and call each other's train functions. Ninjax
-is intended to be used with one or more neural network libraries, such as
-[Haiku][haiku] and [Flax][flax].
-
-The main differences to existing deep learning libraries are:
-
-- Ninjax does not need separate `apply()`/`init()` functions. Instead, the
-  first function call creates variables automatically.
-- Ninjax lets you access and update model parameters inside of impure
-  functions, so modules can handle their own optimizers and update logic.
-- Natural support for modules with multiple functions without need for
-  Flax's `setup()` function or Haiku's `hk.multi_transform()`.
-- Ninjax' flexible state handling makes it trivial to mix and match
-  modules from other deep learning libraries in your models.
+[dataclass]: https://docs.python.org/3/library/dataclasses.html
 
 ## Installation
 
 Ninjax is [a single file][file], so you can just copy it to your project
 directory. Or you can install the package:
 
 ```
@@ -150,26 +136,26 @@
     print(self.getm())  # {'/path/to/module/weights': ..., '/path/to/module/bias': ...}
     return x @ weights + bias
 ```
 
 ### How can I update state entries?
 
 To update the state entries of a module, use `self.put(name, value)` for
-individual entries of `self.putm(mapping)` to update multiple values:
+individual entries of `self.put(mapping)` to update multiple values:
 
 ```python3
 class Module(nj.Module):
 
   def counting(self):
     counter = nj.get('counter', jnp.zeros, (), jnp.int32)
     self.put('counter', counter + 1)
     print(self.get('counter'))  # 1
     state = self.getm()
     state['counter'] += 1
-    self.putm(state)
+    self.put(state)
     print(self.getm()['counter'])  # 2
     print(self.get('counter'))  # 2
 ```
 
 ### How can I use JIT compilation?
 
 The `nj.pure()` function makes the state your JAX code uses explicit, so it can
```

### Comparing `ninjax-2.3.3/README.md` & `ninjax-2.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,55 @@
+Metadata-Version: 2.1
+Name: ninjax
+Version: 2.4.0
+Summary: Flexible Modules for JAX
+Home-page: http://github.com/danijar/ninjax
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI](https://img.shields.io/pypi/v/ninjax.svg)](https://pypi.python.org/pypi/ninjax/#history)
 
 # 🥷  Ninjax: Flexible Modules for JAX
 
-Ninjax is a general module system for [JAX][jax]. It gives the user complete
-and transparent control over updating the state of each module, bringing the
-flexibility of PyTorch and TensorFlow to JAX. Moreover, Ninjax makes it easy to
-mix and match modules from different libraries, such as [Flax][flax] and
-[Haiku][flax].
+Ninjax is a general and practical module system for [JAX][jax]. It gives users
+full and transparent control over updating the state of each module, bringing
+flexibility to JAX and enabling new use cases.
+
+## Overview
+
+Ninjax provides a simple and general `nj.Module` class.
+
+- Modules can store state for things like model parameters, Adam momentum
+  buffer, BatchNorm statistics, recurrent state, etc.
+
+- Modules can read and write their state entries. For example, this allows
+  modules to have train methods, because they can update their parameters from
+  the inside.
+
+- Any method can initialize, read, and write state entries. This avoids the
+  need for a special `build()` method or `@compact` decorator used in Flax.
+
+- Ninjax makes it easy to mix and match modules from different libraries, such
+  as [Flax][flax] and [Haiku][flax].
+
+- Instead of PyTrees, Ninjax state is a flat `dict` that maps
+  string keys like `/net/layer1/weights` to `jnp.array`s. This makes it easy
+  to iterate over, modify, and save or load state.
+
+- Modules can specify typed hyperparameters using the [dataclass][dataclass]
+  syntax.
 
 [jax]: https://github.com/google/jax
 [flax]: https://github.com/google/flax
 [haiku]: https://github.com/deepmind/dm-haiku
-
-## Motivation
-
-Existing deep learning libraries for JAX provide modules, but those modules
-only specify neural networks and cannot easily implement training logic.
-Orchestrating training all in one place, outside of the modules, is fine for
-simple code bases. But it becomes a problem when there are many modules with
-their own training logic and optimizers.
-
-Ninjax solves this problem by giving each `nj.Module` full read and write
-access to its state. This means modules can have train functions to
-implement custom training logic, and call each other's train functions. Ninjax
-is intended to be used with one or more neural network libraries, such as
-[Haiku][haiku] and [Flax][flax].
-
-The main differences to existing deep learning libraries are:
-
-- Ninjax does not need separate `apply()`/`init()` functions. Instead, the
-  first function call creates variables automatically.
-- Ninjax lets you access and update model parameters inside of impure
-  functions, so modules can handle their own optimizers and update logic.
-- Natural support for modules with multiple functions without need for
-  Flax's `setup()` function or Haiku's `hk.multi_transform()`.
-- Ninjax' flexible state handling makes it trivial to mix and match
-  modules from other deep learning libraries in your models.
+[dataclass]: https://docs.python.org/3/library/dataclasses.html
 
 ## Installation
 
 Ninjax is [a single file][file], so you can just copy it to your project
 directory. Or you can install the package:
 
 ```
@@ -138,26 +148,26 @@
     print(self.getm())  # {'/path/to/module/weights': ..., '/path/to/module/bias': ...}
     return x @ weights + bias
 ```
 
 ### How can I update state entries?
 
 To update the state entries of a module, use `self.put(name, value)` for
-individual entries of `self.putm(mapping)` to update multiple values:
+individual entries of `self.put(mapping)` to update multiple values:
 
 ```python3
 class Module(nj.Module):
 
   def counting(self):
     counter = nj.get('counter', jnp.zeros, (), jnp.int32)
     self.put('counter', counter + 1)
     print(self.get('counter'))  # 1
     state = self.getm()
     state['counter'] += 1
-    self.putm(state)
+    self.put(state)
     print(self.getm()['counter'])  # 2
     print(self.get('counter'))  # 2
 ```
 
 ### How can I use JIT compilation?
 
 The `nj.pure()` function makes the state your JAX code uses explicit, so it can
```

### Comparing `ninjax-2.3.3/ninjax/ninjax.py` & `ninjax-2.4.0/ninjax/ninjax.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import inspect
 import re
 import threading
 
 import jax
 import jax.numpy as jnp
 
-__version__ = '2.3.3'
+__version__ = '2.4.0'
 
 
 ###############################################################################
 # State
 ###############################################################################
 
 
@@ -200,15 +200,15 @@
 def grad(fun, keys, has_aux=False):
   """Compute the gradient of an impure function with respect to the specified
   state entries or modules. The transformed function returns a tuple containing
   the computed value, selected state entries, their gradients, and if
   applicable auxiliary outputs of the function."""
   keys = keys if hasattr(keys, '__len__') else (keys,)
   if not has_aux:
-    fun = lambda *args, _fun=fun, **kwargs: (_fun(*args, *kwargs), {})
+    fun = lambda *args, _fun=fun, **kwargs: (_fun(*args, **kwargs), {})
   fun = pure(fun, nested=True)
 
   def wrapper(*args, **kwargs):
     accessed, modified = _prerun(fun, *args, **kwargs)
 
     strs = []
     for key in keys:
@@ -504,40 +504,43 @@
       # Look up the value again to make sure we are registering it as an
       # accessed key in the context.
       return context()[path]
     else:
       self._submodules[name] = value
       return value
 
-  def put(self, *args):
+  def put(self, *args, prefix=False):
     """Update or create state entries that belong to this module. The arguments
     are either string name and value of a single state entry or a dict holding
     multiple state entries."""
     if len(args) == 2:
       name, value = args
       self.put({self.path + '/' + name: value})
       return value
     assert len(args) == 1 and isinstance(args[0], dict)
     mapping = args[0]
-    prefix = self.path + '/'
+    if prefix:
+      mapping = {f'{self.path}/{k}': v for k, v in mapping.items()}
+    start = self.path + '/'
     for key in mapping:
-      if not key.startswith(prefix):
+      if not key.startswith(start):
         raise KeyError(f'Key {key} does not belong to module {self.path}.')
     context().update(mapping)
 
   def find(self, pattern=r'.*', empty_ok=False):
     """Find the state entries of this module, optionally filtered by regex."""
     pattern = re.compile(pattern)
     prefix = self.path + '/'
     results = {}
-    for key, value in context().items():
+    ctx = context()
+    for key in ctx.keys():
       if not key.startswith(prefix):
         continue
       if pattern.match(key[len(prefix):]):
-        results[key] = value
+        results[key] = ctx[key]
     if not empty_ok and not results:
       raise KeyError(f'Pattern {pattern} matched no state keys.')
     return results
 
 
 class Variable(Module):
 
@@ -554,45 +557,91 @@
 
 
 ###############################################################################
 # Integrations
 ###############################################################################
 
 
+def flatten(tree):
+  items, treedef = jax.tree_util.tree_flatten_with_path(tree)
+  paths, values = zip(*items)
+  tostr = lambda x: re.sub(
+      r'[^a-z0-9-_/]+', '_', str(x).lower()).strip('_').replace('/_/', '')
+  strpaths = [[tostr(x) for x in path] for path in paths]
+  keys = ['/'.join(x for x in strpath if x) for strpath in strpaths]
+  if len(set(keys)) < len(keys):
+    raise ValueError(
+        'Cannot flatten PyTree to dict because paths are ambiguous '
+        'after converting them to string keys.\n'
+        'Paths: {paths}\nKeys: {keys}')
+  items = sorted(list(zip(keys, values)), key=lambda x: x[0])
+  return dict(items), treedef
+
+
+def unflatten(mapping, treedef):
+  items = sorted(list(mapping.items()), key=lambda x: x[0])
+  _, values = zip(*items)
+  return jax.tree.unflatten(treedef, values)
+
+
 def FromFlax(ctor):
+
   class FlaxModule(Module):
+
     def __init__(self, *args, **kwargs):
       self.module = ctor(*args, **kwargs)
+      self.treedef = None
+
     def __call__(self, *args, **kwargs):
-      seed_ = seed() if creating() else None
-      state = self.get('flax', self.module.init, seed_, *args, **kwargs)
+      if creating():
+        state, self.treedef = flatten(
+            self.module.init(seed(), *args, **kwargs))
+        self.put(state, prefix=True)
+      state = unflatten(self.find(), self.treedef)
       return self.module.apply(state, *args, **kwargs)
+
   return FlaxModule
 
 
 def FromHaiku(ctor):
+
   class HaikuModule(Module):
+
     def __init__(self, *args, **kwargs):
       import haiku as hk
       def net(*args_, **kwargs_):
         return ctor(*args, **kwargs)(*args_, **kwargs_)
       self.transformed = hk.transform(net)
+      self.treedef = None
+
     def __call__(self, *args, **kwargs):
-      seed_ = seed() if creating() else None
-      state = self.get('haiku', self.transformed.init, seed_, *args, **kwargs)
-      return self.transformed.apply(state, seed_, *args, **kwargs)
+      if creating():
+        state, self.treedef = flatten(
+            self.transformed.init(seed(), *args, **kwargs))
+        self.put(state, prefix=True)
+      state = unflatten(self.find(), self.treedef)
+      return self.transformed.apply(state, seed(), *args, **kwargs)
+
   return HaikuModule
 
 
 def FromOptax(ctor):
+
   class OptaxModule(Module):
+
     def __init__(self, *args, **kwargs):
       self.opt = ctor(*args, **kwargs)
+      self.treedef = None
+
     def __call__(self, loss, keys, *args, **kwargs):
       import optax
       loss, params, grads = grad(loss, keys)(*args, **kwargs)
-      optstate = self.get('state', self.opt.init, params)
-      updates, optstate = self.opt.update(grads, optstate)
-      self.put('state', optstate)
+      if creating():
+        state, self.treedef = flatten(self.opt.init(params))
+        self.put(state, prefix=True)
+      state = unflatten(self.find(), self.treedef)
+      updates, state = self.opt.update(grads, state)
+      self.put(flatten(state)[0], prefix=True)
       context().update(optax.apply_updates(params, updates))
       return loss, params, grads
+
   return OptaxModule
```

### Comparing `ninjax-2.3.3/ninjax.egg-info/PKG-INFO` & `ninjax-2.4.0/ninjax.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 2.3.3
+Version: 2.4.0
 Summary: Flexible Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/ninjax.svg)](https://pypi.python.org/pypi/ninjax/#history)
 
 # 🥷  Ninjax: Flexible Modules for JAX
 
-Ninjax is a general module system for [JAX][jax]. It gives the user complete
-and transparent control over updating the state of each module, bringing the
-flexibility of PyTorch and TensorFlow to JAX. Moreover, Ninjax makes it easy to
-mix and match modules from different libraries, such as [Flax][flax] and
-[Haiku][flax].
+Ninjax is a general and practical module system for [JAX][jax]. It gives users
+full and transparent control over updating the state of each module, bringing
+flexibility to JAX and enabling new use cases.
+
+## Overview
+
+Ninjax provides a simple and general `nj.Module` class.
+
+- Modules can store state for things like model parameters, Adam momentum
+  buffer, BatchNorm statistics, recurrent state, etc.
+
+- Modules can read and write their state entries. For example, this allows
+  modules to have train methods, because they can update their parameters from
+  the inside.
+
+- Any method can initialize, read, and write state entries. This avoids the
+  need for a special `build()` method or `@compact` decorator used in Flax.
+
+- Ninjax makes it easy to mix and match modules from different libraries, such
+  as [Flax][flax] and [Haiku][flax].
+
+- Instead of PyTrees, Ninjax state is a flat `dict` that maps
+  string keys like `/net/layer1/weights` to `jnp.array`s. This makes it easy
+  to iterate over, modify, and save or load state.
+
+- Modules can specify typed hyperparameters using the [dataclass][dataclass]
+  syntax.
 
 [jax]: https://github.com/google/jax
 [flax]: https://github.com/google/flax
 [haiku]: https://github.com/deepmind/dm-haiku
-
-## Motivation
-
-Existing deep learning libraries for JAX provide modules, but those modules
-only specify neural networks and cannot easily implement training logic.
-Orchestrating training all in one place, outside of the modules, is fine for
-simple code bases. But it becomes a problem when there are many modules with
-their own training logic and optimizers.
-
-Ninjax solves this problem by giving each `nj.Module` full read and write
-access to its state. This means modules can have train functions to
-implement custom training logic, and call each other's train functions. Ninjax
-is intended to be used with one or more neural network libraries, such as
-[Haiku][haiku] and [Flax][flax].
-
-The main differences to existing deep learning libraries are:
-
-- Ninjax does not need separate `apply()`/`init()` functions. Instead, the
-  first function call creates variables automatically.
-- Ninjax lets you access and update model parameters inside of impure
-  functions, so modules can handle their own optimizers and update logic.
-- Natural support for modules with multiple functions without need for
-  Flax's `setup()` function or Haiku's `hk.multi_transform()`.
-- Ninjax' flexible state handling makes it trivial to mix and match
-  modules from other deep learning libraries in your models.
+[dataclass]: https://docs.python.org/3/library/dataclasses.html
 
 ## Installation
 
 Ninjax is [a single file][file], so you can just copy it to your project
 directory. Or you can install the package:
 
 ```
@@ -150,26 +148,26 @@
     print(self.getm())  # {'/path/to/module/weights': ..., '/path/to/module/bias': ...}
     return x @ weights + bias
 ```
 
 ### How can I update state entries?
 
 To update the state entries of a module, use `self.put(name, value)` for
-individual entries of `self.putm(mapping)` to update multiple values:
+individual entries of `self.put(mapping)` to update multiple values:
 
 ```python3
 class Module(nj.Module):
 
   def counting(self):
     counter = nj.get('counter', jnp.zeros, (), jnp.int32)
     self.put('counter', counter + 1)
     print(self.get('counter'))  # 1
     state = self.getm()
     state['counter'] += 1
-    self.putm(state)
+    self.put(state)
     print(self.getm()['counter'])  # 2
     print(self.get('counter'))  # 2
 ```
 
 ### How can I use JIT compilation?
 
 The `nj.pure()` function makes the state your JAX code uses explicit, so it can
```

### Comparing `ninjax-2.3.3/setup.py` & `ninjax-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_attrs.py` & `ninjax-2.4.0/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_checkpoint.py` & `ninjax-2.4.0/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_cond.py` & `ninjax-2.4.0/tests/test_cond.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_grad.py` & `ninjax-2.4.0/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_init.py` & `ninjax-2.4.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_jit.py` & `ninjax-2.4.0/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_module.py` & `ninjax-2.4.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_scan.py` & `ninjax-2.4.0/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.3.3/tests/test_variable.py` & `ninjax-2.4.0/tests/test_variable.py`

 * *Files identical despite different names*

