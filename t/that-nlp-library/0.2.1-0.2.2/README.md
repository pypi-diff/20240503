# Comparing `tmp/that-nlp-library-0.2.1.tar.gz` & `tmp/that-nlp-library-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that-nlp-library-0.2.1.tar", last modified: Tue Jan  2 09:03:49 2024, max compression
+gzip compressed data, was "that-nlp-library-0.2.2.tar", last modified: Fri May  3 17:43:04 2024, max compression
```

## Comparing `that-nlp-library-0.2.1.tar` & `that-nlp-library-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/
--rw-rw-r--   0 quan      (1000) quan      (1000)    11337 2023-04-27 10:12:58.000000 that-nlp-library-0.2.1/LICENSE
--rw-rw-r--   0 quan      (1000) quan      (1000)      111 2023-04-27 10:12:58.000000 that-nlp-library-0.2.1/MANIFEST.in
--rw-r--r--   0 quan      (1000) quan      (1000)     9841 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/PKG-INFO
--rw-rw-r--   0 quan      (1000) quan      (1000)     8681 2023-10-10 10:36:29.000000 that-nlp-library-0.2.1/README.md
--rw-rw-r--   0 quan      (1000) quan      (1000)     1244 2024-01-02 08:53:28.000000 that-nlp-library-0.2.1/settings.ini
--rw-rw-r--   0 quan      (1000) quan      (1000)       38 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/setup.cfg
--rw-rw-r--   0 quan      (1000) quan      (1000)     2596 2023-04-27 10:12:58.000000 that-nlp-library-0.2.1/setup.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/that_nlp_library/
--rw-rw-r--   0 quan      (1000) quan      (1000)       22 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/__init__.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    65292 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/_modidx.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     4704 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/evaluations.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    20074 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/model_lm_main.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    29849 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/model_main.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/that_nlp_library/models/
--rw-rw-r--   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/__init__.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/that_nlp_library/models/gpt2/
--rw-rw-r--   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/gpt2/__init__.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    11662 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/gpt2/classifiers.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/that_nlp_library/models/roberta/
--rw-rw-r--   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/roberta/__init__.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    12373 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/roberta/classifiers.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     5585 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/roberta/conditional_prob_classifiers.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    13910 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/models/roberta/deep_hierarchical_classifiers.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     1572 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/text_augmentation.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    35070 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/text_main.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    13583 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/text_main_lm.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    14703 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/text_main_lm_streaming.py
--rw-rw-r--   0 quan      (1000) quan      (1000)    24868 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/text_main_streaming.py
--rw-rw-r--   0 quan      (1000) quan      (1000)      871 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/text_transformation.py
--rw-rw-r--   0 quan      (1000) quan      (1000)     8415 2024-01-02 09:03:25.000000 that-nlp-library-0.2.1/that_nlp_library/utils.py
-drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-01-02 09:03:49.179996 that-nlp-library-0.2.1/that_nlp_library.egg-info/
--rw-r--r--   0 quan      (1000) quan      (1000)     9841 2024-01-02 09:03:49.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/PKG-INFO
--rw-rw-r--   0 quan      (1000) quan      (1000)     1077 2024-01-02 09:03:49.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/SOURCES.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)        1 2024-01-02 09:03:49.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/dependency_links.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)       54 2024-01-02 09:03:49.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/entry_points.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)        1 2023-05-10 04:37:10.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/not-zip-safe
--rw-rw-r--   0 quan      (1000) quan      (1000)      149 2024-01-02 09:03:49.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/requires.txt
--rw-rw-r--   0 quan      (1000) quan      (1000)       17 2024-01-02 09:03:49.000000 that-nlp-library-0.2.1/that_nlp_library.egg-info/top_level.txt
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/
+-rw-rw-r--   0 quan      (1000) quan      (1000)    11337 2023-04-27 10:12:58.000000 that-nlp-library-0.2.2/LICENSE
+-rw-rw-r--   0 quan      (1000) quan      (1000)      111 2023-04-27 10:12:58.000000 that-nlp-library-0.2.2/MANIFEST.in
+-rw-r--r--   0 quan      (1000) quan      (1000)    10000 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/PKG-INFO
+-rw-rw-r--   0 quan      (1000) quan      (1000)     8840 2024-05-03 17:41:42.000000 that-nlp-library-0.2.2/README.md
+-rw-rw-r--   0 quan      (1000) quan      (1000)     1244 2024-05-03 16:27:45.000000 that-nlp-library-0.2.2/settings.ini
+-rw-rw-r--   0 quan      (1000) quan      (1000)       38 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/setup.cfg
+-rw-rw-r--   0 quan      (1000) quan      (1000)     2596 2023-04-27 10:12:58.000000 that-nlp-library-0.2.2/setup.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/that_nlp_library/
+-rw-rw-r--   0 quan      (1000) quan      (1000)       22 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/__init__.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    65382 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/_modidx.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     4704 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/evaluations.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    20679 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/model_lm_main.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    30977 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/model_main.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/that_nlp_library/models/
+-rw-rw-r--   0 quan      (1000) quan      (1000)        0 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/__init__.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/that_nlp_library/models/gpt2/
+-rw-rw-r--   0 quan      (1000) quan      (1000)        0 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/gpt2/__init__.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    11714 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/gpt2/classifiers.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/that_nlp_library/models/roberta/
+-rw-rw-r--   0 quan      (1000) quan      (1000)        0 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/roberta/__init__.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    12366 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/roberta/classifiers.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     5585 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/roberta/conditional_prob_classifiers.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    13910 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/models/roberta/deep_hierarchical_classifiers.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     1572 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/text_augmentation.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    35056 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/text_main.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    13650 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/text_main_lm.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    14885 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/text_main_lm_streaming.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)    25527 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/text_main_streaming.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)      871 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/text_transformation.py
+-rw-rw-r--   0 quan      (1000) quan      (1000)     8415 2024-05-03 17:41:35.000000 that-nlp-library-0.2.2/that_nlp_library/utils.py
+drwxrwxr-x   0 quan      (1000) quan      (1000)        0 2024-05-03 17:43:04.008386 that-nlp-library-0.2.2/that_nlp_library.egg-info/
+-rw-r--r--   0 quan      (1000) quan      (1000)    10000 2024-05-03 17:43:03.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/PKG-INFO
+-rw-rw-r--   0 quan      (1000) quan      (1000)     1077 2024-05-03 17:43:03.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)        1 2024-05-03 17:43:03.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)       54 2024-05-03 17:43:03.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/entry_points.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)        1 2023-05-10 04:37:10.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/not-zip-safe
+-rw-rw-r--   0 quan      (1000) quan      (1000)      149 2024-05-03 17:43:03.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/requires.txt
+-rw-rw-r--   0 quan      (1000) quan      (1000)       17 2024-05-03 17:43:03.000000 that-nlp-library-0.2.2/that_nlp_library.egg-info/top_level.txt
```

### Comparing `that-nlp-library-0.2.1/LICENSE` & `that-nlp-library-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/PKG-INFO` & `that-nlp-library-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-nlp-library
-Version: 0.2.1
+Version: 0.2.2
 Summary: Aim to be a convenient NLP library with the help from HuggingFace
 Home-page: https://github.com/anhquan0412/that-nlp-library
 Author: Quan Tran
 Author-email: anhquan0412@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev,python,nlp,natural language processing,transformer,deep learning,envibert,roberta,gpt2,phobert
 Classifier: Development Status :: 4 - Beta
