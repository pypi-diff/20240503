# Comparing `tmp/llm-dataset-converter-0.2.1.tar.gz` & `tmp/llm-dataset-converter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-dataset-converter-0.2.1.tar", last modified: Thu May  2 02:48:29 2024, max compression
+gzip compressed data, was "llm-dataset-converter-0.2.2.tar", last modified: Fri May  3 02:53:27 2024, max compression
```

## Comparing `llm-dataset-converter-0.2.1.tar` & `llm-dataset-converter-0.2.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6205 2024-05-02 02:47:22.000000 llm-dataset-converter-0.2.1/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1326 2024-02-27 03:36:56.000000 llm-dataset-converter-0.2.1/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 llm-dataset-converter-0.2.1/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     9521 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    26691 2024-05-01 21:39:25.000000 llm-dataset-converter-0.2.1/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1784 2024-05-02 02:47:22.000000 llm-dataset-converter-0.2.1/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.135106 llm-dataset-converter-0.2.1/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.1/src/ldc/__init__.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/api/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       78 2024-02-20 02:26:03.000000 llm-dataset-converter-0.2.1/src/ldc/api/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      740 2024-02-04 22:38:10.000000 llm-dataset-converter-0.2.1/src/ldc/api/_downloader.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      513 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/api/_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10115 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/api/_io.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4518 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/api/pretrain.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/api/supervised/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-20 01:36:43.000000 llm-dataset-converter-0.2.1/src/ldc/api/supervised/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5031 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/api/supervised/classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4930 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/api/supervised/pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4644 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/api/translation.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      732 2024-05-01 00:00:52.000000 llm-dataset-converter-0.2.1/src/ldc/class_lister.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6705 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/core.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.139106 llm-dataset-converter-0.2.1/src/ldc/downloader/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       37 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/downloader/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5145 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.1/src/ldc/downloader/_huggingface.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/filter/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1525 2024-02-29 00:29:25.000000 llm-dataset-converter-0.2.1/src/ldc/filter/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8050 2024-02-28 21:04:31.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_assemble_sentences.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6900 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_change_case.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6756 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_file_filter.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8622 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_find_substr.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8853 2024-02-29 00:25:34.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_inspect.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7806 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_keyword.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3362 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_llama2_to_pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3694 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_max_records.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8496 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_metadata.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4725 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_metadata_from_name.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3716 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_llama2.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4040 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_pretrain.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5430 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_classification.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6427 2024-02-21 03:31:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3863 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_randomize_records.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4963 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_record_files.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5367 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_record_window.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8417 2024-02-28 21:47:45.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_remove_blocks.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6807 2024-02-28 21:47:45.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_remove_empty.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7363 2024-02-28 21:50:46.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_remove_patterns.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8077 2024-02-28 21:50:46.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_replace_patterns.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3675 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_reset_ids.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3049 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_ids.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6269 2024-02-28 21:55:59.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_text.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4994 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6087 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_tee.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8340 2024-02-28 21:55:59.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_text_length.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10587 2024-02-28 21:57:24.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_text_stats.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3555 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_to_llama2_format.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4763 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pairs.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3323 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pretrain.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2923 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.1/src/ldc/help.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/pretrain/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      383 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    24508 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    13378 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4207 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_max_length.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10566 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_parquet.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5020 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_sentences.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1785 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_split.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    18354 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.1/src/ldc/pretrain/_txt.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6875 2024-05-01 05:10:47.000000 llm-dataset-converter-0.2.1/src/ldc/registry.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/supervised/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-11 04:18:56.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/__init__.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.147106 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      343 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3739 2024-02-20 01:43:12.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_classification_label_map.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    26056 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    14455 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11723 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_parquet.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.151106 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      349 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7984 2024-03-13 03:03:11.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_alpaca.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    28291 2024-03-13 03:03:10.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15538 2024-03-13 03:03:10.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    13077 2024-03-13 03:04:17.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_parquet.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6051 2024-02-22 22:49:44.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_update_pair_data.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    15245 2024-03-13 03:04:56.000000 llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_xtuner.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10910 2024-03-13 03:40:26.000000 llm-dataset-converter-0.2.1/src/ldc/text_utils.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.151106 llm-dataset-converter-0.2.1/src/ldc/tool/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.1/src/ldc/tool/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     8605 2024-02-23 01:25:19.000000 llm-dataset-converter-0.2.1/src/ldc/tool/append.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7292 2024-02-21 21:28:28.000000 llm-dataset-converter-0.2.1/src/ldc/tool/convert.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3280 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.1/src/ldc/tool/download.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3783 2024-02-20 02:26:04.000000 llm-dataset-converter-0.2.1/src/ldc/tool/file_encoding.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7104 2024-02-04 23:37:50.000000 llm-dataset-converter-0.2.1/src/ldc/tool/find.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     7313 2024-05-01 05:12:36.000000 llm-dataset-converter-0.2.1/src/ldc/tool/help.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     5520 2024-02-05 00:23:10.000000 llm-dataset-converter-0.2.1/src/ldc/tool/paste.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.151106 llm-dataset-converter-0.2.1/src/ldc/translation/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      416 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.1/src/ldc/translation/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    24398 2024-03-13 03:16:06.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_csv.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    11807 2024-03-13 03:22:55.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_jsonlines.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3908 2024-02-20 01:45:23.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_language.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    10982 2024-03-13 03:22:55.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_parquet.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3203 2024-02-20 01:44:40.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_require_languages.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)    16901 2024-03-13 03:16:06.000000 llm-dataset-converter-0.2.1/src/ldc/translation/_txt.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      931 2024-02-04 22:44:57.000000 llm-dataset-converter-0.2.1/src/ldc/utils.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-02 02:48:29.155106 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     9521 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3087 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      371 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       88 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2024-05-02 02:48:29.000000 llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.192317 llm-dataset-converter-0.2.2/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6246 2024-05-03 02:49:53.000000 llm-dataset-converter-0.2.2/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1326 2024-02-27 03:36:56.000000 llm-dataset-converter-0.2.2/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 llm-dataset-converter-0.2.2/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     9602 2024-05-03 02:53:27.192317 llm-dataset-converter-0.2.2/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    26691 2024-05-01 21:39:25.000000 llm-dataset-converter-0.2.2/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2024-05-03 02:53:27.192317 llm-dataset-converter-0.2.2/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1784 2024-05-03 02:49:53.000000 llm-dataset-converter-0.2.2/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.176317 llm-dataset-converter-0.2.2/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.176317 llm-dataset-converter-0.2.2/src/ldc/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.2/src/ldc/__init__.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.176317 llm-dataset-converter-0.2.2/src/ldc/api/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       78 2024-02-20 02:26:03.000000 llm-dataset-converter-0.2.2/src/ldc/api/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      740 2024-02-04 22:38:10.000000 llm-dataset-converter-0.2.2/src/ldc/api/_downloader.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      513 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.2/src/ldc/api/_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10115 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.2/src/ldc/api/_io.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4518 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/api/pretrain.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.176317 llm-dataset-converter-0.2.2/src/ldc/api/supervised/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2024-02-20 01:36:43.000000 llm-dataset-converter-0.2.2/src/ldc/api/supervised/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5031 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.2/src/ldc/api/supervised/classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4930 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/api/supervised/pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4644 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/api/translation.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      732 2024-05-01 00:00:52.000000 llm-dataset-converter-0.2.2/src/ldc/class_lister.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6705 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.2/src/ldc/core.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.180317 llm-dataset-converter-0.2.2/src/ldc/downloader/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       37 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.2/src/ldc/downloader/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5145 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.2/src/ldc/downloader/_huggingface.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.184317 llm-dataset-converter-0.2.2/src/ldc/filter/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1525 2024-02-29 00:29:25.000000 llm-dataset-converter-0.2.2/src/ldc/filter/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8050 2024-02-28 21:04:31.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_assemble_sentences.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6900 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_change_case.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6756 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_file_filter.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8622 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_find_substr.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8853 2024-02-29 00:25:34.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_inspect.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7806 2024-02-28 21:33:27.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_keyword.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3362 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_llama2_to_pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3694 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_max_records.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8496 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_metadata.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4725 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_metadata_from_name.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3716 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_pairs_to_llama2.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4040 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_pairs_to_pretrain.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5430 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_pretrain_sentences_to_classification.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6427 2024-02-21 03:31:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_pretrain_sentences_to_pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3863 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_randomize_records.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4963 2024-02-21 01:05:00.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_record_files.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5367 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_record_window.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8417 2024-02-28 21:47:45.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_remove_blocks.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6807 2024-02-28 21:47:45.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_remove_empty.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7363 2024-02-28 21:50:46.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_remove_patterns.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8077 2024-02-28 21:50:46.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_replace_patterns.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3675 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_reset_ids.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3049 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_skip_duplicate_ids.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6269 2024-02-28 21:55:59.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_skip_duplicate_text.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4994 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6087 2024-02-28 20:24:40.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_tee.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8340 2024-02-28 21:55:59.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_text_length.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10587 2024-02-28 21:57:24.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_text_stats.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3555 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_to_llama2_format.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4763 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_translation_to_pairs.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3323 2024-02-20 02:26:16.000000 llm-dataset-converter-0.2.2/src/ldc/filter/_translation_to_pretrain.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2923 2024-03-14 00:42:26.000000 llm-dataset-converter-0.2.2/src/ldc/help.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.184317 llm-dataset-converter-0.2.2/src/ldc/pretrain/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      383 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    24508 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13378 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4207 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_max_length.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10566 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_parquet.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5020 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_sentences.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1785 2024-02-20 01:42:25.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_split.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    18354 2024-03-13 03:11:44.000000 llm-dataset-converter-0.2.2/src/ldc/pretrain/_txt.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6875 2024-05-01 05:10:47.000000 llm-dataset-converter-0.2.2/src/ldc/registry.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.188317 llm-dataset-converter-0.2.2/src/ldc/supervised/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-11 04:18:56.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/__init__.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.188317 llm-dataset-converter-0.2.2/src/ldc/supervised/classification/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      343 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/classification/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3739 2024-02-20 01:43:12.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_classification_label_map.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    26056 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    14455 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11723 2024-03-13 03:10:37.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_parquet.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.188317 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      349 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7984 2024-03-13 03:03:11.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_alpaca.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    28291 2024-03-13 03:03:10.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15538 2024-03-13 03:03:10.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    13077 2024-03-13 03:04:17.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_parquet.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6051 2024-02-22 22:49:44.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_update_pair_data.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    15245 2024-03-13 03:04:56.000000 llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_xtuner.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10910 2024-03-13 03:40:26.000000 llm-dataset-converter-0.2.2/src/ldc/text_utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.188317 llm-dataset-converter-0.2.2/src/ldc/tool/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-08-14 22:03:25.000000 llm-dataset-converter-0.2.2/src/ldc/tool/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     8605 2024-02-23 01:25:19.000000 llm-dataset-converter-0.2.2/src/ldc/tool/append.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7292 2024-02-21 21:28:28.000000 llm-dataset-converter-0.2.2/src/ldc/tool/convert.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3280 2024-02-20 02:25:09.000000 llm-dataset-converter-0.2.2/src/ldc/tool/download.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3783 2024-02-20 02:26:04.000000 llm-dataset-converter-0.2.2/src/ldc/tool/file_encoding.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7104 2024-02-04 23:37:50.000000 llm-dataset-converter-0.2.2/src/ldc/tool/find.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     7313 2024-05-01 05:12:36.000000 llm-dataset-converter-0.2.2/src/ldc/tool/help.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     5520 2024-02-05 00:23:10.000000 llm-dataset-converter-0.2.2/src/ldc/tool/paste.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.192317 llm-dataset-converter-0.2.2/src/ldc/translation/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      416 2024-02-20 01:27:00.000000 llm-dataset-converter-0.2.2/src/ldc/translation/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    24398 2024-03-13 03:16:06.000000 llm-dataset-converter-0.2.2/src/ldc/translation/_csv.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    11807 2024-03-13 03:22:55.000000 llm-dataset-converter-0.2.2/src/ldc/translation/_jsonlines.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3908 2024-02-20 01:45:23.000000 llm-dataset-converter-0.2.2/src/ldc/translation/_language.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    10982 2024-03-13 03:22:55.000000 llm-dataset-converter-0.2.2/src/ldc/translation/_parquet.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3203 2024-02-20 01:44:40.000000 llm-dataset-converter-0.2.2/src/ldc/translation/_require_languages.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)    16901 2024-03-13 03:16:06.000000 llm-dataset-converter-0.2.2/src/ldc/translation/_txt.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      931 2024-02-04 22:44:57.000000 llm-dataset-converter-0.2.2/src/ldc/utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2024-05-03 02:53:27.192317 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     9602 2024-05-03 02:53:27.000000 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3087 2024-05-03 02:53:27.000000 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2024-05-03 02:53:27.000000 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      371 2024-05-03 02:53:27.000000 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       88 2024-05-03 02:53:27.000000 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2024-05-03 02:53:27.000000 llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/top_level.txt
```

### Comparing `llm-dataset-converter-0.2.1/CHANGES.rst` & `llm-dataset-converter-0.2.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Changelog
 =========
 
