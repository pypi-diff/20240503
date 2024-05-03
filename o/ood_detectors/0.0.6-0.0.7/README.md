# Comparing `tmp/ood_detectors-0.0.6.tar.gz` & `tmp/ood_detectors-0.0.7.tar.gz`

## Comparing `ood_detectors-0.0.6.tar` & `ood_detectors-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/docki.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/requirements.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/requirements_dev.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/ema.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/eval_utils.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/likelihood.py
--rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/losses.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/models.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/ood_utils.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/ops_utils.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/plot_utils.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/residual.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/sde.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/train.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/tests/init_test.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/LICENSE
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/README.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/docki.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/requirements_dev.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/ema.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/eval_utils.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/likelihood.py
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/losses.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/models.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/ood_utils.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/ops_utils.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/plot_utils.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/residual.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/sde.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/train.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/tests/init_test.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/README.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/PKG-INFO
```

### Comparing `ood_detectors-0.0.6/docki.yaml` & `ood_detectors-0.0.7/docki.yaml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/.github/workflows/publish.yml` & `ood_detectors-0.0.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/ema.py` & `ood_detectors-0.0.7/src/ood_detectors/ema.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/eval_utils.py` & `ood_detectors-0.0.7/src/ood_detectors/eval_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/likelihood.py` & `ood_detectors-0.0.7/src/ood_detectors/likelihood.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/losses.py` & `ood_detectors-0.0.7/src/ood_detectors/losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -186,22 +186,20 @@
                     self.ema.copy_to(model.parameters())
                 loss = self.loss_fn(model, x)
                 if self.ema is not None:
                     self.ema.restore(model.parameters())
         return loss
 
 
-class SDE_EMA_LRS_BF16_GradClip:
+class SDE_LRS_BF16:
     def __init__(
         self,
         sde,
         model,
         optimizer,
-        ema_rate=0.999,
-        grad_clip=1,
         total_steps=100000,
         reduce_mean=True,
         continuous=True,
         likelihood_weighting=False,
     ):
         """Create a one-step training/evaluation class.
         """
@@ -222,51 +220,32 @@
                 self.loss_fn = get_ddpm_loss_fn(sde, reduce_mean=reduce_mean)
             else:
                 raise ValueError(
                     f"Discrete training for {sde.__class__.__name__} is not recommended."
                 )
 
         self.optimizer = optimizer
-        self.ema = ema.ExponentialMovingAverage(model.parameters(), decay=ema_rate)
-        self.step = 0
-        self.grad_clip = grad_clip
         self.lr = optimizer.param_groups[0]["lr"]
         self.scaler = torch.cuda.amp.GradScaler()
         self.total_steps = total_steps
         self.lrs = torch.optim.lr_scheduler.OneCycleLR(
             self.optimizer,
             max_lr=self.lr,
             total_steps=self.total_steps,
         )
 
-    def __call__(self, model, x, train=True):
+    def __call__(self, model, x, *args, **kwargs):
         """Running one step of training or evaluation.
         Returns:
         loss: The average loss value of this state.
         """
 
-        if train:
-            self.optimizer.zero_grad()
-            with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                loss = self.loss_fn(model, x)
-            self.scaler.scale(loss).backward()
-            if self.grad_clip >= 0:
-                self.scaler.unscale_(self.optimizer)
-                torch.nn.utils.clip_grad_norm_(
-                    model.parameters(), max_norm=self.grad_clip
-                )
-            self.scaler.step(self.optimizer)
-            self.scaler.update()
-            self.lrs.step()
-            self.step += 1
-            if self.ema is not None:
-                self.ema.update(model.parameters())
-        else:
-            with torch.no_grad():
-                if self.ema is not None:
-                    self.ema.store(model.parameters())
-                    self.ema.copy_to(model.parameters())
-                with torch.cuda.amp.autocast(dtype=torch.bfloat16):
-                    loss = self.loss_fn(model, x)
-                if self.ema is not None:
-                    self.ema.restore(model.parameters())
+        self.optimizer.zero_grad()
+        with torch.cuda.amp.autocast(dtype=torch.bfloat16):
+            loss = self.loss_fn(model, x)
+        self.scaler.scale(loss).backward()
+        self.scaler.step(self.optimizer)
+        self.scaler.update()
+        self.lrs.step()
+
+
         return loss
```

### Comparing `ood_detectors-0.0.6/src/ood_detectors/models.py` & `ood_detectors-0.0.7/src/ood_detectors/models.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/ood_utils.py` & `ood_detectors-0.0.7/src/ood_detectors/ood_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/ops_utils.py` & `ood_detectors-0.0.7/src/ood_detectors/ops_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/plot_utils.py` & `ood_detectors-0.0.7/src/ood_detectors/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/residual.py` & `ood_detectors-0.0.7/src/ood_detectors/residual.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/sde.py` & `ood_detectors-0.0.7/src/ood_detectors/sde.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/src/ood_detectors/train.py` & `ood_detectors-0.0.7/src/ood_detectors/train.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/LICENSE` & `ood_detectors-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/README.md` & `ood_detectors-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 ood_detector = likelihood.Likelihood(
     sde = sde,
     model = model,
     optimizer = optimizer,
     ).to(device)
 
 update_fn = functools.partial(
-    losses.SDE_EMA_LRS_BF16_GradClip, 
+    losses.SDE_EMA_Warmup_GradClip, 
     ema_rate=ema_rate,
-    total_steps=(len(train_blob['data'])//batch_size) * n_epochs,
+    warmup=warmup,
     grad_clip=grad_clip,
     continuous=continuous,
     reduce_mean=reduce_mean,
     likelihood_weighting=likelihood_weighting,
     )
 
 train_loss = ood_detector.fit(train_data, update_fn, batch_size)
```

### Comparing `ood_detectors-0.0.6/pyproject.toml` & `ood_detectors-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.6/PKG-INFO` & `ood_detectors-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ood_detectors
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: Documentation, https://github.com/Arty-Facts/ood_detectors#readme
 Project-URL: Issues, https://github.com/Arty-Facts/ood_detectors/issues
 Project-URL: Source, https://github.com/Arty-Facts/ood_detectors
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>, Yifan Ding <yifan.ding@liu.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -112,17 +112,17 @@
 ood_detector = likelihood.Likelihood(
     sde = sde,
     model = model,
     optimizer = optimizer,
     ).to(device)
 
 update_fn = functools.partial(
-    losses.SDE_EMA_LRS_BF16_GradClip, 
+    losses.SDE_EMA_Warmup_GradClip, 
     ema_rate=ema_rate,
-    total_steps=(len(train_blob['data'])//batch_size) * n_epochs,
+    warmup=warmup,
     grad_clip=grad_clip,
     continuous=continuous,
     reduce_mean=reduce_mean,
     likelihood_weighting=likelihood_weighting,
     )
 
 train_loss = ood_detector.fit(train_data, update_fn, batch_size)
```

