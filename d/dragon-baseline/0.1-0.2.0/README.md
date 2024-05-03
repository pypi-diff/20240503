# Comparing `tmp/dragon_baseline-0.1.tar.gz` & `tmp/dragon_baseline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragon_baseline-0.1.tar", last modified: Tue Nov 14 14:26:46 2023, max compression
+gzip compressed data, was "dragon_baseline-0.2.0.tar", last modified: Fri May  3 12:01:10 2024, max compression
```

## Comparing `dragon_baseline-0.1.tar` & `dragon_baseline-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-14 14:26:46.308725 dragon_baseline-0.1/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_baseline-0.1/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1426 2023-11-14 14:26:46.308674 dragon_baseline-0.1/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      136 2023-11-13 10:41:08.000000 dragon_baseline-0.1/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      504 2023-11-02 16:39:08.000000 dragon_baseline-0.1/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      879 2023-11-14 14:26:46.308987 dragon_baseline-0.1/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)      734 2023-11-13 10:42:28.000000 dragon_baseline-0.1/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-14 14:26:46.303357 dragon_baseline-0.1/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-14 14:26:46.305059 dragon_baseline-0.1/src/dragon_baseline/
--rw-r--r--   0 joeranbosma   (501) staff       (20)       85 2023-11-13 10:46:15.000000 dragon_baseline-0.1/src/dragon_baseline/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1523 2023-11-13 10:58:40.000000 dragon_baseline-0.1/src/dragon_baseline/__main__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-14 14:26:46.308059 dragon_baseline-0.1/src/dragon_baseline/architectures/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-11-13 10:43:50.000000 dragon_baseline-0.1/src/dragon_baseline/architectures/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5957 2023-11-13 10:46:35.000000 dragon_baseline-0.1/src/dragon_baseline/architectures/clf_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7494 2023-11-13 10:47:28.000000 dragon_baseline-0.1/src/dragon_baseline/architectures/ner_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5752 2023-11-13 10:47:35.000000 dragon_baseline-0.1/src/dragon_baseline/architectures/reg_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    24842 2023-11-14 14:25:44.000000 dragon_baseline-0.1/src/dragon_baseline/main.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    16722 2023-11-14 13:06:20.000000 dragon_baseline-0.1/src/dragon_baseline/nlp_algorithm.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    34016 2023-11-02 16:39:08.000000 dragon_baseline-0.1/src/dragon_baseline/run_classification.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    35990 2023-11-02 16:39:08.000000 dragon_baseline-0.1/src/dragon_baseline/run_classification_multi_label.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29097 2023-11-02 16:39:08.000000 dragon_baseline-0.1/src/dragon_baseline/run_ner.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    27004 2023-11-02 16:39:08.000000 dragon_baseline-0.1/src/dragon_baseline/run_ner_multi_label_binary.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-14 14:26:46.306028 dragon_baseline-0.1/src/dragon_baseline.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1426 2023-11-14 14:26:46.000000 dragon_baseline-0.1/src/dragon_baseline.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      815 2023-11-14 14:26:46.000000 dragon_baseline-0.1/src/dragon_baseline.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-14 14:26:46.000000 dragon_baseline-0.1/src/dragon_baseline.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-13 11:58:50.000000 dragon_baseline-0.1/src/dragon_baseline.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      177 2023-11-14 14:26:46.000000 dragon_baseline-0.1/src/dragon_baseline.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       16 2023-11-14 14:26:46.000000 dragon_baseline-0.1/src/dragon_baseline.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.969351 dragon_baseline-0.2.0/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_baseline-0.2.0/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-03 12:01:10.969283 dragon_baseline-0.2.0/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      136 2023-11-13 10:41:08.000000 dragon_baseline-0.2.0/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      504 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      879 2024-05-03 12:01:10.969712 dragon_baseline-0.2.0/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      736 2024-05-03 11:58:27.000000 dragon_baseline-0.2.0/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.962697 dragon_baseline-0.2.0/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.966286 dragon_baseline-0.2.0/src/dragon_baseline/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       85 2023-11-13 10:46:15.000000 dragon_baseline-0.2.0/src/dragon_baseline/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1346 2024-03-05 15:10:45.000000 dragon_baseline-0.2.0/src/dragon_baseline/__main__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.968241 dragon_baseline-0.2.0/src/dragon_baseline/architectures/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-11-13 10:43:50.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5957 2023-11-13 10:46:35.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/clf_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7494 2023-11-13 10:47:28.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/ner_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5752 2023-11-13 10:47:35.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/reg_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    33112 2024-05-03 11:54:34.000000 dragon_baseline-0.2.0/src/dragon_baseline/main.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    18567 2024-03-05 15:10:45.000000 dragon_baseline-0.2.0/src/dragon_baseline/nlp_algorithm.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    34016 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/src/dragon_baseline/run_classification.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    35990 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/src/dragon_baseline/run_classification_multi_label.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29097 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/src/dragon_baseline/run_ner.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.968600 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      765 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-13 11:58:50.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      177 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       16 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/top_level.txt
```

### Comparing `dragon_baseline-0.1/LICENSE` & `dragon_baseline-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/PKG-INFO` & `dragon_baseline-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragon_baseline
-Version: 0.1
+Version: 0.2.0
 Summary: Baseline training algorithm for the DRAGON Challenge
 Home-page: https://github.com/DIAGNijmegen/dragon_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dragon_baseline/issues
 Platform: unix
 Platform: linux
