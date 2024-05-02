# Comparing `tmp/chatpdb-0.1.7.tar.gz` & `tmp/chatpdb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatpdb-0.1.7.tar", last modified: Thu Apr 18 06:00:38 2024, max compression
+gzip compressed data, was "chatpdb-0.1.9.tar", last modified: Thu Apr 18 06:03:50 2024, max compression
```

## Comparing `chatpdb-0.1.7.tar` & `chatpdb-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.988996 chatpdb-0.1.7/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.7/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 06:00:38.988615 chatpdb-0.1.7/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.7/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.984207 chatpdb-0.1.7/chatpdb/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.7/chatpdb/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.7/chatpdb/__main__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.985889 chatpdb-0.1.7/chatpdb/chat/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.7/chatpdb/chat/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/chat/interface.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.986584 chatpdb-0.1.7/chatpdb/chat/llm/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.7/chatpdb/chat/llm/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.7/chatpdb/chat/llm/interface.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/chat/llm/openai.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.987505 chatpdb-0.1.7/chatpdb/chat/prompts/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-18 05:56:46.000000 chatpdb-0.1.7/chatpdb/chat/prompts/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/chat/prompts/ask.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/chat/prompts/explain.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/chat/prompts/system.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2271 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/chat/prompts/util.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/debugger.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.7/chatpdb/frame.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.7/chatpdb/stdout.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.988283 chatpdb-0.1.7/chatpdb.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 06:00:38.000000 chatpdb-0.1.7/chatpdb.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      637 2024-04-18 06:00:38.000000 chatpdb-0.1.7/chatpdb.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 06:00:38.000000 chatpdb-0.1.7/chatpdb.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 06:00:38.000000 chatpdb-0.1.7/chatpdb.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 06:00:38.000000 chatpdb-0.1.7/chatpdb.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1650 2024-04-18 06:00:34.000000 chatpdb-0.1.7/pyproject.toml
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 06:00:38.989250 chatpdb-0.1.7/setup.cfg
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:00:38.988059 chatpdb-0.1.7/tests/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.7/tests/test_debugger.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.7/tests/test_fixtures.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.7/tests/test_frame.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.346350 chatpdb-0.1.9/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-04-17 01:18:02.000000 chatpdb-0.1.9/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 06:03:50.346112 chatpdb-0.1.9/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2916 2024-04-18 02:40:12.000000 chatpdb-0.1.9/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.340666 chatpdb-0.1.9/chatpdb/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      657 2024-04-17 22:36:33.000000 chatpdb-0.1.9/chatpdb/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    10988 2024-04-17 20:47:59.000000 chatpdb-0.1.9/chatpdb/__main__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.342444 chatpdb-0.1.9/chatpdb/chat/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      126 2024-04-17 20:46:43.000000 chatpdb-0.1.9/chatpdb/chat/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1206 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/chat/interface.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.343165 chatpdb-0.1.9/chatpdb/chat/llm/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      132 2024-04-17 20:46:43.000000 chatpdb-0.1.9/chatpdb/chat/llm/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1233 2024-04-17 22:36:33.000000 chatpdb-0.1.9/chatpdb/chat/llm/interface.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1678 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/chat/llm/openai.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.344072 chatpdb-0.1.9/chatpdb/chat/prompts/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      243 2024-04-18 05:56:46.000000 chatpdb-0.1.9/chatpdb/chat/prompts/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1753 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/chat/prompts/ask.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1901 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/chat/prompts/explain.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      546 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/chat/prompts/system.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2271 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/chat/prompts/util.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1625 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1431 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/frame.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.344746 chatpdb-0.1.9/chatpdb/parsing/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      182 2024-04-17 22:36:33.000000 chatpdb-0.1.9/chatpdb/parsing/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1435 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/parsing/interface.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      139 2024-04-18 02:40:12.000000 chatpdb-0.1.9/chatpdb/parsing/vars.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1041 2024-04-17 21:33:19.000000 chatpdb-0.1.9/chatpdb/stdout.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.345626 chatpdb-0.1.9/chatpdb.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4287 2024-04-18 06:03:50.000000 chatpdb-0.1.9/chatpdb.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      718 2024-04-18 06:03:50.000000 chatpdb-0.1.9/chatpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-18 06:03:50.000000 chatpdb-0.1.9/chatpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       74 2024-04-18 06:03:50.000000 chatpdb-0.1.9/chatpdb.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-04-18 06:03:50.000000 chatpdb-0.1.9/chatpdb.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1661 2024-04-18 06:03:43.000000 chatpdb-0.1.9/pyproject.toml
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-18 06:03:50.346407 chatpdb-0.1.9/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-18 06:03:50.345394 chatpdb-0.1.9/tests/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      452 2024-04-18 02:40:12.000000 chatpdb-0.1.9/tests/test_debugger.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      432 2024-04-18 02:40:12.000000 chatpdb-0.1.9/tests/test_fixtures.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      454 2024-04-18 02:40:12.000000 chatpdb-0.1.9/tests/test_frame.py
```

### Comparing `chatpdb-0.1.7/LICENSE` & `chatpdb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/PKG-INFO` & `chatpdb-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatpdb
-Version: 0.1.7
+Version: 0.1.9
 Summary: A chatgpt enabled python debugger
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/chatpdb
 Project-URL: Issues, https://github.com/never-over/chatpdb/issues
 Keywords: python,chatgpt,pdb,ai,chat,debugger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `chatpdb-0.1.7/README.md` & `chatpdb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/__init__.py` & `chatpdb-0.1.9/chatpdb/__init__.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/__main__.py` & `chatpdb-0.1.9/chatpdb/__main__.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/interface.py` & `chatpdb-0.1.9/chatpdb/chat/interface.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/llm/interface.py` & `chatpdb-0.1.9/chatpdb/chat/llm/interface.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/llm/openai.py` & `chatpdb-0.1.9/chatpdb/chat/llm/openai.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/prompts/ask.py` & `chatpdb-0.1.9/chatpdb/chat/prompts/ask.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/prompts/explain.py` & `chatpdb-0.1.9/chatpdb/chat/prompts/explain.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/prompts/system.py` & `chatpdb-0.1.9/chatpdb/chat/prompts/system.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/chat/prompts/util.py` & `chatpdb-0.1.9/chatpdb/chat/prompts/util.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/debugger.py` & `chatpdb-0.1.9/chatpdb/debugger.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/frame.py` & `chatpdb-0.1.9/chatpdb/frame.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb/stdout.py` & `chatpdb-0.1.9/chatpdb/stdout.py`

 * *Files identical despite different names*

