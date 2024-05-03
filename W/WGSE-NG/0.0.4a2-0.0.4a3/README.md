# Comparing `tmp/wgse_ng-0.0.4a2.tar.gz` & `tmp/wgse_ng-0.0.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-0.0.4a2.tar", last modified: Fri May  3 18:02:17 2024, max compression
+gzip compressed data, was "wgse_ng-0.0.4a3.tar", last modified: Fri May  3 18:17:35 2024, max compression
```

## Comparing `wgse_ng-0.0.4a2.tar` & `wgse_ng-0.0.4a3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.766228 wgse_ng-0.0.4a2/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 18:02:17.766228 wgse_ng-0.0.4a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.766228 wgse_ng-0.0.4a2/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 18:02:17.000000 wgse_ng-0.0.4a2/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-03 18:02:17.000000 wgse_ng-0.0.4a2/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:02:17.000000 wgse_ng-0.0.4a2/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 18:02:17.000000 wgse_ng-0.0.4a2/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 18:02:17.000000 wgse_ng-0.0.4a2/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 18:02:17.000000 wgse_ng-0.0.4a2/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:02:17.766228 wgse_ng-0.0.4a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.758228 wgse_ng-0.0.4a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.758228 wgse_ng-0.0.4a2/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.758228 wgse_ng-0.0.4a2/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.762228 wgse_ng-0.0.4a2/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/chromosome_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/external.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.762228 wgse_ng-0.0.4a2/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.762228 wgse_ng-0.0.4a2/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/fastq/fastq_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/genome_file_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.762228 wgse_ng-0.0.4a2/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/alignment_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/header_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/index_statistics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.762228 wgse_ng-0.0.4a2/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/microarray/raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/prerequisites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.766228 wgse_ng-0.0.4a2/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/reference_genome/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/reference_genome/metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:02:17.766228 wgse_ng-0.0.4a2/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-03 18:02:13.000000 wgse_ng-0.0.4a2/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.013472 wgse_ng-0.0.4a3/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 18:17:35.013472 wgse_ng-0.0.4a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.013472 wgse_ng-0.0.4a3/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 18:17:34.000000 wgse_ng-0.0.4a3/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-03 18:17:34.000000 wgse_ng-0.0.4a3/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:17:34.000000 wgse_ng-0.0.4a3/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 18:17:34.000000 wgse_ng-0.0.4a3/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 18:17:34.000000 wgse_ng-0.0.4a3/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 18:17:34.000000 wgse_ng-0.0.4a3/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:17:35.013472 wgse_ng-0.0.4a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.001473 wgse_ng-0.0.4a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.005473 wgse_ng-0.0.4a3/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.005473 wgse_ng-0.0.4a3/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.005473 wgse_ng-0.0.4a3/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/chromosome_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/external.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.009472 wgse_ng-0.0.4a3/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.009472 wgse_ng-0.0.4a3/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/fastq/fastq_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/genome_file_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.009472 wgse_ng-0.0.4a3/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/alignment_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/header_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/index_statistics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.009472 wgse_ng-0.0.4a3/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/microarray/raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/prerequisites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.009472 wgse_ng-0.0.4a3/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/reference_genome/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/reference_genome/metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:17:35.009472 wgse_ng-0.0.4a3/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-03 18:17:25.000000 wgse_ng-0.0.4a3/wgse/variant_caller.py
```

### Comparing `wgse_ng-0.0.4a2/PKG-INFO` & `wgse_ng-0.0.4a3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a2
+Version: 0.0.4a3
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `wgse_ng-0.0.4a2/README.md` & `wgse_ng-0.0.4a3/README.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-0.0.4a3/WGSE_NG.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 0.0.4a2
+Version: 0.0.4a3
 Summary: Whole Genome Sequencing data manipulation tool
 Home-page: https://github.com/chaplin89/WGSE-NG
 Author: Multiple
 Author-email: 
 Keywords: bioinformatics
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `wgse_ng-0.0.4a2/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-0.0.4a3/WGSE_NG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/setup.py` & `wgse_ng-0.0.4a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 DEPENDENCIES = ["setuptools"]
 