```

### Comparing `dragon_baseline-0.1/setup.cfg` & `dragon_baseline-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/setup.py` & `dragon_baseline-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == "__main__":
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version="0.1",
+        version="0.2.0",
         author_email="Joeran.Bosma@radboudumc.nl",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/DIAGNijmegen/dragon_baseline",
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/dragon_baseline/issues"
         },
```

### Comparing `dragon_baseline-0.1/src/dragon_baseline/__main__.py` & `dragon_baseline-0.2.0/src/dragon_baseline/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,25 +14,21 @@
 
 import sys
 
 from dragon_baseline.run_classification import main as run_classification
 from dragon_baseline.run_classification_multi_label import \
     main as run_classification_multi_label
 from dragon_baseline.run_ner import main as run_ner
-from dragon_baseline.run_ner_multi_label_binary import \
-    main as run_ner_multi_label_binary
 
 if __name__ == '__main__':
     if len(sys.argv) < 2:
         raise ValueError("First argument must specify the problem type")
 
     problem_type = sys.argv.pop(1)
     if problem_type == "ner":
         run_ner()
-    elif problem_type == "multi_label_ner":
-        run_ner_multi_label_binary()
     elif problem_type == "classification":
         run_classification()
     elif problem_type == "multi_label_classification":
         run_classification_multi_label()
     else:
         raise ValueError(f"Unexpected problem type: {problem_type}.")
```

### Comparing `dragon_baseline-0.1/src/dragon_baseline/architectures/__init__.py` & `dragon_baseline-0.2.0/src/dragon_baseline/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline/architectures/clf_multi_head.py` & `dragon_baseline-0.2.0/src/dragon_baseline/architectures/clf_multi_head.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline/architectures/ner_multi_head.py` & `dragon_baseline-0.2.0/src/dragon_baseline/architectures/ner_multi_head.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline/architectures/reg_multi_head.py` & `dragon_baseline-0.2.0/src/dragon_baseline/architectures/reg_multi_head.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline/main.py` & `dragon_baseline-0.2.0/src/dragon_baseline/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import re
 import subprocess
 from pathlib import Path
 from typing import List
 
 import numpy as np
 import pandas as pd
 import torch
@@ -66,14 +67,120 @@
         # Reverse the standard scaling
         inv_X = self.standard_scaler.inverse_transform(X)
 
         # Reverse the log(1 + value) transformation
         return np.expm1(inv_X)
 
 
+def merge_overlapping_labels(tags: list[list[str]]) -> list[list[str]]:
+    """Function to merge overlapping labels"""
+    merged_tags = []
+    for tag_group in tags:
+        if len(tag_group) > 1:
+            # Split each tag into its prefix (B/I) and entity
+            split_tags = [tag.split('-', 1) for tag in tag_group]
+            # Group tags by their prefixes
+            prefix_groups = {}
+            for prefix, entity in split_tags:
+                if prefix in prefix_groups:
+                    prefix_groups[prefix].append(entity)
+                else:
+                    prefix_groups[prefix] = [entity]
+            # Merge entities with the same prefix
+            merged_group = [f'{prefix}-{"[MERGED]".join(entities)}' for prefix, entities in prefix_groups.items()]
+            merged_tags.append(merged_group)
+        else:
+            merged_tags.append(tag_group)
+    return merged_tags
+
+
+def split_merged_labels(tags: list[list[str]]) -> list[list[str]]:
+    """Function to split merged labels"""
+    split_tags = []
+    for tag_group in tags:
+        split_group = []
+        for tag in tag_group:
+            if tag == "O":
+                split_group.append(tag)
+                continue
+
+            # Split each tag into its prefix (B/I) and entity
+            prefix, entity = tag.split('-', 1)
+            # Split entities that were merged
+            if '[MERGED]' in entity:
+                split_entities = entity.split('[MERGED]')
+                for split_entity in split_entities:
+                    split_group.append(f'{prefix}-{split_entity}')
+            else:
+                split_group.append(tag)
+        split_tags.append(split_group)
+    return split_tags
+
+
+def select_entity_labels(df: pd.DataFrame, entity_number: str, label_name: str) -> pd.DataFrame:
+    df = df.copy()
+
+    # select the labels for the current entity number
+    df[label_name] = df[label_name].apply(lambda labels: [
+        [lbl.replace(f"-{entity_number}-", "-") for lbl in token_labels if re.match(f"^[BI]-{entity_number}-", lbl)]
+        for token_labels in labels
+    ])
+
+    # merge the labels for the current entity number if they overlap
+    labels_before = df[label_name].explode().explode()
+    labels_before = labels_before[labels_before.notna()].unique()
+    df[label_name] = df[label_name].apply(merge_overlapping_labels)
+    labels_after = df[label_name].explode().explode()
+    labels_after = labels_after[labels_after.notna()].unique()
+    labels_added = set(labels_after) - set(labels_before)
+    if labels_added:
+        print(f"Merged overlapping labels, {labels_before} -> {labels_after}")
+
+    if not df[label_name].apply(lambda labels: all(len(token_labels) <= 1 for token_labels in labels)).all():
+        raise ValueError("Expected all samples to have exactly one label per token after selecting the entity labels")
+
+    df[label_name] = df[label_name].apply(lambda labels: [
+        (token_labels[0] if len(token_labels) > 0 else "O")
+        for token_labels in labels
+    ])
+    df["block_number"] = entity_number
+    return df
+
+
+def split_multi_label_ner_samples(df: pd.DataFrame, entity_numbers: List[str], label_name: str) -> pd.DataFrame:
+    """
+    Splits multi-label NER samples in a DataFrame based on entity numbers.
+
+    When labels overlap even after splitting based on entity number (i.e. multiple labels for the same token), the labels are merged.
+
+    Args:
+        df (pd.DataFrame): The DataFrame containing the NER samples.
+        entity_numbers (List[str]): The list of entity numbers to split the samples.
+        label_name (str): The name of the label column in the DataFrame.
+
+    Returns:
+        pd.DataFrame: The DataFrame with the multi-label samples split based on entity numbers.
+    """
+    return pd.concat([
+        select_entity_labels(df=df, entity_number=entity_number, label_name=label_name)
+        for entity_number in entity_numbers
+    ], ignore_index=True)
+
+
+def balance_negative_samples(df: pd.DataFrame, label_name: str, seed: int) -> pd.DataFrame:
+    """Select an equal number of samples with a labeled entity, as ones with no labeled entity"""
+    mask = df[label_name].apply(lambda labels: any(any(lbl != "O" for lbl in token_labels) for token_labels in labels))
+
+    if len(df) > 2 * mask.sum():
+        # select a random subset of samples without an entity
+        df = pd.concat([df[mask], df[~mask].sample(n=mask.sum(), random_state=seed)], ignore_index=True)
+
+    return df
+
+
 class DragonBaseline(NLPAlgorithm):
     def __init__(self, input_path: Path = Path("/input"), output_path: Path = Path("/output"), workdir: Path = Path("/opt/app"), models_dir: Path = Path("/opt/app/models"), **kwargs):
         """
         Baseline implementation for the DRAGON Challenge (https://dragon.grand-challenge.org/).
         This baseline uses the HuggingFace Transformers library (https://huggingface.co/transformers/).
 
         The baseline must implement the following methods:
@@ -83,28 +190,102 @@
         """
         super().__init__(input_path=input_path, output_path=output_path, **kwargs)
 
         # default training settings
         self.model_name = models_dir / "distilbert-base-multilingual-cased"
         self.per_device_train_batch_size = 4
         self.gradient_accumulation_steps = 2
