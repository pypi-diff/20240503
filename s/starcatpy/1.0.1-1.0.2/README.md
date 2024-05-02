# Comparing `tmp/starcatpy-1.0.1.tar.gz` & `tmp/starcatpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/starcatpy-1.0.1.tar", last modified: Wed May  1 21:20:53 2024, max compression
+gzip compressed data, was "starcatpy-1.0.2.tar", last modified: Thu May  2 21:42:43 2024, max compression
```

## Comparing `starcatpy-1.0.1.tar` & `starcatpy-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 mc1070   (5169487) srlab    (10036)        0 2024-05-01 21:20:53.000000 starcatpy-1.0.1/
--rw-rw----   0 mc1070   (5169487) srlab    (10036)     1070 2024-05-01 14:42:20.000000 starcatpy-1.0.1/LICENSE
--rw-rw----   0 mc1070   (5169487) srlab    (10036)     4029 2024-05-01 21:20:53.000000 starcatpy-1.0.1/PKG-INFO
--rw-rw----   0 mc1070   (5169487) srlab    (10036)     3387 2024-05-01 21:01:22.000000 starcatpy-1.0.1/README.md
--rw-rw----   0 mc1070   (5169487) srlab    (10036)      103 2024-05-01 20:03:13.000000 starcatpy-1.0.1/pyproject.toml
--rw-rw----   0 mc1070   (5169487) srlab    (10036)       38 2024-05-01 21:20:53.000000 starcatpy-1.0.1/setup.cfg
--rw-rw----   0 mc1070   (5169487) srlab    (10036)     1180 2024-05-01 21:20:01.000000 starcatpy-1.0.1/setup.py
-drwxrwx---   0 mc1070   (5169487) srlab    (10036)        0 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/
-drwxrwx---   0 mc1070   (5169487) srlab    (10036)        0 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcat/
--rwxrwx---   0 mc1070   (5169487) srlab    (10036)       35 2024-05-01 19:26:23.000000 starcatpy-1.0.1/src/starcat/__init__.py
--rwxrwx---   0 mc1070   (5169487) srlab    (10036)    18611 2024-05-01 21:14:40.000000 starcatpy-1.0.1/src/starcat/starcat.py
-drwxrwx---   0 mc1070   (5169487) srlab    (10036)        0 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/
--rw-rw----   0 mc1070   (5169487) srlab    (10036)     4029 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/PKG-INFO
--rw-rw----   0 mc1070   (5169487) srlab    (10036)      312 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/SOURCES.txt
--rw-rw----   0 mc1070   (5169487) srlab    (10036)        1 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/dependency_links.txt
--rw-rw----   0 mc1070   (5169487) srlab    (10036)       42 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/entry_points.txt
--rw-rw----   0 mc1070   (5169487) srlab    (10036)       90 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/requires.txt
--rw-rw----   0 mc1070   (5169487) srlab    (10036)        8 2024-05-01 21:20:53.000000 starcatpy-1.0.1/src/starcatpy.egg-info/top_level.txt
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.098060 starcatpy-1.0.2/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-02 20:08:01.000000 starcatpy-1.0.2/LICENSE
+-rw-r--r--   0 dkotliar   (503) staff       (20)     3816 2024-05-02 21:42:43.097561 starcatpy-1.0.2/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)     2960 2024-05-02 21:00:49.000000 starcatpy-1.0.2/README.md
+-rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-02 20:08:01.000000 starcatpy-1.0.2/pyproject.toml
+-rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-02 21:42:43.098190 starcatpy-1.0.2/setup.cfg
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1191 2024-05-02 21:34:22.000000 starcatpy-1.0.2/setup.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.089421 starcatpy-1.0.2/src/
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.092904 starcatpy-1.0.2/src/starcat/
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)       35 2024-05-02 20:08:01.000000 starcatpy-1.0.2/src/starcat/__init__.py
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)    19188 2024-05-02 20:23:44.000000 starcatpy-1.0.2/src/starcat/starcat.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-02 21:42:43.096937 starcatpy-1.0.2/src/starcatpy.egg-info/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     3816 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)      312 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/SOURCES.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/dependency_links.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       41 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/entry_points.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       90 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/requires.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        8 2024-05-02 21:42:43.000000 starcatpy-1.0.2/src/starcatpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `starcatpy-1.0.1/LICENSE` & `starcatpy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starcatpy-1.0.1/PKG-INFO` & `starcatpy-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: starcatpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 Home-page: https://github.com/immunogenomics/starCAT
 Author: Dylan Kotliar, Michelle Curtis
-Author-email: dylkot@gmail.com, curtism@broadinstitute.org
-License: UNKNOWN
+Author-email: dkotliar@broadinstitute.org, curtism@broadinstitute.org
 Project-URL: Bug Tracker, https://github.com/immunogenomics/starCAT/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scanpy
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: fastcluster
+Requires-Dist: matplotlib
+Requires-Dist: palettable
+Requires-Dist: scipy
+Requires-Dist: pyyaml
+Requires-Dist: cnmf
 
 # starCAT
 Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 
 ## Citation
 If you use *CAT, please cite our [preprint]().
 
 ## Installation
-To install starCAT, first create a conda environment with necessary dependencies.
-```bash
-conda create -n cnmf_env --yes --channel bioconda --channel conda-forge --channel defaults python=3.7 fastcluster matplotlib numpy palettable pandas scipy 'scikit-learn>=1.0' pyyaml 'scanpy>=1.8' && conda clean --yes --all # Create environment, cnmf_env, containing required packages
-conda activate cnmf_env # Activate cnmf_env - necessary before running cnmf
-pip install cnmf # install the actual cnmf package
-    
-## Only needed to load the example notebook in jupyterlab but not needed for non-interactive runs ## 
-conda install --yes jupyterlab && conda clean --yes --all
-```
 
-Then install starCAT via the Python Package Index.
+You can install starCAT and its dependencies via the Python Package Index.
 ```bash
 pip install starcatpy
 ```
 
+We have tested it with scikit-learn 1.0.3, Scanpy 1.8, and python 3.7. You need the jupyter or jupyterlab packages to access the tutorial notebooks. In addition, building the UMAP in the tutorial requires python 3.8+
+
+
 ## Tutorial
 Please see our tutorials in [python](https://github.com/immunogenomics/starCAT/blob/main/Examples/starCAT_vingette.ipynb) and [R](https://github.com/immunogenomics/starCAT/blob/main/Examples/starCAT_vingette_R.ipynb). A sample pipeline using a pre-built reference programs (TCAT.V1) is shown below. 
 
 ```python
 # Load default TCAT reference from starCAT databse
 tcat = starCAT(reference='TCAT.V1')
 
