# Comparing `tmp/sciterra-0.0.2.tar.gz` & `tmp/sciterra-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciterra-0.0.2.tar", last modified: Wed May  1 01:17:42 2024, max compression
+gzip compressed data, was "sciterra-0.0.21.tar", last modified: Fri May  3 19:13:43 2024, max compression
```

## Comparing `sciterra-0.0.2.tar` & `sciterra-0.0.21.tar`

### file list

```diff
@@ -1,56 +1,51 @@
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.011403 sciterra-0.0.2/
--rw-r--r--   0 nathanielimel   (501) staff       (20)     9365 2024-05-01 01:17:42.011084 sciterra-0.0.2/PKG-INFO
--rw-r--r--   0 nathanielimel   (501) staff       (20)     8609 2024-03-22 03:23:54.000000 sciterra-0.0.2/README.md
--rw-r--r--   0 nathanielimel   (501) staff       (20)       84 2023-06-05 00:40:34.000000 sciterra-0.0.2/pyproject.toml
--rw-r--r--   0 nathanielimel   (501) staff       (20)       38 2024-05-01 01:17:42.011442 sciterra-0.0.2/setup.cfg
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1329 2024-05-01 01:13:10.000000 sciterra-0.0.2/setup.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.001912 sciterra-0.0.2/src/
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.002503 sciterra-0.0.2/src/examples/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:29.000000 sciterra-0.0.2/src/examples/__init__.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.002964 sciterra-0.0.2/src/examples/scratch/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:36.000000 sciterra-0.0.2/src/examples/scratch/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)      759 2024-02-06 02:15:00.000000 sciterra-0.0.2/src/examples/scratch/main.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1490 2023-12-26 23:42:31.000000 sciterra-0.0.2/src/examples/scratch/run_topography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     3472 2023-12-26 05:26:00.000000 sciterra-0.0.2/src/examples/scratch/util.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.003077 sciterra-0.0.2/src/sciterra/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      253 2023-07-25 05:25:07.000000 sciterra-0.0.2/src/sciterra/__init__.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.004320 sciterra-0.0.2/src/sciterra/librarians/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      759 2023-11-12 17:04:39.000000 sciterra-0.0.2/src/sciterra/librarians/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     7908 2024-05-01 01:00:35.000000 sciterra-0.0.2/src/sciterra/librarians/adslibrarian.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2332 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/librarians/librarian.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    10475 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/librarians/s2librarian.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.006291 sciterra-0.0.2/src/sciterra/mapping/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      246 2023-07-12 00:09:56.000000 sciterra-0.0.2/src/sciterra/mapping/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     5837 2024-05-01 01:00:35.000000 sciterra-0.0.2/src/sciterra/mapping/atlas.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    32018 2024-05-01 00:58:38.000000 sciterra-0.0.2/src/sciterra/mapping/cartography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     5450 2023-12-27 22:43:43.000000 sciterra-0.0.2/src/sciterra/mapping/publication.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     6257 2024-05-01 01:00:35.000000 sciterra-0.0.2/src/sciterra/mapping/topography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    12388 2024-03-22 03:23:54.000000 sciterra-0.0.2/src/sciterra/mapping/tracing.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.007115 sciterra-0.0.2/src/sciterra/misc/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-19 02:27:46.000000 sciterra-0.0.2/src/sciterra/misc/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4197 2024-03-15 05:07:12.000000 sciterra-0.0.2/src/sciterra/misc/analysis.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4084 2023-11-10 06:06:25.000000 sciterra-0.0.2/src/sciterra/misc/utils.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.009369 sciterra-0.0.2/src/sciterra/vectorization/
--rw-r--r--   0 nathanielimel   (501) staff       (20)      352 2024-02-05 00:13:40.000000 sciterra-0.0.2/src/sciterra/vectorization/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2377 2024-02-06 02:20:47.000000 sciterra-0.0.2/src/sciterra/vectorization/bow.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4725 2024-02-06 03:30:56.000000 sciterra-0.0.2/src/sciterra/vectorization/gpt2.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1763 2023-11-13 01:52:29.000000 sciterra-0.0.2/src/sciterra/vectorization/preprocessing.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     3806 2023-11-11 09:57:21.000000 sciterra-0.0.2/src/sciterra/vectorization/projection.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2858 2024-02-06 03:30:56.000000 sciterra-0.0.2/src/sciterra/vectorization/sbert.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4145 2024-02-06 03:30:56.000000 sciterra-0.0.2/src/sciterra/vectorization/scibert.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1108 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/vectorization/vectorizer.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     4570 2024-03-04 19:14:29.000000 sciterra-0.0.2/src/sciterra/vectorization/word2vec.py
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.010807 sciterra-0.0.2/src/sciterra.egg-info/
--rw-r--r--   0 nathanielimel   (501) staff       (20)     9365 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/PKG-INFO
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1372 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/SOURCES.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)        1 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/dependency_links.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)      143 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/requires.txt
--rw-r--r--   0 nathanielimel   (501) staff       (20)       24 2024-05-01 01:17:41.000000 sciterra-0.0.2/src/sciterra.egg-info/top_level.txt
-drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-01 01:17:42.010614 sciterra-0.0.2/src/tests/
--rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-04 08:04:46.000000 sciterra-0.0.2/src/tests/__init__.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     2943 2023-11-11 09:57:14.000000 sciterra-0.0.2/src/tests/test_atlas.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    21972 2024-05-01 01:00:57.000000 sciterra-0.0.2/src/tests/test_cartography.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     5050 2023-11-11 09:57:13.000000 sciterra-0.0.2/src/tests/test_librarian.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     1110 2023-11-11 09:57:10.000000 sciterra-0.0.2/src/tests/test_publication.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)     8145 2024-03-22 03:23:54.000000 sciterra-0.0.2/src/tests/test_tracing.py
--rw-r--r--   0 nathanielimel   (501) staff       (20)    15974 2024-02-06 00:04:07.000000 sciterra-0.0.2/src/tests/test_vectorization.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.171756 sciterra-0.0.21/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     9366 2024-05-03 19:13:43.171334 sciterra-0.0.21/PKG-INFO
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     8609 2024-03-22 03:23:54.000000 sciterra-0.0.21/README.md
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       84 2023-06-05 00:40:34.000000 sciterra-0.0.21/pyproject.toml
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       38 2024-05-03 19:13:43.171812 sciterra-0.0.21/setup.cfg
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1331 2024-05-03 19:12:50.000000 sciterra-0.0.21/setup.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.157226 sciterra-0.0.21/src/
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.157912 sciterra-0.0.21/src/examples/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-07-08 19:50:29.000000 sciterra-0.0.21/src/examples/__init__.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.158079 sciterra-0.0.21/src/sciterra/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      253 2023-07-25 05:25:07.000000 sciterra-0.0.21/src/sciterra/__init__.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.160972 sciterra-0.0.21/src/sciterra/librarians/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      759 2023-11-12 17:04:39.000000 sciterra-0.0.21/src/sciterra/librarians/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     7908 2024-05-01 01:00:35.000000 sciterra-0.0.21/src/sciterra/librarians/adslibrarian.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2332 2024-03-04 19:14:29.000000 sciterra-0.0.21/src/sciterra/librarians/librarian.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    10475 2024-03-04 19:14:29.000000 sciterra-0.0.21/src/sciterra/librarians/s2librarian.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.163556 sciterra-0.0.21/src/sciterra/mapping/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      246 2023-07-12 00:09:56.000000 sciterra-0.0.21/src/sciterra/mapping/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     5837 2024-05-01 01:00:35.000000 sciterra-0.0.21/src/sciterra/mapping/atlas.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    32018 2024-05-01 00:58:38.000000 sciterra-0.0.21/src/sciterra/mapping/cartography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     5450 2023-12-27 22:43:43.000000 sciterra-0.0.21/src/sciterra/mapping/publication.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     6257 2024-05-01 01:00:35.000000 sciterra-0.0.21/src/sciterra/mapping/topography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    12388 2024-05-01 08:04:06.000000 sciterra-0.0.21/src/sciterra/mapping/tracing.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.164565 sciterra-0.0.21/src/sciterra/misc/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-19 02:27:46.000000 sciterra-0.0.21/src/sciterra/misc/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4197 2024-03-15 05:07:12.000000 sciterra-0.0.21/src/sciterra/misc/analysis.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4084 2023-11-10 06:06:25.000000 sciterra-0.0.21/src/sciterra/misc/utils.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.168168 sciterra-0.0.21/src/sciterra/vectorization/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      352 2024-05-03 19:05:34.000000 sciterra-0.0.21/src/sciterra/vectorization/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2377 2024-02-06 02:20:47.000000 sciterra-0.0.21/src/sciterra/vectorization/bow.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4722 2024-05-03 18:48:07.000000 sciterra-0.0.21/src/sciterra/vectorization/gpt2.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1763 2023-11-13 01:52:29.000000 sciterra-0.0.21/src/sciterra/vectorization/preprocessing.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     3806 2023-11-11 09:57:21.000000 sciterra-0.0.21/src/sciterra/vectorization/projection.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2858 2024-02-06 03:30:56.000000 sciterra-0.0.21/src/sciterra/vectorization/sbert.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4145 2024-02-06 03:30:56.000000 sciterra-0.0.21/src/sciterra/vectorization/scibert.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1108 2024-03-04 19:14:29.000000 sciterra-0.0.21/src/sciterra/vectorization/vectorizer.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     4572 2024-05-03 19:08:54.000000 sciterra-0.0.21/src/sciterra/vectorization/word2vec.py
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.170976 sciterra-0.0.21/src/sciterra.egg-info/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     9366 2024-05-03 19:13:43.000000 sciterra-0.0.21/src/sciterra.egg-info/PKG-INFO
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1242 2024-05-03 19:13:43.000000 sciterra-0.0.21/src/sciterra.egg-info/SOURCES.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        1 2024-05-03 19:13:43.000000 sciterra-0.0.21/src/sciterra.egg-info/dependency_links.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)      143 2024-05-03 19:13:43.000000 sciterra-0.0.21/src/sciterra.egg-info/requires.txt
+-rw-r--r--   0 nathanielimel   (501) staff       (20)       24 2024-05-03 19:13:43.000000 sciterra-0.0.21/src/sciterra.egg-info/top_level.txt
+drwxr-xr-x   0 nathanielimel   (501) staff       (20)        0 2024-05-03 19:13:43.170455 sciterra-0.0.21/src/tests/
+-rw-r--r--   0 nathanielimel   (501) staff       (20)        0 2023-06-04 08:04:46.000000 sciterra-0.0.21/src/tests/__init__.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     2943 2023-11-11 09:57:14.000000 sciterra-0.0.21/src/tests/test_atlas.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    21972 2024-05-01 01:00:57.000000 sciterra-0.0.21/src/tests/test_cartography.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     5050 2023-11-11 09:57:13.000000 sciterra-0.0.21/src/tests/test_librarian.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     1110 2023-11-11 09:57:10.000000 sciterra-0.0.21/src/tests/test_publication.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)     8145 2024-03-22 03:23:54.000000 sciterra-0.0.21/src/tests/test_tracing.py
+-rw-r--r--   0 nathanielimel   (501) staff       (20)    15974 2024-02-06 00:04:07.000000 sciterra-0.0.21/src/tests/test_vectorization.py
```

### Comparing `sciterra-0.0.2/PKG-INFO` & `sciterra-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciterra
-Version: 0.0.2
+Version: 0.0.21
 Summary: Scientific literature data exploration analysis
 Home-page: https://github.com/nathimel/sciterra
 Author: Nathaniel Imel
 Author-email: nimel@uci.edu
 Project-URL: Bug Tracker, https://github.com/nathimel/sciterra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sciterra-0.0.2/README.md` & `sciterra-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/setup.py` & `sciterra-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 requirements = [
     "ads",
     "bibtexparser",
