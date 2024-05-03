# Comparing `tmp/dragon_eval-0.2.3.tar.gz` & `tmp/dragon_eval-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragon_eval-0.2.3.tar", last modified: Fri Nov  3 13:08:36 2023, max compression
+gzip compressed data, was "dragon_eval-0.2.4.tar", last modified: Fri May  3 10:41:09 2024, max compression
```

## Comparing `dragon_eval-0.2.3.tar` & `dragon_eval-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-03 13:08:36.953676 dragon_eval-0.2.3/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_eval-0.2.3/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)     2652 2023-11-03 13:08:36.953608 dragon_eval-0.2.3/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1495 2023-10-12 11:03:52.000000 dragon_eval-0.2.3/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      503 2023-10-11 12:48:20.000000 dragon_eval-0.2.3/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      800 2023-11-03 13:08:36.953941 dragon_eval-0.2.3/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)      728 2023-11-03 13:08:08.000000 dragon_eval-0.2.3/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-03 13:08:36.950758 dragon_eval-0.2.3/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-03 13:08:36.952139 dragon_eval-0.2.3/src/dragon_eval/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      724 2023-10-10 15:42:08.000000 dragon_eval-0.2.3/src/dragon_eval/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1411 2023-10-11 12:23:41.000000 dragon_eval-0.2.3/src/dragon_eval/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12684 2023-11-03 13:06:33.000000 dragon_eval-0.2.3/src/dragon_eval/evaluation.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-11-03 13:08:36.952991 dragon_eval-0.2.3/src/dragon_eval.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     2652 2023-11-03 13:08:36.000000 dragon_eval-0.2.3/src/dragon_eval.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      369 2023-11-03 13:08:36.000000 dragon_eval-0.2.3/src/dragon_eval.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-03 13:08:36.000000 dragon_eval-0.2.3/src/dragon_eval.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-10-12 10:37:46.000000 dragon_eval-0.2.3/src/dragon_eval.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      124 2023-11-03 13:08:36.000000 dragon_eval-0.2.3/src/dragon_eval.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       12 2023-11-03 13:08:36.000000 dragon_eval-0.2.3/src/dragon_eval.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 10:41:09.168428 dragon_eval-0.2.4/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_eval-0.2.4/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     2652 2024-05-03 10:41:09.168325 dragon_eval-0.2.4/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1495 2023-10-12 11:03:52.000000 dragon_eval-0.2.4/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      503 2023-10-11 12:48:20.000000 dragon_eval-0.2.4/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      800 2024-05-03 10:41:09.168810 dragon_eval-0.2.4/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      728 2024-05-03 10:39:56.000000 dragon_eval-0.2.4/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 10:41:09.164759 dragon_eval-0.2.4/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 10:41:09.166429 dragon_eval-0.2.4/src/dragon_eval/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      724 2023-10-10 15:42:08.000000 dragon_eval-0.2.4/src/dragon_eval/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1411 2023-10-11 12:23:41.000000 dragon_eval-0.2.4/src/dragon_eval/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    16021 2024-05-03 10:39:56.000000 dragon_eval-0.2.4/src/dragon_eval/evaluation.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 10:41:09.167630 dragon_eval-0.2.4/src/dragon_eval.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     2652 2024-05-03 10:41:09.000000 dragon_eval-0.2.4/src/dragon_eval.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      369 2024-05-03 10:41:09.000000 dragon_eval-0.2.4/src/dragon_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-03 10:41:09.000000 dragon_eval-0.2.4/src/dragon_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-10-12 10:37:46.000000 dragon_eval-0.2.4/src/dragon_eval.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      124 2024-05-03 10:41:09.000000 dragon_eval-0.2.4/src/dragon_eval.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       12 2024-05-03 10:41:09.000000 dragon_eval-0.2.4/src/dragon_eval.egg-info/top_level.txt
```

### Comparing `dragon_eval-0.2.3/LICENSE` & `dragon_eval-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dragon_eval-0.2.3/PKG-INFO` & `dragon_eval-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragon_eval
-Version: 0.2.3
+Version: 0.2.4
 Summary: Evaluation method for the DRAGON benchmark
 Home-page: https://github.com/DIAGNijmegen/dragon_eval
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dragon_eval/issues
 Platform: unix
 Platform: linux
