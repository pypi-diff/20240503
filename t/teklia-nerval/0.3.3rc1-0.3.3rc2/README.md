# Comparing `tmp/teklia_nerval-0.3.3rc1.tar.gz` & `tmp/teklia_nerval-0.3.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teklia_nerval-0.3.3rc1.tar", last modified: Thu May  2 15:11:32 2024, max compression
+gzip compressed data, was "teklia_nerval-0.3.3rc2.tar", last modified: Fri May  3 07:54:11 2024, max compression
```

## Comparing `teklia_nerval-0.3.3rc1.tar` & `teklia_nerval-0.3.3rc2.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxrwxr-x   0 yschneider  (1000) yschneider  (1000)        0 2024-05-02 15:11:32.130667 teklia_nerval-0.3.3rc1/
--rw-r--r--   0 yschneider  (1000) yschneider  (1000)     8933 2024-05-02 15:11:32.130667 teklia_nerval-0.3.3rc1/PKG-INFO
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     8602 2024-02-19 08:29:04.000000 teklia_nerval-0.3.3rc1/README.md
-drwxrwxr-x   0 yschneider  (1000) yschneider  (1000)        0 2024-05-02 15:11:32.130667 teklia_nerval-0.3.3rc1/nerval/
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)      162 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/nerval/__init__.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     2309 2024-02-19 08:29:04.000000 teklia_nerval-0.3.3rc1/nerval/cli.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)    13524 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/nerval/evaluate.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     6781 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/nerval/parse.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     1646 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/nerval/utils.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     1204 2024-05-02 15:09:28.000000 teklia_nerval-0.3.3rc1/pyproject.toml
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)       52 2024-02-19 08:29:04.000000 teklia_nerval-0.3.3rc1/requirements.txt
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)       38 2024-05-02 15:11:32.130667 teklia_nerval-0.3.3rc1/setup.cfg
-drwxrwxr-x   0 yschneider  (1000) yschneider  (1000)        0 2024-05-02 15:11:32.130667 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/
--rw-r--r--   0 yschneider  (1000) yschneider  (1000)     8933 2024-05-02 15:11:32.000000 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/PKG-INFO
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)      539 2024-05-02 15:11:32.000000 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/SOURCES.txt
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)        1 2024-05-02 15:11:32.000000 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/dependency_links.txt
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)       43 2024-05-02 15:11:32.000000 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/entry_points.txt
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)       52 2024-05-02 15:11:32.000000 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/requires.txt
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)        7 2024-05-02 15:11:32.000000 teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/top_level.txt
-drwxrwxr-x   0 yschneider  (1000) yschneider  (1000)        0 2024-05-02 15:11:32.130667 teklia_nerval-0.3.3rc1/tests/
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)        0 2023-11-20 10:34:33.000000 teklia_nerval-0.3.3rc1/tests/__init__.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)      986 2024-05-02 15:06:50.000000 teklia_nerval-0.3.3rc1/tests/conftest.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)      654 2024-02-19 08:29:04.000000 teklia_nerval-0.3.3rc1/tests/test_align.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     6545 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/tests/test_compute_matches.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     1355 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/tests/test_compute_scores.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     4286 2024-02-19 08:29:04.000000 teklia_nerval-0.3.3rc1/tests/test_get_labels_aligned.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     4828 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/tests/test_parse_bio.py
--rw-rw-r--   0 yschneider  (1000) yschneider  (1000)     3582 2024-05-02 15:11:22.000000 teklia_nerval-0.3.3rc1/tests/test_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 07:54:11.373425 teklia_nerval-0.3.3rc2/
+-rw-r--r--   0 root         (0) root         (0)     8933 2024-05-03 07:54:11.373425 teklia_nerval-0.3.3rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8602 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 07:54:11.369425 teklia_nerval-0.3.3rc2/nerval/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/nerval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/nerval/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    13591 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/nerval/evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)     6835 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/nerval/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/nerval/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 07:54:11.373425 teklia_nerval-0.3.3rc2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 07:54:11.373425 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8933 2024-05-03 07:54:11.000000 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-03 07:54:11.000000 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 07:54:11.000000 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-03 07:54:11.000000 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-03 07:54:11.000000 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-03 07:54:11.000000 teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 07:54:11.373425 teklia_nerval-0.3.3rc2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/tests/test_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     6594 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/tests/test_compute_matches.py
+-rw-rw-rw-   0 root         (0) root         (0)     1397 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/tests/test_compute_scores.py
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/tests/test_get_labels_aligned.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/tests/test_parse_bio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2024-05-03 07:53:24.000000 teklia_nerval-0.3.3rc2/tests/test_run.py
```

### Comparing `teklia_nerval-0.3.3rc1/PKG-INFO` & `teklia_nerval-0.3.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-nerval
-Version: 0.3.3rc1
+Version: 0.3.3rc2
 Summary: Tool to evaluate NER on noisy text.
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 Description-Content-Type: text/markdown
 Requires-Dist: editdistance==0.6.2
 Requires-Dist: edlib==1.3.9
 Requires-Dist: prettytable==3.9.0
