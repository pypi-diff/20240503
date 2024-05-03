# Comparing `tmp/holcstore-0.1.7.tar.gz` & `tmp/holcstore-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holcstore-0.1.7.tar", last modified: Mon Apr 15 08:53:31 2024, max compression
+gzip compressed data, was "holcstore-0.1.8.tar", last modified: Fri May  3 13:59:32 2024, max compression
```

## Comparing `holcstore-0.1.7.tar` & `holcstore-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-15 08:53:27.000000 holcstore-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 08:53:27.000000 holcstore-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 08:53:31.017711 holcstore-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-15 08:53:27.000000 holcstore-0.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.013712 holcstore-0.1.7/holcstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/holcstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/hostore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/hostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/hostore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 08:53:27.000000 holcstore-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 08:53:31.017711 holcstore-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 08:53:27.000000 holcstore-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 13:59:29.000000 holcstore-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 13:59:29.000000 holcstore-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-03 13:59:32.965656 holcstore-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 13:59:29.000000 holcstore-0.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.961656 holcstore-0.1.8/holcstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 13:59:29.000000 holcstore-0.1.8/holcstore/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/holcstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 13:59:32.000000 holcstore-0.1.8/holcstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.961656 holcstore-0.1.8/hostore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/hostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/0004_testdatastore_created_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:32.965656 holcstore-0.1.8/hostore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 13:59:29.000000 holcstore-0.1.8/hostore/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 13:59:29.000000 holcstore-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-03 13:59:32.965656 holcstore-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 13:59:29.000000 holcstore-0.1.8/setup.py
```

### Comparing `holcstore-0.1.7/LICENSE` & `holcstore-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/PKG-INFO` & `holcstore-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.7/README.rst` & `holcstore-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/holcstore/settings.py` & `holcstore-0.1.8/holcstore/settings.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/holcstore/urls.py` & `holcstore-0.1.8/holcstore/urls.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/holcstore.egg-info/PKG-INFO` & `holcstore-0.1.8/holcstore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.7/holcstore.egg-info/SOURCES.txt` & `holcstore-0.1.8/holcstore.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 hostore/manager.py
 hostore/models.py
 hostore/tests.py
 hostore/views.py
 hostore/migrations/0001_initial.py
 hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
 hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+hostore/migrations/0004_testdatastore_created_at.py
 hostore/migrations/__init__.py
 hostore/utils/__init__.py
 hostore/utils/timeseries.py
 hostore/utils/utils.py
```

### Comparing `holcstore-0.1.7/hostore/migrations/0001_initial.py` & `holcstore-0.1.8/hostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py` & `holcstore-0.1.8/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/hostore/models.py` & `holcstore-0.1.8/hostore/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 from django.db import models
 from django.db.models import Max
 from pyarrow import BufferReader
 
 from .manager import StoreQuerySet
 from .utils.timeseries import ts_combine_first, find_constant_sequences, check_ts_completeness
 from .utils.utils import chunks
+from django.utils.timezone import now
 
 logger = logging.getLogger(__name__)
 
 
 class Store(models.Model):
     client_id = models.IntegerField()
     prm = models.CharField(max_length=30)
     last_modified = models.DateTimeField(auto_now=True)
+    created_at = models.DateTimeField(auto_now_add=True, null=True)
     data = models.BinaryField(blank=True, null=True)
     version = models.IntegerField(default=0)
 
     objects = StoreQuerySet.as_manager()
 
     class Meta:
         abstract = True
```

### Comparing `holcstore-0.1.7/hostore/tests.py` & `holcstore-0.1.8/hostore/tests.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/hostore/utils/timeseries.py` & `holcstore-0.1.8/hostore/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.7/setup.cfg` & `holcstore-0.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holcstore
-version = 0.1.7
+version = 0.1.8
 description = A Django App to use a simple load curve store
 long_description = file: README.rst
 url = 
 author = Jean-Pierre Lartigue
 author_email = 
 license = BSD-3-Clause
 classifiers =
```