+0.2.2 (2024-05-03)
+------------------
+
+- requiring seppl>=0.2.3 now
+
+
 0.2.1 (2024-05-02)
 ------------------
 
 - filters `split` and `tee` now support `ClassificationData` as well
 - added `metadata-from-name` filter to extract meta-data from the current input file name
-- requiring seppl>=0.1.3 now
 - added `inspect` filter that allows inspecting data interactively as it passes through the pipeline
 - added `empty_str_if_none` helper method to `ldc.text_utils` to ensure no None/null values are output with writers
 - upgraded seppl to 0.2.2 and switched to using `seppl.ClassListerRegistry`
 
 
 0.2.0 (2024-02-27)
 ------------------
```

### Comparing `llm-dataset-converter-0.2.1/DESCRIPTION.rst` & `llm-dataset-converter-0.2.2/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/PKG-INFO` & `llm-dataset-converter-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: llm-dataset-converter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python3 library for converting between various LLM dataset formats.
 Home-page: https://github.com/waikato-llm/llm-dataset-converter
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: The **llm-dataset-converter** allows the conversion between
         various dataset formats for large language models (LLMs).
@@ -63,20 +63,25 @@
                 --output alpaca_data_cleaned-filtered.json
         
         
         
         Changelog
         =========
         
+        0.2.2 (2024-05-03)
+        ------------------
+        
+        - requiring seppl>=0.2.3 now
+        
+        
         0.2.1 (2024-05-02)
         ------------------
         
         - filters `split` and `tee` now support `ClassificationData` as well
         - added `metadata-from-name` filter to extract meta-data from the current input file name
