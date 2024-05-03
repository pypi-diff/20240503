# Comparing `tmp/skt-0.2.98.tar.gz` & `tmp/skt-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skt-0.2.98.tar", last modified: Thu Nov 23 23:33:01 2023, max compression
+gzip compressed data, was "skt-0.2.99.tar", last modified: Fri Nov 24 00:48:53 2023, max compression
```

## Comparing `skt-0.2.98.tar` & `skt-0.2.99.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 23:33:01.249597 skt-0.2.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-11-23 23:32:56.000000 skt-0.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2023-11-23 23:33:01.249597 skt-0.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-23 23:32:56.000000 skt-0.2.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-23 23:32:56.000000 skt-0.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-11-23 23:33:01.249597 skt-0.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-11-23 23:32:56.000000 skt-0.2.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 23:33:01.245597 skt-0.2.98/skt/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-23 23:32:56.000000 skt-0.2.98/skt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2023-11-23 23:32:56.000000 skt-0.2.98/skt/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-11-23 23:32:56.000000 skt-0.2.98/skt/data_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2023-11-23 23:32:56.000000 skt-0.2.98/skt/eda_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    29856 2023-11-23 23:32:56.000000 skt-0.2.98/skt/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2023-11-23 23:32:56.000000 skt-0.2.98/skt/gcp_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-11-23 23:32:56.000000 skt-0.2.98/skt/github_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2023-11-23 23:32:56.000000 skt-0.2.98/skt/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-11-23 23:32:56.000000 skt-0.2.98/skt/lake.py
--rw-r--r--   0 runner    (1001) docker     (127)    18513 2023-11-23 23:32:56.000000 skt-0.2.98/skt/mls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 23:33:01.249597 skt-0.2.98/skt/model/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-23 23:32:56.000000 skt-0.2.98/skt/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2023-11-23 23:32:56.000000 skt-0.2.98/skt/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-11-23 23:32:56.000000 skt-0.2.98/skt/nes.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-11-23 23:32:56.000000 skt-0.2.98/skt/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-23 23:32:56.000000 skt-0.2.98/skt/vault_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14898 2023-11-23 23:32:56.000000 skt-0.2.98/skt/ye.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 23:33:01.249597 skt-0.2.98/skt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2023-11-23 23:33:01.000000 skt-0.2.98/skt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-23 23:33:01.000000 skt-0.2.98/skt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 23:33:01.000000 skt-0.2.98/skt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-23 23:33:01.000000 skt-0.2.98/skt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-11-23 23:33:01.000000 skt-0.2.98/skt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-23 23:33:01.000000 skt-0.2.98/skt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 00:48:53.645909 skt-0.2.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-11-24 00:48:50.000000 skt-0.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2023-11-24 00:48:53.645909 skt-0.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-24 00:48:50.000000 skt-0.2.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-24 00:48:50.000000 skt-0.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-11-24 00:48:53.645909 skt-0.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-11-24 00:48:50.000000 skt-0.2.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 00:48:53.641909 skt-0.2.99/skt/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-24 00:48:50.000000 skt-0.2.99/skt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2023-11-24 00:48:50.000000 skt-0.2.99/skt/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2023-11-24 00:48:50.000000 skt-0.2.99/skt/data_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2023-11-24 00:48:50.000000 skt-0.2.99/skt/eda_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29874 2023-11-24 00:48:50.000000 skt-0.2.99/skt/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2023-11-24 00:48:50.000000 skt-0.2.99/skt/gcp_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-11-24 00:48:50.000000 skt-0.2.99/skt/github_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2023-11-24 00:48:50.000000 skt-0.2.99/skt/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-11-24 00:48:50.000000 skt-0.2.99/skt/lake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18513 2023-11-24 00:48:50.000000 skt-0.2.99/skt/mls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 00:48:53.645909 skt-0.2.99/skt/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-24 00:48:50.000000 skt-0.2.99/skt/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2023-11-24 00:48:50.000000 skt-0.2.99/skt/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-11-24 00:48:50.000000 skt-0.2.99/skt/nes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2023-11-24 00:48:50.000000 skt-0.2.99/skt/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-24 00:48:50.000000 skt-0.2.99/skt/vault_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14898 2023-11-24 00:48:50.000000 skt-0.2.99/skt/ye.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-24 00:48:53.645909 skt-0.2.99/skt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2023-11-24 00:48:53.000000 skt-0.2.99/skt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-24 00:48:53.000000 skt-0.2.99/skt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-24 00:48:53.000000 skt-0.2.99/skt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-24 00:48:53.000000 skt-0.2.99/skt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2023-11-24 00:48:53.000000 skt-0.2.99/skt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-24 00:48:53.000000 skt-0.2.99/skt.egg-info/top_level.txt
```

### Comparing `skt-0.2.98/LICENSE` & `skt-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/PKG-INFO` & `skt-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skt
-Version: 0.2.98
+Version: 0.2.99
 Summary: SKT package
 Home-page: https://github.com/sktaiflow/skt
 Author: SKT
 Author-email: all@sktai.io
 License: UNKNOWN
 Description: # SKT Package
```

### Comparing `skt-0.2.98/README.md` & `skt-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/setup.py` & `skt-0.2.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "haversine",
     "pyfarmhash",
     "mabalgs",
 ]
 
 setuptools.setup(
     name="skt",
-    version="0.2.98",
+    version="0.2.99",
     author="SKT",
     author_email="all@sktai.io",
     description="SKT package",
     long_description=load_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/sktaiflow/skt",
     packages=setuptools.find_packages(),
```

### Comparing `skt-0.2.98/skt/data_catalog.py` & `skt-0.2.99/skt/data_catalog.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/data_lineage.py` & `skt-0.2.99/skt/data_lineage.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/eda_tools.py` & `skt-0.2.99/skt/eda_tools.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/gcp.py` & `skt-0.2.99/skt/gcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
     nes_client_context = os.environ.get("CLIENT_CONTEXT")
     if nes_client_context:
         nes_client_context_dict = json.loads(nes_client_context)
         job_config_labels.update(nes_client_context_dict)
 
     for k, v in job_config_labels.items():
-        job_config_labels.update({k: v.lower() if v else v})
+        job_config_labels.update({k: v.lower().replace(".", "_") if v else v})
 
     return bigquery.Client(
         credentials=credentials,
         project=project_id,
         location=location,
         default_query_job_config=QueryJobConfig(labels=job_config_labels),
     )
```

### Comparing `skt-0.2.98/skt/gcp_credentials.py` & `skt-0.2.99/skt/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/github_utils.py` & `skt-0.2.99/skt/github_utils.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/hashing.py` & `skt-0.2.99/skt/hashing.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/lake.py` & `skt-0.2.99/skt/lake.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/mls.py` & `skt-0.2.99/skt/mls.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/model/utils.py` & `skt-0.2.99/skt/model/utils.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/nes.py` & `skt-0.2.99/skt/nes.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/spark_utils.py` & `skt-0.2.99/skt/spark_utils.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt/ye.py` & `skt-0.2.99/skt/ye.py`

 * *Files identical despite different names*

### Comparing `skt-0.2.98/skt.egg-info/PKG-INFO` & `skt-0.2.99/skt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skt
-Version: 0.2.98
+Version: 0.2.99
 Summary: SKT package
 Home-page: https://github.com/sktaiflow/skt
 Author: SKT
 Author-email: all@sktai.io
 License: UNKNOWN
 Description: # SKT Package
```

### Comparing `skt-0.2.98/skt.egg-info/requires.txt` & `skt-0.2.99/skt.egg-info/requires.txt`

 * *Files identical despite different names*

