# Comparing `tmp/easy_llama-0.1.7.tar.gz` & `tmp/easy_llama-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_llama-0.1.7.tar", last modified: Thu May  2 16:23:46 2024, max compression
+gzip compressed data, was "easy_llama-0.1.8.tar", last modified: Thu May  2 19:06:08 2024, max compression
```

## Comparing `easy_llama-0.1.7.tar` & `easy_llama-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 16:23:46.868368 easy_llama-0.1.7/
--rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.7/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 16:23:46.868135 easy_llama-0.1.7/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)    13907 2024-05-02 15:43:35.000000 easy_llama-0.1.7/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 16:23:46.867113 easy_llama-0.1.7/easy_llama/
--rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 15:55:14.000000 easy_llama-0.1.7/easy_llama/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.7/easy_llama/formats.py
--rw-r--r--   0 dylan      (501) staff       (20)    24184 2024-05-02 15:54:29.000000 easy_llama-0.1.7/easy_llama/model.py
--rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.7/easy_llama/samplers.py
--rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.7/easy_llama/thread.py
--rw-r--r--   0 dylan      (501) staff       (20)     4705 2024-05-02 15:54:04.000000 easy_llama-0.1.7/easy_llama/utils.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 16:23:46.867951 easy_llama-0.1.7/easy_llama.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-02 16:23:46.868413 easy_llama-0.1.7/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1267 2024-05-02 15:55:17.000000 easy_llama-0.1.7/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 19:06:08.375815 easy_llama-0.1.8/
+-rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.8/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 19:06:08.375590 easy_llama-0.1.8/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)    13907 2024-05-02 15:43:35.000000 easy_llama-0.1.8/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 19:06:08.374629 easy_llama-0.1.8/easy_llama/
+-rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 19:00:17.000000 easy_llama-0.1.8/easy_llama/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.8/easy_llama/formats.py
+-rw-r--r--   0 dylan      (501) staff       (20)    25103 2024-05-02 19:00:07.000000 easy_llama-0.1.8/easy_llama/model.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.8/easy_llama/samplers.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.8/easy_llama/thread.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4705 2024-05-02 15:54:04.000000 easy_llama-0.1.8/easy_llama/utils.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 19:06:08.375387 easy_llama-0.1.8/easy_llama.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-02 19:06:08.000000 easy_llama-0.1.8/easy_llama.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-02 19:06:08.375860 easy_llama-0.1.8/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1267 2024-05-02 19:00:22.000000 easy_llama-0.1.8/setup.py
```

### Comparing `easy_llama-0.1.7/LICENSE` & `easy_llama-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.7/PKG-INFO` & `easy_llama-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.7
+Version: 0.1.8
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.7/README.md` & `easy_llama-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.7/easy_llama/formats.py` & `easy_llama-0.1.8/easy_llama/formats.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.7/easy_llama/model.py` & `easy_llama-0.1.8/easy_llama/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,42 +58,47 @@
 
     def __init__(
             self,
             model_path: str,
             context_length: Optional[int] = None,
             n_gpu_layers: int = 0,
             offload_kqv: bool = True,
+            flash_attn: bool = False,
             verbose: bool = False
         ):
         """
         Given the path to a GGUF file, construct a Model instance.
 
         The model must be in GGUF format.
 
         The following parameters are optional:
         - context_length: The context length at which to load the model, in tokens
         - n_gpu_layers: The number of layers to be offloaded to the GPU
         - offload_kqv: Whether or not the KQV cache (context) should be offloaded
+        - flash_attn: Whether or not to use Flash Attention (experimental)
         - verbose: Whether or not to print additional backend information
         """
 
         assert isinstance(model_path, str), \
             f"Model: model_path should be a string, not {type(model_path)}"
         assert exists(model_path), \
             f"Model: the given model_path '{model_path}' does not exist"
         assert not isdir(model_path), \
             f"Model: the given model_path '{model_path}' is a directory, not a GGUF file"
         assert isinstance(context_length, (int, type(None))), \
             f"Model: context_length should be int or None, not {type(context_length)}"
+        assert isinstance(flash_attn, bool), \
+            f"Model: flash_attn should be bool (True or False), not {type(flash_attn)}"
         
         # save __init__ parameters for __repr__
         self._model_path = model_path
         self._context_length = context_length
         self._n_gpu_layers = n_gpu_layers
         self._offload_kqv = offload_kqv
+        self._flash_attn = flash_attn
         self._verbose = self.verbose = verbose
 
         # if context_length <= 0, use n_ctx_train
         if isinstance(context_length, int) and context_length <= 0:
             context_length = None
 
         # this does not use Llama.metadata because we want to use GGUF