```

### Comparing `dragon_eval-0.2.3/README.md` & `dragon_eval-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dragon_eval-0.2.3/setup.cfg` & `dragon_eval-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dragon_eval-0.2.3/setup.py` & `dragon_eval-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version='0.2.3',
+        version='0.2.4',
         author_email='Joeran.Bosma@radboudumc.nl',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/DIAGNijmegen/dragon_eval',
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/dragon_eval/issues"
         },
```

### Comparing `dragon_eval-0.2.3/src/dragon_eval/__init__.py` & `dragon_eval-0.2.4/src/dragon_eval/__init__.py`

 * *Files identical despite different names*

### Comparing `dragon_eval-0.2.3/src/dragon_eval/__main__.py` & `dragon_eval-0.2.4/src/dragon_eval/__main__.py`

 * *Files identical despite different names*

### Comparing `dragon_eval-0.2.3/src/dragon_eval/evaluation.py` & `dragon_eval-0.2.4/src/dragon_eval/evaluation.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,68 +8,81 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import re
 from enum import Enum
 from pathlib import Path
-from typing import Dict, Iterable, Optional
+from typing import Dict, Iterable, List, Optional
 
 import numpy as np
 import pandas as pd
 import seqeval.metrics
 from evalutils.evalutils import (DEFAULT_EVALUATION_OUTPUT_FILE_PATH,
                                  DEFAULT_GROUND_TRUTH_PATH, DEFAULT_INPUT_PATH,
                                  ClassificationEvaluation)
 from evalutils.io import FileLoader
 from evalutils.validators import ExpectedColumnNamesValidator
 from sklearn.metrics import cohen_kappa_score, roc_auc_score
 
 
 class EvalType(Enum):
     """Problem type of the task"""
-    NER = "named_entity_recognition"
-    REGRESSION = "regression"
-    BINARY_CLASSIFICATION = "binary classification"
-    ORDINAL_MULTI_CLASS_CLASSIFICATION = "ordinal multi-class classification"
-    NONORDINAL_MULTI_CLASS_CLASSIFICATION = "non-ordinal multi-class classification"
+    SINGLE_LABEL_NER = "single-label named entity recognition (macro F1)"
+    MULTI_LABEL_NER = "multi-label named entity recognition (weighted F1)"
+    REGRESSION = "regression (R-SMAPE)"
+    BINARY_CLASSIFICATION = "binary classification (AUC)"
+    BINARY_CLASSIFICATION_NON_SHARED_TASK = "binary classification different objective across labels (Unweighted Cohen's kappa)"
+    ORDINAL_MULTI_CLASS_CLASSIFICATION = "ordinal multi-class classification (Linear Cohen's kappa)"
+    NONORDINAL_MULTI_CLASS_CLASSIFICATION = "non-ordinal multi-class classification (Unweighted Cohen's kappa)"
 
 TASK_TYPE = {
-    "Task000_Example_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task001_Example_reg": EvalType.REGRESSION,
-    "Task002_Example_multi_reg": EvalType.REGRESSION,
-    "Task003_Example_mednli": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task004_Example_ner": EvalType.NER,
-    "Task005_Example_multi_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task006_Example_binary_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task007_Example_multi_binary_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task008_Example_multi_ner": EvalType.BINARY_CLASSIFICATION,
-    "Task100_adhesion_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task101_anonymisation_ner": EvalType.NER,
-    "Task102_colon_pathology_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task103_hip_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task104_kidney_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task105_medical_terminology_ner": EvalType.NER,
-    "Task106_nodules_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task107_nodules_diameter_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task108_nodules_diameter_reg": EvalType.REGRESSION,
-    "Task112_pathology_tumor_origin_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task113_pathology_tissue_modality_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task114_pathology_tissue_type_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task117_prostate_pathology_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task118_prostate_radiology_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
-    "Task119_prostate_radiology_prostate_volume_reg": EvalType.REGRESSION,
-    "Task120_prostate_radiology_psa_reg": EvalType.REGRESSION,
-    "Task121_prostate_radiology_psad_reg": EvalType.REGRESSION,
-    "Task122_recist_baseline_followup_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task123_recist_lesion_size_clf": EvalType.BINARY_CLASSIFICATION,
-    "Task124_recist_lesion_size_reg": EvalType.REGRESSION,
-    "Task125_textual_entailment_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
+    # example tasks
+    "Task101_Example_sl_bin_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task102_Example_sl_mc_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task103_Example_mednli": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task104_Example_ml_bin_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task105_Example_ml_mc_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task106_Example_sl_reg": EvalType.REGRESSION,
+    "Task107_Example_ml_reg": EvalType.REGRESSION,
+    "Task108_Example_sl_ner": EvalType.SINGLE_LABEL_NER,
+    "Task109_Example_ml_ner": EvalType.MULTI_LABEL_NER,
+
+    # tasks from the DRAGON benchmark
+    "Task001_adhesion_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task002_nodule_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task003_kidney_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task004_skin_case_selection_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task005_recist_timeline_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task006_pathology_tumor_origin_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task007_nodule_diameter_presence_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task008_pdac_size_presence_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task009_pdac_diagnosis_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task010_prostate_radiology_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task011_prostate_pathology_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task012_pathology_tissue_modality_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task013_pathology_tissue_type_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task014_textual_entailment_clf": EvalType.ORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task015_colon_pathology_clf": EvalType.BINARY_CLASSIFICATION_NON_SHARED_TASK,
+    "Task016_recist_lesion_size_presence_clf": EvalType.BINARY_CLASSIFICATION,
+    "Task017_pdac_attributes_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task018_osteoarthritis_clf": EvalType.NONORDINAL_MULTI_CLASS_CLASSIFICATION,
+    "Task019_prostate_volume_reg": EvalType.REGRESSION,
+    "Task020_psa_reg": EvalType.REGRESSION,
+    "Task021_psad_reg": EvalType.REGRESSION,
+    "Task022_pdac_size_reg": EvalType.REGRESSION,
+    "Task023_nodule_diameter_reg": EvalType.REGRESSION,
+    "Task024_recist_lesion_size_reg": EvalType.REGRESSION,
+    "Task025_anonymisation_ner": EvalType.SINGLE_LABEL_NER,
+    "Task026_medical_terminology_ner": EvalType.SINGLE_LABEL_NER,
+    "Task027_prostate_biopsy_ner": EvalType.MULTI_LABEL_NER,
+    "Task028_skin_pathology_ner": EvalType.MULTI_LABEL_NER,
 }
 
 
 class JSONLoader(FileLoader):
     """
     Custom file loader for JSON files.
     """
