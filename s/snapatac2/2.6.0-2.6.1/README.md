# Comparing `tmp/snapatac2-2.6.0.tar.gz` & `tmp/snapatac2-2.6.1.tar.gz`

## Comparing `snapatac2-2.6.0.tar` & `snapatac2-2.6.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0     1001      127      991 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/Cargo.toml
--rw-r--r--   0     1001      127     1080 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/LICENSE
--rw-r--r--   0     1001      127      724 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/embedding.rs
--rw-r--r--   0     1001      127    12674 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/export.rs
--rw-r--r--   0     1001      127     2687 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/knn.rs
--rw-r--r--   0     1001      127      117 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/lib.rs
--rw-r--r--   0     1001      127    10726 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/motif.rs
--rw-r--r--   0     1001      127     2765 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/network.rs
--rw-r--r--   0     1001      127    19657 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs
--rw-r--r--   0     1001      127     5504 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/bam.rs
--rw-r--r--   0     1001      127    18667 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/coverage.rs
--rw-r--r--   0     1001      127    31384 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/genome.rs
--rw-r--r--   0     1001      127     9606 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/import.rs
--rw-r--r--   0     1001      127     7967 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/matrix.rs
--rw-r--r--   0     1001      127     6990 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data.rs
--rw-r--r--   0     1001      127      427 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/mod.rs
--rw-r--r--   0     1001      127    12622 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/preprocessing/qc.rs
--rw-r--r--   0     1001      127    13427 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/utils/similarity.rs
--rw-r--r--   0     1001      127     5168 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-core/src/utils.rs
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 snapatac2-2.6.0/snapatac2-python/Cargo.toml
--rw-r--r--   0     1001      127     1080 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/LICENSE
--rw-r--r--   0     1001      127       85 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/README.md
--rw-r--r--   0     1001      127      655 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/__init__.py
--rw-r--r--   0     1001      127     2616 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/_io.py
--rw-r--r--   0     1001      127     3767 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/_utils.py
--rw-r--r--   0     1001      127    11895 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/datasets.py
--rw-r--r--   0     1001      127     7376 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/export/__init__.py
--rw-r--r--   0     1001      127     6065 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/genome.py
--rw-r--r--   0     1001      127     7190 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/metrics/__init__.py
--rw-r--r--   0     1001      127    10983 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/plotting/__init__.py
--rw-r--r--   0     1001      127    16396 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/plotting/_base.py
--rw-r--r--   0     1001      127     2911 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/plotting/_network.py
--rw-r--r--   0     1001      127      204 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/__init__.py
--rw-r--r--   0     1001      127    36750 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_basic.py
--rw-r--r--   0     1001      127     3509 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0     1001      127     3031 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_knn.py
--rw-r--r--   0     1001      127     6030 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0     1001      127     5005 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py
--rw-r--r--   0     1001      127    14287 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py
--rw-r--r--   0     1001      127      324 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/__init__.py
--rw-r--r--   0     1001      127     8737 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_call_peaks.py
--rw-r--r--   0     1001      127    11325 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_clustering.py
--rw-r--r--   0     1001      127     9283 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_diff.py
--rw-r--r--   0     1001      127    19477 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_embedding.py
--rw-r--r--   0     1001      127     1251 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_integration.py
--rw-r--r--   0     1001      127    11022 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_misc.py
--rw-r--r--   0     1001      127     4509 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_motif.py
--rw-r--r--   0     1001      127    19618 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_network.py
--rw-r--r--   0     1001      127     2078 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_smooth.py
--rw-r--r--   0     1001      127    13898 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/call_peaks.rs
--rw-r--r--   0     1001      127    15035 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/embedding.rs
--rw-r--r--   0     1001      127     2583 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/export.rs
--rw-r--r--   0     1001      127      748 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/knn.rs
--rw-r--r--   0     1001      127     3461 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/lib.rs
--rw-r--r--   0     1001      127     4697 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/motif.rs
--rw-r--r--   0     1001      127     1195 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/network.rs
--rw-r--r--   0     1001      127    11430 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/preprocessing.rs
--rw-r--r--   0     1001      127     8499 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/utils/anndata.rs
--rw-r--r--   0     1001      127    10679 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/src/utils.rs
--rw-r--r--   0     1001      127     2015 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_func.py
--rw-r--r--   0     1001      127     2105 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_pipeline.py
--rw-r--r--   0     1001      127     4262 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_similarity.py
--rw-r--r--   0     1001      127      132 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_tools/test.bam
--rw-r--r--   0     1001      127      130 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_tools/test.bed.gz
--rw-r--r--   0     1001      127      131 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_tools/test_clean.tsv.gz
--rw-r--r--   0     1001      127     4668 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/tests/test_tools.py
--rw-r--r--   0     1001      127    96250 2024-03-09 13:28:26.000000 snapatac2-2.6.0/snapatac2-python/Cargo.lock
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 snapatac2-2.6.0/pyproject.toml
--rw-r--r--   0     1001      127     7376 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/export/__init__.py
--rw-r--r--   0     1001      127     3031 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/_knn.py
--rw-r--r--   0     1001      127     3509 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0     1001      127    36750 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/_basic.py
--rw-r--r--   0     1001      127    14287 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/_scrublet.py
--rw-r--r--   0     1001      127     6030 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0     1001      127     5005 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/_scanorama.py
--rw-r--r--   0     1001      127      204 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/preprocessing/__init__.py
--rw-r--r--   0     1001      127     2911 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/plotting/_network.py
--rw-r--r--   0     1001      127    10983 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/plotting/__init__.py
--rw-r--r--   0     1001      127    16396 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/plotting/_base.py
--rw-r--r--   0     1001      127    11895 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/datasets.py
--rw-r--r--   0     1001      127     2616 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/_io.py
--rw-r--r--   0     1001      127     6065 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/genome.py
--rw-r--r--   0     1001      127     8737 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_call_peaks.py
--rw-r--r--   0     1001      127    19618 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_network.py
--rw-r--r--   0     1001      127    19477 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_embedding.py
--rw-r--r--   0     1001      127     4509 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_motif.py
--rw-r--r--   0     1001      127     1251 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_integration.py
--rw-r--r--   0     1001      127     2078 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_smooth.py
--rw-r--r--   0     1001      127     9283 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_diff.py
--rw-r--r--   0     1001      127    11022 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_misc.py
--rw-r--r--   0     1001      127      324 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/__init__.py
--rw-r--r--   0     1001      127    11325 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/tools/_clustering.py
--rw-r--r--   0     1001      127      655 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/__init__.py
--rw-r--r--   0     1001      127     3767 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/_utils.py
--rw-r--r--   0     1001      127     7190 2024-03-09 13:28:26.000000 snapatac2-2.6.0/python/snapatac2/metrics/__init__.py
--rw-r--r--   0     1001      127       85 2024-03-09 13:28:26.000000 snapatac2-2.6.0/README.md
--rw-r--r--   0     1001      127     1080 2024-03-09 13:28:26.000000 snapatac2-2.6.0/LICENSE
--rw-r--r--   0        0        0     2284 1970-01-01 00:00:00.000000 snapatac2-2.6.0/PKG-INFO
+-rw-r--r--   0     1001      127      994 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/Cargo.toml
+-rw-r--r--   0     1001      127     1080 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/LICENSE
+-rw-r--r--   0     1001      127      724 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/embedding.rs
+-rw-r--r--   0     1001      127    12674 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/export.rs
+-rw-r--r--   0     1001      127     2687 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/knn.rs
+-rw-r--r--   0     1001      127      117 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/lib.rs
+-rw-r--r--   0     1001      127    10767 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/motif.rs
+-rw-r--r--   0     1001      127     2765 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/network.rs
+-rw-r--r--   0     1001      127    19661 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs
+-rw-r--r--   0     1001      127     5504 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam.rs
+-rw-r--r--   0     1001      127    18667 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/coverage.rs
+-rw-r--r--   0     1001      127    31384 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/genome.rs
+-rw-r--r--   0     1001      127     9610 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/import.rs
+-rw-r--r--   0     1001      127     7967 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/matrix.rs
+-rw-r--r--   0     1001      127     6990 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data.rs
+-rw-r--r--   0     1001      127      427 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/mod.rs
+-rw-r--r--   0     1001      127    12773 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/preprocessing/qc.rs
+-rw-r--r--   0     1001      127    13427 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/utils/similarity.rs
+-rw-r--r--   0     1001      127     5168 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-core/src/utils.rs
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 snapatac2-2.6.1/snapatac2-python/Cargo.toml
+-rw-r--r--   0     1001      127     1080 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/LICENSE
+-rw-r--r--   0     1001      127       85 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/README.md
+-rw-r--r--   0     1001      127      655 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/__init__.py
+-rw-r--r--   0     1001      127     2616 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/_io.py
+-rw-r--r--   0     1001      127     3767 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/_utils.py
+-rw-r--r--   0     1001      127    11895 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/datasets.py
+-rw-r--r--   0     1001      127     7376 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/export/__init__.py
+-rw-r--r--   0     1001      127     6145 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/genome.py
+-rw-r--r--   0     1001      127     7190 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/metrics/__init__.py
+-rw-r--r--   0     1001      127    11034 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/__init__.py
+-rw-r--r--   0     1001      127    16396 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_base.py
+-rw-r--r--   0     1001      127     2911 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_network.py
+-rw-r--r--   0     1001      127      204 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0     1001      127    37676 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0     1001      127     3509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0     1001      127     3031 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0     1001      127     6030 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0     1001      127     5005 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py
+-rw-r--r--   0     1001      127    14260 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py
+-rw-r--r--   0     1001      127      324 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/__init__.py
+-rw-r--r--   0     1001      127     8737 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0     1001      127    11325 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_clustering.py
+-rw-r--r--   0     1001      127     9283 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_diff.py
+-rw-r--r--   0     1001      127    19537 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_embedding.py
+-rw-r--r--   0     1001      127     1251 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_integration.py
+-rw-r--r--   0     1001      127    11022 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_misc.py
+-rw-r--r--   0     1001      127     4509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_motif.py
+-rw-r--r--   0     1001      127    19618 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_network.py
+-rw-r--r--   0     1001      127     2078 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_smooth.py
+-rw-r--r--   0     1001      127    13935 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/call_peaks.rs
+-rw-r--r--   0     1001      127    15184 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/embedding.rs
+-rw-r--r--   0     1001      127     3156 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/export.rs
+-rw-r--r--   0     1001      127      748 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/knn.rs
+-rw-r--r--   0     1001      127     3451 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/lib.rs
+-rw-r--r--   0     1001      127     4759 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/motif.rs
+-rw-r--r--   0     1001      127     1195 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/network.rs
+-rw-r--r--   0     1001      127    11649 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/preprocessing.rs
+-rw-r--r--   0     1001      127     8499 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/utils/anndata.rs
+-rw-r--r--   0     1001      127    10859 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/src/utils.rs
+-rw-r--r--   0     1001      127     2015 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_func.py
+-rw-r--r--   0     1001      127     2195 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_pipeline.py
+-rw-r--r--   0     1001      127     4262 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_similarity.py
+-rw-r--r--   0     1001      127      132 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools/test.bam
+-rw-r--r--   0     1001      127      130 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools/test.bed.gz
+-rw-r--r--   0     1001      127      131 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools/test_clean.tsv.gz
+-rw-r--r--   0     1001      127     4668 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/tests/test_tools.py
+-rw-r--r--   0     1001      127    99127 2024-05-03 00:36:51.000000 snapatac2-2.6.1/snapatac2-python/Cargo.lock
+-rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 snapatac2-2.6.1/pyproject.toml
+-rw-r--r--   0     1001      127    11325 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_clustering.py
+-rw-r--r--   0     1001      127     1251 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_integration.py
+-rw-r--r--   0     1001      127     8737 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0     1001      127     4509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_motif.py
+-rw-r--r--   0     1001      127     9283 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_diff.py
+-rw-r--r--   0     1001      127     2078 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_smooth.py
+-rw-r--r--   0     1001      127    19537 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_embedding.py
+-rw-r--r--   0     1001      127      324 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/__init__.py
+-rw-r--r--   0     1001      127    19618 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_network.py
+-rw-r--r--   0     1001      127    11022 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/tools/_misc.py
+-rw-r--r--   0     1001      127    16396 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/plotting/_base.py
+-rw-r--r--   0     1001      127    11034 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/plotting/__init__.py
+-rw-r--r--   0     1001      127     2911 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/plotting/_network.py
+-rw-r--r--   0     1001      127    11895 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/datasets.py
+-rw-r--r--   0     1001      127     7190 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/metrics/__init__.py
+-rw-r--r--   0     1001      127     2616 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/_io.py
+-rw-r--r--   0     1001      127      655 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/__init__.py
+-rw-r--r--   0     1001      127    14260 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_scrublet.py
+-rw-r--r--   0     1001      127     6030 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0     1001      127      204 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0     1001      127     5005 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_scanorama.py
+-rw-r--r--   0     1001      127     3509 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0     1001      127     3031 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0     1001      127    37676 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0     1001      127     3767 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/_utils.py
+-rw-r--r--   0     1001      127     6145 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/genome.py
+-rw-r--r--   0     1001      127     7376 2024-05-03 00:36:51.000000 snapatac2-2.6.1/python/snapatac2/export/__init__.py
+-rw-r--r--   0     1001      127       85 2024-05-03 00:36:51.000000 snapatac2-2.6.1/README.md
+-rw-r--r--   0     1001      127     1080 2024-05-03 00:36:51.000000 snapatac2-2.6.1/LICENSE
+-rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 snapatac2-2.6.1/PKG-INFO
```

### Comparing `snapatac2-2.6.0/snapatac2-core/Cargo.toml` & `snapatac2-2.6.1/snapatac2-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 description = "Rust APIs"
 license = "MIT"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
