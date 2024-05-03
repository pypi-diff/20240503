# Comparing `tmp/pytestomatio-2.3.4.tar.gz` & `tmp/pytestomatio-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.3.4.tar", last modified: Wed May  1 16:32:43 2024, max compression
+gzip compressed data, was "pytestomatio-2.3.6.tar", last modified: Fri May  3 10:31:37 2024, max compression
```

## Comparing `pytestomatio-2.3.4.tar` & `pytestomatio-2.3.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.762367 pytestomatio-2.3.4/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/pytestomatio/decor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/decor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/decor/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/decor/pep8.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/s3_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/testItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/pytestomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-01 16:32:43.000000 pytestomatio-2.3.4/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 16:32:43.000000 pytestomatio-2.3.4/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:32:43.000000 pytestomatio-2.3.4/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 16:32:43.000000 pytestomatio-2.3.4/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 16:32:43.000000 pytestomatio-2.3.4/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 16:32:43.000000 pytestomatio-2.3.4/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:43.766367 pytestomatio-2.3.4/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-01 16:32:39.000000 pytestomatio-2.3.4/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.243976 pytestomatio-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-03 10:31:37.243976 pytestomatio-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.239976 pytestomatio-2.3.6/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.239976 pytestomatio-2.3.6/pytestomatio/decor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/decor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/decor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/decor/pep8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/s3_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/testItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/pytestomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.243976 pytestomatio-2.3.6/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-03 10:31:37.000000 pytestomatio-2.3.6/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-03 10:31:37.000000 pytestomatio-2.3.6/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:31:37.000000 pytestomatio-2.3.6/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 10:31:37.000000 pytestomatio-2.3.6/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 10:31:37.000000 pytestomatio-2.3.6/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 10:31:37.000000 pytestomatio-2.3.6/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:31:37.243976 pytestomatio-2.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.239976 pytestomatio-2.3.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.243976 pytestomatio-2.3.6/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:37.243976 pytestomatio-2.3.6/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-03 10:31:31.000000 pytestomatio-2.3.6/tests/test_root.py
```

### Comparing `pytestomatio-2.3.4/LICENSE` & `pytestomatio-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/PKG-INFO` & `pytestomatio-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.4
+Version: 2.3.6
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.3.4/README.md` & `pytestomatio-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pyproject.toml` & `pytestomatio-2.3.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.3.4"
+version = "2.3.6"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest>7.2.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1",
@@ -36,15 +36,14 @@
     "Framework :: Pytest",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.pytest.ini_options]
-plugins = ["dotenv"]
 
 [project.urls]
 "Testomat.io" = "https://testomat.io/"
 "Homepage" = "https://github.com/testomatio/pytestomatio"
 "Bug Tracker" = "https://github.com/testomatio/pytestomatio/issues"
 
 [project.entry-points.pytest11]
```

### Comparing `pytestomatio-2.3.4/pytestomatio/code_collector.py` & `pytestomatio-2.3.6/pytestomatio/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/connector.py` & `pytestomatio-2.3.6/pytestomatio/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     def create_test_run(self, title: str, group_title, env: str, label: str, shared_run: bool, parallel) -> dict | None:
         request = {
             "api_key": self.api_key,
             "title": title,
             "group_title": group_title,
             "env": env,
             "label": label,
-            "parallel": parallel,
-            "shared_run": shared_run,
+            "parallel": True,
+            "shared_run": True,
         }
         filtered_request = {k: v for k, v in request.items() if v is not None}
         print('create_test_run', filtered_request)
         try:
             response = self.session.post(f'{self.base_url}/api/reporter', json=filtered_request)
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
@@ -99,16 +99,16 @@
     def update_test_run(self, id: str, title: str, group_title, env: str, label: str, shared_run: bool, parallel) -> dict | None:
         request = {
             "api_key": self.api_key,
             "title": title,
             "group_title": group_title,
             #"env": env, TODO: enabled when bug with 500 response fixed
             #"label": label, TODO: enabled when bug with 500 response fixed
-            "parallel": parallel,
-            "shared_run": shared_run
+            "parallel": True,
+            "shared_run": True
         }
         filtered_request = {k: v for k, v in request.items() if v is not None}
         
         try:
             response = self.session.put(f'{self.base_url}/api/reporter/{id}', json=filtered_request)
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
@@ -166,15 +166,15 @@
             log.error(f'Generic exception happened. Please report an issue. {e}')
             return
         if response.status_code == 200:
             log.info('Test status updated')
 
     # TODO: I guess this class should be just an API client and used within testRun (testRunConfig)
     def finish_test_run(self, run_id: str) -> None:
-        is_parallel = getenv('TESTOMATIO_SHARED_RUN') in ['True', 'true', '1']
+        is_parallel = getenv('TESTOMATIO_SHARED_RUN', 'false').lower() in ['true', '1']
         status_event = "finish_parallel" if is_parallel else 'finish'
         try:
             self.session.put(f'{self.base_url}/api/reporter/{run_id}?api_key={self.api_key}',
                              json={"status_event": status_event})
         except ConnectionError:
             log.error(f'Failed to connect to {self.base_url}')
             return
```

### Comparing `pytestomatio-2.3.4/pytestomatio/decor/default.py` & `pytestomatio-2.3.6/pytestomatio/decor/default.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/decor/pep8.py` & `pytestomatio-2.3.6/pytestomatio/decor/pep8.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/decorator_updater.py` & `pytestomatio-2.3.6/pytestomatio/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/helper.py` & `pytestomatio-2.3.6/pytestomatio/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/main.py` & `pytestomatio-2.3.6/pytestomatio/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     pytest.testomatio = Testomatio()
     test_run_config = TestRunConfig(
         id=os.environ.get('TESTOMATIO_RUN'),
         title=os.environ.get('TESTOMATIO_TITLE'),
         group_title=os.environ.get('TESTOMATIO_RUNGROUP_TITLE'),
         environment=os.environ.get('TESTOMATIO_ENV'),
-        shared_run=os.environ.get('TESTOMATIO_SHARED_RUN') in ['True', 'true', '1'],
+        shared_run=os.environ.get('TESTOMATIO_SHARED_RUN', default='false').lower() in ['true', '1'],
         label=os.environ.get('TESTOMATIO_LABEL'),
     )
     pytest.testomatio.set_test_run(test_run_config)
     pytest.s3_connector = pytest.testomatio.s3_connector  # backward compatibility
 
     if config.getoption(testomatio) in ('sync', 'report', 'remove'):
         url = config.getini('testomatio_url')
```

### Comparing `pytestomatio-2.3.4/pytestomatio/s3_connector.py` & `pytestomatio-2.3.6/pytestomatio/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/testItem.py` & `pytestomatio-2.3.6/pytestomatio/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio/testRunConfig.py` & `pytestomatio-2.3.6/pytestomatio/testRunConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def __init__(
             self,
             id: str = None,
             title: str = None,
             group_title: str = None,
             environment: str = None,
             label: str = None,
-            parallel: bool = False,
-            shared_run: bool = False
+            parallel: bool = True,
+            shared_run: bool = True
         ):
         self.test_run_id = id
         self.title = title if title else 'test run at ' + dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.environment = self.safe_string_list(environment)
         self.label = self.safe_string_list(label)
         self.group_title = group_title
         self.parallel = parallel
```

### Comparing `pytestomatio-2.3.4/pytestomatio/testomatio.py` & `pytestomatio-2.3.6/pytestomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.3.6/pytestomatio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.3.4
+Version: 2.3.6
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.3.4/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.3.6/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.3.4/tests/test_root.py` & `pytestomatio-2.3.6/tests/test_root.py`

 * *Files identical despite different names*