+        self.gradient_checkpointing = False
         self.max_seq_length = 512
         self.learning_rate = 3e-5
         self.num_train_epochs = 5
         self.warmup_ratio = 0.1
         self.load_best_model_at_end = True
         self.metric_for_best_model = "loss"
         self.fp16 = True
 
         # paths for saving the preprocessed data and model checkpoints
         self.nlp_dataset_train_preprocessed_path = Path(workdir / "nlp-dataset-train-preprocessed.json")
         self.nlp_dataset_val_preprocessed_path = Path(workdir / "nlp-dataset-val-preprocessed.json")
         self.nlp_dataset_test_preprocessed_path = Path(workdir / "nlp-dataset-test-preprocessed.json")
         self.model_save_dir = Path(workdir / "checkpoints")
 
+        # keep track of the common prefix of the reports, to remove it
+        self.common_prefix = None
+
+    @staticmethod
+    def longest_common_prefix(strs: List[str]) -> str:
+        if not strs:
+            return ""
+
+        # Assume the first string is the longest common prefix
+        prefix = strs[0]
+
+        # Compare the prefix with each string
+        for s in strs:
+            while not s.startswith(prefix):
+                # Reduce the prefix by one character at a time
+                prefix = prefix[:-1]
+                if not prefix:
+                    return ""
+        return prefix
+    
+    @staticmethod
+    def longest_common_prefix_tokenized(strs: List[List[str]]) -> List[str]:
+        """Find the longest common prefix of a list of tokenized strings."""
+        if not strs or not strs[0]:
+            return []
+
+        # Assume the first string is the longest common prefix
+        prefix = strs[0]
+
+        # Compare the prefix with each string
+        for s in strs:
+            # Check each token in the prefix
+            for i in range(len(prefix)):
+                # If the current string is shorter than the prefix length or tokens don't match
+                if i >= len(s) or prefix[i] != s[i]:
+                    # Reduce the prefix length
+                    prefix = prefix[:i]
+                    break
+
+            if not prefix:
+                return []
+
+        return prefix
+
+
+    def remove_common_prefix_from_reports(self):
+        """Remove the common prefix from the reports."""
+        # find the common prefix
+        if self.task.input_name == "text":
+            reports = self.df_train[self.task.input_name].to_list()
+            self.common_prefix = self.longest_common_prefix(reports)
+
+            if not self.common_prefix:
+                return
+
+            # remove the common prefix
+            print(f"Removing common prefix from all reports: {self.common_prefix}")
+            for df in [self.df_train, self.df_val, self.df_test]:
+                df[self.task.input_name] = df[self.task.input_name].apply(lambda x: re.sub(f"^{self.common_prefix}", "", x))
+        elif self.task.input_name == "text_parts":
+            reports = self.df_train[self.task.input_name].to_list()
+            self.common_prefix = self.longest_common_prefix_tokenized(reports)
+
+            if not self.common_prefix:
+                return
+
+            # remove the common prefix
+            print(f"Removing common prefix from all reports: {self.common_prefix}")
+            for df in [self.df_train, self.df_val, self.df_test]:
+                df[self.task.input_name] = df[self.task.input_name].apply(lambda x: x[len(self.common_prefix):])
+                if self.task.target.label_name in df.columns:
+                    df[self.task.target.label_name] = df[self.task.target.label_name].apply(lambda x: x[len(self.common_prefix):])
+
     def scale_labels(self) -> pd.DataFrame:
         """Scale the labels."""
         if self.task.target.problem_type in [ProblemType.SINGLE_LABEL_REGRESSION, ProblemType.MULTI_LABEL_REGRESSION]:
             if self.task.target.skew > 1:
                 scaler = CustomLogScaler()
             else:
                 scaler = StandardScaler()
