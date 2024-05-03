# Comparing `tmp/cai_causal_graph-0.4.8.dev1.tar.gz` & `tmp/cai_causal_graph-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cai_causal_graph-0.4.8.dev1.tar", max compression
+gzip compressed data, was "cai_causal_graph-0.4.9.tar", max compression
```

## Comparing `cai_causal_graph-0.4.8.dev1.tar` & `cai_causal_graph-0.4.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/LICENSE
--rw-r--r--   0        0        0     1686 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/README.md
--rw-r--r--   0        0        0     1292 2024-04-10 13:07:46.178974 cai_causal_graph-0.4.8.dev1/cai_causal_graph/__init__.py
--rw-r--r--   0        0        0   101920 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/causal_graph.py
--rw-r--r--   0        0        0     2599 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/exceptions.py
--rw-r--r--   0        0        0    28767 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/graph_components.py
--rw-r--r--   0        0        0    21769 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/identify_utils.py
--rw-r--r--   0        0        0     1865 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/interfaces.py
--rw-r--r--   0        0        0    63360 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/time_series_causal_graph.py
--rw-r--r--   0        0        0     4427 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/type_definitions.py
--rw-r--r--   0        0        0     4914 2024-04-10 13:07:29.815093 cai_causal_graph-0.4.8.dev1/cai_causal_graph/utils.py
--rw-r--r--   0        0        0     2575 2024-04-10 13:07:46.178974 cai_causal_graph-0.4.8.dev1/pyproject.toml
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 cai_causal_graph-0.4.8.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1686 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/README.md
+-rw-r--r--   0        0        0     1287 2024-05-03 10:05:27.409100 cai_causal_graph-0.4.9/cai_causal_graph/__init__.py
+-rw-r--r--   0        0        0   101920 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/causal_graph.py
+-rw-r--r--   0        0        0     2599 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/exceptions.py
+-rw-r--r--   0        0        0    28767 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/graph_components.py
+-rw-r--r--   0        0        0    21769 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/identify_utils.py
+-rw-r--r--   0        0        0     1865 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/interfaces.py
+-rw-r--r--   0        0        0    63977 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/time_series_causal_graph.py
+-rw-r--r--   0        0        0     4427 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/type_definitions.py
+-rw-r--r--   0        0        0     4914 2024-05-03 10:05:11.888962 cai_causal_graph-0.4.9/cai_causal_graph/utils.py
+-rw-r--r--   0        0        0     2570 2024-05-03 10:05:27.405100 cai_causal_graph-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 cai_causal_graph-0.4.9/PKG-INFO
```

### Comparing `cai_causal_graph-0.4.8.dev1/LICENSE` & `cai_causal_graph-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/README.md` & `cai_causal_graph-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/__init__.py` & `cai_causal_graph-0.4.9/cai_causal_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'EDGE_T',  # Keep for backwards compatibility.
     'NODE_T',  # Keep for backwards compatibility.
     # Time series specific tags
     'TIME_LAG',
     'VARIABLE_NAME',
 ]
 
-__version__ = '0.4.8.dev1'
+__version__ = '0.4.9'
 
 from cai_causal_graph.causal_graph import CausalGraph, Skeleton
 from cai_causal_graph.time_series_causal_graph import TimeSeriesCausalGraph
 from cai_causal_graph.type_definitions import (
     EDGE_T,
     NODE_T,
     TIME_LAG,
```

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/causal_graph.py` & `cai_causal_graph-0.4.9/cai_causal_graph/causal_graph.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/exceptions.py` & `cai_causal_graph-0.4.9/cai_causal_graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/graph_components.py` & `cai_causal_graph-0.4.9/cai_causal_graph/graph_components.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/identify_utils.py` & `cai_causal_graph-0.4.9/cai_causal_graph/identify_utils.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/interfaces.py` & `cai_causal_graph-0.4.9/cai_causal_graph/interfaces.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/time_series_causal_graph.py` & `cai_causal_graph-0.4.9/cai_causal_graph/time_series_causal_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,24 @@
 
         # check for floating nodes
         if self.variables is not None and len(self.variables) > 0:
             for variable in self.variables:
                 if (
                     minimal_cg.variables is None or variable not in minimal_cg.variables
                 ) and not minimal_cg.node_exists(variable):
-                    minimal_cg.add_node(variable)
+                    # Guaranteed there is at least one node, take the first for simplicity.
+                    # This aligns with how edges are chosen for minimal graph.
+                    # Only issue is if they have different meta. TODO: CAUSALAI-4784
+                    original_floating_node = self.get_nodes_for_variable_name(variable)[0]
+                    new_floating_node = self._NodeCls(
+                        identifier=variable,
+                        meta=original_floating_node.meta,
+                        variable_type=original_floating_node.variable_type,
+                    )
+                    minimal_cg.add_node(node=new_floating_node)
 
         return minimal_cg
 
     def _get_time_topological_order(self, ordered_nodes: List[str]) -> List[str]:
         """Return the provided list if it is ordered in time; otherwise, an empty list is returned."""
         # Iterate through the list to ensure it respects the time ordering.
         for j, node in enumerate(ordered_nodes):
```

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/type_definitions.py` & `cai_causal_graph-0.4.9/cai_causal_graph/type_definitions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/cai_causal_graph/utils.py` & `cai_causal_graph-0.4.9/cai_causal_graph/utils.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.8.dev1/pyproject.toml` & `cai_causal_graph-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 check_untyped_defs = true
 ignore_missing_imports = true
 pretty = true
 cache_dir = '/dev/null'
 
 [tool.poetry]
 name = "cai-causal-graph"
-version = "0.4.8.dev1"
+version = "0.4.9"
 description = "A Causal AI package for causal graphs."
 license = "Apache-2.0"
 authors = ["causaLens <opensource@causalens.com>"]
 readme = "README.md"
 homepage = "https://causalgraph.causalens.com/"
 repository = "https://github.com/causalens/cai-causal-graph"
 documentation = "https://causalgraph.causalens.com/"
```

### Comparing `cai_causal_graph-0.4.8.dev1/PKG-INFO` & `cai_causal_graph-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cai-causal-graph
-Version: 0.4.8.dev1
+Version: 0.4.9
 Summary: A Causal AI package for causal graphs.
 Home-page: https://causalgraph.causalens.com/
 License: Apache-2.0
 Author: causaLens
 Author-email: opensource@causalens.com
 Requires-Python: >=3.8.0,<3.13.0
 Classifier: License :: OSI Approved :: Apache Software License
```

