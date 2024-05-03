# Comparing `tmp/gpas-1.0.1a3.tar.gz` & `tmp/gpas-1.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpas-1.0.1a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gpas-1.0.1a4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpas-1.0.1a3.tar` & `gpas-1.0.1a4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      740 2024-04-15 08:18:53.470605 gpas-1.0.1a3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1818 2024-01-30 14:52:12.197255 gpas-1.0.1a3/.gitignore
--rw-r--r--   0        0        0      142 2024-01-30 14:52:12.197255 gpas-1.0.1a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      318 2024-04-16 09:45:53.973435 gpas-1.0.1a3/Dockerfile
--rw-r--r--   0        0        0     5728 2024-04-11 12:26:08.345146 gpas-1.0.1a3/LICENSE
--rw-r--r--   0        0        0     3353 2024-04-11 12:26:08.345146 gpas-1.0.1a3/README.md
--rw-r--r--   0        0        0     6162 2024-04-16 09:30:56.563209 gpas-1.0.1a3/README_pypi.md
--rw-r--r--   0        0        0      151 2024-04-15 09:40:34.752324 gpas-1.0.1a3/environment.yml
--rw-r--r--   0        0        0      626 2024-04-16 09:30:56.563209 gpas-1.0.1a3/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-16 09:45:53.973435 gpas-1.0.1a3/src/gpas/__init__.py
--rw-r--r--   0        0        0    10110 2024-04-16 09:30:56.563209 gpas-1.0.1a3/src/gpas/cli.py
--rw-r--r--   0        0        0     4749 2024-04-16 09:30:56.563209 gpas-1.0.1a3/src/gpas/create_upload_csv.py
--rw-r--r--   0        0        0    27235 2024-04-15 08:18:53.470605 gpas-1.0.1a3/src/gpas/lib.py
--rw-r--r--   0        0        0     5949 2024-04-16 09:30:56.567209 gpas-1.0.1a3/src/gpas/models.py
--rw-r--r--   0        0        0     8247 2024-04-16 09:30:56.567209 gpas-1.0.1a3/src/gpas/util.py
--rw-r--r--   0        0        0      360 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/conftest.py
--rw-r--r--   0        0        0      607 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/auto_upload_csvs/batch1.csv
--rw-r--r--   0        0        0      453 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/auto_upload_csvs/batch2.csv
--rw-r--r--   0        0        0      915 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/auto_upload_csvs/illumina.csv
--rw-r--r--   0        0        0      655 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/auto_upload_csvs/ont.csv
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_1_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_1_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_2_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_2_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_3_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_3_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_4_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_4_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_5_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/empty_files/read_5_2.fastq.gz
--rw-r--r--   0        0        0      380 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/illumina-2.csv
--rw-r--r--   0        0        0      264 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/illumina.csv
--rw-r--r--   0        0        0      263 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/invalid/empty-sample-name.csv
--rw-r--r--   0        0        0      271 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/invalid/invalid-control.csv
--rw-r--r--   0        0        0      273 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/invalid/invalid-fastq-path.csv
--rw-r--r--   0        0        0      272 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/invalid/invalid-instrument-platform.csv
--rw-r--r--   0        0        0      264 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/invalid/invalid-specimen-organism.csv
--rw-r--r--   0        0        0      387 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/invalid/mixed-instrument-platform.csv
--rw-r--r--   0        0        0      316 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/ont-2.csv
--rw-r--r--   0        0        0      231 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/ont.csv
--rw-r--r--   0        0        0      164 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/reads/human_1_1.fastq.gz
--rw-r--r--   0        0        0      178 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/reads/human_1_2.fastq.gz
--rw-r--r--   0        0        0      319 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/reads/sars-cov-2_1_1.fastq
--rw-r--r--   0        0        0      319 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/reads/sars-cov-2_1_2.fastq
--rw-r--r--   0        0        0      335 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/reads/tuberculosis_1_1.fastq
--rw-r--r--   0        0        0      335 2024-01-30 14:52:12.201255 gpas-1.0.1a3/tests/data/reads/tuberculosis_1_2.fastq
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/unmatched_files/read_1_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/unmatched_files/read_1_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/data/unmatched_files/read_2_1.fastq.gz
--rw-r--r--   0        0        0     6284 2024-04-16 09:30:56.567209 gpas-1.0.1a3/tests/test_all.py
--rw-r--r--   0        0        0     6784 1970-01-01 00:00:00.000000 gpas-1.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      740 2024-04-15 11:06:27.973441 gpas-1.0.1a4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1818 2024-03-22 09:37:27.815396 gpas-1.0.1a4/.gitignore
+-rw-r--r--   0        0        0      142 2024-03-22 09:37:27.815396 gpas-1.0.1a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      318 2024-05-03 09:44:48.331133 gpas-1.0.1a4/Dockerfile
+-rw-r--r--   0        0        0     1057 2024-05-02 14:30:55.860689 gpas-1.0.1a4/LICENSE
+-rw-r--r--   0        0        0     3367 2024-05-03 09:44:48.331133 gpas-1.0.1a4/README.md
+-rw-r--r--   0        0        0     6169 2024-05-03 09:44:48.331133 gpas-1.0.1a4/README_pypi.md
+-rw-r--r--   0        0        0      151 2024-04-15 11:06:27.973441 gpas-1.0.1a4/environment.yml
+-rw-r--r--   0        0        0      626 2024-05-02 14:30:55.860689 gpas-1.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-05-03 10:08:56.914527 gpas-1.0.1a4/src/gpas/__init__.py
+-rw-r--r--   0        0        0    10110 2024-05-02 15:30:46.322852 gpas-1.0.1a4/src/gpas/cli.py
+-rw-r--r--   0        0        0     4749 2024-05-02 14:30:55.860689 gpas-1.0.1a4/src/gpas/create_upload_csv.py
+-rw-r--r--   0        0        0    27392 2024-05-03 09:44:48.331133 gpas-1.0.1a4/src/gpas/lib.py
+-rw-r--r--   0        0        0     5949 2024-05-02 14:30:55.860689 gpas-1.0.1a4/src/gpas/models.py
+-rw-r--r--   0        0        0     8254 2024-05-03 09:44:48.335133 gpas-1.0.1a4/src/gpas/util.py
+-rw-r--r--   0        0        0      360 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/conftest.py
+-rw-r--r--   0        0        0      607 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/auto_upload_csvs/batch1.csv
+-rw-r--r--   0        0        0      453 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/auto_upload_csvs/batch2.csv
+-rw-r--r--   0        0        0      915 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/auto_upload_csvs/illumina.csv
+-rw-r--r--   0        0        0      655 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/auto_upload_csvs/ont.csv
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_1_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_1_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_2_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_2_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_3_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_3_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_4_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_4_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_5_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/empty_files/read_5_2.fastq.gz
+-rw-r--r--   0        0        0      380 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/illumina-2.csv
+-rw-r--r--   0        0        0      264 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/illumina.csv
+-rw-r--r--   0        0        0      263 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/invalid/empty-sample-name.csv
+-rw-r--r--   0        0        0      271 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/invalid/invalid-control.csv
+-rw-r--r--   0        0        0      273 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/invalid/invalid-fastq-path.csv
+-rw-r--r--   0        0        0      272 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/invalid/invalid-instrument-platform.csv
+-rw-r--r--   0        0        0      264 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/invalid/invalid-specimen-organism.csv
+-rw-r--r--   0        0        0      387 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/invalid/mixed-instrument-platform.csv
+-rw-r--r--   0        0        0      316 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/ont-2.csv
+-rw-r--r--   0        0        0      231 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/ont.csv
+-rw-r--r--   0        0        0      164 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/reads/human_1_1.fastq.gz
+-rw-r--r--   0        0        0      178 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/reads/human_1_2.fastq.gz
+-rw-r--r--   0        0        0      319 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/reads/sars-cov-2_1_1.fastq
+-rw-r--r--   0        0        0      319 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/reads/sars-cov-2_1_2.fastq
+-rw-r--r--   0        0        0      335 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/reads/tuberculosis_1_1.fastq
+-rw-r--r--   0        0        0      335 2024-03-22 09:37:27.815396 gpas-1.0.1a4/tests/data/reads/tuberculosis_1_2.fastq
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/unmatched_files/read_1_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/unmatched_files/read_1_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/data/unmatched_files/read_2_1.fastq.gz
+-rw-r--r--   0        0        0     6284 2024-05-02 14:30:55.860689 gpas-1.0.1a4/tests/test_all.py
+-rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 gpas-1.0.1a4/PKG-INFO
```

### Comparing `gpas-1.0.1a3/.github/workflows/test.yml` & `gpas-1.0.1a4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/.gitignore` & `gpas-1.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/README.md` & `gpas-1.0.1a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
   ```bash
   arch -x86_64 zsh
   ```
 
 - Perform the installation/upgrade:
   ```bash
-  conda create -y -n gpas -c conda-forge -c bioconda hostile
+  conda create -y -n gpas -c conda-forge -c bioconda hostile==1.1.0
   conda activate gpas
   pip install --upgrade gpas
   ```
 
 - Test:
   ```
   gpas --version
@@ -101,15 +101,15 @@
    ```
 
 
 
 ### Installing a pre-release version
 
 ```bash
-conda create --yes -n gpas -c conda-forge -c bioconda hostile
+conda create --yes -n gpas -c conda-forge -c bioconda hostile==1.1.0
 conda activate gpas
 pip install --pre gpas
 ```
 
 
 
 ### Using a local development server
