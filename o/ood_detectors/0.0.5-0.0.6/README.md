# Comparing `tmp/ood_detectors-0.0.5.tar.gz` & `tmp/ood_detectors-0.0.6.tar.gz`

## Comparing `ood_detectors-0.0.5.tar` & `ood_detectors-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/docki.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/requirements.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/requirements_dev.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/__init__.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/ddm_likelihood.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/eval_utils.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/losses.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/ood_utils.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/ops_utils.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/plot_utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/residual.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/train.py
--rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/src/ood_detectors/models/mlp.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/tests/init_test.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/LICENSE
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/README.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 ood_detectors-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/docki.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/requirements_dev.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/ema.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/eval_utils.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/likelihood.py
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/losses.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/models.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/ood_utils.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/ops_utils.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/plot_utils.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/residual.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/sde.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/src/ood_detectors/train.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/tests/init_test.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/README.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 ood_detectors-0.0.6/PKG-INFO
```

### Comparing `ood_detectors-0.0.5/docki.yaml` & `ood_detectors-0.0.6/docki.yaml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.5/.github/workflows/publish.yml` & `ood_detectors-0.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.5/src/ood_detectors/ops_utils.py` & `ood_detectors-0.0.6/src/ood_detectors/ops_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,27 @@
         self.id = id
         self.node = node
         self.process = dummy
         self.start_time = time.perf_counter()
 
 
 def parallelize(func, jobs, gpu_nodes, verbose=True, timeout=3600):
+    """
+    Parallelize the execution of a function on multiple GPUs.
+
+    Args:
+        func (function): The function to be executed in parallel.
+        jobs (list): A list of jobs to be executed by the function.
+        gpu_nodes (list): A list of GPU nodes to be used for execution.
+        verbose (bool, optional): Whether to print verbose output. Defaults to True.
+        timeout (int, optional): Timeout in seconds for each job. Defaults to 3600.
+
+    Returns:
+        None
+    """
     if verbose:
         print(f'Launching {len(jobs)} jobs on {len(set(gpu_nodes))} GPUs. {len(gpu_nodes)//len(set(gpu_nodes))} jobs per GPU in parallel..')
     workers = [Worker(id, node) for id, node in enumerate(gpu_nodes)]
     while len(jobs) > 0:
         random.shuffle(workers)
         for worker in workers:
             if time.perf_counter() - worker.start_time > timeout:
```

### Comparing `ood_detectors-0.0.5/src/ood_detectors/plot_utils.py` & `ood_detectors-0.0.6/src/ood_detectors/plot_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
     sns.kdeplot(data=score_ref, bw_adjust=.2, ax=axs[0, 0], label=f'{id_name} validation: {np.mean(score_ref):.2f}')
     add_shadow(axs[0, 0], score_ref)
 
     for ood_name, score_ood in zip(ood_names, score_oods):
         sns.kdeplot(data=score_ood, bw_adjust=.2, ax=axs[0, 0], label=f'{ood_name}: {np.mean(score_ood):.2f}')
         add_shadow(axs[0, 0], score_ood)
-    axs[0, 0].xaxis.set_major_locator(ticker.MultipleLocator(base=0.5))
-    axs[0, 0].xaxis.set_minor_locator(ticker.MultipleLocator(base=0.1))
+    # axs[0, 0].xaxis.set_major_locator(ticker.MultipleLocator(base=0.5))
+    # axs[0, 0].xaxis.set_minor_locator(ticker.MultipleLocator(base=0.1))
     axs[0, 0].set_title('Density Plots')
     axs[0, 0].set_xlabel('bits/dim')
     axs[0, 0].set_ylabel('Density')
     # axs[0, 0].set_xlim(6.5, 8)
     # axs[0, 0].grid(True)
     axs[0, 0].legend()
```

### Comparing `ood_detectors-0.0.5/src/ood_detectors/models/mlp.py` & `ood_detectors-0.0.6/src/ood_detectors/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def timestep_embedding(timesteps, dim, max_period=10000, repeat_only=False):
     """
     Create sinusoidal timestep embeddings.
     :param timesteps: a 1-D Tensor of N indices, one per batch element.
                       These may be fractional.
     :param dim: the dimension of the output.
     :param max_period: controls the minimum frequency of the embeddings.
+    :param repeat_only: if True, only repeat the timesteps without embedding.
     :return: an [N x dim] Tensor of positional embeddings.
     """
     if not repeat_only:
         half = dim // 2
         freqs = torch.exp(
             -math.log(max_period) * torch.arange(start=0, end=half, dtype=torch.float32) / half
         ).to(device=timesteps.device)
@@ -26,28 +27,31 @@
         embedding = repeat(timesteps, 'b -> b d', d=dim)
     return embedding
 
 
 def zero_module(module):
     """
     Zero out the parameters of a module and return it.
+    :param module: the module to zero out.
+    :return: the zeroed module.
     """
     for p in module.parameters():
         p.detach().zero_()
     return module
 
 
