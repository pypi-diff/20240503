# Comparing `tmp/finaletoolkit-0.5.0.tar.gz` & `tmp/finaletoolkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finaletoolkit-0.5.0.tar", last modified: Tue Apr 30 16:32:48 2024, max compression
+gzip compressed data, was "finaletoolkit-0.5.1.tar", last modified: Fri May  3 19:00:44 2024, max compression
```

## Comparing `finaletoolkit-0.5.0.tar` & `finaletoolkit-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletoolkit-0.5.0/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5940 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3765 2024-04-30 16:24:40.000000 finaletoolkit-0.5.0/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1065 2024-04-30 16:27:58.000000 finaletoolkit-0.5.0/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5940 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1143 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       61 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       14 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 finaletoolkit-0.5.0/src/finaletoolkit/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       40 2024-04-30 16:19:15.000000 finaletoolkit-0.5.0/src/finaletoolkit/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    28006 2024-04-30 16:19:12.000000 finaletoolkit-0.5.0/src/finaletoolkit/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      594 2024-04-30 16:18:16.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9666 2024-04-30 16:18:31.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/agg_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9331 2024-04-30 16:18:27.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7555 2024-04-30 16:16:30.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14535 2024-04-30 16:16:28.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2587 2024-04-30 16:16:29.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    29186 2024-04-30 16:17:22.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14869 2024-04-30 16:17:21.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8468 2024-04-30 16:17:54.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6801 2024-04-30 16:17:19.000000 finaletoolkit-0.5.0/src/finaletoolkit/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       39 2024-04-30 16:17:53.000000 finaletoolkit-0.5.0/src/finaletoolkit/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14341 2024-04-30 16:18:04.000000 finaletoolkit-0.5.0/src/finaletoolkit/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletoolkit-0.5.0/src/finaletoolkit/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletoolkit-0.5.0/src/finaletoolkit/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletoolkit-0.5.0/src/finaletoolkit/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 16:32:48.000000 finaletoolkit-0.5.0/src/finaletoolkit/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       94 2024-04-30 16:31:22.000000 finaletoolkit-0.5.0/src/finaletoolkit/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 finaletoolkit-0.5.0/src/finaletoolkit/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 finaletoolkit-0.5.0/src/finaletoolkit/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-24 03:28:21.000000 finaletoolkit-0.5.0/src/finaletoolkit/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletoolkit-0.5.1/LICENSE
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5986 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3765 2024-04-30 18:09:21.000000 finaletoolkit-0.5.1/README.md
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1131 2024-05-03 18:47:49.000000 finaletoolkit-0.5.1/pyproject.toml
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/setup.cfg
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5986 2024-05-03 18:52:33.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1143 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       61 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       14 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/finaletoolkit/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:40.000000 finaletoolkit-0.5.1/src/finaletoolkit/cli/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       40 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/cli/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    28006 2024-05-03 16:46:05.000000 finaletoolkit-0.5.1/src/finaletoolkit/cli/main_cli.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      547 2024-04-30 19:02:33.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9703 2024-04-30 18:27:49.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/adjust_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9331 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/cleavage_profile.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7555 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/coverage.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14535 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_gc_correct.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2587 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_merge_bins.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    29309 2024-05-03 16:40:30.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14869 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/frag_length.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8468 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/multi_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6801 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/frag/wps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/genome/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       39 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/genome/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    15108 2024-04-30 19:31:47.000000 finaletoolkit-0.5.1/src/finaletoolkit/genome/gaps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/methylation/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/methylation/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/qc/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/qc/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/too/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/too/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-03 19:00:44.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      139 2024-04-30 19:02:29.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4889 2024-04-30 19:03:05.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/agg_bw.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/cli_hist.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3195 2024-04-30 19:59:51.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/filter_bam.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-30 18:09:22.000000 finaletoolkit-0.5.1/src/finaletoolkit/utils/utils.py
```

### Comparing `finaletoolkit-0.5.0/LICENSE` & `finaletoolkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/PKG-INFO` & `finaletoolkit-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FinaleToolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
-Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
+Author-email: James Li <lijw21@wfu.edu>, Ravi Bandaru <ravi.bandaru@northwestern.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `finaletoolkit-0.5.0/README.md` & `finaletoolkit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/pyproject.toml` & `finaletoolkit-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleToolkit"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
+    {name="Ravi Bandaru", email="ravi.bandaru@northwestern.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/PKG-INFO` & `finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FinaleToolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
-Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
+Author-email: James Li <lijw21@wfu.edu>, Ravi Bandaru <ravi.bandaru@northwestern.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `finaletoolkit-0.5.0/src/FinaleToolkit.egg-info/SOURCES.txt` & `finaletoolkit-0.5.1/src/FinaleToolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/FinaleToolkit.egg-info/requires.txt
 src/FinaleToolkit.egg-info/top_level.txt
 src/finaletoolkit/__init__.py
 src/finaletoolkit/cli/__init__.py
 src/finaletoolkit/cli/main_cli.py
 src/finaletoolkit/frag/__init__.py
 src/finaletoolkit/frag/adjust_wps.py