```

### Comparing `gpas-1.0.1a3/README_pypi.md` & `gpas-1.0.1a4/README_pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
   ```bash
   arch -x86_64 zsh
   ```
 
 - Perform the installation/upgrade:
   ```bash
-  conda create -y -n gpas -c conda-forge -c bioconda hostile
+  conda create -y -n gpas -c conda-forge -c bioconda hostile==1.1.0
   conda activate gpas
   pip install --upgrade gpas
   ```
 
 - Test:
   ```
   gpas --version
```

### Comparing `gpas-1.0.1a3/pyproject.toml` & `gpas-1.0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/src/gpas/cli.py` & `gpas-1.0.1a4/src/gpas/cli.py`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/src/gpas/create_upload_csv.py` & `gpas-1.0.1a4/src/gpas/create_upload_csv.py`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/src/gpas/lib.py` & `gpas-1.0.1a4/src/gpas/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from pydantic import BaseModel
 from tqdm import tqdm
 
 import gpas
 import hostile
 
 from gpas import util, models
+from gpas.util import MissingError
 
 
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 DEFAULT_HOST = "research.portal.gpas.world"
 DEFAULT_PROTOCOL = "https"
 HOSTILE_INDEX_NAME = "human-t2t-hla-argos985-mycob140"
@@ -657,15 +658,18 @@
         guids = util.parse_comma_separated_string(samples)
         guids_samples = {guid: None for guid in guids}
         logging.info(f"Using guids {guids}")
     else:
         raise RuntimeError("Specify either a list of samples or a mapping CSV")
     filenames = util.parse_comma_separated_string(filenames)
     for guid, sample in guids_samples.items():