-
 class ResBlock(nn.Module):
     """
     A residual block that can optionally change the number of channels.
     :param channels: the number of input channels.
     :param mid_channels: the number of middle channels.
     :param emb_channels: the number of timestep embedding channels.
     :param dropout: the rate of dropout.
+    :param use_context: if True, use context conditioning.
+    :param context_channels: the number of context channels.
     """
 
     def __init__(
         self,
         channels,
         mid_channels,
         emb_channels,
@@ -79,102 +83,104 @@
                 nn.Linear(mid_channels, channels, bias=True)
             ),
         )
 
         self.use_context = use_context
         if use_context:
             self.context_layers = nn.Sequential(
-            nn.SiLU(),
-            nn.Linear(context_channels, mid_channels, bias=True),
-        )
+                nn.SiLU(),
+                nn.Linear(context_channels, mid_channels, bias=True),
+            )
 
     def forward(self, x, emb, context):
+        """
+        Forward pass of the residual block.
+        :param x: the input tensor.
+        :param emb: the timestep embedding tensor.
+        :param context: the context tensor.
+        :return: the output tensor.
+        """
         h = self.in_layers(x)
         emb_out = self.emb_layers(emb)
         if self.use_context:
             context_out = self.context_layers(context)
             h = h + emb_out + context_out
         else:
             h = h + emb_out
         h = self.out_layers(h)
         return x + h
 
 
 class SimpleMLP(nn.Module):
     """
     The full skip network with timestep embedding.
-    :param in_channels: channels in the input Tensor.
-    :param model_channels: base channel count for the model.
-    :param out_channels: channels in the output Tensor.
+    :param channels: channels in the input Tensor.
+    :param time_embed_dim: dimension of the timestep embedding.
+    :param bottleneck_channels: base channel count for the model.
     :param num_res_blocks: number of residual blocks per downsample.
+    :param dropout: the rate of dropout.
+    :param use_context: if True, use context conditioning.
+    :param context_channels: the number of context channels.
     """
 
     def __init__(
         self,
-        marginal_prob_std,
-        in_channels,
-        time_embed_dim,
-        model_channels,
-        bottleneck_channels,
-        out_channels,
-        num_res_blocks,
+        channels,
+        time_embed_dim=256,
+        bottleneck_channels=1536,
+        num_res_blocks=13,
         dropout=0,
         use_context=False,
         context_channels=512
     ):
         super().__init__()
 
         self.image_size = 1
-        self.in_channels = in_channels
-        self.model_channels = model_channels
-        self.out_channels = out_channels
+        self.channels = channels
         self.num_res_blocks = num_res_blocks
         self.dropout = dropout
-        self.marginal_prob_std = marginal_prob_std
 
         self.time_embed = nn.Sequential(
-            nn.Linear(model_channels, time_embed_dim),
+            nn.Linear(channels, time_embed_dim),
             nn.SiLU(),
             nn.Linear(time_embed_dim, time_embed_dim),
         )
 
-        self.input_proj = nn.Linear(in_channels, model_channels)
+        self.input_proj = nn.Linear(channels, channels)
 
         res_blocks = []
         for i in range(num_res_blocks):
             res_blocks.append(ResBlock(
-                model_channels,
+                channels,
                 bottleneck_channels,
                 time_embed_dim,
                 dropout,
                 use_context=use_context,
                 context_channels=context_channels
             ))
 
         self.res_blocks = nn.ModuleList(res_blocks)
 
         self.out = nn.Sequential(
-            nn.LayerNorm(model_channels, eps=1e-6),
+            nn.LayerNorm(channels, eps=1e-6),
             nn.SiLU(),
-            zero_module(nn.Linear(model_channels, out_channels, bias=True)),
+            zero_module(nn.Linear(channels, channels, bias=True)),
         )
 
     def forward(self, x, timesteps=None, context=None, y=None, **kwargs):
         """
         Apply the model to an input batch.
         :param x: an [N x C x ...] Tensor of inputs.
         :param timesteps: a 1-D batch of timesteps.
-        :param context: conditioning plugged in via crossattn
+        :param context: conditioning plugged in via crossattn.
         :param y: an [N] Tensor of labels, if class-conditional.
         :return: an [N x C x ...] Tensor of outputs.
         """
         x = x.squeeze()
-        #context = context.squeeze()
         x = self.input_proj(x)
-        t_emb = timestep_embedding(timesteps, self.model_channels, repeat_only=False)
+        t_emb = timestep_embedding(timesteps, self.channels, repeat_only=False)
         emb = self.time_embed(t_emb)
 
         for block in self.res_blocks:
             x = block(x, emb, context)
