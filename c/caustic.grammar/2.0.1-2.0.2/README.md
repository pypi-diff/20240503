# Comparing `tmp/caustic.grammar-2.0.1.tar.gz` & `tmp/caustic.grammar-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.grammar-2.0.1.tar", last modified: Wed May  1 18:14:52 2024, max compression
+gzip compressed data, was "caustic.grammar-2.0.2.tar", last modified: Fri May  3 17:22:13 2024, max compression
```

## Comparing `caustic.grammar-2.0.1.tar` & `caustic.grammar-2.0.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.849561 caustic.grammar-2.0.1/
--rw-r--r--   0 shae      (1000) shae      (1000)     1064 2024-04-16 18:17:24.000000 caustic.grammar-2.0.1/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-05-01 18:14:52.849561 caustic.grammar-2.0.1/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)        0 2024-04-24 17:10:33.000000 caustic.grammar-2.0.1/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1053 2024-05-01 18:07:08.000000 caustic.grammar-2.0.1/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-05-01 18:14:52.849561 caustic.grammar-2.0.1/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.842894 caustic.grammar-2.0.1/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.842894 caustic.grammar-2.0.1/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.842894 caustic.grammar-2.0.1/src/caustic/grammar/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.846228 caustic.grammar-2.0.1/src/caustic/grammar/canonical/
--rw-r--r--   0 shae      (1000) shae      (1000)      378 2024-05-01 18:14:28.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/block.pg
--rw-r--r--   0 shae      (1000) shae      (1000)       94 2024-05-01 18:06:23.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/canonical.pg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.846228 caustic.grammar-2.0.1/src/caustic/grammar/canonical/expressions/
--rw-r--r--   0 shae      (1000) shae      (1000)      427 2024-04-30 21:48:58.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/expressions/expressions.pg
--rw-r--r--   0 shae      (1000) shae      (1000)      248 2024-04-30 17:21:22.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/expressions/identifier.pg
--rw-r--r--   0 shae      (1000) shae      (1000)      434 2024-04-30 21:48:38.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/expressions/literals.pg
--rw-r--r--   0 shae      (1000) shae      (1000)     4630 2024-05-01 15:56:47.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/expressions/operators.pg
--rw-r--r--   0 shae      (1000) shae      (1000)     1881 2024-05-01 01:27:17.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/procedure.pg
--rw-r--r--   0 shae      (1000) shae      (1000)     2717 2024-05-01 15:18:40.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/procedure_actions.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.849561 caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/
--rw-r--r--   0 shae      (1000) shae      (1000)      464 2024-05-01 03:22:13.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/declare.pg
--rw-r--r--   0 shae      (1000) shae      (1000)     1805 2024-05-01 15:20:03.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/objects.pg
--rw-r--r--   0 shae      (1000) shae      (1000)     2411 2024-05-01 15:20:27.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/objects_actions.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1719 2024-05-01 15:54:16.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/statements.pg
--rw-r--r--   0 shae      (1000) shae      (1000)      260 2024-05-01 03:11:21.000000 caustic.grammar-2.0.1/src/caustic/grammar/canonical/types.pg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 18:14:52.849561 caustic.grammar-2.0.1/src/caustic.grammar.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-05-01 18:14:52.000000 caustic.grammar-2.0.1/src/caustic.grammar.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      902 2024-05-01 18:14:52.000000 caustic.grammar-2.0.1/src/caustic.grammar.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-05-01 18:14:52.000000 caustic.grammar-2.0.1/src/caustic.grammar.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       27 2024-05-01 18:14:52.000000 caustic.grammar-2.0.1/src/caustic.grammar.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-05-01 18:14:52.000000 caustic.grammar-2.0.1/src/caustic.grammar.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.188562 caustic.grammar-2.0.2/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1064 2024-04-16 18:17:24.000000 caustic.grammar-2.0.2/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-05-03 17:22:13.185228 caustic.grammar-2.0.2/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)        0 2024-04-24 17:10:33.000000 caustic.grammar-2.0.2/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1065 2024-05-03 17:21:57.000000 caustic.grammar-2.0.2/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-05-03 17:22:13.188562 caustic.grammar-2.0.2/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.171895 caustic.grammar-2.0.2/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.171895 caustic.grammar-2.0.2/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.171895 caustic.grammar-2.0.2/src/caustic/grammar/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.181895 caustic.grammar-2.0.2/src/caustic/grammar/canonical/
+-rw-r--r--   0 shae      (1000) shae      (1000)      378 2024-05-01 18:14:28.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/block.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)       94 2024-05-01 18:06:23.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/canonical.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)   899147 2024-05-03 17:19:08.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/canonical.pgt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.185228 caustic.grammar-2.0.2/src/caustic/grammar/canonical/expressions/
+-rw-r--r--   0 shae      (1000) shae      (1000)      427 2024-04-30 21:48:58.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/expressions/expressions.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)      248 2024-04-30 17:21:22.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/expressions/identifier.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)      434 2024-04-30 21:48:38.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/expressions/literals.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)     4630 2024-05-01 15:56:47.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/expressions/operators.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)     1881 2024-05-01 01:27:17.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/procedure.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)     2717 2024-05-01 15:18:40.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/procedure_actions.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.185228 caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/
+-rw-r--r--   0 shae      (1000) shae      (1000)      464 2024-05-01 03:22:13.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/declare.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)     1805 2024-05-01 15:20:03.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/objects.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)     2411 2024-05-01 15:20:27.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/objects_actions.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1719 2024-05-01 15:54:16.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/statements.pg
+-rw-r--r--   0 shae      (1000) shae      (1000)      260 2024-05-01 03:11:21.000000 caustic.grammar-2.0.2/src/caustic/grammar/canonical/types.pg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-03 17:22:13.185228 caustic.grammar-2.0.2/src/caustic.grammar.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-05-03 17:22:12.000000 caustic.grammar-2.0.2/src/caustic.grammar.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-05-03 17:22:13.000000 caustic.grammar-2.0.2/src/caustic.grammar.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-05-03 17:22:12.000000 caustic.grammar-2.0.2/src/caustic.grammar.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       27 2024-05-03 17:22:12.000000 caustic.grammar-2.0.2/src/caustic.grammar.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-05-03 17:22:12.000000 caustic.grammar-2.0.2/src/caustic.grammar.egg-info/top_level.txt
```

### Comparing `caustic.grammar-2.0.1/LICENSE` & `caustic.grammar-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/PKG-INFO` & `caustic.grammar-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.grammar
-Version: 2.0.1
+Version: 2.0.2
 Summary: Caustic's default grammar
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticGrammar
 Project-URL: Issues, https://codeberg.org/Caustic/CausticGrammar/issues
 Keywords: caustic,language,grammar
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `caustic.grammar-2.0.1/pyproject.toml` & `caustic.grammar-2.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.grammar"
-version = "2.0.1"
+version = "2.0.2"
 dependencies = ["caustic.cst", "caustic.parser"]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's default grammar"
 readme = "README.md"
 keywords = ['caustic', 'language', 'grammar']
@@ -27,8 +27,8 @@
 Issues = "https://codeberg.org/Caustic/CausticGrammar/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
-"caustic.grammar" = ["**/*.pg"]
+"caustic.grammar" = ["**/*.pg", "**/*.pgt"]
```