-        output_files = fetch_output_files(sample_id=guid, host=host, latest=True)
+        try:
+            output_files = fetch_output_files(sample_id=guid, host=host, latest=True)
+        except MissingError:
+            pass # Missing output files should not cause the program to end
         with httpx.Client(
             event_hooks=util.httpx_hooks,
             transport=httpx.HTTPTransport(retries=5),
             timeout=7200,  # 2 hours
         ) as client:
             for filename in filenames:
                 prefixed_filename = f"{guid}_{filename}"
```

### Comparing `gpas-1.0.1a3/src/gpas/models.py` & `gpas-1.0.1a4/src/gpas/models.py`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/src/gpas/util.py` & `gpas-1.0.1a4/src/gpas/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         Args:
             this_version (str): The version of installed version
             current_version (str): The version returned by the API
         """
         self.message = (
             f"\n\nThe installed client version ({this_version}) is no longer supported."
             " To update the client, please run:\n\n"
-            "conda create -y -n gpas -c conda-forge -c bioconda hostile && conda activate gpas && pip install --upgrade gpas"
+            "conda create -y -n gpas -c conda-forge -c bioconda hostile==1.1.0 && conda activate gpas && pip install --upgrade gpas"
         )
         super().__init__(self.message)
 
 
 # Python errors for neater client errors
 class AuthorizationError(Exception):
     """Custom exception for authorization issues. 401"""
```

### Comparing `gpas-1.0.1a3/tests/data/auto_upload_csvs/batch1.csv` & `gpas-1.0.1a4/tests/data/auto_upload_csvs/batch1.csv`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/tests/data/auto_upload_csvs/illumina.csv` & `gpas-1.0.1a4/tests/data/auto_upload_csvs/illumina.csv`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/tests/data/auto_upload_csvs/ont.csv` & `gpas-1.0.1a4/tests/data/auto_upload_csvs/ont.csv`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/tests/test_all.py` & `gpas-1.0.1a4/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `gpas-1.0.1a3/PKG-INFO` & `gpas-1.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpas
-Version: 1.0.1a3
+Version: 1.0.1a4
 Summary: The command line and Python client for the GPAS platform
 Author-email: Bede Constantinides <bedeabc@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: platformdirs>=3.9.1,<=4.2.0
@@ -59,15 +59,15 @@
 
   ```bash
   arch -x86_64 zsh
   ```
 
 - Perform the installation/upgrade:
   ```bash
-  conda create -y -n gpas -c conda-forge -c bioconda hostile
+  conda create -y -n gpas -c conda-forge -c bioconda hostile==1.1.0
   conda activate gpas
   pip install --upgrade gpas
   ```
 
 - Test:
   ```
   gpas --version
```

