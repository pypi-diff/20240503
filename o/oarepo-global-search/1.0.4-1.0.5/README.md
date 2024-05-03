# Comparing `tmp/oarepo_global_search-1.0.4.tar.gz` & `tmp/oarepo_global_search-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_global_search-1.0.4.tar", last modified: Mon Apr 22 10:18:28 2024, max compression
+gzip compressed data, was "oarepo_global_search-1.0.5.tar", last modified: Fri May  3 07:45:48 2024, max compression
```

## Comparing `oarepo_global_search-1.0.4.tar` & `oarepo_global_search-1.0.5.tar`

### file list

```diff
@@ -1,38 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.237913 oarepo_global_search-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-22 10:18:28.237913 oarepo_global_search-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.233913 oarepo_global_search-1.0.4/oarepo_global_search/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.233913 oarepo_global_search-1.0.4/oarepo_global_search/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.233913 oarepo_global_search-1.0.4/oarepo_global_search/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.233913 oarepo_global_search-1.0.4/oarepo_global_search/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.237913 oarepo_global_search-1.0.4/oarepo_global_search/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/records/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/records/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/services/records/user_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.237913 oarepo_global_search-1.0.4/oarepo_global_search/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/oarepo_global_search/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:18:28.237913 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-22 10:18:28.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-22 10:18:28.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:18:28.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-22 10:18:28.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:15:29.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 10:18:28.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 10:18:28.000000 oarepo_global_search-1.0.4/oarepo_global_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-22 10:18:28.237913 oarepo_global_search-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-22 10:14:41.000000 oarepo_global_search-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.375393 oarepo_global_search-1.0.5/oarepo_global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.375393 oarepo_global_search-1.0.5/oarepo_global_search/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/services/records/user_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.371393 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.371393 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/semantic-ui/global_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/oarepo_global_search/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:45:48.379393 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:42:53.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 07:45:48.000000 oarepo_global_search-1.0.5/oarepo_global_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      866 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-03 07:45:48.383393 oarepo_global_search-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 07:42:07.000000 oarepo_global_search-1.0.5/setup.py
```

### Comparing `oarepo_global_search-1.0.4/PKG-INFO` & `oarepo_global_search-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: oarepo-global-search
-Version: 1.0.4
+Version: 1.0.5
 Summary: "A model builder plugin for global search"
 Home-page: https://github.com/oarepo/oarepo-global-search
 Author: Alzbeta Pokorna
 Author-email: Alzbeta.Pokorna@cesnet.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-model-builder>=4.0.0
 Requires-Dist: invenio_records_resources>=0.21.4
+Requires-Dist: oarepo-ui
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: autoflake; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 
 # Global search plugin
```

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search/ext.py` & `oarepo_global_search-1.0.5/oarepo_global_search/ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import json
 from pathlib import Path
 
 from importlib_metadata import entry_points
 from invenio_base.utils import obj_or_import_string
 from invenio_records_resources.proxies import current_service_registry
 
+from oarepo_global_search import config
 from oarepo_global_search.resources.records.config import (
     GlobalSearchResourceConfig,
     GlobalUserSearchResourceConfig,
 )
 from oarepo_global_search.resources.records.resource import GlobalSearchResource
 from oarepo_global_search.services.records.service import GlobalSearchService
 from oarepo_global_search.services.records.user_service import GlobalUserSearchService
-
+from oarepo_global_search.ui.config import GlobalSearchUIResource, GlobalSearchUIResourceConfig
 
 class OARepoGlobalSearch(object):
     """OARepo DOI extension."""
 
     global_search_resource: GlobalSearchResource = None
     global_user_search_resource: GlobalSearchResource = None
 
@@ -54,14 +55,14 @@
         """Init resources."""
         self.global_search_resource = GlobalSearchResource(
             config=GlobalSearchResourceConfig(), service=GlobalSearchService()
         )
         self.global_user_search_resource = GlobalSearchResource(
             config=GlobalUserSearchResourceConfig(), service=GlobalUserSearchService()
         )
+        self.global_search_ui_resource = GlobalSearchUIResource(
+            config=GlobalSearchUIResourceConfig()
+        )
 
-    #
-    # @cached_property
-    # def service_records(self):
-    #     return config.MODELA_RECORD_SERVICE_CLASS(
-    #         config=config.MODELA_RECORD_SERVICE_CONFIG(),
-    #     )
+    @functools.cached_property
+    def service_records(self):
+        return config.GLOBAL_SEARCH_RECORD_SERVICE_CLASS()
```

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search/resources/records/resource.py` & `oarepo_global_search-1.0.5/oarepo_global_search/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search/services/records/params.py` & `oarepo_global_search-1.0.5/oarepo_global_search/services/records/params.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search/services/records/results.py` & `oarepo_global_search-1.0.5/oarepo_global_search/services/records/results.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search/services/records/service.py` & `oarepo_global_search-1.0.5/oarepo_global_search/services/records/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             "GlobalSearchServiceConfig",
             (PermissionsPresetsConfigMixin, InvenioRecordServiceConfig),
             {
                 "PERMISSIONS_PRESETS": ["everyone"],
                 "base_permission_policy_cls": GlobalSearchPermissionPolicy,
                 "result_list_cls": GlobalSearchResultList,
                 "record_cls": Record,
-                # todo is there a use case where this would affect any other links??
+                "url_prefix": "/search",
                 "links_search": pagination_links("{+api}/search{?args*}"),
             },
         )
         return config_class()
 
     @config.setter
     def config(self, value):
