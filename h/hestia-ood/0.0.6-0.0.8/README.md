# Comparing `tmp/hestia-ood-0.0.6.tar.gz` & `tmp/hestia_ood-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-ood-0.0.6.tar", last modified: Wed Mar 13 14:12:21 2024, max compression
+gzip compressed data, was "hestia_ood-0.0.8.tar", last modified: Fri May  3 10:29:16 2024, max compression
```

## Comparing `hestia-ood-0.0.6.tar` & `hestia_ood-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:12:21.261662 hestia-ood-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-13 14:12:21.261662 hestia-ood-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:12:21.261662 hestia-ood-0.0.6/hestia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    25631 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    37012 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:12:21.261662 hestia-ood-0.0.6/hestia/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/utils/file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/utils/graph_part_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/hestia/utils/label_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:12:21.261662 hestia-ood-0.0.6/hestia_ood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-13 14:12:21.000000 hestia-ood-0.0.6/hestia_ood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-13 14:12:21.000000 hestia-ood-0.0.6/hestia_ood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:12:21.000000 hestia-ood-0.0.6/hestia_ood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:12:21.000000 hestia-ood-0.0.6/hestia_ood.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-13 14:12:21.000000 hestia-ood-0.0.6/hestia_ood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 14:12:21.000000 hestia-ood-0.0.6/hestia_ood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 14:12:21.261662 hestia-ood-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-13 14:12:17.000000 hestia-ood-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.033675 hestia_ood-0.0.8/hestia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25658 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37111 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.033675 hestia_ood-0.0.8/hestia/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/graph_part_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/hestia/utils/label_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/hestia_ood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:29:15.000000 hestia_ood-0.0.8/hestia_ood.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 10:29:16.000000 hestia_ood-0.0.8/hestia_ood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:29:16.037675 hestia_ood-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-03 10:29:11.000000 hestia_ood-0.0.8/setup.py
```

### Comparing `hestia-ood-0.0.6/LICENSE` & `hestia_ood-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-ood-0.0.6/hestia/clustering.py` & `hestia_ood-0.0.8/hestia/clustering.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 
 import pandas as pd
 from scipy.sparse.csgraph import connected_components
+from tqdm import tqdm
 
 from hestia.similarity import sim_df2mtx
 
 
 def generate_clusters(
     df: pd.DataFrame,
     field_name: str,
@@ -74,22 +75,28 @@
     df['lengths'] = df[field_name].map(len)
     df.sort_values(by='lengths', ascending=False, inplace=True)
 
     clusters = []
     clustered = set()
     sim_df = sim_df[sim_df['metric'] > threshold]
 
-    for i in df.index:
+    if verbose > 2:
+        pbar = tqdm(df.index)
+    else:
+        pbar = df.index
+
+    for i in pbar:
+        if i in clustered:
+            continue
         in_cluster = set(sim_df.loc[sim_df['query'] == i, 'target'])
         in_cluster.update(set(sim_df.loc[sim_df['target'] == i, 'query']))
         in_cluster.update(set([i]))
+        in_cluster = in_cluster.difference(clustered)
 
         for j in in_cluster:
-            if j in clustered:
-                continue
             clusters.append({
                 'cluster': i,
                 'member': j
             })
         clustered.update(in_cluster)
 
     cluster_df = pd.DataFrame(clusters)
@@ -105,35 +112,40 @@
     df: pd.DataFrame,
     sim_df: pd.DataFrame,
     threshold: float,
     verbose: int
 ) -> pd.DataFrame:
     def _find_connectivity(df, sim_df):
         neighbours = []
-        for i in df.index:
+        for i in tqdm(df.index):
             in_cluster = set(sim_df.loc[sim_df['query'] == i, 'target'])
             in_cluster.update(set(sim_df.loc[sim_df['target'] == i, 'query']))
             neighbours.append(in_cluster)
         return neighbours
 
     sim_df = sim_df[sim_df['metric'] > threshold]
     neighbours = _find_connectivity(df, sim_df)
     df['conectivity'] = list(map(len, neighbours))
     df.sort_values(by='conectivity', ascending=False, inplace=True)
 
     clusters = []
     clustered = set()