-anndata = "0.3"
+anndata = "0.3.3"
 anyhow = "1.0"
 bigtools = { version = "0.4", features = ["read", "write"] }
 bincode = "1.3"
 bed-utils = "0.2"
 extsort = "0.4"
 flate2 = "1.0"
 tokio = "1.34"
 hora = "0.1"
 kdtree = "0.7"
 itertools = "0.12"
-indexmap = "2.0"
+indexmap = "2.2"
 indicatif = {version = "0.17", features = ["rayon"] }
 lexical = "6.1"
 log = "0.4"
 ndarray = { version = "0.15", features = ["rayon"] }
 num = "0.4"
-noodles = { version = "0.64", features = ["core", "bam", "sam", "gff", "gtf"] }
+noodles = { version = "0.70", features = ["core", "bam", "sam", "gff", "gtf"] }
 nalgebra-sparse = "0.9"
-polars = { version = "0.37", features = ["ndarray", "dtype-categorical"] }
-rayon = "1.8"
+polars = { version = "0.39", features = ["ndarray", "dtype-categorical"] }
+rayon = "1.10"
 regex = "1.6"
 serde = "1.0"
 statrs = "0.16"
 smallvec = "1.13"
 tempfile = "3.3"
 zstd = { version = "0.13", features = ["zstdmt"] }
```

### Comparing `snapatac2-2.6.0/snapatac2-core/LICENSE` & `snapatac2-2.6.1/snapatac2-core/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/embedding.rs` & `snapatac2-2.6.1/snapatac2-core/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/export.rs` & `snapatac2-2.6.1/snapatac2-core/src/export.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/knn.rs` & `snapatac2-2.6.1/snapatac2-core/src/knn.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/motif.rs` & `snapatac2-2.6.1/snapatac2-core/src/motif.rs`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,16 @@
         let mut cur_match = 0.0;
         loop {
             let sc = match seq[cur_pos + start] {
                 b'A' | b'a' => (self.probability[cur_pos][0] / bg.0[0]).ln(),
                 b'C' | b'c' => (self.probability[cur_pos][1] / bg.0[1]).ln(),
                 b'G' | b'g' => (self.probability[cur_pos][2] / bg.0[2]).ln(),
                 b'T' | b't' => (self.probability[cur_pos][3] / bg.0[3]).ln(),
-                b'N' => 0.0,
-                _ => panic!("invalid nucleotide: {}", seq[cur_pos + start]),
+                b'N' | b'n' => 0.0,
+                _ => panic!("invalid nucleotide: {}", String::from_utf8(vec![seq[cur_pos + start]]).unwrap()),
             };
             cur_match += sc;
             let cur_best = cur_match + remain_best[cur_pos];
 
             if cur_best < thres {
                 return None;
             } else if cur_pos >= n - 1 {
```

### Comparing `snapatac2-2.6.0/snapatac2-core/src/network.rs` & `snapatac2-2.6.1/snapatac2-core/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
                 }
 
                 if flags.is_last_segment() {
                     self.read_2 += 1;
                 }
 
                 if !flags.is_unmapped() {
-                    if flags.is_properly_aligned() {
+                    if flags.is_properly_segmented() {
                         self.proper_pair += 1;
                     }
 
                     if flags.is_mate_unmapped() {
                         self.singleton += 1;
                     } else {
                         self.mate_mapped += 1;
@@ -379,15 +379,15 @@
     //   - read fails platform/vendor quality checks
     //   - read is PCR or optical duplicate
     let flag_failed = Flags::from_bits(1804).unwrap();
     reads.filter(move |r| {
         flagstat.update(r);
         let flag = r.flags();
         let is_properly_aligned = !flag.is_supplementary() &&
-            (!is_paired || flag.is_properly_aligned());
+            (!is_paired || flag.is_properly_segmented());
         let flag_pass = !flag.intersects(flag_failed);
         let mapq_pass = mapq_filter.map_or(true, |min_q| {
             let q = r.mapping_quality().map_or(255, |x| x.get());
             q >= min_q
         });
         is_properly_aligned && flag_pass && mapq_pass
     })
```

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/bam.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/bam.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/coverage.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/coverage.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/genome.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/genome.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/import.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/import.rs`

 * *Files 0% similar despite different names*

```diff
@@ -137,17 +137,17 @@
 where
     V: TryFrom<i64> + Ord,
     <V as TryFrom<i64>>::Error: std::fmt::Debug,
 {
     let mut qc = FragmentSummary::new(mitochrondrial_dna);
     let mut values = Vec::new();
     fragments.into_iter().for_each(|f| {
-        qc.update(&f);
         let chrom = &f.chrom;
         if genome_index.contain_chrom(chrom) {
+            qc.update(&f);
             let start = f.start as i64;
             let end = f.end as i64;
             let size = end - start;
             let pos;
             let shift: V;
             match f.strand {
                 Some(Strand::Reverse) => {
```

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data/matrix.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data/matrix.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/count_data.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/count_data.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/preprocessing/qc.rs` & `snapatac2-2.6.1/snapatac2-core/src/preprocessing/qc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -195,18 +195,18 @@
             num_total_fragment: 0,
             num_mitochondrial: 0,
             mitochondrial_dna,
         }
     }
 
     pub(crate) fn update(&mut self, fragment: &Fragment) {
+        self.num_total_fragment += fragment.count as u64;
         if self.mitochondrial_dna.contains(fragment.chrom.as_str()) {
             self.num_mitochondrial += 1;
         } else {
-            self.num_total_fragment += fragment.count as u64;
             self.num_unique_fragment += 1;
         }
     }
 
     pub(crate) fn get_qc(self) -> QualityControl {
         let frac_duplicated = 1.0 -
             (self.num_unique_fragment + self.num_mitochondrial) as f64 /
@@ -226,15 +226,17 @@
     (0 .. n).map(move |i| {
         let r = i.saturating_sub(half_window) .. std::cmp::min(i + half_window + 1, n);
         let l = r.len() as f64;
         arr[r].iter().sum::<u64>() as f64 / l
     })
 }
 
-/// Read tss from a gtf or gff file
+/// Read tss from a gtf or gff file. Note the returned result can potentially
+/// contain redudant elements as there may be multiple transcripts for the same gene
+/// in the annotation file.
 pub fn read_tss<R: Read>(file: R) -> impl Iterator<Item = (String, u64, bool)> {
     let reader = BufReader::new(file);
     reader.lines().filter_map(|line| {
         let chr_idx: usize = 0;
         let type_idx: usize = 2;
         let start_idx: usize = 3;
         let end_idx: usize = 4;
```

### Comparing `snapatac2-2.6.0/snapatac2-core/src/utils/similarity.rs` & `snapatac2-2.6.1/snapatac2-core/src/utils/similarity.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-core/src/utils.rs` & `snapatac2-2.6.1/snapatac2-core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/Cargo.toml` & `snapatac2-2.6.1/snapatac2-python/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 [package]
 name = "snapatac2"
-version = "2.6.0"
+version = "2.6.1"
 edition = "2021"
 authors = ["Kai Zhang <kai@kzhang.org>"]
 description = "Rust APIs"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
 snapatac2-core = { path = "../snapatac2-core" }
-anndata = "0.3"
+anndata = "0.3.3"
 anndata-hdf5 = "0.2"
-pyanndata = "0.3.1"
+pyanndata = "0.3.3"
 extsort = "0.4"
 anyhow = "1.0"
 bed-utils = "0.2"
 flate2 = "1.0"
 itertools = "0.12"
 indicatif = "0.17"
 linreg = "0.2"
 log = "0.4"
 linfa = "0.6"
 linfa-clustering = "0.6"
-noodles = { version = "0.64", features = ["bam", "sam"] }
-numpy = "0.20.0"
+noodles = { version = "0.70", features = ["bam", "sam"] }
+numpy = "0.21.0"
 nalgebra-sparse = "0.9"
 nalgebra = "0.32"
 ndarray = "0.15"
-polars = { version = "0.37", features = ["ndarray", "dtype-categorical"] }
-pyo3-log = "0.9"
-pyo3-polars = "0.11.3"
+polars = { version = "0.39", features = ["ndarray", "dtype-categorical"] }
+pyo3-log = "0.10"
+pyo3-polars = "0.13"
 rand_isaac = "0.3"
 rand_core = "0.6"
 rand = "0.8"
-rayon = "1.8"
+rayon = "1.10"
 statrs = "0.16"
 tempfile = "3.3"
 zstd = { version = "0.13", features = ["zstdmt"] }
 
 [target.'cfg(not(target_env = "msvc"))'.dependencies]
 tikv-jemallocator = {version = "0.5", features = ["disable_initial_exec_tls"]}
 
 [dependencies.pyo3]
-version = "0.20.2"
+version = "0.21.2"
 features = ["extension-module", "anyhow"]
 
 [lib]
 name = "snapatac2"
 crate-type = ["cdylib"]
```

### Comparing `snapatac2-2.6.0/snapatac2-python/LICENSE` & `snapatac2-2.6.1/snapatac2-python/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/__init__.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/_io.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/_utils.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/_utils.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/datasets.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/export/__init__.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/genome.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/genome.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,16 @@
     chrom_sizes= {"chr1": 248956422, "chr2": 242193529, "chr3": 198295559,
                   "chr4": 190214555, "chr5": 181538259, "chr6": 170805979,
                   "chr7": 159345973, "chr8": 145138636, "chr9": 138394717,
                   "chr10": 133797422, "chr11": 135086622, "chr12": 133275309,
                   "chr13": 114364328, "chr14": 107043718, "chr15": 101991189,
                   "chr16": 90338345, "chr17": 83257441, "chr18": 80373285,
                   "chr19": 58617616, "chr20": 64444167, "chr21": 46709983,
-                  "chr22": 50818468, "chrX": 156040895, "chrY": 57227415},
+                  "chr22": 50818468, "chrX": 156040895, "chrY": 57227415,
+                  "chrM": 16569 },
     )
 hg38 = GRCh38
 
 GRCm39 = Genome(
     fasta=lambda : datasets().fetch(
         "gencode_vM30_GRCm39.fa.gz", processor=Decompress(method = "gzip"), progressbar=True),
     annotation=lambda : datasets().fetch(
@@ -157,14 +158,15 @@
         "chr15": 104073951,
         "chr16": 98008968,
         "chr17": 95294699,
         "chr18": 90720763,
         "chr19": 61420004,
         "chrX": 169476592,
         "chrY": 91455967,
+        "chrM": 16299,
     },
     )
 mm39 = GRCm39
 
 GRCm38 = Genome(
     fasta=lambda : datasets().fetch(
         "gencode_vM25_GRCm38.fa.gz", processor=Decompress(method = "gzip"), progressbar=True),
@@ -188,10 +190,11 @@
         "chr15": 104043685,
         "chr16": 98207768,
         "chr17": 94987271,
         "chr18": 90702639,
         "chr19": 61431566,
         "chrX": 171031299,
         "chrY": 91744698,
+        "chrM": 16299,
     },
     )
 mm10 = GRCm38
```

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/metrics/__init__.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/plotting/__init__.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         "yaxis": { "visible": False, "autorange": "reversed" },
         "xaxis": { "title": groupby },
     }
     fig = go.Figure(data=data, layout=layout)
     return render_plot(fig, width, height, interactive, show, out_file)
 
 def umap(
-    adata: AnnData,
+    adata: AnnData | np.ndarray,
     color: str | np.ndarray | None = None,
     use_rep: str = "X_umap",
     marker_size: float = None,
     marker_opacity: float = 1,
     sample_size: int | None = None,
     **kwargs,
 ) -> 'plotly.graph_objects.Figure' | None:
@@ -258,24 +258,23 @@
     -------
     'plotly.graph_objects.Figure' | None
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
     """
     from natsort import index_natsorted
 
-    embedding = adata.obsm[use_rep] 
-
+    embedding = adata.obsm[use_rep] if is_anndata(adata) else adata
     if isinstance(color, str):
         groups = adata.obs[color].to_numpy()
     else:
         groups = color
         color = "color"
     
-    if sample_size is not None and adata.shape[0] > sample_size:
-        idx = np.random.choice(adata.shape[0], sample_size, replace=False)
+    if sample_size is not None and embedding.shape[0] > sample_size:
+        idx = np.random.choice(embedding.shape[0], sample_size, replace=False)
         embedding = embedding[idx, :]
         if groups is not None: groups = groups[idx]
 
     if groups is not None:
         idx = index_natsorted(groups)
         embedding = embedding[idx, :]
         groups = [groups[i] for i in idx]
```

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/plotting/_base.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/plotting/_network.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_basic.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,18 @@
         Indicate whether the BAM file contain paired-end reads
     barcode_tag
         Extract barcodes from TAG fields of BAM records, e.g., `barcode_tag="CB"`.
     barcode_regex
         Extract barcodes from read names of BAM records using regular expressions.
         Reguler expressions should contain exactly one capturing group 
         (Parentheses group the regex between them) that matches
-        the barcodes. For example, `barcode_regex="(..:..:..:..):\\w+$"`
+        the barcodes. For example, `barcode_regex="(..:..:..:..):\\\\w+$"`
         extracts `bd:69:Y6:10` from
         `A01535:24:HW2MMDSX2:2:1359:8513:3458:bd:69:Y6:10:TGATAGGTTG`.
+        You can test your regex on this website: https://regex101.com/.
     umi_tag
         Extract UMI from TAG fields of BAM records.
     umi_regex
         Extract UMI from read names of BAM records using regular expressions.
         See `barcode_regex` for more details.
     shift_left
         Insertion site correction for the left end. Note this has no effect on single-end reads.
@@ -177,14 +178,28 @@
     - When `file` is not `None`, this function uses constant memory regardless of
       the size of the input file.
     - When `sorted_by_barcode` is `False`, this function will sort the fragment file
       first, during which temporary files will be created in `tempdir`. The size of
       temporary files is proportional to the number of records in the fragment file.
       For large fragment files, it is recommended to set `tempdir` to a location with
       sufficient space in order to avoid running out of disk space.
+    - The QC metrics are computed only for reads that are included by the `whitelist`
+      or `chrom_sizes`.
+
+    Warning
+    -------
+    When the input to the function is a list of files, it employs multiprocessing
+    to process these files concurrently. In this case, however, it is crucial to
+    safeguard the entry point of the program by encapsulating the function call
+    within `if __name__ == '__main__':`. This condition ensures that the module
+    is being run as the main program and not being loaded as a module from
+    another script. Without this protection, each subprocess might attempt to
+    spawn its own subprocesses, leading to a cascade of process spawns—a situation
+    that can cause the program to hang or crash due to infinite recursion.
+    You don't need to do this in Jupyter notebook as it automatically does that.
 
     Parameters
     ----------
     fragment_file
         File name of the fragment file, optionally compressed with gzip or zstd.
         This can be a single file or a list of files.
         If it is a list of files, a separate AnnData object will be created for each file.
```

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_knn.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
     if verbose: logging.info('Spectral embedding ...')
     n = count_matrix.shape[0]
     merged_matrix = ss.vstack([count_matrix, count_matrix_sim])
     del count_matrix_sim
     gc.collect()
     _, evecs = spectral(
-        AnnData(X=merged_matrix, dtype=merged_matrix.dtype),
+        AnnData(X=merged_matrix),
         features=None,
         n_comps=n_comps,
         inplace=False,
     )
     manifold = np.asanyarray(evecs)
     manifold_obs = manifold[0:n, ]
     manifold_sim = manifold[n:, ]
```

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_call_peaks.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_clustering.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_diff.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_diff.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_embedding.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 def umap(
     adata: internal.AnnData | internal.AnnDataSet | np.ndarray,
     n_comps: int = 2,
     use_dims: int | list[int] | None = None,
     use_rep: str = "X_spectral",
     key_added: str = 'umap',
-    random_state: int = 0,
+    random_state: int | None = 0,
     inplace: bool = True,
     **kwargs
 ) -> np.ndarray | None:
     """
     Parameters
     ----------
     adata
@@ -95,15 +95,19 @@
     np.ndarray | None
         if `inplace=True` it stores UMAP embedding in
         `adata.obsm["X_`key_added`"]`.
         Otherwise, it returns the result as a numpy array.
     """
     from umap import UMAP
 
-    data = adata.obsm[use_rep] if is_anndata(adata) else adata
+    if is_anndata(adata):
+        data = adata.obsm[use_rep]
+    else:
+        data = adata
+        inplace = False
 
     if use_dims is not None:
         data = data[:, :use_dims] if isinstance(use_dims, int) else data[:, use_dims]
 
     umap = UMAP(random_state=random_state,
                 n_components=n_comps,
                 **kwargs).fit_transform(data)
```

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_integration.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_misc.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_motif.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_network.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/python/snapatac2/tools/_smooth.py` & `snapatac2-2.6.1/snapatac2-python/python/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/src/call_peaks.rs` & `snapatac2-2.6.1/snapatac2-python/src/call_peaks.rs`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 use anndata_hdf5::H5;
 use anyhow::{ensure, Result};
 use bed_utils::bed::{io::Reader, tree::BedTree, BEDLike, GenomicRange};
 use polars::{
     prelude::{DataFrame, NamedFrom},
     series::Series,
 };
-use pyo3::prelude::*;
+use pyo3::{prelude::*, pybacked::PyBackedStr};
 use pyo3_polars::PyDataFrame;
 use rayon::iter::{ParallelBridge, ParallelIterator};
 use std::collections::HashSet;
 use std::io::Write;
 use std::sync::{Arc, Mutex};
 use std::{collections::HashMap, ops::Deref, path::PathBuf};
 
@@ -63,16 +63,16 @@
         Series::new(key.as_str(), values)
     });
     Ok(PyDataFrame(DataFrame::new(std::iter::once(peaks_str).chain(iter).collect())?))
 }
 
 #[pyfunction]
 pub fn find_reproducible_peaks<'py>(
