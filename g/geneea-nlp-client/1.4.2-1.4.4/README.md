# Comparing `tmp/geneea-nlp-client-1.4.2.tar.gz` & `tmp/geneea-nlp-client-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geneea-nlp-client-1.4.2.tar", last modified: Wed Aug 24 12:06:22 2022, max compression
+gzip compressed data, was "geneea-nlp-client-1.4.4.tar", last modified: Fri May  3 08:50:28 2024, max compression
```

## Comparing `geneea-nlp-client-1.4.2.tar` & `geneea-nlp-client-1.4.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)      502 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneeanlpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneeanlpclient/common/
--rw-rw-rw-   0 root         (0) root         (0)     2736 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/common/common.py
--rw-rw-rw-   0 root         (0) root         (0)     5410 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/common/ud.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/common/dictutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/common/restutil.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/
--rw-rw-rw-   0 root         (0) root         (0)     2952 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/client.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7541 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/writer.py
--rw-rw-rw-   0 root         (0) root         (0)    29568 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/f2converter.py
--rw-rw-rw-   0 root         (0) root         (0)    15679 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/reader.py
--rw-rw-rw-   0 root         (0) root         (0)    54885 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/model.py
--rw-rw-rw-   0 root         (0) root         (0)    18574 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/geneeanlpclient/g3/request.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/examples/g3/
--rw-rw-rw-   0 root         (0) root         (0)     2563 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/relationsToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/quickStartEntities.py
--rw-rw-rw-   0 root         (0) root         (0)        2 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/languageToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2890 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/quickStartAll.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/quickStart.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/entitiesToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/examples/g3/sentimentToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     1232 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1350 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/tests/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/
--rw-rw-rw-   0 root         (0) root         (0)     2743 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/test_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4103 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/test_jsonutil.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/test_ud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/
--rw-rw-rw-   0 root         (0) root         (0)     3674 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_tokenSupport.py
--rw-rw-rw-   0 root         (0) root         (0)     8299 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_rw.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/generate.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     5447 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_treeBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_tokenutils.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_f2converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_charSpan.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 12:06:17.000000 geneea-nlp-client-1.4.2/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)       31 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1562 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1350 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-08-24 12:06:22.000000 geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/dependency_links.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/examples/g3/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/entitiesToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/languageToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/quickStart.py
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/quickStartAll.py
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/quickStartEntities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/relationsToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/sentimentToExcel.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/geneeanlpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/geneeanlpclient/common/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/dictutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/restutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     5410 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/ud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/geneeanlpclient/g3/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    29568 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/f2converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    54885 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    15903 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    18574 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7541 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/geneeanlpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2743 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4103 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_jsonutil.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_ud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_charSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_f2converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     9166 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_rw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenSupport.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_treeBuilder.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/common/common.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/common/common.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/common/ud.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/common/ud.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/common/dictutil.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/common/dictutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/common/restutil.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/common/restutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/client.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/client.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/__init__.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/__init__.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/writer.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/writer.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/f2converter.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/f2converter.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/reader.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 # Except the fromDict function, all functions and classes defined in this file are only internal helpers.
 #
 # Conventions:
 #  - variables prefixed with 'raw' refer to dictionaries based on the json objects returned by the API
 
 
+import logging
 import math
 import re
 import warnings
 from typing import Any, Dict, Iterable, List, Optional
 
 from geneeanlpclient.common import ud
 from geneeanlpclient.common.dictutil import JsonType, getValue
@@ -33,14 +34,16 @@
     'id', 'language', 'paragraphs',
     'entities', 'tags', 'relations',
     'docSentiment', 'itemSentiments', 'docVectors', 'itemVectors',
     'usedChars', 'metadata', 'debugInfo', 'version'
 ])
 """ Standard keys used in G3 analysis JSON """
 
+LOG = logging.getLogger(__name__)
+
 
 def fromDict(rawAnalysis: JsonType) -> Analysis:
     """
     Reads the Analysis object from a JSON-based dictionary as returned from Geneea G3 API.
     """
     return _Reader().fromDict(rawAnalysis)
 
@@ -128,17 +131,21 @@
 
     def _readVersion(self, rawAnalysis: JsonType) -> None:
         version = rawAnalysis.get('version', '3.0.0')
         verMatch = re.fullmatch(r'^([0-9]+)\.([0-9]+)\.([0-9]+)$', version)
         if not verMatch:
             raise ValueError(f'unsupported API version "{version}"')
         verMajor, verMinor, verFix = tuple(map(int, verMatch.groups()))
