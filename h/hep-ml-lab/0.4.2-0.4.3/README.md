# Comparing `tmp/hep_ml_lab-0.4.2.tar.gz` & `tmp/hep_ml_lab-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_ml_lab-0.4.2.tar", max compression
+gzip compressed data, was "hep_ml_lab-0.4.3.tar", max compression
```

## Comparing `hep_ml_lab-0.4.2.tar` & `hep_ml_lab-0.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1064 2023-12-23 08:40:53.016508 hep_ml_lab-0.4.2/LICENSE
--rw-r--r--   0        0        0     3694 2024-04-29 08:02:51.513509 hep_ml_lab-0.4.2/README.md
--rw-r--r--   0        0        0      193 2024-04-29 07:58:59.817508 hep_ml_lab-0.4.2/hml/__init__.py
--rw-r--r--   0        0        0      530 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/__init__.py
--rw-r--r--   0        0        0       92 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/cuts/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/approaches/cuts/cut.py
--rw-r--r--   0        0        0     7318 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.2/hml/approaches/cuts/cut_and_count.py
--rw-r--r--   0        0        0     4244 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/cuts/cut_layer.py
--rw-r--r--   0        0        0       84 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/__init__.py
--rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/cnns/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/approaches/networks/cnns/simple_cnn.py
--rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/gnns/__init__.py
--rw-r--r--   0        0        0       25 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/gnns/simple_gnn.py
--rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/mlps/__init__.py
--rw-r--r--   0        0        0      904 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.2/hml/approaches/networks/mlps/simple_mlp.py
--rw-r--r--   0        0        0       72 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/approaches/trees/__init__.py
--rw-r--r--   0        0        0     9251 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.2/hml/approaches/trees/gradient_boosted_decision_tree.py
--rw-r--r--   0        0        0      552 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/__init__.py
--rw-r--r--   0        0        0       25 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/demo_z_tagging.py
--rw-r--r--   0        0        0       28 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/graph_dataset.py
--rw-r--r--   0        0        0    10756 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/datasets/image_dataset.py
--rw-r--r--   0        0        0     8442 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/datasets/set_dataset.py
--rw-r--r--   0        0        0       47 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.2/hml/generators/__init__.py
--rw-r--r--   0        0        0    17799 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.2/hml/generators/madgraph5.py
--rw-r--r--   0        0        0      148 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/metrics/__init__.py
--rw-r--r--   0        0        0     2463 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/metrics/max_significance.py
--rw-r--r--   0        0        0     1205 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/metrics/rejection_at_efficiency.py
--rw-r--r--   0        0        0     1384 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/__init__.py
--rw-r--r--   0        0        0     1771 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/angular_distance.py
--rw-r--r--   0        0        0      431 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/charge.py
--rw-r--r--   0        0        0     1174 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/invariant_mass.py
--rw-r--r--   0        0        0     2874 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/kinematics.py
--rw-r--r--   0        0        0     3812 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/n_subjettiness.py
--rw-r--r--   0        0        0     6437 2024-04-29 09:02:20.361529 hep_ml_lab-0.4.2/hml/observables/observable.py
--rw-r--r--   0        0        0      848 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/size.py
--rw-r--r--   0        0        0      743 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.2/hml/observables/tag.py
--rw-r--r--   0        0        0      235 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/__init__.py
--rw-r--r--   0        0        0      637 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/fastjet_ops.py
--rw-r--r--   0        0        0     1305 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/keras_ops.py
--rw-r--r--   0        0        0        0 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/repr_ops.py
--rw-r--r--   0        0        0     5529 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/operations/uproot_ops.py
--rw-r--r--   0        0        0     1056 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.2/hml/physics_objects/__init__.py
--rw-r--r--   0        0        0     1969 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/collective.py
--rw-r--r--   0        0        0     2227 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/multiple.py
--rw-r--r--   0        0        0     1800 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/nested.py
--rw-r--r--   0        0        0     1228 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/physics_object.py
--rw-r--r--   0        0        0     1256 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/physics_objects/single.py
--rw-r--r--   0        0        0       71 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/representations/__init__.py
--rw-r--r--   0        0        0       21 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.2/hml/representations/graph.py
--rw-r--r--   0        0        0    17647 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.2/hml/representations/image.py
--rw-r--r--   0        0        0     2545 2024-04-29 09:02:20.361529 hep_ml_lab-0.4.2/hml/representations/set.py
--rw-r--r--   0        0        0     1872 2024-04-29 07:58:52.317508 hep_ml_lab-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 hep_ml_lab-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-12-23 08:40:53.016508 hep_ml_lab-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3998 2024-05-03 09:43:38.031500 hep_ml_lab-0.4.3/README.md
+-rw-r--r--   0        0        0      193 2024-04-30 07:56:24.113996 hep_ml_lab-0.4.3/hml/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/cuts/__init__.py
+-rw-r--r--   0        0        0     3410 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/approaches/cuts/cut.py
+-rw-r--r--   0        0        0     7318 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.3/hml/approaches/cuts/cut_and_count.py
+-rw-r--r--   0        0        0     4244 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/cuts/cut_layer.py
+-rw-r--r--   0        0        0       84 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/networks/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/networks/cnns/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/approaches/networks/cnns/simple_cnn.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/networks/gnns/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/networks/gnns/simple_gnn.py
+-rw-r--r--   0        0        0       34 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/networks/mlps/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-22 13:52:21.094204 hep_ml_lab-0.4.3/hml/approaches/networks/mlps/simple_mlp.py
+-rw-r--r--   0        0        0       72 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.3/hml/approaches/trees/__init__.py
+-rw-r--r--   0        0        0     9251 2024-04-24 08:39:13.799076 hep_ml_lab-0.4.3/hml/approaches/trees/gradient_boosted_decision_tree.py
+-rw-r--r--   0        0        0      552 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.3/hml/datasets/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.3/hml/datasets/demo_z_tagging.py
+-rw-r--r--   0        0        0       28 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.3/hml/datasets/graph_dataset.py
+-rw-r--r--   0        0        0    10756 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.3/hml/datasets/image_dataset.py
+-rw-r--r--   0        0        0     8108 2024-04-30 12:18:09.154085 hep_ml_lab-0.4.3/hml/datasets/set_dataset.py
+-rw-r--r--   0        0        0       47 2024-04-22 13:52:21.106204 hep_ml_lab-0.4.3/hml/generators/__init__.py
+-rw-r--r--   0        0        0    18448 2024-05-02 01:52:42.782851 hep_ml_lab-0.4.3/hml/generators/madgraph5.py
+-rw-r--r--   0        0        0      148 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/metrics/__init__.py
+-rw-r--r--   0        0        0     4617 2024-05-01 10:49:17.942544 hep_ml_lab-0.4.3/hml/metrics/max_significance.py
+-rw-r--r--   0        0        0     1205 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/metrics/rejection_at_efficiency.py
+-rw-r--r--   0        0        0     1384 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/__init__.py
+-rw-r--r--   0        0        0     1771 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/angular_distance.py
+-rw-r--r--   0        0        0      431 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/charge.py
+-rw-r--r--   0        0        0     1174 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/invariant_mass.py
+-rw-r--r--   0        0        0     2874 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/kinematics.py
+-rw-r--r--   0        0        0     3812 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/n_subjettiness.py
+-rw-r--r--   0        0        0     6437 2024-04-29 09:11:38.781533 hep_ml_lab-0.4.3/hml/observables/observable.py
+-rw-r--r--   0        0        0      848 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/size.py
+-rw-r--r--   0        0        0      743 2024-04-29 07:57:23.649507 hep_ml_lab-0.4.3/hml/observables/tag.py
+-rw-r--r--   0        0        0      235 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/operations/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/operations/fastjet_ops.py
+-rw-r--r--   0        0        0     1305 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/operations/keras_ops.py
+-rw-r--r--   0        0        0        0 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/operations/repr_ops.py
+-rw-r--r--   0        0        0     5529 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/operations/uproot_ops.py
+-rw-r--r--   0        0        0     1056 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.3/hml/physics_objects/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/physics_objects/collective.py
+-rw-r--r--   0        0        0     2227 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/physics_objects/multiple.py
+-rw-r--r--   0        0        0     1800 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/physics_objects/nested.py
+-rw-r--r--   0        0        0     1228 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/physics_objects/physics_object.py
+-rw-r--r--   0        0        0     1256 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/physics_objects/single.py
+-rw-r--r--   0        0        0       71 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/representations/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-22 13:52:21.110204 hep_ml_lab-0.4.3/hml/representations/graph.py
+-rw-r--r--   0        0        0    17647 2024-04-24 08:39:13.803076 hep_ml_lab-0.4.3/hml/representations/image.py
+-rw-r--r--   0        0        0     2545 2024-04-29 09:02:20.361529 hep_ml_lab-0.4.3/hml/representations/set.py
+-rw-r--r--   0        0        0     1892 2024-04-30 07:57:24.929997 hep_ml_lab-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5294 1970-01-01 00:00:00.000000 hep_ml_lab-0.4.3/PKG-INFO
```

### Comparing `hep_ml_lab-0.4.2/LICENSE` & `hep_ml_lab-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/README.md` & `hep_ml_lab-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.approaches`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
 ## Updates
 
+### v0.4.3
+- Fix the thresholds issue in `hml.metrics.MaxSignificance` by making it similar to the one returned by `sklearn.metrics.roc_curve`.
+- Change `hml.datasets.SetDataset.show` to display figures using `seaborn`. 
+- Drop the requirement of `executable` in `hml.generators.Madgraph5.from_output`.
+
 ### v0.4.2
 - Fix parsing cuts like "muon0.charge != muon1.charge".
 - Fix inconsistent model layers in `hml.approaches.networks.SimpleCNN`.
 - Fix registering and saving custom observables.
 - Add cross sections, luminosity and weights as parameters in `hml.metrics.MaxSignificance`.
 - Improve the figure ratio in `hml.datasets.SetDataset.show`.
```