-src/finaletoolkit/frag/agg_wps.py
 src/finaletoolkit/frag/cleavage_profile.py
 src/finaletoolkit/frag/coverage.py
 src/finaletoolkit/frag/delfi.py
 src/finaletoolkit/frag/delfi_gc_correct.py
 src/finaletoolkit/frag/delfi_merge_bins.py
 src/finaletoolkit/frag/end_motifs.py
 src/finaletoolkit/frag/frag_length.py
@@ -24,10 +23,11 @@
 src/finaletoolkit/frag/wps.py
 src/finaletoolkit/genome/__init__.py
 src/finaletoolkit/genome/gaps.py
 src/finaletoolkit/methylation/__init__.py
 src/finaletoolkit/qc/__init__.py
 src/finaletoolkit/too/__init__.py
 src/finaletoolkit/utils/__init__.py
+src/finaletoolkit/utils/agg_bw.py
 src/finaletoolkit/utils/cli_hist.py
 src/finaletoolkit/utils/filter_bam.py
 src/finaletoolkit/utils/utils.py
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/cli/main_cli.py` & `finaletoolkit-0.5.1/src/finaletoolkit/cli/main_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from __future__ import annotations
 import argparse
 
 from finaletoolkit.frag.frag_length import (
     _cli_frag_length, frag_length_bins, frag_length_intervals
 )
+from finaletoolkit.utils.agg_bw import agg_bw
 from finaletoolkit.utils.filter_bam import filter_bam
 from finaletoolkit.frag.coverage import coverage
 from finaletoolkit.frag.multi_wps import multi_wps
 from finaletoolkit.frag.delfi import delfi
 from finaletoolkit.frag.adjust_wps import adjust_wps
-from finaletoolkit.frag.agg_wps import agg_wps
 from finaletoolkit.frag.delfi_gc_correct import cli_delfi_gc_correct
 from finaletoolkit.frag.end_motifs import (
     end_motifs, _cli_mds, _cli_interval_mds, interval_end_motifs)
 from finaletoolkit.frag.cleavage_profile import _cli_cleavage_profile
 from finaletoolkit.genome.gaps import _cli_gap_bed
 
 # TODO: implement subcommands read from stdin
@@ -542,24 +542,24 @@
         '-v',
         '--verbose',
         action='count',
         help='Specify verbosity. Number of printed statements is proportional to number of vs.'
     )
     parser_command7.set_defaults(func=adjust_wps)
 