```

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search/services/records/user_service.py` & `oarepo_global_search-1.0.5/oarepo_global_search/services/records/user_service.py`

 * *Files identical despite different names*

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search.egg-info/PKG-INFO` & `oarepo_global_search-1.0.5/oarepo_global_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: oarepo-global-search
-Version: 1.0.4
+Version: 1.0.5
 Summary: "A model builder plugin for global search"
 Home-page: https://github.com/oarepo/oarepo-global-search
 Author: Alzbeta Pokorna
 Author-email: Alzbeta.Pokorna@cesnet.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-model-builder>=4.0.0
 Requires-Dist: invenio_records_resources>=0.21.4
+Requires-Dist: oarepo-ui
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: autoflake; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 
 # Global search plugin
```

### Comparing `oarepo_global_search-1.0.4/oarepo_global_search.egg-info/SOURCES.txt` & `oarepo_global_search-1.0.5/oarepo_global_search.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 MANIFEST.in
 README.md
+format.sh
 pyproject.toml
+run-tests.sh
 setup.cfg
 setup.py
 oarepo_global_search/__init__.py
+oarepo_global_search/config.py
 oarepo_global_search/ext.py
 oarepo_global_search/proxies.py
 oarepo_global_search.egg-info/PKG-INFO
 oarepo_global_search.egg-info/SOURCES.txt
 oarepo_global_search.egg-info/dependency_links.txt
 oarepo_global_search.egg-info/entry_points.txt
 oarepo_global_search.egg-info/not-zip-safe
@@ -20,10 +23,14 @@
 oarepo_global_search/services/__init__.py
 oarepo_global_search/services/records/__init__.py
 oarepo_global_search/services/records/params.py
 oarepo_global_search/services/records/permissions.py
 oarepo_global_search/services/records/results.py
 oarepo_global_search/services/records/service.py
 oarepo_global_search/services/records/user_service.py
+oarepo_global_search/ui/__init__.py
+oarepo_global_search/ui/config.py
+oarepo_global_search/ui/views.py
+oarepo_global_search/ui/templates/semantic-ui/global_search/Search.jinja
 oarepo_global_search/views/__init__.py
 oarepo_global_search/views/api.py
 oarepo_global_search/views/app.py
```

### Comparing `oarepo_global_search-1.0.4/setup.cfg` & `oarepo_global_search-1.0.5/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-global-search
-version = 1.0.4
+version = 1.0.5
 description = "A model builder plugin for global search"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Alzbeta Pokorna
 author_email = Alzbeta.Pokorna@cesnet.cz
@@ -16,17 +16,18 @@
 [options]
 packages = find:
 python_requires = >=3.10
 zip_safe = False
 install_requires = 
 	oarepo-model-builder>=4.0.0
 	invenio_records_resources>=0.21.4
+	oarepo-ui
 
 [options.package_data]
-* = *.yaml, *.json, *.json5, *.jinja2
+* = *.json, *.rst, *.md, *.json5, *.jinja2, *.jinja
 
 [options.extras_require]
 tests = 
 	pytest
 	black
 	autoflake
 	isort
@@ -35,16 +36,18 @@
 invenio_base.apps = 
 	oarepo_global_search = oarepo_global_search.ext:OARepoGlobalSearch
 invenio_base.api_apps = 
 	oarepo_global_search_api = oarepo_global_search.ext:OARepoGlobalSearch
 invenio_base.api_blueprints = 
 	oarepo_global_search_api = oarepo_global_search.views.api:create_global_search
 	oarepo_global_user_search_api = oarepo_global_search.views.api:create_global_user_search
+	ui_oarepo_global_search  = oarepo_global_search.ui.config:create_blueprint
 invenio_base.blueprints = 
 	oarepo_global_search = oarepo_global_search.views.app:create_app_blueprint
+	ui_oarepo_global_search  = oarepo_global_search.ui.config:create_blueprint
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
```