-VERSION = "0.0.4-alpha2"
+VERSION = "0.0.4-alpha3"
 DOC = ""
 
 setup(
     name="WGSE-NG",
     packages=[
         "wgse",
         "wgse.alignment_map",
@@ -19,15 +19,15 @@
         "wgse.utility",
     ],
     author="Multiple",
     author_email="",
     description="Whole Genome Sequencing data manipulation tool",
     long_description="Whole Genome Sequencing data manipulation tool",
     install_requires=DEPENDENCIES,
-    entry_points={"gui_scripts": ["wgse = wgse.gui"]},
+    entry_points={"gui_scripts": ["wgse = wgse:gui"]},
     url="https://github.com/chaplin89/WGSE-NG",
     version=VERSION,
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
```

### Comparing `wgse_ng-0.0.4a2/test/test_buckets.py` & `wgse_ng-0.0.4a3/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/test/test_fasta.py` & `wgse_ng-0.0.4a3/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/test/test_fasta_dictionary.py` & `wgse_ng-0.0.4a3/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/test/test_sequence.py` & `wgse_ng-0.0.4a3/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/test/test_unknown_bases_stats.py` & `wgse_ng-0.0.4a3/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-0.0.4a3/wgse/alignment_map/alignment_map_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-0.0.4a3/wgse/alignment_map/alignment_map_header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-0.0.4a3/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-0.0.4a3/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-0.0.4a3/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-0.0.4a3/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/configuration.py` & `wgse_ng-0.0.4a3/wgse/configuration.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/data/alignment_map_file_info.py` & `wgse_ng-0.0.4a3/wgse/data/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/data/alignment_stats.py` & `wgse_ng-0.0.4a3/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/data/microarray_converter.py` & `wgse_ng-0.0.4a3/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/data/reference.py` & `wgse_ng-0.0.4a3/wgse/data/reference.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/external.py` & `wgse_ng-0.0.4a3/wgse/external.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-0.0.4a3/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/fasta/fasta_stats_files.py` & `wgse_ng-0.0.4a3/wgse/fasta/fasta_stats_files.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/fasta/letter_run_buckets.py` & `wgse_ng-0.0.4a3/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/fasta/letter_run_collection.py` & `wgse_ng-0.0.4a3/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/fasta/reference.py` & `wgse_ng-0.0.4a3/wgse/fasta/reference.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/fastq/fastq_file.py` & `wgse_ng-0.0.4a3/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/genome_file_finder.py` & `wgse_ng-0.0.4a3/wgse/genome_file_finder.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/alignment_statistics_dialog.py` & `wgse_ng-0.0.4a3/wgse/gui/alignment_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/header.py` & `wgse_ng-0.0.4a3/wgse/gui/header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/header_dialog.py` & `wgse_ng-0.0.4a3/wgse/gui/header_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/index_statistics_dialog.py` & `wgse_ng-0.0.4a3/wgse/gui/index_statistics_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/main.py` & `wgse_ng-0.0.4a3/wgse/gui/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/table_dialog.py` & `wgse_ng-0.0.4a3/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/gui/ui_form.py` & `wgse_ng-0.0.4a3/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/microarray/microarray_converter.py` & `wgse_ng-0.0.4a3/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-0.0.4a3/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/microarray/raw_file.py` & `wgse_ng-0.0.4a3/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/reference_genome/decompressor.py` & `wgse_ng-0.0.4a3/wgse/reference_genome/decompressor.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/reference_genome/downloader.py` & `wgse_ng-0.0.4a3/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/reference_genome/finder.py` & `wgse_ng-0.0.4a3/wgse/reference_genome/finder.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/reference_genome/metadata_loader.py` & `wgse_ng-0.0.4a3/wgse/reference_genome/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/reference_genome/repository_manager.py` & `wgse_ng-0.0.4a3/wgse/reference_genome/repository_manager.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/utility/file_type_checker.py` & `wgse_ng-0.0.4a3/wgse/utility/file_type_checker.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/utility/sequence_orderer.py` & `wgse_ng-0.0.4a3/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/utility/sequencers.py` & `wgse_ng-0.0.4a3/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-0.0.4a2/wgse/variant_caller.py` & `wgse_ng-0.0.4a3/wgse/variant_caller.py`

 * *Files identical despite different names*