+    if verbose > 2:
+        pbar = tqdm(df.index)
+    else:
+        pbar = df.index
 
-    for i in df.index:
+    for i in pbar:
+        if i in clustered:
+            continue
         in_cluster = neighbours.pop(0)
         in_cluster.update([i])
+        in_cluster = in_cluster.difference(clustered)
 
         for j in in_cluster:
-            if j in clustered:
-                continue
             clusters.append({
                 'cluster': i,
                 'member': j
             })
         clustered.update(in_cluster)
 
     cluster_df = pd.DataFrame(clusters)
```

### Comparing `hestia-ood-0.0.6/hestia/partition.py` & `hestia_ood-0.0.8/hestia/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,34 +39,34 @@
     """
     train_df, test_df = train_test_split(df.index.tolist(),
                                          test_size=test_size,
                                          random_state=random_state)
     return train_df, test_df
 
 
-def cc_part(
+def ccpart(
     df: pd.DataFrame,
-    similarity_metric: str,
-    field_name: str,
-    label_name: str,
+    similarity_metric: str = None,
+    field_name: str = None,
+    label_name: str = None,
     threads: int = cpu_count(),
     denominator: str = None,
     test_size: float = 0.2,
     valid_size: float = 0.0,
     threshold: float = 0.3,
     verbose: int = 0,
-    species: str = 'protein',
+    data_type: str = 'protein',
     distance: str = 'tanimoto',
     representation: str = '3di+aa',
     bits: int = 1024,
     radius: int = 2,
     config: dict = None,
     sim_df: Optional[pd.DataFrame] = None
 ) -> Union[Tuple[list, list], Tuple[list, list, list]]:
-    """Use connected components partitioning algorithm
+    """Use CCPart algorithm
     to generate training and evaluation subsets
     that maximise the dissimilarity between their
     entities.
 
     :param df: DataFrame with the entities to partition
     :type df: pd.DataFrame
     :param similarity_metric: Similarity function to use.
@@ -116,18 +116,18 @@
     :param verbose: How much information will be displayed.
     Options:
         - 0: Errors,
         - 1: Warnings,
         - 2: All
     Defaults to 0
     :type verbose: int, optional
-    :param species: Biochemical species to which the data belongs.
+    :param data_type: Biochemical data_type to which the data belongs.
     Options: `protein`, `DNA`, `RNA`, or `small_molecule`; defaults to
     'protein'
-    :type species: str, optional
+    :type data_type: str, optional
     :param distance: Distance metrics for small molecule comparison.
     Currently, it is restricted to Tanimoto distance will
     be extended in future patches; if interested in a specific
     metric please let us know.
     Options:
         - `tanimoto`: Calculates the Tanimoto distance
     Defaults to 'tanimoto'.
@@ -171,15 +171,15 @@
         labels = None
 
     expected_test = test_size * size
     expected_valid = valid_size * size
 
     if sim_df is None:
         sim_df = calculate_similarity(
-            df, df, species=species,
+            df, df, data_type=data_type,
             similarity_metric=similarity_metric,
             field_name=field_name, threshold=threshold,
             threads=threads, verbose=verbose,
             save_alignment=False, filename=None, distance=distance,
             bits=bits, denominator=denominator, radius=radius,
             representation=representation, config=config
         )
@@ -246,15 +246,15 @@
     threads: int = cpu_count(),
     clustering_mode: str = "CDHIT",
     denominator: str = "shortest",
     test_size: float = 0.2,
     valid_size: float = 0.0,
     threshold: float = 0.3,
     verbose: int = 2,
-    species: str = 'protein',
+    data_type: str = 'protein',
     representation: str = '3di+aa',
     random_state: int = 42,
     bits: int = 1024,
     radius: int = 2,
     config: dict = None,
     sim_df: Optional[pd.DataFrame] = None
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
@@ -313,18 +313,18 @@
     :param verbose: How much information will be displayed.
     Options:
         - 0: Errors,
         - 1: Warnings,
         - 2: All
     Defaults to 0
     :type verbose: int, optional
-    :param species: Biochemical species to which the data belongs.
+    :param data_type: Biochemical data_type to which the data belongs.
     Options: `protein`, `DNA`, `RNA`, or `small_molecule`; defaults to
     'protein'
-    :type species: str, optional
+    :type data_type: str, optional
     :param distance: Distance metrics for small molecule comparison.
     Currently, it is restricted to Tanimoto distance will
     be extended in future patches; if interested in a specific
     metric please let us know.
     Options:
         - `tanimoto`: Calculates the Tanimoto distance
     Defaults to 'tanimoto'.
@@ -357,15 +357,15 @@
     :type sim_df: Optional[pd.DataFrame], optional
     :return: A tuple with the indexes of training and evaluation samples
     or training, evaluation, and validation samples (if valid_size > 0).
     :rtype: Union[Tuple[list, list], Tuple[list, list, list]]
     """
     df = similarity_reduction(df, similarity_metric, field_name,
                               threads, clustering_mode, denominator,
-                              test_size, threshold, verbose, species,
+                              test_size, threshold, verbose, data_type,
                               representation, bits,
                               radius, sim_df, config)
     train, test = random_partition(df.index.tolist(), test_size=test_size,
                                    random_state=random_state)
     if valid_size > 0:
         adjust_valid = valid_size / (1 - test_size)
         train, valid = random_partition(train, test_size=adjust_valid,
@@ -383,15 +383,15 @@
     threads: int = cpu_count(),
     denominator: str = None,
     test_size: float = 0.0,
     valid_size: float = 0.0,
     threshold: float = 0.3,
     verbose: int = 2,
     n_parts: int = 10,
-    species: str = 'protein',
+    data_type: str = 'protein',
     distance: str = 'tanimoto',
     representation: str = '3di+aa',
     bits: int = 1024,
     radius: int = 2,
     config: dict = None,
     sim_df: Optional[pd.DataFrame] = None
 ):
