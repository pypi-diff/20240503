# Comparing `tmp/dolbaram-0.2.6.tar.gz` & `tmp/dolbaram-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbaram-0.2.6.tar", max compression
+gzip compressed data, was "dolbaram-0.2.7.tar", max compression
```

## Comparing `dolbaram-0.2.6.tar` & `dolbaram-0.2.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.6/dolbaram/__init__.py
--rw-r--r--   0        0        0    19349 2024-04-03 03:47:54.214523 dolbaram-0.2.6/dolbaram/dolbaram.py
--rw-r--r--   0        0        0      576 2024-04-03 03:48:11.431546 dolbaram-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.7/dolbaram/__init__.py
+-rw-r--r--   0        0        0    19353 2024-05-03 03:53:07.281938 dolbaram-0.2.7/dolbaram/dolbaram.py
+-rw-r--r--   0        0        0      576 2024-05-03 03:53:07.275807 dolbaram-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.7/PKG-INFO
```

### Comparing `dolbaram-0.2.6/dolbaram/dolbaram.py` & `dolbaram-0.2.7/dolbaram/dolbaram.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
         :param is_dir:
         :param engine:
         :return:
         '''
 
         self.make_suite(suite_name)
         suite = self.add_expectations(suite_name, ecs)
-        if is_dir:
+        if not is_dir:
             result = self.checkpoint(s3_file_prefix=csv_path,
                                      suite=suite,
                                      engine=engine)
         else:
             token = csv_path.rsplit('/')
             result = self.checkpoint(s3_file_prefix="/".join(token[0:-1]),
                                      s3_file_name=token[-1],
```

### Comparing `dolbaram-0.2.6/pyproject.toml` & `dolbaram-0.2.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolbaram"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
```

### Comparing `dolbaram-0.2.6/PKG-INFO` & `dolbaram-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbaram
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

