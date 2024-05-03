# Comparing `tmp/phykit-1.8.0.tar.gz` & `tmp/phykit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phykit-1.8.0.tar", last modified: Fri Dec 17 16:03:09 2021, max compression
+gzip compressed data, was "phykit-1.9.0.tar", last modified: Mon Dec 20 21:34:28 2021, max compression
```

## Comparing `phykit-1.8.0.tar` & `phykit-1.9.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.043257 phykit-1.8.0/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1078 2020-10-04 18:33:45.000000 phykit-1.8.0/LICENSE.md
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4765 2021-12-17 16:03:09.043017 phykit-1.8.0/PKG-INFO
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4102 2021-11-18 15:37:58.000000 phykit-1.8.0/README.md
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.017827 phykit-1.8.0/phykit/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/__init__.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      113 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/__main__.py
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.022333 phykit-1.8.0/phykit/helpers/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2020-10-04 20:56:18.000000 phykit-1.8.0/phykit/helpers/__init__.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      279 2021-01-24 15:29:30.000000 phykit-1.8.0/phykit/helpers/boolean_argument_parsing.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1375 2021-01-24 15:52:55.000000 phykit-1.8.0/phykit/helpers/files.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1768 2021-01-24 14:15:25.000000 phykit-1.8.0/phykit/helpers/stats_summary.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)    92938 2021-12-17 15:19:26.000000 phykit-1.8.0/phykit/phykit.py
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.022860 phykit-1.8.0/phykit/services/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/__init__.py
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.029423 phykit-1.8.0/phykit/services/alignment/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      609 2021-03-11 18:35:55.000000 phykit-1.8.0/phykit/services/alignment/__init__.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      437 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/alignment/alignment_length.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1329 2021-01-27 15:02:20.000000 phykit-1.8.0/phykit/services/alignment/alignment_length_no_gaps.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3156 2021-04-19 14:40:10.000000 phykit-1.8.0/phykit/services/alignment/base.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2254 2021-02-09 13:28:22.000000 phykit-1.8.0/phykit/services/alignment/column_score.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)    10013 2021-11-17 00:05:14.000000 phykit-1.8.0/phykit/services/alignment/create_concatenation_matrix.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4367 2021-10-17 16:16:42.000000 phykit-1.8.0/phykit/services/alignment/dna_threader.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      413 2021-03-11 18:38:44.000000 phykit-1.8.0/phykit/services/alignment/faidx.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2178 2021-01-24 14:18:24.000000 phykit-1.8.0/phykit/services/alignment/gc_content.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2152 2021-04-07 13:49:34.000000 phykit-1.8.0/phykit/services/alignment/pairwise_identity.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2284 2021-01-24 17:25:32.000000 phykit-1.8.0/phykit/services/alignment/parsimony_informative_sites.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      481 2021-01-24 17:34:06.000000 phykit-1.8.0/phykit/services/alignment/rcv.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2210 2021-10-17 16:26:29.000000 phykit-1.8.0/phykit/services/alignment/rename_fasta_entries.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2788 2021-02-09 03:21:31.000000 phykit-1.8.0/phykit/services/alignment/sum_of_pairs_score.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1286 2021-01-24 17:35:53.000000 phykit-1.8.0/phykit/services/alignment/variable_sites.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      191 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/base.py
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.042679 phykit-1.8.0/phykit/services/tree/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1213 2021-12-16 17:15:26.000000 phykit-1.8.0/phykit/services/tree/__init__.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4349 2021-12-16 22:22:50.000000 phykit-1.8.0/phykit/services/tree/base.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1305 2021-04-15 20:10:11.000000 phykit-1.8.0/phykit/services/tree/bipartition_support_stats.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1176 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/tree/branch_length_multiplier.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      785 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/tree/collapse_branches.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     7388 2021-09-07 14:27:59.000000 phykit-1.8.0/phykit/services/tree/covarying_evolutionary_rates.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3213 2021-01-24 17:55:51.000000 phykit-1.8.0/phykit/services/tree/dvmc.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      661 2021-09-29 22:27:20.000000 phykit-1.8.0/phykit/services/tree/evolutionary_rate.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3592 2021-12-17 01:09:58.000000 phykit-1.8.0/phykit/services/tree/hidden_paralogy_check.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2161 2021-01-24 18:11:58.000000 phykit-1.8.0/phykit/services/tree/internal_branch_stats.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      871 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/tree/internode_labeler.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1015 2021-08-27 11:27:31.000000 phykit-1.8.0/phykit/services/tree/last_common_ancestor_subtree.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3171 2021-04-19 14:22:43.000000 phykit-1.8.0/phykit/services/tree/lb_score.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     5319 2021-12-08 15:54:10.000000 phykit-1.8.0/phykit/services/tree/nearest_neighbor_interchange.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1879 2021-01-24 14:25:34.000000 phykit-1.8.0/phykit/services/tree/patristic_distances.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)    15164 2021-04-17 21:52:28.000000 phykit-1.8.0/phykit/services/tree/polytomy_test.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      748 2021-01-24 14:27:30.000000 phykit-1.8.0/phykit/services/tree/print_tree.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      880 2020-10-04 18:33:45.000000 phykit-1.8.0/phykit/services/tree/prune_tree.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1841 2021-10-25 20:19:50.000000 phykit-1.8.0/phykit/services/tree/rename_tree_tips.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3279 2021-09-07 14:36:25.000000 phykit-1.8.0/phykit/services/tree/rf_distance.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      899 2021-10-25 20:22:50.000000 phykit-1.8.0/phykit/services/tree/root_tree.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3830 2021-01-24 14:28:43.000000 phykit-1.8.0/phykit/services/tree/saturation.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2083 2021-01-27 14:57:51.000000 phykit-1.8.0/phykit/services/tree/spurious_sequence.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      458 2021-01-27 14:59:48.000000 phykit-1.8.0/phykit/services/tree/tip_labels.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1013 2021-12-06 13:48:29.000000 phykit-1.8.0/phykit/services/tree/tip_to_tip_distance.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      599 2021-01-27 14:59:51.000000 phykit-1.8.0/phykit/services/tree/total_tree_length.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      359 2021-01-27 14:54:53.000000 phykit-1.8.0/phykit/services/tree/treeness.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1376 2021-01-27 14:54:18.000000 phykit-1.8.0/phykit/services/tree/treeness_over_rcv.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       21 2021-12-17 01:19:31.000000 phykit-1.8.0/phykit/version.py
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-17 16:03:09.021063 phykit-1.8.0/phykit.egg-info/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4765 2021-12-17 16:03:08.000000 phykit-1.8.0/phykit.egg-info/PKG-INFO
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2265 2021-12-17 16:03:09.000000 phykit-1.8.0/phykit.egg-info/SOURCES.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        1 2021-12-17 16:03:08.000000 phykit-1.8.0/phykit.egg-info/dependency_links.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4758 2021-12-17 16:03:08.000000 phykit-1.8.0/phykit.egg-info/entry_points.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       50 2021-12-17 16:03:08.000000 phykit-1.8.0/phykit.egg-info/requires.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        7 2021-12-17 16:03:08.000000 phykit-1.8.0/phykit.egg-info/top_level.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       38 2021-12-17 16:03:09.043339 phykit-1.8.0/setup.cfg
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     7647 2021-12-17 01:24:21.000000 phykit-1.8.0/setup.py
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.839000 phykit-1.9.0/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1078 2020-10-04 18:33:45.000000 phykit-1.9.0/LICENSE.md
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4765 2021-12-20 21:34:28.838522 phykit-1.9.0/PKG-INFO
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4102 2021-11-18 15:37:58.000000 phykit-1.9.0/README.md
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.789834 phykit-1.9.0/phykit/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/__init__.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      113 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/__main__.py
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.797019 phykit-1.9.0/phykit/helpers/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2020-10-04 20:56:18.000000 phykit-1.9.0/phykit/helpers/__init__.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      279 2021-01-24 15:29:30.000000 phykit-1.9.0/phykit/helpers/boolean_argument_parsing.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1383 2021-12-19 15:00:56.000000 phykit-1.9.0/phykit/helpers/files.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1768 2021-01-24 14:15:25.000000 phykit-1.9.0/phykit/helpers/stats_summary.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)    95818 2021-12-19 15:46:42.000000 phykit-1.9.0/phykit/phykit.py
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.798056 phykit-1.9.0/phykit/services/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/__init__.py
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.810799 phykit-1.9.0/phykit/services/alignment/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      609 2021-03-11 18:35:55.000000 phykit-1.9.0/phykit/services/alignment/__init__.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      437 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/alignment/alignment_length.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1329 2021-01-27 15:02:20.000000 phykit-1.9.0/phykit/services/alignment/alignment_length_no_gaps.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3156 2021-04-19 14:40:10.000000 phykit-1.9.0/phykit/services/alignment/base.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2254 2021-02-09 13:28:22.000000 phykit-1.9.0/phykit/services/alignment/column_score.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)    10013 2021-11-17 00:05:14.000000 phykit-1.9.0/phykit/services/alignment/create_concatenation_matrix.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4367 2021-10-17 16:16:42.000000 phykit-1.9.0/phykit/services/alignment/dna_threader.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      413 2021-03-11 18:38:44.000000 phykit-1.9.0/phykit/services/alignment/faidx.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2178 2021-01-24 14:18:24.000000 phykit-1.9.0/phykit/services/alignment/gc_content.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2152 2021-04-07 13:49:34.000000 phykit-1.9.0/phykit/services/alignment/pairwise_identity.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2284 2021-01-24 17:25:32.000000 phykit-1.9.0/phykit/services/alignment/parsimony_informative_sites.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      481 2021-01-24 17:34:06.000000 phykit-1.9.0/phykit/services/alignment/rcv.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2210 2021-10-17 16:26:29.000000 phykit-1.9.0/phykit/services/alignment/rename_fasta_entries.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2788 2021-02-09 03:21:31.000000 phykit-1.9.0/phykit/services/alignment/sum_of_pairs_score.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1286 2021-01-24 17:35:53.000000 phykit-1.9.0/phykit/services/alignment/variable_sites.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      191 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/base.py
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.837655 phykit-1.9.0/phykit/services/tree/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1257 2021-12-19 14:56:28.000000 phykit-1.9.0/phykit/services/tree/__init__.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4349 2021-12-16 22:22:50.000000 phykit-1.9.0/phykit/services/tree/base.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1305 2021-04-15 20:10:11.000000 phykit-1.9.0/phykit/services/tree/bipartition_support_stats.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1176 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/tree/branch_length_multiplier.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      785 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/tree/collapse_branches.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     7388 2021-09-07 14:27:59.000000 phykit-1.9.0/phykit/services/tree/covarying_evolutionary_rates.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3213 2021-01-24 17:55:51.000000 phykit-1.9.0/phykit/services/tree/dvmc.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      661 2021-09-29 22:27:20.000000 phykit-1.9.0/phykit/services/tree/evolutionary_rate.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3874 2021-12-19 15:37:53.000000 phykit-1.9.0/phykit/services/tree/hidden_paralogy_check.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2161 2021-01-24 18:11:58.000000 phykit-1.9.0/phykit/services/tree/internal_branch_stats.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      871 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/tree/internode_labeler.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1015 2021-08-27 11:27:31.000000 phykit-1.9.0/phykit/services/tree/last_common_ancestor_subtree.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3171 2021-04-19 14:22:43.000000 phykit-1.9.0/phykit/services/tree/lb_score.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3385 2021-12-19 15:45:17.000000 phykit-1.9.0/phykit/services/tree/monophyly_check.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     5319 2021-12-08 15:54:10.000000 phykit-1.9.0/phykit/services/tree/nearest_neighbor_interchange.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1879 2021-01-24 14:25:34.000000 phykit-1.9.0/phykit/services/tree/patristic_distances.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)    15164 2021-04-17 21:52:28.000000 phykit-1.9.0/phykit/services/tree/polytomy_test.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      748 2021-01-24 14:27:30.000000 phykit-1.9.0/phykit/services/tree/print_tree.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      880 2020-10-04 18:33:45.000000 phykit-1.9.0/phykit/services/tree/prune_tree.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1841 2021-10-25 20:19:50.000000 phykit-1.9.0/phykit/services/tree/rename_tree_tips.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3279 2021-09-07 14:36:25.000000 phykit-1.9.0/phykit/services/tree/rf_distance.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      899 2021-10-25 20:22:50.000000 phykit-1.9.0/phykit/services/tree/root_tree.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3830 2021-01-24 14:28:43.000000 phykit-1.9.0/phykit/services/tree/saturation.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2083 2021-01-27 14:57:51.000000 phykit-1.9.0/phykit/services/tree/spurious_sequence.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      458 2021-01-27 14:59:48.000000 phykit-1.9.0/phykit/services/tree/tip_labels.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1013 2021-12-06 13:48:29.000000 phykit-1.9.0/phykit/services/tree/tip_to_tip_distance.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      599 2021-01-27 14:59:51.000000 phykit-1.9.0/phykit/services/tree/total_tree_length.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)      359 2021-01-27 14:54:53.000000 phykit-1.9.0/phykit/services/tree/treeness.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1376 2021-01-27 14:54:18.000000 phykit-1.9.0/phykit/services/tree/treeness_over_rcv.py
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)       21 2021-12-19 15:46:51.000000 phykit-1.9.0/phykit/version.py
+drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2021-12-20 21:34:28.794640 phykit-1.9.0/phykit.egg-info/
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4765 2021-12-20 21:34:28.000000 phykit-1.9.0/phykit.egg-info/PKG-INFO
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2305 2021-12-20 21:34:28.000000 phykit-1.9.0/phykit.egg-info/SOURCES.txt
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)        1 2021-12-20 21:34:28.000000 phykit-1.9.0/phykit.egg-info/dependency_links.txt
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4860 2021-12-20 21:34:28.000000 phykit-1.9.0/phykit.egg-info/entry_points.txt
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)       50 2021-12-20 21:34:28.000000 phykit-1.9.0/phykit.egg-info/requires.txt
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)        7 2021-12-20 21:34:28.000000 phykit-1.9.0/phykit.egg-info/top_level.txt
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)       38 2021-12-20 21:34:28.839612 phykit-1.9.0/setup.cfg
+-rw-r--r--   0 jlsteenwyk   (501) staff       (20)     7779 2021-12-19 15:48:05.000000 phykit-1.9.0/setup.py
```

### Comparing `phykit-1.8.0/LICENSE.md` & `phykit-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/PKG-INFO` & `phykit-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phykit
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/jlsteenwyk/phykit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phykit Version: 1.8.0 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: phykit Version: 1.9.0 Summary: UNKNOWN Home-page:
 https://github.com/jlsteenwyk/phykit Author: Jacob L. Steenwyk Author-email:
 jlsteenwyk@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Topic :: Scientific/Engineering Description-Content-
