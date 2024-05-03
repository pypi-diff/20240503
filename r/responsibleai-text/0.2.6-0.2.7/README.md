# Comparing `tmp/responsibleai_text-0.2.6.tar.gz` & `tmp/responsibleai_text-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_text-0.2.6.tar", last modified: Mon Feb 12 19:34:49 2024, max compression
+gzip compressed data, was "responsibleai_text-0.2.7.tar", last modified: Fri May  3 20:47:35 2024, max compression
```

## Comparing `responsibleai_text-0.2.6.tar` & `responsibleai_text-0.2.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.541539 responsibleai_text-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-12 19:34:49.541539 responsibleai_text-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.537539 responsibleai_text-0.2.6/responsibleai_text/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.537539 responsibleai_text-0.2.6/responsibleai_text/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.537539 responsibleai_text-0.2.6/responsibleai_text/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.537539 responsibleai_text-0.2.6/responsibleai_text/rai_text_insights/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/rai_text_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39341 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/rai_text_insights/rai_text_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.537539 responsibleai_text-0.2.6/responsibleai_text/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/feature_extractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.537539 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.541539 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/coherence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/equivalence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/fluency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/groundedness.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/relevance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/utils/question_answering.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/responsibleai_text/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.541539 responsibleai_text-0.2.6/responsibleai_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-12 19:34:49.000000 responsibleai_text-0.2.6/responsibleai_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-12 19:34:49.000000 responsibleai_text-0.2.6/responsibleai_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 19:34:49.000000 responsibleai_text-0.2.6/responsibleai_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-12 19:34:49.000000 responsibleai_text-0.2.6/responsibleai_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-12 19:34:49.000000 responsibleai_text-0.2.6/responsibleai_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 19:34:49.541539 responsibleai_text-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:34:49.541539 responsibleai_text-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/tests/test_feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/tests/test_genai_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/tests/test_rai_text_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-02-12 19:32:28.000000 responsibleai_text-0.2.6/tests/test_rai_text_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.742736 responsibleai_text-0.2.7/responsibleai_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.742736 responsibleai_text-0.2.7/responsibleai_text/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.742736 responsibleai_text-0.2.7/responsibleai_text/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.742736 responsibleai_text-0.2.7/responsibleai_text/rai_text_insights/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/rai_text_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39341 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/rai_text_insights/rai_text_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.742736 responsibleai_text-0.2.7/responsibleai_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/feature_extractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/coherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/fluency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/groundedness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/relevance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/utils/question_answering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/responsibleai_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/responsibleai_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-03 20:47:35.000000 responsibleai_text-0.2.7/responsibleai_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-03 20:47:35.000000 responsibleai_text-0.2.7/responsibleai_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:47:35.000000 responsibleai_text-0.2.7/responsibleai_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-03 20:47:35.000000 responsibleai_text-0.2.7/responsibleai_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 20:47:35.000000 responsibleai_text-0.2.7/responsibleai_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:47:35.746736 responsibleai_text-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/tests/test_feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/tests/test_genai_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/tests/test_rai_text_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-03 20:45:21.000000 responsibleai_text-0.2.7/tests/test_rai_text_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_text-0.2.6/PKG-INFO` & `responsibleai_text-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_text
-Version: 0.2.6
+Version: 0.2.7
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.17.2
 Requires-Dist: pandas>=0.25.1
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: semver~=2.13.0
 Requires-Dist: nlp-feature-extractors==0.1.0
-Requires-Dist: responsibleai>=0.34.1
+Requires-Dist: responsibleai>=0.35.0
 Provides-Extra: qa
 Requires-Dist: evaluate; extra == "qa"
 Requires-Dist: bert_score; extra == "qa"
 Requires-Dist: nltk; extra == "qa"
 Requires-Dist: rouge_score; extra == "qa"
 Provides-Extra: generative-text
 Requires-Dist: interpret_text; extra == "generative-text"
```

### Comparing `responsibleai_text-0.2.6/README.md` & `responsibleai_text-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/common/constants.py` & `responsibleai_text-0.2.7/responsibleai_text/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/managers/error_analysis_manager.py` & `responsibleai_text-0.2.7/responsibleai_text/managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/managers/explainer_manager.py` & `responsibleai_text-0.2.7/responsibleai_text/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/rai_text_insights/rai_text_insights.py` & `responsibleai_text-0.2.7/responsibleai_text/rai_text_insights/rai_text_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/feature_extractors.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/constants.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/metrics.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/_compute.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/_compute.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/coherence.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/coherence.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/equivalence.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/equivalence.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/fluency.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/fluency.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/groundedness.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/groundedness.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/genai_metrics/scripts/relevance.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/genai_metrics/scripts/relevance.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text/utils/question_answering.py` & `responsibleai_text-0.2.7/responsibleai_text/utils/question_answering.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/responsibleai_text.egg-info/PKG-INFO` & `responsibleai_text-0.2.7/responsibleai_text.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_text
-Version: 0.2.6
+Version: 0.2.7
 Summary: SDK API to assess text Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.17.2
 Requires-Dist: pandas>=0.25.1
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: semver~=2.13.0
 Requires-Dist: nlp-feature-extractors==0.1.0
-Requires-Dist: responsibleai>=0.34.1
+Requires-Dist: responsibleai>=0.35.0
 Provides-Extra: qa
 Requires-Dist: evaluate; extra == "qa"
 Requires-Dist: bert_score; extra == "qa"
 Requires-Dist: nltk; extra == "qa"
 Requires-Dist: rouge_score; extra == "qa"
 Provides-Extra: generative-text
 Requires-Dist: interpret_text; extra == "generative-text"
```

### Comparing `responsibleai_text-0.2.6/responsibleai_text.egg-info/SOURCES.txt` & `responsibleai_text-0.2.7/responsibleai_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/setup.py` & `responsibleai_text-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/tests/test_feature_extractors.py` & `responsibleai_text-0.2.7/tests/test_feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/tests/test_genai_metrics.py` & `responsibleai_text-0.2.7/tests/test_genai_metrics.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/tests/test_rai_text_insights.py` & `responsibleai_text-0.2.7/tests/test_rai_text_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_text-0.2.6/tests/test_rai_text_insights_save_and_load_scenarios.py` & `responsibleai_text-0.2.7/tests/test_rai_text_insights_save_and_load_scenarios.py`

 * *Files identical despite different names*