### Comparing `hep_ml_lab-0.4.2/hml/approaches/__init__.py` & `hep_ml_lab-0.4.3/hml/approaches/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/approaches/cuts/cut.py` & `hep_ml_lab-0.4.3/hml/approaches/cuts/cut.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/approaches/cuts/cut_and_count.py` & `hep_ml_lab-0.4.3/hml/approaches/cuts/cut_and_count.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/approaches/cuts/cut_layer.py` & `hep_ml_lab-0.4.3/hml/approaches/cuts/cut_layer.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/approaches/networks/cnns/simple_cnn.py` & `hep_ml_lab-0.4.3/hml/approaches/networks/cnns/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/approaches/networks/mlps/simple_mlp.py` & `hep_ml_lab-0.4.3/hml/approaches/networks/mlps/simple_mlp.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/approaches/trees/gradient_boosted_decision_tree.py` & `hep_ml_lab-0.4.3/hml/approaches/trees/gradient_boosted_decision_tree.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/datasets/__init__.py` & `hep_ml_lab-0.4.3/hml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/datasets/image_dataset.py` & `hep_ml_lab-0.4.3/hml/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/datasets/set_dataset.py` & `hep_ml_lab-0.4.3/hml/datasets/set_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import reduce
 from io import BytesIO
 
 import awkward as ak
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import seaborn as sns
 from sklearn.model_selection import train_test_split
 
 from hml.approaches import Cut
 from hml.observables import Observable
 from hml.representations import Set
 
 