+        if verMajor > 3:
+            raise ValueError(f'unsupported API version "{version}", major ver.num > 3')
         if verMajor != 3 or verMinor > 2:
-            raise ValueError(f'unsupported API version "{version}", major ver.num != 3 or minor ver.num > 2')
-        self.version = verMajor, verMinor, verFix
+            LOG.warning(f'Reading analysis with version {version} '
+                        f'(higher than {self.version}) is only partially supported')
+        else:
+            self.version = verMajor, verMinor, verFix
 
     def _readSentiment(self, rawSentiment: JsonType) -> Sentiment:
         return Sentiment(
             mean=rawSentiment['mean'],
             label=rawSentiment['label'],
             positive=rawSentiment['positive'],
             negative=rawSentiment['negative'],
```

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/model.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/model.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneeanlpclient/g3/request.py` & `geneea-nlp-client-1.4.4/geneeanlpclient/g3/request.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/relationsToExcel.py` & `geneea-nlp-client-1.4.4/examples/g3/relationsToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/quickStartEntities.py` & `geneea-nlp-client-1.4.4/examples/g3/quickStartEntities.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/languageToExcel.py` & `geneea-nlp-client-1.4.4/examples/g3/languageToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/quickStartAll.py` & `geneea-nlp-client-1.4.4/examples/g3/quickStartAll.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/quickStart.py` & `geneea-nlp-client-1.4.4/examples/g3/quickStart.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/entitiesToExcel.py` & `geneea-nlp-client-1.4.4/examples/g3/entitiesToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/examples/g3/sentimentToExcel.py` & `geneea-nlp-client-1.4.4/examples/g3/sentimentToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/setup.py` & `geneea-nlp-client-1.4.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', mode='r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='geneea-nlp-client',
-    version='1.4.2',
+    version='1.4.4',
 
     author='Geneea Analytics s.r.o',
     author_email='support@geneea.com',
     description='The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='geneea python interpretor nlp nlu api cli',
@@ -20,15 +20,20 @@
         "Source Code": "https://bitbucket.org/geneea/sdk",
     },
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'License :: OSI Approved :: Apache Software License'
     ],
 
     # Dependencies
     install_requires=['requests~=2.25', 'retrying~=1.3'],
     dependency_links=[],
     extras_require={
```

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/test_common.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_common.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/common/test_jsonutil.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_jsonutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_tokenSupport.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenSupport.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_rw.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_rw.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,37 @@
                 expected = json.load(file)
                 if expected.get('itemSentiments') == {}:
                     del expected['itemSentiments']
                 TestRW._replaceClauseByRoot(expected)
 
             self.assertDictEqual(expected, actual)
 
+    def test_read_write_newer_g3(self):
+        """
+        Test that we can read newer G3 with the same major version and write it again.
+        It is assumed that after write some content can be lost.
+        """
+        self.maxDiff = None
+
+        exampleFile = Path(__file__).parent / 'examples' / 'forward_example_ENTITIES_PROPS.json'
+        exampleExpectedFile = Path(__file__).parent / 'examples' / 'example_ENTITIES.json'
+
+        with exampleFile.open(encoding='utf8') as file:
+            obj = fromDict(json.load(file))
+
+        actual = toDict(obj)
+
+        with exampleExpectedFile.open(encoding='utf8') as file:
+            expected = json.load(file)
+            if expected.get('itemSentiments') == {}:
+                del expected['itemSentiments']
+            TestRW._replaceClauseByRoot(expected)
+
+        self.assertDictEqual(expected, actual)
+
     def test_tokens(self):
         obj = examples.example_full_obj()
 
         token0 = obj.paragraphs[0].sentences[0].tokens[0]  # Angela
 
         self.assertEqual(token0._id, 'w0')
         self.assertEqual(token0.text, 'Angela')
```

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/generate.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/generate.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_request.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_request.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/examples.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/examples.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_treeBuilder.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_treeBuilder.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_tokenutils.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenutils.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_f2converter.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_f2converter.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_charSpan.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_charSpan.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/tests/geneeanlpclient/g3/test_analysis.py` & `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_analysis.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.2/geneea_nlp_client.egg-info/SOURCES.txt` & `geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 examples/__init__.py
 examples/g3/__init__.py
 examples/g3/entitiesToExcel.py
 examples/g3/languageToExcel.py
 examples/g3/quickStart.py
```

