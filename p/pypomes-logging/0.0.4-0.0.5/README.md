# Comparing `tmp/pypomes_logging-0.0.4.tar.gz` & `tmp/pypomes_logging-0.0.5.tar.gz`

## Comparing `pypomes_logging-0.0.4.tar` & `pypomes_logging-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0    12788 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.5/PKG-INFO
```

### Comparing `pypomes_logging-0.0.4/src/pypomes_logging/__init__.py` & `pypomes_logging-0.0.5/src/pypomes_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.4/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.0.5/src/pypomes_logging/logging_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,24 +102,25 @@
     if len(errors) == 0:
         # no, proceed
         result = BytesIO()
         with filepath.open() as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(maxsplit=3)
-                # noinspection PyTypeChecker
-                msg_level: int = __get_logging_level(items[2])
-                if msg_level >= log_level:
-                    if log_from or log_to:
-                        timestamp: datetime = datetime_parse(f"{items[0]} {items[1]}")
-                        if (not log_from or timestamp >= log_from) and \
-                           (not log_to or timestamp <= log_to):
-                            result.write(line.encode())
-                    else:
-                            result.write(line.encode())
+                if log_level:
+                    # noinspection PyTypeChecker
+                    msg_level: int = __get_logging_level(items[2])
+                    if msg_level >= log_level:
+                        if log_from or log_to:
+                            timestamp: datetime = datetime_parse(f"{items[0]} {items[1]}")
+                            if (not log_from or timestamp >= log_from) and \
+                               (not log_to or timestamp <= log_to):
+                                result.write(line.encode())
+                        else:
+                                result.write(line.encode())
                 line = f.readline()
 
     return result
 
 
 def logging_send_entries(request: Request) -> Response:
     """
```

### Comparing `pypomes_logging-0.0.4/LICENSE` & `pypomes_logging-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.4/pyproject.toml` & `pypomes_logging-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.9.5",
+    "pypomes_core>=0.9.6",
     "pypomes_http>=0.1.6",
     "python-dateutil>=2.8.2",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_logging-0.0.4/PKG-INFO` & `pypomes_logging-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_logging
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.9.5
+Requires-Dist: pypomes-core>=0.9.6
 Requires-Dist: pypomes-http>=0.1.6
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