-    peaks: &'py PyAny,
-    replicates: Vec<&'py PyAny>,
+    peaks: &Bound<'py, PyAny>,
+    replicates: Vec<Bound<'py, PyAny>>,
     blacklist: Option<PathBuf>,
 ) -> Result<PyDataFrame> {
     let black: BedTree<_> = if let Some(black) = blacklist {
         Reader::new(utils::open_file_for_read(black), None)
             .into_records::<GenomicRange>()
             .map(|x| (x.unwrap(), ()))
             .collect()
@@ -82,40 +82,40 @@
 
     let peaks = get_peaks(peaks)?
         .into_iter()
         .filter(|x| !black.is_overlapped(x))
         .collect::<Vec<_>>();
     let replicates = replicates
         .into_iter()
-        .map(|x| BedTree::from_iter(get_peaks(x).unwrap().into_iter().map(|x| (x, ()))))
+        .map(|x| BedTree::from_iter(get_peaks(&x).unwrap().into_iter().map(|x| (x, ()))))
         .collect::<Vec<_>>();
     let peaks: Vec<_> = peaks
         .into_iter()
         .filter(|x| replicates.iter().all(|y| y.is_overlapped(x)))
         .collect();
     Ok(PyDataFrame(narrow_peak_to_dataframe(peaks)?))
 }
 
 #[pyfunction]
 pub fn fetch_peaks<'py>(
-    peaks: HashMap<String, &'py PyAny>,
+    peaks: HashMap<String, Bound<'py, PyAny>>,
     blacklist: Option<PathBuf>,
 ) -> Result<HashMap<String, PyDataFrame>> {
     let black: BedTree<_> = if let Some(black) = blacklist {
         Reader::new(utils::open_file_for_read(black), None)
             .into_records::<GenomicRange>()
             .map(|x| (x.unwrap(), ()))
             .collect()
     } else {
         Default::default()
     };
     peaks
         .into_iter()
         .map(|(key, peaks)| {
-            let ps = get_peaks(peaks)?
+            let ps = get_peaks(&peaks)?
                 .into_iter()
                 .filter(|x| !black.is_overlapped(x))
                 .collect::<Vec<_>>();
             Ok((key, PyDataFrame(narrow_peak_to_dataframe(ps).unwrap())))
         })
         .collect::<Result<_>>()
 }
@@ -205,15 +205,15 @@
         Series::new("q_value", q_values),
         Series::new("peak", peaks),
     ])?;
 
     Ok(df)
 }
 
