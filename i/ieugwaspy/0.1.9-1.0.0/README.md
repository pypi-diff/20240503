# Comparing `tmp/ieugwaspy-0.1.9.tar.gz` & `tmp/ieugwaspy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieugwaspy-0.1.9.tar", last modified: Tue Oct 24 09:15:06 2023, max compression
+gzip compressed data, was "ieugwaspy-1.0.0.tar", last modified: Fri May  3 12:26:54 2024, max compression
```

## Comparing `ieugwaspy-0.1.9.tar` & `ieugwaspy-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 09:15:06.443706 ieugwaspy-0.1.9/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-10-24 09:15:06.443706 ieugwaspy-0.1.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 09:15:06.443706 ieugwaspy-0.1.9/ieugwaspy/
--rwxr-xr-x   0 runner    (1001) docker     (127)      345 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/ieugwaspy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      411 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/ieugwaspy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      666 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/ieugwaspy/backwards.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      672 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/ieugwaspy/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5319 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/ieugwaspy/query.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/ieugwaspy/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 09:15:06.443706 ieugwaspy-0.1.9/ieugwaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-10-24 09:15:06.000000 ieugwaspy-0.1.9/ieugwaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-10-24 09:15:06.000000 ieugwaspy-0.1.9/ieugwaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 09:15:06.000000 ieugwaspy-0.1.9/ieugwaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-24 09:15:06.000000 ieugwaspy-0.1.9/ieugwaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-24 09:15:06.000000 ieugwaspy-0.1.9/ieugwaspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 09:15:06.443706 ieugwaspy-0.1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      695 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 09:15:06.443706 ieugwaspy-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-24 09:14:55.000000 ieugwaspy-0.1.9/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1453 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/ieugwaspy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/backwards.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5628 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/ieugwaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      695 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/tests/test_api.py
```

### Comparing `ieugwaspy-0.1.9/LICENSE` & `ieugwaspy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ieugwaspy-0.1.9/PKG-INFO` & `ieugwaspy-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: ieugwaspy
-Version: 0.1.9
+Version: 1.0.0
 Summary: Python interface to IEU GWAS database API
 Home-page: https://mrcieu.github.io/ieugwaspy/
 Author: Tom Gaunt
 Author-email: tom@biocompute.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: retry
 
 # Perform fast queries in Python against a massive database of complete GWAS summary data
 
 [![Actions Status](https://github.com/MRCIEU/ieugwaspy/workflows/ieugwaspy_test/badge.svg)](https://github.com/MRCIEU/ieugwaspy/actions)
 
-The [IEU GWAS database](https://gwas.mrcieu.ac.uk/) comprises over 10,000 curated, QC'd and harmonised complete GWAS summary datasets and can be queried using an API. See [here](http://gwasapi.mrcieu.ac.uk/docs/) for documentation on the API itself. This Python package package is a wrapper to make generic calls to the API, plus convenience functions for specific queries.
+The [IEU OpenGWAS database](https://gwas.mrcieu.ac.uk/) comprises over 50,000 curated, QC'd and harmonised complete GWAS summary datasets and can be queried using an API. See [here](https://api.opengwas.io/api/) for documentation on the API itself. This Python package is a wrapper to make generic calls to the API, plus convenience functions for specific queries.
 
 [See ieugwaspy documentation](https://mrcieu.github.io/ieugwaspy/) for details of how to use this package.
 
-### Installation:
+### Installation
 
 Install using ```pip install ieugwaspy```
 
-### Features:
+### Features
 
 - Get meta data about specific or all studies
 - Obtain the top hits (with on the fly clumping as an option) from each of the GWAS datasets. Clumping and significance thresholds can be specified
 - Obtain the summary results of specific variants across specific studies. LD-proxy lookups are performed automatically if a specific variant is absent from a study
 - Perform PheWAS (look up all associations for a variant)
 - Convert between chromosome:position and rsids and getting annotations
+
+
+#### Developer notes
+To run tests, use `pytest -v -s --select-api="dev"`
+To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
```

### Comparing `ieugwaspy-0.1.9/README.md` & `ieugwaspy-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Perform fast queries in Python against a massive database of complete GWAS summary data
 
 [![Actions Status](https://github.com/MRCIEU/ieugwaspy/workflows/ieugwaspy_test/badge.svg)](https://github.com/MRCIEU/ieugwaspy/actions)
 
-The [IEU GWAS database](https://gwas.mrcieu.ac.uk/) comprises over 10,000 curated, QC'd and harmonised complete GWAS summary datasets and can be queried using an API. See [here](http://gwasapi.mrcieu.ac.uk/docs/) for documentation on the API itself. This Python package package is a wrapper to make generic calls to the API, plus convenience functions for specific queries.
+The [IEU OpenGWAS database](https://gwas.mrcieu.ac.uk/) comprises over 50,000 curated, QC'd and harmonised complete GWAS summary datasets and can be queried using an API. See [here](https://api.opengwas.io/api/) for documentation on the API itself. This Python package is a wrapper to make generic calls to the API, plus convenience functions for specific queries.
 
 [See ieugwaspy documentation](https://mrcieu.github.io/ieugwaspy/) for details of how to use this package.
 
-### Installation:
+### Installation
 
 Install using ```pip install ieugwaspy```
 
-### Features:
+### Features
 
 - Get meta data about specific or all studies
 - Obtain the top hits (with on the fly clumping as an option) from each of the GWAS datasets. Clumping and significance thresholds can be specified
 - Obtain the summary results of specific variants across specific studies. LD-proxy lookups are performed automatically if a specific variant is absent from a study
 - Perform PheWAS (look up all associations for a variant)
 - Convert between chromosome:position and rsids and getting annotations
+
+
+#### Developer notes
+To run tests, use `pytest -v -s --select-api="dev"`
+To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
```

### Comparing `ieugwaspy-0.1.9/ieugwaspy/backwards.py` & `ieugwaspy-1.0.0/ieugwaspy/backwards.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Backwards compatibility for old IDs
 """
 
 
 def legacy_ids(study_ids):
     """Handle legacy study IDs, returning the new format
 
-    Parameters:
+    Args:
         study_ids: List of study IDs (new or old)
 
     Returns:
         result: List of new study IDs
 
     """
     legacy_id_subs = {
```

### Comparing `ieugwaspy-0.1.9/ieugwaspy/variants.py` & `ieugwaspy-1.0.0/ieugwaspy/variants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """SNP/variant helper functions
 """
 
 
-def variants_to_rsid(variants):
-    """This function returns dbSNP rsid for variants provided in chr:pos format, calling the variants_chrpos function for each variant 
+def variants_chrpos(chrpos):
+    """This function returns the dbSNP rsid for a single variant in chr:pos format. Note: only the first rsid will be returned
 
-    Parameters:
-        variants: list of variants in chr:pos format (Python list) (leaves rsids unchanged)
+    Args:
+        chrpos (str): variant in `chr:pos` format
 
     Returns:
-        data: list of variant rsids (Python list)
+        result: single variant rsid string
 
     """
-    for pos, variant in enumerate(variants):
-        if variant.find(":") > 0:
-            variants[pos] = variants_chrpos(variant)
-    variants = list(dict.fromkeys(variants))
-    return variants
+    import ieugwaspy.query as query
+
+    variantdata = query._api_query("variants/chrpos/{}".format(chrpos))
+    result = variantdata[0][0]["_id"]
+    return result
 
 
-def variants_chrpos(chrpos, radius=0):
-    """This function returns the dbSNP rsid for a single variant in chr:pos format
+def variants_to_rsid(variants):
+    """This function returns dbSNP rsid for variants provided in chr:pos format, calling the variants_chrpos() function for each variant. Note: only one rsid will be returned for each chr:pos
 
-    Parameters:
-        chrpos: variant in chr:pos format (string)
+    Args:
+        variants (list): variants in chr:pos format (leaves rsids unchanged), e.g. ["rs1234", "10:44865737"]
 
     Returns:
-        data: variant rsid (string)
+        variants: list of variant rsids
 
     """
-    import ieugwaspy.query as query
-
-    variantdata = query.api_query("variants/chrpos/{}".format(chrpos))
-    result = variantdata[0][0]["_id"]
-    return result
+    for pos, variant in enumerate(variants):
+        if variant.find(":") > 0:
+            variants[pos] = variants_chrpos(variant)
+    return variants
```

### Comparing `ieugwaspy-0.1.9/ieugwaspy.egg-info/PKG-INFO` & `ieugwaspy-1.0.0/ieugwaspy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: ieugwaspy
-Version: 0.1.9
+Version: 1.0.0
 Summary: Python interface to IEU GWAS database API
 Home-page: https://mrcieu.github.io/ieugwaspy/
 Author: Tom Gaunt
 Author-email: tom@biocompute.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: retry
 
 # Perform fast queries in Python against a massive database of complete GWAS summary data
 
 [![Actions Status](https://github.com/MRCIEU/ieugwaspy/workflows/ieugwaspy_test/badge.svg)](https://github.com/MRCIEU/ieugwaspy/actions)
 
-The [IEU GWAS database](https://gwas.mrcieu.ac.uk/) comprises over 10,000 curated, QC'd and harmonised complete GWAS summary datasets and can be queried using an API. See [here](http://gwasapi.mrcieu.ac.uk/docs/) for documentation on the API itself. This Python package package is a wrapper to make generic calls to the API, plus convenience functions for specific queries.
+The [IEU OpenGWAS database](https://gwas.mrcieu.ac.uk/) comprises over 50,000 curated, QC'd and harmonised complete GWAS summary datasets and can be queried using an API. See [here](https://api.opengwas.io/api/) for documentation on the API itself. This Python package is a wrapper to make generic calls to the API, plus convenience functions for specific queries.
 
 [See ieugwaspy documentation](https://mrcieu.github.io/ieugwaspy/) for details of how to use this package.
 
-### Installation:
+### Installation
 
 Install using ```pip install ieugwaspy```
 
-### Features:
+### Features
 
 - Get meta data about specific or all studies
 - Obtain the top hits (with on the fly clumping as an option) from each of the GWAS datasets. Clumping and significance thresholds can be specified
 - Obtain the summary results of specific variants across specific studies. LD-proxy lookups are performed automatically if a specific variant is absent from a study
 - Perform PheWAS (look up all associations for a variant)
 - Convert between chromosome:position and rsids and getting annotations
+
+
+#### Developer notes
+To run tests, use `pytest -v -s --select-api="dev"`
+To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
```

### Comparing `ieugwaspy-0.1.9/setup.py` & `ieugwaspy-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="ieugwaspy",
-    version="0.1.9",
+    version="1.0.0",
     author="Tom Gaunt",
     author_email="tom@biocompute.org.uk",
     description="Python interface to IEU GWAS database API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mrcieu.github.io/ieugwaspy/",
     packages=setuptools.find_packages(),
```

