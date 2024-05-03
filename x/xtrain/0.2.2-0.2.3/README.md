# Comparing `tmp/xtrain-0.2.2.tar.gz` & `tmp/xtrain-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.2.2.tar", max compression
+gzip compressed data, was "xtrain-0.2.3.tar", max compression
```

## Comparing `xtrain-0.2.2.tar` & `xtrain-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-04-23 13:38:19.629050 xtrain-0.2.2/LICENSE
--rw-r--r--   0        0        0     1231 2024-04-23 13:38:19.629050 xtrain-0.2.2/README.md
--rw-r--r--   0        0        0      833 2024-04-23 13:38:39.005170 xtrain-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      160 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/__init__.py
--rw-r--r--   0        0        0    10925 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/base_trainer.py
--rw-r--r--   0        0        0     1464 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/loss.py
--rw-r--r--   0        0        0     4564 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/strategy.py
--rw-r--r--   0        0        0     5517 2024-04-23 13:38:19.629050 xtrain-0.2.2/xtrain/utils.py
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-03 20:13:02.317288 xtrain-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1231 2024-05-03 20:13:02.317288 xtrain-0.2.3/README.md
+-rw-r--r--   0        0        0      833 2024-05-03 20:13:18.473312 xtrain-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/__init__.py
+-rw-r--r--   0        0        0    11115 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     3986 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/closure.py
+-rw-r--r--   0        0        0     1631 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/loss.py
+-rw-r--r--   0        0        0     4564 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/strategy.py
+-rw-r--r--   0        0        0     5517 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/utils.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.3/PKG-INFO
```

### Comparing `xtrain-0.2.2/LICENSE` & `xtrain-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.2/README.md` & `xtrain-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.2/pyproject.toml` & `xtrain-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtrain"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Flax trainer"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flax = "^0.8"
```

### Comparing `xtrain-0.2.2/xtrain/base_trainer.py` & `xtrain-0.2.3/xtrain/base_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,18 @@
     def loss(self):
         return self._compute_loss_log()
 
     @property
     def has_aux(self):
         return self.ctx.mutable or self.ctx.capture_intermediates
 
+    def __iter__(self):
+        self.data = Peekable(iter(self.ctx.dataset))
+        return self
+
     def _compute_loss_log(self) -> dict:
         return {
             _get_name(loss_log.loss_fn): loss_log.compute()
             for loss_log in self.loss_logs
         }
 
     def reset(self):
@@ -203,14 +207,15 @@
         self,
         dataset: Iterable,
         *,
         strategy: type | None = None,
         rng_cols: Sequence[str] = ["dropout"],
         init_vars: dict | None = None,
         frozen: dict | None = None,
+        method: Union[Callable[..., Any], str, None] = None,
         **kwargs,
     ) -> TrainIterator:
         """Create the training iterator
 
         Args:
             dataset: An iterator or iterable to supply the training data.
                 The dataset should produce ```(inputs, labels, sample_weight)```, however
@@ -266,14 +271,15 @@
 
         params = init_vars.pop("params")
         train_state = TrainState.create(
             apply_fn=_cached_partial(
                 self.model.apply,
                 mutable=self.mutable,
                 capture_intermediates=self.capture_intermediates,
+                method=method,
                 **kwargs,
             ),
             params=params,
             tx=tx,
         )
 
         losses = self.losses
```

### Comparing `xtrain-0.2.2/xtrain/loss.py` & `xtrain-0.2.3/xtrain/loss.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Protocol, Sequence, Union, Any
 
 from functools import partial
 
 import jax.numpy as jnp
 from flax import struct
 
-from .utils import _get_name
+from .utils import _get_name, unpack_x_y_sample_weight
 
 class LossFunc_(Protocol):
     def __call__(self, batch: Any, prediction: Any) -> float:
         ...
 
 LossFunc = LossFunc_ | str
 
@@ -24,29 +24,32 @@
 
     def __post_init__(self):
         self.__name__ = _get_name(self.loss_fn)
 
     # update() is meant to be called in JAX transformation, where objects are immutable
     # so it returns a copy of self in order for the caller to track changes to the object.
     def update(self, batch, prediction):
+        _, _, sample_weight = unpack_x_y_sample_weight(batch)
+
         if isinstance(self.loss_fn, str):
             loss = prediction
             for k in self.loss_fn.split("/"):
                 loss = loss[k]
         else:
             loss = self.loss_fn(batch, prediction)
 
         if loss is None:
             return 0.0, self
 
-        loss *= self.weight
-        self.cnt += 1
-        self.sum += loss
+        if sample_weight is not None:
+            loss *= sample_weight
+        self.cnt += loss.size
+        self.sum += loss.sum()
 
-        return loss, self
+        return loss.sum() * self.weight, self
 
     def compute(self):
         if self.cnt == 0:
             return 0
         else:
             return self.sum / self.cnt
```

### Comparing `xtrain-0.2.2/xtrain/strategy.py` & `xtrain-0.2.3/xtrain/strategy.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.2/xtrain/utils.py` & `xtrain-0.2.3/xtrain/utils.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.2/PKG-INFO` & `xtrain-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