```

### Comparing `teklia_nerval-0.3.3rc1/README.md` & `teklia_nerval-0.3.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `teklia_nerval-0.3.3rc1/nerval/cli.py` & `teklia_nerval-0.3.3rc2/nerval/cli.py`

 * *Files identical despite different names*

### Comparing `teklia_nerval-0.3.3rc1/nerval/evaluate.py` & `teklia_nerval-0.3.3rc2/nerval/evaluate.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from pathlib import Path
 from typing import List
 
 import editdistance
 import edlib
 
+from nerval import ALL_ENTITIES
 from nerval.parse import (
     BEGINNING_POS,
     NOT_ENTITY_TAG,
     get_position_label,
     get_type_label,
     look_for_further_entity_part,
     parse_bio,
@@ -52,22 +53,22 @@
 
     Inputs :
     annotation : str, example : "Tolkie-n- was a writer- -."
     prediction : str, example : "Tolkieene xas --writear ,."
     labels_annot : list of strings,   example : ['B-P','I-P','I-P','I-P','I-P','I-P','I-P','I-P','I-P','O', ...]
     labels_predict : list of string , example : ['B-P','I-P','I-P','I-P','I-P','I-P','I-P','I-P','I-P','O', ...]
 
-    Output : {TAG1 : nb_entity_matched, ...}, example : {'All': 1, 'OCC': 0, 'PER': 1}
+    Output : {TAG1 : nb_entity_matched, ...}, example : {'ALL': 1, 'OCC': 0, 'PER': 1}
     """
     assert annotation, "Annotation is empty"
     assert prediction, "Prediction is empty"
     assert labels_annot, "Annotation labels are empty"
     assert labels_predict, "Prediction labels are empty"
 
-    entity_count = {"All": 0}
+    entity_count = {ALL_ENTITIES: 0}
     last_tag = NOT_ENTITY_TAG
 
     # Track indexes of characters found for continuation of nested entities
     visited_annot = []
     visited_predict = []
 
     # Iterating on reference string
@@ -168,15 +169,15 @@
                 score = (
                     1
                     if editdistance.eval(entity_ref, entity_compar) / len_entity
                     <= threshold
                     else 0
                 )
                 entity_count[last_tag] = entity_count.get(last_tag, 0) + score
-                entity_count["All"] += score
+                entity_count[ALL_ENTITIES] += score
                 current_ref = []
                 current_compar = []
 
     return entity_count
 
 
 def get_labels_aligned(original: str, aligned: str, labels_original: list) -> list:
@@ -378,17 +379,17 @@
         if not (annot and predict):
             raise Exception(
                 f"No file found for files {row[ANNO_COLUMN]}, {row[PRED_COLUMN]}"
             )
 
         count += 1
         scores = run(annot, predict, threshold, verbose)
-        precision += scores["All"]["P"]
-        recall += scores["All"]["R"]
-        f1 += scores["All"]["F1"]
+        precision += scores[ALL_ENTITIES]["P"]
+        recall += scores[ALL_ENTITIES]["R"]
+        f1 += scores[ALL_ENTITIES]["F1"]
 
     if not count:
         raise Exception("No file were counted")
 
     logger.info("Average score on all corpus")
     result = [
         round(precision / count, 3),
```

### Comparing `teklia_nerval-0.3.3rc1/nerval/parse.py` & `teklia_nerval-0.3.3rc2/nerval/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import List
 
+from nerval import ALL_ENTITIES
+
 NOT_ENTITY_TAG = "O"
 BEGINNING_POS = ["B", "S", "U"]
 
 REGEX_IOB_LINE = re.compile(r"^(\S*) ((?:[BIESLU]-|O).*)$")
 REGEX_LABEL = re.compile(r"[BIESLU]-(.*)$")
 
 
@@ -53,15 +55,15 @@
     """Parse a BIO file to get text content, character-level NE labels and entity types count.
 
     Input: lines of a valid BIO file
     Output format: { "words": str, "labels": list, "entity_count": { tag: int } }
     """
     words = []
     labels = []
-    entity_count = {"All": 0}
+    entity_count = {ALL_ENTITIES: 0}
     last_tag = None
 
     if "§" in " ".join(lines):
         raise (
             Exception(
                 "§ found in input file. Since this character is used in a specific way during evaluation, please remove it from files."
             )
@@ -136,15 +138,15 @@
             labels += [f"B-{tag}"] + [f"I-{tag}"] * (len(word) - 1)
         else:
             labels += [label] * len(word)
 
         # Count nb entity for each type
         if get_position_label(label) in BEGINNING_POS:
             entity_count[tag] = entity_count.get(tag, 0) + 1
-            entity_count["All"] += 1
+            entity_count[ALL_ENTITIES] += 1
 
         last_tag = tag
 
     result = None
 
     if words:
         result = {}
@@ -152,15 +154,15 @@
         result["labels"] = labels
         result["entity_count"] = entity_count
 
         assert len(result["words"]) == len(
             result["labels"]
         ), f'Found {len(result["words"])} word(s) for {len(result["labels"])} label(s)'
         for tag in result["entity_count"]:
-            if tag != "All":
+            if tag != ALL_ENTITIES:
                 assert (
                     result["labels"].count(f"B-{tag}") == result["entity_count"][tag]
                 ), f'Found {result["entity_count"][tag]} entities for {result["labels"].count(f"B-{tag}")} label(s) for entity {tag}'
 
     return result
```

### Comparing `teklia_nerval-0.3.3rc1/nerval/utils.py` & `teklia_nerval-0.3.3rc2/nerval/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,32 @@
 from prettytable import MARKDOWN, PrettyTable
 
+from nerval import ALL_ENTITIES
+
 
 def print_markdown_table(header: list[str], rows: list[list]) -> None:
     """Prints a Markdown table filled with the provided header and rows."""
     table = PrettyTable()
     table.field_names = header
     table.set_style(MARKDOWN)
+    # Align all columns at right
+    table.align = "r"
+    # First column should be left aligned still
+    table.align[header[0]] = "l"
+
+    def _special_sort(row: list[str]) -> str:
+        if row[0] == ALL_ENTITIES:
+            # Place the line for all entities at the very top
+            return ""
+        return row[0]
+
+    rows.sort(key=_special_sort)
+    # Place ALL_ENTITIES row at the end
+    rows.append(rows.pop(0))
+
     table.add_rows(rows)
     print(table)
 
 
 def print_results(scores: dict) -> None:
     """Display final results.
 
@@ -37,19 +54,19 @@
         ["tag", "predicted", "matched", "Precision", "Recall", "F1", "Support"],
         results,
     )
 
 
 def print_result_compact(scores: dict) -> None:
     result = [
-        "All",
-        scores["All"]["predicted"],
-        scores["All"]["matched"],
-        round(scores["All"]["P"], 3),
-        round(scores["All"]["R"], 3),
-        round(scores["All"]["F1"], 3),
-        scores["All"]["Support"],
+        ALL_ENTITIES,
+        scores[ALL_ENTITIES]["predicted"],
+        scores[ALL_ENTITIES]["matched"],
+        round(scores[ALL_ENTITIES]["P"], 3),
+        round(scores[ALL_ENTITIES]["R"], 3),
+        round(scores[ALL_ENTITIES]["F1"], 3),
+        scores[ALL_ENTITIES]["Support"],
     ]
     print_markdown_table(
         ["tag", "predicted", "matched", "Precision", "Recall", "F1", "Support"],
         [result],
     )
