# Comparing `tmp/nanomotif-0.2.1.tar.gz` & `tmp/nanomotif-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.2.1.tar", last modified: Tue Apr 16 09:18:22 2024, max compression
+gzip compressed data, was "nanomotif-0.3.0.tar", last modified: Fri May  3 10:18:33 2024, max compression
```

## Comparing `nanomotif-0.2.1.tar` & `nanomotif-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.096362 nanomotif-0.2.1/
--rw-rw-r--   0 shei      (1000) shei      (1000)     1084 2023-11-30 15:56:56.000000 nanomotif-0.2.1/LICENSE
--rw-r--r--   0 shei      (1000) shei      (1000)    18166 2024-04-16 09:18:22.096362 nanomotif-0.2.1/PKG-INFO
--rw-rw-r--   0 shei      (1000) shei      (1000)    17643 2024-04-16 09:16:26.000000 nanomotif-0.2.1/README.md
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.048362 nanomotif-0.2.1/nanomotif/
--rw-rw-r--   0 shei      (1000) shei      (1000)      278 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)       22 2024-04-16 09:16:45.000000 nanomotif-0.2.1/nanomotif/_version.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     8496 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/argparser.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6009 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/bin_consensus.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.052362 nanomotif-0.2.1/nanomotif/binnary/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    13167 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/analysis.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    15629 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/data_processing.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3729 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/detect_contamination.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3014 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/include_contigs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      890 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/logging.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     9127 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/binnary/scoring.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      522 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/binnary/utils.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    14165 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/candidate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1061 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/constants.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1698 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/dataload.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.052362 nanomotif-0.2.1/nanomotif/datasets/
--rw-rw-r--   0 shei      (1000) shei      (1000)       27 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-rw-r--   0 shei      (1000) shei      (1000)   176247 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-rw-r--   0 shei      (1000) shei      (1000) 26479844 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-rw-r--   0 shei      (1000) shei      (1000)     1106 2024-03-29 17:14:10.000000 nanomotif-0.2.1/nanomotif/datasets.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    28677 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/evaluate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      539 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/feature.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      321 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/logger.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    18855 2024-04-16 09:16:26.000000 nanomotif-0.2.1/nanomotif/main.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1037 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/model.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     5639 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/old_search_method.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      850 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/parallel.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6202 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/postprocess.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7193 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/scoremotifs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      197 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/seed.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    20090 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/seq.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2677 2024-03-29 12:58:11.000000 nanomotif-0.2.1/nanomotif/utils.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.092362 nanomotif-0.2.1/nanomotif.egg-info/
--rw-r--r--   0 shei      (1000) shei      (1000)    18166 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/PKG-INFO
--rw-rw-r--   0 shei      (1000) shei      (1000)     1606 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/SOURCES.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)        1 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/dependency_links.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       50 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/entry_points.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)        1 2023-11-30 15:56:57.000000 nanomotif-0.2.1/nanomotif.egg-info/not-zip-safe
--rw-rw-r--   0 shei      (1000) shei      (1000)      132 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/requires.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       16 2024-04-16 09:18:22.000000 nanomotif-0.2.1/nanomotif.egg-info/top_level.txt
--rw-rw-r--   0 shei      (1000) shei      (1000)       38 2024-04-16 09:18:22.096362 nanomotif-0.2.1/setup.cfg
--rw-rw-r--   0 shei      (1000) shei      (1000)      918 2024-03-29 17:14:10.000000 nanomotif-0.2.1/setup.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.092362 nanomotif-0.2.1/tests/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2023-11-30 15:56:56.000000 nanomotif-0.2.1/tests/__init__.py
-drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-04-16 09:18:22.092362 nanomotif-0.2.1/tests/binnary/
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/__init__.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2089 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/conftest.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1019 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_arg_parser.py
--rw-rw-r--   0 shei      (1000) shei      (1000)    11132 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/test_cli_commands.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     6352 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_data_processing_functions.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2585 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_detect_contamination.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1404 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_generate_output.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2132 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_include_contigs.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     3317 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/test_scoring.py
--rw-rw-r--   0 shei      (1000) shei      (1000)      744 2024-03-29 17:14:10.000000 nanomotif-0.2.1/tests/binnary/test_utils.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     5405 2024-04-16 09:16:26.000000 nanomotif-0.2.1/tests/binnary/test_write_bins.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     7236 2023-11-30 15:56:57.000000 nanomotif-0.2.1/tests/test_candidate.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     1365 2024-03-29 11:56:23.000000 nanomotif-0.2.1/tests/test_dataload.py
--rw-rw-r--   0 shei      (1000) shei      (1000)     2933 2024-03-29 11:56:23.000000 nanomotif-0.2.1/tests/test_motif_find.py
--rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 11:56:23.000000 nanomotif-0.2.1/tests/test_motif_score.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.492056 nanomotif-0.3.0/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1084 2023-09-06 10:54:37.000000 nanomotif-0.3.0/LICENSE
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7350 2024-05-03 10:18:33.492056 nanomotif-0.3.0/PKG-INFO
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6794 2024-05-03 10:10:14.000000 nanomotif-0.3.0/README.md
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:32.380055 nanomotif-0.3.0/nanomotif/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      278 2024-01-23 08:11:50.000000 nanomotif-0.3.0/nanomotif/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       22 2024-05-03 10:10:32.000000 nanomotif-0.3.0/nanomotif/_version.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11018 2024-05-03 08:31:51.000000 nanomotif-0.3.0/nanomotif/argparser.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6016 2024-02-20 08:34:47.000000 nanomotif-0.3.0/nanomotif/bin_consensus.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:32.752055 nanomotif-0.3.0/nanomotif/binnary/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    13167 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/analysis.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    15629 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/data_processing.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3729 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/detect_contamination.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3014 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/include_contigs.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      890 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/logging.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     9127 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/binnary/scoring.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      522 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/binnary/utils.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    14165 2024-02-07 10:11:10.000000 nanomotif-0.3.0/nanomotif/candidate.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1078 2024-05-03 08:31:51.000000 nanomotif-0.3.0/nanomotif/constants.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1698 2023-11-17 10:28:11.000000 nanomotif-0.3.0/nanomotif/dataload.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:32.792055 nanomotif-0.3.0/nanomotif/datasets/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       27 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)   176247 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164) 26479844 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1106 2024-03-29 17:11:23.000000 nanomotif-0.3.0/nanomotif/datasets.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    28603 2024-05-03 08:31:52.000000 nanomotif-0.3.0/nanomotif/evaluate.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      539 2023-10-03 09:15:12.000000 nanomotif-0.3.0/nanomotif/feature.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      321 2023-11-19 13:30:13.000000 nanomotif-0.3.0/nanomotif/logger.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    19829 2024-05-03 08:31:52.000000 nanomotif-0.3.0/nanomotif/main.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1037 2024-02-19 12:26:57.000000 nanomotif-0.3.0/nanomotif/model.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.168056 nanomotif-0.3.0/nanomotif/mtase_linker/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       47 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/mtase_linker/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5051 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/mtase_linker/command.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3615 2024-05-03 08:31:42.000000 nanomotif-0.3.0/nanomotif/mtase_linker/dependencies.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5639 2023-10-16 10:50:49.000000 nanomotif-0.3.0/nanomotif/old_search_method.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      850 2024-01-23 09:46:13.000000 nanomotif-0.3.0/nanomotif/parallel.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6202 2024-02-07 10:11:10.000000 nanomotif-0.3.0/nanomotif/postprocess.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7193 2024-01-23 11:48:10.000000 nanomotif-0.3.0/nanomotif/scoremotifs.py
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      197 2024-01-23 07:18:32.000000 nanomotif-0.3.0/nanomotif/seed.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    20090 2024-02-19 12:26:57.000000 nanomotif-0.3.0/nanomotif/seq.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2677 2024-02-26 13:37:04.000000 nanomotif-0.3.0/nanomotif/utils.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.488056 nanomotif-0.3.0/nanomotif.egg-info/
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7350 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/PKG-INFO
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1714 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/SOURCES.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/dependency_links.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       50 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/entry_points.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2023-09-07 09:00:46.000000 nanomotif-0.3.0/nanomotif.egg-info/not-zip-safe
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      150 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/requires.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       16 2024-05-03 10:18:32.000000 nanomotif-0.3.0/nanomotif.egg-info/top_level.txt
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       38 2024-05-03 10:18:33.492056 nanomotif-0.3.0/setup.cfg
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      947 2024-05-03 08:31:42.000000 nanomotif-0.3.0/setup.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.252056 nanomotif-0.3.0/tests/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2023-10-17 07:22:50.000000 nanomotif-0.3.0/tests/__init__.py
+drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-03 10:18:33.456056 nanomotif-0.3.0/tests/binnary/
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/__init__.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2089 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/conftest.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1019 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_arg_parser.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11132 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/test_cli_commands.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6352 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_data_processing_functions.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2585 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_detect_contamination.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1404 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_generate_output.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2132 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_include_contigs.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3317 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/test_scoring.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      744 2024-03-29 17:11:23.000000 nanomotif-0.3.0/tests/binnary/test_utils.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5405 2024-05-03 08:31:42.000000 nanomotif-0.3.0/tests/binnary/test_write_bins.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7236 2023-11-17 09:23:51.000000 nanomotif-0.3.0/tests/test_candidate.py
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1365 2024-01-23 08:24:14.000000 nanomotif-0.3.0/tests/test_dataload.py
+-rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2933 2024-01-23 09:52:43.000000 nanomotif-0.3.0/tests/test_motif_find.py
+-rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-02 08:30:14.000000 nanomotif-0.3.0/tests/test_motif_score.py
```

### Comparing `nanomotif-0.2.1/LICENSE` & `nanomotif-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/argparser.py` & `nanomotif-0.3.0/nanomotif/argparser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 from nanomotif._version import __version__
+import os
 
 
 def  create_parser():
     parser = argparse.ArgumentParser(description="Motif identification and utilisation commands")
     parser.add_argument("--version", action="version", version="%(prog)s {}".format(__version__))
     subparsers = parser.add_subparsers(help="Command descriptions", dest="command")
 