@@ -449,18 +449,18 @@
     :param verbose: How much information will be displayed.
     Options:
         - 0: Errors,
         - 1: Warnings,
         - 2: All
     Defaults to 0
     :type verbose: int, optional
-    :param species: Biochemical species to which the data belongs.
+    :param data_type: Biochemical data_type to which the data belongs.
     Options: `protein`, `DNA`, `RNA`, or `small_molecule`; defaults to
     'protein'
-    :type species: str, optional
+    :type data_type: str, optional
     :param distance: Distance metrics for small molecule comparison.
     Currently, it is restricted to Tanimoto distance will
     be extended in future patches; if interested in a specific
     metric please let us know.
     Options:
         - `tanimoto`: Calculates the Tanimoto distance
     Defaults to 'tanimoto'.
@@ -493,15 +493,15 @@
     :type sim_df: Optional[pd.DataFrame], optional
     :return: A tuple with the indexes of training and evaluation samples
     or training, evaluation, and validation samples (if valid_size > 0).
     :rtype: Union[Tuple[list, list], Tuple[list, list, list]]
     """
     if sim_df is None:
         sim_df = calculate_similarity(
-            df, df, species=species,
+            df, df, data_type=data_type,
             similarity_metric=similarity_metric,
             field_name=field_name, threshold=threshold,
             threads=threads, verbose=verbose,
             save_alignment=False, filename=None, distance=distance,
             bits=bits, denominator=denominator, radius=radius,
             representation=representation, config=config
         )
```

### Comparing `hestia-ood-0.0.6/hestia/reduction.py` & `hestia_ood-0.0.8/hestia/reduction.py`

 * *Files identical despite different names*

### Comparing `hestia-ood-0.0.6/hestia/similarity.py` & `hestia_ood-0.0.8/hestia/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     matrix = spr.csr_matrix(spr.vstack(all_rows))
     return matrix.maximum(matrix.transpose())
 
 
 def calculate_similarity(
     df_query: pd.DataFrame,
     df_target: pd.DataFrame = None,
-    species: str = 'protein',
+    data_type: str = 'protein',
     similarity_metric: str = 'mmseqs+prefilter',
     field_name: str = 'sequence',
     threshold: float = 0.3,
     threads: int = cpu_count(),
     verbose: int = 0,
     save_alignment: bool = False,
     filename: str = None,
@@ -73,18 +73,18 @@
 
     :param df_query: DataFrame with query entities to calculate similarities
     :type df_query: pd.DataFrame
     :param df_target: DataFrame with target entities to calculate
     similarities. If not specified, the `df_query` will be used as `df_target`
     as well, defaults to None
     :type df_target: pd.DataFrame, optional
-    :param species: Biochemical species to which the data belongs.
+    :param data_type: Biochemical data_type to which the data belongs.
     Options: `protein`, `DNA`, `RNA`, or `small_molecule`; defaults to
     'protein'
-    :type species: str, optional
+    :type data_type: str, optional
     :param similarity_metric: Similarity function to use.
     Options:
         - `protein`: `mmseqs` (local alignment),
           `mmseqs+prefilter` (fast local alignment), `needle` (global
            alignment), or `foldseek` (structural alignment).
         - `DNA` or `RNA`: `mmseqs` (local alignment),
           `mmseqs+prefilter` (fast local alignment), or `needle`
@@ -154,29 +154,29 @@
         - "gapopen": 10,
         - "gapextend": 0.5,
         - "endweight": True,
         - "endopen": 10,
         - "endextend": 0.5,
         - "matrix": "EBLOSUM62"
     :type config: dict, optional
-    :raises NotImplementedError: Biochemical species is not supported
-                                 see `species`.
+    :raises NotImplementedError: Biochemical data_type is not supported
+                                 see `data_type`.
     :raises NotImplementedError: Similarity metric is not supported
                                  see `similarity_algorithm`
     :return: DataFrame with similarities (`metric`) between
     `query` and `target`.
     `query` and `target` are named as the indexes obtained from the 
     `pd.unique` function on the corresponding input DataFrames.
     :rtype: pd.DataFrame
     """
     mssg = f'Alignment method: {similarity_metric} '