```

### Comparing `teklia_nerval-0.3.3rc1/pyproject.toml` & `teklia_nerval-0.3.3rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "teklia-nerval"
-version = "0.3.3-rc1"
+version = "0.3.3rc2"
 description = "Tool to evaluate NER on noisy text."
 dynamic = ["dependencies"]
 authors = [
     { name = "Teklia", email = "contact@teklia.com" },
 ]
 maintainers = [
     { name = "Teklia", email = "contact@teklia.com" },
```

### Comparing `teklia_nerval-0.3.3rc1/teklia_nerval.egg-info/PKG-INFO` & `teklia_nerval-0.3.3rc2/teklia_nerval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-nerval
-Version: 0.3.3rc1
+Version: 0.3.3rc2
 Summary: Tool to evaluate NER on noisy text.
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 Description-Content-Type: text/markdown
 Requires-Dist: editdistance==0.6.2
 Requires-Dist: edlib==1.3.9
 Requires-Dist: prettytable==3.9.0
```

### Comparing `teklia_nerval-0.3.3rc1/tests/test_align.py` & `teklia_nerval-0.3.3rc2/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `teklia_nerval-0.3.3rc1/tests/test_compute_matches.py` & `teklia_nerval-0.3.3rc2/tests/test_compute_matches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from nerval import evaluate
+from nerval import ALL_ENTITIES, evaluate
 
 THRESHOLD = 0.30
 
 
 fake_tags_aligned_nested_perfect = [
     # Labels 1
     "B-PER",
@@ -366,55 +366,55 @@
             (
                 "Gérard de -N-erval was bo-rn in Paris in 1808 -.",
                 "G*rard de *N*erval ----bo*rn in Paris in 1833 *.",
                 fake_annot_tags_aligned,
                 fake_predict_tags_aligned,
                 THRESHOLD,
             ),
-            {"All": 1, "PER": 1, "LOC": 0, "DAT": 0},
+            {ALL_ENTITIES: 1, "PER": 1, "LOC": 0, "DAT": 0},
         ),
         (
             (
                 "Louis par la grâce de Dieu roy de France et de Navarre.",
                 "Louis par la grâce de Dieu roy de France et de Navarre.",
                 fake_tags_aligned_nested_perfect,
                 fake_tags_aligned_nested_perfect,
                 THRESHOLD,
             ),
-            {"All": 3, "PER": 1, "LOC": 2},
+            {ALL_ENTITIES: 3, "PER": 1, "LOC": 2},
         ),
         (
             (
                 "Louis par la grâce de Dieu roy de France et de Navarre.",
                 "Louis par la grâce de Dieu roy de France et de Navarre.",
                 fake_tags_aligned_nested_perfect,
                 fake_tags_aligned_nested_false,
                 THRESHOLD,
             ),
-            {"All": 2, "PER": 1, "LOC": 1},
+            {ALL_ENTITIES: 2, "PER": 1, "LOC": 1},
         ),
         (
             (
                 "The red dragon",
                 "The red dragon",
                 fake_annot_tags_bk_boundary,
                 fake_predict_tags_bk_boundary,
                 THRESHOLD,
             ),
-            {"All": 0, "PER": 0},
+            {ALL_ENTITIES: 0, "PER": 0},
         ),
         (
             (
                 "A red dragon",
                 "A red dragon",
                 fake_annot_tags_bk_boundary_2,
                 fake_predict_tags_bk_boundary_2,
                 THRESHOLD,
             ),
-            {"All": 1, "PER": 1},
+            {ALL_ENTITIES: 1, "PER": 1},
         ),
     ],
 )
 def test_compute_matches(test_input, expected):
     assert evaluate.compute_matches(*test_input) == expected
```

### Comparing `teklia_nerval-0.3.3rc1/tests/test_compute_scores.py` & `teklia_nerval-0.3.3rc2/tests/test_compute_scores.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 
-from nerval import evaluate
+from nerval import ALL_ENTITIES, evaluate
 
 
 @pytest.mark.parametrize(
     ("annot", "predict", "matches"),
     [
         (
-            {"All": 3, "DAT": 1, "LOC": 1, "PER": 1},
-            {"All": 3, "DAT": 1, "***": 1, "PER": 1},
-            {"All": 1, "PER": 1, "LOC": 0, "DAT": 0},
+            {ALL_ENTITIES: 3, "DAT": 1, "LOC": 1, "PER": 1},
+            {ALL_ENTITIES: 3, "DAT": 1, "***": 1, "PER": 1},
+            {ALL_ENTITIES: 1, "PER": 1, "LOC": 0, "DAT": 0},
         ),
     ],
 )
 def test_compute_scores(annot, predict, matches):
     assert evaluate.compute_scores(annot, predict, matches) == {
         "***": {
             "P": 0.0,
@@ -27,15 +27,15 @@
             "P": 0.0,
             "R": 0.0,
             "F1": 0,
             "predicted": 1,
             "matched": 0,
             "Support": 1,
         },
-        "All": {
+        ALL_ENTITIES: {
             "P": 0.3333333333333333,
             "R": 0.3333333333333333,
             "F1": 0.3333333333333333,
             "predicted": 3,
             "matched": 1,
             "Support": 3,
         },
```

### Comparing `teklia_nerval-0.3.3rc1/tests/test_get_labels_aligned.py` & `teklia_nerval-0.3.3rc2/tests/test_get_labels_aligned.py`

 * *Files identical despite different names*

### Comparing `teklia_nerval-0.3.3rc1/tests/test_parse_bio.py` & `teklia_nerval-0.3.3rc2/tests/test_parse_bio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 
 import pytest
 
-from nerval import evaluate
+from nerval import ALL_ENTITIES, evaluate
 from nerval.parse import get_type_label, parse_line
 
 expected_parsed_annot = {
-    "entity_count": {"All": 3, "DAT": 1, "LOC": 1, "PER": 1},
+    "entity_count": {ALL_ENTITIES: 3, "DAT": 1, "LOC": 1, "PER": 1},
     "labels": [
         "B-PER",
         "I-PER",
         "I-PER",
         "I-PER",
         "I-PER",
         "I-PER",
@@ -53,15 +53,15 @@
         "O",
         "O",
     ],
     "words": "Gérard de Nerval was born in Paris in 1808 .",
 }
 
 expected_parsed_predict = {
-    "entity_count": {"All": 3, "DAT": 1, "***": 1, "PER": 1},
+    "entity_count": {ALL_ENTITIES: 3, "DAT": 1, "***": 1, "PER": 1},
     "labels": [
         "B-PER",
         "I-PER",
         "I-PER",
         "I-PER",
         "I-PER",
         "I-PER",
@@ -104,15 +104,15 @@
         "O",
         "O",
     ],
     "words": "G*rard de *N*erval bo*rn in Paris in 1833 *.",
 }
 
 expected_parsed_end_of_file = {
-    "entity_count": {"All": 3, "LOC": 2, "PER": 1},
+    "entity_count": {ALL_ENTITIES: 3, "LOC": 2, "PER": 1},
     "labels": [
         "B-PER",
         "I-PER",
         "I-PER",
         "I-PER",
         "I-PER",
         "I-PER",
```

### Comparing `teklia_nerval-0.3.3rc1/tests/test_run.py` & `teklia_nerval-0.3.3rc2/tests/test_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from pathlib import Path
 
 import pytest
 
-from nerval import evaluate
+from nerval import ALL_ENTITIES, evaluate
 
 
 @pytest.mark.parametrize(
     ("annotation", "prediction", "expected"),
     [
         (
             pytest.lazy_fixture("fake_annot_bio"),
@@ -25,15 +25,15 @@
                     "P": 0.0,
                     "R": 0.0,
                     "F1": 0,
                     "predicted": 1,
                     "matched": 0,
                     "Support": 1,
                 },
-                "All": {
+                ALL_ENTITIES: {
                     "P": 0.3333333333333333,
                     "R": 0.3333333333333333,
                     "F1": 0.3333333333333333,
                     "predicted": 3,
                     "matched": 1,
                     "Support": 3,
                 },
@@ -55,15 +55,15 @@
                 },
             },
         ),
         (
             pytest.lazy_fixture("nested_bio"),
             pytest.lazy_fixture("nested_bio"),
             {
-                "All": {
+                ALL_ENTITIES: {
                     "P": 1.0,
                     "R": 1.0,
                     "F1": 1.0,
                     "predicted": 3,
                     "matched": 3,
                     "Support": 3,
                 },
```