```

### Comparing `phykit-1.8.0/README.md` & `phykit-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/helpers/files.py` & `phykit-1.9.0/phykit/helpers/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
             print(f"{alignment_file_path} corresponds to no such file.")
             print("Please check file name and pathing")
             sys.exit()
 
 def read_single_column_file_to_list(single_col_file_path: str) -> list:
     try:
         with open(single_col_file_path) as f:
-            return [line.rstrip('\n') for line in f]
+            return [line.rstrip('\n').strip() for line in f]
     except FileNotFoundError:
         print(f"{single_col_file_path} corresponds to no such file or directory.")
         print("Please check file name and pathing")
         sys.exit()
```

### Comparing `phykit-1.8.0/phykit/helpers/stats_summary.py` & `phykit-1.9.0/phykit/helpers/stats_summary.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/phykit.py` & `phykit-1.9.0/phykit/phykit.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     DVMC,
     EvolutionaryRate,
     HiddenParalogyCheck,
     InternalBranchStats,
     InternodeLabeler,
     LastCommonAncestorSubtree,
     LBScore,
+    MonophylyCheck,
     NearestNeighborInterchange,
     PatristicDistances,
     PolytomyTest,
     PrintTree,
     PruneTree,
     RenameTreeTips,
     RobinsonFouldsDistance,