@@ -129,27 +310,29 @@
                 predictions[self.task.target.prediction_name] = scaler.inverse_transform(predictions[self.task.target.prediction_name].values.reshape(-1, 1))
             elif self.task.target.problem_type == ProblemType.MULTI_LABEL_REGRESSION:
                 predictions[self.task.target.prediction_name] = predictions[self.task.target.prediction_name].apply(lambda x: np.ravel(scaler.inverse_transform(np.array(x).reshape(-1, 1))))
         return predictions
 
     def add_dummy_test_labels(self):
         """Add dummy labels for test data. This allows to use the dataset in the huggingface pipeline."""
-        if self.task.target.problem_type in [ProblemType.SINGLE_LABEL_NER, ProblemType.MULTI_LABEL_BINARY_NER]:
-            dummy_label = self.df_train[self.task.target.label_name].iloc[0][0]
+        if self.task.target.problem_type in [ProblemType.SINGLE_LABEL_NER, ProblemType.MULTI_LABEL_NER]:
+            train_labels = self.df_train[self.task.target.label_name].explode()
+            dummy_label = train_labels[~train_labels.isna()].iloc[0]
             self.df_test[self.task.target.label_name] = self.df_test.apply(lambda row: [dummy_label]*len(row[self.task.input_name]), axis=1)
         else:
             dummy_label = self.df_train[self.task.target.label_name].iloc[0]
             self.df_test[self.task.target.label_name] = [dummy_label]*len(self.df_test)
 
-    def prepare_labels(self):
+    def prepare_labels_for_huggingface(self):
         """
         Prepare labels for training in the HuggingFace pipeline.
 
         For multi-label binary classification tasks, convert the list of 0/1 ints to list of "labelX" strings.
-        For other multi-label tasks, convert the multiple values in the label column to one value per column.
+        For multi-label regression and multi-class classification tasks, convert the multiple values in the label column to one value per column.
+        For mutli-label NER tasks, split the samples into one sample per entity group.
         """
         if self.task.target.problem_type == ProblemType.MULTI_LABEL_BINARY_CLASSIFICATION:
             for df in [self.df_train, self.df_val, self.df_test]:
                 # convert list of 0/1 ints to list of "labelX" strings
                 df[self.task.target.label_name] = df[self.task.target.label_name].apply(lambda labels: [
                     f"label{i}" for i, lbl in enumerate(labels) if lbl == 1
                 ])
@@ -159,25 +342,53 @@
             ProblemType.MULTI_LABEL_REGRESSION,
             ProblemType.MULTI_LABEL_MULTI_CLASS_CLASSIFICATION,
         ]:
             num_labels = len(self.df_train[self.task.target.label_name].iloc[0])
             for df in [self.df_train, self.df_val, self.df_test]:
                 for i in range(num_labels):
                     df[f"{self.task.target.label_name}_{i}"] = df[self.task.target.label_name].apply(lambda x: x[i])
+        elif self.task.target.problem_type == ProblemType.MULTI_LABEL_NER:
+            # collect all unique labels and remove the "B-" and "I-" prefixes
+            self.task.target.values = sorted(set([
+                re.sub(r"^[BI]-", "", lbl)
+                for lbl in self.df_train[self.task.target.label_name].explode().explode().unique()
+                if lbl != "O"
+            ]))
+
+            if not all(re.match(r"^\d+-.+$", lbl) for lbl in self.task.target.values):
+                raise ValueError(f"Expected all labels to start with a number followed by a dash, but got {self.task.target.values}")
+
+            # split the samples into one sample per entity group
+            entity_numbers = sorted(set([lbl.split("-")[0] for lbl in self.task.target.values]))
+            self.df_train = split_multi_label_ner_samples(df=self.df_train, entity_numbers=entity_numbers, label_name=self.task.target.label_name)
+            self.df_val = split_multi_label_ner_samples(df=self.df_val, entity_numbers=entity_numbers, label_name=self.task.target.label_name)
+            self.df_test = split_multi_label_ner_samples(df=self.df_test, entity_numbers=entity_numbers, label_name=self.task.target.label_name)
+
+            # select an equal number of samples with a labeled entity, as ones with no labeled entity
+            self.df_train = balance_negative_samples(df=self.df_train, label_name=self.task.target.label_name, seed=self.task.jobid)
+            self.df_val = balance_negative_samples(df=self.df_val, label_name=self.task.target.label_name, seed=self.task.jobid)
+
+            # add block number to the text parts
+            for df in [self.df_train, self.df_val, self.df_test]:
+                df[self.task.input_name] = df.apply(lambda row: [row["block_number"]] + row[self.task.input_name], axis=1)
+                df[self.task.target.label_name] = df[self.task.target.label_name].apply(lambda labels: ["O"] + labels)
 
     def shuffle_train_data(self):
         """Shuffle the training data."""
         self.df_train = self.df_train.sample(frac=1, random_state=self.task.jobid)
 
     def preprocess(self):
         """Preprocess the data."""
