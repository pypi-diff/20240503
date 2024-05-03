# Comparing `tmp/namedivider_python-0.2.3.tar.gz` & `tmp/namedivider_python-0.3.0.tar.gz`

## Comparing `namedivider_python-0.2.3.tar` & `namedivider_python-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,39 @@
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/__init__.py
--rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/cli.py
--rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divided_name.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/kanji_statistics.py
--rwxr-xr-x   0        0        0    15134 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/name_divider.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/util.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/version.py
--rwxr-xr-x   0        0        0    30784 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/assets/kanji.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divider/__init__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divider/basic_name_divider.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divider/config.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divider/divided_name.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divider/gbdt_name_divider.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/divider/name_divider_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/feature/__init__.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/feature/extractor.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/feature/family_name.py
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/feature/functional.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/feature/kanji.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/training/__init__.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/namedivider/training/kanji_statistics_taker.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/LICENSE
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/README.md
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 namedivider_python-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/__init__.py
+-rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/cli.py
+-rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divided_name.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/kanji_statistics.py
+-rwxr-xr-x   0        0        0    15134 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/name_divider.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/util.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/version.py
+-rwxr-xr-x   0        0        0    30784 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/assets/kanji.csv
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/beta_bert_divider/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/beta_bert_divider/__init__.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/beta_bert_divider/bert_name_divider_only_katakana.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/beta_bert_divider/combined_name_divider.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/beta_bert_divider/config.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/beta_bert_divider/vocab.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divider/__init__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divider/basic_name_divider.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divider/config.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divider/divided_name.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divider/gbdt_name_divider.py
+-rw-r--r--   0        0        0     7519 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/divider/name_divider_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/feature/__init__.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/feature/extractor.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/feature/family_name.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/feature/functional.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/feature/kanji.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/__init__.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/kanji_kana_rule.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/pipeline.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/rule.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/specific_family_name_rule.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/specific_given_name_rule.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/rule/two_char_rule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/training/__init__.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/namedivider/training/kanji_statistics_taker.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/README.md
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 namedivider_python-0.3.0/PKG-INFO
```

### Comparing `namedivider_python-0.2.3/namedivider/__init__.py` & `namedivider_python-0.3.0/namedivider/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from .divider.basic_name_divider import BasicNameDivider
-from .divider.config import BasicNameDividerConfig, NameDividerVersions
+from .divider.config import (
+    BasicNameDividerConfig,
+    GBDTNameDividerConfig,
+    NameDividerVersions,
+)
 from .divider.divided_name import DividedName
 from .divider.gbdt_name_divider import GBDTNameDivider
 from .feature.kanji import KanjiStatistics
 from .name_divider import NameDivider
+from .rule.specific_family_name_rule import SpecificFamilyNameRule
+from .rule.specific_given_name_rule import SpecificGivenNameRule
 from .version import __version__
 
 __all__ = [
     "NameDivider",
     "BasicNameDivider",
     "GBDTNameDivider",
     "DividedName",
     "KanjiStatistics",
     "NameDividerVersions",
     "BasicNameDividerConfig",
+    "GBDTNameDividerConfig",
+    "SpecificFamilyNameRule",
+    "SpecificGivenNameRule",
     "__version__",
 ]
```

### Comparing `namedivider_python-0.2.3/namedivider/cli.py` & `namedivider_python-0.3.0/namedivider/cli.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/divided_name.py` & `namedivider_python-0.3.0/namedivider/divided_name.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/kanji_statistics.py` & `namedivider_python-0.3.0/namedivider/kanji_statistics.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/name_divider.py` & `namedivider_python-0.3.0/namedivider/name_divider.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/util.py` & `namedivider_python-0.3.0/namedivider/util.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/assets/kanji.csv` & `namedivider_python-0.3.0/namedivider/assets/kanji.csv`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/divider/basic_name_divider.py` & `namedivider_python-0.3.0/namedivider/divider/basic_name_divider.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/divider/config.py` & `namedivider_python-0.3.0/namedivider/divider/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
-from typing import Union
+from typing import List, Optional, Union
 
+from namedivider.rule.rule import Rule
 from namedivider.util import (
     get_family_name_pkl_default_path,
     get_gbdt_model_v1_default_path,
     get_kanji_csv_default_path,
 )
 
 KANJI_CSV_DEFAULT_PATH = get_kanji_csv_default_path()
@@ -31,14 +32,15 @@
     into orthographic character form(正字体) before processing them.
     algorithm_name: Name of algorithm.
     """
 
     separator: str = " "
     normalize_name: bool = True
     algorithm_name: str = "unknown_algorithm"
+    custom_rules: Optional[List[Rule]] = None
 
 
 @dataclass(frozen=True)
 class BasicNameDividerConfig(NameDividerConfigBase):
     """
     path_csv: Path of the file containing the kanji information.
     only_order_score_when_4: If True, only order score is used for 4-character names. Not recommended to be True.
```

