# Comparing `tmp/repo2docs-0.1.1.tar.gz` & `tmp/repo2docs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2docs-0.1.1.tar", max compression
+gzip compressed data, was "repo2docs-0.1.2.tar", max compression
```

## Comparing `repo2docs-0.1.1.tar` & `repo2docs-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.1/LICENSE
--rw-r--r--   0        0        0     2576 2024-05-03 02:03:32.612872 repo2docs-0.1.1/README.md
--rw-r--r--   0        0        0      507 2024-05-03 02:03:51.229643 repo2docs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.1/repo2docs/__init__.py
--rw-r--r--   0        0        0     1456 2024-05-03 01:56:39.798050 repo2docs-0.1.1/repo2docs/llm.py
--rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.1/repo2docs/prompts.py
--rw-r--r--   0        0        0     3268 2024-05-03 01:56:53.227931 repo2docs-0.1.1/repo2docs/repo2docs.py
--rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.1/repo2docs/repo_to_text.py
--rw-r--r--   0        0        0     2098 2024-05-03 01:52:50.826712 repo2docs-0.1.1/repo2docs/text_to_docs.py
--rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 repo2docs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2576 2024-05-03 02:03:32.612872 repo2docs-0.1.2/README.md
+-rw-r--r--   0        0        0      507 2024-05-03 02:13:37.875410 repo2docs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.2/repo2docs/__init__.py
+-rw-r--r--   0        0        0     2011 2024-05-03 02:12:41.755256 repo2docs-0.1.2/repo2docs/llm.py
+-rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.2/repo2docs/prompts.py
+-rw-r--r--   0        0        0     3268 2024-05-03 01:56:53.227931 repo2docs-0.1.2/repo2docs/repo2docs.py
+-rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.2/repo2docs/repo_to_text.py
+-rw-r--r--   0        0        0     2098 2024-05-03 01:52:50.826712 repo2docs-0.1.2/repo2docs/text_to_docs.py
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 repo2docs-0.1.2/PKG-INFO
```

### Comparing `repo2docs-0.1.1/LICENSE` & `repo2docs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.1/README.md` & `repo2docs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.1/repo2docs/prompts.py` & `repo2docs-0.1.2/repo2docs/prompts.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.1/repo2docs/repo2docs.py` & `repo2docs-0.1.2/repo2docs/repo2docs.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.1/repo2docs/repo_to_text.py` & `repo2docs-0.1.2/repo2docs/repo_to_text.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.1/repo2docs/text_to_docs.py` & `repo2docs-0.1.2/repo2docs/text_to_docs.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.1/PKG-INFO` & `repo2docs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2docs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Documentation from your codebase using LLMs
 License: MIT
 Author: Joe Petrantoni
 Author-email: 79169021+jpetrantoni@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