-        x = self.out(x)#.unsqueeze(-1).unsqueeze(-1)
-        x = x / self.marginal_prob_std(timesteps)[:, None]
+        x = self.out(x)
         return x
```

### Comparing `ood_detectors-0.0.5/LICENSE` & `ood_detectors-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.5/README.md` & `ood_detectors-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -20,58 +20,111 @@
 ```console
 pip install ood_detectors
 ```
 
 ## Usage
 This package includes several OOD detection algorithms, each tailored to different aspects of OOD detection:
 
-- DDM_Likelihood: A likelihood-based detector that utilizes score-based denoising diffusion models (DDM) to map complex distributions to known ones.
+- Likelihood Based: SubSDE_DDM, VPSDE_DDM and VESDE_DDM are likelihood-based methods that use different variations stochastic differential equations for DDMS to detect OOD samples. 
 
 - Residual: This method employs the least significant eigen vector for OOD detection.
 
 All detectors share a common interface:
 
 1. Initialize the detector with necessary hyperparameters.
 2. Fit the model using fit() with the training data.
 3. Use predict() to obtain OOD scores for new data samples.
 
 ## Example
 ```python
-from ood_detectors import DDM_Likelihood
+import ood_detectors.likelihood as likelihood
 
-ood_detector = DDM_Likelihood()
-ood_detector.fit(train_data, n_epochs, batch_size)
+ood_detector = likelihood.SubSDE_DDM(feat_dim).to('cuda')
+train_loss = ood_detector.fit(train_data, n_epochs, batch_size)
 scores = ood_detector.predict(test_data, batch_size)
 ```
 
 ```python
 from ood_detectors import Residual
 
 ood_detector = Residual()
-ood_detector.fit(train_data)
+train_loss = ood_detector.fit(train_data)
 scores = ood_detector.predict(test_data)
 ```
+
+## low-level interface
+
+The low-level interface allows you to customize the training process and access the model's internal components.
+
+```python
+import ood_detectors.likelihood as likelihood
+import ood_detectors.sde as sde_lib 
+import ood_detectors.models as models
+import ood_detectors.losses as losses
+...
+sde = sde_lib.subVPSDE(beta_min=beta_min, beta_max=beta_max)
+
+model = models.SimpleMLP(
+    channels=feat_dim,
+    bottleneck_channels=bottleneck_channels,
+    num_res_blocks=num_res_blocks,
+    time_embed_dim=time_embed_dim,
+    dropout=dropout,
+)
+
+optimizer = functools.partial(
+                torch.optim.Adam,
+                lr=lr,
+                betas=(beta1, beta2),
+                eps=eps,
+                weight_decay=weight_decay,
+                )
+
+ood_detector = likelihood.Likelihood(
+    sde = sde,
+    model = model,
+    optimizer = optimizer,
+    ).to(device)
+
+update_fn = functools.partial(
+    losses.SDE_EMA_LRS_BF16_GradClip, 
+    ema_rate=ema_rate,
+    total_steps=(len(train_blob['data'])//batch_size) * n_epochs,
+    grad_clip=grad_clip,
+    continuous=continuous,
+    reduce_mean=reduce_mean,
+    likelihood_weighting=likelihood_weighting,
+    )
+
+train_loss = ood_detector.fit(train_data, update_fn, batch_size)
+```
+
+## Create a custom component
+
+You can create a custom component by doing the same thing as the library does. Good luck!
+
+
 ## Evaluate 
 
 To assess the performance of the OOD detectors, you can utilize the following metrics:
 
 - AUC: Area under the ROC curve
 - FPR95: False positive rate when the true positive rate is 95%
 
 ```python
 import ood_detectors.eval_utils as eval_utils
-score_id = model_residual.predict(train_data)
-score_ref = model_residual.predict(reference_data)
+score_id = ood_detector.predict(train_data)
+score_ref = ood_detector.predict(reference_data)
 print(f"Train AUC: {eval_utils.auc(-score_ref, -score_id):.2%}")
 print(f"Train FPR95: {eval_utils.fpr95(-score_ref, -score_id):.2%}")
 ```
 
 ```python
-results = eval_utils.eval_ood(model, train_data, reference_data, ood_data, batch_size, verbose=False)
-plot_utils.plot(results, id_name, ood_names, encoder=embedding, model=model.__class__.__name__,
+results = eval_utils.eval_ood(ood_detector, train_data, reference_data, ood_data, batch_size, verbose=False)
+plot_utils.plot(results, id_name, ood_names, encoder=embedding, model=ood_detector.name,
                 train_loss=train_loss,
                 config=conf,
                 )
 ```
 
 
 ## License
```

### Comparing `ood_detectors-0.0.5/pyproject.toml` & `ood_detectors-0.0.6/pyproject.toml`

 * *Files identical despite different names*