-    mssg += f'not implemented for species: {species}'
-    mssg2 = f'Species: {species} not supported'
+    mssg += f'not implemented for data_type: {data_type}'
+    mssg2 = f'data_type: {data_type} not supported'
 
-    if species == 'protein':
+    if data_type == 'protein':
         if 'mmseqs' in similarity_metric:
             sim_df = _mmseqs2_alignment(
                 df_query=df_query,
                 df_target=df_target,
                 field_name=field_name,
                 threshold=threshold,
                 threads=threads,
@@ -212,17 +212,17 @@
                 threads=threads,
                 verbose=verbose,
                 save_alignment=save_alignment,
                 filename=filename
             )
         else:
             mssg = f'Alignment method: {similarity_metric} '
-            mssg += f'not implemented for species: {species}'
+            mssg += f'not implemented for data_type: {data_type}'
             raise NotImplementedError(mssg)
-    elif species.upper() == 'DNA' or species.upper() == 'RNA':
+    elif data_type.upper() == 'DNA' or data_type.upper() == 'RNA':
         if 'mmseqs' in similarity_metric:
             sim_df = _mmseqs2_alignment(
                 df_query=df_query,
                 df_target=df_target,
                 field_name=field_name,
                 threshold=threshold,
                 threads=threads,
@@ -244,17 +244,17 @@
                 verbose=verbose,
                 config=config,
                 save_alignment=save_alignment,
                 filename=filename
             )
         else:
             mssg = f'Alignment method: {similarity_metric} '