@@ -226,38 +227,29 @@
         instance = cls(set.observables)
         instance.been_split = config["been_split"]
         instance.seed = config["seed"]
 
         return instance
 
     def show(self, n_feature_per_line=3, n_samples=-1, target=None):
-        if n_samples != -1:
-            samples = self.samples[:n_samples]
-        else:
-            samples = self.samples
+        df = self.to_pandas()
+        df = df.sample(n=n_samples) if n_samples != -1 else df
 
         n_features = len(self.feature_names)
         n_rows = (n_features + n_feature_per_line - 1) // n_feature_per_line
         plt.figure(figsize=(4 * n_feature_per_line, 3 * n_rows))
+
         for i, name in enumerate(self.feature_names):
             ax = plt.subplot(n_rows, n_feature_per_line, i + 1)
 
-            if target is None:
-                for i_target in np.unique(self.targets):
-                    ax.hist(
-                        samples[np.squeeze(self.targets == i_target)][:, i],
-                        bins=50,
-                        histtype="step",
-                        label=f"Target {i_target}",
-                    )
-            else:
-                ax.hist(
-                    samples[np.squeeze(self.targets == i_target)][:, i],
-                    bins=50,
-                    histtype="step",
-                    label=f"Target {i_target}",
-                )
-            ax.set_title(name)
+            sns.histplot(
+                df if target is None else df.query(f"Target == {target}"),
+                x=name,
+                hue="Target",
+                bins=40,
+                element="step",
+                multiple="layer",
+            )
+            ax.grid(axis="y", alpha=0.5, linewidth=0.4)
 