### Comparing `caustic.grammar-2.0.1/src/caustic/grammar/canonical/expressions/operators.pg` & `caustic.grammar-2.0.2/src/caustic/grammar/canonical/expressions/operators.pg`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/src/caustic/grammar/canonical/procedure.pg` & `caustic.grammar-2.0.2/src/caustic/grammar/canonical/procedure.pg`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/src/caustic/grammar/canonical/procedure_actions.py` & `caustic.grammar-2.0.2/src/caustic/grammar/canonical/procedure_actions.py`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/objects.pg` & `caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/objects.pg`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/objects_actions.py` & `caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/objects_actions.py`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/src/caustic/grammar/canonical/statements/statements.pg` & `caustic.grammar-2.0.2/src/caustic/grammar/canonical/statements/statements.pg`

 * *Files identical despite different names*

### Comparing `caustic.grammar-2.0.1/src/caustic.grammar.egg-info/PKG-INFO` & `caustic.grammar-2.0.2/src/caustic.grammar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.grammar
-Version: 2.0.1
+Version: 2.0.2
 Summary: Caustic's default grammar
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticGrammar
 Project-URL: Issues, https://codeberg.org/Caustic/CausticGrammar/issues
 Keywords: caustic,language,grammar
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `caustic.grammar-2.0.1/src/caustic.grammar.egg-info/SOURCES.txt` & `caustic.grammar-2.0.2/src/caustic.grammar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/caustic.grammar.egg-info/PKG-INFO
 src/caustic.grammar.egg-info/SOURCES.txt
 src/caustic.grammar.egg-info/dependency_links.txt
 src/caustic.grammar.egg-info/requires.txt
 src/caustic.grammar.egg-info/top_level.txt
 src/caustic/grammar/canonical/block.pg
 src/caustic/grammar/canonical/canonical.pg
+src/caustic/grammar/canonical/canonical.pgt
 src/caustic/grammar/canonical/procedure.pg
 src/caustic/grammar/canonical/procedure_actions.py
 src/caustic/grammar/canonical/types.pg
 src/caustic/grammar/canonical/expressions/expressions.pg
 src/caustic/grammar/canonical/expressions/identifier.pg
 src/caustic/grammar/canonical/expressions/literals.pg
 src/caustic/grammar/canonical/expressions/operators.pg
```