@@ -23,45 +24,44 @@
     ###########################################################################
     # Find Motifs
     parser_shared_find_motifs = argparse.ArgumentParser(add_help=False)
     parser_shared_find_motifs.add_argument("--search_frame_size", type=int, default=40, help="length of the sequnces sampled around confident methylatyion sites. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--threshold_methylation_confident", type=float, default=0.80, help="minimum fraction of reads that must be methylated at a position for the position to be considered confiently methylated. These position are used to search for candidate motifs. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--threshold_valid_coverage", type=int, default=5, help="minimum valid base coverage for a position to be considered. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--minimum_kl_divergence", type=float, default=0.05, help="minimum KL-divergence for a position to considered for expansion in  motif search. Higher value means less exhaustive, but faster search. Default: %(default)s")
-    parser_find_motifs = subparsers.add_parser(
-        'find-motifs', 
-        parents=[parser_positional, parser_optional, parser_shared_find_motifs], 
-        help="identifies motifs in contigs"
-    )
+    #parser_find_motifs = subparsers.add_parser(
+    #    'find-motifs', 
+    #    parents=[parser_positional, parser_optional, parser_shared_find_motifs], 
+    #    help="identifies motifs in contigs"
+    #)
 
     ###########################################################################
     # Score motifs
-    parser_score_motifs = subparsers.add_parser(
-        'score-motifs', 
-        parents=[parser_positional, parser_optional],
-        help="generate feature complete output"
-    )
-    parser_score_motifs.add_argument("motifs", type=str, help="path to the motifs file.")
+    #parser_score_motifs = subparsers.add_parser(
+    #    'score-motifs', 
+    #    parents=[parser_positional, parser_optional],
+    #    help="generate feature complete output"
+    #)
+    #parser_score_motifs.add_argument("motifs", type=str, help="path to the motifs file.")
     
     ###########################################################################
     # Bin consensus
     parser_shared_bin_consensus = argparse.ArgumentParser(add_help=False, conflict_handler="resolve")
     parser_shared_bin_consensus.add_argument("bins", type=str, help="tsv file specifying which bin contigs belong.")
