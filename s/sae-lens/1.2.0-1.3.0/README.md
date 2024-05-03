# Comparing `tmp/sae_lens-1.2.0.tar.gz` & `tmp/sae_lens-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.2.0.tar", max compression
+gzip compressed data, was "sae_lens-1.3.0.tar", max compression
```

## Comparing `sae_lens-1.2.0.tar` & `sae_lens-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-04-29 16:18:15.546059 sae_lens-1.2.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-04-29 16:18:15.546059 sae_lens-1.2.0/README.md
--rw-r--r--   0        0        0     1811 2024-04-29 16:18:16.550067 sae_lens-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-29 16:18:16.550067 sae_lens-1.2.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    15926 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    18451 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     6645 2024-04-29 16:18:15.554059 sae_lens-1.2.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    16793 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2849 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     9927 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1528 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8052 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    16225 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    19179 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-29 16:18:15.558059 sae_lens-1.2.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 sae_lens-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-03 10:11:03.016341 sae_lens-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-05-03 10:11:03.016341 sae_lens-1.3.0/README.md
+-rw-r--r--   0        0        0     1889 2024-05-03 10:11:04.744338 sae_lens-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-05-03 10:11:04.744338 sae_lens-1.3.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6643 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    16793 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2849 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    10112 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8266 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    17403 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    19601 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 sae_lens-1.3.0/PKG-INFO
```

### Comparing `sae_lens-1.2.0/LICENSE` & `sae_lens-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/README.md` & `sae_lens-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/pyproject.toml` & `sae_lens-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.2.0"
+version = "1.3.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
+include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 transformer-lens = "^1.14.0"
 transformers = "^4.38.1"
 jupyter = "^1.0.0"
 plotly = "^5.19.0"
@@ -16,26 +17,28 @@
 nbformat = "^5.9.2"
 ipykernel = "^6.29.2"
 matplotlib = "^3.8.3"
 matplotlib-inline = "^0.1.6"
 datasets = "^2.17.1"
 babe = "^0.0.7"
 nltk = "^3.8.1"
-sae-vis = "^0.2.15"
+sae-vis = "^0.2.18"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.15"
 mkdocs-autorefs = "^1.0.1"
 mkdocs-section-index = "^0.3.8"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
 safetensors = "^0.4.2"
 typer = "^0.12.3"
 mamba-lens = { version = "^0.0.4", optional = true }
 pyzmq = "26.0.0"
-automated-interpretability = "^0.0.2"
+automated-interpretability = "^0.0.3"
+python-dotenv = "^1.0.1"
+pyyaml = "^6.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "24.4.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
```

### Comparing `sae_lens-1.2.0/sae_lens/__init__.py` & `sae_lens-1.3.0/sae_lens/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.2.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.3.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.3.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-1.3.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,73 @@
+import asyncio
 import json
 import os
 import urllib.parse
 import webbrowser
 from datetime import datetime
-from typing import Literal, Optional
+from typing import Any, Optional, TypeVar
 
 import requests
+from dotenv import load_dotenv
+from neuron_explainer.activations.activation_records import calculate_max_activation
+from neuron_explainer.activations.activations import ActivationRecord
+from neuron_explainer.explanations.calibrated_simulator import (
+    UncalibratedNeuronSimulator,
+)
+from neuron_explainer.explanations.explainer import (
+    HARMONY_V4_MODELS,
+    ContextSize,
+    TokenActivationPairExplainer,
+)
+from neuron_explainer.explanations.explanations import ScoredSimulation
+from neuron_explainer.explanations.few_shot_examples import FewShotExampleSet
+from neuron_explainer.explanations.prompt_builder import PromptFormat
+from neuron_explainer.explanations.scoring import (
+    _simulate_and_score_sequence,
+    aggregate_scored_sequence_simulations,
+)
+from neuron_explainer.explanations.simulator import (
+    LogprobFreeExplanationTokenSimulator,
+    NeuronSimulator,
+)
+from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 NEURONPEDIA_DOMAIN = "https://neuronpedia.org"
 
 # Constants for replacing NaNs and Infs in outputs
 POSITIVE_INF_REPLACEMENT = 9999
 NEGATIVE_INF_REPLACEMENT = -9999
 NAN_REPLACEMENT = 0
 OTHER_INVALID_REPLACEMENT = -99999
 
+# Pick up OPENAI_API_KEY from environment variable
+load_dotenv()
+
 
 def NanAndInfReplacer(value: str):
+    """Replace NaNs and Infs in outputs."""
     replacements = {
         "-Infinity": NEGATIVE_INF_REPLACEMENT,
         "Infinity": POSITIVE_INF_REPLACEMENT,
         "NaN": NAN_REPLACEMENT,
     }
     if value in replacements:
-        replacedValue = replacements[value]
-        # print(f"Warning: Replacing value {value} with {replacedValue}")
-        return float(replacedValue)
+        replaced_value = replacements[value]
+        return float(replaced_value)
     else:
-        # print(f"Warning: Replacing value {value} with {NAN_REPLACEMENT}")
         return NAN_REPLACEMENT
 
 
 def get_neuronpedia_feature(
-    feature: int,
-    layer: int,
-    model: str = "gpt2-small",
-    dataset: str = "res-jb",
-):
-    url = NEURONPEDIA_DOMAIN + "/api/feature/"
-    url = url + f"{model}/{layer}-{dataset}/{feature}"
-
+    feature: int, layer: int, model: str = "gpt2-small", dataset: str = "res-jb"
+) -> dict[str, Any]:
+    """Fetch a feature from Neuronpedia API."""
+    url = f"{NEURONPEDIA_DOMAIN}/api/feature/{model}/{layer}-{dataset}/{feature}"
     result = requests.get(url).json()
     result["index"] = int(result["index"])
-
     return result
 
 
 def get_neuronpedia_quick_list(
     features: list[int],
     layer: int,
     model: str = "gpt2-small",
@@ -66,62 +87,82 @@
     ]
     url = url + "&features=" + urllib.parse.quote(json.dumps(list_feature))
     webbrowser.open(url)
 
     return url
 
 
-class NeuronpediaActivation(object):
-    id: str = ""
-    tokens = []
-    act_values = []
+class NeuronpediaActivation:
+    """Represents an activation from Neuronpedia."""
 
     def __init__(self, id: str, tokens: list[str], act_values: list[float]):
         self.id = id
         self.tokens = tokens
         self.act_values = act_values
 
 
-class NeuronpediaFeature(object):
-    modelId = ""
-    layer = 0
-    dataset = ""
-    index = 0
-    description = ""
-    activations = []
-    autointerp_explanation = ""
-    autointerp_explanation_score = 0
+class NeuronpediaFeature:
+    """Represents a feature from Neuronpedia."""
 
     def __init__(
         self,
         modelId: str,
         layer: int,
         dataset: str,
         feature: int,
         description: str = "",
-        activations: list[NeuronpediaActivation] = [],
+        activations: list[NeuronpediaActivation] | None = None,
         autointerp_explanation: str = "",
         autointerp_explanation_score: float = 0.0,
     ):
         self.modelId = modelId
         self.layer = layer
         self.dataset = dataset
         self.feature = feature
         self.description = description
         self.activations = activations
         self.autointerp_explanation = autointerp_explanation
         self.autointerp_explanation_score = autointerp_explanation_score
 
