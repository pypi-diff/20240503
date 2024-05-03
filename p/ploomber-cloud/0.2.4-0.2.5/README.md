# Comparing `tmp/ploomber-cloud-0.2.4.tar.gz` & `tmp/ploomber-cloud-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.4.tar", last modified: Thu May  2 14:11:57 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.5.tar", last modified: Thu May  2 18:06:32 2024, max compression
```

## Comparing `ploomber-cloud-0.2.4.tar` & `ploomber-cloud-0.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.609134 ploomber-cloud-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.169358 ploomber-cloud-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.173358 ploomber-cloud-0.2.5/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-02 18:06:16.000000 ploomber-cloud-0.2.5/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:06:32.177358 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 18:06:31.000000 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 18:06:31.000000 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:06:31.000000 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 18:06:31.000000 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 18:06:31.000000 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 18:06:31.000000 ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.4/CHANGELOG.md` & `ploomber-cloud-0.2.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.2.5 (2024-05-02)
+
+- [Feature] Add `--watch-incremental` option to `ploomber-cloud deploy`.
+
 ## 0.2.4 (2024-05-02)
 
 - [Feature] Allow deploying secrets using `secret-keys` in `ploomber-cloud.json`
 
 ## 0.2.3 (2024-04-26)
 
 - [Feature] Add `ploomber-cloud labels` for adding or deleting labels of the project.
```

### Comparing `ploomber-cloud-0.2.4/pyproject.toml` & `ploomber-cloud-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/setup.py` & `ploomber-cloud-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -201,7 +201,17 @@
         """Updates labels for an application"""
         response = requests.put(
             f"{API_ROOT}/projects/{project_id}/labels",
             json=labels,
             headers=self._get_headers(),
         )
         return self._process_response(response)
+
+    def get_job_logs_by_id_and_timestamp(self, id, start_time):
+        """Return docker logs and webservice logs by job id
+        and starting from a particular timestamp"""
+        response = requests.get(
+            f"{API_ROOT}/jobs/{id}/logs",
+            params={"start_time": start_time},
+            headers=self._get_headers(),
+        )
+        return self._process_response(response)
```

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,23 @@
     api_key.set_api_key(key)
 
 
 @cli.command()
 @click.option(
     "--watch", is_flag=True, help="Track deployment status in the command line"
 )
-def deploy(watch):
+@click.option(
+    "--watch-incremental",
+    "watch_incremental",
+    is_flag=True,
+    help="Track incremental deployment logs in the command line",
+)
+def deploy(watch, watch_incremental):
     """Deploy your project to Ploomber Cloud"""
-    deploy_.deploy(watch)
+    deploy_.deploy(watch, watch_incremental)
 
 
 @cli.command()
 @click.option(
     "--project-id",
     "project_id",
     type=str,
```

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/config.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.5/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.5/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,7 @@
 )
 
 CONFIGURE_RESOURCES_MESSAGE = (
     "To configure resources for this project, run "
     "'ploomber-cloud resources' or to deploy with default "
     "configurations, run 'ploomber-cloud deploy'"
 )
-
-ADD_LABELS_MESSAGE = (
-    "To add labels to the project, run 'ploomber-cloud "
-    "labels --add <label>. To learn more, "
-    "refer to the documentation: "
-    "https://docs.cloud.ploomber.io/en/latest/user-guide/cli.html#add-labels"
-)  # noqa
```

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     examples_choices = []
     for ex in examples[selected_framework].keys():
         title = examples[selected_framework][ex]["title"]
         description = examples[selected_framework][ex]["description"]
         examples_choices.append(f"{title}: {description}")
 
     selected_example_index = util.prompt_for_choice_from_list(
-        examples_choices, f"\nChoose a {selected_framework} example:\n", index=True
+        examples_choices, f"\nChoose a {selected_framework} example", index=True
     )
 
     if selected_example_index is None:
         quit()
 
     selected_example_title = list(examples[selected_framework].keys())[
         selected_example_index
```

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 from ploomber_cloud.constants import (
     VALID_PROJECT_TYPES,
     VALID_DOCKER_PROJECT_TYPES,
     RETAINED_RESOURCES_WARNING,
     CONFIGURE_RESOURCES_MESSAGE,
     RETAINED_LABELS_WARNING,
-    ADD_LABELS_MESSAGE,
 )
 from ploomber_cloud.config import PloomberCloudConfig
 from ploomber_cloud.github import display_github_workflow_info_message
 from ploomber_cloud._telemetry import telemetry
 from ploomber_cloud.util import pretty_print
 
 
@@ -194,10 +193,10 @@
             output["labels"] = labels
             click.echo(RETAINED_LABELS_WARNING.format(labels=pretty_print(labels)))
 
         config.dump(output)
         click.echo(f"Your app {output['id']!r} has been configured successfully!")
 
         if not force:
-            click.echo(f"{CONFIGURE_RESOURCES_MESSAGE}\n{ADD_LABELS_MESSAGE}")
+            click.echo(f"{CONFIGURE_RESOURCES_MESSAGE}")
 
         display_github_workflow_info_message()
```

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/io.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/io.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/labels.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/labels.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/templates.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/templates.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.5/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.5/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