-
-    parser_bin_consensus = subparsers.add_parser(
-        'bin-consensus', 
-        parents=[parser_positional, parser_optional, parser_shared_bin_consensus],
-        help="generate consensus set of motif for each bin"
-    )
-    parser_bin_consensus.add_argument("motifs", type=str, help="path to the motifs file.")
-    parser_bin_consensus.add_argument("motifs_scored", metavar="motifs-scored", type=str, help="path to the motif-scored file.")
+    #parser_bin_consensus = subparsers.add_parser(
+    #    'bin-consensus', 
+    #    parents=[parser_positional, parser_optional, parser_shared_bin_consensus],
+    #    help="generate consensus set of motif for each bin"
+    #)
+    #parser_bin_consensus.add_argument("motifs", type=str, help="path to the motifs file.")
+    #parser_bin_consensus.add_argument("motifs_scored", metavar="motifs-scored", type=str, help="path to the motif-scored file.")
 
     ###########################################################################
     # Complete workflow
-    parser_complete_workflow = subparsers.add_parser('complete-workflow', help='run find-motifs, score-motifs and bin-consensus', parents=[parser_positional, parser_optional, parser_shared_find_motifs, parser_shared_bin_consensus], conflict_handler="resolve")
+    parser_complete_workflow = subparsers.add_parser('find_motifs', help='Identify methylated motifs on and contig and bin level', parents=[parser_positional, parser_optional, parser_shared_find_motifs, parser_shared_bin_consensus], conflict_handler="resolve")
 
     ###########################################################################
     # Check installation
     parser_check_installation = subparsers.add_parser('check-installation', parents=[parser_optional, parser_shared_find_motifs], add_help=False)
     
     
     ###########################################################################