@@ -136,16 +136,18 @@
 This library also a **streamed version of Text Controller**
 ([`TextDataControllerStreaming`](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html#textdatacontrollerstreaming)),
 allowing you to work with data without having it entirely on your hard
 drive. You can still perform all the processings in the non-streamed
 version, except for **Train/Validation split** (which means you have to
 define your validation set beforehand), and **Upsampling**.
 
-For more details on **streaming**, visit
-[here](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html).
+For more details on **streaming**, visit [how to create a streamed
+dataset](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html)
+and [how to train a model with a streamed
+dataset](https://anhquan0412.github.io/that-nlp-library/roberta_singlehead_for_streaming)
 
 If you are curious on the time and space efficiency between streamed and
 non-streamed version, visit the benchmark
 [here](https://anhquan0412.github.io/that-nlp-library/text_main_benchmark.html)
 
 ### **Model and [`ModelController`](https://anhquan0412.github.io/that-nlp-library/model_main.html#modelcontroller)**
 
@@ -192,15 +194,15 @@
 for training your data. There’s a quick tutorial on this decoupling
 [here](https://anhquan0412.github.io/that-nlp-library/model_classification_tutorial.html#train-model-with-only-a-tokenized-datasetdict-no-textdatacontroller)
 
 ## Language Modeling
 
 For language modeling, the main pipeline also contains 2 parts
 
-### Text Data Controlelr for Language Model: [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
+### Text Data Controller for Language Model: [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
 
 Similarly to `TextDatController`,
 [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
 also provide a list of processings (except for **Label Processing**,
 **Upsampling** and **Text Augmentation**). The controller also allow
 tokenization line-by-line or by token concatenation. Visit the tutorial
 [here](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html)
```

### Comparing `that-nlp-library-0.2.1/README.md` & `that-nlp-library-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -101,16 +101,18 @@
 This library also a **streamed version of Text Controller**
 ([`TextDataControllerStreaming`](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html#textdatacontrollerstreaming)),
 allowing you to work with data without having it entirely on your hard
 drive. You can still perform all the processings in the non-streamed
 version, except for **Train/Validation split** (which means you have to
 define your validation set beforehand), and **Upsampling**.
 
-For more details on **streaming**, visit
-[here](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html).
+For more details on **streaming**, visit [how to create a streamed
+dataset](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html)
+and [how to train a model with a streamed
+dataset](https://anhquan0412.github.io/that-nlp-library/roberta_singlehead_for_streaming)
 
 If you are curious on the time and space efficiency between streamed and
 non-streamed version, visit the benchmark
 [here](https://anhquan0412.github.io/that-nlp-library/text_main_benchmark.html)
 
 ### **Model and [`ModelController`](https://anhquan0412.github.io/that-nlp-library/model_main.html#modelcontroller)**
 
@@ -157,15 +159,15 @@
 for training your data. There’s a quick tutorial on this decoupling
 [here](https://anhquan0412.github.io/that-nlp-library/model_classification_tutorial.html#train-model-with-only-a-tokenized-datasetdict-no-textdatacontroller)
 
 ## Language Modeling
 
 For language modeling, the main pipeline also contains 2 parts
 
-### Text Data Controlelr for Language Model: [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
+### Text Data Controller for Language Model: [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
 
 Similarly to `TextDatController`,
 [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
 also provide a list of processings (except for **Label Processing**,
 **Upsampling** and **Text Augmentation**). The controller also allow
 tokenization line-by-line or by token concatenation. Visit the tutorial
 [here](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html)
```

### Comparing `that-nlp-library-0.2.1/settings.ini` & `that-nlp-library-0.2.2/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = that-nlp-library
 lib_name = %(repo)s
-version = 0.2.1
+version = 0.2.2
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = that_nlp_library
```

### Comparing `that-nlp-library-0.2.1/setup.py` & `that-nlp-library-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library/_modidx.py` & `that-nlp-library-0.2.2/that_nlp_library/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,14 @@
                                                                                                                             'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.TextDataController.prepare_test_dataset_from_raws': ( 'text_main.html#textdatacontroller.prepare_test_dataset_from_raws',
                                                                                                                               'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.TextDataController.process_and_tokenize': ( 'text_main.html#textdatacontroller.process_and_tokenize',
                                                                                                                     'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.TextDataController.save_as_pickles': ( 'text_main.html#textdatacontroller.save_as_pickles',
                                                                                                                'that_nlp_library/text_main.py'),
-                                            'that_nlp_library.text_main.TextDataController.set_data_collator': ( 'text_main.html#textdatacontroller.set_data_collator',
-                                                                                                                 'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.TextDataController.set_verbose': ( 'text_main.html#textdatacontroller.set_verbose',
                                                                                                            'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.TextDataController.validate_input': ( 'text_main.html#textdatacontroller.validate_input',
                                                                                                               'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.concat_metadatas': ( 'text_main.html#concat_metadatas',
                                                                                              'that_nlp_library/text_main.py'),
                                             'that_nlp_library.text_main.tokenize_function': ( 'text_main.html#tokenize_function',
@@ -289,14 +287,16 @@
                                                                                                                                                        'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._determine_multihead_multilabel': ( 'text_main_streaming.html#textdatacontrollerstreaming._determine_multihead_multilabel',
                                                                                                                                                             'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_filtering': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_filtering',
                                                                                                                                           'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_label_transformation': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_label_transformation',
                                                                                                                                                      'that_nlp_library/text_main_streaming.py'),
+                                                      'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_transformation': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_transformation',
+                                                                                                                                               'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_transformation_augmentation_tokenization': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_transformation_augmentation_tokenization',
                                                                                                                                                                          'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_transformation_augmentation_tokenization_generator': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_transformation_augmentation_tokenization_generator',
                                                                                                                                                                                    'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_transformation_augmentation_tokenization_generator_linebyline': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_transformation_augmentation_tokenization_generator_linebyline',
                                                                                                                                                                                               'that_nlp_library/text_main_streaming.py'),
                                                       'that_nlp_library.text_main_streaming.TextDataControllerStreaming._do_transformation_tokenization': ( 'text_main_streaming.html#textdatacontrollerstreaming._do_transformation_tokenization',
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/evaluations.py` & `that-nlp-library-0.2.2/that_nlp_library/evaluations.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library/model_lm_main.py` & `that-nlp-library-0.2.2/that_nlp_library/model_lm_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,41 +97,44 @@
                 lr_scheduler_type='cosine',  # The scheduler type to use. Including: linear, cosine, cosine_with_restarts, polynomial, constant, constant_with_warmup
                 warmup_ratio=0.1, # The warmup ratio for some lr scheduler
                 no_valid=False, # Whether there is a validation set or not
                 val_bs=None, # Validation batch size
                 seed=None, # Random seed
                 report_to='none', # The list of integrations to report the results and logs to. Supported platforms are "azure_ml", "comet_ml", "mlflow", "neptune", "tensorboard","clearml" and "wandb". Use "all" to report to all integrations installed, "none" for no integrations.
                 trainer_class=None, # You can include the class name of your custom trainer here
+                len_train=None, # estimated number of samples in the whole training set (for streaming dataset only)
             ):
     "The main model training/finetuning function"
     torch.cuda.empty_cache()
     gc.collect()
     if val_bs is None: val_bs = bs
 
     if seed:
         seed_everything(seed)
         
     training_args = TrainingArguments(o_dir, 
-                                     learning_rate=lr, 
-                                     warmup_ratio=warmup_ratio,
-                                     lr_scheduler_type=lr_scheduler_type, 
-                                     fp16=True,
-                                     do_train=True,
-                                     do_eval= not no_valid,
-                                     evaluation_strategy="no" if no_valid else "epoch", 
-                                     save_strategy="epoch" if save_checkpoint else 'no',
-                                     overwrite_output_dir=True,
-                                     gradient_accumulation_steps=grad_accum_steps,
-                                     per_device_train_batch_size=bs, 
-                                     per_device_eval_batch_size=val_bs,
-                                     num_train_epochs=epochs, weight_decay=wd,
-                                     report_to=report_to,
-                                     logging_dir=os.path.join(o_dir, 'log') if report_to!='none' else None,
-                                     logging_steps = len(ddict["train"]) // bs,
-                                     )
+                                      learning_rate=lr, 
+                                      warmup_ratio=warmup_ratio,
+                                      lr_scheduler_type=lr_scheduler_type, 
+                                      fp16=True,
+                                      do_train=True,
+                                      do_eval= not no_valid,
+                                      evaluation_strategy="no" if no_valid else "epoch", 
+                                      save_strategy="epoch" if save_checkpoint else 'no',
+                                      overwrite_output_dir=True,
+                                      gradient_accumulation_steps=grad_accum_steps,
+                                      per_device_train_batch_size=bs, 
+                                      per_device_eval_batch_size=val_bs,
+                                      num_train_epochs=epochs,
+                                      max_steps=epochs*((len_train//bs)//grad_accum_steps) if len_train else -1,
+                                      weight_decay=wd,
+                                      report_to=report_to,
+                                      logging_dir=os.path.join(o_dir, 'log') if report_to!='none' else None,
+                                      logging_steps = len_train//bs if len_train else len(ddict["train"]) // bs
+                                      )
 
     # instantiate trainer
     trainer_class = Trainer if trainer_class is None else trainer_class
     trainer = trainer_class(
         model=model,
         model_init=model_init if model is None else None,
         args=training_args,
@@ -153,26 +156,28 @@
                           data_collator=None, # HuggingFace data collator
                           state_name='last_hidden_state', # Name of the state to extract
                           state_idx=0, # The index (or indices) of the state to extract
                           device = None, # device that the model is trained on
                           ):
     state_idx = val2iterable(state_idx)
     
-    if data_collator is not None:    
+    if 'input_ids' in batch and isinstance(batch['input_ids'],list):
 # --- Convert from  
 # {'input_ids': [tensor([    0, 10444,   244, 14585,   125,  2948,  5925,   368,     2]), 
 #                tensor([    0, 16098,  2913,   244,   135,   198, 34629,  6356,     2])]
 # 'attention_mask': [tensor([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]), 
 #                    tensor([1, 1, 1, 1, 1, 1, 1, 1, 1])]
 #                    }
 # --- to
 # [{'input_ids': tensor([    0, 10444,   244, 14585,   125,  2948,  5925,   368,     2]),
 #   'attention_mask': tensor([1, 1, 1, 1, 1, 1, 1, 1, 1])},
 #  {'input_ids': tensor([    0, 16098,  2913,   244,   135,   198, 34629,  6356,     2]),
 #   'attention_mask': tensor([1, 1, 1, 1, 1, 1, 1, 1, 1])}]
+# --- so that you can apply data_collator to add padding
+
 
         # remove string text, due to transformer new version       
         collator_inp = []
         ks = [k for k in batch.keys() if k in model_input_names]
         vs = [batch[k] for k in ks]
         for pair in zip(*vs):
             collator_inp.append({k:v for k,v in zip(ks,pair)})
@@ -224,14 +229,15 @@
             save_checkpoint=False, # Whether to save weights (checkpoints) to o_dir
             hf_report_to='none', # The list of HuggingFace-allowed integrations to report the results and logs to
             grad_accum_steps=2, # Gradient will be accumulated over gradient_accumulation_steps steps.
             tokenizer=None, # Tokenizer (to override one in ```data_store```)
             data_collator=None, # Data Collator (to override one in ```data_store```)
             is_mlm=None, # Whether this is masked LM or casual LM
             trainer_class=None, # You can include the class name of your custom trainer here
+            len_train=None, # estimated number of samples in the whole training set (for streaming dataset only)
            ):
         
         if tokenizer is None: tokenizer=check_and_get_attribute(self.data_store,'tokenizer')
         if data_collator is None: data_collator=check_and_get_attribute(self.data_store,'data_collator')
         if ddict is None: ddict = check_and_get_attribute(self.data_store,'main_ddict')
         if is_mlm is None: is_mlm = check_and_get_attribute(self.data_store,'is_mlm')
         
@@ -259,15 +265,17 @@
                               grad_accum_steps=grad_accum_steps,
                               lr_scheduler_type=lr_scheduler_type,
                               warmup_ratio=warmup_ratio,
                               no_valid=no_valid,
                               val_bs=val_batch_size,
                               seed=self.seed,
                               trainer_class=trainer_class,
-                              report_to=hf_report_to)
+                              report_to=hf_report_to,
+                              len_train=len_train,
+                             )
         
         if not no_valid:
             eval_results = trainer.evaluate()
             try:
                 perplexity = math.exp(eval_results["eval_loss"])
                 print(f'Perplexity on validation set: {perplexity:.3f}')
             except OverflowError:
@@ -305,15 +313,15 @@
                       dset:Dataset, # A processed and tokenized Dataset
                       **kwargs, # keyword arguments for HuggingFace's text-generation (for clm) or fill-mask (for mlm)
                      ):
         is_mlm = check_and_get_attribute(self.data_store,'is_mlm')
         tokenizer=check_and_get_attribute(self.data_store,'tokenizer')
         main_text=check_and_get_attribute(self.data_store,'main_text')
         _task = 'fill-mask' if is_mlm else 'text-generation'
-        pipeline_obj = pipeline(_task,model=self.model,tokenizer=tokenizer,device=self.model.device)
+        pipeline_obj = pipeline(task=_task,model=self.model,tokenizer=tokenizer,device=self.model.device)
         str_list = dset[main_text]
         if _task=='fill-mask':
             all_tfms = self.data_store.content_tfms 
             all_tfms = partial(func_all,functions=all_tfms) if len(all_tfms) else lambda x: x
             mask_str = all_tfms(tokenizer.mask_token)
             str_list = [str(s).replace(mask_str,tokenizer.mask_token) for s in str_list]
         return [pipeline_obj(s,**kwargs) for s in str_list]
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/model_main.py` & `that-nlp-library-0.2.2/that_nlp_library/model_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_model_main.ipynb.
 
 # %% ../nbs/03_model_main.ipynb 3
 from __future__ import annotations
 import os
-from transformers import Trainer, TrainingArguments, AutoConfig
+from transformers import Trainer, TrainingArguments, AutoConfig, DataCollatorWithPadding
 from datasets import DatasetDict,Dataset
 import torch
 import gc
 from sklearn.metrics import accuracy_score
 from functools import partial
 import numpy as np
 from .utils import *
@@ -207,40 +207,45 @@
              lr_scheduler_type='cosine',  # The scheduler type to use. Including: linear, cosine, cosine_with_restarts, polynomial, constant, constant_with_warmup
              warmup_ratio=0.1, # The warmup ratio for some lr scheduler
              no_valid=False, # Whether there is a validation set or not
              val_bs=None, # Validation batch size
              seed=None, # Random seed
              report_to='none', # The list of integrations to report the results and logs to. Supported platforms are "azure_ml", "comet_ml", "mlflow", "neptune", "tensorboard","clearml" and "wandb". Use "all" to report to all integrations installed, "none" for no integrations.
              trainer_class=None, # You can include the class name of your custom trainer here
+             len_train=None, # estimated number of samples in the whole training set (for streaming dataset only)
             ):
     "The main model training/finetuning function"
     torch.cuda.empty_cache()
     gc.collect()
     if val_bs is None: val_bs = bs
     if seed:
         seed_everything(seed)
         
     training_args = TrainingArguments(o_dir, 
-                                learning_rate=lr, 
-                                warmup_ratio=warmup_ratio,
-                                lr_scheduler_type=lr_scheduler_type, 
-                                fp16=True,
-                                do_train=True,
-                                do_eval= not no_valid,
-                                evaluation_strategy="no" if no_valid else "epoch", 
-                                save_strategy="epoch" if save_checkpoint else 'no',
-                                overwrite_output_dir=True,
-                                gradient_accumulation_steps=grad_accum_steps,
-                                per_device_train_batch_size=bs, 
-                                per_device_eval_batch_size=val_bs,
-                                num_train_epochs=epochs, weight_decay=wd,
-                                report_to=report_to,
-                                logging_dir=os.path.join(o_dir, 'log') if report_to!='none' else None,
-                                logging_steps = len(ddict["train"]) // bs,
-                                )
+                                      learning_rate=lr, 
+                                      warmup_ratio=warmup_ratio,
+                                      lr_scheduler_type=lr_scheduler_type, 
+                                      fp16=True,
+                                      do_train=True,
+                                      do_eval= not no_valid,
+                                      evaluation_strategy="no" if no_valid else "epoch", 
+                                      save_strategy="epoch" if save_checkpoint else 'no',
+                                      overwrite_output_dir=True,
+                                      gradient_accumulation_steps=grad_accum_steps,
+                                      per_device_train_batch_size=bs, 
+                                      per_device_eval_batch_size=val_bs,
+                                      num_train_epochs=epochs,
+                                      max_steps=epochs*((len_train//bs)//grad_accum_steps) if len_train else -1,
+                                      weight_decay=wd,
+                                      report_to=report_to,
+                                      logging_dir=os.path.join(o_dir, 'log') if report_to!='none' else None,
+                                      logging_steps = len_train//bs if len_train else len(ddict["train"]) // bs 
+                                     )
+    # reference for max_steps:
+#     https://stackoverflow.com/questions/76011298/huggingface-trainer-max-step-to-set-for-streaming-dataset
 
     # instantiate trainer
     trainer_class = Trainer if trainer_class is None else trainer_class
     trainer = trainer_class(
         model=model,
         model_init=model_init if model is None else None,
         args=training_args,
@@ -263,36 +268,40 @@
                              model_input_names=['input_ids', 'token_type_ids', 'attention_mask'], # Model required inputs, from tokenizer.model_input_names
                              data_collator=None, # HuggingFace data collator
                              label_names=[], # Names of the label columns
                              head_sizes=[], # Class size for each head. Regression head will have head size 1
                              device = None, # device that the model is trained on
                              are_heads_separated=False, # is this multi-head, but each head has a separated logit?
                              ):
-    if data_collator is not None:
+    
+    if 'input_ids' in batch and isinstance(batch['input_ids'],list):
         
 # --- Convert from  
 # {'input_ids': [tensor([    0, 10444,   244, 14585,   125,  2948,  5925,   368,     2]), 
 #                tensor([    0, 16098,  2913,   244,   135,   198, 34629,  6356,     2])]
 # 'attention_mask': [tensor([1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]), 
 #                    tensor([1, 1, 1, 1, 1, 1, 1, 1, 1])]
 #                    }
 # --- to
 # [{'input_ids': tensor([    0, 10444,   244, 14585,   125,  2948,  5925,   368,     2]),
 #   'attention_mask': tensor([1, 1, 1, 1, 1, 1, 1, 1, 1])},
 #  {'input_ids': tensor([    0, 16098,  2913,   244,   135,   198, 34629,  6356,     2]),
 #   'attention_mask': tensor([1, 1, 1, 1, 1, 1, 1, 1, 1])}]
+# --- so that you can apply data_collator to add padding
 
         # remove string text, due to transformer new version       
         collator_inp = []
         ks = [k for k in batch.keys() if k in model_input_names+['label']]
         vs = [batch[k] for k in ks]
+        
         for pair in zip(*vs):
             collator_inp.append({k:v for k,v in zip(ks,pair)})
         
         batch = data_collator(collator_inp)
+        
     
     inputs = {k:v.to(device) for k,v in batch.items()
               if k in model_input_names}
     
     assert len(label_names)==len(head_sizes), "Length of `label_names` must equal to length of `head_sizes`"
         
     # switch to eval mode for evaluation
@@ -405,24 +414,27 @@
             warmup_ratio=0.1, # The warmup ratio for some lr scheduler
             o_dir = './tmp_weights', # Directory to save weights
             save_checkpoint=False, # Whether to save weights (checkpoints) to o_dir
             hf_report_to='none', # The list of HuggingFace-allowed integrations to report the results and logs to
             compute_metrics=compute_metrics, # A function to compute metric, e.g. `compute_metrics` which utilizes the given ```metric_funcs``` 
             grad_accum_steps=2, # Gradient will be accumulated over gradient_accumulation_steps steps.
             tokenizer=None, # Tokenizer (to override one in ```data_store```)
-            data_collator=None, # Data Collator (to override one in ```data_store```)
             label_names=None, # Names of the label (dependent variable) columns (to override one in ```data_store```)
             head_sizes=None, # Class size for each head (to override one in ```model```)
             trainer_class=None, # You can include the class name of your custom trainer here
+            len_train=None, # Number of samples in the whole training set (for streaming dataset only)
            ):
         
         if tokenizer is None: tokenizer=check_and_get_attribute(self.data_store,'tokenizer')
-        if data_collator is None: data_collator=getattr(self.data_store,'data_collator',None)
-        if ddict is None: ddict = check_and_get_attribute(self.data_store,'main_ddict')
             
+        # define data collator if no padding is added during preprocess (aka when max_length is -1)
+        max_length = getattr(self.data_store,'max_length',-1) 
+        data_collator= DataCollatorWithPadding(tokenizer,padding=True,pad_to_multiple_of=8) if max_length==-1 else None
+        
+        if ddict is None: ddict = check_and_get_attribute(self.data_store,'main_ddict')    
         if label_names is None: label_names=check_and_get_attribute(self.data_store,'label_names')
         label_names = val2iterable(label_names)
         
         if val_batch_size is None: val_batch_size=batch_size
         
         if head_sizes is None: 
             head_sizes=check_and_get_attribute(self.data_store,'label_lists')
@@ -436,28 +448,35 @@
         _compute_metrics = partial(compute_metrics,
                                    metric_funcs=metric_funcs,
                                    metric_types=metric_types,
                                    head_sizes=head_sizes,
                                    label_names=label_names 
                                   )
         
-        trainer = finetune(learning_rate,batch_size,weight_decay,epochs,
-                           ddict,tokenizer,o_dir,
+        trainer = finetune(learning_rate,
+                           batch_size,
+                           weight_decay,
+                           epochs,
+                           ddict,
+                           tokenizer,
+                           o_dir,
                            save_checkpoint=save_checkpoint,
                            model=self.model,
                            data_collator=data_collator,
                            compute_metrics=_compute_metrics,
                            grad_accum_steps=grad_accum_steps,
                            lr_scheduler_type=lr_scheduler_type,
                            warmup_ratio=warmup_ratio,
                            no_valid=no_valid,
                            val_bs=val_batch_size,
                            seed=self.seed,
                            trainer_class=trainer_class,
-                           report_to=hf_report_to)
+                           report_to=hf_report_to,
+                           len_train=len_train,
+                          )
         self.trainer = trainer
         
     def predict_raw_text(self,
                          content:dict|list|str, # Either a single sentence, list of sentence or a dictionary where keys are metadata, values are list
                          is_multilabel=None, # Is this a multilabel classification?
                          multilabel_threshold=0.5, # Threshold for multilabel classification
                          topk=1, # Number of labels to return for each head
@@ -504,25 +523,27 @@
                       ddict:DatasetDict|Dataset=None, # A processed and tokenized DatasetDict/Dataset (will override one in ```data_store```)
                       ds_type='test', # The split of DatasetDict to predict
                       batch_size=16, # Batch size for making prediction on GPU
                       is_multilabel=None, # Is this a multilabel classification?
                       multilabel_threshold=0.5, # Threshold for multilabel classification
                       topk=1, # Number of labels to return for each head
                       tokenizer=None, # Tokenizer (to override one in ```data_store```)
-                      data_collator=None, # Data Collator (to override one in ```data_store```)
                       label_names=None, # Names of the label (dependent variable) columns (to override one in ```data_store```)
                       class_names_predefined=None, # List of names associated with the labels (same index order) (to override one in ```data_store```)
                       are_heads_separated=False # Are outputs (of model) separate heads?
                      ):
         device = self.model.device
         if is_multilabel is None: is_multilabel=getattr(self.model,'is_multilabel',False)
         label_lists = class_names_predefined
-        if tokenizer is None: tokenizer=check_and_get_attribute(self.data_store,'tokenizer')
-        if data_collator is None: data_collator=getattr(self.data_store,'data_collator',None)
-        if label_names is None: label_names=check_and_get_attribute(self.data_store,'label_names')
+        if tokenizer is None: tokenizer = check_and_get_attribute(self.data_store,'tokenizer')
+            
+        # use data collator to pad any batch of tokenized texts that have not been padded
+        data_collator = DataCollatorWithPadding(tokenizer,padding=True,pad_to_multiple_of=8)
+    
+        if label_names is None: label_names = check_and_get_attribute(self.data_store,'label_names')
         if label_lists is None: label_lists = check_and_get_attribute(self.data_store,'label_lists')
         label_names = val2iterable(label_names)
         if not isinstance(label_lists[0],list):
             label_lists=[label_lists]    
         head_sizes = [len(hs) if len(hs) else 1 for hs in label_lists]
         if ddict is None: ddict = check_and_get_attribute(self.data_store,'main_ddict')
         if isinstance(ddict,DatasetDict):
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/models/gpt2/classifiers.py` & `that-nlp-library-0.2.2/that_nlp_library/models/gpt2/classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     def __init__(self,config, # HuggingFace model configuration
                  layer2concat=4, # number of hidden layer to concatenate (counting from top)
                  is_multilabel=False, # Whether this is a multilabel classification
                  is_multihead=False, # Whether this is a multihead (multi-level) classification
                  head_class_sizes=[], # Class size for each head
                  head_weights=[], # loss weight for each head. This will be multiplied to the loss of each head's output
-                 head_class=None, # The class object of the head
+                 head_class=None, # The class object of the head. You can use ConcatHeadSimple or ConcatHeadExtended
                  **head_class_kwargs, # Keyword arguments for the head class
                 ):
         super().__init__(config)
         self.is_multilabel = is_multilabel
         self.is_multihead = is_multihead
         self.head_class_sizes = val2iterable(head_class_sizes)
         self.head_weights = val2iterable(head_weights,lsize=len(self.head_class_sizes))
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/models/roberta/classifiers.py` & `that-nlp-library-0.2.2/that_nlp_library/models/roberta/classifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,16 @@
                 ):
         super().__init__()
         self.dense = torch.nn.Linear(config.hidden_size, config.hidden_size)
         self.dropout = torch.nn.Dropout(classifier_dropout)
         num_labels=num_labels if num_labels is not None else config.num_labels
         self.out_proj = torch.nn.Linear(config.hidden_size, num_labels)
 
-    def forward(self, features, **kwargs):
-        x = self.dropout(x)
+    def forward(self, inp, **kwargs):
+        x = self.dropout(inp)
         x = self.dense(x)
         x = torch.tanh(x)
         x = self.dropout(x)
         x = self.out_proj(x)
         return x
 
 # %% ../../../nbs/04_models.roberta.classifiers.ipynb 12
@@ -194,15 +194,15 @@
 
     def __init__(self,config, # HuggingFace model configuration
                  layer2concat=4, # number of hidden layer to concatenate (counting from top)
                  is_multilabel=False, # Whether this is a multilabel classification
                  is_multihead=False, # Whether this is a multihead (multi-level) classification
                  head_class_sizes=[], # Class size for each head
                  head_weights=[], # loss weight for each head. This will be multiplied to the loss of each head's output
-                 head_class=None, # The class object of the head. You can use RobertaClassificationHeadCustom as default
+                 head_class=None, # The class object of the head. You can use ConcatHeadSimple or ConcatHeadExtended
                  **head_class_kwargs, # Keyword arguments for the head class
                 ):
         super().__init__(config)
         self.is_multilabel = is_multilabel
         self.is_multihead = is_multihead
         self.head_class_sizes = val2iterable(head_class_sizes)
         self.head_weights = val2iterable(head_weights,lsize=len(self.head_class_sizes))
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/models/roberta/conditional_prob_classifiers.py` & `that-nlp-library-0.2.2/that_nlp_library/models/roberta/conditional_prob_classifiers.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library/models/roberta/deep_hierarchical_classifiers.py` & `that-nlp-library-0.2.2/that_nlp_library/models/roberta/deep_hierarchical_classifiers.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library/text_augmentation.py` & `that-nlp-library-0.2.2/that_nlp_library/text_augmentation.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library/text_main.py` & `that-nlp-library-0.2.2/that_nlp_library/text_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
                    truncation=True,
                    is_split_into_words=is_split_into_words,
                    return_tensors=return_tensors,
                    return_special_tokens_mask=return_special_tokens_mask
                   )
     if isinstance(max_length,int) and max_length>0:
         # pad to the largest length of the current batch, and start truncating at max_length
+        # Note: that means it does not always pad to max length
         return tok(text, padding=True, 
                    max_length=max_length,
                    truncation=True,
                    is_split_into_words=is_split_into_words,
                    return_tensors=return_tensors,
                    return_special_tokens_mask=return_special_tokens_mask
                   )
@@ -620,14 +621,15 @@
                         trn_size=None, # The number of training data to be tokenized
                         tok_num_proc=None, # Number of processes for tokenization
                        ):
         print_msg('Tokenization',20,verbose=self.verbose)
         self.tokenizer = tokenizer
         self.max_length = max_length
         self.tok_num_proc = tok_num_proc if tok_num_proc else self.num_proc
+        
         tok_func = partial(tokenize_function,tok=tokenizer,max_length=max_length)
         _func = partial(lambda_map_batch,
                         feature=self.main_text,
                         func=tok_func,
                         output_feature=None,
                         is_batched=self.is_batched)
         
@@ -637,15 +639,15 @@
             else: # int
                 trn_len=len(self.main_ddict['train'])
                 num_shard = trn_len//trn_size
             self.main_ddict['train'] = self.main_ddict['train'].shard(num_shard,0)
         
         for k in self.main_ddict.keys():
             self.main_ddict[k] = hf_map_dset(self.main_ddict[k],_func,self.is_batched,self.batch_size,self.tok_num_proc)
-
+        
         self.verboseprint('Done')
         return self.main_ddict
         
     def process_and_tokenize(self,
                              tokenizer, # Tokenizer (preferably from HuggingFace)
                              max_length=None, # pad to model's allowed max length (default is max_sequence_length)
                              trn_size=None, # The number of training data to be tokenized
@@ -657,17 +659,14 @@
         This will perform `do_all_processing` then `do_tokenization`
         """
         if self.seed:
             seed_everything(self.seed) 
         _ = self.do_all_preprocessing(shuffle_trn,check_val_leak)
         _ = self.do_tokenization(tokenizer,max_length,trn_size,tok_num_proc)
         
-    
-    def set_data_collator(self,data_collator):
-        self.data_collator = data_collator
         
     
     def prepare_test_dataset_from_csv(self,
                                       file_path, # path to csv file
                                       do_filtering=False # whether to perform data filtering on this test set
                                      ):
         file_path = Path(file_path)
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/text_main_lm.py` & `that-nlp-library-0.2.2/that_nlp_library/text_main_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,18 @@
                           is_mlm=True, # Is this masked language model (True) or causal language model (False)
                           mlm_prob=0.15, # Mask probability for masked language model
                          ):
         if not hasattr(self,'max_length'):
             raise ValueError("Please call `process_and_tokenize' or `do_tokenization` to tokenize your dataset")
         
         self.is_mlm = is_mlm
-        pad_to_multiple_of_8 = (self.max_length<0) # get data collator to pad
+        
+        # get data collator to pad
+        pad_to_multiple_of_8 = True if self.max_length is not None and self.max_length<0 else False
+
         self.data_collator = DataCollatorForLanguageModeling(tokenizer=self.tokenizer,
                                                              mlm=is_mlm,
                                                              mlm_probability=mlm_prob,
                                                              pad_to_multiple_of=8 if pad_to_multiple_of_8 else None
                                                             )
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/text_main_lm_streaming.py` & `that-nlp-library-0.2.2/that_nlp_library/text_main_lm_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 class TextDataLMControllerStreaming(TextDataControllerStreaming):
     def __init__(self,
                  inp, # HuggingFainpce Dataset or DatasetDict
                  main_text:str, # Name of the main text column
                  filter_dict={}, # A dictionary: {feature: filtering_function_for_that_feature}
                  metadatas=[], # Names of the metadata columns
                  process_metas=True, # Whether to do simple text processing on the chosen metadatas
+                 metas_sep='.', # Separator, for multiple metadatas concatenation
                  content_transformations=[], # A list of text transformations
                  seed=None, # Random seed
                  batch_size=1024, # Transformation + Tokenization batch size
                  num_proc=1, # Number of process for multiprocessing
                  cols_to_keep=None, # Columns to keep after all processings
                  verbose=True, # Whether to prdint processing information
                 ):
         
         super().__init__(inp=inp,
                          main_text=main_text,
                          filter_dict=filter_dict,
                          metadatas=metadatas,
                          process_metas=process_metas,
+                         metas_sep=metas_sep,
                          content_transformations=content_transformations,
                          seed=seed,
                          batch_size=batch_size,
                          num_proc=num_proc,
                          cols_to_keep=cols_to_keep,
                          verbose=verbose
                         )
@@ -237,29 +239,34 @@
     
     def set_data_collator(self,
                           is_mlm=True, # Is this masked language model (True) or causal language model (False)
                           mlm_prob=0.15, # Mask probability for masked language model
                          ):
         if not hasattr(self,'max_length'):
             raise ValueError("Please call `process_and_tokenize' or `do_tokenization` to tokenize your dataset")
-            
-        pad_to_multiple_of_8 = (self.max_length<0) # get data collator to pad when tokenizer does not apply padding
+        
+        self.is_mlm = is_mlm
+        
+        # get data collator to pad
+        pad_to_multiple_of_8 = True if self.max_length is not None and self.max_length<0 else False
+
         self.data_collator = DataCollatorForLanguageModeling(tokenizer=self.tokenizer,
                                                              mlm=is_mlm,
                                                              mlm_probability=mlm_prob,
                                                              pad_to_multiple_of=8 if pad_to_multiple_of_8 else None
                                                             )
                                                
+    
     def prepare_test_dataset_from_raws(self,
                                        content, # Either a single sentence, list of sentence or a dictionary with keys are metadata columns and values are list
                                        do_tokenize=False, # Whether to tokenize text
                                       ):
         if len(self.metadatas) and not isinstance(content,dict):
             raise ValueError(f'There is/are metadatas in the preprocessing step. Please include a dictionary including these keys for metadatas: {self.metadatas}, and texture content: {self.main_text}')
-            
+        
         _dic = {self.main_text:[content]} if isinstance(content,str) else content
         for k in _dic.keys():
             _dic[k] = val2iterable(_dic[k])
         
         test_dict = Dataset.from_dict(_dic)
         
         # set num_proc to 1 for small data processing
@@ -272,15 +279,15 @@
         self.tok_num_proc=_tmp2
         return results
         
     def prepare_test_dataset(self,
                              test_dset, # The HuggingFace Dataset as Test set
                              do_tokenize, # Whether to tokenize text
                             ):
-            
+        
         test_cols = set(get_dset_col_names(test_dset))
         missing_cols = set(self.cols_to_keep) - test_cols
         if len(missing_cols):
             raise ValueError(f'Test set does not have these columns required for preprocessings: {missing_cols}')
             
         print_msg('Start Test Set Transformation',20,verbose=self.verbose)
         
@@ -290,15 +297,15 @@
         # Content transformation
         test_dset = self._do_transformation(test_dset)
         
         # Drop unused columns
         cols_to_remove = test_cols - set(self.cols_to_keep)
         test_dset = test_dset.remove_columns(list(cols_to_remove))
         
-        if do_tokenize:
+        if do_tokenize:   
             print_msg('Tokenization',20,verbose=self.verbose)
             tok_func = partial(tokenize_function,
                            tok=self.tokenizer,
                            max_length=self.max_length if self.line_by_line else -1,
                            return_special_tokens_mask=True
                           )
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/text_main_streaming.py` & `that-nlp-library-0.2.2/that_nlp_library/text_main_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  label_names=[], # Names of the label (dependent variable) columns
                  sup_types=[], # Type of supervised learning for each label name ('classification' or 'regression')
                  class_names_predefined=[], # List of names associated with the labels (same index order)
                  filter_dict={}, # A dictionary: {feature: filtering_function_based_on_the_feature}
                  label_tfm_dict={}, # A dictionary: {label_name: transform_function_for_that_label}
                  metadatas=[], # Names of the metadata columns
                  process_metas=True, # Whether to do simple text processing on the chosen metadatas
+                 metas_sep='.', # Separator, for multiple metadatas concatenation
                  content_transformations=[], # A list of text transformations
                  content_augmentations=[], # A list of text augmentations
                  seed=None, # Random seed
                  batch_size=1024, # CPU batch size
                  num_proc=1, # Number of process for multiprocessing. This will be applied on non-streamed validation set
                  cols_to_keep=None, # Columns to keep after all processings
                  verbose=True, # Whether to print processing information
@@ -43,31 +44,27 @@
         self._check_sup_types()
         self.label_lists = class_names_predefined
         
         self.filter_dict = filter_dict
         self.label_tfm_dict = label_tfm_dict
         self.metadatas = val2iterable(metadatas)
         self.process_metas = process_metas
+        self.metas_sep = metas_sep
 
         self.content_tfms = val2iterable(content_transformations)
         self.aug_tfms = val2iterable(content_augmentations)
         
         self.seed = seed
         self.is_batched = batch_size>1
         self.batch_size = batch_size
         self.num_proc = num_proc
         self.cols_to_keep = cols_to_keep
 
         self.main_ddict=DatasetDict()
-        self.verbose = verbose
-        self.verboseprint = print if verbose else lambda *a, **k: None
-        if not self.verbose:
-            disable_progress_bar() # turn off huggingface `map` progress bar
-        else:
-            enable_progress_bar()
+        self.set_verbose(verbose)
             
         if hasattr(inp,'keys'): # is datasetdict
             if 'train' not in inp.keys(): 
                 raise ValueError('The given DatasetDict has no "train" split')
             else:
                 self.main_ddict['train'] = inp['train']
             val_key = list(set(inp.keys()) & set(['val','validation','valid']))
@@ -96,14 +93,18 @@
                     parent='pickle_files' # Parent folder
                    ):
         return load_pickle(fname,parent=parent)
     
     def set_verbose(self,verbose):
         self.verbose = verbose
         self.verboseprint = print if verbose else lambda *a, **k: None
+        if not self.verbose:
+            disable_progress_bar() # turn off huggingface `map` progress bar
+        else:
+            enable_progress_bar()
     
     def _convert_regression_to_float(self):
         if len(self.sup_types)==0: return
         # convert regression labels to float64
         reg_idxs = [i for i,v in enumerate(self.sup_types) if v=='regression']
         for i in reg_idxs:
             self.main_ddict['train'] = self.main_ddict['train'].cast_column(self.label_names[i],Value("float64"))
@@ -146,14 +147,15 @@
     
     def _process_metadatas(self,dtrain):
         if len(self.metadatas):
             map_func = partial(concat_metadatas,
                                main_text=self.main_text,
                                metadatas=self.metadatas,
                                process_metas=self.process_metas,
+                               sep=self.metas_sep,
                                is_batched=self.is_batched)
             dtrain = hf_map_dset(dtrain,map_func,self.is_batched,self.batch_size,self.num_proc)
         return dtrain
     
     def _do_label_transformation(self):
         if len(self.label_names)==0 or len(self.label_tfm_dict)==0: return
         print_msg('Label Transformation',20,verbose=self.verbose)
@@ -259,15 +261,25 @@
                     _func = partial(lambda_batch,
                                     feature=f,
                                     func=tfm,
                                     is_batched=self.is_batched)
                     dtrain = hf_filter_dset(dtrain,_func,self.is_batched,self.batch_size,self.num_proc)
         return dtrain
         
-
+    def _do_transformation(self,dset):
+        if len(self.content_tfms):
+            for tfm in self.content_tfms:
+                _func = partial(lambda_map_batch,
+                               feature=self.main_text,
+                               func=tfm,
+                               is_batched=self.is_batched)
+                dset = hf_map_dset(dset,_func,self.is_batched,self.batch_size,self.num_proc)
+                
+        return dset
+    
     def _do_transformation_tokenization(self,dtrain):
         tok_func = partial(tokenize_function,tok=self.tokenizer,max_length=self.max_length)
         if len(self.content_tfms):            
             for tfm in self.content_tfms:
                 _func = partial(lambda_map_batch,
                                 feature=self.main_text,
                                 func=tfm,
@@ -336,25 +348,24 @@
             
         if len(final_dict[self.main_text]):
             # hasn't reached batch_size (of last batch)
             dtrain = Dataset.from_dict(final_dict)
             dtrain = self._do_transformation_augmentation_tokenization(dtrain,tok_func,all_tfms)
             yield from _get_generator(dtrain)
             
-        
-            
+         
     def _do_transformation_augmentation_tokenization_generator(self):
         tok_func = partial(tokenize_function,tok=self.tokenizer,max_length=self.max_length)
         all_tfms = self.content_tfms + self.aug_tfms
         
         self.main_ddict['train'] = IterableDataset.from_generator(self._construct_generator_with_batch,
-                                                   gen_kwargs={'dset': self.main_ddict['train'],
-                                                               'tok_func':tok_func,
-                                                               'all_tfms': all_tfms
-                                                              }
+                                                                  gen_kwargs={'dset': self.main_ddict['train'],
+                                                                              'tok_func':tok_func,
+                                                                              'all_tfms': all_tfms
+                                                                             }
                                                                  )
     
     def _do_transformation_augmentation_tokenization_generator_linebyline(self):
         def _get_generator(dset,tok_func,all_tfms):
             for inp in dset:
                 # inp[text_name] will be a single item
                 inp[self.main_text]=all_tfms(inp[self.main_text])
@@ -365,18 +376,18 @@
         
         # no padding for tokenization
         tok_func = partial(tokenize_function,tok=self.tokenizer,max_length=-1) 
         all_tfms = self.content_tfms + self.aug_tfms
         all_tfms = partial(func_all,functions=all_tfms) if len(all_tfms) else lambda x: x
            
         self.main_ddict['train'] = IterableDataset.from_generator(_get_generator,
-                                                   gen_kwargs={'dset': self.main_ddict['train'],
-                                                               'tok_func':tok_func,
-                                                               'all_tfms': all_tfms
-                                                              }
+                                                                  gen_kwargs={'dset': self.main_ddict['train'],
+                                                                              'tok_func':tok_func,
+                                                                              'all_tfms': all_tfms
+                                                                             }
                                                                  )
 
         
     def process_and_tokenize(self,
                              tokenizer, # Tokenizer (preferably from HuggingFace)
                              max_length=None, # pad to model's allowed max length (default is max_sequence_length)
                              tok_num_proc=None, # Number of processes for tokenization
@@ -405,15 +416,15 @@
         
         # Label transformation
         self._do_label_transformation()
         
         # Process labels
         self._encode_labels()
 
-        # Dropping unused columns
+        # Drop unused columns
         self._simplify_ddict()
 
         if self.seed:
             seed_everything(self.seed)
             
         # Content transformation + tokenization for validation
         if 'validation' in self.main_ddict.keys():
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library/text_transformation.py` & `that-nlp-library-0.2.2/that_nlp_library/text_transformation.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library/utils.py` & `that-nlp-library-0.2.2/that_nlp_library/utils.py`

 * *Files identical despite different names*

### Comparing `that-nlp-library-0.2.1/that_nlp_library.egg-info/PKG-INFO` & `that-nlp-library-0.2.2/that_nlp_library.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-nlp-library
-Version: 0.2.1
+Version: 0.2.2
 Summary: Aim to be a convenient NLP library with the help from HuggingFace
 Home-page: https://github.com/anhquan0412/that-nlp-library
 Author: Quan Tran
 Author-email: anhquan0412@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev,python,nlp,natural language processing,transformer,deep learning,envibert,roberta,gpt2,phobert
 Classifier: Development Status :: 4 - Beta
@@ -136,16 +136,18 @@
 This library also a **streamed version of Text Controller**
 ([`TextDataControllerStreaming`](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html#textdatacontrollerstreaming)),
 allowing you to work with data without having it entirely on your hard
 drive. You can still perform all the processings in the non-streamed
 version, except for **Train/Validation split** (which means you have to
 define your validation set beforehand), and **Upsampling**.
 
-For more details on **streaming**, visit
-[here](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html).
+For more details on **streaming**, visit [how to create a streamed
+dataset](https://anhquan0412.github.io/that-nlp-library/text_main_streaming.html)
+and [how to train a model with a streamed
+dataset](https://anhquan0412.github.io/that-nlp-library/roberta_singlehead_for_streaming)
 
 If you are curious on the time and space efficiency between streamed and
 non-streamed version, visit the benchmark
 [here](https://anhquan0412.github.io/that-nlp-library/text_main_benchmark.html)
 
 ### **Model and [`ModelController`](https://anhquan0412.github.io/that-nlp-library/model_main.html#modelcontroller)**
 
@@ -192,15 +194,15 @@
 for training your data. There’s a quick tutorial on this decoupling
 [here](https://anhquan0412.github.io/that-nlp-library/model_classification_tutorial.html#train-model-with-only-a-tokenized-datasetdict-no-textdatacontroller)
 
 ## Language Modeling
 
 For language modeling, the main pipeline also contains 2 parts
 
-### Text Data Controlelr for Language Model: [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
+### Text Data Controller for Language Model: [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
 
 Similarly to `TextDatController`,
 [`TextDataLMController`](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html#textdatalmcontroller)
 also provide a list of processings (except for **Label Processing**,
 **Upsampling** and **Text Augmentation**). The controller also allow
 tokenization line-by-line or by token concatenation. Visit the tutorial
 [here](https://anhquan0412.github.io/that-nlp-library/text_main_lm.html)
```

### Comparing `that-nlp-library-0.2.1/that_nlp_library.egg-info/SOURCES.txt` & `that-nlp-library-0.2.2/that_nlp_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