-    "gensim", # N.B.: requires scipy <= 1.10.1
+    "gensim",  # N.B.: requires scipy <= 1.10.1
     "numpy",
     "pandas",
     "plotnine",
     "scikit-learn",
     "scipy==1.10.1",
     "sentence-transformers",
     "semanticscholar==0.5.0",  # 0.6.0 has AsyncSemanticScholar which creates difficulties
@@ -23,15 +23,15 @@
     "black",
     "coverage",
     "pytest",
 ]
 
 setuptools.setup(
     name="sciterra",
-    version="0.0.2",
+    version="0.0.21",
     author="Nathaniel Imel",
     author_email="nimel@uci.edu",
     description="Scientific literature data exploration analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathimel/sciterra",
     project_urls={"Bug Tracker": "https://github.com/nathimel/sciterra/issues"},
```

### Comparing `sciterra-0.0.2/src/sciterra/librarians/__init__.py` & `sciterra-0.0.21/src/sciterra/librarians/__init__.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/librarians/adslibrarian.py` & `sciterra-0.0.21/src/sciterra/librarians/adslibrarian.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/librarians/librarian.py` & `sciterra-0.0.21/src/sciterra/librarians/librarian.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/librarians/s2librarian.py` & `sciterra-0.0.21/src/sciterra/librarians/s2librarian.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/mapping/atlas.py` & `sciterra-0.0.21/src/sciterra/mapping/atlas.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/mapping/cartography.py` & `sciterra-0.0.21/src/sciterra/mapping/cartography.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/mapping/publication.py` & `sciterra-0.0.21/src/sciterra/mapping/publication.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/mapping/topography.py` & `sciterra-0.0.21/src/sciterra/mapping/topography.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/mapping/tracing.py` & `sciterra-0.0.21/src/sciterra/mapping/tracing.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/misc/analysis.py` & `sciterra-0.0.21/src/sciterra/misc/analysis.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/misc/utils.py` & `sciterra-0.0.21/src/sciterra/misc/utils.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/bow.py` & `sciterra-0.0.21/src/sciterra/vectorization/bow.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/gpt2.py` & `sciterra-0.0.21/src/sciterra/vectorization/gpt2.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             input_ids = encoded["input_ids"]
             assert input_ids.size()[-1] <= 1024
 
             # Put data on GPU
             for k, v in encoded.items():
                 encoded[k] = v.to(self.device)
 
-            # Run the text through SciBERT,
+            # Run the text through GPT2,
             # collecting all of the hidden states produced from all 12 layers.
             with torch.no_grad():
                 outputs = self.model(  # discard logits
                     **encoded,
                 )
 
             # Get the embeddings of each final token in the batch
```

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/preprocessing.py` & `sciterra-0.0.21/src/sciterra/vectorization/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/projection.py` & `sciterra-0.0.21/src/sciterra/vectorization/projection.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/sbert.py` & `sciterra-0.0.21/src/sciterra/vectorization/sbert.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/scibert.py` & `sciterra-0.0.21/src/sciterra/vectorization/scibert.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/vectorizer.py` & `sciterra-0.0.21/src/sciterra/vectorization/vectorizer.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/sciterra/vectorization/word2vec.py` & `sciterra-0.0.21/src/sciterra/vectorization/word2vec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """We use a simple word2vec model that gets a document vector by averaging all words in the document.
 
 Since we are getting vectors for scientific documents, we must load a vocabulary to train the model from scratch. Therefore we define different subclasses for each scientific field, which may differ substantially by vocabulary.
 
-There exists a Doc2Vec module by gensim, but it seems that empirically Word2Vec + averaging can do just as well; furthermore, we're mainly interested in a simple baseline to compare with sophisticated embeddings.
+There exists a Doc2Vec module by gensim, but we're mainly interested in a simple baseline to compare with sophisticated embeddings.
 
 Links:
     gensim: https://radimrehurek.com/gensim/auto_examples/tutorials/run_word2vec.html#
 """
 
 import os
 import time
@@ -39,14 +39,15 @@
         corpus_path: str,
         model_path: str = None,
         vector_size: int = EMBEDDING_DIM,
         window: int = 5,
         min_count: int = 2,
         workers: int = cpu_count(),
         epochs: int = 10,
+        sg: bool = True,  # use skipgram for large datasets
         tokenizer: Callable[[str], list[str]] = None,
         **kwargs,
     ) -> None:
         """Construct a Word2Vec based document embedding model from a corpus."""
         super().__init__()
 
         if tokenizer is None:
@@ -68,14 +69,15 @@
             model = Word2Vec(
                 sentences=sentences,
                 vector_size=vector_size,
                 window=window,
                 min_count=min_count,
                 workers=workers,
                 epochs=epochs,
+                sg=sg,
             )
             duration = time.time() - start
             print(f"Loaded corpus and trained model in {duration:.2f} seconds.")
         else:
             print(f"Loading saved Word2Vec model from {model_path}.")
             model = Word2Vec.load(model_path)
```

### Comparing `sciterra-0.0.2/src/sciterra.egg-info/PKG-INFO` & `sciterra-0.0.21/src/sciterra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciterra
-Version: 0.0.2
+Version: 0.0.21
 Summary: Scientific literature data exploration analysis
 Home-page: https://github.com/nathimel/sciterra
 Author: Nathaniel Imel
 Author-email: nimel@uci.edu
 Project-URL: Bug Tracker, https://github.com/nathimel/sciterra/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sciterra-0.0.2/src/tests/test_atlas.py` & `sciterra-0.0.21/src/tests/test_atlas.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/tests/test_cartography.py` & `sciterra-0.0.21/src/tests/test_cartography.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/tests/test_librarian.py` & `sciterra-0.0.21/src/tests/test_librarian.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/tests/test_publication.py` & `sciterra-0.0.21/src/tests/test_publication.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/tests/test_tracing.py` & `sciterra-0.0.21/src/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `sciterra-0.0.2/src/tests/test_vectorization.py` & `sciterra-0.0.21/src/tests/test_vectorization.py`

 * *Files identical despite different names*