-        plt.legend()
         plt.tight_layout()
         plt.show()
```

### Comparing `hep_ml_lab-0.4.2/hml/generators/madgraph5.py` & `hep_ml_lab-0.4.3/hml/generators/madgraph5.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,45 +17,60 @@
 
 class Madgraph5:
     def __init__(
         self,
         executable: PathLike,
         verbose: int = 1,
     ):
+        self.verbose = verbose
         self.executable = executable
-        self.child = pexpect.spawn(f"{self.executable.as_posix()}")
-        self.process_log = ""
         self.DEFAULT_LOG_DIR = Path("Logs")
         self.DEFAULT_DIAGRAM_DIR = Path("Diagrams")
-        self.verbose = verbose
-
-        self.process_log += self.run_command("")
 
     @property
     def executable(self) -> Path:
+        if self._executable is None:
+            raise AttributeError("Madgraph5 executable not set yet")
+
         return self._executable
 
     @executable.setter
-    def executable(self, value: PathLike):
-        if (_executable := shutil.which(value)) is None:
+    def executable(self, value: PathLike | None):
+        if value is None:
+            self._executable = value
+
+        elif shutil.which(value) is None:
             raise FileNotFoundError(f"Could not find Madgraph5 executable {value}")
 
-        self._executable = Path(_executable).resolve()
+        else:
+            self._executable = Path(shutil.which(value)).resolve()
+            self.child = pexpect.spawn(f"{self._executable.as_posix()}")
+            self.process_log = self.run_command("")
 
     @property
-    def home(self) -> Path:
-        return self.executable.parent.parent
+    def home(self) -> Path | None:
+        if self._executable is not None:
+            return self.executable.parent.parent
 
     @property
     def version(self) -> str:
         _version = "unknown"
-        with (self.home / "VERSION").open() as f:
-            for line in f.readlines():
-                if line.startswith("version") and _version == "unknown":
-                    _version = line.split("=")[1].strip()
+
+        if self.home is not None:
+            with (self.home / "VERSION").open() as f:
+                for line in f.readlines():
+                    if line.startswith("version") and _version == "unknown":
+                        _version = line.split("=")[1].strip()
+
+        elif _version == "unknown" and hasattr(self, "output_dir"):
+            if (version_file := self.output_dir / "MGMEVersion.txt").exists():
+                with version_file.open() as f:
+                    content = f.readlines()
+                    if len(content) == 1:
+                        _version = content[0].strip()
 
         return _version
 
     def __repr__(self):
         return f"Madgraph5 v{self.version}"
 
     def run_command(
@@ -354,15 +369,19 @@
                 f"{run.n_events:,}",
                 f"{run.seed}",
             )
 
         console.print(table)
 
     @classmethod
-    def from_output(cls, output_dir: PathLike, executable: PathLike) -> Madgraph5:
+    def from_output(
+        cls,
+        output_dir: PathLike,
+        executable: PathLike | None = None,
+    ) -> Madgraph5:
         output_dir = Path(output_dir)
         if not output_dir.exists():
             raise FileNotFoundError(f"Output directory {output_dir} does not exist")
 
         output_dir = output_dir.resolve()
         mg5 = cls(executable, verbose=0)
         mg5.verbose = 1