### Comparing `namedivider_python-0.2.3/namedivider/divider/divided_name.py` & `namedivider_python-0.3.0/namedivider/divider/divided_name.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/divider/gbdt_name_divider.py` & `namedivider_python-0.3.0/namedivider/divider/gbdt_name_divider.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/divider/name_divider_base.py` & `namedivider_python-0.3.0/namedivider/divider/name_divider_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import abc
+import warnings
 from typing import List, Optional
 
 import numpy as np
 import regex
 
 from namedivider.divider.config import (
     NameDividerConfigBase,
     NameDividerVersions,
     get_config_from_version,
 )
 from namedivider.divider.divided_name import DividedName
+from namedivider.rule.pipeline import Pipeline
 
 
 class _UndividedNameHolder:
     def __init__(self, original_name: str):
         """
         Class to hold original and normalized name for dividing.
         :param original_name: Original name
@@ -64,15 +66,16 @@
         :param config: Configuration of NameDivider.
         """
         if config is None:
             config = NameDividerConfigBase()
         self.separator = config.separator
         self.normalize_name = config.normalize_name
         self.algorithm_name = config.algorithm_name
-        self.compiled_regex_kanji = regex.compile(r"\p{Script=Han}+")
+        self._rule_pipeline = Pipeline(separator=self.separator, custom_rules=config.custom_rules)
+        self._compiled_regex_kanji = regex.compile(r"\p{Script=Han}+")
 
     @abc.abstractmethod
     def calc_score(self, family: str, given: str) -> float:
         """
         Calculates the score. The higher the score, the more likely the division is correct.
         :param family: Family name.
         :param given: Given name.
@@ -120,47 +123,41 @@
         :return: Softmax scores
         :rtype: np.ndarray
         """
         u = np.sum(np.exp(x))
         softmax_val: List[float] = np.exp(x) / u
         return softmax_val
 
+    @property
+    def compiled_regex_kanji(self):  # type: ignore
+        """
+        This property was added for only backward compatibility.
+        """
+        warnings.warn(
+            "_NameDivider.compiled_regex_kanji is deprecated in 0.3 and will be removed in 0.4. "
+            "Use regex.compile if you want to use compiled_regex_kanji.",
+            category=FutureWarning,
+            stacklevel=1,
+        )
+        return self._compiled_regex_kanji
+
     def _divide_by_rule_base(self, undivided_name: str) -> Optional[DividedName]:
         """
         Divides undivided name without using kanji statistics.
         :param undivided_name: Names with no space between the family name and given name
         :return:
             if fits the rules: Divided name
             else: None
         :rtype:
             if fits the rules: DividedName
             else: None
         """
-        # If the undivided name consists of 2 characters,
-        # the first characters is family name, and the last characters is given name.
-        if len(undivided_name) == 2:
-            return self._create_divided_name(family=undivided_name[0], given=undivided_name[-1], algorithm="rule")
-
-        # If the undivided name consists of kanji and other types of characters (hiragana, katakana, etc...),
-        # the undivided name will be divided where the kanji and other character types are switched.
-        # The criterion for determining switched is whether "two" consecutive characters are having
-        # different type of characters from first character type.
-        # The reason of "two" is some family names consist of some kanji and one katakana.
-        # (ex: "井ノ原", "三ツ又",　"関ヶ原" contains "ノ", "ツ", "ヶ". They are all katakana.)
-        is_kanji_list = []
-        for i, _char in enumerate(undivided_name):
-            is_kanji = True if self.compiled_regex_kanji.fullmatch(_char) else False
-            is_kanji_list.append(is_kanji)
-            if i >= 2:
-                if is_kanji_list[0] != is_kanji and is_kanji_list[-2] == is_kanji:
-                    return self._create_divided_name(
-                        family=undivided_name[: i - 1], given=undivided_name[i - 1 :], algorithm="rule"
-                    )
+        divided_name_or_none = self._rule_pipeline.apply(undivided_name)
 
