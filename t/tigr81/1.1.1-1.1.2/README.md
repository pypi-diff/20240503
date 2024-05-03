# Comparing `tmp/tigr81-1.1.1.tar.gz` & `tmp/tigr81-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigr81-1.1.1.tar", max compression
+gzip compressed data, was "tigr81-1.1.2.tar", max compression
```

## Comparing `tigr81-1.1.1.tar` & `tigr81-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      786 2024-05-01 18:43:05.699437 tigr81-1.1.1/README.md
--rw-r--r--   0        0        0      719 2024-05-01 18:43:05.699437 tigr81-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      433 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/__init__.py
--rw-r--r--   0        0        0      182 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/cli_settings.py
--rw-r--r--   0        0        0        0 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/core/__init__.py
--rw-r--r--   0        0        0     2647 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/core/poetry_pm.py
--rw-r--r--   0        0        0     2528 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/core/scaffold.py
--rw-r--r--   0        0        0        0 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/monorepo/__init__.py
--rw-r--r--   0        0        0      203 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/monorepo/constants.py
--rw-r--r--   0        0        0     5057 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/monorepo/manifest.py
--rw-r--r--   0        0        0     7232 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/monorepo/monorepo.py
--rw-r--r--   0        0        0        0 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/scaffold/__init__.py
--rw-r--r--   0        0        0     4254 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/scaffold/project_template.py
--rw-r--r--   0        0        0     2347 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/commands/scaffold/scaffold.py
--rw-r--r--   0        0        0      454 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/main.py
--rw-r--r--   0        0        0      211 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/utils/pretty.py
--rw-r--r--   0        0        0      187 2024-05-01 18:43:05.699437 tigr81-1.1.1/tigr81/utils/read_yaml.py
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 tigr81-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      786 2024-05-03 19:46:46.786305 tigr81-1.1.2/README.md
+-rw-r--r--   0        0        0      719 2024-05-03 19:46:46.786305 tigr81-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      433 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/cli_settings.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/core/__init__.py
+-rw-r--r--   0        0        0     2647 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/core/poetry_pm.py
+-rw-r--r--   0        0        0     2528 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/core/scaffold.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/monorepo/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/monorepo/constants.py
+-rw-r--r--   0        0        0     5057 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/monorepo/manifest.py
+-rw-r--r--   0        0        0     7232 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/monorepo/monorepo.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/scaffold/__init__.py
+-rw-r--r--   0        0        0     4254 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/scaffold/project_template.py
+-rw-r--r--   0        0        0     2347 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/commands/scaffold/scaffold.py
+-rw-r--r--   0        0        0      494 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/main.py
+-rw-r--r--   0        0        0      211 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/utils/pretty.py
+-rw-r--r--   0        0        0      187 2024-05-03 19:46:46.786305 tigr81-1.1.2/tigr81/utils/read_yaml.py
+-rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 tigr81-1.1.2/PKG-INFO
```

### Comparing `tigr81-1.1.1/README.md` & `tigr81-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/pyproject.toml` & `tigr81-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tigr81"
-version = "1.1.1"
+version = "1.1.2"
 description = ""
 authors = ["Giuseppe Ambrosio <giuambro97@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 tigr81 = "tigr81.main:app"
```

### Comparing `tigr81-1.1.1/tigr81/commands/core/poetry_pm.py` & `tigr81-1.1.2/tigr81/commands/core/poetry_pm.py`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/tigr81/commands/core/scaffold.py` & `tigr81-1.1.2/tigr81/commands/core/scaffold.py`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/tigr81/commands/monorepo/manifest.py` & `tigr81-1.1.2/tigr81/commands/monorepo/manifest.py`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/tigr81/commands/monorepo/monorepo.py` & `tigr81-1.1.2/tigr81/commands/monorepo/monorepo.py`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/tigr81/commands/scaffold/project_template.py` & `tigr81-1.1.2/tigr81/commands/scaffold/project_template.py`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/tigr81/commands/scaffold/scaffold.py` & `tigr81-1.1.2/tigr81/commands/scaffold/scaffold.py`

 * *Files identical despite different names*

### Comparing `tigr81-1.1.1/PKG-INFO` & `tigr81-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigr81
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Author: Giuseppe Ambrosio
 Author-email: giuambro97@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

