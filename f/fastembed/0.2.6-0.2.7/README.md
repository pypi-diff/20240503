# Comparing `tmp/fastembed-0.2.6.tar.gz` & `tmp/fastembed-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastembed-0.2.6.tar", max compression
+gzip compressed data, was "fastembed-0.2.7.tar", max compression
```

## Comparing `fastembed-0.2.6.tar` & `fastembed-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-04-01 15:24:42.768703 fastembed-0.2.6/LICENSE
--rw-r--r--   0        0        0     3591 2024-04-01 15:24:42.768703 fastembed-0.2.6/README.md
--rw-r--r--   0        0        0      259 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/__init__.py
--rw-r--r--   0        0        0     8338 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/model_management.py
--rw-r--r--   0        0        0     2030 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/models.py
--rw-r--r--   0        0        0     4701 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/onnx_model.py
--rw-r--r--   0        0        0      890 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/utils.py
--rw-r--r--   0        0        0      604 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/embedding.py
--rw-r--r--   0        0        0        0 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/image/__init__.py
--rw-r--r--   0        0        0     7539 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/parallel_processor.py
--rw-r--r--   0        0        0      192 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/__init__.py
--rw-r--r--   0        0        0     1062 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/sparse_embedding_base.py
--rw-r--r--   0        0        0     3063 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/sparse_text_embedding.py
--rw-r--r--   0        0        0     4669 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/splade_pp.py
--rw-r--r--   0        0        0       85 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/__init__.py
--rw-r--r--   0        0        0     1923 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/e5_onnx_embedding.py
--rw-r--r--   0        0        0     2191 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/jina_onnx_embedding.py
--rw-r--r--   0        0        0     8286 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/onnx_embedding.py
--rw-r--r--   0        0        0     3399 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/text_embedding.py
--rw-r--r--   0        0        0     1819 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/text_embedding_base.py
--rw-r--r--   0        0        0     1180 2024-04-01 15:24:42.776703 fastembed-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 fastembed-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 16:37:04.473064 fastembed-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4125 2024-05-03 16:37:04.473064 fastembed-0.2.7/README.md
+-rw-r--r--   0        0        0      398 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/common/__init__.py
+-rw-r--r--   0        0        0     8675 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/common/model_management.py
+-rw-r--r--   0        0        0     2030 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/common/models.py
+-rw-r--r--   0        0        0     5266 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/common/onnx_model.py
+-rw-r--r--   0        0        0      890 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/common/utils.py
+-rw-r--r--   0        0        0      604 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/embedding.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/image/__init__.py
+-rw-r--r--   0        0        0     7539 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/parallel_processor.py
+-rw-r--r--   0        0        0      192 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/sparse/__init__.py
+-rw-r--r--   0        0        0     1133 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/sparse/sparse_embedding_base.py
+-rw-r--r--   0        0        0     3234 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/sparse/sparse_text_embedding.py
+-rw-r--r--   0        0        0     4902 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/sparse/splade_pp.py
+-rw-r--r--   0        0        0       85 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/text/__init__.py
+-rw-r--r--   0        0        0     2049 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/text/e5_onnx_embedding.py
+-rw-r--r--   0        0        0     2273 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/text/jina_onnx_embedding.py
+-rw-r--r--   0        0        0    10151 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/text/onnx_embedding.py
+-rw-r--r--   0        0        0     3570 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/text/text_embedding.py
+-rw-r--r--   0        0        0     1890 2024-05-03 16:37:04.477064 fastembed-0.2.7/fastembed/text/text_embedding_base.py
+-rw-r--r--   0        0        0     1178 2024-05-03 16:37:04.477064 fastembed-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 fastembed-0.2.7/PKG-INFO
```

### Comparing `fastembed-0.2.6/LICENSE` & `fastembed-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.6/README.md` & `fastembed-0.2.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # ⚡️ What is FastEmbed?
 
 FastEmbed is a lightweight, fast, Python library built for embedding generation. We [support popular text models](https://qdrant.github.io/fastembed/examples/Supported_Models/). Please [open a GitHub issue](https://github.com/qdrant/fastembed/issues/new) if you want us to add a new model.
 
-The default text embedding (`TextEmbedding`) model is Flag Embedding, presented in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/examples/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/examples/Usage_With_Qdrant/).
+The default text embedding (`TextEmbedding`) model is Flag Embedding, presented in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/qdrant/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/qdrant/Usage_With_Qdrant/).
 
 ## 📈 Why FastEmbed?
 
 1. Light: FastEmbed is a lightweight library with few external dependencies. We don't require a GPU and don't download GBs of PyTorch dependencies, and instead use the ONNX Runtime. This makes it a great candidate for serverless runtimes like AWS Lambda. 
 
 2. Fast: FastEmbed is designed for speed. We use the ONNX Runtime, which is faster than PyTorch. We also use data-parallelism for encoding large datasets.
 
 3. Accurate: FastEmbed is better than OpenAI Ada-002. We also [supported](https://qdrant.github.io/fastembed/examples/Supported_Models/) an ever expanding set of models, including a few multilingual models.
 
 ## 🚀 Installation
 
-To install the FastEmbed library, pip works:
+To install the FastEmbed library, pip works best. You can install it with or without GPU support:
 
 ```bash
 pip install fastembed
 ```
 
+### ⚡️ With GPU
+
+```bash
+pip install fastembed-gpu
+```
+
 ## 📖 Quickstart
 
 ```python
 from fastembed import TextEmbedding
 from typing import List
 
 # Example list of documents
@@ -38,23 +44,46 @@
 
 embeddings_generator = embedding_model.embed(documents)  # reminder this is a generator
 embeddings_list = list(embedding_model.embed(documents))
   # you can also convert the generator to a list, and that to a numpy array
 len(embeddings_list[0]) # Vector of 384 dimensions
 ```
 
+### ⚡️ FastEmbed on a GPU
+
+FastEmbed supports running on GPU devices. It requires installation of the `fastembed-gpu` package.
+Make sure not to have the `fastembed` package installed, as it might interfere with the `fastembed-gpu` package.
+
+```bash
+pip install fastembed-gpu
+``` 
+
+```python
+from fastembed import TextEmbedding
+
+embedding_model = TextEmbedding(model_name="BAAI/bge-small-en-v1.5", providers=["CUDAExecutionProvider"])
+print("The model BAAI/bge-small-en-v1.5 is ready to use on a GPU.")
+
+```
+
 ## Usage with Qdrant
 
 Installation with Qdrant Client in Python:
 
 ```bash
 pip install qdrant-client[fastembed]
 ```
 
-You might have to use ```pip install 'qdrant-client[fastembed]'``` on zsh.
+or 
+
+```bash
+pip install qdrant-client[fastembed-gpu]
+```
+
+You might have to use quotes ```pip install 'qdrant-client[fastembed]'``` on zsh.
 
 ```python
 from qdrant_client import QdrantClient
 
 # Initialize the client
 client = QdrantClient("localhost", port=6333) # For production
 # client = QdrantClient(":memory:") # For small experiments
@@ -81,12 +110,8 @@
 )
 
 search_result = client.query(
     collection_name="demo_collection",
     query_text="This is a query document"
 )
 print(search_result)
-```
-
-#### Similar Work
-
-Ilyas M. wrote about using [FlagEmbeddings with Optimum](https://twitter.com/IlysMoutawwakil/status/1705215192425288017) over CUDA.
+```
```

### Comparing `fastembed-0.2.6/fastembed/common/model_management.py` & `fastembed-0.2.7/fastembed/common/model_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,14 @@
 import requests
 from huggingface_hub import snapshot_download
 from huggingface_hub.utils import RepositoryNotFoundError
 from tqdm import tqdm
 from loguru import logger
 
 
-def locate_model_file(model_dir: Path, file_names: List[str]) -> Path:
-    """
-    Find model path for both TransformerJS style `onnx`  subdirectory structure and direct model weights structure used
-    by Optimum and Qdrant
-    """
-    if not model_dir.is_dir():
-        raise ValueError(f"Provided model path '{model_dir}' is not a directory.")
-
-    for file_name in file_names:
-        file_paths = [path for path in model_dir.rglob(file_name) if path.is_file()]
-
-        if file_paths:
-            return file_paths[0]
-
-    raise ValueError(f"Could not find either of {', '.join(file_names)} in {model_dir}")
-
-
 class ModelManagement:
     @classmethod
     def list_supported_models(cls) -> List[Dict[str, Any]]:
         """Lists the supported models.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing the model information.
@@ -100,29 +83,44 @@
                     if chunk:  # Filter out keep-alive new chunks
                         progress_bar.update(len(chunk))
                         file.write(chunk)
         return output_path
 
     @classmethod
     def download_files_from_huggingface(
-        cls, hf_source_repo: str, cache_dir: Optional[str] = None
+        cls,
+        hf_source_repo: str,
+        cache_dir: Optional[str] = None,
+        extra_patterns: Optional[List[str]] = None,
+        **kwargs,
     ) -> str:
         """
         Downloads a model from HuggingFace Hub.
         Args:
             hf_source_repo (str): Name of the model on HuggingFace Hub, e.g. "qdrant/all-MiniLM-L6-v2-onnx".
             cache_dir (Optional[str]): The path to the cache directory.
+            extra_patterns (Optional[List[str]]): extra patterns to allow in the snapshot download, typically
+                includes the required model files.
         Returns:
             Path: The path to the model directory.
         """
+        allow_patterns = [
+            "config.json",
+            "tokenizer.json",
+            "tokenizer_config.json",
+            "special_tokens_map.json",
+        ]
+        if extra_patterns is not None:
+            allow_patterns.extend(extra_patterns)
 
         return snapshot_download(
             repo_id=hf_source_repo,
-            ignore_patterns=["model.safetensors", "pytorch_model.bin"],
+            allow_patterns=allow_patterns,
             cache_dir=cache_dir,
+            local_files_only=kwargs.get("local_files_only", False),
         )
 
     @classmethod
     def decompress_to_cache(cls, targz_path: str, cache_dir: str):
         """
         Decompresses a .tar.gz file to a cache directory.
 
@@ -171,14 +169,17 @@
         if model_tmp_dir.exists():
             shutil.rmtree(model_tmp_dir)
 
         cache_tmp_dir.mkdir(parents=True, exist_ok=True)
 
         model_tar_gz = Path(cache_dir) / f"{fast_model_name}.tar.gz"
 
+        if model_tar_gz.exists():
+            model_tar_gz.unlink()
+
         cls.download_file_from_gcs(
             source_url,
             output_path=str(model_tar_gz),
         )
 
         cls.decompress_to_cache(targz_path=str(model_tar_gz), cache_dir=str(cache_tmp_dir))
         assert model_tmp_dir.exists(), f"Could not find {model_tmp_dir} in {cache_tmp_dir}"
@@ -186,15 +187,15 @@
         model_tar_gz.unlink()
         # Rename from tmp to final name is atomic
         model_tmp_dir.rename(model_dir)
 
         return model_dir
 
     @classmethod
-    def download_model(cls, model: Dict[str, Any], cache_dir: Path) -> Path:
+    def download_model(cls, model: Dict[str, Any], cache_dir: Path, **kwargs) -> Path:
         """
         Downloads a model from HuggingFace Hub or Google Cloud Storage.
 
         Args:
             model (Dict[str, Any]): The model description.
                 Example:
                 ```
@@ -215,17 +216,25 @@
             Path: The path to the downloaded model directory.
         """
 
         hf_source = model.get("sources", {}).get("hf")
         url_source = model.get("sources", {}).get("url")
 
         if hf_source:
+            extra_patterns = [model["model_file"]]
+            extra_patterns.extend(model.get("additional_files", []))
+
             try:
                 return Path(
-                    cls.download_files_from_huggingface(hf_source, cache_dir=str(cache_dir))
+                    cls.download_files_from_huggingface(
+                        hf_source,
+                        cache_dir=str(cache_dir),
+                        extra_patterns=extra_patterns,
+                        local_files_only=kwargs.get("local_files_only", False),
+                    )
                 )
             except (EnvironmentError, RepositoryNotFoundError, ValueError) as e:
                 logger.error(
                     f"Could not download model from HuggingFace: {e}"
                     "Falling back to other sources."
                 )
```

### Comparing `fastembed-0.2.6/fastembed/common/models.py` & `fastembed-0.2.7/fastembed/common/models.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.6/fastembed/common/onnx_model.py` & `fastembed-0.2.7/fastembed/common/onnx_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import os
 from multiprocessing import get_all_start_methods
 from pathlib import Path
-from typing import Any, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    Sequence,
+)
 
 import numpy as np
 import onnxruntime as ort
 
-from fastembed.common.model_management import locate_model_file
 from fastembed.common.models import load_tokenizer
 from fastembed.common.utils import iter_batch
 from fastembed.parallel_processor import ParallelWorkerPool, Worker
 
+
 # Holds type of the embedding result
 T = TypeVar("T")
 
+OnnxProvider = Union[str, Tuple[str, Dict[Any, Any]]]
+
 
 class OnnxModel(Generic[T]):
     @classmethod
     def _get_worker_class(cls) -> Type["EmbeddingWorker"]:
         raise NotImplementedError("Subclasses must implement this method")
 
     @classmethod
@@ -30,28 +44,43 @@
 
     def _preprocess_onnx_input(self, onnx_input: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
         """
         Preprocess the onnx input.
         """
         return onnx_input
 
-    def load_onnx_model(self, model_dir: Path, threads: Optional[int], max_length: int) -> None:
-        model_path = locate_model_file(model_dir, ["model.onnx", "model_optimized.onnx"])
+    def load_onnx_model(
+        self,
+        model_dir: Path,
+        model_file: str,
+        threads: Optional[int],
+        providers: Optional[Sequence[OnnxProvider]] = None,
+    ) -> None:
+        model_path = model_dir / model_file
 
         # List of Execution Providers: https://onnxruntime.ai/docs/execution-providers
-        onnx_providers = ["CPUExecutionProvider"]
+
+        onnx_providers = ["CPUExecutionProvider"] if providers is None else list(providers)
+        available_providers = ort.get_available_providers()
+        for provider in onnx_providers:
+            # check providers available
+            provider_name = provider if isinstance(provider, str) else provider[0]
+            if provider_name not in available_providers:
+                raise ValueError(
+                    f"Provider {provider_name} is not available. Available providers: {available_providers}"
+                )
 
         so = ort.SessionOptions()
         so.graph_optimization_level = ort.GraphOptimizationLevel.ORT_ENABLE_ALL
 
         if threads is not None:
             so.intra_op_num_threads = threads
             so.inter_op_num_threads = threads
 
-        self.tokenizer = load_tokenizer(model_dir=model_dir, max_length=max_length)
+        self.tokenizer = load_tokenizer(model_dir=model_dir)
         self.model = ort.InferenceSession(
             str(model_path), providers=onnx_providers, sess_options=so
         )
 
     def onnx_embed(self, documents: List[str]) -> Tuple[np.ndarray, np.ndarray]:
         encoded = self.tokenizer.encode_batch(documents)
         input_ids = np.array([e.ids for e in encoded])
```

### Comparing `fastembed-0.2.6/fastembed/common/utils.py` & `fastembed-0.2.7/fastembed/common/utils.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.6/fastembed/embedding.py` & `fastembed-0.2.7/fastembed/embedding.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.6/fastembed/parallel_processor.py` & `fastembed-0.2.7/fastembed/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.6/fastembed/sparse/sparse_embedding_base.py` & `fastembed-0.2.7/fastembed/sparse/sparse_embedding_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         **kwargs,
     ):
         self.model_name = model_name
         self.cache_dir = cache_dir
         self.threads = threads
+        self._local_files_only = kwargs.pop("local_files_only", False)
 
     def embed(
         self,
         documents: Union[str, Iterable[str]],
         batch_size: int = 256,
         parallel: Optional[int] = None,
         **kwargs,
```

### Comparing `fastembed-0.2.6/fastembed/sparse/sparse_text_embedding.py` & `fastembed-0.2.7/fastembed/sparse/sparse_text_embedding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import List, Type, Dict, Any, Union, Iterable, Optional
+from typing import List, Type, Dict, Any, Union, Iterable, Optional, Sequence
 
+from fastembed.common import OnnxProvider
 from fastembed.sparse.sparse_embedding_base import SparseTextEmbeddingBase, SparseEmbedding
 from fastembed.sparse.splade_pp import SpladePP
 
 
 class SparseTextEmbedding(SparseTextEmbeddingBase):
     EMBEDDINGS_REGISTRY: List[Type[SparseTextEmbeddingBase]] = [
         SpladePP,
@@ -38,22 +39,25 @@
         return result
 
     def __init__(
         self,
         model_name: str,
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        providers: Optional[Sequence[OnnxProvider]] = None,
         **kwargs,
     ):
         super().__init__(model_name, cache_dir, threads, **kwargs)
 
         for EMBEDDING_MODEL_TYPE in self.EMBEDDINGS_REGISTRY:
             supported_models = EMBEDDING_MODEL_TYPE.list_supported_models()
             if any(model_name.lower() == model["model"].lower() for model in supported_models):
-                self.model = EMBEDDING_MODEL_TYPE(model_name, cache_dir, threads, **kwargs)
+                self.model = EMBEDDING_MODEL_TYPE(
+                    model_name, cache_dir, threads, providers=providers, **kwargs
+                )
                 return
 
         raise ValueError(
             f"Model {model_name} is not supported in SparseTextEmbedding."
             "Please check the supported models using `SparseTextEmbedding.list_supported_models()`"
         )
```

### Comparing `fastembed-0.2.6/fastembed/sparse/splade_pp.py` & `fastembed-0.2.7/fastembed/sparse/splade_pp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, Type
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, Type, Sequence
 
 import numpy as np
 
-from fastembed.common.onnx_model import EmbeddingWorker, OnnxModel
+from fastembed.common.onnx_model import EmbeddingWorker, OnnxModel, OnnxProvider
 from fastembed.common.utils import define_cache_dir
 from fastembed.sparse.sparse_embedding_base import SparseEmbedding, SparseTextEmbeddingBase
 
 supported_splade_models = [
     {
         "model": "prithvida/Splade_PP_en_v1",
         "vocab_size": 30522,
         "description": "Misspelled version of the model. Retained for backward compatibility. Independent Implementation of SPLADE++ Model for English",
         "size_in_GB": 0.532,
         "sources": {
             "hf": "Qdrant/SPLADE_PP_en_v1",
         },
+        "model_file": "model.onnx",
     },
     {
         "model": "prithivida/Splade_PP_en_v1",
         "vocab_size": 30522,
         "description": "Independent Implementation of SPLADE++ Model for English",
         "size_in_GB": 0.532,
         "sources": {
             "hf": "Qdrant/SPLADE_PP_en_v1",
         },
+        "model_file": "model.onnx",
     },
 ]
 
 
 class SpladePP(SparseTextEmbeddingBase, OnnxModel[SparseEmbedding]):
     @classmethod
     def _post_process_onnx_output(
@@ -57,14 +59,15 @@
         return supported_splade_models
 
     def __init__(
         self,
         model_name: str,
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        providers: Optional[Sequence[OnnxProvider]] = None,
         **kwargs,
     ):
         """
         Args:
             model_name (str): The name of the model to use.
             cache_dir (str, optional): The path to the cache directory.
                                        Can be set using the `FASTEMBED_CACHE_PATH` env variable.
@@ -73,22 +76,27 @@
 
         Raises:
             ValueError: If the model_name is not in the format <org>/<model> e.g. BAAI/bge-base-en.
         """
 
         super().__init__(model_name, cache_dir, threads, **kwargs)
 
-        self.model_name = model_name
-        self._model_description = self._get_model_description(model_name)
+        model_description = self._get_model_description(model_name)
+        cache_dir = define_cache_dir(cache_dir)
 
-        self._cache_dir = define_cache_dir(cache_dir)
-        self._model_dir = self.download_model(self._model_description, self._cache_dir)
-        self._max_length = 512
+        model_dir = self.download_model(
+            model_description, cache_dir, local_files_only=self._local_files_only
+        )
 
-        self.load_onnx_model(self._model_dir, self.threads, self._max_length)
+        self.load_onnx_model(
+            model_dir=model_dir,
+            model_file=model_description["model_file"],
+            threads=threads,
+            providers=providers,
+        )
 
     def embed(
         self,
         documents: Union[str, Iterable[str]],
         batch_size: int = 256,
         parallel: Optional[int] = None,
         **kwargs,
@@ -106,15 +114,15 @@
                 If None, don't use data-parallel processing, use default onnxruntime threading instead.
 
         Returns:
             List of embeddings, one per document
         """
         yield from self._embed_documents(
             model_name=self.model_name,
-            cache_dir=str(self._cache_dir),
+            cache_dir=str(self.cache_dir),
             documents=documents,
             batch_size=batch_size,
             parallel=parallel,
         )
 
     @classmethod
     def _get_worker_class(cls) -> Type[EmbeddingWorker]:
```

### Comparing `fastembed-0.2.6/fastembed/text/e5_onnx_embedding.py` & `fastembed-0.2.7/fastembed/text/e5_onnx_embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,26 @@
         "dim": 1024,
         "description": "Multilingual model, e5-large. Recommend using this model for non-English languages",
         "size_in_GB": 2.24,
         "sources": {
             "url": "https://storage.googleapis.com/qdrant-fastembed/fast-multilingual-e5-large.tar.gz",
             "hf": "qdrant/multilingual-e5-large-onnx",
         },
+        "model_file": "model.onnx",
+        "additional_files": ["model.onnx_data"],
     },
     {
         "model": "sentence-transformers/paraphrase-multilingual-mpnet-base-v2",
         "dim": 768,
         "description": "Sentence-transformers model for tasks like clustering or semantic search",
         "size_in_GB": 1.00,
         "sources": {
             "hf": "xenova/paraphrase-multilingual-mpnet-base-v2",
         },
+        "model_file": "onnx/model.onnx",
     },
 ]
 
 
 class E5OnnxEmbedding(OnnxTextEmbedding):
     @classmethod
     def _get_worker_class(cls) -> Type["EmbeddingWorker"]:
```

### Comparing `fastembed-0.2.6/fastembed/text/jina_onnx_embedding.py` & `fastembed-0.2.7/fastembed/text/jina_onnx_embedding.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 supported_jina_models = [
     {
         "model": "jinaai/jina-embeddings-v2-base-en",
         "dim": 768,
         "description": "English embedding model supporting 8192 sequence length",
         "size_in_GB": 0.52,
         "sources": {"hf": "xenova/jina-embeddings-v2-base-en"},
+        "model_file": "onnx/model.onnx",
     },
     {
         "model": "jinaai/jina-embeddings-v2-small-en",
         "dim": 512,
         "description": "English embedding model supporting 8192 sequence length",
         "size_in_GB": 0.12,
         "sources": {"hf": "xenova/jina-embeddings-v2-small-en"},
+        "model_file": "onnx/model.onnx",
     },
 ]
 
 
 class JinaOnnxEmbedding(OnnxTextEmbedding):
     @classmethod
     def _get_worker_class(cls) -> Type[EmbeddingWorker]:
```

### Comparing `fastembed-0.2.6/fastembed/text/text_embedding.py` & `fastembed-0.2.7/fastembed/text/text_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Any, Dict, Iterable, List, Optional, Type, Union
+from typing import Any, Dict, Iterable, List, Optional, Type, Union, Sequence
 
 import numpy as np
 
+from fastembed.common import OnnxProvider
 from fastembed.text.e5_onnx_embedding import E5OnnxEmbedding
 from fastembed.text.jina_onnx_embedding import JinaOnnxEmbedding
 from fastembed.text.onnx_embedding import OnnxTextEmbedding
 from fastembed.text.text_embedding_base import TextEmbeddingBase
 
 
 class TextEmbedding(TextEmbeddingBase):
@@ -45,22 +46,25 @@
         return result
 
     def __init__(
         self,
         model_name: str = "BAAI/bge-small-en-v1.5",
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
+        providers: Optional[Sequence[OnnxProvider]] = None,
         **kwargs,
     ):
         super().__init__(model_name, cache_dir, threads, **kwargs)
 
         for EMBEDDING_MODEL_TYPE in self.EMBEDDINGS_REGISTRY:
             supported_models = EMBEDDING_MODEL_TYPE.list_supported_models()
             if any(model_name.lower() == model["model"].lower() for model in supported_models):
-                self.model = EMBEDDING_MODEL_TYPE(model_name, cache_dir, threads, **kwargs)
+                self.model = EMBEDDING_MODEL_TYPE(
+                    model_name, cache_dir, threads, providers=providers, **kwargs
+                )
                 return
 
         raise ValueError(
             f"Model {model_name} is not supported in TextEmbedding."
             "Please check the supported models using `TextEmbedding.list_supported_models()`"
         )
```

### Comparing `fastembed-0.2.6/fastembed/text/text_embedding_base.py` & `fastembed-0.2.7/fastembed/text/text_embedding_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         cache_dir: Optional[str] = None,
         threads: Optional[int] = None,
         **kwargs,
     ):
         self.model_name = model_name
         self.cache_dir = cache_dir
         self.threads = threads
+        self._local_files_only = kwargs.pop("local_files_only", False)
 
     def embed(
         self,
         documents: Union[str, Iterable[str]],
         batch_size: int = 256,
         parallel: Optional[int] = None,
         **kwargs,
```

### Comparing `fastembed-0.2.6/pyproject.toml` & `fastembed-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastembed"
-version = "0.2.6"
+version = "0.2.7"
 description = "Fast, light, accurate library built for retrieval embedding generation"
 authors = ["NirantK <nirant.bits@gmail.com>"]
 license = "Apache License"
 readme = "README.md"
 packages = [{include = "fastembed"}]
 homepage = "https://github.com/qdrant/fastembed"
 repository = "https://github.com/qdrant/fastembed"
@@ -12,15 +12,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<3.13"
 onnx = "^1.15.0"
 onnxruntime = "^1.17.0"
 tqdm = "^4.66"
 requests = "^2.31"
-tokenizers = "^0.15.1"
+tokenizers = "^0.15"
 huggingface-hub = "^0.20"
 loguru = "^0.7.2"
 numpy = [
     { version = ">=1.21", python = "<3.12" },
     { version = ">=1.26", python = ">=3.12" }
 ]
```

### Comparing `fastembed-0.2.6/PKG-INFO` & `fastembed-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastembed
-Version: 0.2.6
+Version: 0.2.7
 Summary: Fast, light, accurate library built for retrieval embedding generation
 Home-page: https://github.com/qdrant/fastembed
 License: Apache License
 Keywords: vector,embedding,neural,search,qdrant,sentence-transformers
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8.0,<3.13
@@ -18,41 +18,47 @@
 Requires-Dist: huggingface-hub (>=0.20,<0.21)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: numpy (>=1.21) ; python_version < "3.12"
 Requires-Dist: numpy (>=1.26) ; python_version >= "3.12"
 Requires-Dist: onnx (>=1.15.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.17.0,<2.0.0)
 Requires-Dist: requests (>=2.31,<3.0)
-Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
+Requires-Dist: tokenizers (>=0.15,<0.16)
 Requires-Dist: tqdm (>=4.66,<5.0)
 Project-URL: Repository, https://github.com/qdrant/fastembed
 Description-Content-Type: text/markdown
 
 # ⚡️ What is FastEmbed?
 
 FastEmbed is a lightweight, fast, Python library built for embedding generation. We [support popular text models](https://qdrant.github.io/fastembed/examples/Supported_Models/). Please [open a GitHub issue](https://github.com/qdrant/fastembed/issues/new) if you want us to add a new model.
 
-The default text embedding (`TextEmbedding`) model is Flag Embedding, presented in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/examples/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/examples/Usage_With_Qdrant/).
+The default text embedding (`TextEmbedding`) model is Flag Embedding, presented in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/qdrant/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/qdrant/Usage_With_Qdrant/).
 
 ## 📈 Why FastEmbed?
 
 1. Light: FastEmbed is a lightweight library with few external dependencies. We don't require a GPU and don't download GBs of PyTorch dependencies, and instead use the ONNX Runtime. This makes it a great candidate for serverless runtimes like AWS Lambda. 
 
 2. Fast: FastEmbed is designed for speed. We use the ONNX Runtime, which is faster than PyTorch. We also use data-parallelism for encoding large datasets.
 
 3. Accurate: FastEmbed is better than OpenAI Ada-002. We also [supported](https://qdrant.github.io/fastembed/examples/Supported_Models/) an ever expanding set of models, including a few multilingual models.
 
 ## 🚀 Installation
 
-To install the FastEmbed library, pip works:
+To install the FastEmbed library, pip works best. You can install it with or without GPU support:
 
 ```bash
 pip install fastembed
 ```
 
+### ⚡️ With GPU
+
+```bash
+pip install fastembed-gpu
+```
+
 ## 📖 Quickstart
 
 ```python
 from fastembed import TextEmbedding
 from typing import List
 
 # Example list of documents
@@ -67,23 +73,46 @@
 
 embeddings_generator = embedding_model.embed(documents)  # reminder this is a generator
 embeddings_list = list(embedding_model.embed(documents))
   # you can also convert the generator to a list, and that to a numpy array
 len(embeddings_list[0]) # Vector of 384 dimensions
 ```
 
+### ⚡️ FastEmbed on a GPU
+
+FastEmbed supports running on GPU devices. It requires installation of the `fastembed-gpu` package.
+Make sure not to have the `fastembed` package installed, as it might interfere with the `fastembed-gpu` package.
+
+```bash
+pip install fastembed-gpu
+``` 
+
+```python
+from fastembed import TextEmbedding
+
+embedding_model = TextEmbedding(model_name="BAAI/bge-small-en-v1.5", providers=["CUDAExecutionProvider"])
+print("The model BAAI/bge-small-en-v1.5 is ready to use on a GPU.")
+
+```
+
 ## Usage with Qdrant
 
 Installation with Qdrant Client in Python:
 
 ```bash
 pip install qdrant-client[fastembed]
 ```
 
-You might have to use ```pip install 'qdrant-client[fastembed]'``` on zsh.
+or 
+
+```bash
+pip install qdrant-client[fastembed-gpu]
+```
+
+You might have to use quotes ```pip install 'qdrant-client[fastembed]'``` on zsh.
 
 ```python
 from qdrant_client import QdrantClient
 
 # Initialize the client
 client = QdrantClient("localhost", port=6333) # For production
 # client = QdrantClient(":memory:") # For small experiments
@@ -111,12 +140,7 @@
 
 search_result = client.query(
     collection_name="demo_collection",
     query_text="This is a query document"
 )
 print(search_result)
 ```
-
-#### Similar Work
-
-Ilyas M. wrote about using [FlagEmbeddings with Optimum](https://twitter.com/IlysMoutawwakil/status/1705215192425288017) over CUDA.
-
```

