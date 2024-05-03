# Comparing `tmp/sdeper-1.2.0.tar.gz` & `tmp/sdeper-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeper-1.2.0.tar", last modified: Sun Apr 28 05:24:34 2024, max compression
+gzip compressed data, was "sdeper-1.2.1.tar", last modified: Fri May  3 02:57:10 2024, max compression
```

## Comparing `sdeper-1.2.0.tar` & `sdeper-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:34.496528 sdeper-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-28 05:24:26.000000 sdeper-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-28 05:24:26.000000 sdeper-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-28 05:24:34.496528 sdeper-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-28 05:24:26.000000 sdeper-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-28 05:24:26.000000 sdeper-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 05:24:26.000000 sdeper-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:24:34.496528 sdeper-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-28 05:24:26.000000 sdeper-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:34.496528 sdeper-1.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/admm_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44389 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/cvae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/cvaeglrm.py
--rw-r--r--   0 runner    (1001) docker     (127)    23811 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/diagnosis_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/hyper_parameter_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/imputation.py
--rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/local_fit_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    52767 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/parse_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/run_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:24:34.496528 sdeper-1.2.0/src/sdeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-28 05:24:34.000000 sdeper-1.2.0/src/sdeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23236 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 05:24:26.000000 sdeper-1.2.0/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:57:10.102728 sdeper-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 02:56:59.000000 sdeper-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 02:56:59.000000 sdeper-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-03 02:57:10.102728 sdeper-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-03 02:56:59.000000 sdeper-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 02:56:59.000000 sdeper-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 02:56:59.000000 sdeper-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:57:10.102728 sdeper-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-03 02:56:59.000000 sdeper-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:57:10.102728 sdeper-1.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/admm_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45857 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/cvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/cvaeglrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30905 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/diagnosis_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/hyper_parameter_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49987 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/local_fit_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19609 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55558 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/parse_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/run_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:57:10.102728 sdeper-1.2.1/src/sdeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 02:57:09.000000 sdeper-1.2.1/src/sdeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23397 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 02:56:59.000000 sdeper-1.2.1/src/version.py
```

### Comparing `sdeper-1.2.0/LICENSE` & `sdeper-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/PKG-INFO` & `sdeper-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.12
+Requires-Python: >=3.9.12, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.22.4
 Requires-Dist: scipy==1.8.1
 Requires-Dist: pandas==1.4.3
 Requires-Dist: networkx==2.8.4
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: scikit-learn==1.1.1
@@ -28,20 +28,22 @@
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: umap-learn==0.5.3
 Requires-Dist: distinctipy==1.2.2
 Requires-Dist: reportlab==4.1.0
 Requires-Dist: opencv-python==4.6.0.66
 
 # SDePER
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
+![OS](https://img.shields.io/badge/os-linux-blue) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
 
+SDePER currently supports only Linux operating systems such as Ubuntu, and is compatible with Python versions 3.9.12 up to but not including 3.11.
+
 SDePER can be installed via conda
 
 ```bash
 conda create -n sdeper-env -c bioconda -c conda-forge python=3.9.12 sdeper
 ```
 
 or pip
```

### Comparing `sdeper-1.2.0/README.md` & `sdeper-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SDePER
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
+![OS](https://img.shields.io/badge/os-linux-blue) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
 
+SDePER currently supports only Linux operating systems such as Ubuntu, and is compatible with Python versions 3.9.12 up to but not including 3.11.
+
 SDePER can be installed via conda
 
 ```bash
 conda create -n sdeper-env -c bioconda -c conda-forge python=3.9.12 sdeper
 ```
 
 or pip
```

### Comparing `sdeper-1.2.0/setup.py` & `sdeper-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     name = "sdeper",    # short and all lower case
     version = cur_version,
     author = "Ningshan Li",
     author_email = "hill103.2@gmail.com",
     description = "Spatial Deconvolution method with Platform Effect Removal",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    python_requires = ">=3.9.12",    # Minimum Python version
+    python_requires = ">=3.9.12, <3.11",    # Specifies Python version support
     install_requires = requirements,    # Dependencies
     license_files = "LICENSE",    # license file will be include in top-level automatically (failed, specify it in MANIFEST.in)
     package_dir = {"": "src"},    # py files are in src folder
     # no need to specify 'packages=' since we only have one 'package' corresonding to the src folder
     # also no need to specify 'py_modules=', all py files under src folder will be recognized as modules
     # we need to include two non-python files
     # one way is include_package_data=True + MANIFEST.in, which can make sure the file is in top-level
```

### Comparing `sdeper-1.2.0/src/admm_fit.py` & `sdeper-1.2.1/src/admm_fit.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/config.py` & `sdeper-1.2.1/src/config.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/cvae.py` & `sdeper-1.2.1/src/cvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,15 +432,15 @@
     
     new_decoder = build_new_decoder(p, p_cond, latent_dim, p_decoder_lst, hidden_act, output_act, use_batch_norm)
     
     return cvae, new_decoder
 
 
 
-def build_CVAE(spatial_df, scRNA_df, scRNA_celltype, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, rerun_DE=True, filter_gene=True):
+def build_CVAE(spatial_df, scRNA_df, scRNA_celltype, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, rerun_DE=True, filter_gene=True):
     '''
     build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
     
     input gene expression in datasets only included genes needed for downstream analysis and already been normalized by sequencing depth
 
     Parameters
     ----------
@@ -462,14 +462,20 @@
         a scaler of scRNA-seq sequencing depth.
     cvae_input_scaler : int
         maximum value of the scaled input for CVAE.
     cvae_init_lr : float
         initial learning rate for training CVAE.
     num_hidden_layer : int
         number of hidden layers in encoder and decoder.
+    use_batch_norm : bool
+        whether to use Batch Normalization.
+    cvae_train_epoch : int
+        max number of training epochs for the CVAE.
+    use_spatial_pseudo : int
+        whether to generate "pseudo-spots" in spatial condition.
     use_fdr : bool
         whether to use FDR adjusted p value for filtering and sorting.
     p_val_cutoff : float
         threshold of p value (or FDR if --use_fdr is true) in marker genes filtering.
     fc_cutoff : float
         threshold of fold change (without log transform!) in marker genes filtering.
     pct1_cutoff : float
@@ -495,14 +501,22 @@
     new_markers : list or None
         marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE (rerun_DE=False).
     '''
     
     assert((scRNA_df.index == scRNA_celltype.index).all())
     assert((spatial_df.columns == scRNA_df.columns).all())
     
+    
+    if diagnosis:
+        # first plot UMAP for raw input gene expressions
+        from diagnosis_plots import defineColor, rawInputUMAP
+        plot_colors = defineColor(spatial_df.shape[0], scRNA_celltype)
+        rawInputUMAP(spatial_df, scRNA_df, scRNA_celltype, plot_colors)
+        
+    
     # some settings
     # max number of pseudo spots (training+validation, without training single cells)
     n_max_pseudo_spots = n_pseudo_spot
     # scaler to multiply the normalized gene values and transform back to raw nUMI counts
     depth_scaler = seq_depth_scaler
     # percentage of training pseudo spots
     training_pct = 0.8
@@ -529,15 +543,18 @@
     pseudo_spots_df, pseudo_spots_celltype_prop, n_cell_in_spot = generate_pseudo_spots(scRNA_df, scRNA_celltype, n_spot_scrna, celltype_order, pseudo_spot_min_cell, pseudo_spot_max_cell)
     
     # convert scRNA-seq cell-type annotation to proportions
     scrna_cell_celltype_prop = celltype2props(scRNA_celltype, celltype_order)
     
     
     # generate pseudo-spots by combining spatial spots
-    n_spot_spatial = int(0.5 * n_spot_scrna)
+    if use_spatial_pseudo:
+        n_spot_spatial = int(0.5 * n_spot_scrna)
+    else:
+        n_spot_spatial = 0
     n_train_spot_spatial = int(np.floor(n_spot_spatial * training_pct))
     n_valid_spot_spatial = int(n_spot_spatial - n_train_spot_spatial)
     print(f'generate {n_spot_spatial} pseudo-spots containing 2 to 6 spots from spatial spots...')
     pseudo_spatial_df = combine_spatial_spots(spatial_df, n_spot_spatial, 2, 6)
     
     
     if use_log_transform:
@@ -625,57 +642,70 @@
     hidden_dim = list(np.floor(np.geomspace(latent_dim, p, num_hidden_layer+2)[1:num_hidden_layer+1]).astype('int'))
     
     print('\nCVAE structure:')
     print(f'Encoder: {" - ".join([str(x) for x in ([p+p_cond] + hidden_dim[::-1] + [latent_dim])])}')
     print(f'Decoder: {" - ".join([str(x) for x in ([latent_dim+p_cond] + hidden_dim + [p])])}\n')
     
     # note hidden layer in encoder is a reverse of the hidden_dim variable
-    cvae, new_decoder = CVAE_keras_model(p, p_cond, latent_dim, hidden_dim[::-1], hidden_dim, use_batch_norm=True, cvae_init_lr=cvae_init_lr)
+    cvae, new_decoder = CVAE_keras_model(p, p_cond, latent_dim, hidden_dim[::-1], hidden_dim, use_batch_norm=use_batch_norm, cvae_init_lr=cvae_init_lr)
     
     # learning rate decay
     lrate = ReduceLROnPlateau(monitor='val_loss', factor=0.9, patience=10, min_lr=5e-4, cooldown=5, verbose=False)
     
     # early stopping based on validation loss
     early_stop = EarlyStopping(monitor='val_loss', min_delta=0, patience=30, restore_best_weights=True, verbose=False)
     
     
     # change tensorflow seed value, set the same seed value for sampling samples from latent space to decoder before training
     # still has unknown randomness source even set seed here...
     set_random_seed(1154)
     
+    # if not use Batch Normalization, we use all training data for one epoch
+    if use_batch_norm:
+        one_batch_size = 16384
+        do_shuffle = True
+    else:
+        one_batch_size = data.shape[0]
+        do_shuffle = False
+    
     # Train CVAE
     # note when there is no pseudo-spots, then there is no validation data
     if valid_data.shape[0] == 0:
         print('\nStart training without validation data...\n')
         history_callback = cvae.fit([data, labels], data,
-                                epochs=500,
-                                batch_size=16384,
-                                shuffle=True,
+                                epochs=cvae_train_epoch,
+                                batch_size=one_batch_size,
+                                shuffle=do_shuffle,
                                 callbacks=[lrate, early_stop],
                                 sample_weight=sample_weight,
                                 verbose=True)
     else:
          print('\nStart training...\n')
          history_callback = cvae.fit([data, labels], data,
                                 validation_data=([valid_data, valid_labels], valid_data),
-                                epochs=500,
-                                batch_size=16384,
-                                shuffle=True,
+                                epochs=cvae_train_epoch,
+                                batch_size=one_batch_size,
+                                shuffle=do_shuffle,
                                 callbacks=[lrate, early_stop],
                                 sample_weight=sample_weight,
                                 verbose=True)
     
     n_epoch = len(history_callback.history['loss'])
     
-    if n_epoch < 500:
+    if n_epoch < cvae_train_epoch:
         print(f'\ntraining finished in {n_epoch} epochs (early stop), transform data to adjust the platform effect...\n')
     else:
         print(f'\ntraining finished in {n_epoch} epochs (reach max pre-specified epoches), transform data to adjust the platform effect...\n')
 
-    
+    if diagnosis:
+        # plot loss
+        from diagnosis_plots import plotCVAELoss
+        plotCVAELoss(history_callback)
+
+
     # postprocess the trained models
     # Subset the encoder
     encoder = Model([cvae.get_layer('encoder_input').input, cvae.get_layer('cond_input').input],
                     [cvae.get_layer('z_mean').output, cvae.get_layer('z_log_var').output],
                     name='encoder')
     
     # update layer weights for the decoder
@@ -756,24 +786,24 @@
         
         
         from diagnosis_plots import diagnosisCVAE
         diagnosisCVAE(cvae, encoder, new_decoder,
                       spatial_embed, spatial_transformed_df, spatial_transformed_numi, pseudo_spatial_embed,
                       scRNA_celltype, celltype_order, celltype_count_dict, scrna_cell_celltype_prop, scRNA_embed,
                       pseudo_spots_celltype_prop, n_cell_in_spot, pseudo_spot_embed,
-                      scRNA_decode_df, scRNA_decode_avg_df, new_markers)
+                      scRNA_decode_df, scRNA_decode_avg_df, new_markers, plot_colors)
 
 
     #print(f'before CVAE building function return RAM usage: {psutil.Process().memory_info().rss/1024**2:.2f} MB')
     
     return spatial_transformed_numi, scRNA_decode_avg_df, new_markers
 
 
 
-def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene):
+def build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene):
     '''
     read related CSV files, build CVAE to adjust platform effect, return transformed spatial gene expression and scRNA-seq cell-type gene signature
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
@@ -797,14 +827,20 @@
         a scaler of scRNA-seq sequencing depth.
     cvae_input_scaler : int
         maximum value of the scaled input for CVAE.
     cvae_init_lr : float
         initial learning rate for training CVAE.
     num_hidden_layer : int
         number of hidden layers in encoder and decoder.
+    use_batch_norm : bool
+        whether to use Batch Normalization.
+    cvae_train_epoch : int
+        max number of training epochs for the CVAE.
+    use_spatial_pseudo : int
+        whether to generate "pseudo-spots" in spatial condition.
     redo_de : bool
         whether to redo DE after CVAE transformation.
     use_fdr : bool
         whether to use FDR adjusted p value for filtering and sorting.
     p_val_cutoff : float
         threshold of p value (or FDR if --use_fdr is true) in marker genes filtering.
     fc_cutoff : float
@@ -902,14 +938,14 @@
     # build CVAE
     (spatial_transformed_numi,
      scRNA_decode_avg_df,
      new_markers) = build_CVAE(sc.get.obs_df(spatial_spot_obj, keys=final_gene_list),
                                sc.get.obs_df(scrna_obj, keys=final_gene_list),
                                scrna_celltype,
                                n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler,
-                               cvae_input_scaler, cvae_init_lr, num_hidden_layer,
+                               cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo,
                                use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc,
                                diagnosis, rerun_DE=redo_de, filter_gene=filter_gene)
     
     print(f'\nplatform effect adjustment by CVAE finished. Elapsed time: {(time()-start_time)/60.0:.2f} minutes.\n\n')
     
     return spatial_transformed_numi, scRNA_decode_avg_df, new_markers
```

### Comparing `sdeper-1.2.0/src/cvaeglrm.py` & `sdeper-1.2.1/src/cvaeglrm.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
     session_conf = tf.compat.v1.ConfigProto(intra_op_parallelism_threads=paramdict['n_cores'], inter_op_parallelism_threads=paramdict['n_cores'])
     sess = tf.compat.v1.Session(graph=tf.compat.v1.get_default_graph(), config=session_conf)
     tf.compat.v1.keras.backend.set_session(sess)
     
     
     print('\n\n######### Preprocessing... #########\n')
-    data = preprocess(paramdict['spatial_file'], paramdict['ref_file'], paramdict['ref_celltype_file'], paramdict['marker_file'], paramdict['A_file'], paramdict['use_cvae'], paramdict['n_hv_gene'], paramdict['n_marker_per_cmp'], paramdict['n_pseudo_spot'], paramdict['pseudo_spot_min_cell'], paramdict['pseudo_spot_max_cell'], paramdict['seq_depth_scaler'], paramdict['cvae_input_scaler'], paramdict['cvae_init_lr'], paramdict['num_hidden_layer'], paramdict['redo_de'], paramdict['use_fdr'], paramdict['p_val_cutoff'], paramdict['fc_cutoff'], paramdict['pct1_cutoff'], paramdict['pct2_cutoff'], paramdict['sortby_fc'], paramdict['filter_cell'], paramdict['filter_gene'], paramdict['diagnosis'])
+    data = preprocess(paramdict['spatial_file'], paramdict['ref_file'], paramdict['ref_celltype_file'], paramdict['marker_file'], paramdict['A_file'], paramdict['use_cvae'], paramdict['n_hv_gene'], paramdict['n_marker_per_cmp'], paramdict['n_pseudo_spot'], paramdict['pseudo_spot_min_cell'], paramdict['pseudo_spot_max_cell'], paramdict['seq_depth_scaler'], paramdict['cvae_input_scaler'], paramdict['cvae_init_lr'], paramdict['num_hidden_layer'], paramdict['use_batch_norm'], paramdict['cvae_train_epoch'], paramdict['use_spatial_pseudo'], paramdict['redo_de'], paramdict['use_fdr'], paramdict['p_val_cutoff'], paramdict['fc_cutoff'], paramdict['pct1_cutoff'], paramdict['pct2_cutoff'], paramdict['sortby_fc'], paramdict['filter_cell'], paramdict['filter_gene'], paramdict['diagnosis'])
     
     
     # whether to estimate gamma_g, if CVAE is used then disable gamma_g estimation
     if paramdict['use_cvae']:
         estimate_gamma_g = False
     else:
         estimate_gamma_g = True
```

### Comparing `sdeper-1.2.0/src/diagnosis_plots.py` & `sdeper-1.2.1/src/diagnosis_plots.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,29 +8,203 @@
 We move all functions for generating diagnosis plots to here.
 """
 
 
 
 import os
 from config import print, diagnosis_path
-from tensorflow.keras.utils import plot_model
+#from tensorflow.keras.utils import plot_model
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.colors import Normalize
 import seaborn as sns
 sns.set()
 import umap
 from distinctipy import distinctipy
 from scipy.interpolate import griddata
 
 
 
-def diagnosisCVAE(cvae, encoder, decoder, spatial_embed, spatial_transformed_df, spatial_transformed_numi, pseudo_spatial_embed, scRNA_celltype, celltype_order, celltype_count_dict, scrna_cell_celltype_prop, scRNA_embed, pseudo_spots_celltype_prop, n_cell_in_spot, pseudo_spot_embed, scRNA_decode_df, scRNA_decode_avg_df, new_markers):
+def plotCVAELoss(history):
+    '''
+    plot training and validation loss in CVAE training
+
+    Parameters
+    ----------
+    history : History object
+        History object returned by Keras Model.fit in CVAE training.
+
+    Returns
+    -------
+    None.
+    '''
+    
+    # need to create subfolders first, otherwise got FileNotFoundError
+    os.makedirs(os.path.join(diagnosis_path, 'CVAE_training'), exist_ok=True)
+    
+    
+    # plot total loss
+    plt.figure(figsize=(6.4*2, 4.8*2))
+    plt.plot(history.history['loss'], label='Training')
+    if 'val_loss' in history.history:
+        plt.plot(history.history['val_loss'], label='Validation')
+    plt.ylabel('Total Loss')
+    plt.xlabel('Epoch')
+    plt.legend(loc='upper right')
+    plt.savefig(os.path.join(diagnosis_path, 'CVAE_training', 'CVAE_total_loss_in_training.png'))
+    plt.close()
+    
+    
+    # plot components of loss
+    plt.figure(figsize=(6.4*2, 4.8*2))
+    
+    # Training KL Loss
+    plt.plot(history.history['KL_loss'], color='#1f77b4', marker='o', label='Training KL Loss')
+    # Validation KL Loss
+    plt.plot(history.history['val_KL_loss'], color='#ff7f0e', marker='o', label='Validation KL Loss')
+
+    # Training Reconstruction Loss
+    plt.plot(history.history['reconstruction_loss'], color='#1f77b4', marker='s', linestyle='dashed', label='Training Reconstruction Loss')
+    # Validation Reconstruction Loss
+    plt.plot(history.history['val_reconstruction_loss'], color='#ff7f0e', marker='s', linestyle='dashed', label='Validation Reconstruction Loss')
+    
+    # Adding labels
+    plt.xlabel('Epoch')
+    plt.ylabel('Model Loss')
+    # Add a legend
+    plt.legend(loc='upper right')
+    plt.savefig(os.path.join(diagnosis_path, 'CVAE_training', 'CVAE_loss_components_in_training.png'))
+    plt.close()
+
+
+
+def defineColor(n_spatial_spot, scRNA_celltype):
+    '''
+    generate n visually distinct colours for cell-types. Use these colours across whole pipeline for consistency
+
+    Parameters
+    ----------
+    n_spatial_spot : int
+        number of spatial spots.
+    scRNA_celltype : dataframe
+        cell-type annotations for cells in scRNA-seq data. Only 1 column named <celltype>.
+
+    Returns
+    -------
+    plot_colors : dict
+        generated color palette, keys are cell-types together with the number of cells with this cell-type, and values are RGB colors.
+    '''
+    
+    celltype_order = sorted(list(scRNA_celltype.celltype.unique()))
+    celltype_count_dict = scRNA_celltype.celltype.value_counts().to_dict()
+    
+    plot_colors = {}
+    for one_celltype, one_color in zip([f'spatial ({n_spatial_spot})']+[f'{x} ({celltype_count_dict[x]})' for x in celltype_order], distinctipy.get_colors(len(celltype_order)+1)):
+        plot_colors[one_celltype] = one_color
+    # assign pseudo spots as gray80
+    plot_colors['pseudo'] = '#cccccc'
+    
+    return plot_colors
+
+
+
+def rawInputUMAP(spatial_df, scRNA_df, scRNA_celltype, plot_colors):
+    '''
+    generate UMAP of spatial spots together with scRNA-seq cells
+
+    Parameters
+    ----------
+    spatial_df : dataframe
+        normalized gene expression in spatial transcriptomic data (spots * genes).
+    scRNA_df : dataframe
+        normalized gene expression in scRNA-seq data (cells * genes).
+    scRNA_celltype : dataframe
+        cell-type annotations for cells in scRNA-seq data. Only 1 column named <celltype>.
+    plot_colors : dict
+        color palette for plot.
+
+    Returns
+    -------
+    None.
+    '''
+    
+    assert((scRNA_df.index == scRNA_celltype.index).all())
+    assert((spatial_df.columns == scRNA_df.columns).all())
+    
+    # need to create subfolders first, otherwise got FileNotFoundError
+    os.makedirs(os.path.join(diagnosis_path, 'raw_input_data'), exist_ok=True)
+    
+    celltype_count_dict = scRNA_celltype.celltype.value_counts().to_dict()
+    
+    # take average within cell-types to get cell-type specific marker gene profile
+    scRNA_avg_df = scRNA_df.copy()
+    scRNA_avg_df['celltype'] = scRNA_celltype.celltype
+    scRNA_avg_df = scRNA_avg_df.groupby(['celltype']).mean()
+    
+    # UMAP of raw input spatial and scRNA-seq cell gene expression
+    # we also add marker gene expression profile here
+    # the order will affect the point overlay, first row draw first
+    # umap has embeded seed (default 42), by specify random_state, umap will use special mode to keep reproducibility
+    # note here both gene expressions are sequencing normalized values, without log transform and scaling
+    tmp_df = pd.concat([spatial_df, scRNA_df, scRNA_avg_df], ignore_index=True)
+    
+    all_umap = umap.UMAP(random_state=42).fit_transform(tmp_df.values)
+    
+    # add cell/spot count in the annotation
+    plot_df = pd.DataFrame({'UMAP1': all_umap[:, 0],
+                            'UMAP2': all_umap[:, 1],
+                            'celltype': [f'spatial ({spatial_df.shape[0]})']*spatial_df.shape[0] +
+                                        [f'{x} ({celltype_count_dict[x]})' for x in scRNA_celltype.celltype.to_list()] +
+                                        [f'{x} ({celltype_count_dict[x]})' for x in scRNA_avg_df.index],
+                            'dataset': ['spatial']*spatial_df.shape[0] +
+                                       ['scRNA-seq']*scRNA_df.shape[0] +
+                                       ['scRNA-seq']*scRNA_avg_df.shape[0],
+                            'datatype': ['cell/spot']*spatial_df.shape[0] +
+                                        ['cell/spot']*scRNA_df.shape[0] +
+                                        ['marker']*scRNA_avg_df.shape[0]
+                            },
+                           index = spatial_df.index.to_list() +
+                                   scRNA_df.index.to_list() +
+                                   [f'{x}-marker' for x in scRNA_avg_df.index])
+    
+    plot_sizes = {'cell/spot': 20, 'marker': 200}
+    plot_markers = {'cell/spot': 'o', 'marker': 'X'}
+    # color for plot already defined
+
+    sns.set_style("darkgrid")
+    
+    # relplot return a FacetGrid object
+    # specify figure size by Height (in inches) of each facet, and Aspect ratio of each facet
+    fgrid = sns.relplot(data=plot_df, x='UMAP1', y='UMAP2', hue='celltype', size='datatype', style='datatype', sizes=plot_sizes, markers=plot_markers, palette=plot_colors, kind='scatter', col='dataset', col_order=['scRNA-seq', 'spatial'], height=4.8*2, aspect=6.4/4.8)
+    fgrid.set(xlabel='Embedding Dimension 1', ylabel='Embedding Dimension 2')
+    # Put the legend out of the figure
+    #ax.legend(loc='center left', bbox_to_anchor=(1, 0.5))
+    
+    # add cell-type annotations around marker coordinates
+    # adjustText do not support seaborn relplot
+    #from adjustText import adjust_text
+    # fgrid.axes return an array of all axes in the figure
+    ax = fgrid.axes[0, 0]
+    texts = []
+    for one_row in scRNA_avg_df.index:
+        texts.append(ax.text(plot_df.at[one_row+'-marker', 'UMAP1'], plot_df.at[one_row+'-marker', 'UMAP2'], one_row, weight='bold'))
+    #adjust_text(texts)
+    
+    plt.savefig(os.path.join(diagnosis_path, 'raw_input_data', 'UMAP_raw_input_color_by_celltype.png'))
+    plt.close()
+    
+    
+    # also save UMAP coordinates
+    plot_df[['UMAP1', 'UMAP2']].to_csv(os.path.join(diagnosis_path, 'raw_input_data', 'UMAP_coordinates_raw_input.csv.gz'), compression='gzip')
+
+
+
+def diagnosisCVAE(cvae, encoder, decoder, spatial_embed, spatial_transformed_df, spatial_transformed_numi, pseudo_spatial_embed, scRNA_celltype, celltype_order, celltype_count_dict, scrna_cell_celltype_prop, scRNA_embed, pseudo_spots_celltype_prop, n_cell_in_spot, pseudo_spot_embed, scRNA_decode_df, scRNA_decode_avg_df, new_markers, plot_colors):
     '''
     save CVAE related Keras models to h5 file, generate figures to diagnosis the training of CVAE
 
     Parameters
     ----------
     cvae : Keras model
         already trained CVAE model