```

### Comparing `hep_ml_lab-0.4.2/hml/metrics/rejection_at_efficiency.py` & `hep_ml_lab-0.4.3/hml/metrics/rejection_at_efficiency.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/__init__.py` & `hep_ml_lab-0.4.3/hml/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/angular_distance.py` & `hep_ml_lab-0.4.3/hml/observables/angular_distance.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/invariant_mass.py` & `hep_ml_lab-0.4.3/hml/observables/invariant_mass.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/kinematics.py` & `hep_ml_lab-0.4.3/hml/observables/kinematics.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/n_subjettiness.py` & `hep_ml_lab-0.4.3/hml/observables/n_subjettiness.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/observable.py` & `hep_ml_lab-0.4.3/hml/observables/observable.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/size.py` & `hep_ml_lab-0.4.3/hml/observables/size.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/observables/tag.py` & `hep_ml_lab-0.4.3/hml/observables/tag.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/operations/fastjet_ops.py` & `hep_ml_lab-0.4.3/hml/operations/fastjet_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/operations/keras_ops.py` & `hep_ml_lab-0.4.3/hml/operations/keras_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/operations/uproot_ops.py` & `hep_ml_lab-0.4.3/hml/operations/uproot_ops.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/physics_objects/__init__.py` & `hep_ml_lab-0.4.3/hml/physics_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/physics_objects/collective.py` & `hep_ml_lab-0.4.3/hml/physics_objects/collective.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/physics_objects/multiple.py` & `hep_ml_lab-0.4.3/hml/physics_objects/multiple.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/physics_objects/nested.py` & `hep_ml_lab-0.4.3/hml/physics_objects/nested.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/physics_objects/physics_object.py` & `hep_ml_lab-0.4.3/hml/physics_objects/physics_object.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/physics_objects/single.py` & `hep_ml_lab-0.4.3/hml/physics_objects/single.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/representations/image.py` & `hep_ml_lab-0.4.3/hml/representations/image.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/hml/representations/set.py` & `hep_ml_lab-0.4.3/hml/representations/set.py`

 * *Files identical despite different names*

### Comparing `hep_ml_lab-0.4.2/pyproject.toml` & `hep_ml_lab-0.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hep-ml-lab"
-version = "0.4.2"
+version = "0.4.3"
 description = "An end-to-end framework used for research combining high-energy physics phenomenology with machine learning."
 license = "MIT"
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
 homepage = "https://github.com/Star9daisy/hep-ml-lab"
 documentation = "https://star9daisy.github.io/hep-ml-lab/"
 keywords = ["high energy physics", "machine learning", "framework"]
@@ -22,14 +22,15 @@
 pexpect = "^4.9.0"
 awkward = "^2.5.1"
 fastjet = "^3.4.1.3"
 matplotlib = "^3.8.2"
 vector = "^1.3.0"
 numba = "^0.59.0"
 keras = ">=3.0.0"
+seaborn = "^0.13.2"
 
 [tool.poetry.group.dev.dependencies]
 deptry = "^0.12.0"
 mkdocs = "^1.4.3"
 mkdocs-exclude = "^1.0.2"
 mkdocs-material = "^9.1.15"
 mkdocstrings = { extras = ["python"], version = "^0.22.0" }
```

### Comparing `hep_ml_lab-0.4.2/PKG-INFO` & `hep_ml_lab-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-ml-lab
-Version: 0.4.2
+Version: 0.4.3
 Summary: An end-to-end framework used for research combining high-energy physics phenomenology with machine learning.
 Home-page: https://github.com/Star9daisy/hep-ml-lab
 License: MIT
 Keywords: high energy physics,machine learning,framework
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.9,<3.12
@@ -21,14 +21,15 @@
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numba (>=0.59.0,<0.60.0)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pexpect (>=4.9.0,<5.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: vector (>=1.3.0,<2.0.0)
 Project-URL: Documentation, https://star9daisy.github.io/hep-ml-lab/
 Description-Content-Type: text/markdown
 
 # HEP ML Lab (HML)
 [![PyPI - Version](https://img.shields.io/pypi/v/hep-ml-lab)](https://pypi.org/project/hep-ml-lab/)
 [![Downloads](https://static.pepy.tech/badge/hep-ml-lab)](https://pepy.tech/project/hep-ml-lab)
@@ -64,14 +65,19 @@
 - `hml.representations`: Different data structure used to represent an event;
 - `hml.datasets`: Existing datasets and helper classes for creating new datasets;
 - `hml.approaches`: Cuts, trees and networks for classification;
 - `hml.metrics`: Metrics used in classical signal vs background analysis;
 
 ## Updates
 
+### v0.4.3
+- Fix the thresholds issue in `hml.metrics.MaxSignificance` by making it similar to the one returned by `sklearn.metrics.roc_curve`.
+- Change `hml.datasets.SetDataset.show` to display figures using `seaborn`. 
+- Drop the requirement of `executable` in `hml.generators.Madgraph5.from_output`.
+
 ### v0.4.2
 - Fix parsing cuts like "muon0.charge != muon1.charge".
 - Fix inconsistent model layers in `hml.approaches.networks.SimpleCNN`.
 - Fix registering and saving custom observables.
 - Add cross sections, luminosity and weights as parameters in `hml.metrics.MaxSignificance`.
 - Improve the figure ratio in `hml.datasets.SetDataset.show`.
```

