# Comparing `tmp/idc_index-0.5.2.tar.gz` & `tmp/idc_index-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr 23 20:32:50 2024, max compression
+gzip compressed data, last modified: Wed May  1 17:07:39 2024, max compression
```

## Comparing `idc_index-0.5.2.tar` & `idc_index-0.5.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      125 2024-04-23 20:32:50.000000 idc_index-0.5.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-23 20:32:50.000000 idc_index-0.5.2/.gitattributes
--rw-r--r--   0        0        0     2357 2024-04-23 20:32:50.000000 idc_index-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-23 20:32:50.000000 idc_index-0.5.2/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-04-23 20:32:50.000000 idc_index-0.5.2/noxfile.py
--rw-r--r--   0        0        0     2394 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1581 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-04-23 20:32:50.000000 idc_index-0.5.2/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-04-23 20:32:50.000000 idc_index-0.5.2/docs/conf.py
--rw-r--r--   0        0        0      196 2024-04-23 20:32:50.000000 idc_index-0.5.2/docs/index.md
--rw-r--r--   0        0        0      263 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/_version.pyi
--rw-r--r--   0        0        0    27954 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-04-23 20:32:50.000000 idc_index-0.5.2/idc_index/py.typed
--rw-r--r--   0        0        0        0 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     3779 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-04-23 20:32:50.000000 idc_index-0.5.2/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-04-23 20:32:50.000000 idc_index-0.5.2/.gitignore
--rw-r--r--   0        0        0     1077 2024-04-23 20:32:50.000000 idc_index-0.5.2/LICENSE
--rw-r--r--   0        0        0     4290 2024-04-23 20:32:50.000000 idc_index-0.5.2/README.md
--rw-r--r--   0        0        0     6121 2024-04-23 20:32:50.000000 idc_index-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7531 2024-04-23 20:32:50.000000 idc_index-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-05-01 17:07:39.000000 idc_index-0.5.3/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-05-01 17:07:39.000000 idc_index-0.5.3/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-05-01 17:07:39.000000 idc_index-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-05-01 17:07:39.000000 idc_index-0.5.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-05-01 17:07:39.000000 idc_index-0.5.3/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1581 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-05-01 17:07:39.000000 idc_index-0.5.3/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-05-01 17:07:39.000000 idc_index-0.5.3/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-05-01 17:07:39.000000 idc_index-0.5.3/docs/index.md
+-rw-r--r--   0        0        0      263 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/_version.pyi
+-rw-r--r--   0        0        0    28034 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-05-01 17:07:39.000000 idc_index-0.5.3/idc_index/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     3779 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      437 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-05-01 17:07:39.000000 idc_index-0.5.3/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-05-01 17:07:39.000000 idc_index-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1077 2024-05-01 17:07:39.000000 idc_index-0.5.3/LICENSE
+-rw-r--r--   0        0        0     4290 2024-05-01 17:07:39.000000 idc_index-0.5.3/README.md
+-rw-r--r--   0        0        0     6121 2024-05-01 17:07:39.000000 idc_index-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     7531 2024-05-01 17:07:39.000000 idc_index-0.5.3/PKG-INFO
```

### Comparing `idc_index-0.5.2/.pre-commit-config.yaml` & `idc_index-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/noxfile.py` & `idc_index-0.5.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/.github/CONTRIBUTING.md` & `idc_index-0.5.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/.github/matchers/pylint.json` & `idc_index-0.5.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/.github/workflows/cd.yml` & `idc_index-0.5.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/.github/workflows/ci.yml` & `idc_index-0.5.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/docs/conf.py` & `idc_index-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/idc_index/index.py` & `idc_index-0.5.3/idc_index/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class IDCClient:
     def __init__(self):
         file_path = idc_index_data.IDC_INDEX_PARQUET_FILEPATH
 
         # Read index file
         logger.debug(f"Reading index file v{idc_index_data.__version__}")
         self.index = pd.read_parquet(file_path)
-        self.index = self.index.astype(str).replace("nan", "")
+        # self.index = self.index.astype(str).replace("nan", "")
         self.index["series_size_MB"] = self.index["series_size_MB"].astype(float)
         self.collection_summary = self.index.groupby("collection_id").agg(
             {"Modality": pd.Series.unique, "series_size_MB": "sum"}
         )
 
         # Lookup s5cmd
         self.s5cmdPath = shutil.which("s5cmd")
@@ -365,19 +365,19 @@
 
         Returns:
             list of strings containing the AWS S3 URLs of the files corresponding to the SeriesInstanceUID
         """
         # Query to get the S3 URL
         s3url_query = f"""
         SELECT
-          series_aws_url
+        series_aws_url
         FROM
-          index
+        index
         WHERE
-          SeriesInstanceUID='{seriesInstanceUID}'
+        SeriesInstanceUID='{seriesInstanceUID}'
         """
         s3url_query_df = self.sql_query(s3url_query)
         s3_url = s3url_query_df.series_aws_url[0]
 
         # Remove the last character from the S3 URL
         s3_url = s3_url[:-1]
 
@@ -387,15 +387,19 @@
             stdout=subprocess.PIPE,
             check=False,
         )
         output = result.stdout.decode("utf-8")
 
         # Parse the output to get the file names
         lines = output.split("\n")
-        file_names = [s3_url + line.split()[-1] for line in lines if line]
+        file_names = [
+            s3_url + line.split()[-1]
+            for line in lines
+            if line and line.split()[-1].endswith(".dcm")
+        ]
 
         return file_names
 
     def get_viewer_URL(
         self, seriesInstanceUID=None, studyInstanceUID=None, viewer_selector=None
     ):
         """
```

### Comparing `idc_index-0.5.2/tests/idcindex.py` & `idc_index-0.5.3/tests/idcindex.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/.gitignore` & `idc_index-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/LICENSE` & `idc_index-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/README.md` & `idc_index-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/pyproject.toml` & `idc_index-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idc_index-0.5.2/PKG-INFO` & `idc_index-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.5.2
+Version: 0.5.3
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
```

