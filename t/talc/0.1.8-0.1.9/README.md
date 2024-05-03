# Comparing `tmp/talc-0.1.8.tar.gz` & `tmp/talc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talc-0.1.8.tar", last modified: Thu Feb 15 18:39:15 2024, max compression
+gzip compressed data, was "talc-0.1.9.tar", last modified: Thu Feb 15 18:58:53 2024, max compression
```

## Comparing `talc-0.1.8.tar` & `talc-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:39:15.831174 talc-0.1.8/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.1.8/LICENSE
--rw-r--r--   0 mkerr      (501) staff       (20)     4469 2024-02-15 18:39:15.830977 talc-0.1.8/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)     3892 2024-02-08 20:56:36.000000 talc-0.1.8/README.md
--rw-r--r--   0 mkerr      (501) staff       (20)      696 2024-02-15 18:37:03.000000 talc-0.1.8/pyproject.toml
--rw-r--r--   0 mkerr      (501) staff       (20)       38 2024-02-15 18:39:15.831215 talc-0.1.8/setup.cfg
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:39:15.827881 talc-0.1.8/src/
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:39:15.829314 talc-0.1.8/src/talc/
--rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-09-04 22:22:33.000000 talc-0.1.8/src/talc/__init__.py
--rw-r--r--   0 mkerr      (501) staff       (20)    12706 2024-02-14 23:17:03.000000 talc-0.1.8/src/talc/cli.py
--rw-r--r--   0 mkerr      (501) staff       (20)     5774 2024-02-14 21:57:58.000000 talc-0.1.8/src/talc/evals.py
--rw-r--r--   0 mkerr      (501) staff       (20)    15698 2023-09-05 20:38:15.000000 talc-0.1.8/src/talc/logger.py
-drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:39:15.830751 talc-0.1.8/src/talc.egg-info/
--rw-r--r--   0 mkerr      (501) staff       (20)     4469 2024-02-15 18:39:15.000000 talc-0.1.8/src/talc.egg-info/PKG-INFO
--rw-r--r--   0 mkerr      (501) staff       (20)      300 2024-02-15 18:39:15.000000 talc-0.1.8/src/talc.egg-info/SOURCES.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        1 2024-02-15 18:39:15.000000 talc-0.1.8/src/talc.egg-info/dependency_links.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       39 2024-02-15 18:39:15.000000 talc-0.1.8/src/talc.egg-info/entry_points.txt
--rw-r--r--   0 mkerr      (501) staff       (20)       79 2024-02-15 18:39:15.000000 talc-0.1.8/src/talc.egg-info/requires.txt
--rw-r--r--   0 mkerr      (501) staff       (20)        5 2024-02-15 18:39:15.000000 talc-0.1.8/src/talc.egg-info/top_level.txt
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:58:53.018987 talc-0.1.9/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-07-05 18:11:13.000000 talc-0.1.9/LICENSE
+-rw-r--r--   0 mkerr      (501) staff       (20)     4507 2024-02-15 18:58:53.018783 talc-0.1.9/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)     3892 2024-02-08 20:56:36.000000 talc-0.1.9/README.md
+-rw-r--r--   0 mkerr      (501) staff       (20)      726 2024-02-15 18:58:12.000000 talc-0.1.9/pyproject.toml
+-rw-r--r--   0 mkerr      (501) staff       (20)       38 2024-02-15 18:58:53.019027 talc-0.1.9/setup.cfg
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:58:53.015552 talc-0.1.9/src/
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:58:53.017014 talc-0.1.9/src/talc/
+-rw-r--r--   0 mkerr      (501) staff       (20)        0 2023-09-04 22:22:33.000000 talc-0.1.9/src/talc/__init__.py
+-rw-r--r--   0 mkerr      (501) staff       (20)    13297 2024-02-15 18:56:57.000000 talc-0.1.9/src/talc/cli.py
+-rw-r--r--   0 mkerr      (501) staff       (20)     5774 2024-02-14 21:57:58.000000 talc-0.1.9/src/talc/evals.py
+-rw-r--r--   0 mkerr      (501) staff       (20)    15698 2023-09-05 20:38:15.000000 talc-0.1.9/src/talc/logger.py
+drwxr-xr-x   0 mkerr      (501) staff       (20)        0 2024-02-15 18:58:53.018460 talc-0.1.9/src/talc.egg-info/
+-rw-r--r--   0 mkerr      (501) staff       (20)     4507 2024-02-15 18:58:53.000000 talc-0.1.9/src/talc.egg-info/PKG-INFO
+-rw-r--r--   0 mkerr      (501) staff       (20)      300 2024-02-15 18:58:53.000000 talc-0.1.9/src/talc.egg-info/SOURCES.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        1 2024-02-15 18:58:53.000000 talc-0.1.9/src/talc.egg-info/dependency_links.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)       39 2024-02-15 18:58:53.000000 talc-0.1.9/src/talc.egg-info/entry_points.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)      102 2024-02-15 18:58:53.000000 talc-0.1.9/src/talc.egg-info/requires.txt
+-rw-r--r--   0 mkerr      (501) staff       (20)        5 2024-02-15 18:58:53.000000 talc-0.1.9/src/talc.egg-info/top_level.txt
```

### Comparing `talc-0.1.8/PKG-INFO` & `talc-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: supabase>=1.0.3
 Requires-Dist: openai>=0.11.6
 Requires-Dist: click>=8.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=1.10.11