@@ -153,10 +153,42 @@
     parser_inclusion.add_argument(
         "--min_motif_comparisons",
         type=int,
         default=5,
         help="Minimum number of non-NA motif comparisons required to include a contig in the analysis. Default is 5",
     )
     
+    ###########################################################################
+    # MTase-linker
+    parser_mtase_linker = subparsers.add_parser(
+        'MTase-linker', 
+        help="Commands related to MTase-linker"
+    )
+
+    mtase_linker_subparsers = parser_mtase_linker.add_subparsers(
+        title="MTase-linker commands", 
+        dest="mtase_linker_command"
+    )
+
+    parser_mtase_linker_run = mtase_linker_subparsers.add_parser(
+        'run', 
+        help="Run the MTase-linker workflow"
+    )
+    parser_mtase_linker_run.add_argument("-t", "--threads", type=int, default=1, help="Number of threads to use. Default is 1")
+    parser_mtase_linker_run.add_argument("--forceall", type=bool, default=False, help="Forcerun workflow regardless of already created output (default = False)")
+    parser_mtase_linker_run.add_argument("--dryrun", type=bool, default=False, help="Dry-run the workflow. Default is False")
+    parser_mtase_linker_run.add_argument("--binsdir", type=str, required=True, help="Directory with bin files or assembly files. Needs to have the .fa extension.")
+    parser_mtase_linker_run.add_argument("--contig_bin", type=str, required=True, help="tsv file specifying which bin contigs belong.")
+    parser_mtase_linker_run.add_argument("--bin_motifs", type=str, required=True, help="bin-motifs.tsv output from nanomotif.")
+    parser_mtase_linker_run.add_argument("-d", "--dependency_dir", type=str, default=os.path.join(os.getcwd(), "ML_dependencies"), help="Same as for installation. Path to directory of the ML_dependencies directory created during installation of the MTase-linker module. Default is cwd/ML_dependencies")
+    parser_mtase_linker_run.add_argument("-o", "--outputdir", type=str, default=os.path.join(os.getcwd(), "mtase_linker"), help="Output directory. Default is cwd")
+    parser_mtase_linker_run.add_argument("--identity", type=str, default=80, help="Identity threshold for motif prediction. Default is 80")
+    parser_mtase_linker_run.add_argument("--qcovs", type=str, default=80, help="Query coverage for motif prediction. Default is 80")
+
+    parser_mtase_linker_install = mtase_linker_subparsers.add_parser(
+        'install', 
+        help="Install additional dependencies for MTase-linker"
+    )
+    parser_mtase_linker_install.add_argument("-d", "--dependency_dir", type=str, default=os.getcwd(), help="Path to the directory, where dependencies should be installed. A folder named ML_dependencies will be generated. Default is cwd.")
     
     return parser