-fn get_peaks<'py>(peak_io_obj: &'py PyAny) -> Result<Vec<NarrowPeak>> {
+fn get_peaks<'py>(peak_io_obj: &Bound<'py, PyAny>) -> Result<Vec<NarrowPeak>> {
     peak_io_obj
         .getattr("peaks")?
         .downcast::<pyo3::types::PyDict>()
         .unwrap()
         .iter()
         .flat_map(|(chr, peaks)| {
             let chrom = String::from_utf8(chr.extract().unwrap()).unwrap();
@@ -247,29 +247,28 @@
         .collect()
 }
 
 #[pyfunction]
 pub fn create_fwtrack_obj<'py>(
     py: Python<'py>,
     files: Vec<PathBuf>,
-) -> Result<(&'py PyAny, Vec<&'py PyAny>)> {
-    let macs = py.import("MACS3.Signal.FixWidthTrack")?;
+) -> Result<(Bound<'py, PyAny>, Vec<Bound<'py, PyAny>>)> {
+    let macs = py.import_bound("MACS3.Signal.FixWidthTrack")?;
     let merged = macs.getattr("FWTrack")?.call1((1000000,))?;
     let has_replicate = files.len() > 1;
     let replicates = files
         .into_iter()
         .map(|fl| {
-            let kwargs = pyo3::types::PyDict::new(py);
+            let kwargs = pyo3::types::PyDict::new_bound(py);
             kwargs.set_item("buffer_size", 100000)?;
-            let fwt = macs.getattr("FWTrack")?.call((), Some(kwargs))?;
+            let fwt = macs.getattr("FWTrack")?.call((), Some(&kwargs))?;
             let reader = utils::open_file_for_read(&fl);
             bed_utils::bed::io::Reader::new(reader, None)
                 .into_records::<Fragment>()
                 .try_for_each(|x| {
-                    let _pool = unsafe { py.new_pool() }; // This is necessary to release memory of objects created in the loop
                     let x = x?;
                     let chr = x.chrom().as_bytes();
                     match x.strand() {
                         None => {
                             fwt.call_method1("add_loc", (chr, x.start(), 0))?;
                             fwt.call_method1("add_loc", (chr, x.end() - 1, 1))?;
                             if has_replicate {
@@ -296,26 +295,26 @@
             Ok(fwt)
         })
         .collect::<Result<Vec<_>>>()?;
     if has_replicate {
         merged.call_method0("finalize")?;
         Ok((merged, replicates))
     } else {
-        Ok((replicates[0], Vec::new()))
+        Ok((replicates.into_iter().next().unwrap(), Vec::new()))
     }
 }
 
 #[pyfunction]
 pub fn export_tags(
     anndata: AnnDataLike,
     dir: PathBuf,
-    group_by: Vec<&str>,
-    replicates: Option<Vec<&str>>,
+    group_by: Vec<PyBackedStr>,
+    replicates: Option<Vec<PyBackedStr>>,
     max_frag_size: Option<u64>,
-    selections: Option<HashSet<&str>>,
+    selections: Option<HashSet<String>>,
 ) -> Result<HashMap<String, Vec<PathBuf>>> {
     macro_rules! run {
         ($data:expr) => {
             _export_tags(
                 $data,
                 dir,
                 &group_by,
@@ -328,28 +327,28 @@
 
     crate::with_anndata!(&anndata, run)
 }
 
 fn _export_tags<D: SnapData, P: AsRef<std::path::Path>>(
     data: &D,
     dir: P,
-    group_by: &Vec<&str>,
-    replicates: Option<&Vec<&str>>,
+    group_by: &Vec<PyBackedStr>,
+    replicates: Option<&Vec<PyBackedStr>>,
     max_frag_size: Option<u64>,
-    selections: Option<HashSet<&str>>,
+    selections: Option<HashSet<String>>,
 ) -> Result<HashMap<String, Vec<PathBuf>>> {
     // Get keys
     ensure!(data.n_obs() == group_by.len(), "lengths differ");
     let keys: Vec<(&str, &str)> = match replicates {
         Some(rep) => group_by
             .iter()
             .zip(rep.iter())
-            .map(|(x, y)| (*x, *y))
+            .map(|(x, y)| (x.as_ref(), y.as_ref()))
             .collect(),
-        None => group_by.iter().map(|x| (*x, "")).collect(),
+        None => group_by.iter().map(|x| (x.as_ref(), "")).collect(),
     };
     let mut unique_keys: HashSet<(&str, &str)> = keys.iter().cloned().unique().collect();
 
     // Create output files
     if let Some(select) = selections {
         unique_keys.retain(|x| select.contains(x.0));
     }
```

### Comparing `snapatac2-2.6.0/snapatac2-python/src/embedding.rs` & `snapatac2-2.6.1/snapatac2-python/src/embedding.rs`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 use rayon::prelude::{ParallelBridge, ParallelIterator};
 use std::ops::Deref;
 
 #[pyfunction]
 pub(crate) fn spectral_embedding<'py>(
     py: Python<'py>,
     anndata: AnnDataLike,
-    selected_features: &PyAny,
+    selected_features: &Bound<'_, PyAny>,
     n_components: usize,
     random_state: i64,
     feature_weights: Option<Vec<f64>>,
-) -> Result<(&'py PyArray1<f64>, &'py PyArray2<f64>)> {
+) -> Result<(Bound<'py, PyArray1<f64>>, Bound<'py, PyArray2<f64>>)> {
     macro_rules! run {
         ($data:expr) => {{
             let slice = pyanndata::data::to_select_elem(selected_features, $data.n_vars())?;
             let mut mat: CsrMatrix<f64> = $data.x().slice_axis(1, slice)?.unwrap();
             if let Some(weights) = feature_weights {
                 normalize(&mut mat, &weights);
             } else {
@@ -42,30 +42,30 @@
             let (v, u, _) = spectral_mf(mat, n_components, random_state)?;
             anyhow::Ok((v, u))
         }};
     }
     let (evals, evecs) = crate::with_anndata!(&anndata, run)?;
 
     Ok((
-        PyArray1::from_owned_array(py, evals),
-        PyArray2::from_owned_array(py, evecs),
+        PyArray1::from_owned_array_bound(py, evals),
+        PyArray2::from_owned_array_bound(py, evecs),
     ))
 }
 
 #[pyfunction]
 pub(crate) fn spectral_embedding_nystrom<'py>(
     py: Python<'py>,
     anndata: AnnDataLike,
-    selected_features: &PyAny,
+    selected_features: &Bound<'_, PyAny>,
     n_components: usize,
     sample_size: usize,
     weighted_by_degree: bool,
     chunk_size: usize,
     feature_weights: Option<Vec<f64>>,
-) -> Result<(&'py PyArray1<f64>, &'py PyArray2<f64>)> {
+) -> Result<(Bound<'py, PyArray1<f64>>, Bound<'py, PyArray2<f64>>)> {
     macro_rules! run {
         ($data:expr) => {{
             let selected_features =
                 pyanndata::data::to_select_elem(selected_features, $data.n_vars())?;
             let weights = if let Some(weights) = feature_weights {
                 weights
             } else {
@@ -111,16 +111,16 @@
                 }),
             )
         }};
     }
 
     let (evals, evecs) = crate::with_anndata!(&anndata, run)?;
     Ok((
-        PyArray1::from_owned_array(py, evals),
-        PyArray2::from_owned_array(py, evecs),
+        PyArray1::from_owned_array_bound(py, evals),
+        PyArray2::from_owned_array_bound(py, evecs),
     ))
 }
 
 /// Matrix-free spectral embedding.
 /// The input is assumed to be a csr matrix with rows normalized to unit L2 norm.
 fn spectral_mf(
     mut input: CsrMatrix<f64>,
@@ -141,15 +141,15 @@
     input
         .row_iter_mut()
         .zip(degree_inv.iter())
         .for_each(|(mut row, d)| row.values_mut().iter_mut().for_each(|x| *x *= d.sqrt()));
 
     // Compute eigenvalues and eigenvectors
     let (v, u) = Python::with_gil(|py| {
-        let fun: Py<PyAny> = PyModule::from_code(
+        let fun: Py<PyAny> = PyModule::from_code_bound(
             py,
             "def eigen(X, D, k, seed):
                 from scipy.sparse.linalg import LinearOperator, eigsh
                 import numpy
                 numpy.random.seed(seed)
                 def f(v):
                     return X @ (v.T @ X).T - D * v
@@ -164,15 +164,15 @@
             "",
             "",
         )?
         .getattr("eigen")?
         .into();
         let args = (
             PyArrayData::from(ArrayData::from(input)),
-            PyArray1::from_iter(py, degree_inv.into_iter().copied()),
+            PyArray1::from_iter_bound(py, degree_inv.into_iter().copied()),
             n_components,
             random_state,
         );
         let result = fun.call1(py, args)?;
         let (evals, evecs): (&PyArray1<f64>, &PyArray2<f64>) = result.extract(py)?;
 
         anyhow::Ok((evals.to_owned_array(), evecs.to_owned_array()))
@@ -200,19 +200,19 @@
         .zip(degrees.iter())
         .for_each(|(mut row, d)| row *= d.sqrt().recip());
     // normalize the eigenvectors by eigenvalues.
     evecs
         .axis_iter_mut(Axis(1))
         .zip(evals.iter())
         .for_each(|(mut col, v)| col *= v.recip());
-    let evecs_py = PyArray2::from_array(py, evecs);
-    let evals_py = PyArray1::from_array(py, evals);
+    let evecs_py = PyArray2::from_array_bound(py, evecs);
+    let evals_py = PyArray1::from_array_bound(py, evals);
     let seed_matrix_py = PyArrayData::from(ArrayData::from(seed_matrix)).into_py(py);
 
-    let nystrom_py: Py<PyAny> = PyModule::from_code(
+    let nystrom_py: Py<PyAny> = PyModule::from_code_bound(
         py,
         "def nystrom(seed, sample, evecs, evals):
             import numpy as np
             q = sample @ (seed.T @ evecs)
             t = q.sum(axis=0) * evals
             d = q @ t.reshape((-1, 1))
             d[d<=0] = np.min(d[d>0])
@@ -230,16 +230,16 @@
     .unwrap();
     let output: Vec<f64> = inputs
         .into_iter()
         .map(|sample| {
             let args = (
                 &seed_matrix_py,
                 PyArrayData::from(ArrayData::from(sample)),
-                evecs_py,
-                evals_py,
+                &evecs_py,
+                &evals_py,
             );
             nystrom_py
                 .call1(py, args)
                 .unwrap()
                 .extract::<&PyArray2<_>>(py)
                 .unwrap()
                 .to_vec()
@@ -376,27 +376,27 @@
 }
 
 /// Multi-view spectral embedding.
 #[pyfunction]
 pub(crate) fn multi_spectral_embedding<'py>(
     py: Python<'py>,
     anndata: Vec<AnnDataLike>,
-    selected_features: Vec<&PyAny>,
+    selected_features: Vec<Bound<'_, PyAny>>,
     weights: Vec<f64>,
     n_components: usize,
     random_state: i64,
-) -> Result<(&'py PyArray1<f64>, &'py PyArray2<f64>)> {
+) -> Result<(Bound<'py, PyArray1<f64>>, Bound<'py, PyArray2<f64>>)> {
     info!("Compute normalized views...");
     let mats = anndata
         .into_iter()
         .zip(selected_features.into_iter())
         .map(|(a, s)| {
             macro_rules! get_mat {
                 ($data:expr) => {{
-                    let slice = pyanndata::data::to_select_elem(s, $data.n_vars())
+                    let slice = pyanndata::data::to_select_elem(&s, $data.n_vars())
                         .expect("Invalid feature selection");
                     let mut mat: CsrMatrix<f64> =
                         $data.x().slice_axis(1, slice).unwrap().expect("X is None");
                     let feature_weights = idf(&mat);
 
                     // feature weighting and L2 norm normalization.
                     normalize(&mut mat, &feature_weights);
@@ -428,22 +428,22 @@
         })
         .reduce(|a, b| hstack(a, b))
         .unwrap();
 
     info!("Compute embedding...");
     let (evals, evecs, _) = spectral_mf(mat, n_components, random_state)?;
     Ok((
-        PyArray1::from_owned_array(py, evals),
-        PyArray2::from_owned_array(py, evecs),
+        PyArray1::from_owned_array_bound(py, evals),
+        PyArray2::from_owned_array_bound(py, evecs),
     ))
 }
 
 fn frobenius_norm(x: &CsrMatrix<f64>) -> f64 {
     let sum: f64 = Python::with_gil(|py| {
-        let fun: Py<PyAny> = PyModule::from_code(
+        let fun: Py<PyAny> = PyModule::from_code_bound(
             py,
             "def f(X):
                 import numpy as np
                 return np.power(X @ X.T, 2).sum()",
             "",
             "",
         )?
```

### Comparing `snapatac2-2.6.0/snapatac2-python/src/export.rs` & `snapatac2-2.6.1/snapatac2-python/src/export.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 use crate::utils::AnnDataLike;
 use snapatac2_core::{export::{Exporter, Normalization, CoverageOutputFormat}, utils};
 
+use pyo3::{prelude::*, pybacked::PyBackedStr};
 use std::ops::Deref;
 use anndata::Backend;
 use anndata_hdf5::H5;
-use pyo3::prelude::*;
 use std::{collections::{HashSet, HashMap}, path::PathBuf};
 use anyhow::Result;
 use bed_utils::bed::{GenomicRange, io::Reader, tree::BedTree};
 use std::str::FromStr;
 
 #[pyfunction]
 pub fn export_fragments(
     anndata: AnnDataLike,
-    barcodes: Vec<&str>,
-    group_by: Vec<&str>,
+    barcodes: Vec<PyBackedStr>,
+    group_by: Vec<PyBackedStr>,
     dir: PathBuf,
     prefix: &str,
     suffix: &str,
-    selections: Option<HashSet<&str>>,
+    selections: Option<HashSet<PyBackedStr>>,
     min_frag_length: Option<u64>,
     max_frag_length: Option<u64>,
     compression: Option<&str>,
     compression_level: Option<u32>,
 ) -> Result<HashMap<String, PathBuf>> {
+    let barcodes = barcodes.iter().map(|x| x.as_ref()).collect();
+    let group_by = group_by.iter().map(|x| x.as_ref()).collect();
+    let selections = selections.as_ref()
+        .map(|s| s.iter().map(|x| x.as_ref()).collect());
     macro_rules! run {
         ($data:expr) => {
             $data.export_fragments(
                 Some(&barcodes), &group_by, selections, min_frag_length, max_frag_length, dir, prefix, suffix,
                 compression.map(|x| utils::Compression::from_str(x).unwrap()), compression_level
             )
         }
     }
     crate::with_anndata!(&anndata, run)
 }
 
 #[pyfunction]
 pub fn export_coverage(
     anndata: AnnDataLike,
-    group_by: Vec<&str>,
+    group_by: Vec<PyBackedStr>,
     resolution: usize,
     dir: PathBuf,
     prefix: &str,
     suffix:&str,
     output_format: &str,
-    selections: Option<HashSet<&str>>,
+    selections: Option<HashSet<PyBackedStr>>,
     blacklist: Option<PathBuf>,
     normalization: Option<&str>,
-    ignore_for_norm: Option<HashSet<&str>>,
+    ignore_for_norm: Option<HashSet<PyBackedStr>>,
     min_frag_length: Option<u64>,
     max_frag_length: Option<u64>,
     compression: Option<&str>,
     compression_level: Option<u32>,
     temp_dir: Option<PathBuf>,
     num_threads: Option<usize>,
 ) -> Result<HashMap<String, PathBuf>> {
+    let group_by = group_by.iter().map(|x| x.as_ref()).collect();
+    let selections = selections.as_ref()
+        .map(|s| s.iter().map(|x| x.as_ref()).collect());
+    let ignore_for_norm = ignore_for_norm.as_ref()
+        .map(|s| s.iter().map(|x| x.as_ref()).collect());
+
     let black: Option<BedTree<()>> = blacklist.map(|black| {
         Reader::new(utils::open_file_for_read(black), None)
             .into_records::<GenomicRange>()
             .map(|x| (x.unwrap(), ()))
             .collect()
     });
```

### Comparing `snapatac2-2.6.0/snapatac2-python/src/knn.rs` & `snapatac2-2.6.1/snapatac2-python/src/knn.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/src/lib.rs` & `snapatac2-2.6.1/snapatac2-python/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 mod call_peaks;
 mod preprocessing;
 mod embedding;
 mod network;
 mod motif;
 mod knn;
 
-use pyo3::{prelude::*, PyResult, Python};
+use pyo3::{prelude::*, PyResult};
 use pyanndata;
 
 #[cfg(not(target_env = "msvc"))]
 use tikv_jemallocator::Jemalloc;
 
 #[cfg(not(target_env = "msvc"))]
 #[global_allocator]
 static GLOBAL: Jemalloc = Jemalloc;
 
 #[pymodule]
-fn _snapatac2(_py: Python, m: &PyModule) -> PyResult<()> {
+fn _snapatac2(m: &Bound<'_, PyModule>) -> PyResult<()> {
     pyo3_log::init();
 
     // AnnData related functions
     m.add_class::<pyanndata::AnnData>().unwrap();
     m.add_class::<pyanndata::AnnDataSet>().unwrap();
     m.add_class::<pyanndata::PyArrayElem>().unwrap();
     m.add_function(wrap_pyfunction!(pyanndata::read, m)?)?;
```

### Comparing `snapatac2-2.6.0/snapatac2-python/src/motif.rs` & `snapatac2-2.6.1/snapatac2-python/src/motif.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use pyo3::prelude::*;
+use pyo3::{prelude::*, pybacked::PyBackedStr};
 use numpy::{Ix2, PyReadonlyArray};
 use std::fs::File;
 use std::path::Path;
 use std::io::Read;
 use rayon::iter::{IntoParallelIterator, ParallelIterator};
 use statrs::distribution::{Binomial, DiscreteCDF};
 
@@ -14,15 +14,15 @@
 pub struct PyDNAMotif(pub motif::DNAMotif);
 
 #[pymethods]
 impl PyDNAMotif {
     #[new]
     fn new<'py>(
         id: &str,
-        matrix: &'py PyAny,
+        matrix: Bound<'py, PyAny>,
     ) -> Self {
         let pwm: PyReadonlyArray<f64, Ix2> = matrix.extract().unwrap();
         let motif = motif::DNAMotif {
             id: id.to_string(),
             name: None,
             family: None,
             probability: pwm.as_array().rows().into_iter()
@@ -87,20 +87,20 @@
     #[pyo3(signature = (seq, pvalue=1e-5, rc=true))]
     fn exist(&self, seq: &str, pvalue: f64, rc: bool) -> bool {
         self.0.find(seq.as_bytes(), pvalue).next().is_some() ||
             (rc && self.0.find(rev_compl(seq).as_bytes(), pvalue).next().is_some())
     }
 
     #[pyo3(signature = (seqs, pvalue=1e-5, rc=true))]
-    fn exists(&self, seqs: Vec<&str>, pvalue: f64, rc: bool) -> Vec<bool> {
-        seqs.into_par_iter().map(|x| self.exist(x, pvalue, rc)).collect()
+    fn exists(&self, seqs: Vec<PyBackedStr>, pvalue: f64, rc: bool) -> Vec<bool> {
+        seqs.into_par_iter().map(|x| self.exist(x.as_ref(), pvalue, rc)).collect()
     }
 
     #[pyo3(signature = (seqs, pvalue=1e-5))]
-    fn with_background(&self, seqs: Vec<&str>, pvalue: f64) -> PyDNAMotifTest {
+    fn with_background(&self, seqs: Vec<PyBackedStr>, pvalue: f64) -> PyDNAMotifTest {
         let n = seqs.len();
         PyDNAMotifTest {
             scanner: self.clone(),
             pvalue,
             occurrence_background: seqs.into_par_iter().filter(|x| self.exist(x, pvalue, true)).count(),
             total_background: n,
         }
@@ -129,15 +129,15 @@
 impl PyDNAMotifTest {
     #[getter]
     fn id(&self) -> String { self.scanner.id() }
 
     #[getter]
     fn name(&self) -> Option<String> { self.scanner.name() }
 
-    fn test(&self, seqs: Vec<&str>) -> (f64, f64) {
+    fn test(&self, seqs: Vec<PyBackedStr>) -> (f64, f64) {
         let n = seqs.len().try_into().unwrap();
         let occurrence: u64 = seqs.into_par_iter()
             .filter(|x| self.scanner.exist(x, self.pvalue, true)).count()
             .try_into().unwrap();
         let p = self.occurrence_background as f64 / self.total_background as f64;
         let log_fc = ((occurrence as f64 / n as f64) / p).log2();
         let bion = Binomial::new(p, n).unwrap();
```

### Comparing `snapatac2-2.6.0/snapatac2-python/src/network.rs` & `snapatac2-2.6.1/snapatac2-python/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/src/preprocessing.rs` & `snapatac2-2.6.1/snapatac2-python/src/preprocessing.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use crate::utils::*;
 
+use itertools::Itertools;
+use pyo3::{prelude::*, pybacked::PyBackedStr};
 use anndata::Backend;
 use anndata_hdf5::H5;
 use snapatac2_core::preprocessing::count_data::TranscriptParserOptions;
 use snapatac2_core::preprocessing::count_data::CountingStrategy;
 use std::io::{BufRead, BufReader};
 use std::path::PathBuf;
 use std::{str::FromStr, collections::BTreeMap, ops::Deref, collections::HashSet};
-use pyo3::prelude::*;
 use bed_utils::{bed, bed::GenomicRange};
 use pyanndata::PyAnnData;
 use anyhow::Result;
 
 use snapatac2_core::{
     preprocessing::{Fragment, Contact, FlagStat, SnapData},
     preprocessing, utils,
@@ -68,15 +69,15 @@
     Ok(PyFlagStat(stat))
 }
 
 #[pyfunction]
 pub(crate) fn import_fragments(
     anndata: AnnDataLike,
     fragment_file: PathBuf,
-    chrom_size: BTreeMap<&str, u64>,
+    chrom_size: BTreeMap<String, u64>,
     mitochondrial_dna: Vec<String>,
     min_num_fragment: u64,
     fragment_is_sorted_by_name: bool,
     shift_left: i64,
     shift_right: i64,
     chunk_size: usize,
     white_list: Option<HashSet<String>>,
@@ -138,15 +139,15 @@
     }
 }
 
 #[pyfunction]
 pub(crate) fn import_contacts(
     anndata: AnnDataLike,
     contact_file: PathBuf,
-    chrom_size: BTreeMap<&str, u64>,
+    chrom_size: BTreeMap<String, u64>,
     fragment_is_sorted_by_name: bool,
     chunk_size: usize,
     tempdir: Option<PathBuf>,
 ) -> Result<()>
 {
     let chrom_sizes = chrom_size.into_iter().map(|(chr, s)| GenomicRange::new(chr, 0, s)).collect();
 
@@ -190,20 +191,22 @@
 
 #[pyfunction]
 pub(crate) fn mk_tile_matrix(
     anndata: AnnDataLike,
     bin_size: usize,
     chunk_size: usize,
     strategy: &str,
-    exclude_chroms: Option<Vec<&str>>,
+    exclude_chroms: Option<Vec<PyBackedStr>>,
     min_fragment_size: Option<u64>,
     max_fragment_size: Option<u64>,
     out: Option<AnnDataLike>
 ) -> Result<()>
 {
+    let exclude_chroms = exclude_chroms.as_ref()
+        .map(|s| s.iter().map(|x| x.as_ref()).collect::<Vec<_>>());
     macro_rules! run {
         ($data:expr) => {
             if let Some(out) = out {
                 macro_rules! run2 {
                     ($out_data:expr) => {
                         preprocessing::create_tile_matrix(
                             $data,
@@ -236,15 +239,15 @@
     crate::with_anndata!(&anndata, run);
     Ok(())
 }
 
 #[pyfunction]
 pub(crate) fn mk_peak_matrix(
     anndata: AnnDataLike,
-    peaks: &PyAny,
+    peaks: Bound<'_, PyAny>,
     chunk_size: usize,
     use_x: bool,
     strategy: &str,
     min_fragment_size: Option<u64>,
     max_fragment_size: Option<u64>,
     out: Option<AnnDataLike>,
 ) -> Result<()>
@@ -322,28 +325,29 @@
 
 #[pyfunction]
 pub(crate) fn tss_enrichment(
     anndata: AnnDataLike,
     gtf_file: PathBuf,
 ) -> Result<Vec<f64>>
 {
-    let promoters = preprocessing::make_promoter_map(preprocessing::read_tss(utils::open_file_for_read(gtf_file)));
+    let tss = preprocessing::read_tss(utils::open_file_for_read(gtf_file)).unique();
+    let promoters = preprocessing::make_promoter_map(tss);
 
     macro_rules! run {
         ($data:expr) => {
             $data.tss_enrichment(&promoters)
         }
     }
     crate::with_anndata!(&anndata, run)
 }
 
 #[pyfunction]
 pub(crate) fn add_frip(
     anndata: AnnDataLike,
-    regions: BTreeMap<String, Vec<&str>>,
+    regions: BTreeMap<String, Vec<String>>,
 ) -> Result<BTreeMap<String, Vec<f64>>>
 {
     let trees: Vec<_> = regions.values().map(|x|
         x.into_iter().map(|y| (GenomicRange::from_str(y).unwrap(), ())).collect()
     ).collect();
 
     macro_rules! run {
```

### Comparing `snapatac2-2.6.0/snapatac2-python/src/utils/anndata.rs` & `snapatac2-2.6.1/snapatac2-python/src/utils/anndata.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/src/utils.rs` & `snapatac2-2.6.1/snapatac2-python/src/utils.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 mod anndata;
 
-pub use self::anndata::{PyAnnData, AnnDataLike, RustAnnDataLike};
+pub use self::anndata::AnnDataLike;
 
 use pyo3::{
     prelude::*,
     types::PyIterator,
     PyResult, Python,
 };
-use numpy::{Element, PyReadonlyArrayDyn, PyReadonlyArray, Ix1, Ix2, PyArray, IntoPyArray};
+use numpy::{Element, PyReadonlyArrayDyn, PyReadonlyArray, Ix1, Ix2, PyArray, IntoPyArray, PyArrayMethods};
 use snapatac2_core::preprocessing::count_data::TranscriptParserOptions;
 use snapatac2_core::preprocessing::{Transcript, read_transcripts_from_gff, read_transcripts_from_gtf};
 use snapatac2_core::utils;
 
 use bed_utils::{bed, bed::GenomicRange, bed::BED};
 use std::io::BufReader;
 use std::str::FromStr;
@@ -41,30 +41,30 @@
     }
 }
  
 
 #[pyfunction]
 pub(crate) fn jaccard_similarity<'py>(
     py: Python<'py>,
-    mat: &'py PyAny,
-    other: Option<&'py PyAny>,
+    mat: &Bound<'py, PyAny>,
+    other: Option<&Bound<'py, PyAny>>,
     weights: Option<PyReadonlyArray<f64, Ix1>>,
-) -> PyResult<&'py PyArray<f64, Ix2>> {
+) -> PyResult<Bound<'py, PyArray<f64, Ix2>>> {
     let weights_ = match weights {
         None => None,
         Some(ref ws) => Some(ws.as_slice().unwrap()),
     };
 
     macro_rules! with_csr {
         ($mat:expr) => {
             match other {
-                None => Ok(utils::similarity::jaccard($mat, weights_).into_pyarray(py)),
+                None => Ok(utils::similarity::jaccard($mat, weights_).into_pyarray_bound(py)),
                 Some(mat2) => {
                     macro_rules! xxx {
-                        ($m:expr) => { Ok(utils::similarity::jaccard2($mat, $m, weights_).into_pyarray(py)) };
+                        ($m:expr) => { Ok(utils::similarity::jaccard2($mat, $m, weights_).into_pyarray_bound(py)) };
                     }
                     let shape: Vec<usize> = mat2.getattr("shape")?.extract()?;
                     with_sparsity_pattern!(
                         mat2.getattr("indices")?.getattr("dtype")?.getattr("name")?.extract()?,
                         mat2.getattr("indices")?,
                         mat2.getattr("indptr")?,
                         shape[1],
@@ -97,120 +97,120 @@
     let indices = indices_.as_slice().unwrap();
     Ok(utils::similarity::BorrowedSparsityPattern::new(indptr, indices, n))
 }
 
 #[pyfunction]
 pub(crate) fn cosine_similarity<'py>(
     py: Python<'py>,
-    mat: &'py PyAny,
-    other: Option<&'py PyAny>,
+    mat: &Bound<'py, PyAny>,
+    other: Option<&Bound<'py, PyAny>>,
     weights: Option<PyReadonlyArray<f64, Ix1>>,
-) -> PyResult<&'py PyArray<f64, Ix2>> {
+) -> PyResult<Bound<'py, PyArray<f64, Ix2>>> {
     let weights_ = match weights {
         None => None,
         Some(ref ws) => Some(ws.as_slice().unwrap()),
     };
     match other {
-        None => Ok(utils::similarity::cosine(csr_to_rust(mat)?, weights_).into_pyarray(py)),
+        None => Ok(utils::similarity::cosine(csr_to_rust(mat)?, weights_).into_pyarray_bound(py)),
         Some(mat2) => Ok(
             utils::similarity::cosine2(
                 csr_to_rust(mat)?,
                 csr_to_rust(mat2)?,
                 weights_,
-            ).into_pyarray(py)
+            ).into_pyarray_bound(py)
         ),
     }
 }
 
 #[pyfunction]
 pub(crate) fn pearson<'py>(
     py: Python<'py>,
-    mat: &'py PyAny,
-    other: &'py PyAny,
+    mat: &Bound<'py, PyAny>,
+    other: &Bound<'py, PyAny>,
 ) -> PyResult<PyObject> {
     match mat.getattr("dtype")?.getattr("name")?.extract()? {
         "float32" => {
             let mat_ = mat.extract::<PyReadonlyArray<f32, Ix2>>()?.to_owned_array();
             let other_ = other.extract::<PyReadonlyArray<f32, Ix2>>()?.to_owned_array();
-            Ok(utils::similarity::pearson2(mat_, other_).into_pyarray(py).to_object(py))
+            Ok(utils::similarity::pearson2(mat_, other_).into_pyarray_bound(py).to_object(py))
         },
         "float64" => {
             let mat_ = mat.extract::<PyReadonlyArray<f64, Ix2>>()?.to_owned_array();
             let other_ = other.extract::<PyReadonlyArray<f64, Ix2>>()?.to_owned_array();
-            Ok(utils::similarity::pearson2(mat_, other_).into_pyarray(py).to_object(py))
+            Ok(utils::similarity::pearson2(mat_, other_).into_pyarray_bound(py).to_object(py))
         },
         ty => panic!("Cannot compute correlation for type {}", ty),
     }
 }
 
 #[pyfunction]
 pub(crate) fn spearman<'py>(
     py: Python<'py>,
-    mat: &'py PyAny,
-    other: &'py PyAny,
+    mat: &Bound<'py, PyAny>,
+    other: &Bound<'py, PyAny>,
 ) -> PyResult<PyObject> {
     match mat.getattr("dtype")?.getattr("name")?.extract()? {
         "float32" => {
             let mat_ = mat.extract::<PyReadonlyArray<f32, Ix2>>()?.to_owned_array();
             match other.getattr("dtype")?.getattr("name")?.extract()? {
                 "float32" => {
                     let other_ = other.extract::<PyReadonlyArray<f32, Ix2>>()?.to_owned_array();
-                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray(py).to_object(py))
+                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray_bound(py).to_object(py))
                 },
                 "float64" => {
                     let other_ = other.extract::<PyReadonlyArray<f64, Ix2>>()?.to_owned_array();
-                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray(py).to_object(py))
+                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray_bound(py).to_object(py))
                 },
                 ty => panic!("Cannot compute correlation for type {}", ty),
             }
         },
         "float64" => {
             let mat_ = mat.extract::<PyReadonlyArray<f64, Ix2>>()?.to_owned_array();
             match other.getattr("dtype")?.getattr("name")?.extract()? {
                 "float32" => {
                     let other_ = other.extract::<PyReadonlyArray<f32, Ix2>>()?.to_owned_array();
-                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray(py).to_object(py))
+                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray_bound(py).to_object(py))
                 },
                 "float64" => {
                     let other_ = other.extract::<PyReadonlyArray<f64, Ix2>>()?.to_owned_array();
-                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray(py).to_object(py))
+                    Ok(utils::similarity::spearman2(mat_, other_).into_pyarray_bound(py).to_object(py))
                 },
                 ty => panic!("Cannot compute correlation for type {}", ty),
             }
         },
         ty => panic!("Cannot compute correlation for type {}", ty),
     }
 }
 
-fn csr_to_rust<'py>(csr: &'py PyAny) -> PyResult<CsrMatrix<f64>> {
+fn csr_to_rust<'py>(csr: &Bound<'py, PyAny>) -> PyResult<CsrMatrix<f64>> {
     let shape: Vec<usize> = csr.getattr("shape")?.extract()?;
-    let indices = cast_pyarray(csr.getattr("indices")?)?;
-    let indptr = cast_pyarray(csr.getattr("indptr")?)?;
-    let data = cast_pyarray(csr.getattr("data")?)?;
+    let indices = cast_pyarray(&csr.getattr("indices")?)?;
+    let indptr = cast_pyarray(&csr.getattr("indptr")?)?;
+    let data = cast_pyarray(&csr.getattr("data")?)?;
     Ok(CsrMatrix::try_from_csr_data(
         shape[0], shape[1], indptr, indices, data,
     ).unwrap())
 }
 
-fn cast_pyarray<'py, T: Element>(arr: &'py PyAny) -> PyResult<Vec<T>> {
+fn cast_pyarray<'py, T: Element>(arr: &Bound<'py, PyAny>) -> PyResult<Vec<T>> {
     let vec = match arr.getattr("dtype")?.getattr("name")?.extract()? {
         "uint32" => arr.extract::<PyReadonlyArrayDyn<u32>>()?.cast(false)?.to_vec().unwrap(),
         "int32" => arr.extract::<PyReadonlyArrayDyn<i32>>()?.cast(false)?.to_vec().unwrap(),
         "uint64" => arr.extract::<PyReadonlyArrayDyn<u64>>()?.cast(false)?.to_vec().unwrap(),
         "int64" => arr.extract::<PyReadonlyArrayDyn<i64>>()?.cast(false)?.to_vec().unwrap(),
         "float32" => arr.extract::<PyReadonlyArrayDyn<f32>>()?.cast(false)?.to_vec().unwrap(),
         "float64" => arr.extract::<PyReadonlyArrayDyn<f64>>()?.cast(false)?.to_vec().unwrap(),
         ty => panic!("cannot cast type {}", ty),
     };
     Ok(vec)
 }
 
 /// Simple linear regression
 #[pyfunction]
-pub(crate) fn simple_lin_reg(py_iter: &PyIterator) -> PyResult<(f64, f64)> {
+pub(crate) fn simple_lin_reg(py_iter: Bound<'_, PyIterator>) -> PyResult<(f64, f64)> {
     Ok(lin_reg_imprecise(py_iter.map(|x| x.unwrap().extract().unwrap())).unwrap())
 }
 
 /// Perform regression
 #[pyfunction]
 pub(crate) fn jm_regress(
     jm_: PyReadonlyArrayDyn<'_, f64>,
@@ -230,36 +230,36 @@
 #[pyfunction]
 pub(crate) fn read_regions(file: PathBuf) -> Vec<String> {
     let mut reader = bed::io::Reader::new(utils::open_file_for_read(file), None);
     reader.records::<GenomicRange>().map(|x| x.unwrap().pretty_show()).collect()
 }
 
 #[pyfunction]
-pub(crate) fn intersect_bed<'py>(regions: &'py PyAny, bed_file: &str) -> PyResult<Vec<bool>> {
+pub(crate) fn intersect_bed<'py>(regions: Bound<'py, PyAny>, bed_file: &str) -> PyResult<Vec<bool>> {
     let bed_tree: bed::tree::BedTree<()> = bed::io::Reader::new(utils::open_file_for_read(bed_file), None)
         .into_records().map(|x: Result<BED<3>, _>| (x.unwrap(), ())).collect();
-    let res = PyIterator::from_object(regions)?
+    let res = PyIterator::from_bound_object(&regions)?
         .map(|x| bed_tree.is_overlapped(&GenomicRange::from_str(x.unwrap().extract().unwrap()).unwrap()))
         .collect();
     Ok(res)
 }
 
 #[pyfunction]
 pub(crate) fn kmeans<'py>(
     py: Python<'py>,
     n_clusters: usize,
     observations_: PyReadonlyArray<'_, f64, Ix2>,
-) -> PyResult<&'py PyArray<usize, Ix1>> {
+) -> PyResult<Bound<'py, PyArray<usize, Ix1>>> {
     let seed = 42;
     let rng: Isaac64Rng = SeedableRng::seed_from_u64(seed);
     let observations = DatasetBase::from(observations_.as_array());
     let model = KMeans::params_with_rng(n_clusters, rng)
         .fit(&observations)
         .expect("KMeans fitted");
-    Ok(model.predict(observations).targets.into_pyarray(py))
+    Ok(model.predict(observations).targets.into_pyarray_bound(py))
 }
 
 pub fn read_transcripts<P: AsRef<std::path::Path>>(file_path: P, options: &TranscriptParserOptions) -> Vec<Transcript> {
     let path = if file_path.as_ref().extension().unwrap() == "gz" {
         file_path.as_ref().file_stem().unwrap().as_ref()
     } else {
         file_path.as_ref()
```

### Comparing `snapatac2-2.6.0/snapatac2-python/tests/test_func.py` & `snapatac2-2.6.1/snapatac2-python/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/tests/test_pipeline.py` & `snapatac2-2.6.1/snapatac2-python/tests/test_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,25 @@
 
 def test_exclude():
     fragment_file = snap.datasets.pbmc500(downsample=True)
 
     data1 = snap.pp.import_data(
         fragment_file,
         chrom_sizes={chr: size for chr, size in snap.genome.hg38.chrom_sizes.items() if chr not in ["chr1", "chr10"]},
-        sorted_by_barcode=False
+        sorted_by_barcode=False,
+        min_num_fragments=0,
     )
     snap.pp.add_tile_matrix(data1, exclude_chroms=None)
 
-    data2 = snap.pp.import_data(fragment_file, chrom_sizes=snap.genome.hg38, sorted_by_barcode=False)
+    data2 = snap.pp.import_data(
+        fragment_file,
+        chrom_sizes=snap.genome.hg38,
+        sorted_by_barcode=False,
+        min_num_fragments=0,
+    )
     snap.pp.add_tile_matrix(data2, exclude_chroms=["chr1", "chr10"])
 
     np.testing.assert_array_equal(data1.X.data, data2.X.data)
     np.testing.assert_array_equal(data1.obs_names, data2.obs_names)
     np.testing.assert_array_equal(data1.var_names, data2.var_names)
 
 def pipeline(data):
```

### Comparing `snapatac2-2.6.0/snapatac2-python/tests/test_similarity.py` & `snapatac2-2.6.1/snapatac2-python/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/tests/test_tools.py` & `snapatac2-2.6.1/snapatac2-python/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/snapatac2-python/Cargo.lock` & `snapatac2-2.6.1/snapatac2-python/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anndata"
-version = "0.3.1"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f1697ee6fea7f88ee27fb9c229e1794877e4cfc8583465a92f29df92e516ec9"
+checksum = "bb25ab5522d849dda564d6807e7cd17dac43a0fd10d14770c8f8d9b39d4a12be"
 dependencies = [
  "anyhow",
  "flate2",
  "indexmap 2.2.3",
  "itertools 0.12.1",
  "log",
  "nalgebra-sparse",
@@ -172,17 +172,17 @@
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "argminmax"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "202108b46429b765ef483f8a24d5c46f48c14acfdacc086dd4ab6dddf6bcdbd2"
+checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
@@ -863,14 +863,20 @@
 dependencies = [
  "rayon",
  "skeptic",
  "tempfile",
 ]
 
 [[package]]
+name = "fallible-streaming-iterator"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7360491ce676a36bf9bb3c56c1aa791658183a54d2744120f27285738d90465a"
+
+[[package]]
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
 name = "fastrand"
@@ -1820,47 +1826,47 @@
 checksum = "978fe6e6ebc0bf53de533cd456ca2d9de13de13856eda1518a285d7705a213af"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "noodles"
-version = "0.64.0"
+version = "0.70.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fa9a3104049a2a6b31b8b3cf414774832f28cc6fe3fb5fca21ed28e77c7f95f"
+checksum = "e5c7777c4301ec50202f778c15d73b88c30f9240a074f9b9a98fe7babfa5bfc8"
 dependencies = [
  "noodles-bam",
  "noodles-core",
  "noodles-gff",
  "noodles-gtf",
  "noodles-sam",
 ]
 
 [[package]]
 name = "noodles-bam"
-version = "0.56.0"
+version = "0.60.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3189e8ecee801ab5c3f4ea9908c4196b429137d8d35d733f00f6681f9188be7"
+checksum = "880f71c52dab49e073361e0427610e07eccea07ff48a2ecd8f133c648cb115d8"
 dependencies = [
  "bit-vec 0.6.3",
  "bstr",
  "byteorder",
  "bytes",
  "indexmap 2.2.3",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "noodles-sam",
 ]
 
 [[package]]
 name = "noodles-bgzf"
-version = "0.26.0"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8970db2e84adb1007377dd3988258d7a64e3fc4c05602ebf94e1f8cba207c030"
+checksum = "eff82b0fb78c11947b29ef50e8ddf0093813fa9e613af0e13dc53fc12b2dc3ea"
 dependencies = [
  "byteorder",
  "bytes",
  "crossbeam-channel",
  "flate2",
 ]
 
@@ -1868,54 +1874,54 @@
 name = "noodles-core"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7336c3be652de4e05444c9b12a32331beb5ba3316e8872d92bfdd8ef3b06c282"
 
 [[package]]
 name = "noodles-csi"
-version = "0.30.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a60dfe0919f7ecbd081a82eb1d32e8f89f9041932d035fe8309073c8c01277bf"
+checksum = "938d7d865a3fbb079c7855e76eb1ef0be5d285dc039fa7776622225c7f708411"
 dependencies = [
  "bit-vec 0.6.3",
  "byteorder",
  "indexmap 2.2.3",
  "noodles-bgzf",
  "noodles-core",
 ]
 
 [[package]]
 name = "noodles-gff"
-version = "0.27.0"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14f8ec87fe3630f57d6d8ea24cbc2cbd0bfed1fe66238bda7a7c3fb6a36d3713"
+checksum = "9216634517bf888abb425b10f3df7857ee3f584d4e46c8d6a2bb2c84acc4e10e"
 dependencies = [
  "indexmap 2.2.3",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "percent-encoding",
 ]
 
 [[package]]
 name = "noodles-gtf"
-version = "0.23.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab70f06b15bbf2be2144fc6cbedd63666b23ba5fc2513a218973a01702457b2f"
+checksum = "99d4fabc2e574e80c00341685e8f4df37ae0b5a00a6fecccfd7c99eb45d5a4cf"
 dependencies = [
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
 ]
 
 [[package]]
 name = "noodles-sam"
-version = "0.53.0"
+version = "0.57.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f0d8e441368374f6e144989f823fd7c05e58cdaa3f97d22bb4d75b534327b87"
+checksum = "6b0598e959a0e56fc60f11b3bc63bf11c332a530cb54883196c0eab1bd0d4b8a"
 dependencies = [
  "bitflags 2.4.2",
  "bstr",
  "indexmap 2.2.3",
  "lexical-core",
  "memchr",
  "noodles-bgzf",
@@ -2031,17 +2037,17 @@
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -2129,14 +2135,20 @@
  "libc",
  "redox_syscall 0.4.1",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "parquet-format-safe"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
+
+[[package]]
 name = "parse-zoneinfo"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
 dependencies = [
  "regex",
 ]
@@ -2242,33 +2254,37 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e43795c49010cb851d45227caa17769e83760e21d260ba6285c563b754e1652f"
+checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
 dependencies = [
  "getrandom",
+ "polars-arrow",
  "polars-core",
+ "polars-error",
  "polars-io",
  "polars-lazy",
  "polars-ops",
+ "polars-parquet",
  "polars-sql",
  "polars-time",
+ "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faacd21a2548fa6d50c72d6b8d4649a8e029a0f3c6c5545b7f436f0610e49b0f"
+checksum = "725b09f2b5ef31279b66e27bbab63c58d49d8f6696b66b1f46c7eaab95e80f75"
 dependencies = [
  "ahash",
  "atoi",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -2303,31 +2319,33 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d9dc87f8003ae0edeef5ad9ac92b2a345480bbe17adad64496113ae84706dd"
+checksum = "a796945b14b14fbb79b91ef0406e6fddca2be636e889f81ea5d6ee7d36efb4fe"
 dependencies = [
  "bytemuck",
+ "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
+ "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "befd4d280a82219a01035c4f901319ceba65998c594d0c64f9a439cdee1d7777"
+checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "comfy-table",
@@ -2350,29 +2368,29 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50f2435b02d1ba36d8c1f6a722cad04e4c0b2705a3112c5706e6960d405d7798"
+checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
 dependencies = [
  "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b51fba2cf014cb39c2b38353d601540fb9db643be65abb9ca8ff44b9c4c4a88e"
+checksum = "b2c8589e418cbe4a48228d64b2a8a40284a82ec3c98817c0c2bcc0267701338b"
 dependencies = [
  "ahash",
  "atoi_simd",
  "bytes",
  "chrono",
  "fast-float",
  "flate2",
@@ -2394,17 +2412,17 @@
  "simdutf8",
  "smartstring",
  "zstd",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d83343e413346f048f3a5ad07c0ea4b5d0bada701a482878213142970b0ddff8"
+checksum = "89b2632b1af668e2058d5f8f916d8fbde3cac63d03ae29a705f598e41dcfeb7f"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
@@ -2417,17 +2435,17 @@
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6395f5fd5e1adf016fd6403c0a493181c1a349a7a145b2687cdf50a0d630310a"
+checksum = "efdbdb4d9a92109bc2e0ce8e17af5ae8ab643bb5b7ee9d1d74f0aeffd1fbc95f"
 dependencies = [
  "ahash",
  "argminmax",
  "base64",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -2446,18 +2464,37 @@
  "regex",
  "smartstring",
  "unicode-reverse",
  "version_check",
 ]
 
 [[package]]
+name = "polars-parquet"
+version = "0.39.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b421d2196f786fdfe162db614c8485f8308fe41575d4de634a39bbe460d1eb6a"
+dependencies = [
+ "ahash",
+ "base64",
+ "ethnum",
+ "num-traits",
+ "parquet-format-safe",
+ "polars-arrow",
+ "polars-error",
+ "polars-utils",
+ "seq-macro",
+ "simdutf8",
+ "streaming-decompression",
+]
+
+[[package]]
 name = "polars-pipe"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "390a831b864bc57a4cb260b0595030dfb6a4260a3723cf8ca17968ee2078b8ff"
+checksum = "48700f1d5bd56a15451e581f465c09541492750360f18637b196f995470a015c"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown 0.14.3",
  "num-traits",
  "polars-arrow",
@@ -2466,57 +2503,61 @@
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
  "polars-utils",
  "rayon",
  "smartstring",
+ "uuid",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb7d7527be2aa33baace9000f6772eb9df7cd57ec010a4b273435d2dc1349e8"
+checksum = "2fb8e2302e20c44defd5be8cad9c96e75face63c3a5f609aced8c4ec3b3ac97d"
 dependencies = [
  "ahash",
  "bytemuck",
  "chrono-tz",
+ "hashbrown 0.14.3",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
+ "recursive",
  "regex",
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4984d97aad3d0db92afe76ebcab10b5e37a1216618b5703ae0d2917ccd6168c"
+checksum = "a515bdc68c2ae3702e3de70d89601f3b71ca8137e282a226dddb53ee4bacfa2e"
 dependencies = [
+ "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-sql"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77f62a8b8f93146ec1eb2ef340d77eeb174e8010035e449bfdd424d2b1fd944a"
+checksum = "7b4bb7cc1c04c3023d1953b2f1dec50515e8fd8169a5a2bf4967b3b082232db7"
 dependencies = [
  "hex",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-lazy",
  "polars-plan",
@@ -2524,17 +2565,17 @@
  "serde",
  "serde_json",
  "sqlparser",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d75348a51d0c97f3b83df860ecb35a6ac6c5dafc6278cac4e1ac101d96dc753"
+checksum = "efc18e3ad92eec55db89d88f16c22d436559ba7030cf76f86f6ed7a754b673f1"
 dependencies = [
  "atoi",
  "chrono",
  "chrono-tz",
  "now",
  "once_cell",
  "polars-arrow",
@@ -2544,27 +2585,29 @@
  "polars-utils",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.37.0"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f9c955bb1e9b55d835aeb7fe4e4e8826e01abe5f0ada979ceb7d2b9af7b569"
+checksum = "c760b6c698cfe2fbbbd93d6cfb408db14ececfe1d92445dae2229ce1b5b21ae8"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown 0.14.3",
  "indexmap 2.2.3",
  "num-traits",
  "once_cell",
  "polars-error",
+ "raw-cpuid",
  "rayon",
  "smartstring",
+ "stacker",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -2607,29 +2650,38 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "pulldown-cmark"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "57206b407293d2bcd3af849ce869d52068623f19e1b5ff8e8778e3309439682b"
 dependencies = [
  "bitflags 2.4.2",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyanndata"
-version = "0.3.1"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d10b056db3c5f1b9824615e47552a6dfe5c51331734526fa408329411c122eb7"
+checksum = "0c30551f41c9b8c2d04ad34ee5029c3db6c321a5a0297901c7bb700d3100e91f"
 dependencies = [
  "anndata",
  "anndata-hdf5",
  "anyhow",
  "downcast-rs",
  "flate2",
  "hdf5",
@@ -2646,17 +2698,17 @@
  "rand",
  "rayon",
  "thiserror",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
@@ -2666,73 +2718,73 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.9.0"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c10808ee7250403bedb24bc30c32493e93875fef7ba3e4292226fe924f398bd"
+checksum = "2af49834b8d2ecd555177e63b273b708dea75150abc6f5341d0a6e1a9623976c"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.50",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.50",
 ]
 
 [[package]]
 name = "pyo3-polars"
-version = "0.11.3"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fa311764163c831c75f9ca49499abacbf7ece676cad0b059d962a384aa18224"
+checksum = "469bd1d378fb3a34c1b182383e84741d9e7c5451a5d29a3f9c557aac161876cd"
 dependencies = [
  "polars",
  "polars-core",
  "pyo3",
  "thiserror",
 ]
 
@@ -2800,24 +2852,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f97cdb2a36ed4183de61b2f824cc45c9f1037f28afe0a322e9fff4c108b5aaa"
 dependencies = [
  "rand_core",
 ]
 
 [[package]]
+name = "raw-cpuid"
+version = "11.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e29830cbb1290e404f24c73af91c5d8d631ce7e128691e9477556b540cd01ecd"
+dependencies = [
+ "bitflags 2.4.2",
+]
+
+[[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -2826,14 +2887,34 @@
 checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "recursive"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0786a43debb760f491b1bc0269fe5e84155353c67482b9e60d0cfb596054b43e"
+dependencies = [
+ "recursive-proc-macro-impl",
+ "stacker",
+]
+
+[[package]]
+name = "recursive-proc-macro-impl"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76009fbe0614077fc1a2ce255e3a1881a2e3a3527097d5dc6d8212c585e7e38b"
+dependencies = [
+ "quote",
+ "syn 2.0.50",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -3064,14 +3145,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "seq-macro"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
+
+[[package]]
 name = "serde"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
@@ -3175,15 +3262,15 @@
  "autocfg",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "snapatac2"
-version = "2.6.0"
+version = "2.6.1"
 dependencies = [
  "anndata",
  "anndata-hdf5",
  "anyhow",
  "bed-utils",
  "extsort",
  "flate2",
@@ -3265,14 +3352,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "743b4dc2cbde11890ccb254a8fc9d537fa41b36da00de2a1c5e9848c9bc42bd7"
 dependencies = [
  "log",
 ]
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "statrs"
@@ -3284,14 +3384,23 @@
  "lazy_static",
  "nalgebra 0.29.0",
  "num-traits",
  "rand",
 ]
 
 [[package]]
+name = "streaming-decompression"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf6cc3b19bfb128a8ad11026086e31d3ce9ad23f8ea37354b31383a187c44cf3"
+dependencies = [
+ "fallible-streaming-iterator",
+]
+
+[[package]]
 name = "streaming-iterator"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b2231b7c3057d5e4ad0156fb3dc807d900806020c5ffa3ee6ff2c8c76fb8520"
 
 [[package]]
 name = "strength_reduce"
@@ -3566,14 +3675,23 @@
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "vec_map"
```

### Comparing `snapatac2-2.6.0/pyproject.toml` & `snapatac2-2.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -53,11 +53,18 @@
 Homepage = "https://kzhang.org/SnapATAC2/index.html"
 Documentation = "https://kzhang.org/SnapATAC2/index.html"
 Repository = "https://kzhang.org/SnapATAC2/"
 Issues = "https://github.com/kaizhang/SnapATAC2/issues"
 Changelog = "https://kzhang.org/SnapATAC2/version/dev/changelog.html"
 
 [project.optional-dependencies]
-extra = ["scanorama>=1.7.3", "harmonypy>=0.0.9", "xgboost>=1.4", "umap-learn>=0.5.0"]
-recommend = ["scanpy>=1.9", "scvi-tools>=1.0"]
-all = ["snapatac2[extra]", "snapatac2[recommend]"]
+recommend = [
+    "scanorama>=1.7.3",
+    "harmonypy>=0.0.9",
+    "xgboost>=1.4",
+    "umap-learn>=0.5.0",
+    "scanpy>=1.9",
+    "scvi-tools>=1.0",
+    "scikit-misc>=0.1.3",
+    "magic-impute>=2.0",
+]
 test = ["pytest", "hypothesis==6.72.4"]
```

### Comparing `snapatac2-2.6.0/python/snapatac2/export/__init__.py` & `snapatac2-2.6.1/python/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/preprocessing/_knn.py` & `snapatac2-2.6.1/python/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.6.1/python/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/preprocessing/_basic.py` & `snapatac2-2.6.1/python/snapatac2/preprocessing/_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,18 @@
         Indicate whether the BAM file contain paired-end reads
     barcode_tag
         Extract barcodes from TAG fields of BAM records, e.g., `barcode_tag="CB"`.
     barcode_regex
         Extract barcodes from read names of BAM records using regular expressions.
         Reguler expressions should contain exactly one capturing group 
         (Parentheses group the regex between them) that matches
-        the barcodes. For example, `barcode_regex="(..:..:..:..):\\w+$"`
+        the barcodes. For example, `barcode_regex="(..:..:..:..):\\\\w+$"`
         extracts `bd:69:Y6:10` from
         `A01535:24:HW2MMDSX2:2:1359:8513:3458:bd:69:Y6:10:TGATAGGTTG`.
+        You can test your regex on this website: https://regex101.com/.
     umi_tag
         Extract UMI from TAG fields of BAM records.
     umi_regex
         Extract UMI from read names of BAM records using regular expressions.
         See `barcode_regex` for more details.
     shift_left
         Insertion site correction for the left end. Note this has no effect on single-end reads.
@@ -177,14 +178,28 @@
     - When `file` is not `None`, this function uses constant memory regardless of
       the size of the input file.
     - When `sorted_by_barcode` is `False`, this function will sort the fragment file
       first, during which temporary files will be created in `tempdir`. The size of
       temporary files is proportional to the number of records in the fragment file.
       For large fragment files, it is recommended to set `tempdir` to a location with
       sufficient space in order to avoid running out of disk space.
+    - The QC metrics are computed only for reads that are included by the `whitelist`
+      or `chrom_sizes`.
+
+    Warning
+    -------
+    When the input to the function is a list of files, it employs multiprocessing
+    to process these files concurrently. In this case, however, it is crucial to
+    safeguard the entry point of the program by encapsulating the function call
+    within `if __name__ == '__main__':`. This condition ensures that the module
+    is being run as the main program and not being loaded as a module from
+    another script. Without this protection, each subprocess might attempt to
+    spawn its own subprocesses, leading to a cascade of process spawns—a situation
+    that can cause the program to hang or crash due to infinite recursion.
+    You don't need to do this in Jupyter notebook as it automatically does that.
 
     Parameters
     ----------
     fragment_file
         File name of the fragment file, optionally compressed with gzip or zstd.
         This can be a single file or a list of files.
         If it is a list of files, a separate AnnData object will be created for each file.
```

### Comparing `snapatac2-2.6.0/python/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.6.1/python/snapatac2/preprocessing/_scrublet.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
     if verbose: logging.info('Spectral embedding ...')
     n = count_matrix.shape[0]
     merged_matrix = ss.vstack([count_matrix, count_matrix_sim])
     del count_matrix_sim
     gc.collect()
     _, evecs = spectral(
-        AnnData(X=merged_matrix, dtype=merged_matrix.dtype),
+        AnnData(X=merged_matrix),
         features=None,
         n_comps=n_comps,
         inplace=False,
     )
     manifold = np.asanyarray(evecs)
     manifold_obs = manifold[0:n, ]
     manifold_sim = manifold[n:, ]
```

### Comparing `snapatac2-2.6.0/python/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.6.1/python/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/preprocessing/_scanorama.py` & `snapatac2-2.6.1/python/snapatac2/preprocessing/_scanorama.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/plotting/_network.py` & `snapatac2-2.6.1/python/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/plotting/__init__.py` & `snapatac2-2.6.1/python/snapatac2/plotting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         "yaxis": { "visible": False, "autorange": "reversed" },
         "xaxis": { "title": groupby },
     }
     fig = go.Figure(data=data, layout=layout)
     return render_plot(fig, width, height, interactive, show, out_file)
 
 def umap(
-    adata: AnnData,
+    adata: AnnData | np.ndarray,
     color: str | np.ndarray | None = None,
     use_rep: str = "X_umap",
     marker_size: float = None,
     marker_opacity: float = 1,
     sample_size: int | None = None,
     **kwargs,
 ) -> 'plotly.graph_objects.Figure' | None:
@@ -258,24 +258,23 @@
     -------
     'plotly.graph_objects.Figure' | None
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
     """
     from natsort import index_natsorted
 
-    embedding = adata.obsm[use_rep] 
-
+    embedding = adata.obsm[use_rep] if is_anndata(adata) else adata
     if isinstance(color, str):
         groups = adata.obs[color].to_numpy()
     else:
         groups = color
         color = "color"
     
-    if sample_size is not None and adata.shape[0] > sample_size:
-        idx = np.random.choice(adata.shape[0], sample_size, replace=False)
+    if sample_size is not None and embedding.shape[0] > sample_size:
+        idx = np.random.choice(embedding.shape[0], sample_size, replace=False)
         embedding = embedding[idx, :]
         if groups is not None: groups = groups[idx]
 
     if groups is not None:
         idx = index_natsorted(groups)
         embedding = embedding[idx, :]
         groups = [groups[i] for i in idx]
```

### Comparing `snapatac2-2.6.0/python/snapatac2/plotting/_base.py` & `snapatac2-2.6.1/python/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/datasets.py` & `snapatac2-2.6.1/python/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/_io.py` & `snapatac2-2.6.1/python/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/genome.py` & `snapatac2-2.6.1/python/snapatac2/genome.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,16 @@
     chrom_sizes= {"chr1": 248956422, "chr2": 242193529, "chr3": 198295559,
                   "chr4": 190214555, "chr5": 181538259, "chr6": 170805979,
                   "chr7": 159345973, "chr8": 145138636, "chr9": 138394717,
                   "chr10": 133797422, "chr11": 135086622, "chr12": 133275309,
                   "chr13": 114364328, "chr14": 107043718, "chr15": 101991189,
                   "chr16": 90338345, "chr17": 83257441, "chr18": 80373285,
                   "chr19": 58617616, "chr20": 64444167, "chr21": 46709983,
-                  "chr22": 50818468, "chrX": 156040895, "chrY": 57227415},
+                  "chr22": 50818468, "chrX": 156040895, "chrY": 57227415,
+                  "chrM": 16569 },
     )
 hg38 = GRCh38
 
 GRCm39 = Genome(
     fasta=lambda : datasets().fetch(
         "gencode_vM30_GRCm39.fa.gz", processor=Decompress(method = "gzip"), progressbar=True),
     annotation=lambda : datasets().fetch(
@@ -157,14 +158,15 @@
         "chr15": 104073951,
         "chr16": 98008968,
         "chr17": 95294699,
         "chr18": 90720763,
         "chr19": 61420004,
         "chrX": 169476592,
         "chrY": 91455967,
+        "chrM": 16299,
     },
     )
 mm39 = GRCm39
 
 GRCm38 = Genome(
     fasta=lambda : datasets().fetch(
         "gencode_vM25_GRCm38.fa.gz", processor=Decompress(method = "gzip"), progressbar=True),
@@ -188,10 +190,11 @@
         "chr15": 104043685,
         "chr16": 98207768,
         "chr17": 94987271,
         "chr18": 90702639,
         "chr19": 61431566,
         "chrX": 171031299,
         "chrY": 91744698,
+        "chrM": 16299,
     },
     )
 mm10 = GRCm38
```

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_call_peaks.py` & `snapatac2-2.6.1/python/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_network.py` & `snapatac2-2.6.1/python/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_embedding.py` & `snapatac2-2.6.1/python/snapatac2/tools/_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 def umap(
     adata: internal.AnnData | internal.AnnDataSet | np.ndarray,
     n_comps: int = 2,
     use_dims: int | list[int] | None = None,
     use_rep: str = "X_spectral",
     key_added: str = 'umap',
-    random_state: int = 0,
+    random_state: int | None = 0,
     inplace: bool = True,
     **kwargs
 ) -> np.ndarray | None:
     """
     Parameters
     ----------
     adata
@@ -95,15 +95,19 @@
     np.ndarray | None
         if `inplace=True` it stores UMAP embedding in
         `adata.obsm["X_`key_added`"]`.
         Otherwise, it returns the result as a numpy array.
     """
     from umap import UMAP
 
-    data = adata.obsm[use_rep] if is_anndata(adata) else adata
+    if is_anndata(adata):
+        data = adata.obsm[use_rep]
+    else:
+        data = adata
+        inplace = False
 
     if use_dims is not None:
         data = data[:, :use_dims] if isinstance(use_dims, int) else data[:, use_dims]
 
     umap = UMAP(random_state=random_state,
                 n_components=n_comps,
                 **kwargs).fit_transform(data)
```

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_motif.py` & `snapatac2-2.6.1/python/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_integration.py` & `snapatac2-2.6.1/python/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_smooth.py` & `snapatac2-2.6.1/python/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_diff.py` & `snapatac2-2.6.1/python/snapatac2/tools/_diff.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_misc.py` & `snapatac2-2.6.1/python/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/tools/_clustering.py` & `snapatac2-2.6.1/python/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/__init__.py` & `snapatac2-2.6.1/python/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/_utils.py` & `snapatac2-2.6.1/python/snapatac2/_utils.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/python/snapatac2/metrics/__init__.py` & `snapatac2-2.6.1/python/snapatac2/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/LICENSE` & `snapatac2-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.0/PKG-INFO` & `snapatac2-2.6.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapatac2
-Version: 2.6.0
+Version: 2.6.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: anndata >=0.8.0, <0.11.0
 Requires-Dist: kaleido
 Requires-Dist: multiprocess
@@ -19,27 +19,25 @@
 Requires-Dist: pyarrow
 Requires-Dist: pyfaidx >=0.7.0, <0.8.0
 Requires-Dist: rustworkx
 Requires-Dist: scipy >=1.4, <2.0.0
 Requires-Dist: scikit-learn >=1.0, <2.0.0
 Requires-Dist: tqdm >=4.62
 Requires-Dist: typing-extensions
-Requires-Dist: scanorama >=1.7.3 ; extra == 'extra'
-Requires-Dist: harmonypy >=0.0.9 ; extra == 'extra'
-Requires-Dist: xgboost >=1.4 ; extra == 'extra'
-Requires-Dist: umap-learn >=0.5.0 ; extra == 'extra'
+Requires-Dist: scanorama >=1.7.3 ; extra == 'recommend'
+Requires-Dist: harmonypy >=0.0.9 ; extra == 'recommend'
+Requires-Dist: xgboost >=1.4 ; extra == 'recommend'
+Requires-Dist: umap-learn >=0.5.0 ; extra == 'recommend'
 Requires-Dist: scanpy >=1.9 ; extra == 'recommend'
 Requires-Dist: scvi-tools >=1.0 ; extra == 'recommend'
-Requires-Dist: snapatac2[extra] ; extra == 'all'
-Requires-Dist: snapatac2[recommend] ; extra == 'all'
+Requires-Dist: scikit-misc >=0.1.3 ; extra == 'recommend'
+Requires-Dist: magic-impute >=2.0 ; extra == 'recommend'
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: hypothesis ==6.72.4 ; extra == 'test'
-Provides-Extra: extra
 Provides-Extra: recommend
-Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
 Summary: SnapATAC2: Single-cell epigenomics analysis pipeline
 Keywords: single-cell,biology
 Home-Page: https://github.com/
 Author: Kai Zhang <kai@kzhang.org>
 Author-email: Kai Zhang <zhangkai33@westlake.edu.cn>
```

