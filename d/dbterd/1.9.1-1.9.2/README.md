# Comparing `tmp/dbterd-1.9.1.tar.gz` & `tmp/dbterd-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.9.1.tar", max compression
+gzip compressed data, was "dbterd-1.9.2.tar", max compression
```

## Comparing `dbterd-1.9.1.tar` & `dbterd-1.9.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1067 2024-01-20 02:59:30.402589 dbterd-1.9.1/LICENSE
--rw-r--r--   0        0        0     3310 2024-01-20 02:59:30.406589 dbterd-1.9.1/README.md
--rw-r--r--   0        0        0        0 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0      580 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/adapter.py
--rw-r--r--   0        0        0        0 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0     7002 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/algos/base.py
--rw-r--r--   0        0        0     6196 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     6280 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/base.py
--rw-r--r--   0        0        0     3777 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/dbt_cloud.py
--rw-r--r--   0        0        0     3980 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/dbt_invocation.py
--rw-r--r--   0        0        0     4519 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/filter.py
--rw-r--r--   0        0        0      897 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/meta.py
--rw-r--r--   0        0        0        0 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      306 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      296 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/d2/__init__.py
--rw-r--r--   0        0        0     1591 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/d2/d2_test_relationship.py
--rw-r--r--   0        0        0      304 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0     2257 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0      168 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      320 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/graphviz/__init__.py
--rw-r--r--   0        0        0     2778 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/graphviz/graphviz_test_relationship.py
--rw-r--r--   0        0        0      316 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     2162 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      320 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/plantuml/__init__.py
--rw-r--r--   0        0        0     2012 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/adapters/targets/plantuml/plantuml_test_relationship.py
--rw-r--r--   0        0        0        0 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     2061 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/cli/main.py
--rw-r--r--   0        0        0     5584 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/cli/params.py
--rw-r--r--   0        0        0      164 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/constants.py
--rw-r--r--   0        0        0      284 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/default.py
--rw-r--r--   0        0        0        0 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     5661 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2024-01-20 02:59:30.410589 dbterd-1.9.1/dbterd/main.py
--rw-r--r--   0        0        0     2200 2024-01-20 02:59:39.286629 dbterd-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 dbterd-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-07 03:06:34.881626 dbterd-1.9.2/LICENSE
+-rw-r--r--   0        0        0     3310 2024-02-07 03:06:34.881626 dbterd-1.9.2/README.md
+-rw-r--r--   0        0        0        0 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0      580 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/adapter.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     7002 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     6196 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     6280 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/base.py
+-rw-r--r--   0        0        0     3777 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/dbt_cloud.py
+-rw-r--r--   0        0        0     3980 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/dbt_invocation.py
+-rw-r--r--   0        0        0     4527 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/filter.py
+-rw-r--r--   0        0        0      897 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/meta.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      306 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      296 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/d2/__init__.py
+-rw-r--r--   0        0        0     1591 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/d2/d2_test_relationship.py
+-rw-r--r--   0        0        0      304 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     2257 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      320 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/graphviz/__init__.py
+-rw-r--r--   0        0        0     2778 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/graphviz/graphviz_test_relationship.py
+-rw-r--r--   0        0        0      316 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     2162 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      320 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/plantuml/__init__.py
+-rw-r--r--   0        0        0     2012 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/adapters/targets/plantuml/plantuml_test_relationship.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2061 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/cli/main.py
+-rw-r--r--   0        0        0     5584 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/cli/params.py
+-rw-r--r--   0        0        0      164 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/constants.py
+-rw-r--r--   0        0        0      284 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/default.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     5661 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2024-02-07 03:06:34.889627 dbterd-1.9.2/dbterd/main.py
+-rw-r--r--   0        0        0     2200 2024-02-07 03:06:48.397712 dbterd-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 dbterd-1.9.2/PKG-INFO
```

### Comparing `dbterd-1.9.1/LICENSE` & `dbterd-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/README.md` & `dbterd-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/adapter.py` & `dbterd-1.9.2/dbterd/adapters/adapter.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/algos/base.py` & `dbterd-1.9.2/dbterd/adapters/algos/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.9.2/dbterd/adapters/algos/test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/base.py` & `dbterd-1.9.2/dbterd/adapters/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/dbt_cloud.py` & `dbterd-1.9.2/dbterd/adapters/dbt_cloud.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/dbt_invocation.py` & `dbterd-1.9.2/dbterd/adapters/dbt_invocation.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/filter.py` & `dbterd-1.9.2/dbterd/adapters/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         rule (str, optional): Rule def. Defaults to "".
 
     Returns:
         bool: True if satisfied `equal` logic applied to Table name
     """
     if not rule:
         return True
-    return table.node_name == rule
+    return table.node_name.lower() == rule
 
 
 def is_satisfied_by_schema(table: Table, rule: str = ""):
     """Evaluate rule by Schema name
 
     Args:
         table (Table): Table object
```

### Comparing `dbterd-1.9.1/dbterd/adapters/meta.py` & `dbterd-1.9.2/dbterd/adapters/meta.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/targets/d2/d2_test_relationship.py` & `dbterd-1.9.2/dbterd/adapters/targets/d2/d2_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.9.2/dbterd/adapters/targets/dbml/dbml_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/targets/graphviz/graphviz_test_relationship.py` & `dbterd-1.9.2/dbterd/adapters/targets/graphviz/graphviz_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py` & `dbterd-1.9.2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/adapters/targets/plantuml/plantuml_test_relationship.py` & `dbterd-1.9.2/dbterd/adapters/targets/plantuml/plantuml_test_relationship.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/cli/main.py` & `dbterd-1.9.2/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/cli/params.py` & `dbterd-1.9.2/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/helpers/cli_messaging.py` & `dbterd-1.9.2/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/helpers/dict.py` & `dbterd-1.9.2/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/helpers/file.py` & `dbterd-1.9.2/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/helpers/jsonify.py` & `dbterd-1.9.2/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/helpers/log.py` & `dbterd-1.9.2/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/dbterd/helpers/yaml.py` & `dbterd-1.9.2/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.9.1/pyproject.toml` & `dbterd-1.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.9.1"
+version = "1.9.2"
 description = "CLI to generate ERD Diagram file from dbt artifact files"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
```

### Comparing `dbterd-1.9.1/PKG-INFO` & `dbterd-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.9.1
+Version: 1.9.2
 Summary: CLI to generate ERD Diagram file from dbt artifact files
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
```