+Requires-Dist: pdfminer.six>=20231228
 
 ## What Talc Does
 
 LLM applications often require custom datasets to develop and improve outputs. This is relevant not only during the training and tuning process of creating a model, but also during the software development cycle for feedback and testing on new changes.
 
 Historically this has been done with human labelers, but humans are slow and often incorrect.
```

### Comparing `talc-0.1.8/README.md` & `talc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `talc-0.1.8/pyproject.toml` & `talc-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "talc"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Max Kerr", email="max@talc.ai" },
   { name="Matt Lee", email="matt@talc.ai" },
 ]
 description = "Logging client for Talc Debugger."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -19,14 +19,15 @@
 ]
 dependencies = [
     "supabase>=1.0.3",
     "openai>=0.11.6",
     "click>=8.1.3",
     "requests>=2.31.0",
     "pydantic>=1.10.11",
+    "pdfminer.six>=20231228",
 ]
 
 [project.urls]
 homepage = "https://talc.ai"
 
 [project.scripts]
 talc = "talc.cli:main"
```

### Comparing `talc-0.1.8/src/talc/cli.py` & `talc-0.1.9/src/talc/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,15 +94,22 @@
 @click.option(
     "--infile",
     prompt="Results CSV path",
     help="Path to CSV file to load results from. Columns should be 'id', 'result'. Header row is required and case sensitive.",
 )
 @click.option("--print_failed", is_flag=True, help="Print the failed test cases.")
 @click.option("--outfile", default=None, help="Optionally save output as CSV.")
-def eval(api_key: str, infile: str, print_failed: bool, outfile: str):
+@click.option(
+    "--fail_on_error",
+    is_flag=True,
+    help="Exit with a non-zero status if any test cases fail.",
+)
+def eval(
+    api_key: str, infile: str, print_failed: bool, outfile: str, fail_on_error: bool
+):
     """Grade a test run from a csv. Columns should be 'id', question, and 'result'. CSV should have a header row."""
 
     if api_key is None:
         raise click.UsageError(
             "No API key provided. Please set the TALC_API_KEY environment variable or provide the --api_key option."
         )
 
@@ -115,32 +122,41 @@
             TestCaseResponse(id=row["id"], response=row["result"]) for row in reader
         ]
 
     run_info = client.start_run()
     client.submit_responses(results)
     print("Submitted results. Beginning grading for run ID: " + run_info.id)
 