-    def has_activating_text(self):
-        has_activating_text = False
-        for activation in self.activations:
-            if max(activation.act_values) > 0:
-                has_activating_text = True
-                break
-        return has_activating_text
+    def has_activating_text(self) -> bool:
+        """Check if the feature has activating text."""
+        if self.activations is None:
+            return False
+        else:
+            return any(
+                max(activation.act_values) > 0 for activation in self.activations
+            )
+
+
+T = TypeVar("T")
+
+
+@retry(wait=wait_random_exponential(min=1, max=500), stop=stop_after_attempt(10))
+def sleep_identity(x: T) -> T:
+    """Dummy function for retrying."""
+    return x
+
+
+@retry(wait=wait_random_exponential(min=1, max=500), stop=stop_after_attempt(10))
+async def simulate_and_score(
+    simulator: NeuronSimulator, activation_records: list[ActivationRecord]
+) -> ScoredSimulation:
+    """Score an explanation of a neuron by how well it predicts activations on the given text sequences."""
+    scored_sequence_simulations = await asyncio.gather(
+        *[
+            sleep_identity(
+                _simulate_and_score_sequence(
+                    simulator,
+                    activation_record,
+                )
+            )
+            for activation_record in activation_records
+        ]
+    )
+    return aggregate_scored_sequence_simulations(scored_sequence_simulations)
 
 
 def make_neuronpedia_list_with_features(
     api_key: str,
     list_name: str,
     features: list[NeuronpediaFeature],
     list_description: Optional[str] = None,
@@ -151,83 +192,84 @@
         webbrowser.open(result["url"])
         return result["url"]
     else:
         raise Exception("Error in creating list: " + result["message"])
 
 
 def test_key(api_key: str):
-    url = NEURONPEDIA_DOMAIN + "/api/test"
-    body = {
-        "apiKey": api_key,
-    }
+    """Test the validity of the Neuronpedia API key."""
+    url = f"{NEURONPEDIA_DOMAIN}/api/test"
+    body = {"apiKey": api_key}
     response = requests.post(url, json=body)
     if response.status_code != 200:
         raise Exception("Neuronpedia API key is not valid.")
 
 
 async def autointerp_neuronpedia_features(
     features: list[NeuronpediaFeature],
-    openai_api_key: str,
+    openai_api_key: str | None = None,
     autointerp_retry_attempts: int = 3,
-    autointerp_score_max_concurrent: int = 20,  # good for this to match num_activations_to_use_for_score
-    neuronpedia_api_key: str = "",
-    # TODO check max budget estimate based on: num features, num act texts, act text lengths. fail if too high.
-    # max_budget_approx_usd: float = 5.00,
+    autointerp_score_max_concurrent: int = 20,
+    neuronpedia_api_key: str | None = None,
     do_score: bool = True,
     output_dir: str = "neuronpedia_outputs/autointerp",
     num_activations_to_use: int = 20,
+    max_explanation_activation_records: int = 20,
     upload_to_neuronpedia: bool = True,
-    autointerp_model_name: Literal["gpt-3.5-turbo", "gpt-4-turbo"] = "gpt-3.5-turbo",
+    autointerp_explainer_model_name: str = "gpt-4-1106-preview",
+    autointerp_scorer_model_name: str = "gpt-3.5-turbo",
 ):
-    print("\n\n")
+    """
+    Autointerp Neuronpedia features.
 
-    # make output_file named autointerp-<timestamp>
-    output_file = output_dir + "/" + datetime.now().strftime("%Y%m%d-%H%M%S") + ".jsonl"
-    if not os.path.exists(output_dir):
-        print("Creating output directory " + output_dir)
-        os.makedirs(output_dir, exist_ok=True)
-    print("===== Your results will be saved to: " + output_file + "=====")
-
-    # we import this here instead of top of file because the library requires the API key to be set first
-    os.environ["OPENAI_API_KEY"] = openai_api_key
-    from neuron_explainer.activations.activation_records import calculate_max_activation
-    from neuron_explainer.activations.activations import ActivationRecord
-    from neuron_explainer.explanations.calibrated_simulator import (
-        UncalibratedNeuronSimulator,
-    )
-    from neuron_explainer.explanations.explainer import (
-        ContextSize,
-        TokenActivationPairExplainer,
-    )
-    from neuron_explainer.explanations.few_shot_examples import FewShotExampleSet
-    from neuron_explainer.explanations.prompt_builder import PromptFormat
-    from neuron_explainer.explanations.scoring import simulate_and_score
-    from neuron_explainer.explanations.simulator import (
-        LogprobFreeExplanationTokenSimulator,
-    )
+    Args:
+        features: List of NeuronpediaFeature objects.
+        openai_api_key: OpenAI API key.
+        autointerp_retry_attempts: Number of retry attempts for autointerp.
+        autointerp_score_max_concurrent: Maximum number of concurrent requests for autointerp scoring.
+        neuronpedia_api_key: Neuronpedia API key.
+        do_score: Whether to score the features.
+        output_dir: Output directory for saving the results.
+        num_activations_to_use: Number of activations to use.
+        max_explanation_activation_records: Maximum number of activation records for explanation.
+        upload_to_neuronpedia: Whether to upload the results to Neuronpedia.
+        autointerp_explainer_model_name: Model name for autointerp explainer.
+        autointerp_scorer_model_name: Model name for autointerp scorer.
 
+    Returns:
+        None
     """
-    This does the following:
-    1. Fetches the features from Neuronpedia, including their activation texts
-    2. Explains the features using the autointerp_explainer_model_name
-    3. Scores the features using the autointerp_scorer_model_name
-    4. Saves the results in output_dir
-    5. Uploads the results to Neuronpedia
+    print("\n\n")
 
-    The openai_api_key is not sent to Neuronpedia, only to OpenAI.
-    """
+    if os.getenv("OPENAI_API_KEY") is None:
+        if openai_api_key is None:
+            raise Exception(
+                "You need to provide an OpenAI API key either in environment variable OPENAI_API_KEY or as an argument."
+            )
+        else:
+            os.environ["OPENAI_API_KEY"] = openai_api_key
+
+    if autointerp_explainer_model_name not in HARMONY_V4_MODELS:
+        raise Exception(
+            f"Invalid explainer model name: {autointerp_explainer_model_name}. Must be one of: {HARMONY_V4_MODELS}"
+        )
 
-    if upload_to_neuronpedia and neuronpedia_api_key == "":
+    if autointerp_scorer_model_name not in HARMONY_V4_MODELS:
         raise Exception(
-            "You need to provide a Neuronpedia API key to upload the results to Neuronpedia."
+            f"Invalid scorer model name: {autointerp_scorer_model_name}. Must be one of: {HARMONY_V4_MODELS}"
         )
 
-    test_key(neuronpedia_api_key)
+    if upload_to_neuronpedia:
+        if neuronpedia_api_key is None:
+            raise Exception(
+                "You need to provide a Neuronpedia API key to upload the results to Neuronpedia."
+            )
+        else:
+            test_key(neuronpedia_api_key)
 
-    # 1. Fetches the features from Neuronpedia, including their activation texts. Perform check for dead features.
     print("\n\n=== Step 1) Fetching features from Neuronpedia")
     for feature in features:
         feature_data = get_neuronpedia_feature(
             feature=feature.feature,
             layer=feature.layer,
             model=feature.modelId,
             dataset=feature.dataset,
@@ -252,114 +294,109 @@
                         id=activation["id"],
                         tokens=activation["tokens"],
                         act_values=activation["values"],
                     )
                 )
         feature.activations = activations_to_add
 
-        if feature.has_activating_text() is False:
+        if not feature.has_activating_text():
             raise Exception(
                 f"Feature {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature} appears dead - it does not have activating text."
             )
 
-    # TODO check max budget estimate based on number of features and act texts and act text length, fail if too high
-
-    # 2. Explain the features using the selected autointerp_explainer_model_name
     for iteration_num, feature in enumerate(features):
-        # print start time
         start_time = datetime.now()
 
         print(
             f"\n========== Feature {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature} ({iteration_num + 1} of {len(features)} Features) =========="
         )
         print(
             f"\n=== Step 2) Explaining feature {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature}"
         )
-        activationRecords = []
-        for activation in feature.activations:
-            activationRecord = ActivationRecord(
+
+        if feature.activations is None:
+            feature.activations = []
+        activation_records = [
+            ActivationRecord(
                 tokens=activation.tokens, activations=activation.act_values
             )
-            activationRecords.append(activationRecord)
+            for activation in feature.activations
+        ]
+
+        activation_records_explaining = activation_records[
+            :max_explanation_activation_records
+        ]
 
         explainer = TokenActivationPairExplainer(
-            model_name=autointerp_model_name,
+            model_name=autointerp_explainer_model_name,
             prompt_format=PromptFormat.HARMONY_V4,
             context_size=ContextSize.SIXTEEN_K,
             max_concurrent=1,
         )
 
         explanations = []
         for _ in range(autointerp_retry_attempts):
             try:
                 explanations = await explainer.generate_explanations(
-                    all_activation_records=activationRecords,
-                    max_activation=calculate_max_activation(activationRecords),
+                    all_activation_records=activation_records_explaining,
+                    max_activation=calculate_max_activation(
+                        activation_records_explaining
+                    ),
                     num_samples=1,
                 )
             except Exception as e:
                 print(f"ERROR, RETRYING: {e}")
             else:
                 break
         else:
             print(
                 f"ERROR: Failed to explain feature {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature}"
             )
 
         assert len(explanations) == 1
-        explanation = explanations[0]
-        # GPT ends its explanations with a period. Remove it.
-        if explanation.endswith("."):
-            explanation = explanation[:-1]
-        print(f"===== {autointerp_model_name}'s explanation: {explanation}")
+        explanation = explanations[0].rstrip(".")
+        print(f"===== {autointerp_explainer_model_name}'s explanation: {explanation}")
         feature.autointerp_explanation = explanation
 
-        # 3. Scores the features using the autointerp_scorer_model_name
         if do_score:
             print(
                 f"\n=== Step 3) Scoring feature {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature}"
             )
             print("=== This can take up to 30 seconds.")
 
-            # GPT struggles with non-ascii so we turn them into string representations
-            # make a temporary activation records copy for this, so we can return the original later
-            tempActivationRecords: list[ActivationRecord] = []
-            for activationRecord in activationRecords:
-                replacedActTokens: list[str] = []
-                for _, token in enumerate(activationRecord.tokens):
-                    replacedActTokens.append(
+            temp_activation_records = [
+                ActivationRecord(
+                    tokens=[
                         token.replace("<|endoftext|>", "<|not_endoftext|>")
                         .replace(" 55", "_55")
                         .encode("ascii", errors="backslashreplace")
                         .decode("ascii")
-                    )
-                tempActivationRecords.append(
-                    ActivationRecord(
-                        tokens=replacedActTokens,
-                        activations=activationRecord.activations,
-                    )
+                        for token in activation_record.tokens
+                    ],
+                    activations=activation_record.activations,
                 )
+                for activation_record in activation_records
+            ]
 
-            # Simulate and score the explanation.
             score = None
             scored_simulation = None
             for _ in range(autointerp_retry_attempts):
                 try:
                     simulator = UncalibratedNeuronSimulator(
                         LogprobFreeExplanationTokenSimulator(
-                            autointerp_model_name,
+                            autointerp_scorer_model_name,
                             explanation,
                             json_mode=True,
                             max_concurrent=autointerp_score_max_concurrent,
                             few_shot_example_set=FewShotExampleSet.JL_FINE_TUNED,
                             prompt_format=PromptFormat.HARMONY_V4,
                         )
                     )
                     scored_simulation = await simulate_and_score(
-                        simulator, tempActivationRecords
+                        simulator, temp_activation_records
                     )
                     score = scored_simulation.get_preferred_score()
                 except Exception as e:
                     print(f"ERROR, RETRYING: {e}")
                 else:
                     break
 
@@ -370,57 +407,57 @@
                 != num_activations_to_use
             ):
                 print(
                     f"ERROR: Failed to score feature {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature}. Skipping it."
                 )
                 continue
             feature.autointerp_explanation_score = score
-            print(f"===== {autointerp_model_name}'s score: {(score * 100):.0f}")
+            print(f"===== {autointerp_scorer_model_name}'s score: {(score * 100):.0f}")
+
+            output_file = (
+                f"{output_dir}/{feature.layer}-{feature.dataset}_feature-{feature.feature}_score-"
+                f"{feature.autointerp_explanation_score}_time-{datetime.now().strftime('%Y%m%d-%H%M%S')}.jsonl"
+            )
+            os.makedirs(output_dir, exist_ok=True)
+            print(f"===== Your results will be saved to: {output_file} =====")
 
-            # replace NaNs and Infs in the output so we get valid JSON
             output_data = json.dumps(
                 {
                     "apiKey": neuronpedia_api_key,
                     "feature": {
                         "modelId": feature.modelId,
                         "layer": f"{feature.layer}-{feature.dataset}",
                         "index": feature.feature,
                         "activations": feature.activations,
                         "explanation": feature.autointerp_explanation,
                         "explanationScore": feature.autointerp_explanation_score,
-                        "autointerpModel": autointerp_model_name,
+                        "explanationModel": autointerp_explainer_model_name,
+                        "autointerpModel": autointerp_scorer_model_name,
                         "simulatedActivations": scored_simulation.scored_sequence_simulations,
                     },
                 },
                 default=vars,
             )
-            output_data_json = json.loads(
-                output_data,
-                parse_constant=NanAndInfReplacer,
-            )
+            output_data_json = json.loads(output_data, parse_constant=NanAndInfReplacer)
             output_data_str = json.dumps(output_data)
 
-            # 4. Save the results in output_file
-            # open output_file and append the feature
             print(f"\n=== Step 4) Saving feature to {output_file}")
             with open(output_file, "a") as f:
                 f.write(output_data_str)
                 f.write("\n")
 
-            # 5. Uploads the results to Neuronpedia
             if upload_to_neuronpedia:
                 print(
                     f"\n=== Step 5) Uploading feature to Neuronpedia: {feature.modelId}@{feature.layer}-{feature.dataset}:{feature.feature}"
                 )
-                url = NEURONPEDIA_DOMAIN + "/api/upload-explanation"
+                url = f"{NEURONPEDIA_DOMAIN}/api/upload-explanation"
                 body = output_data_json
                 response = requests.post(url, json=body)
                 if response.status_code != 200:
                     print(
                         f"ERROR: Couldn't upload explanation to Neuronpedia: {response.text}"
                     )
 
-        # print end_time minus start_time)
         end_time = datetime.now()
-        print("\n========== Time Spent for Feature: {}\n".format(end_time - start_time))
+        print(f"\n========== Time Spent for Feature: {end_time - start_time}\n")
 
     print("\n\n========== Generation and Upload Complete ==========\n\n")
```

### Comparing `sae_lens-1.2.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.3.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         # token pars
         n_batches_to_sample_from: int = 2**12,
         n_prompts_to_select: int = 4096 * 6,
         # batching
         n_features_at_a_time: int = 128,
         start_batch_inclusive: int = 0,
         end_batch_inclusive: Optional[int] = None,
+        # quantiles
+        n_quantiles: int = 5,
+        top_acts_group_size: int = 20,
+        quantile_group_size: int = 5,
     ):
 
         self.device = "cpu"
         if torch.backends.mps.is_available():
             self.device = "mps"
         elif torch.cuda.is_available():
             self.device = "cuda"
@@ -93,14 +97,17 @@
         self.sae_id = sae_id
         self.sparsity_threshold = sparsity_threshold
         self.n_features_at_a_time = n_features_at_a_time
         self.n_batches_to_sample_from = n_batches_to_sample_from
         self.n_prompts_to_select = n_prompts_to_select
         self.start_batch = start_batch_inclusive
         self.end_batch = end_batch_inclusive
+        self.n_quantiles = n_quantiles
+        self.top_acts_group_size = top_acts_group_size
+        self.quantile_group_size = quantile_group_size
 
         if not os.path.exists(outputs_dir):
             os.makedirs(outputs_dir)
         self.outputs_dir = outputs_dir
 
     def get_tokens(
         self,
@@ -250,17 +257,17 @@
                 layout = SaeVisLayoutConfig(
                     columns=[
                         Column(
                             SequencesConfig(
                                 stack_mode="stack-all",
                                 buffer=None,  # type: ignore
                                 compute_buffer=True,
-                                n_quantiles=5,
-                                top_acts_group_size=20,
-                                quantile_group_size=5,
+                                n_quantiles=self.n_quantiles,
+                                top_acts_group_size=self.top_acts_group_size,
+                                quantile_group_size=self.quantile_group_size,
                             ),
                             ActsHistogramConfig(),
                             LogitsHistogramConfig(),
                             LogitsTableConfig(),
                             FeatureTablesConfig(n_rows=3),
                         )
                     ]
@@ -359,22 +366,47 @@
                     feature_output["num_tokens_for_dashboard"] = (
                         self.n_prompts_to_select
                     )
 
                     activations = []
                     sdbs = feature.sequence_data
                     for sgd in sdbs.seq_group_data:
+                        binMin = 0
+                        binMax = 0
+                        binContains = 0
+                        if "TOP ACTIVATIONS" in sgd.title:
+                            binMin = -1
+                            try:
+                                binMax = float(sgd.title.split(" = ")[-1])
+                            except ValueError:
+                                print(f"Error parsing top acts: {sgd.title}")
+                                binMax = 99
+                            binContains = -1
+                        elif "INTERVAL" in sgd.title:
+                            try:
+                                split = sgd.title.split("<br>")
+                                firstSplit = split[0].split(" ")
+                                binMin = float(firstSplit[1])
+                                binMax = float(firstSplit[-1])
+                                secondSplit = split[1].split(" ")
+                                binContains = float(secondSplit[-1].rstrip("%")) / 100
+                            except ValueError:
+                                print(f"Error parsing interval: {sgd.title}")
                         for sd in sgd.seq_data:
                             if (
                                 sd.top_token_ids is not None
                                 and sd.bottom_token_ids is not None
                                 and sd.top_logits is not None
                                 and sd.bottom_logits is not None
                             ):
                                 activation = {}
+                                activation["binMin"] = binMin
+                                activation["binMax"] = binMax
+                                activation["binContains"] = binContains
+
                                 strs = []
                                 posContribs = []
                                 negContribs = []
                                 for i in range(len(sd.token_ids)):
                                     strs.append(
                                         self.to_str_tokens_safe(
                                             vocab_dict, sd.token_ids[i]
```

### Comparing `sae_lens-1.2.0/sae_lens/analysis/tsea.py` & `sae_lens-1.3.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import pathlib
 from typing import Optional, Tuple
 
 import torch
-from huggingface_hub import hf_hub_download, list_files_info
+from huggingface_hub import hf_hub_download, list_repo_tree
 from safetensors import safe_open
 from tqdm import tqdm
 
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
@@ -168,15 +168,15 @@
 def get_gpt2_small_ckrk_attn_out_saes() -> dict[str, SparseAutoencoder]:
 
     REPO_ID = "ckkissane/attn-saes-gpt2-small-all-layers"
 
     # list all files in repo
     saes_weights = {}
     sae_configs = {}
-    repo_files = list_files_info(REPO_ID)
+    repo_files = list_repo_tree(REPO_ID)
     for i in tqdm(repo_files):
         file_name = i.path
         if file_name.endswith(".pt"):
             # print(f"Downloading {file_name}")
             path = hf_hub_download(REPO_ID, file_name)
             name = path.split("/")[-1].split(".pt")[0]
             saes_weights[name] = torch.load(path, map_location="mps")
```

### Comparing `sae_lens-1.2.0/sae_lens/training/activations_store.py` & `sae_lens-1.3.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-1.3.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/config.py` & `sae_lens-1.3.0/sae_lens/training/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import dataclass, field
 from typing import Any, Optional, cast
 
 import torch
 import wandb
 
+from sae_lens import __version__
+
 DTYPE_MAP = {
     "torch.float32": torch.float32,
     "torch.float64": torch.float64,
     "torch.float16": torch.float16,
     "torch.bfloat16": torch.bfloat16,
 }
 
@@ -104,14 +106,16 @@
     wandb_log_frequency: int = 10
 
     # Misc
     n_checkpoints: int = 0
     checkpoint_path: str = "checkpoints"
     verbose: bool = True
     model_kwargs: dict[str, Any] = field(default_factory=dict)
+    sae_lens_version: str = field(default_factory=lambda: __version__)
+    sae_lens_training_version: str = field(default_factory=lambda: __version__)
 
     def __post_init__(self):
         if self.use_cached_activations and self.cached_activations_path is None:
             self.cached_activations_path = _default_cached_activations_path(
                 self.dataset_path,
                 self.model_name,
                 self.hook_point,
```

### Comparing `sae_lens-1.2.0/sae_lens/training/evals.py` & `sae_lens-1.3.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/geometric_median.py` & `sae_lens-1.3.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/lm_runner.py` & `sae_lens-1.3.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/load_model.py` & `sae_lens-1.3.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/optim.py` & `sae_lens-1.3.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/sae_group.py` & `sae_lens-1.3.0/sae_lens/training/sae_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,17 +125,21 @@
             raise ValueError(
                 f"Unexpected file extension: {path}, supported extensions are .pt, .pkl, and .pkl.gz"
             )
 
         # handle loading old autoencoders where before SAEGroup existed, where we just save a dict
         if isinstance(group, dict):
             cfg = group["cfg"]
-            # need to add this field to old configs
+            # need to add fields to old configs
             if not hasattr(cfg, "model_kwargs"):
                 cfg.model_kwargs = {}
+            if not hasattr(cfg, "sae_lens_version"):
+                cfg.sae_lens_version = "0.0.0"
+            if not hasattr(cfg, "sae_lens_training_version"):
+                cfg.sae_lens_training_version = "0.0.0"
             sparse_autoencoder = SparseAutoencoder(cfg=cfg)
             # add dummy scaling factor to the state dict
             group["state_dict"]["scaling_factor"] = torch.ones(
                 cfg.d_sae, dtype=cfg.dtype, device=cfg.device
             )
             sparse_autoencoder.load_state_dict(group["state_dict"])
             group = cls(cfg)
```

### Comparing `sae_lens-1.2.0/sae_lens/training/session_loader.py` & `sae_lens-1.3.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.3.0/sae_lens/training/sparse_autoencoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 import os
 import pickle
 from typing import Callable, NamedTuple, Optional
 
 import einops
 import torch
 from jaxtyping import Float
-from safetensors import safe_open
 from safetensors.torch import save_file
 from torch import nn
 from transformer_lens.hook_points import HookedRootModule, HookPoint
 
+from sae_lens.toolkit.pretrained_sae_loaders import (
+    NAMED_PRETRAINED_SAE_LOADERS,
+    load_pretrained_sae_lens_sae_components,
+)
+from sae_lens.toolkit.pretrained_saes_directory import get_pretrained_saes_directory
 from sae_lens.training.activation_functions import get_activation_fn
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.utils import BackwardsCompatiblePickleClass
 
 
 class ForwardOutput(NamedTuple):
     sae_out: torch.Tensor
@@ -354,43 +358,75 @@
                 instance.cfg.d_sae, dtype=instance.cfg.dtype, device=instance.cfg.device
             )
         instance.load_state_dict(state_dict["state_dict"], strict=True)
 
         return instance
 
     @classmethod
-    def load_from_pretrained(cls, path: str, device: str = "cpu"):
+    def load_from_pretrained(
+        cls, path: str, device: str = "cpu"
+    ) -> "SparseAutoencoder":
 
         config_path = os.path.join(path, "cfg.json")
         weight_path = os.path.join(path, "sae_weights.safetensors")
 
-        with open(config_path, "r") as f:
-            config = json.load(f)
+        cfg, state_dict = load_pretrained_sae_lens_sae_components(
+            config_path, weight_path, device
+        )
+
+        sae = cls(cfg)
+        sae.load_state_dict(state_dict)
+
+        return sae
+
+    @classmethod
+    def from_pretrained(
+        cls, release: str, sae_id: str, device: str = "cpu"
+    ) -> "SparseAutoencoder":
+        """
+
+        Load a pretrained SAE from the Hugging Face model hub.
+
+        Args:
+            release: The release name. This will be mapped to a huggingface repo id based on the pretrained_saes.yaml file.
+            id: The id of the SAE to load. This will be mapped to a path in the huggingface repo.
+            device: The device to load the SAE on.
 
-        var_names = LanguageModelSAERunnerConfig.__init__.__code__.co_varnames
-        # filter config for varnames
-        config = {k: v for k, v in config.items() if k in var_names}
-        config["verbose"] = False
-        config["device"] = device
-        config = LanguageModelSAERunnerConfig(**config)
-        sae = SparseAutoencoder(config)
-
-        tensors = {}
-        with safe_open(weight_path, framework="pt", device=device) as f:  # type: ignore
-            for k in f.keys():
-                tensors[k] = f.get_tensor(k)
-
-        # old saves may not have scaling factors.
-        if "scaling_factor" not in tensors:
-            assert isinstance(config.d_sae, int)
-            tensors["scaling_factor"] = torch.ones(
-                config.d_sae, dtype=config.dtype, device=config.device
+        """
+
+        # get sae directory
+        sae_directory = get_pretrained_saes_directory()
+
+        # get the repo id and path to the SAE
+        if release not in sae_directory:
+            raise ValueError(
+                f"Release {release} not found in pretrained SAEs directory."
             )
+        if sae_id not in sae_directory[release].saes_map:
+            raise ValueError(f"ID {sae_id} not found in release {release}.")
+        sae_info = sae_directory[release]
+        hf_repo_id = sae_info.repo_id
+        hf_path = sae_info.saes_map[sae_id]
+
+        conversion_loader_name = sae_info.conversion_func or "sae_lens"
+        if conversion_loader_name not in NAMED_PRETRAINED_SAE_LOADERS:
+            raise ValueError(
+                f"Conversion func {conversion_loader_name} not found in NAMED_PRETRAINED_SAE_LOADERS."
+            )
+        conversion_loader = NAMED_PRETRAINED_SAE_LOADERS[conversion_loader_name]
+
+        cfg, state_dict = conversion_loader(
+            repo_id=hf_repo_id,
+            folder_name=hf_path,
+            device=device,
+            force_download=False,
+        )
 
-        sae.load_state_dict(tensors)
+        sae = cls(cfg)
+        sae.load_state_dict(state_dict)
 
         return sae
 
     def get_name(self):
         sae_name = f"sparse_autoencoder_{self.cfg.model_name}_{self.cfg.hook_point}_{self.cfg.d_sae}"
         return sae_name
```

### Comparing `sae_lens-1.2.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.3.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/toy_models.py` & `sae_lens-1.3.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.3.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import wandb
 from safetensors.torch import save_file
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from tqdm import tqdm
 from transformer_lens.hook_points import HookedRootModule
 
+from sae_lens import __version__
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
 from sae_lens.training.optim import get_scheduler
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
@@ -107,14 +108,15 @@
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
 ) -> TrainSAEGroupOutput:
+    _update_sae_lens_training_version(sae_group)
     total_training_tokens = (
         sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
     )
     total_training_steps = total_training_tokens // batch_size
     n_training_steps = 0
     n_training_tokens = 0
     started_fine_tuning = False
@@ -344,14 +346,23 @@
         elif hyperparams.b_dec_init_method == "mean":
             layer_acts = activation_store.storage_buffer.detach().cpu()[
                 :, sae_layer_id, :
             ]
             sae.initialize_b_dec_with_mean(layer_acts)
 
 
+def _update_sae_lens_training_version(sae_group: SparseAutoencoderDictionary) -> None:
+    """
+    Make sure we record the version of SAELens used for the training run
+    """
+    sae_group.cfg.sae_lens_training_version = __version__
+    for sae in sae_group.autoencoders.values():
+        sae.cfg.sae_lens_training_version = __version__
+
+
 @dataclass
 class TrainStepOutput:
     sae_in: torch.Tensor
     sae_out: torch.Tensor
     feature_acts: torch.Tensor
     loss: torch.Tensor
     mse_loss: torch.Tensor
```

### Comparing `sae_lens-1.2.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.3.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/sae_lens/training/utils.py` & `sae_lens-1.3.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.2.0/PKG-INFO` & `sae_lens-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.2.0
+Version: 1.3.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mamba
-Requires-Dist: automated-interpretability (>=0.0.2,<0.0.3)
+Requires-Dist: automated-interpretability (>=0.0.3,<0.0.4)
 Requires-Dist: babe (>=0.0.7,<0.0.8)
 Requires-Dist: datasets (>=2.17.1,<3.0.0)
 Requires-Dist: ipykernel (>=6.29.2,<7.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: mamba-lens (>=0.0.4,<0.0.5) ; extra == "mamba"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: matplotlib-inline (>=0.1.6,<0.2.0)
@@ -23,16 +23,18 @@
 Requires-Dist: mkdocs-section-index (>=0.3.8,<0.4.0)
 Requires-Dist: mkdocstrings (>=0.24.1,<0.25.0)
 Requires-Dist: mkdocstrings-python (>=1.9.0,<2.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: plotly (>=5.19.0,<6.0.0)
 Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (==26.0.0)
-Requires-Dist: sae-vis (>=0.2.15,<0.3.0)
+Requires-Dist: sae-vis (>=0.2.18,<0.3.0)
 Requires-Dist: safetensors (>=0.4.2,<0.5.0)
 Requires-Dist: transformer-lens (>=1.14.0,<2.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 <img width="1308" alt="Screenshot 2024-03-21 at 3 08 28 pm" src="https://github.com/jbloomAus/mats_sae_training/assets/69127271/209012ec-a779-4036-b4be-7b7739ea87f6">
```