@@ -81,9 +83,7 @@
 starcat --reference "TCAT.V1" --counts {counts_fn} --output-dir {output_dir} --name {outuput_name}
 ```
 * --reference - name of a default reference to download (ex. TCAT.V1) OR filepath containing a reference set of GEPs by genes (*.tsv/.csv/.txt), default is 'TCAT.V1'
 * --counts - filepath to input (cell x gene) counts matrix as a matrix market (.mtx.gz), tab delimited text file, or anndata file (.h5ad)
 * --scores - optional path to yaml file for calculating score add-ons, not necessary for pre-built references
 * --output-dir - the output directory. all output will be placed in {output-dir}/{name}...'. default directory is '.'
 * --name - the output analysis prefix name, default is 'starCAT'
-
-
```

### Comparing `starcatpy-1.0.1/README.md` & `starcatpy-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # starCAT
 Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 
 ## Citation
 If you use *CAT, please cite our [preprint]().
 
 ## Installation
-To install starCAT, first create a conda environment with necessary dependencies.
-```bash
-conda create -n cnmf_env --yes --channel bioconda --channel conda-forge --channel defaults python=3.7 fastcluster matplotlib numpy palettable pandas scipy 'scikit-learn>=1.0' pyyaml 'scanpy>=1.8' && conda clean --yes --all # Create environment, cnmf_env, containing required packages
-conda activate cnmf_env # Activate cnmf_env - necessary before running cnmf
-pip install cnmf # install the actual cnmf package
-    
-## Only needed to load the example notebook in jupyterlab but not needed for non-interactive runs ## 
-conda install --yes jupyterlab && conda clean --yes --all
-```
 