-    return poll_results(client, run_info.id, print_failed, outfile)
+    res = poll_results(client, run_info.id, print_failed, outfile)
+    if fail_on_error and res != 0:
+        exit(res)
 
 
 @evals.command()
 @click.option("--api_key", default=talc_api_key, help="Talc API key")
 @click.option("--run_id", prompt="Run ID", help="The ID of the run to get results for.")
 @click.option("--print_failed", is_flag=True, help="Print the failed test cases.")
-def get_results(api_key: str, run_id: str, print_failed: bool):
+@click.option(
+    "--fail_on_error",
+    is_flag=True,
+    help="Exit with a non-zero status if any test cases fail.",
+)
+def get_results(api_key: str, run_id: str, print_failed: bool, fail_on_error: bool):
     """Get the grades for a test run."""
 
     if api_key is None:
         raise click.UsageError(
             "No API key provided. Please set the TALC_API_KEY environment variable or provide the --api_key option."
         )
 
     client = EvalsClient(api_key, talc_base_url, run_id)
 
-    return poll_results(client, run_id, print_failed, None)
+    res = poll_results(client, run_id, print_failed, None)
+    if fail_on_error and res != 0:
+        exit(res)
 
 
 @evals.command()
 @click.option("--api_key", default=talc_api_key, help="Talc API key")
 @click.option(
     "--csv",
     prompt="CSV path",
@@ -191,15 +207,20 @@
 )
 @click.option(
     "--name",
     prompt="Dataset name",
     help="The name of the dataset.",
     default="Temp Dataset",
 )
-def upload_and_grade(api_key: str, csv: str, name: str):
+@click.option(
+    "--fail_on_error",
+    is_flag=True,
+    help="Exit with a non-zero status if any test cases fail.",
+)
+def upload_and_grade(api_key: str, csv: str, name: str, fail_on_error: bool):
     """Upload a CSV with questions, reference answers, and user answers. Grade the user answers and return the grade. Useful for manual testing."""
 
     if api_key is None:
         raise click.UsageError(
             "No API key provided. Please set the TALC_API_KEY environment variable or provide the --api_key option."
         )
 
@@ -243,15 +264,17 @@
     ]
 
     # Create a run and submit the results
     run_info = client.start_run()
     client.submit_responses(results)
     print("Submitted results. Beginning grading for run ID: " + run_info.id)
 
-    return poll_results(client, run_info.id, True, None)
+    res = poll_results(client, run_info.id, True, None)
+    if fail_on_error and res != 0:
+        exit(res)
 
 
 @evals.command()
 @click.option("--api_key", default=talc_api_key, help="Talc API key")
 @click.option(
     "--file",
     prompt="Input folder, single file path, or URL.",
```

### Comparing `talc-0.1.8/src/talc/evals.py` & `talc-0.1.9/src/talc/evals.py`

 * *Files identical despite different names*

### Comparing `talc-0.1.8/src/talc/logger.py` & `talc-0.1.9/src/talc/logger.py`

 * *Files identical despite different names*

### Comparing `talc-0.1.8/src/talc.egg-info/PKG-INFO` & `talc-0.1.9/src/talc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: talc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Logging client for Talc Debugger.
 Author-email: Max Kerr <max@talc.ai>, Matt Lee <matt@talc.ai>
 Project-URL: homepage, https://talc.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: supabase>=1.0.3
 Requires-Dist: openai>=0.11.6
 Requires-Dist: click>=8.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic>=1.10.11
+Requires-Dist: pdfminer.six>=20231228
 
 ## What Talc Does
 
 LLM applications often require custom datasets to develop and improve outputs. This is relevant not only during the training and tuning process of creating a model, but also during the software development cycle for feedback and testing on new changes.
 
 Historically this has been done with human labelers, but humans are slow and often incorrect.
```