@@ -186,14 +187,16 @@
                     - calculates summary statistics for internal branch lengths 
                 internode_labeler (alias: il)
                     - create labels at internodes in a phylogeny
                 last_common_ancestor_subtree (alias: lca_subtree)
                     - get last common ancestor of a set of taxa
                 long_branch_score (alias: lb_score; lbs)
                     - calculates lb (long branch) score for taxa in a phylogeny
+                monophyly_check (alias: is_monophyletic)
+                    - determines if a set of tip names are monophyletic
                 nearest_neighbor_interchange (alias: nni)
                     - make nearest neighbor interchange moves on a tree
                 patristic_distances (alias: pd)
                     - calculate all pairwise distances between tips in a tree
                 polytomy_test (alias: polyt_test; polyt; ptt)
                     - conducts a polytomy test using gene
                       support frequencies
@@ -292,15 +295,17 @@
             return self.internal_branch_stats(argv)
         elif command == 'il':
             return self.internode_labeler(argv)
         elif command in ['lca_subtree']:
             return self.last_common_ancestor_subtree(argv)
         elif command in ['long_branch_score', 'lbs']:
             return self.lb_score(argv)
-        elif command in ['nni']:
+        elif command == 'is_monophyletic':
+            return self.monophyly_check(argv)
+        elif command == 'nni':
             return self.nearest_neighbor_interchange(argv)
         elif command == 'pd':
             return self.patristic_distances(argv)
         elif command in ['polyt_test', 'ptt', 'polyt']:
             return self.polytomy_test(argv)
         elif command in ['print', 'pt']:
             return self.print_tree(argv)