-    # Subcommand 8: aggregate WPS
+    # Subcommand 8: aggregate BigWig/WPS
     parser_command8 = subparsers.add_parser(
-        'agg-wps',
+        'agg-bw',
         prog='finaletoolkit-agg-wps',
-        description='Reads WPS data from a WIG file and aggregates over'
+        description='Reads data from a BigWig file and aggregates over'
         ' intervals in a BED file.'
     )
     parser_command8.add_argument(
         'input_file',
-        help='BigWig file with WPS data.'
+        help='BigWig file with data.'
     )
     parser_command8.add_argument(
         'interval_file',
         help='BED file containing intervals over which wps was calculated'
     )
     parser_command8.add_argument(
         '-o',
@@ -577,15 +577,15 @@
     )
     parser_command8.add_argument(
         '-v',
         '--verbose',
         action='count',
         help='Specify verbosity. Number of printed statements is proportional to number of vs.'
     )
-    parser_command8.set_defaults(func=agg_wps)
+    parser_command8.set_defaults(func=agg_bw)
 
     # Subcommand 9: delfi gc correct
     parser_command9 = subparsers.add_parser(
         'delfi-gc-correct',
         prog='finaletoolkit-delfi-gc-correct',
         description='Performs gc-correction on raw delfi data.'
     )
@@ -784,15 +784,15 @@
         default='-',
         help='Tab-delimited or similar file containing one column for all '
         'k-mers a one column for frequency. Reads from stdin by default.'
     )
     parser_command11a.add_argument(
         '-s',
         '--sep',
-        default=',',
+        default='\t',
         help='Separator used in tabular file. Default is tab.'
     )
     parser_command11a.add_argument(
         'file_out',
         default='-'
     )
     parser_command11a.set_defaults(func=_cli_interval_mds)
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/__init__.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,9 +3,8 @@
 from finaletoolkit.frag.wps import wps
 from finaletoolkit.frag.multi_wps import multi_wps
 from finaletoolkit.frag.cleavage_profile import cleavage_profile
 from finaletoolkit.frag.delfi import delfi
 from finaletoolkit.frag.delfi_gc_correct import delfi_gc_correct
 from finaletoolkit.frag.delfi_merge_bins import delfi_merge_bins
 from finaletoolkit.frag.adjust_wps import adjust_wps
-from finaletoolkit.frag.agg_wps import agg_wps
 from finaletoolkit.frag.end_motifs import *
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/adjust_wps.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/adjust_wps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from sys import stdin, stdout, stderr
 from typing import TextIO, Union
 from multiprocessing import Pool
 from time import time
 import traceback
+import gzip
 
 import numpy as np
 from numpy.typing import NDArray
 import pyBigWig as pbw
 from scipy.signal import savgol_filter
 
 from finaletoolkit.utils import genome2list
@@ -58,14 +59,15 @@
         start: int,
         stop: int,
         median_window_size: int=1000,
         savgol_window_size: int=21,
         savgol_poly_deg: int=2,
         mean: bool=False,
         subtract_edges: bool=False,
+        edge_size: int=500,
 ):
     """
     Takes a wps WIG file and applies a median filter and a Savitsky-
     Golay filter (Savitsky and Golay, 1964) on it. Also returns
     positions for the window (which is truncated by the median filter).
     """
 
@@ -99,15 +101,14 @@
                 'multiple entries for one position or gaps in the '
                 'regions specified in the interval file.'
             )
 
         # adjusting/filtering
         if subtract_edges:
             # TODO: add option for edge size
-            edge_size = 500
             start_mean = np.mean(intervals['scores'][:edge_size])
             stop_mean = np.mean(intervals['scores'][-edge_size:])
             mean = np.mean([start_mean, stop_mean])
             intervals['scores'] = intervals['scores'] - mean
 
         if not mean:
             adjusted_positions, adjusted_scores = _median_filter(
@@ -150,14 +151,15 @@
     output_file: str,
     genome_file: str,
     median_window_size: int=1000,
     savgol_window_size: int=21,
     savgol_poly_deg: int=2,
     mean: bool=False,
     subtract_edges: bool=False,
+    edge_size: int=500,
     workers: int=1,
     verbose: Union(bool, int)=False
 ):
     """
     Adjusts raw WPS data in a BigWig by applying a median filter and
     Savitsky-Golay filter (Savitsky and Golay, 1964).
 
@@ -193,22 +195,21 @@
 
     """
     if verbose:
         start_time = time()
         stderr.write('Reading intervals from bed...\n')
 
     # read intervals