### Comparing `chatpdb-0.1.7/chatpdb.egg-info/PKG-INFO` & `chatpdb-0.1.9/chatpdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatpdb
-Version: 0.1.7
+Version: 0.1.9
 Summary: A chatgpt enabled python debugger
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/chatpdb
 Project-URL: Issues, https://github.com/never-over/chatpdb/issues
 Keywords: python,chatgpt,pdb,ai,chat,debugger
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `chatpdb-0.1.7/chatpdb.egg-info/SOURCES.txt` & `chatpdb-0.1.9/chatpdb.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,10 +17,13 @@
 chatpdb/chat/llm/interface.py
 chatpdb/chat/llm/openai.py
 chatpdb/chat/prompts/__init__.py
 chatpdb/chat/prompts/ask.py
 chatpdb/chat/prompts/explain.py
 chatpdb/chat/prompts/system.py
 chatpdb/chat/prompts/util.py
+chatpdb/parsing/__init__.py
+chatpdb/parsing/interface.py
+chatpdb/parsing/vars.py
 tests/test_debugger.py
 tests/test_fixtures.py
 tests/test_frame.py
```

### Comparing `chatpdb-0.1.7/pyproject.toml` & `chatpdb-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chatpdb"
-version = "0.1.7"
+version = "0.1.9"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A chatgpt enabled python debugger"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -49,8 +49,8 @@
 reportMissingTypeStubs = false
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-packages = ["chatpdb", "chatpdb.chat.prompts"]
+packages = ["chatpdb", "chatpdb.chat", "chatpdb.parsing"]
```

