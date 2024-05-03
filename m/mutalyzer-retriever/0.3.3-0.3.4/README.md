# Comparing `tmp/mutalyzer_retriever-0.3.3.tar.gz` & `tmp/mutalyzer_retriever-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutalyzer_retriever-0.3.3.tar", last modified: Tue Jan 30 14:22:04 2024, max compression
+gzip compressed data, was "mutalyzer_retriever-0.3.4.tar", last modified: Fri May  3 07:50:38 2024, max compression
```

## Comparing `mutalyzer_retriever-0.3.3.tar` & `mutalyzer_retriever-0.3.4.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-30 14:22:04.696843 mutalyzer_retriever-0.3.3/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1778 2024-01-30 14:22:04.696843 mutalyzer_retriever-0.3.3/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1059 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-30 14:22:04.692843 mutalyzer_retriever-0.3.3/mutalyzer_retriever/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      765 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5784 2024-01-30 12:18:12.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1893 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/configuration.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      688 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/parser.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-30 14:22:04.692843 mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       17 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      378 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/fasta.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12453 2024-01-30 14:19:22.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/gff3.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6582 2021-07-23 07:32:49.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/lrg.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3284 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/reference.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10322 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/related.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      996 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/request.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12786 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/retriever.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      638 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/schema_validation.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-30 14:22:04.692843 mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4372 2024-01-30 14:19:37.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/ensembl.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2756 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/lrg.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6127 2023-08-03 15:10:07.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/ncbi.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    15125 2024-01-30 13:16:35.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/ncbi_assemblies.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      612 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever/util.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-30 14:22:04.692843 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1778 2024-01-30 14:22:04.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1085 2024-01-30 14:22:04.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-01-30 14:22:04.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2024-01-30 14:22:04.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/entry_points.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       64 2024-01-30 14:22:04.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       20 2024-01-30 14:22:04.000000 mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1187 2024-01-30 14:22:04.696843 mutalyzer_retriever-0.3.3/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.3/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-30 14:22:04.692843 mutalyzer_retriever-0.3.3/tests/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4121 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.3/tests/test_cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2739 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.3/tests/test_fetch.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2690 2024-01-29 14:32:51.000000 mutalyzer_retriever-0.3.3/tests/test_model_validation.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2609 2021-10-14 13:27:57.000000 mutalyzer_retriever-0.3.3/tests/test_related.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2852 2024-01-29 14:32:46.000000 mutalyzer_retriever-0.3.3/tests/test_retriever_model.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1480 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      761 2024-01-31 08:29:20.000000 mutalyzer_retriever-0.3.4/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-03 07:50:38.882897 mutalyzer_retriever-0.3.4/mutalyzer_retriever/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      765 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5816 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/cli.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1948 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/configuration.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      791 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parser.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       17 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      378 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/fasta.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12453 2024-01-30 14:19:22.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/gff3.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5209 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/json_ensembl.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6582 2021-07-23 07:32:49.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/lrg.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3284 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/reference.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10322 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/related.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      996 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/request.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13255 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/retriever.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      638 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/schema_validation.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5419 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/ensembl.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2756 2022-06-03 13:11:00.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/lrg.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6753 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/ncbi.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    15125 2024-01-30 13:16:35.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/ncbi_assemblies.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      612 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever/util.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     1480 2024-05-03 07:50:38.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1182 2024-05-03 07:50:38.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-05-03 07:50:38.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2024-05-03 07:50:38.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/entry_points.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       64 2024-05-03 07:50:38.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       26 2024-05-03 07:50:38.000000 mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1187 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-03 07:50:38.886898 mutalyzer_retriever-0.3.4/tests/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/tests/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4465 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/tests/commons.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      164 2021-07-22 13:18:05.000000 mutalyzer_retriever-0.3.4/tests/conftest.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4121 2023-01-10 12:34:41.000000 mutalyzer_retriever-0.3.4/tests/test_cli.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2171 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/tests/test_fetch.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2025 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/tests/test_model_validation.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2609 2021-10-14 13:27:57.000000 mutalyzer_retriever-0.3.4/tests/test_related.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1585 2024-05-02 13:17:56.000000 mutalyzer_retriever-0.3.4/tests/test_retriever_model.py
```

### Comparing `mutalyzer_retriever-0.3.3/LICENSE` & `mutalyzer_retriever-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/PKG-INFO` & `mutalyzer_retriever-0.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer_retriever
-Version: 0.3.3
+Version: 0.3.4
 Summary: Mutalyzer genomic reference retriever.
 Home-page: https://github.com/mutalyzer/retriever
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,reference,retriever,genomic
 Classifier: Intended Audience :: Science/Research