-Then install starCAT via the Python Package Index.
+You can install starCAT and its dependencies via the Python Package Index.
 ```bash
 pip install starcatpy
 ```
 
+We have tested it with scikit-learn 1.0.3, Scanpy 1.8, and python 3.7. You need the jupyter or jupyterlab packages to access the tutorial notebooks. In addition, building the UMAP in the tutorial requires python 3.8+
+
+
 ## Tutorial
 Please see our tutorials in [python](https://github.com/immunogenomics/starCAT/blob/main/Examples/starCAT_vingette.ipynb) and [R](https://github.com/immunogenomics/starCAT/blob/main/Examples/starCAT_vingette_R.ipynb). A sample pipeline using a pre-built reference programs (TCAT.V1) is shown below. 
 
 ```python
 # Load default TCAT reference from starCAT databse
 tcat = starCAT(reference='TCAT.V1')
```

### Comparing `starcatpy-1.0.1/setup.py` & `starcatpy-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="starcatpy",
-    version="1.0.1",
+    version="1.0.2",
     author="Dylan Kotliar, Michelle Curtis",
-    author_email="dylkot@gmail.com, curtism@broadinstitute.org",
+    author_email="dkotliar@broadinstitute.org, curtism@broadinstitute.org",
     description="Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/immunogenomics/starCAT",
     project_urls={
         "Bug Tracker": "https://github.com/immunogenomics/starCAT/issues",
     },
```

### Comparing `starcatpy-1.0.1/src/starcat/starcat.py` & `starcatpy-1.0.2/src/starcat/starcat.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import scipy.sparse as sp
 import yaml
 import requests
 import tarfile
 import warnings
 
+reference_url = 'https://raw.githubusercontent.com/immunogenomics/starCAT/main/current_references.tsv'
 _nmf_kwargs = dict(
                    beta_loss='frobenius',
                    solver='mu',
                    tol=1e-4,
                    max_iter=1000,
                    init='random',
                    update_H = False
@@ -49,29 +50,46 @@
 
 def load_df_from_npz(filename):
     with np.load(filename, allow_pickle=True) as f:
         obj = pd.DataFrame(**f)
     return obj
 
 
+def load_table_url(url, **kwargs):
+    '''
+    Load URL from web.
+    
+    Additional key word arguments are passed to pandas.read_csv
+    '''
+    response = requests.get(url)
+
+    # Ensure the request was successful
+    if response.status_code == 200:
+        # Use pandas to read the tab-delimited file
+        from io import StringIO
+        data = pd.read_csv(StringIO(response.text), sep='\t', **kwargs)
+        return(data)
+    else:
+        raise Exception('Failed to load url: %s' % url)
+
+
 class starCAT(cNMF):  
     def __init__(self, reference = 'TCAT.V1', score_path = None, cachedir='./cache'):
         """
         Runs *CAT on a query dataset.
         
         Parameters
         ----------
         reference : str, name of reference from starCAT database or path to a custom reference file ending in .tsv or .txt (Default="TCAT.V1") 
         
         score_path : str, optional path to a yaml file to compute addon scores for discrete or continuous features from starCAT output.
         Only needed if reference is a path to a custom reference file and not a starCAT database name (default=None)        
         """
         
         self._nmf_kwargs = _nmf_kwargs
-        self._classpath = os.path.dirname(os.path.realpath(__file__))
         self._cache = cachedir
         self.ref_name = reference
         self.usage = None
         self.usage_norm = None
         self.scores = None
         
         if reference.endswith('.txt') or reference.endswith('.tsv'):
@@ -97,16 +115,19 @@
     def _initialize_ref(self):
         """"
         Initializes a reference set of GEPs by genes from a file name ending in the extension .txt or .tsv
         or using the name of a pre-built reference (default reference is TCAT.V1).
         
         """
 
-        ref_list_fn = os.path.join(self._classpath, '../../current_references.tsv')
-        ref_list = pd.read_csv(ref_list_fn, index_col = 0, sep = '\t', skiprows = 1)
+        try:
+            ref_list = load_table_url(reference_url, comment='#')
+        except:
+            raise Exception('Failed to load reference database URL file. Make sure you are connected to the internet')
+
         available_refs = ref_list['Name'].values
 
         if self.ref_name not in available_refs:
             refliststr = ','.join(available_refs)
             raise Exception(
                 "{ref} is not found in list of pre-built reference names. "
                 "It is also not a valid path to a reference file which would "
```

### Comparing `starcatpy-1.0.1/src/starcatpy.egg-info/PKG-INFO` & `starcatpy-1.0.2/src/starcatpy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: starcatpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 Home-page: https://github.com/immunogenomics/starCAT
 Author: Dylan Kotliar, Michelle Curtis
-Author-email: dylkot@gmail.com, curtism@broadinstitute.org
-License: UNKNOWN
+Author-email: dkotliar@broadinstitute.org, curtism@broadinstitute.org
 Project-URL: Bug Tracker, https://github.com/immunogenomics/starCAT/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scanpy
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: fastcluster
+Requires-Dist: matplotlib
+Requires-Dist: palettable
+Requires-Dist: scipy
+Requires-Dist: pyyaml
+Requires-Dist: cnmf
 
 # starCAT
 Implements *CellAnnotator (aka *CAT/starCAT), annotating scRNA-Seq with predefined gene expression programs
 
 ## Citation
 If you use *CAT, please cite our [preprint]().
 
 ## Installation
-To install starCAT, first create a conda environment with necessary dependencies.
-```bash
-conda create -n cnmf_env --yes --channel bioconda --channel conda-forge --channel defaults python=3.7 fastcluster matplotlib numpy palettable pandas scipy 'scikit-learn>=1.0' pyyaml 'scanpy>=1.8' && conda clean --yes --all # Create environment, cnmf_env, containing required packages
-conda activate cnmf_env # Activate cnmf_env - necessary before running cnmf
-pip install cnmf # install the actual cnmf package
-    
-## Only needed to load the example notebook in jupyterlab but not needed for non-interactive runs ## 
-conda install --yes jupyterlab && conda clean --yes --all
-```
 
-Then install starCAT via the Python Package Index.
+You can install starCAT and its dependencies via the Python Package Index.
 ```bash
 pip install starcatpy
 ```
 
+We have tested it with scikit-learn 1.0.3, Scanpy 1.8, and python 3.7. You need the jupyter or jupyterlab packages to access the tutorial notebooks. In addition, building the UMAP in the tutorial requires python 3.8+
+
+
 ## Tutorial
 Please see our tutorials in [python](https://github.com/immunogenomics/starCAT/blob/main/Examples/starCAT_vingette.ipynb) and [R](https://github.com/immunogenomics/starCAT/blob/main/Examples/starCAT_vingette_R.ipynb). A sample pipeline using a pre-built reference programs (TCAT.V1) is shown below. 
 
 ```python
 # Load default TCAT reference from starCAT databse
 tcat = starCAT(reference='TCAT.V1')
 
@@ -81,9 +83,7 @@
 starcat --reference "TCAT.V1" --counts {counts_fn} --output-dir {output_dir} --name {outuput_name}
 ```
 * --reference - name of a default reference to download (ex. TCAT.V1) OR filepath containing a reference set of GEPs by genes (*.tsv/.csv/.txt), default is 'TCAT.V1'
 * --counts - filepath to input (cell x gene) counts matrix as a matrix market (.mtx.gz), tab delimited text file, or anndata file (.h5ad)
 * --scores - optional path to yaml file for calculating score add-ons, not necessary for pre-built references
 * --output-dir - the output directory. all output will be placed in {output-dir}/{name}...'. default directory is '.'
 * --name - the output analysis prefix name, default is 'starCAT'
-
-
```