@@ -81,15 +94,15 @@
 
         with open(fname) as fp:
             return pd.read_json(fp, dtype={"uid": str})
 
 
 def score_rsmape(
     *, y_true, y_pred, epsilon: float, ignore_missing_targets: bool = False,
-):
+) -> float:
     """Robust symmetric mean absolute percentage score (R-SMAPE)
     The R-SMAPE is a robust version of the symmetric mean absolute percentage error (SMAPE) by adding epsilon to the denominator.
     SMAPE is a symmetric version of the mean absolute percentage error (MAPE) by adding the absolute value of the predicted values to the denominator.
     This results in a score that is more robust to outliers and makes sure that swapping the true and predicted values does not change the score.
     """
     y_true = np.asarray(y_true)
     y_pred = np.asarray(y_pred)
@@ -106,14 +119,51 @@
     # compute R-SMAPE
     numerator = np.abs(y_true - y_pred)
     denominator = np.abs(y_true) + np.abs(y_pred) + epsilon
     rsmape = numerator / denominator
     return 1 - np.mean(rsmape)
 
 
+def select_entity_labels(labels: List[List[str]], entity_lbl: str) -> List[str]:
+    labels = [[lbl for lbl in token_labels if entity_lbl in lbl] for token_labels in labels]
+    return [(token_labels[0] if len(token_labels) > 0 else "O") for token_labels in labels]
+
+
+def score_multi_label_f1(
+    *, y_true: pd.Series, y_pred: pd.Series, average: str = "weighted", out_label: str = "O",
+) -> float:
+    """Multi-label F1 score"""
+    label_values = sorted(set([re.sub(r"^[BI]-", "", lbl) for lbl in y_true.explode().explode().unique() if lbl != out_label]))
+
+    per_lbl_score, per_lbl_support = [], []
+    for entity_lbl in label_values:
+        # select labels for the current entity
+        y_true_lbl = y_true.apply(lambda labels: select_entity_labels(labels, entity_lbl=entity_lbl))
+        y_pred_lbl = y_pred.apply(lambda labels: select_entity_labels(labels, entity_lbl=entity_lbl))
+        support = len(seqeval.metrics.sequence_labeling.get_entities(y_true_lbl))
+
+        # calculate F1 score
+        score = seqeval.metrics.f1_score(
+            y_true=y_true_lbl,
+            y_pred=y_pred_lbl,
+            average=average,
+        )
+        per_lbl_score.append(score)
+        per_lbl_support.append(support)
+
+    # calculate average of F1 scores
+    if average == "macro":
+        score = np.mean(per_lbl_score)
+    elif average == "weighted":
+        score = np.average(per_lbl_score, weights=per_lbl_support)
+    else:
+        raise ValueError(f"Unsupported average: {average}")
+    return score
+
+
 class DragonEval(ClassificationEvaluation):
     def __init__(self, folds: Iterable[int] = range(5), tasks: Optional[Iterable[str]] = None, **kwargs):
         super().__init__(
             file_loader=JSONLoader(),
             validators=(
                 ExpectedColumnNamesValidator(
                     expected=("uid", ), extra_cols_check=False,
@@ -213,42 +263,67 @@
             # note: each subtask is the same, so we pool the labels and predictions
             # metric: AUC
             score = roc_auc_score(
                 y_true=y_true.explode().explode().values.astype(int),
                 y_score=y_pred.explode().explode().values.astype(float),
             )
 
+        elif TASK_TYPE[task_name] == EvalType.BINARY_CLASSIFICATION_NON_SHARED_TASK:
+            # evaluate binary classification tasks with different objectives across labels
+            # metric: mean AUC per objective
+            score = np.mean([
+                roc_auc_score(
+                    y_true=y_true.apply(lambda values: values[i]),
+                    y_score=y_pred.apply(lambda values: values[i]),
+                )
+                for i in range(len(y_true.iloc[0]))
+            ])
+
         elif TASK_TYPE[task_name] == EvalType.REGRESSION:
             # evaluate regression tasks
             # note: for the multi-label regression task, each subtask is the same,
             #       so we pool the labels and predictions
             # metric: R-SMAPE
             epsilon = {
-                "Task001_Example_reg": 4,
-                "Task002_Example_multi_reg": 4,
-                "Task115_prostate_radiology_prostate_volume_reg": 4,
-                "Task116_prostate_radiology_psa_reg": 0.4,
-                "Task117_prostate_radiology_psad_reg": 0.04,
-                "Task120_nodules_diameter_reg": 4,
-                "Task123_recist_lesion_size_reg": 4,
+                # example tasks
+                "Task106_Example_sl_reg": 4,
+                "Task107_Example_ml_reg": 4,
+
+                # DRAGON benchmark tasks
+                "Task019_prostate_volume_reg": 4,
+                "Task020_psa_reg": 0.4,
+                "Task021_psad_reg": 0.04,
+                "Task022_pdac_size_reg": 4,
+                "Task023_nodule_diameter_reg": 4,
+                "Task024_recist_lesion_size_reg": 4,
             }[task_name]
 
             score = score_rsmape(
                 y_true=y_true.explode().astype(float),
                 y_pred=y_pred.explode().astype(float),
                 epsilon=epsilon,
                 ignore_missing_targets=True,
             )
 
-        elif TASK_TYPE[task_name] == EvalType.NER:
-            # evaluate named entity recognition tasks
+        elif TASK_TYPE[task_name] == EvalType.SINGLE_LABEL_NER:
+            # evaluate single-label named entity recognition tasks
             # metric: F1 score
             score = seqeval.metrics.f1_score(
                 y_true=y_true,
                 y_pred=y_pred,
+                average="macro",
+            )
+
+        elif TASK_TYPE[task_name] == EvalType.MULTI_LABEL_NER:
+            # evaluate multi-label named entity recognition tasks
+            # metric: weighted F1 score
+            score = score_multi_label_f1(
+                y_true=y_true,
+                y_pred=y_pred,
+                average="weighted",
             )
 
         else:
             raise ValueError(f"Unexpexted task: {task_name}")
 
         # save score for the current job
         if task_name not in self._scores:
```

### Comparing `dragon_eval-0.2.3/src/dragon_eval.egg-info/PKG-INFO` & `dragon_eval-0.2.4/src/dragon_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dragon-eval
-Version: 0.2.3
+Name: dragon_eval
+Version: 0.2.4
 Summary: Evaluation method for the DRAGON benchmark
 Home-page: https://github.com/DIAGNijmegen/dragon_eval
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dragon_eval/issues
 Platform: unix
 Platform: linux
```

