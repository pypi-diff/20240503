# Comparing `tmp/praisonai_tools-0.0.1.tar.gz` & `tmp/praisonai_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praisonai_tools-0.0.1.tar", max compression
+gzip compressed data, was "praisonai_tools-0.0.2.tar", max compression
```

## Comparing `praisonai_tools-0.0.1.tar` & `praisonai_tools-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       18 2024-05-03 06:28:23.758153 praisonai_tools-0.0.1/README.md
--rw-r--r--   0        0        0       49 2024-05-03 06:33:08.923654 praisonai_tools-0.0.1/praisonai_tools/__init__.py
--rw-r--r--   0        0        0      619 2024-05-03 06:27:22.862095 praisonai_tools-0.0.1/praisonai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1701 2024-05-03 06:27:22.862182 praisonai_tools-0.0.1/praisonai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0        0 2024-05-03 06:33:36.075281 praisonai_tools-0.0.1/praisonai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-05-03 02:15:32.000000 praisonai_tools-0.0.1/praisonai_tools/tools/base_tool.py
--rw-r--r--   0        0        0      723 2024-05-03 06:38:48.171947 praisonai_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1063 1970-01-01 00:00:00.000000 praisonai_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-05-03 06:28:23.758153 praisonai_tools-0.0.2/README.md
+-rw-r--r--   0        0        0       45 2024-05-03 12:17:08.621490 praisonai_tools-0.0.2/praisonai_tools/__init__.py
+-rw-r--r--   0        0        0      619 2024-05-03 06:27:22.862095 praisonai_tools-0.0.2/praisonai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1701 2024-05-03 06:27:22.862182 praisonai_tools-0.0.2/praisonai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-03 06:33:36.075281 praisonai_tools-0.0.2/praisonai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-05-03 02:15:32.000000 praisonai_tools-0.0.2/praisonai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0      747 2024-05-03 12:17:55.222964 praisonai_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 praisonai_tools-0.0.2/PKG-INFO
```

### Comparing `praisonai_tools-0.0.1/praisonai_tools/adapters/embedchain_adapter.py` & `praisonai_tools-0.0.2/praisonai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `praisonai_tools-0.0.1/praisonai_tools/adapters/lancedb_adapter.py` & `praisonai_tools-0.0.2/praisonai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `praisonai_tools-0.0.1/praisonai_tools/tools/base_tool.py` & `praisonai_tools-0.0.2/praisonai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `praisonai_tools-0.0.1/pyproject.toml` & `praisonai_tools-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "praisonai-tools"
-version = "0.0.1"
+version = "0.0.2"
 description = "Set of tools for the PraisonAI framework"
 authors = ["Mervin Praison"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
@@ -15,14 +15,15 @@
 embedchain = {extras = ["github", "youtube"], version = "^0.1.85"}
 chromadb = "^0.4.22"
 pyright = "^1.1.350"
 pytube = "^15.0.0"
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.3"
 selenium = "^4.18.1"
+crewai-tools = "^0.1.1"
 
 [tool.poetry.urls]
 Homepage = "https://praisonai.com"
 Repository = "https://github.com/mervinpraisoin/PraisonAI-tools"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `praisonai_tools-0.0.1/PKG-INFO` & `praisonai_tools-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: praisonai-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Set of tools for the PraisonAI framework
 Author: Mervin Praison
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: chromadb (>=0.4.22,<0.5.0)
+Requires-Dist: crewai-tools (>=0.1.1,<0.2.0)
 Requires-Dist: embedchain[github,youtube] (>=0.1.85,<0.2.0)
 Requires-Dist: lancedb (>=0.5.4,<0.6.0)
 Requires-Dist: langchain (>=0.1.4,<0.2.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pyright (>=1.1.350,<2.0.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
```

