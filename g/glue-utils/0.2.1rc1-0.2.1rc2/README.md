# Comparing `tmp/glue_utils-0.2.1rc1.tar.gz` & `tmp/glue_utils-0.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.1rc1.tar", max compression
+gzip compressed data, was "glue_utils-0.2.1rc2.tar", max compression
```

## Comparing `glue_utils-0.2.1rc1.tar` & `glue_utils-0.2.1rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.1rc1/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.1rc1/README.md
--rw-r--r--   0        0        0     3315 2024-05-03 06:49:17.235811 glue_utils-0.2.1rc1/pyproject.toml
--rw-r--r--   0        0        0       99 2024-05-03 06:49:37.866944 glue_utils-0.2.1rc1/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-02 06:53:45.157325 glue_utils-0.2.1rc1/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     2695 2024-05-03 06:44:56.735881 glue_utils-0.2.1rc1/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0      982 2024-05-02 06:53:45.158192 glue_utils-0.2.1rc1/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-02 06:53:45.158255 glue_utils-0.2.1rc1/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 glue_utils-0.2.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.1rc2/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.1rc2/README.md
+-rw-r--r--   0        0        0     3315 2024-05-03 09:24:31.630985 glue_utils-0.2.1rc2/pyproject.toml
+-rw-r--r--   0        0        0       96 2024-05-03 09:05:24.415379 glue_utils-0.2.1rc2/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.1rc2/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-03 09:02:47.986360 glue_utils-0.2.1rc2/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0      794 2024-05-03 09:02:47.986701 glue_utils-0.2.1rc2/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.1rc2/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 glue_utils-0.2.1rc2/PKG-INFO
```

### Comparing `glue_utils-0.2.1rc1/LICENSE` & `glue_utils-0.2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc1/README.md` & `glue_utils-0.2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc1/pyproject.toml` & `glue_utils-0.2.1rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.1rc1"
+version = "0.2.1rc2"
 # Uncomment this when dependabot has finally been updated to it is 
 # supported by dependabot.
 # package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `glue_utils-0.2.1rc1/src/glue_utils/glueetl/job.py` & `glue_utils-0.2.1rc2/src/glue_utils/glueetl/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
 from glue_utils import BaseOptions
 
 T = TypeVar("T", bound=BaseOptions, default=BaseOptions)
 
 
 class GlueETLJob(Generic[T]):
-    """A class that handles the boilerplate setup for Glue ETL jobs."""
+    """Class that handles the boilerplate setup for Glue ETL jobs."""
 
+    name: str
     options: T
-    glue_context: GlueContext
     spark: SparkSession
+    glue_context: GlueContext
 
     @overload
     def __init__(
         self: "GlueETLJob[BaseOptions]",
     ) -> None: ...
 
     @overload
@@ -50,33 +51,37 @@
             Has to be a subclass of BaseOptions, by default BaseOptions
 
         """
         if not issubclass(options_cls, BaseOptions):
             msg = "options_cls must be a subclass of BaseOptions."
             raise TypeError(msg)
 
-        job_options = getResolvedOptions(
-            sys.argv,
-            [field.name for field in fields(options_cls)],
-        )
+        params = []
+        if "--JOB_NAME" in sys.argv:
+            params.append("JOB_NAME")
+        params.extend(field.name for field in fields(options_cls))
+
+        job_options = getResolvedOptions(sys.argv, params)
 
         self.options = cast(T, options_cls.from_resolved_options(job_options))
 
+        self.name = job_options.get("JOB_NAME", "glueetl-job")
+
         self.glue_context = self.create_glue_context()
         self.spark = self.glue_context.spark_session
 
         self._job = Job(self.glue_context)
-        self._job.init(self.options.JOB_NAME, job_options)
+        self._job.init(self.name, job_options)
 
     def create_glue_context(self) -> GlueContext:
         """Create a GlueContext.
 
         Override this method to customize the GlueContext creation.
         """
-        spark_conf = SparkConf().setAppName(self.options.JOB_NAME)
+        spark_conf = SparkConf().setAppName(self.name)
         spark_context = SparkContext.getOrCreate(spark_conf)
 
         return GlueContext(spark_context)
 
     @contextmanager
     def managed_glue_context(
         self,
```

### Comparing `glue_utils-0.2.1rc1/src/glue_utils/options.py` & `glue_utils-0.2.1rc2/src/glue_utils/options.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,30 +6,22 @@
 from typing_extensions import Self
 
 
 @dataclass(frozen=True)
 class BaseOptions:
     """Dataclass for storing resolved options."""
 
-    JOB_NAME: str
-
     @classmethod
     def from_resolved_options(
         cls,
         resolved_options: dict[str, Any] | None = None,
     ) -> Self:
         """Create an instance of the class from Glue's resolved options."""
-        default_job_name = ""
-
         if not resolved_options:
-            return cls(JOB_NAME=default_job_name)
-
-        resolved_options["JOB_NAME"] = resolved_options.get(
-            "JOB_NAME", default_job_name
-        )
+            return cls()
 
         field_names = {field.name for field in fields(cls)}
 
         return cls(
             **{
                 key: value
                 for key, value in resolved_options.items()
```

### Comparing `glue_utils-0.2.1rc1/PKG-INFO` & `glue_utils-0.2.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.1rc1
+Version: 0.2.1rc2
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.10,<4.0
```