-        return None
+        return divided_name_or_none
 
     def _divide_by_algorithm(self, undivided_name: str) -> DividedName:
         """
         Divides undivided name using kanji statistics.
         :param undivided_name: Names with no space between the family name and given name
         :return: Divided name
         :rtype: DividedName
```

### Comparing `namedivider_python-0.2.3/namedivider/feature/extractor.py` & `namedivider_python-0.3.0/namedivider/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/feature/family_name.py` & `namedivider_python-0.3.0/namedivider/feature/family_name.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/feature/functional.py` & `namedivider_python-0.3.0/namedivider/feature/functional.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/feature/kanji.py` & `namedivider_python-0.3.0/namedivider/feature/kanji.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/namedivider/training/kanji_statistics_taker.py` & `namedivider_python-0.3.0/namedivider/training/kanji_statistics_taker.py`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/LICENSE` & `namedivider_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `namedivider_python-0.2.3/README.md` & `namedivider_python-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 # {'algorithm': 'kanji_feature',
 # 'family': '菅',
 # 'given': '義偉',
 # 'score': 0.7300634880343344,
 # 'separator': ' '}
 ```
 
+For more advanced features, see [here](docs/advanced_features.md).
+
 ## NameDivider API
 
 NameDivider API is a Docker container that provides a RESTful API for dividing the Japanese full name into a family name and a given name.
 
 I am developing NameDivider API to provide NameDivider functionality to non-Python language users.
 
 ### Installation
@@ -115,14 +117,17 @@
 ```
 
 ## License
 
 ### Source code and gbdt_model_v1.txt
 MIT License
 
+### bert_katakana_v0_3_0.pt
+cc-by-sa-4.0
+
 ### family_name_repository.pickle
 
 - English
 
 (1) Purpose of use
 
 family_name_repository.pickle is available for commercial/non-commercial use if you use this software to divide name, and to develop algorithms for dividing name.
```

### Comparing `namedivider_python-0.2.3/pyproject.toml` & `namedivider_python-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "/namedivider",
 ]
 
 [tool.hatch.build.targets.wheel.force-include]
 "namedivider/assets/kanji.csv" = "namedivider/assets/kanji.csv"
+"namedivider/beta_bert_divider/config.json" = "namedivider/beta_bert_divider/config.json"
+"namedivider/beta_bert_divider/vocab.json" = "namedivider/beta_bert_divider/vocab.json"
 
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 module = "namedivider"
 ignore_missing_imports = true
```

### Comparing `namedivider_python-0.2.3/PKG-INFO` & `namedivider_python-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namedivider-python
-Version: 0.2.3
+Version: 0.3.0
 Summary: A tool for dividing the Japanese full name into a family name and a given name.
 Project-URL: Homepage, https://github.com/rskmoi/namedivider-python
 Author-email: rskmoi <rei.sakamoto.92@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -73,14 +73,16 @@
 # {'algorithm': 'kanji_feature',
 # 'family': '菅',
 # 'given': '義偉',
 # 'score': 0.7300634880343344,
 # 'separator': ' '}
 ```
 
+For more advanced features, see [here](docs/advanced_features.md).
+
 ## NameDivider API
 
 NameDivider API is a Docker container that provides a RESTful API for dividing the Japanese full name into a family name and a given name.
 
 I am developing NameDivider API to provide NameDivider functionality to non-Python language users.
 
 ### Installation
@@ -138,14 +140,17 @@
 ```
 
 ## License
 
 ### Source code and gbdt_model_v1.txt
 MIT License
 
+### bert_katakana_v0_3_0.pt
+cc-by-sa-4.0
+
 ### family_name_repository.pickle
 
 - English
 
 (1) Purpose of use
 
 family_name_repository.pickle is available for commercial/non-commercial use if you use this software to divide name, and to develop algorithms for dividing name.
```