```

### Comparing `nanomotif-0.2.1/nanomotif/bin_consensus.py` & `nanomotif-0.3.0/nanomotif/bin_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     result = methylated_contig_mass.join(all_contig_mass, on=["bin", "motif", "mod_type", "mod_position"]) \
         .with_columns(
             (pl.col("n_motif_meth_contigs") / pl.col("n_motif_contigs")).alias("methylated_proportion")
         )
     motifs_scored_filt = motifs_scored.join(result, on=["bin", "motif", "mod_type", "mod_position"]).filter(pl.col("methylated_proportion") > minimum_bin_methylation)
 
     
-    log.debug("Removing submotifs")
+    #log.debug("Removing submotifs")
     # Remove submotifs
-    contig_motifs = nm.postprocess.remove_sub_motifs(motifs_scored_filt)
+    #contig_motifs = nm.postprocess.remove_sub_motifs(motifs_scored_filt)
 
-    contig_motifs = contig_motifs.with_columns(
+    contig_motifs = motifs_scored_filt.with_columns(
             pl.col("motif").apply(lambda x: nm.seq.regex_to_iupac(x)).alias("motif"),
             (pl.col("n_mod")  / (pl.col("n_mod") + pl.col("n_nomod"))).alias("mean")
         )
     bin_motifs = contig_motifs.groupby("bin", "motif", "mod_position", "mod_type") \
         .agg(
             pl.col("n_mod").sum().alias("n_mod_bin"),
             pl.col("n_nomod").sum().alias("n_nomod_bin"),
```

### Comparing `nanomotif-0.2.1/nanomotif/binnary/analysis.py` & `nanomotif-0.3.0/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/binnary/data_processing.py` & `nanomotif-0.3.0/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.3.0/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/binnary/include_contigs.py` & `nanomotif-0.3.0/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/binnary/logging.py` & `nanomotif-0.3.0/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/binnary/scoring.py` & `nanomotif-0.3.0/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/binnary/utils.py` & `nanomotif-0.3.0/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/candidate.py` & `nanomotif-0.3.0/nanomotif/candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/constants.py` & `nanomotif-0.3.0/nanomotif/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,10 @@
     "N": [1, 1, 1, 1],
     ".": [1, 1, 1, 1]
 }
 BASE_TO_INT = {"A":1, "T":2, "G":3, "C":4, "N":5, "R":6, "Y":7, "S":8, "W":9, "K":10, "M":11, "B":12, "D":13, "H":14, "V":15}
 INT_TO_BASE = {i: n for n, i in BASE_TO_INT.items()}
 MOD_TYPE_TO_CANONICAL = {
     "m":"C",
-    "a":"A"
+    "a":"A",
+    "21839":"C"
 }
```

### Comparing `nanomotif-0.2.1/nanomotif/dataload.py` & `nanomotif-0.3.0/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.3.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/datasets.py` & `nanomotif-0.3.0/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/evaluate.py` & `nanomotif-0.3.0/nanomotif/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     - contig_meth_positions (list): The positions of the methylation sites in the contig.
 
     Returns:
     - tuple: A tuple of two numpy arrays, the first containing the positions of the methylated motifs, the second containing the positions of the non-methylated motifs.
     """
     assert len(motif) > 0, "Motif is empty"
     assert len(sequence) > 0, "Sequence is empty"
-    assert len(methylated_positions) > 0, "Methylated positions is empty"
     assert type(motif) == Motif, "Motif is not a Motif type"
     # Get the index of the methylation in the motif in the contig
     motif_index = subseq_indices(motif.string, sequence) + motif.mod_position
 
     # Methylated motif positions
     meth_occurences = np.intersect1d(methylated_positions, motif_index)
```

### Comparing `nanomotif-0.2.1/nanomotif/feature.py` & `nanomotif-0.3.0/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/main.py` & `nanomotif-0.3.0/nanomotif/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,52 +119,67 @@
         df = format_motif_df(df)
         df = df.sort(["contig", "mod_type", "motif"])
         df.write_csv(args.out + "/" + name + ".tsv", separator="\t")
     os.makedirs(args.out + "/precleanup-motifs/", exist_ok=True)
     save_motif_df(motifs, "precleanup-motifs/motifs-raw")
 
     log.info("Postprocessing motifs")
+    motifs_file_name = "precleanup-motifs/motifs"
 
     log.info(" - Writing motifs")
     motifs = motifs.filter(pl.col("score") > 0.1)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
-    save_motif_df(motifs, "precleanup-motifs/motifs-score")
+    
+    motifs_file_name = motifs_file_name + "-score"
+    save_motif_df(motifs, motifs_file_name)
 
-    log.info(" - Removing sub motifs")
-    motifs = nm.postprocess.remove_sub_motifs(motifs)
-    if len(motifs) == 0:
-        log.info("No motifs found")
-        return
-    save_motif_df(motifs, "precleanup-motifs/motifs-score-sub")
+    #log.info(" - Removing sub motifs")
+    #motifs = nm.postprocess.remove_sub_motifs(motifs)
+    #if len(motifs) == 0:
+    #    log.info("No motifs found")
+    #    return
+    #motifs_file_name = motifs_file_name +   "-sub"
+    #save_motif_df(motifs, motifs_file_name)
 
     log.info(" - Removing noisy motifs")
     motifs = nm.postprocess.remove_noisy_motifs(motifs)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
-    save_motif_df(motifs, "precleanup-motifs/motifs-score-sub-noise")
+    motifs_file_name = motifs_file_name +   "-noise"
+    save_motif_df(motifs, motifs_file_name)
 
     log.info(" - Merging motifs")
     motifs = nm.postprocess.merge_motifs_in_df(motifs, pileup, assembly)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
-    save_motif_df(motifs, "precleanup-motifs/motifs-score-sub-noise-merge")
+    motifs_file_name = motifs_file_name +   "-merge"
+    save_motif_df(motifs, motifs_file_name)
 
     log.info(" - Joining motif complements")
     motifs = nm.postprocess.join_motif_complements(motifs)
-    save_motif_df(motifs, "precleanup-motifs/motifs-score-sub-noise-merge-complement")
+    if len(motifs) == 0:
+        log.info("No motifs found")
+        return
+    motifs_file_name = motifs_file_name +   "-complement"
+    save_motif_df(motifs, motifs_file_name)
 
     log.info(" - Removing motifs observed less than min count")
-    motifs = motifs.filter(pl.col("n_mod") + pl.col("n_nomod") > 50)
+    motifs = motifs.filter(pl.col("n_mod") + pl.col("n_nomod") > 1)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
+    motifs_file_name = motifs_file_name +   "-mincount"
+    save_motif_df(motifs, motifs_file_name)
+
+
+
     save_motif_df(motifs, "motifs")
 
     log.info("Done finding motifs")
     return format_motif_df(motifs)
 
 def score_motifs(args, pileup = None, assembly = None, motifs = None):
     log.info("Starting nanomotif motif scorer")
@@ -441,23 +456,36 @@
         
         data_processing.write_bins_from_contigs(new_contig_bins, assembly, bin_dir)
     
     log.info(f"Analysis Completed. Results are saved to: {args.out}")
     print("Analysis Completed. Results are saved to:", args.out)
 
 
+from nanomotif.mtase_linker.dependencies import snakemake_create_environments, get_models, defensefinder_update
+from nanomotif.mtase_linker.command import run_MTase_linker
+
+def mtase_linker(args):
+    if args.mtase_linker_command == "install":
+        snakemake_create_environments(args)
+        get_models(args)
+        defensefinder_update(args)
+    elif args.mtase_linker_command == "run":
+        run_MTase_linker(args)
+    else:
+        print(f"Unknown MTase-linker command: {args.mtase_linker_command}")
+       
 
 
 
 def main():
     # Parse arguments
     parser = nm.argparser.create_parser()
     args = parser.parse_args()
     
-    if args.command in ["detect_contamination", "include_contigs"]:
+    if args.command in ["detect_contamination", "include_contigs", "MTase-linker"]:
         args.verbose = False
         args.seed = 1
     
     
     if args.command == "find-motifs":
         shared_setup(args, args.out)
         find_motifs(args)
@@ -474,12 +502,17 @@
         args.out = "nanomotif_install_check"
         shared_setup(args, args.out)
         check_install(args)
 
     elif args.command in ["detect_contamination", "include_contigs"]:
         shared_setup(args, args.out)
         binnary(args)
+
+    elif args.command == "MTase-linker":
+        mtase_linker(args)
+
+
     else:
         parser.print_help()
         exit()
 if __name__ == "__main__":
     main()
```

### Comparing `nanomotif-0.2.1/nanomotif/model.py` & `nanomotif-0.3.0/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/old_search_method.py` & `nanomotif-0.3.0/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/parallel.py` & `nanomotif-0.3.0/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/postprocess.py` & `nanomotif-0.3.0/nanomotif/postprocess.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/scoremotifs.py` & `nanomotif-0.3.0/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/seq.py` & `nanomotif-0.3.0/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif/utils.py` & `nanomotif-0.3.0/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.3.0/nanomotif.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 nanomotif/binnary/include_contigs.py
 nanomotif/binnary/logging.py
 nanomotif/binnary/scoring.py
 nanomotif/binnary/utils.py
 nanomotif/datasets/geobacillus-contig-bin.tsv
 nanomotif/datasets/geobacillus-plasmids.assembly.fasta
 nanomotif/datasets/geobacillus-plasmids.pileup.bed
+nanomotif/mtase_linker/__init__.py
+nanomotif/mtase_linker/command.py
+nanomotif/mtase_linker/dependencies.py
 tests/__init__.py
 tests/test_candidate.py
 tests/test_dataload.py
 tests/test_motif_find.py
 tests/test_motif_score.py
 tests/binnary/__init__.py
 tests/binnary/conftest.py
```

### Comparing `nanomotif-0.2.1/setup.py` & `nanomotif-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         "numpy>=1.24.4",
         "pandas>=2.0.2",
         "polars>=0.19",
         "scipy>=1.10.1",
         "networkx>=3.1",
         "pyarrow>=15.0.2",
         "Bio>=1.6.2",
+        "snakemake>=7.32.4",
         "progressbar2>=3.53.1"
     ],
     entry_points={
             'console_scripts': [
                   'nanomotif = nanomotif.main:main'
             ]
     }
```

### Comparing `nanomotif-0.2.1/tests/binnary/conftest.py` & `nanomotif-0.3.0/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_arg_parser.py` & `nanomotif-0.3.0/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_cli_commands.py` & `nanomotif-0.3.0/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.3.0/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_detect_contamination.py` & `nanomotif-0.3.0/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_generate_output.py` & `nanomotif-0.3.0/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_include_contigs.py` & `nanomotif-0.3.0/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_scoring.py` & `nanomotif-0.3.0/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_utils.py` & `nanomotif-0.3.0/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/binnary/test_write_bins.py` & `nanomotif-0.3.0/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/test_candidate.py` & `nanomotif-0.3.0/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/test_dataload.py` & `nanomotif-0.3.0/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.2.1/tests/test_motif_find.py` & `nanomotif-0.3.0/tests/test_motif_find.py`

 * *Files identical despite different names*

