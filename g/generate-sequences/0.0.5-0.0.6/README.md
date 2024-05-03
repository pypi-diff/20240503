# Comparing `tmp/generate_sequences-0.0.5.tar.gz` & `tmp/generate_sequences-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_sequences-0.0.5.tar", last modified: Mon Apr 29 07:25:14 2024, max compression
+gzip compressed data, was "generate_sequences-0.0.6.tar", last modified: Fri May  3 17:10:41 2024, max compression
```

## Comparing `generate_sequences-0.0.5.tar` & `generate_sequences-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:25:14.752354 generate_sequences-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-29 07:25:14.752354 generate_sequences-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:25:14.748354 generate_sequences-0.0.5/generate_sequences/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/generate_sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/generate_sequences/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/generate_sequences/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/generate_sequences/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:25:14.748354 generate_sequences-0.0.5/generate_sequences.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-29 07:25:14.000000 generate_sequences-0.0.5/generate_sequences.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-29 07:25:14.000000 generate_sequences-0.0.5/generate_sequences.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:25:14.000000 generate_sequences-0.0.5/generate_sequences.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-29 07:25:14.000000 generate_sequences-0.0.5/generate_sequences.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 07:25:14.000000 generate_sequences-0.0.5/generate_sequences.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-29 07:17:08.000000 generate_sequences-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:25:14.752354 generate_sequences-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:10:41.018571 generate_sequences-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-03 17:10:41.018571 generate_sequences-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:10:41.014571 generate_sequences-0.0.6/generate_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/generate_sequences/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:10:41.014571 generate_sequences-0.0.6/generate_sequences.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14973 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 17:10:41.000000 generate_sequences-0.0.6/generate_sequences.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 17:08:30.000000 generate_sequences-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:10:41.018571 generate_sequences-0.0.6/setup.cfg
```

### Comparing `generate_sequences-0.0.5/LICENSE` & `generate_sequences-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_sequences-0.0.5/PKG-INFO` & `generate_sequences-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,29 +213,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm==4.66.*
 Requires-Dist: numpy>=1.24.0