-    # TODO: add support for bedgz
     if interval_file.endswith('.bed') or interval_file.endswith('.bed.gz'):
         # amount taken by median filter
         end_decrease = median_window_size//2
-        if interval_file.endswith('.gz'):
-            raise NotImplementedError('bed.gz not supported yet')
         intervals = []
-        with open(interval_file, 'r') as file:
+        with (gzip.open(interval_file, 'rt')
+              if interval_file.endswith('.gz')
+              else open(interval_file, 'rt')) as file:
             for line in file:
                 # read segment from BED
                 contents = line.split('\t')
                 contig = contents[0].strip()
                 start = int(contents[1])
                 stop = int(contents[2])
 
@@ -232,20 +233,22 @@
                     int(start),
                     int(stop),
                     median_window_size,
                     savgol_window_size,
                     savgol_poly_deg,
                     mean,
                     subtract_edges,
+                    edge_size,
                 ))
     else:
         raise ValueError('Invalid filetype for interval_file.')
 
     if verbose:
-        stderr.write('Opening pool\n')
+        stderr.write('Opening pool...\n')
+        
     try:
         # use pool of processes to process wps scores into an iterator
         pool = Pool(workers)
         processed_scores = pool.imap(_single_adjust_wps_star, intervals)
 
         if verbose:
             stderr.write('Writing to output\n')
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/agg_wps.py` & `finaletoolkit-0.5.1/src/finaletoolkit/utils/agg_bw.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 from sys import stdin, stdout, stderr
 from typing import Union
 import time
 
 import numpy as np
 import pyBigWig as pbw
 