-        - requiring seppl>=0.1.3 now
         - added `inspect` filter that allows inspecting data interactively as it passes through the pipeline
         - added `empty_str_if_none` helper method to `ldc.text_utils` to ensure no None/null values are output with writers
         - upgraded seppl to 0.2.2 and switched to using `seppl.ClassListerRegistry`
         
         
         0.2.0 (2024-02-27)
         ------------------
```

### Comparing `llm-dataset-converter-0.2.1/README.md` & `llm-dataset-converter-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/setup.py` & `llm-dataset-converter-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     install_requires=[
         "chardet",
         "pandas",
         "jsonlines",
         "pyarrow",
         "pyzstd",
         "huggingface-hub",
-        "seppl>=0.2.2",
+        "seppl>=0.2.3",
         "pyyaml",
         "wai.logging",
     ],
-    version="0.2.1",
+    version="0.2.2",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     entry_points={
         "console_scripts": [
             "llm-append=ldc.tool.append:sys_main",
             "llm-convert=ldc.tool.convert:sys_main",
             "llm-download=ldc.tool.download:sys_main",
```

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/_downloader.py` & `llm-dataset-converter-0.2.2/src/ldc/api/_downloader.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/_filter.py` & `llm-dataset-converter-0.2.2/src/ldc/api/_filter.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/_io.py` & `llm-dataset-converter-0.2.2/src/ldc/api/_io.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/pretrain.py` & `llm-dataset-converter-0.2.2/src/ldc/api/pretrain.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/supervised/classification.py` & `llm-dataset-converter-0.2.2/src/ldc/api/supervised/classification.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/supervised/pairs.py` & `llm-dataset-converter-0.2.2/src/ldc/api/supervised/pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/api/translation.py` & `llm-dataset-converter-0.2.2/src/ldc/api/translation.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/class_lister.py` & `llm-dataset-converter-0.2.2/src/ldc/class_lister.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/core.py` & `llm-dataset-converter-0.2.2/src/ldc/core.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/downloader/_huggingface.py` & `llm-dataset-converter-0.2.2/src/ldc/downloader/_huggingface.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/__init__.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_assemble_sentences.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_assemble_sentences.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_change_case.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_change_case.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_file_filter.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_file_filter.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_find_substr.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_find_substr.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_inspect.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_inspect.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_keyword.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_keyword.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_llama2_to_pairs.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_llama2_to_pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_max_records.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_max_records.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_metadata.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_metadata.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_metadata_from_name.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_metadata_from_name.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_llama2.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_pairs_to_llama2.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_pairs_to_pretrain.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_pairs_to_pretrain.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_classification.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_pretrain_sentences_to_classification.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_pretrain_sentences_to_pairs.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_pretrain_sentences_to_pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_randomize_records.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_randomize_records.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_record_files.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_record_files.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_record_window.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_record_window.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_remove_blocks.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_remove_blocks.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_remove_empty.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_remove_empty.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_remove_patterns.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_remove_patterns.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_replace_patterns.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_replace_patterns.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_reset_ids.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_reset_ids.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_ids.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_skip_duplicate_ids.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_skip_duplicate_text.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_skip_duplicate_text.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_split.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_split.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_tee.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_tee.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_text_length.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_text_length.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_text_stats.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_text_stats.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_to_llama2_format.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_to_llama2_format.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pairs.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_translation_to_pairs.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/filter/_translation_to_pretrain.py` & `llm-dataset-converter-0.2.2/src/ldc/filter/_translation_to_pretrain.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/help.py` & `llm-dataset-converter-0.2.2/src/ldc/help.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_csv.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_csv.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_jsonlines.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_jsonlines.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_max_length.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_max_length.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_parquet.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_parquet.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_sentences.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_sentences.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_split.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_split.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/pretrain/_txt.py` & `llm-dataset-converter-0.2.2/src/ldc/pretrain/_txt.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/registry.py` & `llm-dataset-converter-0.2.2/src/ldc/registry.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_classification_label_map.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_classification_label_map.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_csv.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_csv.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_jsonlines.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_jsonlines.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/classification/_parquet.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/classification/_parquet.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_alpaca.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_alpaca.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_csv.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_csv.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_jsonlines.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_jsonlines.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_parquet.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_parquet.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_update_pair_data.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_update_pair_data.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/supervised/pairs/_xtuner.py` & `llm-dataset-converter-0.2.2/src/ldc/supervised/pairs/_xtuner.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/text_utils.py` & `llm-dataset-converter-0.2.2/src/ldc/text_utils.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/append.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/append.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/convert.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/convert.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/download.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/download.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/file_encoding.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/file_encoding.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/find.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/find.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/help.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/help.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/tool/paste.py` & `llm-dataset-converter-0.2.2/src/ldc/tool/paste.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/translation/_csv.py` & `llm-dataset-converter-0.2.2/src/ldc/translation/_csv.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/translation/_jsonlines.py` & `llm-dataset-converter-0.2.2/src/ldc/translation/_jsonlines.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/translation/_language.py` & `llm-dataset-converter-0.2.2/src/ldc/translation/_language.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/translation/_parquet.py` & `llm-dataset-converter-0.2.2/src/ldc/translation/_parquet.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/translation/_require_languages.py` & `llm-dataset-converter-0.2.2/src/ldc/translation/_require_languages.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/translation/_txt.py` & `llm-dataset-converter-0.2.2/src/ldc/translation/_txt.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/ldc/utils.py` & `llm-dataset-converter-0.2.2/src/ldc/utils.py`

 * *Files identical despite different names*

### Comparing `llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/PKG-INFO` & `llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: llm-dataset-converter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python3 library for converting between various LLM dataset formats.
 Home-page: https://github.com/waikato-llm/llm-dataset-converter
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: The **llm-dataset-converter** allows the conversion between
         various dataset formats for large language models (LLMs).
@@ -63,20 +63,25 @@
                 --output alpaca_data_cleaned-filtered.json
         
         
         
         Changelog
         =========
         
+        0.2.2 (2024-05-03)
+        ------------------
+        
+        - requiring seppl>=0.2.3 now
+        
+        
         0.2.1 (2024-05-02)
         ------------------
         
         - filters `split` and `tee` now support `ClassificationData` as well
         - added `metadata-from-name` filter to extract meta-data from the current input file name
-        - requiring seppl>=0.1.3 now
         - added `inspect` filter that allows inspecting data interactively as it passes through the pipeline
         - added `empty_str_if_none` helper method to `ldc.text_utils` to ensure no None/null values are output with writers
         - upgraded seppl to 0.2.2 and switched to using `seppl.ClassListerRegistry`
         
         
         0.2.0 (2024-02-27)
         ------------------
```

### Comparing `llm-dataset-converter-0.2.1/src/llm_dataset_converter.egg-info/SOURCES.txt` & `llm-dataset-converter-0.2.2/src/llm_dataset_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