-Requires-Dist: torch==2.2.*
+Requires-Dist: torch<2.4,>=2.2
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.1.29; extra == "dev"
+Requires-Dist: furo==2024.4.27; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: evaluate==0.4.*; extra == "dev"
```

### Comparing `generate_sequences-0.0.5/generate_sequences/generate.py` & `generate_sequences-0.0.6/generate_sequences/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class GreedyGenerator(BaseGenerator):
     @torch.no_grad()
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         outputs = []
         # add user warning if temperature is not 1.0 that greedy search is not appropriate
         if self.temperature != 1.0 and not self.multinomial_sampling:
             warnings.warn(
-                "Temperature does not have an affect on Greedy search if multinomial sampling is set to False! If forgot to add multinomail sampling, set `multinomial_sampling=True` to the generator."
+                "Temperature does not have an affect on Greedy search if multinomial sampling is set to False! If forgot to add multinomial sampling, set `multinomial_sampling=True` to the generator."
             )
 
         for batch_inputs in self.get_batches(inputs):
             batch_size = len(batch_inputs)
             decoder_inputs = torch.full(
                 (batch_size, self.max_length),
                 self.eos_token_id,  # Pre-fill with EOS; only overwrite if generating
@@ -103,53 +103,16 @@
     """Calculates the adjusted score of a node for beam sorting. Applies length penalty to score."""
     tokens = node.tokens
     if eos_token_id in tokens:
         tokens = tokens[1 : tokens.index(eos_token_id) + 1]
     return node.score / (len(tokens) ** length_penalty)
 
 
-class Beam:
-    """Manages a list of BeamNodes for the beam search algorithm with a fixed beam width."""
-
-    def __init__(
-        self,
-        eos_token_id: int,
-        beam_width: int = 4,
-        length_penalty: float = 1.0,
-        beam_nodes_ordering_function: Callable[
-            [BeamNode, int, float], float
-        ] = default_beam_nodes_ordering_fn,
-    ):
-        self.nodes: List[BeamNode] = []
-        self.beam_width = beam_width
-        self.eos_token_id = eos_token_id
-        self.length_penalty = length_penalty
-        self.beam_nodes_ordering_function = beam_nodes_ordering_function
-
-    def add(self, node: BeamNode) -> None:
-        """Adds a new node to the beam."""
-        self.nodes.append(node)
-
-    def get_topk(self) -> List[BeamNode]:
-        """Returns the top k nodes in the beam according to the ordering function."""
-        return heapq.nlargest(
-            self.beam_width,
-            self.nodes,
-            key=lambda node: self.beam_nodes_ordering_function(
-                node,
-                self.eos_token_id,
-                self.length_penalty,
-            ),
-        )
-
-    def has_finished(self) -> bool:
-        """Checks if all nodes in the beam have reached the end of sequence token."""
-        return all(node.tokens[-1] == self.eos_token_id for node in self.nodes)
-
-
+# this implementation is inspired by:
+# https://hussainwali.medium.com/simple-implementation-of-beam-search-in-python-64b2d3e2fd7e
 class BeamSearchGenerator(BaseGenerator):
     def __init__(
         self,
         decoder_start_token_id: int,
         eos_token_id: int,
         generation_forward: Callable[
             [Union[List[torch.Tensor], List[str]], torch.Tensor],
@@ -178,49 +141,57 @@
             use_tqdm,
             multinomial_sampling,
         )
         self.beam_width = beam_width
         self.length_penalty = length_penalty
         self.beam_nodes_ordering_function = beam_nodes_ordering_function
 
+    def get_top_nodes(self, nodes) -> List[BeamNode]:
+        """Returns the top k nodes in the beam according to the ordering function."""
+        return heapq.nlargest(
+            self.beam_width,
+            nodes,
+            key=lambda node: self.beam_nodes_ordering_function(
+                node,
+                self.eos_token_id,
+                self.length_penalty,
+            ),
+        )
+
     @torch.no_grad
     def generate(self, inputs: Union[List[torch.Tensor], List[str]]) -> List[torch.Tensor]:
         predictions = []
         for batch in self.get_batches(inputs):
-            beams = []
-            for _ in range(len(batch)):
-                beam = Beam(
-                    beam_width=self.beam_width,
-                    eos_token_id=self.eos_token_id,
-                    length_penalty=self.length_penalty,
-                    beam_nodes_ordering_function=self.beam_nodes_ordering_function,
-                )
-                beam.add(
+            batch_nodes = [
+                [
                     BeamNode(
                         tokens=[self.decoder_start_token_id],
                         score=0.0,
                     )
-                )
-                beams.append(beam)
-            for t in range(self.max_length):
-                next_beams = [
-                    Beam(
-                        beam_width=self.beam_width,
-                        eos_token_id=self.eos_token_id,
-                        length_penalty=self.length_penalty,
-                        beam_nodes_ordering_function=self.beam_nodes_ordering_function,
-                    )
-                    for _ in range(len(batch))
                 ]
-                best_beams_nodes = [beam.get_topk() for beam in beams]
-                for k in range(
-                    len(best_beams_nodes[0])
-                ):  # beam width, taking the case where k < len(best_beams_nodes[0])
+                for _ in range(len(batch))
+            ]
+            batch_best_nodes = batch_nodes
+            for step in range(self.max_length):
+                next_nodes: List[List[BeamNode]] = [[] for _ in range(len(batch))]
+                batch_best_nodes = [
+                    self.get_top_nodes(sample_nodes) for sample_nodes in batch_best_nodes
+                ]
+                # break when all best nodes ends with eos
+                if all(
+                    batch_best_nodes[sample_index][i].tokens[-1] == self.eos_token_id
+                    for sample_index in range(len(batch))
+                    for i in range(len(batch_best_nodes[sample_index]))
+                ):
+                    break
+                # beam width, taking the case where k < len(best_beams_nodes[0]), i.e. in the first step
+                beam_width = 1 if step == 0 else self.beam_width
+                for k in range(beam_width):
                     decoder_input_ids = torch.LongTensor(
-                        [topk_nodes[k].tokens for topk_nodes in best_beams_nodes]
+                        [sample_best_nodes[k].tokens for sample_best_nodes in batch_best_nodes]
                     ).to(self.device)
                     batch_outputs = self.generation_forward(batch, decoder_input_ids)
                     batch_outputs = batch_outputs[:, -1, :]
                     batch_outputs = batch_outputs / self.temperature
                     batch_outputs = F.log_softmax(batch_outputs, dim=-1)
                     # check for multinomial sampling
                     if self.multinomial_sampling:
@@ -228,42 +199,40 @@
                             torch.exp(batch_outputs),
                             self.beam_width,
                             replacement=True,
                         )
                         topk_scores = batch_outputs.gather(1, topk_indices)
                     else:
                         topk_scores, topk_indices = torch.topk(batch_outputs, self.beam_width)
-                    for beam_index, beam in enumerate(next_beams):
-                        # Check if this sequence has already reached eos token
-                        if best_beams_nodes[beam_index][k].tokens[-1] == self.eos_token_id:
-                            beam.add(
+                    for sample_index in range(len(batch)):
+                        if batch_best_nodes[sample_index][k].tokens[-1] == self.eos_token_id:
+                            next_nodes[sample_index] += [
                                 BeamNode(
-                                    tokens=best_beams_nodes[beam_index][k].tokens
+                                    tokens=batch_best_nodes[sample_index][k].tokens
                                     + [self.eos_token_id],
                                     score=0,
                                 )
-                            )
+                            ] * self.beam_width
                         else:
-                            for k2 in range(self.beam_width):
-                                beam.add(
-                                    BeamNode(
-                                        tokens=best_beams_nodes[beam_index][k].tokens
-                                        + [topk_indices[beam_index][k2].item()],
-                                        score=best_beams_nodes[beam_index][k].score
-                                        + topk_scores[beam_index][k2].item(),
-                                    )
+                            next_nodes[sample_index] += [
+                                BeamNode(
+                                    tokens=batch_best_nodes[sample_index][k].tokens
+                                    + [topk_indices[sample_index][i].item()],
+                                    score=batch_best_nodes[sample_index][k].score
+                                    + topk_scores[sample_index][i].item(),
                                 )
-                beams = next_beams  # Update beams for the next time step
-                if all(beam.has_finished() for beam in beams):
-                    break
+                                for i in range(self.beam_width)
+                            ]
+
+                batch_best_nodes = next_nodes  # Update beams for the next time step
 
             batch_predictions = []
-            for beam in beams:
+            for sample_nodes in batch_best_nodes:
                 best_node = max(
-                    beam.nodes,
+                    sample_nodes,
                     key=lambda node: self.beam_nodes_ordering_function(
                         node,
                         self.eos_token_id,
                         self.length_penalty,
                     ),
                 )
                 batch_predictions.append(best_node.tokens)
```

### Comparing `generate_sequences-0.0.5/generate_sequences.egg-info/PKG-INFO` & `generate_sequences-0.0.6/generate_sequences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-sequences
-Version: 0.0.5
+Version: 0.0.6
 Author-email: "Maged S. Al-Shaibani" <mageedsaeed1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,29 +213,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm==4.66.*
 Requires-Dist: numpy>=1.24.0
-Requires-Dist: torch==2.2.*
+Requires-Dist: torch<2.4,>=2.2
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: Sphinx<7.4.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.1.29; extra == "dev"
+Requires-Dist: furo==2024.4.27; extra == "dev"
 Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev"
 Requires-Dist: sphinx-autodoc-typehints==2.0.0; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: evaluate==0.4.*; extra == "dev"
```

### Comparing `generate_sequences-0.0.5/pyproject.toml` & `generate_sequences-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 authors = [{ name = "Maged S. Al-Shaibani", email = "mageedsaeed1@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
   # Add your own dependencies here
   "tqdm==4.66.*",
   "numpy>=1.24.0",
-  "torch==2.2.*",
+  "torch>=2.2,<2.4",
 ]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/MagedSaeed/generate-sequences"
 Repository = "https://github.com/MagedSaeed/generate-sequences"
 Changelog = "https://github.com/MagedSaeed/generate-sequences/blob/main/CHANGELOG.md"
@@ -40,15 +40,15 @@
   "pytest-sphinx",
   "pytest-cov",
   "twine>=1.11.0",
   "build",
   "setuptools",
   "wheel",
   "Sphinx>=4.3.0,<7.4.0",
-  "furo==2024.1.29",
+  "furo==2024.4.27",
   "myst-parser>=1.0,<2.1",
   "sphinx-copybutton==0.5.2",
   "sphinx-autobuild==2021.3.14",
   "sphinx-autodoc-typehints==2.0.0",
   "packaging",
   "pre-commit==3.5.0",
   # added for testing
@@ -95,15 +95,15 @@
 [tool.pyright]
 reportPrivateImportUsage = false
 
 [tool.ruff]
 line-length = 115
 target-version = "py39"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.mypy]
 ignore_missing_imports = true
 no_site_packages = true
 check_untyped_defs = true
```