@@ -64,14 +238,16 @@
         mu in latent space of pseudo spots (pseudo-spots * latent neurons); NO scRNA-seq cells included. It will have 0 rows if no scRNA-seq pseudo-spots generated
     scRNA_decode_df : dataframe
         CVAE decodered gene expression (normalized) of scRNA-seq cells (cells * genes)
     scRNA_decode_avg_df : dataframe
         CVAE decodered average gene expression (normalized) of cell-types in scRNA-seq data (cell-types * genes)
     new_markers : list or None
         marker genes from re-run DE on CVAE transformed scRNA-seq data. It will be None if not re-run DE (rerun_DE=False)
+    plot_colors : dict
+        color palette for plot
         
     Returns
     -------
     None.
     '''
     
     print('\nsave variables related to CVAE to files!')
@@ -161,20 +337,16 @@
                                         ['scrna-cell']*scRNA_embed.shape[0] +
                                         ['spatial-spot']*spatial_embed.shape[0],
                             },
                            index = [f'scrna_pseudo{x}' for x in range(pseudo_spot_embed.shape[0])] +
                                    [f'spatial_pseudo{x}' for x in range(pseudo_spatial_embed.shape[0])] +
                                    scRNA_decode_df.index.to_list() +
                                    spatial_transformed_df.index.to_list())
-    plot_colors = {}
-    for one_celltype, one_color in zip([f'spatial ({spatial_embed.shape[0]})']+[f'{x} ({celltype_count_dict[x]})' for x in celltype_order], distinctipy.get_colors(len(celltype_order)+1)):
-        plot_colors[one_celltype] = one_color
-    # assign pseudo spots as gray80
-    plot_colors['pseudo'] = '#cccccc'
     
+    # plot colors already defined
     sns.set_style("darkgrid")
     
     # relplot return a FacetGrid object
     # specify figure size by Height (in inches) of each facet, and Aspect ratio of each facet
     fgrid = sns.relplot(data=plot_df, x='UMAP1', y='UMAP2', hue='celltype', s=20, marker='o', palette=plot_colors, kind='scatter', col='dataset', col_order=['scRNA-seq', 'spatial'], height=4.8*2, aspect=6.4/4.8)
     fgrid.set(xlabel='Embedding Dimension 1', ylabel='Embedding Dimension 2')
     # Put the legend out of the figure
```

### Comparing `sdeper-1.2.0/src/hyper_parameter_optimization.py` & `sdeper-1.2.1/src/hyper_parameter_optimization.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/imputation.py` & `sdeper-1.2.1/src/imputation.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/local_fit_numba.py` & `sdeper-1.2.1/src/local_fit_numba.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/model_fit.py` & `sdeper-1.2.1/src/model_fit.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/parse_opt.py` & `sdeper-1.2.1/src/parse_opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import copy
 
 
 
 # default value for options
 default_paramdict = {'spatial_file': None, 'ref_file': None, 'ref_celltype_file': None, 'marker_file': None, 'loc_file': None, 'A_file': None,
                      'n_cores': 1, 'threshold': 0, 'use_cvae': True, 'use_imputation': False, 'diagnosis': False, 'verbose': True,
-                     'use_fdr': True, 'p_val_cutoff': 0.05, 'fc_cutoff': 1.2, 'pct1_cutoff': 0.3, 'pct2_cutoff': 0.1, 'sortby_fc': True, 'n_marker_per_cmp': 10, 'filter_cell': True, 'filter_gene': True,
-                     'n_hv_gene': 200,  'n_pseudo_spot': 500000, 'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.01, 'num_hidden_layer': 2, 'redo_de': True, 'seed': 383,
+                     'use_fdr': True, 'p_val_cutoff': 0.05, 'fc_cutoff': 1.2, 'pct1_cutoff': 0.3, 'pct2_cutoff': 0.1, 'sortby_fc': True, 'n_marker_per_cmp': 20, 'filter_cell': True, 'filter_gene': True,
+                     'n_hv_gene': 200,  'n_pseudo_spot': 500000, 'pseudo_spot_min_cell': 2, 'pseudo_spot_max_cell':8, 'seq_depth_scaler': 10000, 'cvae_input_scaler': 10, 'cvae_init_lr':0.01, 'num_hidden_layer': 2, 'use_batch_norm': True, 'cvae_train_epoch': 500, 'use_spatial_pseudo': False, 'redo_de': True, 'seed': 383,
                      'lambda_r': None, 'lambda_r_range_min': 0.1, 'lambda_r_range_max': 100, 'lambda_r_range_k': 8,
                      'lambda_g': None, 'lambda_g_range_min': 0.1, 'lambda_g_range_max': 100, 'lambda_g_range_k': 8,
                      'diameter': 200, 'impute_diameter': [160, 114, 80]
                     }
 
 
 
@@ -102,14 +102,17 @@
     --n_pseudo_spot         maximum number of pseudo-spots generated by randomly combining scRNA-seq cells into one pseudo-spot in CVAE training. Default value is {default_paramdict["n_pseudo_spot"]}.
     --pseudo_spot_min_cell  minimum value of cells in one pseudo-spot when combining cells into pseudo-spots. Default value is {default_paramdict["pseudo_spot_min_cell"]}.
     --pseudo_spot_max_cell  maximum value of cells in one pseudo-spot when combining cells into pseudo-spots. Default value is {default_paramdict["pseudo_spot_max_cell"]}.
     --seq_depth_scaler      a scaler of scRNA-seq sequencing depth to transform CVAE decoded values (sequencing depth normalized gene expressions) back to raw nUMI counts. Default value is {default_paramdict["seq_depth_scaler"]} for all cells.
     --cvae_input_scaler     maximum value of the scaled input for CVAE input layer. Default value is {default_paramdict["cvae_input_scaler"]}, i.e. linearly scale all the sequencing depth normalized gene expressions to range [0, {default_paramdict["cvae_input_scaler"]}].
     --cvae_init_lr          initial learning rate for training CVAE. Default value is {default_paramdict["cvae_init_lr"]}. Although learning rate will decreasing automatically during training, large initial learning rate will cause training failure at the very beginning of training. If loss function value do NOT monotonically decrease, please try smaller initial learning rate.
     --num_hidden_layer      number of hidden layers in encoder and decoder of CVAE. Default value is {default_paramdict["num_hidden_layer"]}. The number of neurons in each hidden layer will be determined automatically.
+    --use_batch_norm        whether to use Batch Normalization in CVAE training. Default value is {default_paramdict["use_batch_norm"]}. If true, enables Batch Normalization in CVAE training.
+    --cvae_train_epoch      maximum number of training epochs for the CVAE. Default value is {default_paramdict["cvae_train_epoch"]}.
+    --use_spatial_pseudo    whether to generate "pseudo-spots" in spatial condition by randomly combining existing spatial spots in CVAE training. Default value is {default_paramdict["use_spatial_pseudo"]}. If true, half of the total number specified by option `n_pseudo_spot` will be created.
     --redo_de               control whether to redo Differential analysis on CVAE transformed scRNA-seq gene expressions to get a new set of marker gene list of cell-types (true/false). Default value is {default_paramdict["redo_de"]}. It's recommended to redo Differential analysis since CVAE transformation may change the marker gene profile of cell-types.
     --seed                  seed value of TensorFlow to control the randomness in building CVAE. Default value is {default_paramdict["seed"]}.
     
     
     -------------- GLRM hyper-parameter related options ---------------
     
     We incorporate adaptive Lasso penalty and graph Laplacian penalty in GLRM, and use the hyper-parameters lambda_r and lambda_g to balance the strength of those two penalties respectively.
@@ -159,14 +162,17 @@
             n_pseudo_spot : number of pseudo-spots\n
             pseudo_spot_min_cell : minimum value of cells in pseudo-spot\n
             pseudo_spot_max_cell : maximum value of cells in pseudo-spot\n
             seq_depth_scaler : a scaler of scRNA-seq sequencing depth\n
             cvae_input_scaler : maximum value of the scaled input for CVAE\n
             cvae_init_lr : initial learning rate for training CVAE\n
             num_hidden_layer : number of hidden layers in encoder and decoder\n
+            use_batch_norm : whether to use Batch Normalization\n
+            cvae_train_epoch : max number of training epochs for the CVAE\n
+            use_spatial_pseudo : whether to generate "pseudo-spots" in spatial condition\n
             redo_de : whether to redo DE after CVAE transformation\n
             seed : seed value for random in building CVAE\n
             diagnosis : True or False, if True save more information to files for diagnosis CVAE and hyper-parameter selection\n
             verbose : True or False, if True print more information during program running\n
             use_fdr : whether to use FDR adjusted p value for filtering and sorting\n
             p_val_cutoff : threshold of p value (or FDR if --use_fdr is true) in marker genes filtering\n
             fc_cutoff : threshold of fold change (without log transform!) in marker genes filtering\n
@@ -186,15 +192,15 @@
         print('Use -h or --help for detailed help!')
         sys.exit(1)
         
     # 定义命令行参数
     # 短选项名后的冒号(:)表示该选项必须有附加的参数
     # 长选项名后的等号(=)表示该选项必须有附加的参数
     shortargs = 'hq:r:c:m:l:a:o:n:v'
-    longargs = ['help', 'query=', 'ref=', 'ref_anno=', 'marker=', 'loc=', 'adjacency=', 'n_cores=', 'lambda_r=', 'lambda_r_range_min=', 'lambda_r_range_max=', 'lambda_r_range_k=', 'lambda_g=', 'lambda_g_range_min=', 'lambda_g_range_max=', 'lambda_g_range_k=', 'use_cvae=', 'threshold=', 'n_hv_gene=', 'n_marker_per_cmp=', 'n_pseudo_spot=', 'pseudo_spot_min_cell=', 'pseudo_spot_max_cell=', 'seq_depth_scaler=', 'cvae_input_scaler=', 'cvae_init_lr=', 'num_hidden_layer=', 'redo_de=', 'seed=', 'diagnosis=', 'verbose=', 'use_fdr=', 'p_val_cutoff=', 'fc_cutoff=', 'pct1_cutoff=', 'pct2_cutoff=', 'sortby_fc=', 'filter_cell=', 'filter_gene=', 'use_imputation=', 'diameter=', 'impute_diameter=', 'version']
+    longargs = ['help', 'query=', 'ref=', 'ref_anno=', 'marker=', 'loc=', 'adjacency=', 'n_cores=', 'lambda_r=', 'lambda_r_range_min=', 'lambda_r_range_max=', 'lambda_r_range_k=', 'lambda_g=', 'lambda_g_range_min=', 'lambda_g_range_max=', 'lambda_g_range_k=', 'use_cvae=', 'threshold=', 'n_hv_gene=', 'n_marker_per_cmp=', 'n_pseudo_spot=', 'pseudo_spot_min_cell=', 'pseudo_spot_max_cell=', 'seq_depth_scaler=', 'cvae_input_scaler=', 'cvae_init_lr=', 'num_hidden_layer=', 'use_batch_norm=', 'cvae_train_epoch=', 'use_spatial_pseudo=', 'redo_de=', 'seed=', 'diagnosis=', 'verbose=', 'use_fdr=', 'p_val_cutoff=', 'fc_cutoff=', 'pct1_cutoff=', 'pct2_cutoff=', 'sortby_fc=', 'filter_cell=', 'filter_gene=', 'use_imputation=', 'diameter=', 'impute_diameter=', 'version']
     
   
     # 解析命令行参数
     # sys.argv[0]为python脚本名，后续全为参数
     # opts为分析出的参数信息，args为不符合格式信息的剩余参数
     opts, args = getopt(sys.argv[1:], shortargs, longargs)
     
@@ -518,14 +524,46 @@
                     print(f'WARNING: invalid option value `{paramdict["num_hidden_layer"]}` for num_hidden_layer! Please use integer which >= 1. Currently num_hidden_layer is set to be value `1`!')
                     paramdict['num_hidden_layer'] = 1
             except:
                 print(f'WARNING: unrecognized option value `{val}` for num_hidden_layer! Please use numeric value. Currently num_hidden_layer is set to be default value `{default_paramdict["num_hidden_layer"]}`!')
             continue
         
         
+        if opt in ('--use_batch_norm'):
+            if val.casefold() == 'true'.casefold():
+                paramdict['use_batch_norm'] = True
+            elif val.casefold() == 'false'.casefold():
+                paramdict['use_batch_norm'] = False
+            else:
+                print(f'WARNING: unrecognized option value `{val}` for use_batch_norm! Please use string of true or false. Currently use_batch_norm is set to be default value `{default_paramdict["use_batch_norm"]}`!')
+            continue
+        
+        
+        if opt in ('--cvae_train_epoch'):
+            try:
+                paramdict['cvae_train_epoch'] = int(float(val))
+                
+                if paramdict['cvae_train_epoch'] < 30:
+                    print(f'WARNING: invalid option value `{paramdict["cvae_train_epoch"]}` for cvae_train_epoch! Please use integer which >= 30. Currently cvae_train_epoch is set to be value `30`!')
+                    paramdict['cvae_train_epoch'] = 30
+            except:
+                print(f'WARNING: unrecognized option value `{val}` for cvae_train_epoch! Please use numeric value. Currently cvae_train_epoch is set to be default value `{default_paramdict["cvae_train_epoch"]}`!')
+            continue
+        
+        
+        if opt in ('--use_spatial_pseudo'):
+            if val.casefold() == 'true'.casefold():
+                paramdict['use_spatial_pseudo'] = True
+            elif val.casefold() == 'false'.casefold():
+                paramdict['use_spatial_pseudo'] = False
+            else:
+                print(f'WARNING: unrecognized option value `{val}` for use_spatial_pseudo! Please use string of true or false. Currently use_spatial_pseudo is set to be default value `{default_paramdict["use_spatial_pseudo"]}`!')
+            continue
+        
+        
         if opt in ('--redo_de'):
             if val.casefold() == 'true'.casefold():
                 paramdict['redo_de'] = True
             elif val.casefold() == 'false'.casefold():
                 paramdict['redo_de'] = False
             else:
                 print(f'WARNING: unrecognized option value `{val}` for redo_de! Please use string of true or false. Currently redo_de is set to be default value `{default_paramdict["redo_de"]}`!')
```

### Comparing `sdeper-1.2.0/src/preprocess.py` & `sdeper-1.2.1/src/preprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import pandas as pd
 from cvae import build_CVAE_whole
 from utils import run_DE_only
 from config import print
 
 
 
-def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, filter_cell, filter_gene, diagnosis):
+def preprocess(spatial_file, ref_file, ref_anno_file, marker_file, A_file, use_cvae, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, filter_cell, filter_gene, diagnosis):
     '''
     preprocess files
 
     Parameters
     ----------
     spatial_file : string
         full path of input csv file of raw nUMI counts in spatial transcriptomic data (spots * genes).
