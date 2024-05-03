# Comparing `tmp/glue_utils-0.2.1rc3.tar.gz` & `tmp/glue_utils-0.2.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.1rc3.tar", max compression
+gzip compressed data, was "glue_utils-0.2.1rc4.tar", max compression
```

## Comparing `glue_utils-0.2.1rc3.tar` & `glue_utils-0.2.1rc4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.1rc3/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.1rc3/README.md
--rw-r--r--   0        0        0     3315 2024-05-03 10:44:00.449586 glue_utils-0.2.1rc3/pyproject.toml
--rw-r--r--   0        0        0       99 2024-05-03 10:43:56.445227 glue_utils-0.2.1rc3/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.1rc3/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     3077 2024-05-03 10:32:18.579737 glue_utils-0.2.1rc3/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0      794 2024-05-03 09:02:47.986701 glue_utils-0.2.1rc3/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.1rc3/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 glue_utils-0.2.1rc3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.1rc4/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.1rc4/README.md
+-rw-r--r--   0        0        0     3315 2024-05-03 11:12:53.179892 glue_utils-0.2.1rc4/pyproject.toml
+-rw-r--r--   0        0        0       99 2024-05-03 11:12:59.063439 glue_utils-0.2.1rc4/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.1rc4/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     3114 2024-05-03 11:12:21.569002 glue_utils-0.2.1rc4/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0      794 2024-05-03 09:02:47.986701 glue_utils-0.2.1rc4/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.1rc4/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 glue_utils-0.2.1rc4/PKG-INFO
```

### Comparing `glue_utils-0.2.1rc3/LICENSE` & `glue_utils-0.2.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc3/README.md` & `glue_utils-0.2.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc3/pyproject.toml` & `glue_utils-0.2.1rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.1rc3"
+version = "0.2.1rc4"
 # Uncomment this when dependabot has finally been updated to it is 
 # supported by dependabot.
 # package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `glue_utils-0.2.1rc3/src/glue_utils/glueetl/job.py` & `glue_utils-0.2.1rc4/src/glue_utils/glueetl/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         job_options = getResolvedOptions(sys.argv, params)
 
         self.options = cast(T, options_cls.from_resolved_options(job_options))
 
         self.name = job_options.get("JOB_NAME", "glueetl-job")
 
         self.sc = self.create_spark_context()
+        self.sc.setLogLevel("DEBUG")
         self.glue_context = self.create_glue_context()
         self.spark = self.glue_context.spark_session
 
         self._job = Job(self.glue_context)
         self._job.init(self.name, job_options)
 
     def create_spark_context(self) -> SparkContext:
```

### Comparing `glue_utils-0.2.1rc3/src/glue_utils/options.py` & `glue_utils-0.2.1rc4/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc3/PKG-INFO` & `glue_utils-0.2.1rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.1rc3
+Version: 0.2.1rc4
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.10,<4.0
```