-        # scale the labels
+        # prepare the reports
+        self.remove_common_prefix_from_reports()
+
+        # prepare the labels
         self.scale_labels()
         self.add_dummy_test_labels()
-        self.prepare_labels()
+        self.prepare_labels_for_huggingface()
         self.shuffle_train_data()
 
     def train(self):
         """Train the model."""
         # save the preprocessed data for training through command line interface of the HuggingFace library
         for path in [
             self.nlp_dataset_train_preprocessed_path,
@@ -189,18 +400,16 @@
         self.df_val.to_json(self.nlp_dataset_val_preprocessed_path, orient="records")
         self.df_test.to_json(self.nlp_dataset_test_preprocessed_path, orient="records")
 
         # load the tokenizer
         tokenizer = AutoTokenizer.from_pretrained(self.model_name, truncation_side=self.task.recommended_truncation_side)
 
         # train the model
-        if self.task.target.problem_type == ProblemType.SINGLE_LABEL_NER:
+        if self.task.target.problem_type in [ProblemType.SINGLE_LABEL_NER, ProblemType.MULTI_LABEL_NER]:
             trainer = "ner"
-        elif self.task.target.problem_type == ProblemType.MULTI_LABEL_BINARY_NER:
-            trainer = "multi_label_ner"
         elif self.task.target.problem_type in [ProblemType.MULTI_LABEL_REGRESSION, ProblemType.MULTI_LABEL_MULTI_CLASS_CLASSIFICATION]:
             trainer = "multi_label_classification"
         else:
             trainer = "classification"
 
         cmd = [
             "python", "-m", "dragon_baseline",
@@ -216,14 +425,15 @@
             "--max_seq_length", self.max_seq_length,
             "--truncation_side", self.task.recommended_truncation_side,
             "--load_best_model_at_end", self.load_best_model_at_end,
             "--save_strategy", "epoch",
             "--evaluation_strategy", "epoch",
             "--per_device_train_batch_size", self.per_device_train_batch_size,
             "--gradient_accumulation_steps", self.gradient_accumulation_steps,
+            "--gradient_checkpointing", self.gradient_checkpointing,
             "--train_file", self.nlp_dataset_train_preprocessed_path,
             "--validation_file", self.nlp_dataset_val_preprocessed_path,
             "--test_file", self.nlp_dataset_test_preprocessed_path,
             "--output_dir", self.model_save_dir,
             "--overwrite_output_dir",
             "--save_total_limit", "2",
             "--seed", self.task.jobid,
@@ -239,15 +449,15 @@
             cmd.extend([
                 "--label_column_names", ",".join(label_names),
             ])
         else:
             cmd.extend([
                 "--label_column_name", self.task.target.label_name,
             ])
-        if not self.task.target.problem_type in [ProblemType.SINGLE_LABEL_NER, ProblemType.MULTI_LABEL_BINARY_NER]:
+        if not self.task.target.problem_type in [ProblemType.SINGLE_LABEL_NER, ProblemType.MULTI_LABEL_NER]:
             cmd.extend([
                 "--text_column_delimiter", tokenizer.sep_token,
             ])
         if self.metric_for_best_model is not None:
             cmd.extend([
                 "--metric_for_best_model", str(self.metric_for_best_model),
             ])
@@ -308,70 +518,46 @@
                         found_match = True
                         break
 
                 if not found_match:
                     prediction.append("O")
                 start = end + 1
 
+            # add "O" tokens for the tokens that were removed
+            prediction = ["O"] * len(self.common_prefix) + prediction
+
             pred = {
                 self.task.target.prediction_name: prediction
             }
             results.append({"uid": row["uid"], **pred})
         return pd.DataFrame(results)
 
-    def predict_multi_label_binary_ner(self, *, df: pd.DataFrame) -> pd.DataFrame:
+    def predict_multi_label_ner(self, *, df: pd.DataFrame) -> pd.DataFrame:
         """Predict the labels for the test data."""
-        # load the model and tokenizer
-        tokenizer = AutoTokenizer.from_pretrained(self.model_save_dir, truncation_side=self.task.recommended_truncation_side)
-        model = AutoModelForMultiHeadTokenClassification.from_pretrained(self.model_save_dir).to(self.device)
+        # predict the labels for each entity group
+        predictions = self.predict_ner(df=df)
+        predictions["block_number"] = df["block_number"]
 
-        # predict
         results = []
-        for _, row in tqdm(df.iterrows(), desc="Predicting", total=len(df)):
-            # tokenize inputs
-            inputs = row[self.task.input_name]
-            tokenized_inputs = tokenizer(inputs, return_tensors="pt", truncation=True, is_split_into_words=True, padding=True).to(self.device)
-
-            # predict
-            result: SequenceClassifierOutput = model(**tokenized_inputs)
-            logits: np.ndarray = result.logits.detach().cpu().numpy()
-
-            # select the logits for the first token of each word and convert to probabilities
-            predictions = []
-            for batch_idx in range(len(logits)):
-                word_ids = tokenized_inputs.word_ids(batch_index=batch_idx)
-                previous_word_idx = None
-                batch_predictions = []
-                for token_idx, word_idx in enumerate(word_ids):
-                    if word_idx is None:
-                        # skip special tokens
-                        continue
-
-                    if word_idx == previous_word_idx:
-                        # skip subwords
-                        continue
-
-                    p = expit(logits[batch_idx, token_idx])
-                    batch_predictions.append(p)
-                    previous_word_idx = word_idx
-                predictions.append(batch_predictions)
-            predictions = np.array(predictions)
-
-            if predictions.shape[1] < len(inputs):
-                # pad the predictions to the length of the inputs
-                # note: feel free to implement a better solution! For example, using stride > 0 in the pipeline.
-                predictions = np.pad(predictions, ((0, 0), (0, len(inputs) - predictions.shape[1]), (0, 0)), mode="constant", constant_values=0)
+        for uid, group in predictions.groupby("uid"):
+            prediction = []
 
-            # convert to labels
-            expected_shape = (1, len(inputs), model.config.num_labels)
-            if predictions.shape != expected_shape:
-                raise ValueError(f"Expected predictions to have shape {expected_shape}, but got {predictions.shape}")
+            # combine the predictions for each entity group
+            for _, row in group.iterrows():
+                label_list = [re.sub("^(B|I)-", r"\1-" + row["block_number"] + "-", lbl) for lbl in row[self.task.target.prediction_name]]
+                prediction.append(label_list)
+
+            # remove the prediction for the block number
+            prediction = np.array(prediction).transpose()[1:].tolist()
+
+            # convert to list of labels per token
+            prediction = [(["O"] if set(token_labels) == {"O"} else sorted(set(token_labels) - {"O"})) for token_labels in prediction]
+            prediction = split_merged_labels(prediction)
 
-            prediction = {self.task.target.prediction_name: predictions[0]}
-            results.append({"uid": row["uid"], **prediction})
+            results.append({"uid": uid, self.task.target.prediction_name: prediction})
 
         return pd.DataFrame(results)
 
     def predict_huggingface(self, *, df: pd.DataFrame) -> pd.DataFrame:
         """Predict the labels for the test data."""
         # load the model and tokenizer
         tokenizer = AutoTokenizer.from_pretrained(self.model_save_dir, truncation_side=self.task.recommended_truncation_side)
@@ -462,33 +648,33 @@
         return df_pred
 
     def predict(self, *, df: pd.DataFrame) -> pd.DataFrame:
         """Predict the labels for the test data."""
         with torch.no_grad():
             if self.task.target.problem_type == ProblemType.SINGLE_LABEL_NER:
                 return self.predict_ner(df=df)
-            elif self.task.target.problem_type == ProblemType.MULTI_LABEL_BINARY_NER:
-                return self.predict_multi_label_binary_ner(df=df)
+            elif self.task.target.problem_type == ProblemType.MULTI_LABEL_NER:
+                return self.predict_multi_label_ner(df=df)
             else:
                 return self.predict_huggingface(df=df)
 
 
 if __name__ == "__main__":
     # Note: to debug (outside of Docker), you can set the input and output paths.
     # You probably need to change self.model_name too.
     for job_name in [
-        "Task000_Example_clf-fold0",
-        "Task001_Example_reg-fold0",
-        "Task002_Example_mutli_reg-fold0",
-        "Task003_Example_mednli-fold0",
-        "Task004_Example_ner-fold0",
-        "Task005_Example_multi_clf-fold0",
-        "Task006_Example_binary_clf-fold0",
-        "Task007_Example_multi_binary_clf-fold0",
-        "Task008_Example_multi_ner-fold0",
+        "Task101_Example_sl_bin_clf-fold0",
+        "Task102_Example_sl_mc_clf-fold0",
+        "Task103_Example_mednli-fold0",
+        "Task104_Example_ml_bin_clf-fold0",
+        "Task105_Example_ml_mc_clf-fold0",
+        "Task106_Example_sl_reg-fold0",
+        "Task107_Example_ml_reg-fold0",
+        "Task108_Example_sl_ner-fold0",
+        "Task109_Example_ml_ner-fold0",
     ]:
         DragonBaseline(
             input_path=Path(f"test-input/{job_name}"),
             output_path=Path(f"test-output/{job_name}"),
             workdir=Path(f"test-workdir/{job_name}"),
             models_dir=Path(f"test-workdir/models"),
         ).process()
```

### Comparing `dragon_baseline-0.1/src/dragon_baseline/nlp_algorithm.py` & `dragon_baseline-0.2.0/src/dragon_baseline/nlp_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,69 +31,122 @@
     SINGLE_LABEL_REGRESSION = "single_label_regression"
     MULTI_LABEL_REGRESSION = "multi_label_regression"
     SINGLE_LABEL_BINARY_CLASSIFICATION = "single_label_binary_classification"
     MULTI_LABEL_BINARY_CLASSIFICATION = "multi_label_binary_classification"
     SINGLE_LABEL_MULTI_CLASS_CLASSIFICATION = "single_label_multi_class_classification"
     MULTI_LABEL_MULTI_CLASS_CLASSIFICATION = "multi_label_multi_class_classification"
     SINGLE_LABEL_NER = "named_entity_recognition"
-    MULTI_LABEL_BINARY_NER = "multi_label_binary_named_entity_recognition"
+    MULTI_LABEL_NER = "multi_label_named_entity_recognition"
 
 
 def string_to_ProblemType(type_str):
-    """Convert a string to a corresponding Enum member if possible."""
+    """
+    Convert a string to a corresponding Enum member if possible.
+
+    Args:
+        type_str (str): The string representation of the ProblemType.
+
+    Returns:
+        ProblemType: The corresponding Enum member.
+
+    Raises:
+        ValueError: If the type_str does not correspond to a valid ProblemType.
+    """
     for problem_type in ProblemType:
         if problem_type.value == type_str:
             return problem_type
 
     raise ValueError(f"{type_str} does not correspond to a valid ProblemType")
 
 
 @dataclass
 class LabelDetails:
     """
     Details about a label.
-    The `None` values are set after calling `analyze()`.
+
+    Attributes:
+        problem_type (str): The type of problem associated with the label.
+        label_name (str): The name of the label.
+        prediction_name (str): The name of the prediction associated with the label.
+        values (List[Union[str, int, float]], optional): The list of values associated with the label. Set after calling `NLPAlgorithm.analyze()`.
+        mean (float, optional): The mean value of the label. Defaults to None. Set after calling `NLPAlgorithm.analyze()`.
+        std (float, optional): The standard deviation of the label. Defaults to None. Set after calling `NLPAlgorithm.analyze()`.
+        min (float, optional): The minimum value of the label. Defaults to None. Set after calling `NLPAlgorithm.analyze()`.
+        max (float, optional): The maximum value of the label. Defaults to None. Set after calling `NLPAlgorithm.analyze()`.
+        skew (float, optional): The skewness of the label. Defaults to None. Set after calling `NLPAlgorithm.analyze()`.
     """
+
     problem_type: str
     label_name: str
     prediction_name: str
     values: List[Union[str, int, float]] = None
     mean: float = None
     std: float = None
     min: float = None
     max: float = None
     skew: float = None
 
     @classmethod
     def from_label_name(cls, name: str):
-        """Create a `LabelDetails` object from a label name as {problem_type}_target."""
+        """Create a `LabelDetails` object from a label name as {problem_type}_target`.
+
+        Args:
+            name (str): The label name.
+
+        Returns:
+            LabelDetails: The created `LabelDetails` object.
+
+        Raises:
+            ValueError: If the label name does not end with '_target'.
+        """
         if not name.endswith("_target"):
             raise ValueError(f"Expected label name to end with '_target', but got '{name}'")
         prediction_name = name[:-len("_target")]
         problem_type = string_to_ProblemType(prediction_name)
 
         return cls(
             problem_type=problem_type,
             label_name=name,
             prediction_name=prediction_name,
         )
 
 
 @dataclass
 class TaskDetails:
-    """Details about the task."""
-    version: str  # version of the task details format
-    jobid: int  # unique identifier for this job
-    task_name: str  # name of the task
-    input_name: str  # name of algorithm input ("text" for a single input string, "text_parts" for a list of strings)
-    target: LabelDetails  # details about the target
-    recommended_truncation_side: str  # "left" or "right"
+    """Details about the task.
+
+    Attributes:
+        version (str): Version of the task details format.
+        jobid (int): Unique identifier for this job.
+        task_name (str): Name of the task.
+        input_name (str): Name of algorithm input ("text" for a single input string, "text_parts" for a list of strings).
+        target (LabelDetails): Details about the target.
+        recommended_truncation_side (str): "left" or "right".
+
+    Methods:
+        from_json(cls, path: Path) -> TaskDetails: Create a TaskDetails object from a JSON file.
+    """
+
+    version: str
+    jobid: int
+    task_name: str
+    input_name: str
+    target: LabelDetails
+    recommended_truncation_side: str
 
     @classmethod
-    def from_json(cls, path: Path):
+    def from_json(cls, path: Path) -> "TaskDetails":
+        """Create a TaskDetails object from a JSON file.
+
+        Args:
+            path (Path): Path to the JSON file.
+
+        Returns:
+            TaskDetails: The created TaskDetails object.
+        """
         with open(path) as f:
             task_details = json.load(f)
         return cls(
             version=task_details["version"],
             jobid=task_details["jobid"],
             task_name=task_details["task_name"],
             input_name=task_details["input_name"],
@@ -104,22 +157,17 @@
 
 class NLPAlgorithm(ClassificationAlgorithm):
     def __init__(self, **kwargs):
         """
         The base class for NLP algorithms. Sets the environment and controls
         the flow of the processing once `process` is called.
 
-        Parameters
-        ----------
-        input_path
-            The path in the container where the ground truth will be loaded
-            from. Default: `/input`
-        output_path
-            The path in the container where the output images will be written.
-            Default: `/output/images`
+        Args:
+            input_path (Path): Path to the data folder. Default: `/input`
+            output_path (Path): Path where the output predictions will be written. Default: `/output/images`
         """
 
         super().__init__(index_key="input_json", **kwargs)
 
         # defaults
         self.df_train: pd.DataFrame = None  # loaded in self.load()
         self.df_val: pd.DataFrame = None  # loaded in self.load()
@@ -176,16 +224,16 @@
                     raise ValueError(f"Expected values in column '{target.label_name}' to be 0 or 1")
             elif target.problem_type == ProblemType.SINGLE_LABEL_MULTI_CLASS_CLASSIFICATION:
                 df[target.label_name] = df[target.label_name].astype(str)
             elif target.problem_type == ProblemType.MULTI_LABEL_MULTI_CLASS_CLASSIFICATION:
                 df[target.label_name] = df[target.label_name].apply(lambda x: [str(value) for value in x])
             elif target.problem_type == ProblemType.SINGLE_LABEL_NER:
                 df[target.label_name] = df[target.label_name].apply(lambda x: [str(value) for value in x])
-            elif target.problem_type == ProblemType.MULTI_LABEL_BINARY_NER:
-                df[target.label_name] = df[target.label_name].apply(lambda x: [[bool(val) for val in value] for value in x])
+            elif target.problem_type == ProblemType.MULTI_LABEL_NER:
+                df[target.label_name] = df[target.label_name].apply(lambda x: [[str(val) for val in value] for value in x])
             else:
                 raise ValueError(f"Unexpected problem type '{target.problem_type}'")
 
         return df
 
     def load(self):
         """Load the input data."""
@@ -240,52 +288,53 @@
         """Verify the predictions.
         
         The predictions need to satisfy the following:
         - contain a "uid" column that matches the test data.
         - contain a column with the predictions (named after the problem_type).
         - the values in each label column must be valid.
         """
+        df_test = self.load_dataset(self.dataset_test_path)
         with open(self.test_predictions_path) as f:
             predictions = json.load(f)
         df = pd.DataFrame(predictions)
         if not "uid" in df.columns:
             raise ValueError("Expected column 'uid' in predictions")
         prediction_uids = set(df["uid"].tolist())
-        test_uids = set(self.df_test["uid"].tolist())
+        test_uids = set(df_test["uid"].tolist())
         if len(prediction_uids) != len(df):
             raise ValueError("Expected unique uids in predictions")
         if prediction_uids != test_uids:
             raise ValueError("Expected predictions to contain the same uids as the test data")
         if len(df.columns) != 2:
             raise ValueError(f"Expected 2 columns in predictions, but got {len(df.columns)}: {df.columns}")
 
         col = self.task.target.prediction_name
         if not col in df.columns:
             raise ValueError(f"Expected column '{col}' in predictions")
         if self.task.target.problem_type == ProblemType.SINGLE_LABEL_NER:
-            df_test = self.df_test.set_index("uid")
+            df_test = df_test.set_index("uid")
             for _, row in df.iterrows():
                 # check if all values are a list of strings
                 if not isinstance(row[col], list):
                     raise ValueError(f"Expected lists in column '{col}'")
                 if not all(isinstance(value, str) for value in row[col]):
                     raise ValueError(f"Expected lists of strings in column '{col}'")
                 # check if the number of values matches the number of words in the report
                 if len(row[col]) != len(df_test.loc[row.uid, self.task.input_name]):
                     raise ValueError(f"Expected {len(row[self.task.input_name])} values in column '{col}'")
-        elif self.task.target.problem_type == ProblemType.MULTI_LABEL_BINARY_NER:
-            df_test = self.df_test.set_index("uid")
+        elif self.task.target.problem_type == ProblemType.MULTI_LABEL_NER:
+            df_test = df_test.set_index("uid")
             for _, row in df.iterrows():
-                # check if all values are a list of lists of floats
+                # check if all values are a list of lists of strings
                 if not isinstance(row[col], list):
                     raise ValueError(f"Expected lists in column '{col}'")
                 if not all(isinstance(value, list) for value in row[col]):
                     raise ValueError(f"Expected list of lists in column '{col}'")
-                if not all(isinstance(value, float) for values in row[col] for value in values):
-                    raise ValueError(f"Expected list of lists of floats in column '{col}'")
+                if not all(isinstance(value, str) for values in row[col] for value in values):
+                    raise ValueError(f"Expected list of lists of strings in column '{col}'")
                 # check if the number of values matches the number of words in the report
                 if len(row[col]) != len(df_test.loc[row.uid, self.task.input_name]):
                     raise ValueError(f"Expected {len(row[self.task.input_name])} values in column '{col}'")
         elif self.task.target.problem_type == ProblemType.SINGLE_LABEL_BINARY_CLASSIFICATION:
             # check if all values are a float
             if not all(isinstance(value, float) for value in df[col]):
                 raise ValueError(f"Expected values in column '{col}' to be a float")
```

### Comparing `dragon_baseline-0.1/src/dragon_baseline/run_classification.py` & `dragon_baseline-0.2.0/src/dragon_baseline/run_classification.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline/run_classification_multi_label.py` & `dragon_baseline-0.2.0/src/dragon_baseline/run_classification_multi_label.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline/run_ner.py` & `dragon_baseline-0.2.0/src/dragon_baseline/run_ner.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.1/src/dragon_baseline.egg-info/PKG-INFO` & `dragon_baseline-0.2.0/src/dragon_baseline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dragon-baseline
-Version: 0.1
+Name: dragon_baseline
+Version: 0.2.0
 Summary: Baseline training algorithm for the DRAGON Challenge
 Home-page: https://github.com/DIAGNijmegen/dragon_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dragon_baseline/issues
 Platform: unix
 Platform: linux
```

### Comparing `dragon_baseline-0.1/src/dragon_baseline.egg-info/SOURCES.txt` & `dragon_baseline-0.2.0/src/dragon_baseline.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 src/dragon_baseline/__init__.py
 src/dragon_baseline/__main__.py
 src/dragon_baseline/main.py
 src/dragon_baseline/nlp_algorithm.py
 src/dragon_baseline/run_classification.py
 src/dragon_baseline/run_classification_multi_label.py
 src/dragon_baseline/run_ner.py
-src/dragon_baseline/run_ner_multi_label_binary.py
 src/dragon_baseline.egg-info/PKG-INFO
 src/dragon_baseline.egg-info/SOURCES.txt
 src/dragon_baseline.egg-info/dependency_links.txt
 src/dragon_baseline.egg-info/not-zip-safe
 src/dragon_baseline.egg-info/requires.txt
 src/dragon_baseline.egg-info/top_level.txt
 src/dragon_baseline/architectures/__init__.py
```

