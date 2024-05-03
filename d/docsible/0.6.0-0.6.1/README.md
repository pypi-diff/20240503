# Comparing `tmp/docsible-0.6.0.tar.gz` & `tmp/docsible-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsible-0.6.0.tar", max compression
+gzip compressed data, was "docsible-0.6.1.tar", max compression
```

## Comparing `docsible-0.6.0.tar` & `docsible-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.6.0/LICENSE
--rw-r--r--   0        0        0     4478 2024-04-24 22:33:33.753996 docsible-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.6.0/docsible/__init__.py
--rw-r--r--   0        0        0     9952 2024-04-24 22:33:33.753996 docsible-0.6.0/docsible/cli.py
--rw-r--r--   0        0        0     6708 2024-04-24 22:33:33.753996 docsible-0.6.0/docsible/markdown_template.py
--rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.6.0/docsible/utils/__init__.py
--rw-r--r--   0        0        0     6208 2024-02-06 18:36:44.373788 docsible-0.6.0/docsible/utils/mermaid.py
--rw-r--r--   0        0        0     1823 2024-01-24 19:17:56.690945 docsible-0.6.0/docsible/utils/special_tasks_keys.py
--rw-r--r--   0        0        0     4749 2024-04-23 17:40:53.516849 docsible-0.6.0/docsible/utils/yaml.py
--rw-r--r--   0        0        0      860 2024-04-24 22:33:33.753996 docsible-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 docsible-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4478 2024-04-24 22:33:33.753996 docsible-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.6.1/docsible/__init__.py
+-rw-r--r--   0        0        0     9952 2024-05-03 00:32:09.500714 docsible-0.6.1/docsible/cli.py
+-rw-r--r--   0        0        0     6708 2024-05-02 23:22:22.429711 docsible-0.6.1/docsible/markdown_template.py
+-rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.6.1/docsible/utils/__init__.py
+-rw-r--r--   0        0        0    12952 2024-05-03 00:32:09.500714 docsible-0.6.1/docsible/utils/mermaid.py
+-rw-r--r--   0        0        0     1823 2024-01-24 19:17:56.690945 docsible-0.6.1/docsible/utils/special_tasks_keys.py
+-rw-r--r--   0        0        0     4749 2024-04-23 17:40:53.516849 docsible-0.6.1/docsible/utils/yaml.py
+-rw-r--r--   0        0        0      860 2024-05-03 00:32:09.500714 docsible-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 docsible-0.6.1/PKG-INFO
```

### Comparing `docsible-0.6.0/LICENSE` & `docsible-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docsible-0.6.0/README.md` & `docsible-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `docsible-0.6.0/docsible/cli.py` & `docsible-0.6.1/docsible/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jinja2 import Environment, BaseLoader, FileSystemLoader 
 from docsible.markdown_template import static_template, collection_template
 from docsible.utils.mermaid import generate_mermaid_playbook, generate_mermaid_role_tasks_per_file
 from docsible.utils.yaml import load_yaml_generic, load_yaml_files_from_dir_custom, get_task_commensts
 from docsible.utils.special_tasks_keys import process_special_task_keys
 
 def get_version():
-    return "0.6.0"
+    return "0.6.1"
 
 def manage_docsible_file_keys(docsible_path):
     default_data = {
         'description': None,
         'requester': None,
         'users': None,
         'dt_dev': None,
```

### Comparing `docsible-0.6.0/docsible/markdown_template.py` & `docsible-0.6.1/docsible/markdown_template.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.0/docsible/utils/special_tasks_keys.py` & `docsible-0.6.1/docsible/utils/special_tasks_keys.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.0/docsible/utils/yaml.py` & `docsible-0.6.1/docsible/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.0/pyproject.toml` & `docsible-0.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docsible"
-version = "0.6.0"
+version = "0.6.1"
 description = "Document generator for ansible role/collection"
 authors = ["Lucian BLETAN <neuraluc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `docsible-0.6.0/PKG-INFO` & `docsible-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsible
-Version: 0.6.0
+Version: 0.6.1
 Summary: Document generator for ansible role/collection
 License: MIT
 Author: Lucian BLETAN
 Author-email: neuraluc@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