-def agg_wps(
+def agg_bw(
     input_file: str,
     interval_file: str,
     output_file: str,
     median_window_size: int=0,
-    verbose: Union[bool, int]=False
+    mean: bool=False,
+    strand_location: int=5,
+    verbose: bool=False
 ):
     """
-    Takes a BigWig containing adjusted WPS scores and an interval BED and
-    aggregates scores along the intervals.
+    Takes a BigWig and an interval BED and
+    aggregates signal along the intervals.
+
+    For aggregating WPS signals, note that the median filter trims the
+    ends of each interval by half of the window size of the filter
+    while adjusting data. There are two way this can be approached in
+    aggregation:
 
-    Note that the median filter trims the ends of each interval by half
-    of the window size of the filter while adjusting raw WPS data. There
-    are two way this can be approached in aggregation:
     1. supply an interval file containing smaller intervals. e.g. if
     you used 5kb intervals for WPS and used a median filter window
     of 1kb, supply a BED file with 4kb windows to this function.
 
     2. provide the size of the median filter window in
     `median_window_size` along with the original intervals. e.g if
     5kb intervals were used for WPS and a 1kb median filter window
@@ -35,93 +39,109 @@
     Parameters
     ----------
     input_file : str
     interval_file : str
     output_file : str
     median_window_size : int, optional
         default is 0
+    mean : bool
+        use mean instead
+    strand_location : int
+        which column (starting at 0) of the interval file contains the
+        strand. Default is 5.
     verbose : int or bool, optional
         default is False
 
     Return
     ------
     agg_scores : NDArray
     """
     if verbose:
         start_time = time.time()
         stderr.write('Reading intervals from bed...\n')
 
     # reading intervals from interval_file into a list
     if interval_file.endswith('.bed') or interval_file.endswith('.bed.gz'):
-        # TODO: add support for bed.gz
-        if interval_file.endswith('.gz'):
-            raise NotImplementedError('bed.gz not supported yet')
         intervals = []
-        with open(interval_file, 'r') as file:
+        with (gzip.open(interval_file, 'rt')
+              if interval_file.endswith('.gz')
+              else open(interval_file, 'rt')) as file:
             for line in file:
                 # read segment from BED
                 contents = line.split('\t')
                 contig = contents[0]
                 start = int(contents[1])
                 stop = int(contents[2])
-                strand = contents[5]
+                strand = contents[strand_location]
 
                 intervals.append((
                     contig,
                     int(start),
                     int(stop),
                     strand.strip(),
                 ))
     else:
         raise ValueError('Invalid filetype for interval_file.')
 
     with pbw.open(input_file, 'r') as raw_wps:
         # get size of interval based on first entry in interval_file
         interval_size = intervals[0][2] - intervals[0][1] - median_window_size
         agg_scores = np.zeros(interval_size, dtype=np.int64)
-        # HACK: excepting for random intervals with wrong size or improperly
-        # formatted BigWigs
+        num_intervals_added = 0
         for contig, start, stop, strand in intervals:
             try:
-                values = np.array(raw_wps.values(contig, start, stop))
+                signal = raw_wps.values(contig, start, stop)
+                if signal==None:
+                    print("There was no information found in the interval: ", contig, start, stop)
+                    continue
+                values = np.nan_to_num(np.array(signal), nan=0)
             except RuntimeError as e:
                 print(e)
                 continue
+
             # trimmed from median filter
             trimmed = values[median_window_size//2:-median_window_size//2]
             if trimmed.shape[0] != interval_size:
                 print(f"Trimmed size {trimmed.shape[0]} is not equal to interval size {interval_size}. Skipping.")
                 continue
+
             # flip scores if on reverse strand
             if strand == '+':
                 agg_scores = agg_scores + trimmed
+                num_intervals_added+=1
             elif strand == '-':
                 agg_scores = agg_scores + np.flip(trimmed)
+                num_intervals_added+=1
             elif verbose:
                 stderr.write(
                     'A segment without strand was encountered. Skipping.'
                 )
-    positions = np.arange(-interval_size//2, interval_size//2)
+
+    if mean:
+        agg_scores = agg_scores/num_intervals_added
+
     if output_file.endswith('wig'):
         with open(output_file, 'wt') as out:
             if (verbose):
                 stderr.write(f'File opened! Writing...\n')
             # declaration line
             out.write(
                 f'fixedStep\tchrom=.\tstart={-interval_size//2}\tstep={1}\tspan'
                 f'={interval_size}\n'
             )
             for score in agg_scores:
                 out.write(f'{score}\n')
     else:
         raise ValueError(
-            'output_file is unaccepted type.'
+            'The output_file is an unaccepted type. Must be a wiggle file '
+            'ending in .wig'
         )
     
     if verbose:
         end_time = time.time()
-        stderr.write(f'Agg-WPS took {end_time-start_time} s to run.\n')
+        stderr.write(f'Aggregating bigWig took {end_time-start_time} s '
+                     'to run.\n')
 
     return agg_scores
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/cleavage_profile.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/coverage.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/coverage.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/delfi.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/delfi_gc_correct.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/delfi_merge_bins.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/delfi_merge_bins.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/end_motifs.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/end_motifs.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         """
         Calculates a motif diversity score (MDS) using normalized
         Shannon entropy as described by Jiang et al (2020). This
         function is generalized for any k instead of just 4-mers.
         """
         num_kmers = 4**self.k
         freq = np.array(self.frequencies())
-        mds = np.sum(-freq*np.log(freq)/np.log(num_kmers))
+        # if freq is 0, ignore
+        mds = np.sum(-freq*np.nan_to_num(np.log(freq), neginf=0)/np.log(num_kmers))
 
         return mds
 
     @classmethod
     def from_file(
             cls,
             file_path: str,
@@ -283,15 +284,17 @@
         function is generalized for any k instead of just 4-mers.
         """
         num_kmers = 4**self.k
         mds = []
         for interval, kmers in self.intervals:
             freq = np.array(list(kmers.values()))
             try:
-                interval_mds = np.sum(-freq*np.log(freq))/np.log(num_kmers)
+                interval_mds = np.sum(
+                    -freq*np.nan_to_num(np.log(freq), neginf=0)
+                    )/np.log(num_kmers)
             except RuntimeWarning:
                 interval_mds = np.NaN
             mds.append((interval, interval_mds))
         return mds
 
     def mds_bed(self, output_file: str, sep: str='\t'):
         """Writes MDS for each interval to a bed/bedgraph file."""
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/frag_length.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/multi_wps.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/frag/wps.py` & `finaletoolkit-0.5.1/src/finaletoolkit/frag/wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/genome/gaps.py` & `finaletoolkit-0.5.1/src/finaletoolkit/genome/gaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 import numpy as np
 from numpy.typing import NDArray
 
 import finaletoolkit.genome as genome
 
 HG19GAPS: Path = (files(genome) / 'data' / 'hg19.gap.txt.gz')
-HG38GAPS: Path = (files(genome) / 'data' / 'hg19.gap.txt.gz')
-HG38CENTROMERES: Path = (files(genome) / 'data' / 'hg38.centromeres.txt.gz')
+HG38GAPS: Path = (files(genome) / 'data' / 'hg38.gap.txt.gz')
 
 
 class GenomeGaps:
     """
     Reads telomere, centromere, and short_arm intervals from a bed file
     or generates these intervals from UCSC gap and centromere tracks for
     hg19 and hg38.
@@ -117,16 +116,41 @@
         genome_gaps.telomeres = gaps[gaps['type'] == 'telomere']
         genome_gaps.short_arms = gaps[gaps['type'] == 'short_arm']
         genome_gaps.gaps = gaps
 
         return genome_gaps
 
     @classmethod
-    def ucsc_hg38(cls):
-        return NotImplemented
+    def hg38(cls):
+        """
+        Creates a GenomeGaps for the hg38 reference genome. This
+        sequences uses chromosome names that start with 'chr' and is
+        synonymous with the GRCh38 reference genome.
+        Returns
+        -------
+        gaps : GenomeGaps
+            GenomeGaps for the hg38 reference genome.
+        """
+        genome_gaps = cls()
+        gaps = np.genfromtxt(
+            HG38GAPS,
+            usecols=[1, 2, 3, 7],
+            dtype=[
+                ('contig', '<U32'),
+                ('start', '<i8'),
+                ('stop', '<i8'),
+                ('type', '<U32'),
+            ]
+        )
+        genome_gaps.centromeres = gaps[gaps['type'] == 'centromere']
+        genome_gaps.telomeres = gaps[gaps['type'] == 'telomere']
+        genome_gaps.short_arms = gaps[gaps['type'] == 'short_arm']
+        genome_gaps.gaps = gaps
+
+        return genome_gaps
 
     def in_tcmere(self, contig: str, start: int, stop: int) -> bool:
         """
         Checks if specified interval is in a centromere or telomere
 
         Parameters
         ----------
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/utils/cli_hist.py` & `finaletoolkit-0.5.1/src/finaletoolkit/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/utils/filter_bam.py` & `finaletoolkit-0.5.1/src/finaletoolkit/utils/filter_bam.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 import traceback
 from sys import stderr
 from os.path import isdir
 from shutil import rmtree
 
 import pysam
 
-
-
 def filter_bam(
         input_file: str,
         region_file: str=None,
         output_file: str=None,
-        fraction_high: int=None,
-        fraction_low: int=None,
+        max_length: int=None,
+        min_length: int=None,
         quality_threshold: int=30,
         workers: int=1,
         verbose: bool=False):
     """
     Accepts the path to a BAM file and creates a bam file where all
     reads are read1 in a proper pair, exceed the specified quality
     threshold, do not intersect a region in the given blacklist
@@ -28,93 +26,74 @@
     Parameters
     ----------
     input_bam : str
         Path string or AlignmentFile pointing to the BAM file to be
         filtered.
     region_file : str, option
     output_file : str, optional
+    min_length : int, optional
+    max_length : int, optional
     quality_threshold : int, optional
     workers : int, optional
     verbose : bool, optional
 
     Returns
     -------
     output_file : str
     """
 
     # create tempfile to contain filtered bam
     if output_file is None:
         _, output_file = tf.mkstemp(suffix='.bam')
-    elif output_file.endswith('bam') or output_file == '-':
-        pass
-    else:
-        raise ValueError('output_file should have suffix .bam')
+    elif not output_file.endswith('bam') and output_file != '-':
+        raise ValueError('Output file should have suffix .bam')
 
 
         # create temp dir to store intermediate sorted file
     try:
-        temp_dir = tf.TemporaryDirectory()
-
-        flag_filtered_bam = temp_dir.name + '/flag_filtered.bam'
-
-        samtools_command = (
-            f'samtools view {input_file} -F 3852 -f 66 -b -h -o '
-            f'{flag_filtered_bam} -q {quality_threshold} -@ {workers}'
-        )
-
-        if region_file is not None:
-            samtools_command += f' -M -L {region_file}'
-
-        try:
-            process1 = subprocess.run(samtools_command, shell=True, check=True)
-        except Exception as e:
-            traceback.print_exc()
-            exit(1)
+        with tf.TemporaryDirectory() as temp_dir:
+            flag_filtered_bam = f'{temp_dir}/flag_filtered.bam'
+            samtools_command = (
+                f'samtools view {input_file} -F 3852 -f 66 -b -h -o '
+                f'{flag_filtered_bam} -q {quality_threshold} -@ {workers}'
+            )
 
-        # supress index file warning
-        save = pysam.set_verbosity(0)
+            if region_file is not None:
+                samtools_command += f' -M -L {region_file}'
 
-        # filter for reads on different reference
-        with pysam.AlignmentFile(flag_filtered_bam, 'rb') as in_file:
-            with pysam.AlignmentFile(
-                output_file,
-                'wb',
-                template=in_file
-            ) as out_file:
-                if fraction_high is None and fraction_low is None:
+            try:
+                subprocess.run(samtools_command, shell=True, check=True)
+            except Exception:
+                traceback.print_exc()
+                exit(1)
+
+            # suppress index file warning
+            save = pysam.set_verbosity(0)
+
+            # filter for reads on different reference
+            with pysam.AlignmentFile(flag_filtered_bam, 'rb') as in_file:
+                with pysam.AlignmentFile(
+                    output_file, 'wb', template=in_file) as out_file:
                     for read in in_file:
-                        if read.reference_name == read.next_reference_name:
-                            out_file.write(read)
-                elif fraction_high is None:
-                    for read in in_file:
-                        if (read.reference_name == read.next_reference_name
-                            and read.template_length >= fraction_low
-                        ):
-                            out_file.write(read)
-                elif fraction_low is None:
-                    for read in in_file:
-                        if (read.reference_name == read.next_reference_name
-                            and read.template_length <= fraction_high
-                        ):
-                            out_file.write(read)
-                else:
-                    for read in in_file:
-                        if (read.reference_name == read.next_reference_name
-                            and read.template_length >= fraction_low
-                            and read.template_length <= fraction_high
+                        if (
+                            read.reference_name == read.next_reference_name
+                            and (max_length is None
+                                 or read.template_length <= max_length)
+                            and (min_length is None
+                                 or read.template_length >= min_length)
                         ):
                             out_file.write(read)
+
     finally:
-        temp_dir.cleanup()
         pysam.set_verbosity(save)
 
     if output_file != '-':
         # generate index for output_file
         try:
-            process3 = subprocess.run(
+            subprocess.run(
                 f'samtools index {output_file} {output_file}.bai',
                 shell=True,
                 check=True
             )
-        except Exception as e:
+        except Exception:
             traceback.print_exc()
             exit(1)
```

### Comparing `finaletoolkit-0.5.0/src/finaletoolkit/utils/utils.py` & `finaletoolkit-0.5.1/src/finaletoolkit/utils/utils.py`

 * *Files identical despite different names*

