# Comparing `tmp/processing_pypelines-0.0.56.tar.gz` & `tmp/processing_pypelines-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing_pypelines-0.0.56.tar", last modified: Wed Apr 10 21:23:23 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.57.tar", last modified: Fri May  3 16:41:44 2024, max compression
```

## Comparing `processing_pypelines-0.0.56.tar` & `processing_pypelines-0.0.57.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-04-10 21:23:11.892750 processing_pypelines-0.0.56/LICENSE
--rw-r--r--   0        0        0      118 2024-04-10 21:23:11.892750 processing_pypelines-0.0.56/README.md
--rw-r--r--   0        0        0     1152 2024-04-10 21:23:23.196619 processing_pypelines-0.0.56/pyproject.toml
--rw-r--r--   0        0        0      367 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/__init__.py
--rw-r--r--   0        0        0     4483 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/accessors.py
--rw-r--r--   0        0        0     4633 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/arguments.py
--rw-r--r--   0        0        0    34226 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/celery_tasks.py
--rw-r--r--   0        0        0    11851 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/disk.py
--rw-r--r--   0        0        0     6647 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/examples.py
--rw-r--r--   0        0        0   352259 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/feature_test.ipynb
--rw-r--r--   0        0        0     7880 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/graphs.py
--rw-r--r--   0        0        0    17038 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/loggs.py
--rw-r--r--   0        0        0     5985 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/multisession.py
--rw-r--r--   0        0        0    18914 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/pickle_backend.py
--rw-r--r--   0        0        0     6559 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/pipelines.py
--rw-r--r--   0        0        0     8676 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/pipes.py
--rw-r--r--   0        0        0     3084 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/sessions.py
--rw-r--r--   0        0        0    36877 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/steps.py
--rw-r--r--   0        0        0     3915 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/tasks.py
--rw-r--r--   0        0        0     7360 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/versions.py
--rw-r--r--   0        0        0        0 2024-04-10 21:23:11.980749 processing_pypelines-0.0.56/tests/__init__.py
--rw-r--r--   0        0        0      962 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/tests/tests.py
--rw-r--r--   0        0        0     1230 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/tests/versions_example.json
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 processing_pypelines-0.0.56/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-03 16:41:34.858793 processing_pypelines-0.0.57/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-03 16:41:34.858793 processing_pypelines-0.0.57/README.md
+-rw-r--r--   0        0        0     1152 2024-05-03 16:41:44.130626 processing_pypelines-0.0.57/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4633 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34226 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-05-03 16:41:34.862793 processing_pypelines-0.0.57/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17038 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6559 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     9444 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    37032 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-05-03 16:41:34.866793 processing_pypelines-0.0.57/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-05-03 16:41:34.870793 processing_pypelines-0.0.57/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:41:34.918792 processing_pypelines-0.0.57/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-03 16:41:34.870793 processing_pypelines-0.0.57/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-05-03 16:41:34.870793 processing_pypelines-0.0.57/tests/versions_example.json
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.57/PKG-INFO
```

### Comparing `processing_pypelines-0.0.56/LICENSE` & `processing_pypelines-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/pyproject.toml` & `processing_pypelines-0.0.57/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = []
-version = "0.0.56"
+version = "0.0.57"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 celery = [
     "celery>=5.3.5",
```

### Comparing `processing_pypelines-0.0.56/src/pypelines/accessors.py` & `processing_pypelines-0.0.57/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/arguments.py` & `processing_pypelines-0.0.57/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.57/src/pypelines/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/disk.py` & `processing_pypelines-0.0.57/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/examples.py` & `processing_pypelines-0.0.57/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/feature_test.ipynb` & `processing_pypelines-0.0.57/src/pypelines/feature_test.ipynb`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/graphs.py` & `processing_pypelines-0.0.57/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/loggs.py` & `processing_pypelines-0.0.57/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/multisession.py` & `processing_pypelines-0.0.57/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.57/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/pipelines.py` & `processing_pypelines-0.0.57/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/pipes.py` & `processing_pypelines-0.0.57/src/pypelines/pipes.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from .multisession import BaseMultisessionAccessor
 from .sessions import Session
 from .disk import BaseDiskObject
 
 from functools import wraps
 import inspect, hashlib
 
+from pandas import DataFrame
+
 from abc import ABCMeta, abstractmethod
 
 from typing import Callable, Type, Iterable, Protocol, TYPE_CHECKING, Literal, Dict
 from types import MethodType
 
 if TYPE_CHECKING:
     from .pipelines import Pipeline
@@ -204,11 +206,27 @@
         else:
             reverse = True
 
         ordered_steps = sorted(
             list(self.steps.values()), key=lambda item: item.get_level(selfish=True), reverse=reverse
         )
 
+        highest_step = None
+
+        if isinstance(session, DataFrame):
+            # if multisession, we assume we are trying to just load sessions
+            # that all have reached the same level of requirements. (otherwise, use generate)
+            # because of that, we use only the first session in the lot to search the highest loadable step
+            search_on_session = session.iloc[0]
+        else:
+            search_on_session = session
+
         for step in ordered_steps:
-            if step.get_disk_object(session, extra).is_matching():
-                return step.load(session, extra)
+            if step.get_disk_object(search_on_session, extra).is_matching():
+                highest_step = step
+
+        if highest_step is not None:  # if we found one : it is not None
+            # we use the load wrapper, wich will dispatch to multissession or not automatically,
+            # depending on session type (Series or DataFrame)
+            return highest_step.load(session, extra)
+
         raise ValueError(f"Could not find a {self} object to load for the session {session.alias} with extra {extra}")
```

### Comparing `processing_pypelines-0.0.56/src/pypelines/sessions.py` & `processing_pypelines-0.0.57/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/steps.py` & `processing_pypelines-0.0.57/src/pypelines/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import wraps, partial, update_wrapper
 from .loggs import loggedmethod, NAMELENGTH
 from .arguments import autoload_arguments
-import logging, inspect
 
+import logging, inspect
+from pandas import DataFrame
 from dataclasses import dataclass
 
 from types import MethodType
 from typing import Callable, Type, Iterable, Protocol, List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .pipelines import Pipeline
@@ -254,14 +255,17 @@
             Returns:
                 The loaded disk object.
 
             Raises:
                 ValueError: If the disk object does not match and has a status message.
             """
             # print("extra in load wrapper : ", extra)
+            if isinstance(session, DataFrame):
+                return self.multisession.load(sessions=session, extras=extra)
+
             if extra is None:
                 extra = self.get_default_extra()
             # print("extra in load wrapper after None : ", extra)
             self.pipeline.resolve()
             disk_object = self.get_disk_object(session, extra)
             if not disk_object.is_matching():
                 raise ValueError(disk_object.get_status_message())
```

### Comparing `processing_pypelines-0.0.56/src/pypelines/tasks.py` & `processing_pypelines-0.0.57/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/src/pypelines/versions.py` & `processing_pypelines-0.0.57/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/tests/tests.py` & `processing_pypelines-0.0.57/tests/tests.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/tests/versions_example.json` & `processing_pypelines-0.0.57/tests/versions_example.json`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.56/PKG-INFO` & `processing_pypelines-0.0.57/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.56
+Version: 0.0.57
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Home-page: https://gitlab.pasteur.fr/haisslab/data-management/pypelines
-Author-Email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
-Maintainer-Email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
+Author-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
+Maintainer-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Requires-Python: >=3.10
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: dynaconf>=3.2.4
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