@@ -18,18 +18,15 @@
 Requires-Dist: bcbio-gff>=0.7.1
 Requires-Dist: requests>=2.26.0
 Requires-Dist: schema>=0.7.4
 
 # Mutalyzer Retriever
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/mutalyzer/retriever)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/mutalyzer/retriever/Python%20package%20CI)
 ![Read the Docs](https://img.shields.io/readthedocs/mutalyzer-retriever)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/mutalyzer/retriever)
-![GitHub Release Date](https://img.shields.io/github/release-date/mutalyzer/retriever)
 ![PyPI](https://img.shields.io/pypi/v/mutalyzer_retriever)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/mutalyzer/retriever)
 ![GitHub language count](https://img.shields.io/github/languages/count/mutalyzer/retriever)
 ![GitHub top language](https://img.shields.io/github/languages/top/mutalyzer/retriever)
 ![GitHub](https://img.shields.io/github/license/mutalyzer/retriever)
 
 ---
```

### Comparing `mutalyzer_retriever-0.3.3/README.md` & `mutalyzer_retriever-0.3.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # Mutalyzer Retriever
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/mutalyzer/retriever)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/mutalyzer/retriever/Python%20package%20CI)
 ![Read the Docs](https://img.shields.io/readthedocs/mutalyzer-retriever)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/mutalyzer/retriever)
-![GitHub Release Date](https://img.shields.io/github/release-date/mutalyzer/retriever)
 ![PyPI](https://img.shields.io/pypi/v/mutalyzer_retriever)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/mutalyzer/retriever)
 ![GitHub language count](https://img.shields.io/github/languages/count/mutalyzer/retriever)
 ![GitHub top language](https://img.shields.io/github/languages/top/mutalyzer/retriever)
 ![GitHub](https://img.shields.io/github/license/mutalyzer/retriever)
 
 ---
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/__init__.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/cli.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     )
 
     parser.add_argument("-v", action="version", version=version(parser.prog))
 
     parser.add_argument("--id", help="the reference id")
 
     parser.add_argument(
-        "-s", "--source", help="retrieval source", choices=["ncbi", "ensembl", "lrg"]
+        "-s", "--source", help="retrieval source", choices=["ncbi", "ensembl", "ensembl_tark", "ensembl_rest", "lrg"]
     )
 
     parser.add_argument(
         "-t",
         "--type",
         help="reference type",
         choices=["gff3", "genbank", "json", "fasta"],
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/configuration.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 DEFAULT_SETTINGS = {
     "NCBI_GFF3_URL": "https://eutils.ncbi.nlm.nih.gov/sviewer/viewer.cgi",
     "LRG_URL": "http://ftp.ebi.ac.uk/pub/databases/lrgex/",
     "MAX_FILE_SIZE": 10 * 1048576,
     "ENSEMBL_API": "https://rest.ensembl.org",
     "ENSEMBL_API_GRCH37": "https://grch37.rest.ensembl.org",
+    "ENSEMBL_TARK_API":"https://tark.ensembl.org/api",
 }
 
 
 def setup_settings():
     """
     Setting up the configuration from the default dictionary above or (/ond
     updated) from a file path specified via the MUTALYZER_SETTINGS
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/parser.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .parsers import fasta, gff3, lrg
+from .parsers import fasta, gff3, json_ensembl, lrg
 
 
 def _get_reference_type(content):
     if content.startswith("<?xml version="):
         return "lrg"
     elif content.startswith("LOCUS"):
         return "genbank_ncbi"
@@ -15,11 +15,13 @@
 
     if reference_type == "lrg":
         model = lrg.parse(reference_content)
     elif reference_type == "gff3":
         model = gff3.parse(reference_content, reference_source)
     elif reference_type == "fasta":
         model = fasta.parse(reference_content)
+    elif reference_type == "json":
+        model = json_ensembl.parse(reference_content)
     else:
         return None
 
     return model
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/gff3.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/gff3.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/parsers/lrg.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/parsers/lrg.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/reference.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/reference.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/related.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/related.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/request.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/request.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/retriever.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     pass
 
 
 class NoReferenceError(Exception):
     def __init__(self, status, uncertain_sources):
         self.uncertain_sources = uncertain_sources
         message = ""
-        if uncertain_sources is not []:
+        if uncertain_sources != []:
             message = f"\n\nUncertain sources: {', '.join(uncertain_sources)}\n"
 
         for source in status.keys():
             source_errors = []
             message += f"\n{source}:"
             for error in status[source]["errors"]:
                 if isinstance(error, ValueError):
@@ -46,36 +46,36 @@
     uncertain_sources = []
     for source in status.keys():
         if not (
             len(status[source]["errors"]) == 1
             and isinstance(status[source]["errors"][0], NameError)
         ):
             uncertain_sources.append(source)
-    if uncertain_sources is []:
+    if uncertain_sources == []:
         raise NoReferenceRetrieved
     raise NoReferenceError(status, uncertain_sources)
 
 
-def _fetch_unknown_source(reference_id, reference_type, size_off=True, timeout=1):
+def _fetch_unknown_source(
+    reference_id, reference_type, reference_source, size_off=True, timeout=1
+):
 
     status = {"lrg": {"errors": []}, "ncbi": {"errors": []}, "ensembl": {"errors": []}}
 
     # LRG
     if reference_type in [None, "lrg"]:
         try:
             reference_content = lrg.fetch_lrg(reference_id, timeout=timeout)
         except (NameError, ConnectionError) as e:
             status["lrg"]["errors"].append(e)
         else:
             return reference_content, "lrg", "lrg"
     else:
         status["lrg"]["errors"].append(
-            ValueError(
-                "Lrg fetch does not support '{}' reference type.".format(reference_type)
-            )
+            ValueError(f"Lrg fetch does not support '{reference_type}' reference type.")
         )
 
     # NCBI
     try:
         reference_content, reference_type = ncbi.fetch(
             reference_id, reference_type, size_off, timeout
         )
@@ -85,15 +85,15 @@
         raise e
     else:
         return reference_content, reference_type, "ncbi"
 
     # Ensembl
     try:
         reference_content, reference_type = ensembl.fetch(
-            reference_id, reference_type, timeout
+            reference_id, reference_type, reference_source, timeout
         )
     except (NameError, ConnectionError, ValueError) as e:
         status["ensembl"]["errors"].append(e)
     else:
         return reference_content, reference_type, "ensembl"
 
     _raise_error(status)
@@ -118,29 +118,28 @@
     :returns: Reference content.
     :rtype: str
     """
     reference_content = None
 
     if reference_source is None:
         reference_content, reference_type, reference_source = _fetch_unknown_source(
-            reference_id, reference_type, size_off, timeout
+            reference_id, reference_type, reference_source, size_off, timeout
         )
     elif reference_source == "ncbi":
         reference_content, reference_type = ncbi.fetch(
             reference_id, reference_type, timeout
         )
-    elif reference_source == "ensembl":
+    elif reference_source in ["ensembl", "ensembl_tark", "ensembl_rest"]:
         reference_content, reference_type = ensembl.fetch(
-            reference_id, reference_type, timeout
+            reference_id, reference_type, reference_source, timeout
         )
     elif reference_source == "lrg":
         reference_content = lrg.fetch_lrg(reference_id, timeout=timeout)
         if reference_content:
             reference_type = "lrg"
-
     return reference_content, reference_type, reference_source
 
 
 def retrieve_model(
     reference_id,
     reference_source=None,
     reference_type=None,
@@ -163,17 +162,17 @@
         reference_id, reference_source, reference_type, size_off, timeout=timeout
     )
 
     if reference_type == "lrg":
         model = parser.parse(reference_content, reference_type, reference_source)
         if model_type == "all":
             return model
-        elif model_type == "sequence":
+        if model_type == "sequence":
             return model["sequence"]
-        elif model_type == "annotations":
+        if model_type == "annotations":
             return model["annotations"]
     elif reference_type == "gff3":
         if model_type == "all":
             annotations = parser.parse(
                 reference_content, reference_type, reference_source
             )
             fasta = retrieve_raw(
@@ -191,14 +190,24 @@
                 reference_content, reference_source, "fasta", reference_source
             )
     elif reference_type == "fasta":
         return {
             "sequence": parser.parse(reference_content, "fasta"),
         }
 
+    elif reference_type == "json":
+        if "ensembl" in reference_source:
+            json_model = parser.parse(reference_content, "json")
+            if model_type == "all":
+                return json_model
+            elif model_type == "annotations":
+                return json_model["annotations"]
+            elif model_type == "sequence":
+                return json_model["sequence"]["seq"]
+
 
 def retrieve_model_from_file(paths=[], is_lrg=False):
     """
 
     :arg list paths: Path towards the gff3, fasta, or lrg files.
     :arg bool is_lrg: If there is only one file path of an lrg.
     :returns: Reference model.
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/schema_validation.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/schema_validation.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/lrg.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/lrg.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/ncbi.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/ncbi.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,15 +186,29 @@
 
     :arg str reference_id: The reference ID.
     :arg str reference_type: The reference type ("gff3" - default, or "genbank").
     :arg bool size_on: Consider maximum file size.
 
     :returns tuple: raw annotations, type ("gff3" or "genbank")
     """
-    db = _get_database(reference_id)
+    db = "nuccore"
+    # https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4702849/
+    # https://support.nlm.nih.gov/knowledgebase/article/KA-03437/
+    # https://support.nlm.nih.gov/knowledgebase/article/KA-03434/
+    # https://support.nlm.nih.gov/knowledgebase/article/KA-03389/
+    # https://www.ncbi.nlm.nih.gov/books/NBK21091/table/ch18.T.refseq_accession_numbers_and_mole/
+    if (
+        reference_id.startswith("AP_")
+        or reference_id.startswith("NP_")
+        or reference_id.startswith("WP_")
+        or reference_id.startswith("XP_")
+        or reference_id.startswith("YP_")
+        or reference_id.startswith("ZP_")
+    ):
+        db = "protein"
     if reference_type in [None, "gff3"]:
         return fetch_gff3(reference_id, db, timeout), "gff3"
     elif reference_type == "fasta":
         return fetch_fasta(reference_id, db), "fasta"
     elif reference_type == "genbank":
         return fetch_genbank(reference_id, size_on), "genbank"
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/sources/ncbi_assemblies.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/sources/ncbi_assemblies.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever/util.py` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever/util.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/PKG-INFO` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer_retriever
-Version: 0.3.3
+Version: 0.3.4
 Summary: Mutalyzer genomic reference retriever.
 Home-page: https://github.com/mutalyzer/retriever
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,reference,retriever,genomic
 Classifier: Intended Audience :: Science/Research
@@ -18,18 +18,15 @@
 Requires-Dist: bcbio-gff>=0.7.1
 Requires-Dist: requests>=2.26.0
 Requires-Dist: schema>=0.7.4
 
 # Mutalyzer Retriever
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/mutalyzer/retriever)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/mutalyzer/retriever/Python%20package%20CI)
 ![Read the Docs](https://img.shields.io/readthedocs/mutalyzer-retriever)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/mutalyzer/retriever)
-![GitHub Release Date](https://img.shields.io/github/release-date/mutalyzer/retriever)
 ![PyPI](https://img.shields.io/pypi/v/mutalyzer_retriever)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/mutalyzer/retriever)
 ![GitHub language count](https://img.shields.io/github/languages/count/mutalyzer/retriever)
 ![GitHub top language](https://img.shields.io/github/languages/top/mutalyzer/retriever)
 ![GitHub](https://img.shields.io/github/license/mutalyzer/retriever)
 
 ---
```

### Comparing `mutalyzer_retriever-0.3.3/mutalyzer_retriever.egg-info/SOURCES.txt` & `mutalyzer_retriever-0.3.4/mutalyzer_retriever.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 mutalyzer_retriever.egg-info/dependency_links.txt
 mutalyzer_retriever.egg-info/entry_points.txt
 mutalyzer_retriever.egg-info/requires.txt
 mutalyzer_retriever.egg-info/top_level.txt
 mutalyzer_retriever/parsers/__init__.py
 mutalyzer_retriever/parsers/fasta.py
 mutalyzer_retriever/parsers/gff3.py
+mutalyzer_retriever/parsers/json_ensembl.py
 mutalyzer_retriever/parsers/lrg.py
 mutalyzer_retriever/sources/__init__.py
 mutalyzer_retriever/sources/ensembl.py
 mutalyzer_retriever/sources/lrg.py
 mutalyzer_retriever/sources/ncbi.py
 mutalyzer_retriever/sources/ncbi_assemblies.py
+tests/__init__.py
+tests/commons.py
+tests/conftest.py
 tests/test_cli.py
 tests/test_fetch.py
 tests/test_model_validation.py
 tests/test_related.py
 tests/test_retriever_model.py
```

### Comparing `mutalyzer_retriever-0.3.3/setup.cfg` & `mutalyzer_retriever-0.3.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer_retriever
-version = 0.3.3
+version = 0.3.4
 description = Mutalyzer genomic reference retriever.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mihai Lefter
 author_email = M.Lefter@lumc.nl
 url = https://github.com/mutalyzer/retriever
 keywords = Mutalyzer, HGVS, reference, retriever, genomic
```

### Comparing `mutalyzer_retriever-0.3.3/tests/test_cli.py` & `mutalyzer_retriever-0.3.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_retriever-0.3.3/tests/test_related.py` & `mutalyzer_retriever-0.3.4/tests/test_related.py`

 * *Files identical despite different names*