@@ -1153,27 +1158,30 @@
                 "A", "B", and "C" are monophyletic and "D",
                 "E", and "F" are expected to be monophyletic, the
                 clade file should be formatted as follows:
                 "
                 A B C
                 D E F
                 "
+                Tip names not present in the tree will not be considered
+                when assessing hidden paralogy.
 
                 The output will have six columns and as many rows
                 as clades were specified in the -c file. For example,
                 if there were three rows of clades to examine the 
                 monophyly of, there will be three rows in the output
                 where the first row in the output corresponds to the 
                 results of the first row in the clade file.
                 col 1: if the clade was or wasn't monophyletic
                 col 2: average bipartition support value in the clade of interest
                 col 3: maximum bipartition support value in the clade of interest
                 col 4: minimum bipartition support value in the clade of interest
                 col 5: standard deviation of bipartition support values in the clade of interest
-                col 6: tip names of the clade specified in the clade file
+                col 6: tip names of taxa monophyletic with the lineage of interest
+                       excluding those that are listed in the taxa_of_interest file
 
                 The concept behind this analysis follows
                 Siu-Ting et al., Molecular Biology and Evolution (2019).
 
                 Aliases:
                   hidden_paralogy_check, clan_check
                 Command line interfaces:
@@ -1368,14 +1376,67 @@
         )
         parser.add_argument("tree", type=str, help=SUPPRESS)
         parser.add_argument("-v", "--verbose", action="store_true", required=False, help=SUPPRESS)
         args = parser.parse_args(argv)
         LBScore(args).run()
 
     @staticmethod