@@ -167,19 +172,14 @@
 
             elif context_length/n_ctx_train >= 8:
                 print_warning(
                     'loading model with 8x native context length or more, ' + \
                     'expect SIGNIFICANT loss of quality'
                 )
         
-        # expose these values because they may be useful / informative
-        self.n_ctx_train = n_ctx_train
-        self.rope_freq_base_train = rope_freq_base_train
-        self.rope_freq_base = rope_freq_base
-        
         try:
             self.tokens: List[str] = self.metadata['tokenizer.ggml.tokens']
         except KeyError:
             print_warning(
                 "could not set Model.tokens, defaulting to None"
             )
             self.tokens = None
@@ -202,57 +202,80 @@
 
         # these values for n_threads and n_threads_batch are
         # known to be optimal for most systems
         n_batch = 512 # can this be optimized?
         n_threads = max(cpu_count//2, 1)
         n_threads_batch = cpu_count
 
+        if flash_attn:
+            if n_gpu_layers == 0:
+                print_warning(
+                    "disabling flash_attn because n_gpu_layers == 0"
+                )
+                flash_attn = False
+            else:
+                print_warning(
+                    "flash_attn enabled"
+                )
+                print_warning(
+                    "please note that flash_attn is currently experimental"
+                )
+
         self.llama: Llama = Llama(
             model_path=model_path,
             n_ctx=self.context_length,
             n_gpu_layers=n_gpu_layers,
             use_mmap=True,
             use_mlock=False,
             logits_all=False,
             n_batch=n_batch,
             n_threads=n_threads,
             n_threads_batch=n_threads_batch,
             rope_freq_base=rope_freq_base,
             mul_mat_q=True,
             offload_kqv=offload_kqv,
+            flash_attn=flash_attn,
             # KV cache quantization
             # use 1 for F16 (default), 8 for q8_0, 2 for q4_0, 3 for q4_1
             #type_k=8,
             #type_v=8,
             verbose=verbose
         )
         
         # once model is loaded, replace metadata (as read using internal class)
         # with metadata (as read using the more robust llama-cpp-python code) 
         self.metadata = self.llama.metadata
 
+        # expose these values because they may be useful / informative
+        self.n_ctx_train = n_ctx_train
+        self.rope_freq_base_train = rope_freq_base_train
+        self.rope_freq_base = rope_freq_base
+        self.flash_attn = flash_attn
+
         if self.verbose:
             print_verbose("new Model instance with the following attributes:")
             print_verbose(f"model: {model_path}")
             print_verbose(f"param: n_gpu_layers         == {n_gpu_layers}")
             print_verbose(f"param: offload_kqv          == {offload_kqv}")
+            print_verbose(f"param: flash_attn           == {flash_attn}")
             print_verbose(f"param: n_batch              == {n_batch}")
             print_verbose(f"param: n_threads            == {n_threads}")
             print_verbose(f"param: n_threads_batch      == {n_threads_batch}")
             print_verbose(f" gguf: n_ctx_train          == {n_ctx_train}")
             print_verbose(f"param: self.context_length  == {self.context_length}")
             print_verbose(f" gguf: rope_freq_base_train == {rope_freq_base_train}")
             print_verbose(f"param: rope_freq_base       == {rope_freq_base}")
     
     def __repr__(self) -> str:
         return \
             f"Model({repr(self._model_path)}, " + \
             f"context_length={self._context_length}, " + \
             f"n_gpu_layers={self._n_gpu_layers}, " + \
             f"offload_kqv={self._offload_kqv}, "+ \
+            f"flash_attn={self._flash_attn}, " + \
             f"verbose={self._verbose})"
 
     def __del__(self):
         self.unload()
     
     def __enter__(self):
         return self
```

### Comparing `easy_llama-0.1.7/easy_llama/samplers.py` & `easy_llama-0.1.8/easy_llama/samplers.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.7/easy_llama/thread.py` & `easy_llama-0.1.8/easy_llama/thread.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.7/easy_llama/utils.py` & `easy_llama-0.1.8/easy_llama/utils.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.7/easy_llama.egg-info/PKG-INFO` & `easy_llama-0.1.8/easy_llama.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.7
+Version: 0.1.8
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.7/setup.py` & `easy_llama-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # easy_llama.py
 # https://github.com/ddh0/easy-llama/
 
 from setuptools import setup
 
 setup(
     name='easy_llama',
-    version='0.1.7',
+    version='0.1.8',
     description='Text generation in Python, made easy',
     long_description="""To view the current documentation for easy-llama, visit the project's GitHub repository:\nhttps://github.com/ddh0/easy-llama""",
     url='https://github.com/ddh0/easy-llama/',
     author='Dylan Halladay',
     author_email='dylanhalladay02@icloud.com',
     license='The Unlicense',
     packages=['easy_llama'],
```