-            mssg += f'not implemented for species: {species}'
+            mssg += f'not implemented for data_type: {data_type}'
             raise NotImplementedError(mssg)
-    elif species == 'small_molecule' or species.lower() == 'smiles':
+    elif data_type == 'small_molecule' or data_type.lower() == 'smiles':
         if similarity_metric == 'scaffold':
             sim_df = _scaffold_alignment(
                 df_query=df_query,
                 df_target=df_target,
                 field_name=field_name,
                 threads=threads,
                 verbose=verbose,
@@ -271,14 +271,17 @@
                 threads=threads,
                 verbose=verbose,
                 bits=bits,
                 radius=radius,
                 save_alignment=save_alignment,
                 filename=filename
             )
+        else:
+            mssg = f'Alignment method: {similarity_metric} '
+            mssg += f'not implemented for data_type: {data_type}'
     else:
         raise NotImplementedError(mssg2)
     return sim_df
 
 
 def _scaffold_alignment(
     df_query: pd.DataFrame,
@@ -450,24 +453,23 @@
     if df_target is None:
         df_target = df_query
         target_fps = query_fps
     else:
         target_fps = thread_map(_get_fp, df_query[field_name],
                                 max_workers=threads)
 
-    chunk_size = threads * 100
+    chunk_size = threads * 1_000
     chunks_target = (len(df_target) // chunk_size) + 1
     queries, targets, metrics = [], [], []
     pbar = tqdm(range(len(query_fps)))
 
     with ThreadPoolExecutor(max_workers=threads) as executor:
         for chunk in pbar:
             jobs = []
             for chunk_t in range(chunks_target):
-                pbar.set_description(f'Covered: {chunk_t:,} / {chunks_target:,}')
                 start_t = chunk_t * chunk_size
                 if chunk_t == chunks_target - 1:
                     end_t = -1
                 else:
                     end_t = (chunk_t + 1) * chunk_size
                 chunk_fps = target_fps[start_t:end_t]
                 query_fp = query_fps[chunk]
```

### Comparing `hestia-ood-0.0.6/hestia/utils/file_format.py` & `hestia_ood-0.0.8/hestia/utils/file_format.py`

 * *Files identical despite different names*

### Comparing `hestia-ood-0.0.6/hestia/utils/graph_part_utils.py` & `hestia_ood-0.0.8/hestia/utils/graph_part_utils.py`

 * *Files identical despite different names*

### Comparing `hestia-ood-0.0.6/hestia/utils/label_balance.py` & `hestia_ood-0.0.8/hestia/utils/label_balance.py`

 * *Files identical despite different names*

### Comparing `hestia-ood-0.0.6/setup.py` & `hestia_ood-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 
 this_directory = Path(__file__).parent
 readme = (this_directory / "README.md").read_text()
 
-requirements = [ 
+requirements = [
     'networkx',
     'scipy',
     'scikit-learn',
     'pandas',
     'numpy',
-    'rdkit',
     'tqdm'
 ]
 
 test_requirements = requirements
 
 setup(
-author="Raul Fernandez-Diaz",
+    author="Raul Fernandez-Diaz",
     author_email='raul.fernandezdiaz@ucdconnect.ie',
     python_requires='>=3.9',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
@@ -41,13 +40,14 @@
     install_requires=requirements,
     license="MIT",
     long_description=readme + '\n\n',
     include_package_data=True,
     keywords='hestia',
     name='hestia-ood',
     packages=find_packages(),
+    long_description_content_type="text/markdown",
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/IBM/Hestia-OOD',
-    version='0.0.6',
+    version='0.0.8',
     zip_safe=False,
 )
```