+    def monophyly_check(argv):
+        parser = ArgumentParser(add_help=True,
+            usage=SUPPRESS,
+            formatter_class=RawDescriptionHelpFormatter,
+            description=textwrap.dedent(
+                f"""\
+                {help_header}
+                Check for monophyly of a lineage.
+
+                This analysis can be used to determine if a set of 
+                taxa are monophyletic.
+
+                Requires a taxa file, which species which tip names
+                are expected to be monophyletic. File format is a
+                single column file with tip names. Tip names not
+                present in the tree will not be considered when
+                examining monophyly.
+
+                The output will have six columns.
+                col 1: if the clade was or wasn't monophyletic
+                col 2: average bipartition support value in the clade of interest
+                col 3: maximum bipartition support value in the clade of interest
+                col 4: minimum bipartition support value in the clade of interest
+                col 5: standard deviation of bipartition support values in the clade of interest
+                col 6: tip names of taxa monophyletic with the lineage of interest
+                       excluding those that are listed in the taxa_of_interest file
+
+                Aliases:
+                  monophyly_check, is_monophyletic
+                Command line interfaces:
+                  pk_monophyly_check, pk_is_monophyletic
+
+                Usage:
+                phykit monophyly_check <tree> <list_of_taxa>
+
+                Options
+                =====================================================
+                <tree>                      first argument after 
+                                            function name should be
+                                            a tree file
+
+                <list_of_taxa>              single column file with
+                                            list of tip names to 
+                                            examine the monophyly of
+                """
+            ),
+        )
+        parser.add_argument("tree", type=str, help=SUPPRESS)
+        parser.add_argument("list_of_taxa", type=str, help=SUPPRESS)
+        args = parser.parse_args(argv)
+        MonophylyCheck(args).run()
+
+    @staticmethod
     def nearest_neighbor_interchange(argv):
         parser = ArgumentParser(add_help=True,
             usage=SUPPRESS,
             formatter_class=RawDescriptionHelpFormatter,
             description=textwrap.dedent(
                 f"""\
                 {help_header}
@@ -2251,14 +2312,17 @@
 
 def last_common_ancestor_subtree(argv=None):
     Phykit.last_common_ancestor_subtree(sys.argv[1:])
 
 def lb_score(argv=None):
     Phykit.lb_score(sys.argv[1:])
 
+def monophyly_check(argv=None):
+    Phykit.monophyly_check(sys.argv[1:])
+
 def nearest_neighbor_interchange(argv=None):
     Phykit.nearest_neighbor_interchange(sys.argv[1:])
 
 def patristic_distances(argv=None):
     Phykit.patristic_distances(sys.argv[1:])
 
 def polytomy_test(argv=None):
```

### Comparing `phykit-1.8.0/phykit/services/alignment/__init__.py` & `phykit-1.9.0/phykit/services/alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/alignment_length_no_gaps.py` & `phykit-1.9.0/phykit/services/alignment/alignment_length_no_gaps.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/base.py` & `phykit-1.9.0/phykit/services/alignment/base.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/column_score.py` & `phykit-1.9.0/phykit/services/alignment/column_score.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/create_concatenation_matrix.py` & `phykit-1.9.0/phykit/services/alignment/create_concatenation_matrix.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/dna_threader.py` & `phykit-1.9.0/phykit/services/alignment/dna_threader.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/gc_content.py` & `phykit-1.9.0/phykit/services/alignment/gc_content.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/pairwise_identity.py` & `phykit-1.9.0/phykit/services/alignment/pairwise_identity.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/parsimony_informative_sites.py` & `phykit-1.9.0/phykit/services/alignment/parsimony_informative_sites.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/rename_fasta_entries.py` & `phykit-1.9.0/phykit/services/alignment/rename_fasta_entries.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/sum_of_pairs_score.py` & `phykit-1.9.0/phykit/services/alignment/sum_of_pairs_score.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/alignment/variable_sites.py` & `phykit-1.9.0/phykit/services/alignment/variable_sites.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/__init__.py` & `phykit-1.9.0/phykit/services/tree/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .dvmc import DVMC
 from .evolutionary_rate import EvolutionaryRate
 from .hidden_paralogy_check import HiddenParalogyCheck
 from .internal_branch_stats import InternalBranchStats
 from .internode_labeler import InternodeLabeler
 from .last_common_ancestor_subtree import LastCommonAncestorSubtree
 from .lb_score import LBScore
+from .monophyly_check import MonophylyCheck
 from .nearest_neighbor_interchange import NearestNeighborInterchange
 from .patristic_distances import PatristicDistances
 from .polytomy_test import PolytomyTest
 from .print_tree import PrintTree
 from .prune_tree import PruneTree
 from .rename_tree_tips import RenameTreeTips
 from .root_tree import RootTree
```

### Comparing `phykit-1.8.0/phykit/services/tree/base.py` & `phykit-1.9.0/phykit/services/tree/base.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/bipartition_support_stats.py` & `phykit-1.9.0/phykit/services/tree/bipartition_support_stats.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/branch_length_multiplier.py` & `phykit-1.9.0/phykit/services/tree/branch_length_multiplier.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/collapse_branches.py` & `phykit-1.9.0/phykit/services/tree/collapse_branches.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/covarying_evolutionary_rates.py` & `phykit-1.9.0/phykit/services/tree/covarying_evolutionary_rates.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/dvmc.py` & `phykit-1.9.0/phykit/services/tree/dvmc.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/evolutionary_rate.py` & `phykit-1.9.0/phykit/services/tree/evolutionary_rate.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/hidden_paralogy_check.py` & `phykit-1.9.0/phykit/services/tree/hidden_paralogy_check.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,23 +33,23 @@
             # determine shared tips
             shared_tree_tips = self.shared_tips(clade_of_interest, tree_tips)
             # get tips that differ
             diff_tips = list(set(tree_tips) - set(shared_tree_tips))
             # root tree with different tips
             tree.root_with_outgroup(diff_tips)
             # get common ancestor of clan of interest
-            tree = tree.common_ancestor(clan)
+            tree = tree.common_ancestor(shared_tree_tips)
             # get common ancestor tree tips
             common_ancestor_tips = self.get_tip_names_from_tree(tree)        
             diff_tips_between_clade_and_curr_tree = list(set(clade_of_interest) ^ set(common_ancestor_tips))
 
             stats = self.get_bootstrap_statistics(tree)
 
             res_arr = self.populate_res_arr(
-                clade,
+                shared_tree_tips,
                 diff_tips_between_clade_and_curr_tree,
                 stats,
                 res_arr
             )
 
         self.print_results(res_arr)
 
@@ -80,15 +80,15 @@
                 bs_vals.append(terminal.confidence)
         stats = calculate_summary_statistics_from_arr(bs_vals)
 
         return stats
 
     def populate_res_arr(
         self,
-        clade,
+        shared_tree_tips,
         diff_tips_between_clade_and_curr_tree,
         stats,
         res_arr
     ):
 
         temp = []
 
@@ -96,18 +96,22 @@
             temp.append("monophyletic")
         else:
             temp.append("not_monophyletic")
         temp.append(stats["mean"])
         temp.append(stats["maximum"])
         temp.append(stats["minimum"])
         temp.append(stats["standard_deviation"])
-        temp.append(clade)
+        temp.append(diff_tips_between_clade_and_curr_tree)
         res_arr.append(temp)
 
         return res_arr
 
     def print_results(self, res_arr):
         for res in res_arr:
             try:
-                print(f"{res[0]}\t{round(res[1], 4)}\t{round(res[2], 4)}\t{round(res[3], 4)}\t{round(res[4], 4)}\t{';'.join(res[5])}")
+                if len(res[5]) != 0:
+                    res[5].sort()
+                    print(f"{res[0]}\t{round(res[1], 4)}\t{round(res[2], 4)}\t{round(res[3], 4)}\t{round(res[4], 4)}\t{';'.join(res[5])}")
+                else:
+                    print(f"{res[0]}\t{round(res[1], 4)}\t{round(res[2], 4)}\t{round(res[3], 4)}\t{round(res[4], 4)}")
             except IndexError:
                 print(f"{res[0]}")
```

### Comparing `phykit-1.8.0/phykit/services/tree/internal_branch_stats.py` & `phykit-1.9.0/phykit/services/tree/internal_branch_stats.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/internode_labeler.py` & `phykit-1.9.0/phykit/services/tree/internode_labeler.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/last_common_ancestor_subtree.py` & `phykit-1.9.0/phykit/services/tree/last_common_ancestor_subtree.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/lb_score.py` & `phykit-1.9.0/phykit/services/tree/lb_score.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/nearest_neighbor_interchange.py` & `phykit-1.9.0/phykit/services/tree/nearest_neighbor_interchange.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/patristic_distances.py` & `phykit-1.9.0/phykit/services/tree/patristic_distances.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/polytomy_test.py` & `phykit-1.9.0/phykit/services/tree/polytomy_test.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/print_tree.py` & `phykit-1.9.0/phykit/services/tree/print_tree.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/prune_tree.py` & `phykit-1.9.0/phykit/services/tree/prune_tree.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/rename_tree_tips.py` & `phykit-1.9.0/phykit/services/tree/rename_tree_tips.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/rf_distance.py` & `phykit-1.9.0/phykit/services/tree/rf_distance.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/root_tree.py` & `phykit-1.9.0/phykit/services/tree/root_tree.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/saturation.py` & `phykit-1.9.0/phykit/services/tree/saturation.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/spurious_sequence.py` & `phykit-1.9.0/phykit/services/tree/spurious_sequence.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/tip_to_tip_distance.py` & `phykit-1.9.0/phykit/services/tree/tip_to_tip_distance.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/total_tree_length.py` & `phykit-1.9.0/phykit/services/tree/total_tree_length.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit/services/tree/treeness_over_rcv.py` & `phykit-1.9.0/phykit/services/tree/treeness_over_rcv.py`

 * *Files identical despite different names*

### Comparing `phykit-1.8.0/phykit.egg-info/PKG-INFO` & `phykit-1.9.0/phykit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phykit
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/jlsteenwyk/phykit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phykit Version: 1.8.0 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: phykit Version: 1.9.0 Summary: UNKNOWN Home-page:
 https://github.com/jlsteenwyk/phykit Author: Jacob L. Steenwyk Author-email:
 jlsteenwyk@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Topic :: Scientific/Engineering Description-Content-
```

### Comparing `phykit-1.8.0/phykit.egg-info/SOURCES.txt` & `phykit-1.9.0/phykit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 phykit/services/tree/dvmc.py
 phykit/services/tree/evolutionary_rate.py
 phykit/services/tree/hidden_paralogy_check.py
 phykit/services/tree/internal_branch_stats.py
 phykit/services/tree/internode_labeler.py
 phykit/services/tree/last_common_ancestor_subtree.py
 phykit/services/tree/lb_score.py
+phykit/services/tree/monophyly_check.py
 phykit/services/tree/nearest_neighbor_interchange.py
 phykit/services/tree/patristic_distances.py
 phykit/services/tree/polytomy_test.py
 phykit/services/tree/print_tree.py
 phykit/services/tree/prune_tree.py
 phykit/services/tree/rename_tree_tips.py
 phykit/services/tree/rf_distance.py
```

### Comparing `phykit-1.8.0/phykit.egg-info/entry_points.txt` & `phykit-1.9.0/phykit.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,22 @@
 pk_ge = phykit.phykit:faidx
 pk_get_entry = phykit.phykit:faidx
 pk_hidden_paralogy_check = phykit.phykit:hidden_paralogy_check
 pk_ibs = phykit.phykit:internal_branch_stats
 pk_il = phykit.phykit:internode_labeler
 pk_internal_branch_stats = phykit.phykit:internal_branch_stats
 pk_internode_labeler = phykit.phykit:internode_labeler
+pk_is_monophyletic = phykit.phykit:monophyly_check
 pk_labels = phykit.phykit:tip_labels
 pk_last_common_ancestor_subtree = phykit.phykit:last_common_ancestor_subtree
 pk_lb_score = phykit.phykit:lb_score
 pk_lbs = phykit.phykit:lb_score
 pk_lca_subtree = phykit.phykit:last_common_ancestor_subtree
 pk_long_branch_score = phykit.phykit:lb_score
+pk_monophyly_check = phykit.phykit:monophyly_check
 pk_nearest_neighbor_interchange = phykit.phykit:nearest_neighbor_interchange
 pk_nni = phykit.phykit:nearest_neighbor_interchange
 pk_p2n = phykit.phykit:thread_dna
 pk_pairwise_id = phykit.phykit:pairwise_identity
 pk_pairwise_identity = phykit.phykit:pairwise_identity
 pk_pal2nal = phykit.phykit:thread_dna
 pk_parsimony_informative_sites = phykit.phykit:parsimony_informative_sites
```

### Comparing `phykit-1.8.0/setup.py` & `phykit-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
             "pk_internode_labeler = phykit.phykit:internode_labeler",
             "pk_il = phykit.phykit:internode_labeler",
             "pk_last_common_ancestor_subtree = phykit.phykit:last_common_ancestor_subtree",
             "pk_lca_subtree = phykit.phykit:last_common_ancestor_subtree",
             "pk_lb_score = phykit.phykit:lb_score",
             "pk_long_branch_score = phykit.phykit:lb_score",
             "pk_lbs = phykit.phykit:lb_score",
+            "pk_monophyly_check = phykit.phykit:monophyly_check",
+            "pk_is_monophyletic = phykit.phykit:monophyly_check",
             "pk_nearest_neighbor_interchange = phykit.phykit:nearest_neighbor_interchange",
             "pk_nni = phykit.phykit:nearest_neighbor_interchange",
             "pk_patristic_distances = phykit.phykit:patristic_distances",
             "pk_pd = phykit.phykit:patristic_distances",
             "pk_polytomy_test = phykit.phykit:polytomy_test",
             "pk_polyt_test = phykit.phykit:polytomy_test",
             "pk_ptt = phykit.phykit:polytomy_test",
```