@@ -62,14 +62,20 @@
         a scaler of scRNA-seq sequencing depth.
     cvae_input_scaler : int
         maximum value of the scaled input for CVAE.
     cvae_init_lr : float
         initial learning rate for training CVAE.
     num_hidden_layer : int
         number of hidden layers in encoder and decoder.
+    use_batch_norm : bool
+        whether to use Batch Normalization.
+    cvae_train_epoch : int
+        max number of training epochs for the CVAE.
+    use_spatial_pseudo : int
+        whether to generate "pseudo-spots" in spatial condition.
     redo_de : bool
         whether to redo DE after CVAE transformation.
     use_fdr : bool
         whether to use FDR adjusted p value for filtering and sorting.
     p_val_cutoff : float
         threshold of p value (or FDR if --use_fdr is true) in marker genes filtering.
     fc_cutoff : float
@@ -104,15 +110,15 @@
     # first determine whether to build CVAE
     if use_cvae:
         if ref_file is None or ref_anno_file is None:
             raise Exception('ERROR: building CVAE requires both reference scRNA-seq data and corresponding cell-type annotation specified! But at least one of them is not specified!')
             
         print('first build CVAE...\n')
         # build CVAE, and return the data dict including transformed spatial data and reference gene expression
-        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
+        spatial_df, cvae_marker_df, new_markers = build_CVAE_whole(spatial_file, ref_file, ref_anno_file, marker_file, n_hv_gene, n_marker_per_cmp, n_pseudo_spot, pseudo_spot_min_cell, pseudo_spot_max_cell, seq_depth_scaler, cvae_input_scaler, cvae_init_lr, num_hidden_layer, use_batch_norm, cvae_train_epoch, use_spatial_pseudo, redo_de, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
         
         # calculate squencing depth, sum also works on sparse dataframe
         N = spatial_df.sum(axis=1)
     
     else:
         
         print('building CVAE skipped...\n')
@@ -164,16 +170,17 @@
             print(f'from user specified marker gene expression use {len(marker_genes)} marker genes overlapped with spatial + scRNA-seq data')
             # if len(marker_genes) < spatial_df.shape[1]:
             #     print(f'{spatial_df.shape[1]-len(marker_genes)} genes in overlapped gene list between spatial and scRNA-seq data but not found in user provided marker gene expression: {", ".join(set(spatial_df.columns).difference(set(marker_genes)))}\n')
             
         else:
             # perform DE, return the marker gene expression. The identified markers but not in spatial data has already been removed
             print('no marker gene profile provided. Perform DE to get cell-type marker genes on scRNA-seq data...\n')
-            marker_df = run_DE_only(ref_file, ref_anno_file, spatial_df.columns.tolist(), n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
-            marker_genes = marker_df.columns
+            tmp_scrna_obj, marker_df = run_DE_only(ref_file, ref_anno_file, spatial_df.columns.tolist(), n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, diagnosis, filter_cell, filter_gene)
+            # note dataframe index and columns returns a RangeIndex object rather than list
+            marker_genes = marker_df.columns.to_list()
     
     else:
         
         print('use the marker genes derived from CVAE transformed scRNA-seq for downstream regression!')
         marker_genes = new_markers
     
     
@@ -213,14 +220,24 @@
         print(f'{len(exclude_spots):d} spots will be excluded as sum of nUMI < {nUMI_threshold:d}')
         spatial_df.drop(exclude_spots, inplace=True)
         if A_df is not None:
             A_df.drop(exclude_spots, inplace=True)
             A_df.drop(exclude_spots, axis=1, inplace=True)
     else:
         print('all spots passed filtering')
+        
+        
+    if diagnosis and not use_cvae:
+        # plot UMAP for raw input gene expressions here
+        import scanpy as sc
+        from diagnosis_plots import defineColor, rawInputUMAP
+        tmp_scrna_celltype = sc.get.obs_df(tmp_scrna_obj, keys='celltype').to_frame()
+        tmp_scrna_celltype['celltype'] = tmp_scrna_celltype['celltype'].astype(str)
+        plot_colors = defineColor(spatial_df.shape[0], tmp_scrna_celltype)
+        rawInputUMAP(spatial_df, sc.get.obs_df(tmp_scrna_obj, keys=marker_genes), tmp_scrna_celltype, plot_colors)
 
     
     # record the zeros in spatial data if filtering zeros is turned on
     filter_zero_gene = False
     use_original_nUMI = True
     
     if filter_zero_gene:
```

### Comparing `sdeper-1.2.0/src/run_model.py` & `sdeper-1.2.1/src/run_model.py`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/sdeper.egg-info/PKG-INFO` & `sdeper-1.2.1/src/sdeper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sdeper
-Version: 1.2.0
+Version: 1.2.1
 Summary: Spatial Deconvolution method with Platform Effect Removal
 Home-page: https://az7jh2.github.io/SDePER/
 Author: Ningshan Li
 Author-email: hill103.2@gmail.com
 Project-URL: Documentation, https://sdeper.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/az7jh2/SDePER
 Project-URL: Changelog, https://sdeper.readthedocs.io/en/latest/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.12
+Requires-Python: >=3.9.12, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.22.4
 Requires-Dist: scipy==1.8.1
 Requires-Dist: pandas==1.4.3
 Requires-Dist: networkx==2.8.4
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: scikit-learn==1.1.1
@@ -28,20 +28,22 @@
 Requires-Dist: seaborn==0.11.2
 Requires-Dist: umap-learn==0.5.3
 Requires-Dist: distinctipy==1.2.2
 Requires-Dist: reportlab==4.1.0
 Requires-Dist: opencv-python==4.6.0.66
 
 # SDePER
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
+![OS](https://img.shields.io/badge/os-linux-blue) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sdeper)](https://www.python.org/) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/az7jh2/SDePER)](https://github.com/az7jh2/SDePER) [![PyPI](https://img.shields.io/pypi/v/sdeper)](https://pypi.org/project/sdeper/)  [![Conda Version](https://img.shields.io/conda/vn/bioconda/sdeper)](https://anaconda.org/bioconda/sdeper) [![Docker Image Version (latest by date)](https://img.shields.io/docker/v/az7jh2/sdeper?label=docker)](https://hub.docker.com/r/az7jh2/sdeper) [![Read the Docs (version)](https://img.shields.io/readthedocs/sdeper/latest)](https://sdeper.readthedocs.io/en/latest/)
 
 **SDePER** (**S**patial **De**convolution method with **P**latform **E**ffect **R**emoval) is a **hybrid** machine learning and regression method to deconvolve Spatial barcoding-based transcriptomic data using reference single-cell RNA sequencing data, considering **platform effects removal**, **sparsity** of cell types per capture spot and across-spots **spatial correlation** in cell type compositions. SDePER is also able to **impute** cell type compositions and gene expression at unmeasured locations in a tissue map with **enhanced resolution**.
 
 ## Quick Start
 
+SDePER currently supports only Linux operating systems such as Ubuntu, and is compatible with Python versions 3.9.12 up to but not including 3.11.
+
 SDePER can be installed via conda
 
 ```bash
 conda create -n sdeper-env -c bioconda -c conda-forge python=3.9.12 sdeper
 ```
 
 or pip
```

### Comparing `sdeper-1.2.0/src/sdeper.egg-info/SOURCES.txt` & `sdeper-1.2.1/src/sdeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdeper-1.2.0/src/utils.py` & `sdeper-1.2.1/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,17 @@
     
     # first calculate pct for each cell-type
     pct_dict = {}
     for this_celltype in celltypes:
         pct_dict[this_celltype] = calc_pct(sc_obj, this_celltype)
     
     # perform test
-    for this_celltype in celltypes:
+    for t, this_celltype in enumerate(celltypes):
+        
+        print(f'{t/len(celltypes):.0%}...', end='')
         
         for other_celltype in celltypes:
             if this_celltype == other_celltype:
                 continue
             
             # compare one cell-type against another cell-type
             sc.tl.rank_genes_groups(sc_obj, groupby='celltype', use_raw=False, corr_method='benjamini-hochberg',
@@ -408,14 +410,16 @@
     filter_cell : bool
         whether to filter cells before DE
     filter_gene : bool
         whether to filter genes before DE
         
     Returns
     -------
+    scrna_obj : AnnData object
+        a AnnData object for scRNA-seq data
     marker_gene_profile : DataFrame
         average gene expressions of identified cell-type specific marker genes from refer scRNA-seq data
     '''
     
     scrna_obj = read_scRNA_data(ref_file, ref_anno_file, filter_cell, filter_gene)
     
     # subset genes
@@ -431,15 +435,15 @@
     # generate average gene expressions (gene signature) for cell-types based on normalized values
     tmp_df = sc.get.obs_df(scrna_obj, keys=marker_genes)
     
     tmp_df['celltype'] = scrna_obj.obs['celltype']
 
     tmp_df = tmp_df.groupby(['celltype']).mean()
     
-    return tmp_df
+    return scrna_obj, tmp_df
 
 
 
 def rerun_DE(scRNA_df, scRNA_celltype, n_marker_per_cmp, use_fdr, p_val_cutoff, fc_cutoff, pct1_cutoff, pct2_cutoff, sortby_fc, save_result=False, filter_gene=True):
     '''
     rerun DE on CVAE transformed scRNA-seq data
```

