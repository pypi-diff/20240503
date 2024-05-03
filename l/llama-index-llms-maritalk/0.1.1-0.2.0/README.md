# Comparing `tmp/llama_index_llms_maritalk-0.1.1.tar.gz` & `tmp/llama_index_llms_maritalk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_maritalk-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_llms_maritalk-0.2.0.tar", max compression
```

## Comparing `llama_index_llms_maritalk-0.1.1.tar` & `llama_index_llms_maritalk-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       40 2024-02-23 15:18:05.378877 llama_index_llms_maritalk-0.1.1/README.md
--rw-r--r--   0        0        0       17 2024-02-23 15:18:05.378877 llama_index_llms_maritalk-0.1.1/llama_index/llms/maritalk/BUILD
--rw-r--r--   0        0        0       77 2024-02-23 15:18:05.378877 llama_index_llms_maritalk-0.1.1/llama_index/llms/maritalk/__init__.py
--rw-r--r--   0        0        0     6673 2024-02-23 23:13:27.290643 llama_index_llms_maritalk-0.1.1/llama_index/llms/maritalk/base.py
--rw-r--r--   0        0        0     1564 2024-02-24 00:58:24.696170 llama_index_llms_maritalk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 llama_index_llms_maritalk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      651 2024-05-03 00:41:37.799229 llama_index_llms_maritalk-0.2.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 00:41:37.799229 llama_index_llms_maritalk-0.2.0/llama_index/llms/maritalk/BUILD
+-rw-r--r--   0        0        0       77 2024-05-03 00:41:37.799229 llama_index_llms_maritalk-0.2.0/llama_index/llms/maritalk/__init__.py
+-rw-r--r--   0        0        0    13374 2024-05-03 00:41:37.799229 llama_index_llms_maritalk-0.2.0/llama_index/llms/maritalk/base.py
+-rw-r--r--   0        0        0     1564 2024-05-03 00:41:37.799229 llama_index_llms_maritalk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 llama_index_llms_maritalk-0.2.0/PKG-INFO
```

### Comparing `llama_index_llms_maritalk-0.1.1/pyproject.toml` & `llama_index_llms_maritalk-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms maritalk integration"
 license = "MIT"
 name = "llama-index-llms-maritalk"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.1"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
```

