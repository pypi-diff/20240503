# Comparing `tmp/glue_utils-0.2.0.tar.gz` & `tmp/glue_utils-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.0.tar", max compression
+gzip compressed data, was "glue_utils-0.2.1rc1.tar", max compression
```

## Comparing `glue_utils-0.2.0.tar` & `glue_utils-0.2.1rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.0/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.0/README.md
--rw-r--r--   0        0        0     3312 2024-05-02 06:54:14.343575 glue_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       96 2024-05-02 06:55:10.579843 glue_utils-0.2.0/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-02 06:53:45.157325 glue_utils-0.2.0/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-02 06:53:45.157808 glue_utils-0.2.0/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0      982 2024-05-02 06:53:45.158192 glue_utils-0.2.0/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-02 06:53:45.158255 glue_utils-0.2.0/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 glue_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.1rc1/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.1rc1/README.md
+-rw-r--r--   0        0        0     3315 2024-05-03 06:49:17.235811 glue_utils-0.2.1rc1/pyproject.toml
+-rw-r--r--   0        0        0       99 2024-05-03 06:49:37.866944 glue_utils-0.2.1rc1/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-02 06:53:45.157325 glue_utils-0.2.1rc1/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     2695 2024-05-03 06:44:56.735881 glue_utils-0.2.1rc1/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0      982 2024-05-02 06:53:45.158192 glue_utils-0.2.1rc1/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:53:45.158255 glue_utils-0.2.1rc1/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 glue_utils-0.2.1rc1/PKG-INFO
```

### Comparing `glue_utils-0.2.0/LICENSE` & `glue_utils-0.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.0/README.md` & `glue_utils-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.0/pyproject.toml` & `glue_utils-0.2.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.0"
+version = "0.2.1rc1"
 # Uncomment this when dependabot has finally been updated to it is 
 # supported by dependabot.
 # package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `glue_utils-0.2.0/src/glue_utils/glueetl/job.py` & `glue_utils-0.2.1rc1/src/glue_utils/glueetl/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 """Module providing the GlueETLJob class for handling Glue ETL jobs."""
 
 import sys
 from collections.abc import Generator
 from contextlib import contextmanager
 from dataclasses import fields
-from typing import Generic
+from typing import Generic, cast, overload
 
 from awsglue.context import GlueContext
 from awsglue.job import Job
 from awsglue.utils import getResolvedOptions
 from pyspark import SparkConf, SparkContext
 from pyspark.sql import SparkSession
 from typing_extensions import TypeVar
 
 from glue_utils import BaseOptions
 
-T = TypeVar("T", bound=BaseOptions)
+T = TypeVar("T", bound=BaseOptions, default=BaseOptions)
 
 
 class GlueETLJob(Generic[T]):
     """A class that handles the boilerplate setup for Glue ETL jobs."""
 
     options: T
     glue_context: GlueContext
     spark: SparkSession
 
+    @overload
+    def __init__(
+        self: "GlueETLJob[BaseOptions]",
+    ) -> None: ...
+
+    @overload
+    def __init__(
+        self: "GlueETLJob[T]",
+        *,
+        options_cls: type[T],
+    ) -> None: ...
+
     def __init__(
         self,
         *,
-        options_cls: type[T] = BaseOptions,  # type: ignore[assignment]
+        options_cls: type[T] | type[BaseOptions] = BaseOptions,
     ) -> None:
-        """Initialize the GlueETLJob."""
+        """Initialize the GlueETLJob.
+
+        Parameters
+        ----------
+        options_cls, optional
+            Has to be a subclass of BaseOptions, by default BaseOptions
+
+        """
+        if not issubclass(options_cls, BaseOptions):
+            msg = "options_cls must be a subclass of BaseOptions."
+            raise TypeError(msg)
+
         job_options = getResolvedOptions(
             sys.argv,
             [field.name for field in fields(options_cls)],
         )
 
-        self.options = options_cls.from_resolved_options(job_options)
+        self.options = cast(T, options_cls.from_resolved_options(job_options))
 
         self.glue_context = self.create_glue_context()
         self.spark = self.glue_context.spark_session
 
         self._job = Job(self.glue_context)
         self._job.init(self.options.JOB_NAME, job_options)
```

### Comparing `glue_utils-0.2.0/src/glue_utils/options.py` & `glue_utils-0.2.1rc1/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.0/PKG-INFO` & `glue_utils-0.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.0
+Version: 0.2.1rc1
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.10,<4.0
```

