# Comparing `tmp/historydag-1.2.0.tar.gz` & `tmp/historydag-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "historydag-1.2.0.tar", last modified: Fri Jan 12 19:08:02 2024, max compression
+gzip compressed data, was "historydag-1.3.0.tar", last modified: Fri May  3 17:39:31 2024, max compression
```

## Comparing `historydag-1.2.0.tar` & `historydag-1.3.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 19:08:02.633085 historydag-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-01-12 19:07:54.000000 historydag-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-12 19:07:54.000000 historydag-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-01-12 19:08:02.633085 historydag-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-01-12 19:07:54.000000 historydag-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 19:08:02.633085 historydag-1.2.0/historydag/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-12 19:08:02.633085 historydag-1.2.0/historydag/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/beast_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16760 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/compact_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/counterops.py
--rw-r--r--   0 runner    (1001) docker     (127)   156127 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    21507 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/dag_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/dag_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (127)    31436 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/mutation_annotated_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    24598 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/parsimony.py
--rw-r--r--   0 runner    (1001) docker     (127)    34400 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/parsimony_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/sankoff_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/sequence_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    41839 2024-01-12 19:07:54.000000 historydag-1.2.0/historydag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 19:08:02.633085 historydag-1.2.0/historydag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-01-12 19:08:02.000000 historydag-1.2.0/historydag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-12 19:08:02.000000 historydag-1.2.0/historydag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 19:08:02.000000 historydag-1.2.0/historydag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-12 19:08:02.000000 historydag-1.2.0/historydag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-12 19:08:02.000000 historydag-1.2.0/historydag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-12 19:08:02.633085 historydag-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-12 19:07:54.000000 historydag-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 19:08:02.633085 historydag-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_compact_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_dag_sankoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_disambiguate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_edgeset.py
--rw-r--r--   0 runner    (1001) docker     (127)    37268 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_historydag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_mutation_annotated_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_node_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_subclass_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-12 19:07:54.000000 historydag-1.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-01-12 19:07:54.000000 historydag-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:31.339131 historydag-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-03 17:39:27.000000 historydag-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 17:39:27.000000 historydag-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-03 17:39:31.339131 historydag-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-03 17:39:27.000000 historydag-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:31.339131 historydag-1.3.0/historydag/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-03 17:39:31.339131 historydag-1.3.0/historydag/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/beast_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/compact_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/counterops.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166021 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/dag_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/dag_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31436 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/mutation_annotated_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/parsimony.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34409 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/parsimony_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/sankoff_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/sequence_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47988 2024-05-03 17:39:27.000000 historydag-1.3.0/historydag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:31.339131 historydag-1.3.0/historydag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-03 17:39:31.000000 historydag-1.3.0/historydag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-03 17:39:31.000000 historydag-1.3.0/historydag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:39:31.000000 historydag-1.3.0/historydag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 17:39:31.000000 historydag-1.3.0/historydag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 17:39:31.000000 historydag-1.3.0/historydag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 17:39:31.339131 historydag-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-03 17:39:27.000000 historydag-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:31.339131 historydag-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_compact_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_dag_sankoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_disambiguate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_edgeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_historydag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_mutation_annotated_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_node_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_subclass_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-03 17:39:27.000000 historydag-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-05-03 17:39:27.000000 historydag-1.3.0/versioneer.py
```

### Comparing `historydag-1.2.0/LICENSE` & `historydag-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/PKG-INFO` & `historydag-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historydag
-Version: 1.2.0
+Version: 1.3.0
 Summary: Basic history DAG implementation
 Home-page: https://matsengrp.github.io/historydag
 Author: Will Dumm
 Author-email: wdumm88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `historydag-1.2.0/README.md` & `historydag-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/__init__.py` & `historydag-1.3.0/historydag/__init__.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/beast_loader.py` & `historydag-1.3.0/historydag/beast_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""Provides utilities for parsing BEAST outputs and storing sampled trees in
+HistoryDag objects.
+
+This module uses ``dendropy`` to parse the newick strings found in BEAST output files, since
+``ete3`` is incompatible with newick strings containing commas other than those which separate
+nodes. The ``historydag`` package does not require ``dendropy``, so to use this module, you must
+manually ensure that ``dendropy`` is installed in your environment.
+"""
+
 import historydag as hdag
 from warnings import warn
 import dendropy
 import xml.etree.ElementTree as ET
 import historydag.parsimony_utils as parsimony_utils
 
 
@@ -16,23 +25,25 @@
     include_sequence_names_in_labels=False,
     transition_model=parsimony_utils.default_nt_transitions,
 ):
     """A convenience method to build a dag out of the output from
     :meth:`load_beast_trees`.
 
     Args:
-        beast_xml_file: ''
-        beast_output_file: ''
+        beast_xml_file: The xml input file to BEAST
+        beast_output_file: The .trees output file from BEAST
         reference_sequence: Provide a reference sequence, if desired. Otherwise, an arbitrary
             observed sequence will be used.
         topologies_only: If True, no internal sequences will be recovered from the beast output.
             In this case, leaf compact genomes will contain observed (possibly ambiguous)
             sequences regardless of the value of `use_original_leaves`.
-        mask_ambiguous_sites: ''
-        remove_ambiguous_sites: ''
+        mask_ambiguous_sites: If True, ignore mutations for all sites whose observed set
+            of characters is a subset of {N, -, ?} (recommended).
+        remove_ambiguous_sites: If True, acts like ``mask_ambiguous_sites=True``, except
+            the sites in question are actually removed from the sequence, rather than masked.
         use_original_leaves: Use the original observed sequences for leaf node labels, instead
             of thos derived from simulated mutations.
         include_sequence_names_in_labels: If True, augment leaf node labels with a ``name`` attribute
             containing the name of the corresponding sequence. Useful for distinguishing leaves when
             observed sequences are not unique.
     """
     dp_trees = load_beast_trees(
@@ -117,14 +128,15 @@
             the sites in question are actually removed from the sequence, rather than masked.
 
     Returns:
         A generator yielding :class:`dendropy.Tree`s output by BEAST, and a set of 0-based sites
         which are removed from sequences. If remove_ambiguous_sites is False, this set contains only
         sites ignored by BEAST. Otherwise, it also contains additional sites removed.
         Each tree has:
+
         * ancestral sequence attribute on each tree object, containing the complete reference
             for that tree
         * cg attribute on all nodes, containing a compact genome relative to the reference
             sequence
         * observed_cg attribute on leaf nodes, containing a compact genome describing the original
             observed sequence, with ambiguities, but with sites ignored by BEAST removed.
         * mut attribute on all nodes containing a list of mutations on parent branch, in
```

### Comparing `historydag-1.2.0/historydag/compact_genome.py` & `historydag-1.3.0/historydag/compact_genome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""This module provides a CompactGenome class, intended as a convenient and
+compact representation of a nucleotide sequence as a collection of mutations
+relative to a reference sequence.
+
+This object also provides methods to conveniently mutate CompactGenome
+objects according to a list of mutations, produce mutations defining the
+difference between two CompactGenome objects, and efficiently access the
+base at a site (or the entire sequence, as a string) implied by a
+CompactGenome.
+"""
+
 from frozendict import frozendict
 from typing import Dict, Sequence
 from warnings import warn
 from historydag.parsimony_utils import (
     standard_nt_ambiguity_map,
     default_nt_transitions,
     CharacterSequence,
```

### Comparing `historydag-1.2.0/historydag/counterops.py` & `historydag-1.3.0/historydag/counterops.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/dag.py` & `historydag-1.3.0/historydag/dag.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,114 @@
     This is a wrapper for the ``newclass.from_history_dag`` method,
     which for most subclasses should be identical to
     :meth:`HistoryDag.from_history_dag`.
     """
     return newclass.from_history_dag(dag)
 
 
+# Preorder tree creation class
+
+TreeBuilderNode = Any
+
+
+class PreorderTreeBuilder:
+    """Any class implementing a PreorderTreeBuilder interface can be used as a
+    tree sample constructor in :meth:`HistoryDag.fast_sample`. Subclasses
+    implementing this interface may implement an arbitrary constructor
+    interface, as the user will be responsible for creating instances to be
+    used for sampling. In addition, subclasses must implement the following
+    methods:
+
+    Methods:
+        add_node: This method must accept a :class:HistoryDagNode object ``dag_node`` and, optionally
+            a TreeBuilderNode instance ``parent``, representing the parent node of the node to be added,
+            and returns a TreeBuilderNode instance representing the added node in the sampled
+            tree. TreeBuilderNode can be any type which is convenient for the internal
+            implementation of the PreorderTreeBuilder subclass. This method can expect to be
+            called on nodes in a sampled tree in a pre-ordering. A parent node will always be
+            provided unless `dag_node` is the root node.
+        get_finished_tree: This method takes no arguments and returns the data defining the
+            sampled tree, after any necessary clean-up or final tree construction steps. Its
+            return value is the return value of :meth:`HistoryDag.fast_sample`.
+    """
+
+    pass
+
+
+class EteTreeBuilder(PreorderTreeBuilder):
+    def __init__(
+        self,
+        name_func: Callable[[HistoryDagNode], str] = lambda n: "unnamed",
+        features: Optional[List[str]] = [],
+        feature_funcs: Mapping[str, Callable[[HistoryDagNode], str]] = {},
+    ):
+        self.treeroot = None
+        self.name_func = name_func
+        self.feature_funcs = feature_funcs
+
+        for feature in features:
+
+            def feature_func(node):
+                return getattr(node.label, feature)
+
+            self.feature_funcs[feature] = feature_func
+
+        self.feature_funcs = tuple(self.feature_funcs.items())
+
+    def add_node(
+        self,
+        dag_node: HistoryDagNode,
+        parent: ete3.TreeNode = None,
+    ) -> ete3.TreeNode:
+        # Skip the UA Node
+        if isinstance(dag_node, UANode):
+            return None
+        newnode = ete3.TreeNode()
+        newnode.name = self.name_func(dag_node)
+        for feature, feature_func in self.feature_funcs:
+            newnode.add_feature(feature, feature_func(dag_node))
+        if parent is None:
+            assert self.treeroot is None
+            self.treeroot = newnode
+        else:
+            parent.add_child(child=newnode)
+        return newnode
+
+    def get_finished_tree(self):
+        return self.treeroot
+
+
+class PreorderHistoryBuilder(PreorderTreeBuilder):
+    def __init__(
+        self,
+        dag_type,
+    ):
+        self.root_node = None
+        self.edges = []
+        self.dag_type = dag_type
+
+    def add_node(
+        self,
+        dag_node: HistoryDagNode,
+        parent: HistoryDagNode = None,
+    ) -> HistoryDagNode:
+        new_node = dag_node.empty_copy()
+        if parent is None:
+            assert self.root_node is None
+            self.root_node = new_node
+        else:
+            self.edges.append((parent, new_node))
+        return new_node
+
+    def get_finished_tree(self):
+        for parent, child in reversed(self.edges):
+            parent.add_edge(child)
+        return self.dag_type(self.root_node)
+
+
 class HistoryDag:
     r"""An object to represent a collection of internally labeled trees. A
     wrapper object to contain exposed HistoryDag methods and point to a
     HistoryDagNode root.
 
     Args:
         dagroot: The root node of the history DAG
@@ -282,27 +382,63 @@
         ``self``.
         """
         if isinstance(key, utils.HistoryDagFilter):
             dag = self.copy()
             dag.trim_optimal_weight(**key)
             return dag
         elif isinstance(key, int):
+            # This call to count_histories is essential because we use
+            # the cached node counts later. For faster indexing, call this
+            # method once and call _get_subhistory_by_subid yourself.
             length = self.count_histories()
             if key < 0:
                 key = length + key
             if not (key >= 0 and key < length):
                 raise IndexError
-            self.count_histories()
-            return self.__class__(self.dagroot._get_subhistory_by_subid(key))
+            builder = PreorderHistoryBuilder(type(self))
+            self.dagroot._get_subhistory_by_subid(key, builder)
+            return builder.get_finished_tree()
         else:
             raise TypeError(
                 f"History DAG indices must be integers or utils.HistoryDagFilter"
                 f" objects, not {type(key)}"
             )
 
+    def get_histories_by_index(self, key_iterator, tree_builder_func=None):
+        """Retrieving a history by index is slow, since each retrieval requires
+        running the ``trim_optimal_weight`` method on the entire DAG to
+        populate node counts. This method instead runs that method a single
+        time and yields a history for each index yielded by ``key_iterator``.
+
+        Args:
+            key_iterator: An iterator on desired history indices. May be consumable, as
+                it will only be used once.
+            tree_builder_func: A function accepting an index and returning a
+                :class:`PreorderTreeBuilder` instance to be used to build the history
+                with that index. If None (default), then tree-shaped HistoryDag objects
+                will be yielded using :class:`PreorderHistoryBuilder`.
+        """
+        if tree_builder_func is None:
+
+            def tree_builder_func(idx):
+                return PreorderHistoryBuilder(type(self))
+
+        length = self.count_histories()
+
+        for key in key_iterator:
+            if key < 0:
+                key = length + key
+            if not (key >= 0 and key < length):
+                raise IndexError(
+                    f"Invalid index {key} in DAG containing {length} histories"
+                )
+            builder = tree_builder_func(key)
+            self.dagroot._get_subhistory_by_subid(key, builder)
+            yield builder.get_finished_tree()
+
     def get_label_type(self) -> type:
         """Return the type for labels on this dag's nodes."""
         return type(next(self.dagroot.children()).label)
 
     @get_default_args(["start_func", "edge_weight_func"])
     def trim_within_range(
         self,
@@ -676,25 +812,65 @@
         """Return the first (non-UA) node for which ``filter_func`` evaluates
         to True."""
         try:
             return next(self.find_nodes(filter_func))
         except StopIteration:
             raise ValueError("No matching node found.")
 
+    def fast_sample(
+        self,
+        tree_builder: PreorderTreeBuilder = None,
+        log_probabilities=False,
+    ):
+        """This is a non-recursive alternative to :meth:`HistoryDag.sample`,
+        which is likely to be slower on small DAGs, but may allow significant
+        optimizations on large DAGs, or in the case that the data format being
+        sampled is something other than a tree-shaped HistoryDag object.
+
+        This method does not provide an edge_selector argument like :meth:`HistoryDag.sample`.
+        Instead, any masking of edges should be done prior to sampling using the :meth:`HistoryDag.set_sample_mask`
+        method, or by modifying the arguments to :meth:`HistoryDag.probability_annotate`.
+
+        Args:
+            tree_builder: a PreorderTreeBuilder instance to handle construction of the sampled tree.
+            log_probabilities: Whether edge probabilities annotated on this DAG (using, for example,
+                :meth:`HistoryDag.probability_annotate`) are on a log-scale.
+        """
+        if tree_builder is None:
+            tree_builder = PreorderHistoryBuilder(type(self))
+
+        def get_sampled_children(node):
+            for clade, eset in node.clades.items():
+                sampled_target, _ = eset.sample(log_probabilities=log_probabilities)
+                yield sampled_target
+
+        node_queue = [(self.dagroot, tree_builder.add_node(self.dagroot))]
+
+        while len(node_queue) > 0:
+            parent, parent_repr = node_queue.pop()
+            for child in get_sampled_children(parent):
+                child_repr = tree_builder.add_node(child, parent=parent_repr)
+                node_queue.append((child, child_repr))
+
+        return tree_builder.get_finished_tree()
+
     def sample(
         self, edge_selector=lambda e: True, log_probabilities=False
     ) -> "HistoryDag":
         r"""Samples a history from the history DAG. (A history is a sub-history
         DAG containing the root and all leaf nodes) For reproducibility, set
         ``random.seed`` before sampling.
 
-        When there is an option, edges pointing to nodes on which `selection_func` is True
+        When there is an option, edges pointing to nodes on which `edge_selector` is True
         will always be chosen.
 
         Returns a new HistoryDag object.
+
+        To use the more general sampling pattern which allows an arbitrary PreorderTreeBuilder
+        object, use :meth:`HistoryDag.fast_sample` instead.
         """
         return self.__class__(
             self.dagroot._sample(
                 edge_selector=edge_selector, log_probabilities=log_probabilities
             )
         )
 
@@ -1167,37 +1343,28 @@
 
         Returns:
             An ete3 Tree with the same topology as self, and node names and attributes
             as specified.
         """
         # First build a dictionary of ete3 nodes keyed by HDagNodes.
         if features is None:
-            labelfeatures = list(
-                list(self.dagroot.children())[0].label._asdict().keys()
-            )
-        else:
-            labelfeatures = features
+            features = list(list(self.dagroot.children())[0].label._asdict().keys())
 
-        def etenode(node: HistoryDagNode) -> ete3.TreeNode:
-            newnode = ete3.TreeNode()
-            newnode.name = name_func(node)
-            for feature in labelfeatures:
-                newnode.add_feature(feature, getattr(node.label, feature))
-            for feature, func in feature_funcs.items():
-                newnode.add_feature(feature, func(node))
-            return newnode
-
-        nodedict = {node: etenode(node) for node in self.preorder(skip_ua_node=True)}
-
-        for node in nodedict:
-            for target in node.children():
-                nodedict[node].add_child(child=nodedict[target])
+        tree_builder = EteTreeBuilder(
+            name_func=name_func, features=features, feature_funcs=feature_funcs
+        )
+        nodes_to_process = [(self.dagroot, tree_builder.add_node(self.dagroot))]
+        while len(nodes_to_process) > 0:
+            node, node_repr = nodes_to_process.pop()
+            for child in node.children():
+                nodes_to_process.append(
+                    (child, tree_builder.add_node(child, parent=node_repr))
+                )
 
-        # Since self is cladetree, dagroot can have only one child
-        return nodedict[list(self.dagroot.children())[0]]
+        return tree_builder.get_finished_tree()
 
     def to_graphviz(
         self,
         labelfunc: Optional[Callable[[HistoryDagNode], str]] = None,
         namedict: Mapping[Label, str] = {},
         show_child_clades: bool = True,
         show_partitions: bool = None,
@@ -2945,14 +3112,44 @@
         for edge, _, prob in self.get_annotated_edges():
             key = collapse_key(edge)
             prob_list = edge_probabilities.setdefault(key, [])
             prob_list.append(accum_func([node_probabilities[edge[0]], prob]))
 
         return {key: aggregate_func(val) for key, val in edge_probabilities.items()}
 
+    def set_sample_mask(self, edge_selector, log_probabilities=False):
+        """Zero out edge weights for masked edges before calling
+        :meth:`HistoryDag.fast_sample`. This should be equivalent to passing
+        the same edge_selector function to :meth:`HistoryDag.sample`.
+
+        Args:
+            edge_selector: A function accepting an edge (a tuple of HistoryDagNode objects) and
+                returning True of False. An edge marked False will be ineligible for sampling, unless
+                all other edges in the same edge set are also marked False.
+            log_probabilities: Since the mask is applied by modifying edge probabilities, one must specify
+                whether those probabilities are on a log scale.
+
+        Take care to verify that you shouldn't instead use :meth:`HistoryDag.probability_annotate` with
+        a choice of ``edge_weight_func`` that takes into account the masking preferences.
+        """
+
+        if log_probabilities:
+            mask_value = float("-inf")
+        else:
+            mask_value = 0
+
+        for node in self.preorder():
+            for clade, eset in node.clades.items():
+                mask = tuple(edge_selector((node, target)) for target in eset.targets)
+                # If all mask values are false, then skip modifying probs.
+                if any(mask):
+                    for i, val in enumerate(mask):
+                        if not val:
+                            eset.probs[i] = mask_value
+
     def probability_annotate(
         self,
         edge_weight_func,
         log_probabilities=False,
         normalize_edgeweights=None,
         accum_func=None,
         aggregate_func=None,
@@ -3692,22 +3889,68 @@
     those nodes."""
     # use dictionary to preserve order
     nodes = {node.empty_copy(): node for node in nodes}
     # check for UA node in passed set, and recover if present:
     ua_node = UANode(EdgeSet())
     if ua_node in nodes:
         ua_node = nodes[ua_node].empty_copy()
-    nodes.pop(ua_node)
+        nodes.pop(ua_node)
     clade_dict = _clade_union_dict(nodes.keys())
     edge_dict = {
         node: [child for clade in node.clades for child in clade_dict[clade]]
         for node in nodes
     }
     children = {node: "" for _, children in edge_dict.items() for node in children}
     source_nodes = set(nodes) - set(children.keys())
     edge_dict[ua_node] = list(source_nodes)
 
     for node, children in edge_dict.items():
         for child in children:
             node.add_edge(child)
 
     return HistoryDag(ua_node)
+
+
+def make_binary_complete_dag(leaf_labels):
+    """Produce a history DAG containing all binary topologies on the provided
+    iterable of leaf labels."""
+    leaf_labels = list(leaf_labels)
+    model_label = leaf_labels[0]
+    if not isinstance(model_label, tuple):
+        raise ValueError(
+            "Provided labels must be a historydag Label type (a typing.NamedTuple instance)"
+        )
+    field_values = tuple(Ellipsis for _ in model_label)
+    internal_label = type(model_label)(*field_values)
+
+    node_set = {UANode(EdgeSet())}
+    for clade in utils.powerset(leaf_labels, start_size=1):
+        # Now need to get all splits of this clade into two child clades
+        cladesize = len(clade)
+        for child_mask in utils.powerset(
+            range(cladesize), start_size=1, end_size=cladesize - 1
+        ):
+            splitter_mask = [False] * cladesize
+            for idx in child_mask:
+                splitter_mask[idx] = True
+            clade1 = frozenset(
+                clade[idx] for idx, flag in enumerate(splitter_mask) if flag
+            )
+            clade2 = frozenset(
+                clade[idx] for idx, flag in enumerate(splitter_mask) if not flag
+            )
+            node_set.add(
+                HistoryDagNode(
+                    internal_label,
+                    {clade1: EdgeSet(), clade2: EdgeSet()},
+                    {},
+                )
+            )
+    for leaf_label in leaf_labels:
+        node_set.add(
+            HistoryDagNode(
+                leaf_label,
+                {},
+                {},
+            )
+        )
+    return history_dag_from_nodes(node_set)
```

### Comparing `historydag-1.2.0/historydag/dag_node.py` & `historydag-1.3.0/historydag/dag_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,23 @@
     Generator,
     Iterable,
     Set,
     Optional,
     Tuple,
     Dict,
     FrozenSet,
+    TYPE_CHECKING,
 )
 from copy import deepcopy
 from historydag import utils
 from historydag.utils import Weight, Label, UALabel
 
+if TYPE_CHECKING:
+    from historydag.dag import PreorderTreeBuilder
+
 
 class HistoryDagNode:
     r"""A recursive representation of a history DAG object.
 
     - a dictionary keyed by clades (frozensets) containing EdgeSet objects
     - a label, which is a namedtuple.
     """
@@ -179,43 +183,43 @@
             return self.clades[key].add_to_edgeset(
                 target,
                 weight=weight,
                 prob=prob,
                 prob_norm=prob_norm,
             )
 
-    def _get_subhistory_by_subid(self, subid: int) -> "HistoryDagNode":
-        r"""Returns the subtree below the current HistoryDagNode corresponding
-        to the given index."""
+    def _get_subhistory_by_subid(
+        self, subid: int, tree_builder: "PreorderTreeBuilder", parent_repr=None
+    ):
+        r"""Uses ``tree_builder`` to build the subtree below the current
+        HistoryDagNode corresponding to the given index."""
+        this_repr = tree_builder.add_node(self, parent=parent_repr)
         if self.is_leaf():  # base case - the node is a leaf
-            return self
+            return
         else:
-            history = self.empty_copy()
-
             # get the subtree for each of the clades
             for clade, eset in self.clades.items():
                 # get the sum of subtrees of the edges for this clade
                 num_subtrees = 0
                 for child, weight, _ in eset:
                     num_subtrees = num_subtrees + child._dp_data
                 curr_index = subid % num_subtrees
 
                 # find the edge corresponding to the curr_index
                 for child, weight, _ in eset:
                     if curr_index >= child._dp_data:
                         curr_index = curr_index - child._dp_data
                     else:
                         # add this edge to the tree somehow
-                        history.clades[clade].add_to_edgeset(
-                            child._get_subhistory_by_subid(curr_index)
+                        child._get_subhistory_by_subid(
+                            curr_index, tree_builder, parent_repr=this_repr
                         )
                         break
 
                 subid = subid / num_subtrees
-        return history
 
     def remove_edge_by_clade_and_id(self, target: "HistoryDagNode", clade: frozenset):
         key: frozenset
         if self.is_ua_node():
             key = frozenset()
         else:
             key = clade
@@ -523,16 +527,16 @@
             self._targetset = set(self.targets)
 
     def sample(
         self, mask=None, log_probabilities=False
     ) -> Tuple[HistoryDagNode, float]:
         """Returns a randomly sampled child edge, and its corresponding weight.
 
-        When possible, only edges pointing to child nodes on which
-        ``selection_function`` evaluates to True will be sampled.
+        When possible, only edges with nonzero mask value will be
+        sampled.
         """
         if log_probabilities:
             weights = [exp(weight) for weight in self.probs]
         else:
             weights = self.probs
 
         if mask is None or sum(mask) == 0:
```

### Comparing `historydag-1.2.0/historydag/dag_pb2.py` & `historydag-1.3.0/historydag/dag_pb2.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/likelihoods.py` & `historydag-1.3.0/historydag/likelihoods.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/mutation_annotated_dag.py` & `historydag-1.3.0/historydag/mutation_annotated_dag.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/parsimony.py` & `historydag-1.3.0/historydag/parsimony.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,16 @@
             or of type ``HistoryDag``, or else a list of nodes that respects postorder traversal. This last
             option is useful when using the Sankoff algorithm to compute node labels for a subset of the
             internal nodes of a history DAG, as only the nodes in the list will be relabelled. However it
             does assume that the remaining internal nodes are in fact equipped with a sequence.
         seq_len: The length of sequence for each leaf node.
         sequence_attr_name: the field name of the label attribute that is used to store sequences on nodes.
             Default value is set to 'sequence'
-        transition_model: The type of ``TransitionModel`` to use for Sankoff. See docstring for more information.
+        transition_model: The type of :meth:`parsimony_utils.TransitionModel` to use for Sankoff.
+            See docstring for more information.
         use_internal_node_sequences: (used when tree is of type ``ete3.TreeNode``) If True, then compute the
             transition cost for sequences assigned to internal nodes.
     """
 
     adj_arr = transition_model.get_adjacency_array(seq_len)
     if isinstance(node_list, ete3.TreeNode):
         # First pass of Sankoff: compute cost vectors
@@ -381,18 +382,23 @@
         compute_cvs: If true, compute upward sankoff cost vectors. If ``sankoff_upward`` was
             already run on the tree, this may be skipped.
         random_state: A ``random`` module random state, returned by ``random.getstate()``. Output
             from this function is otherwise deterministic.
         remove_cvs: Remove sankoff cost vectors from tree nodes after disambiguation.
         adj_dist: Recompute hamming parsimony distances on tree after disambiguation, and store them
             in ``dist`` node attributes.
+        transition_model: The type of :meth:`parsimony_utils.TransitionModel` to use for Sankoff.
+            See docstring for more information.
         min_ambiguities: If True, leaves ambiguities in reconstructed sequences, expressing which
             bases are possible at each site in a maximally parsimonious disambiguation of the given
             topology. In the history DAG paper, this is known as a strictly min-weight ambiguous labeling.
             Otherwise, sequences are resolved in one possible way, and include no ambiguities.
+        use_internal_node_sequences: If True, then instead of overwriting internal node sequences, only
+            disambiguate ambiguous bases in those sequences. For example, to fix a root sequence, this
+            option must be True.
     """
     if random_state is None:
         random.seed(tree.write(format=1))
     else:
         random.setstate(random_state)
 
     seq_len = len(next(tree.iter_leaves()).sequence)
```

### Comparing `historydag-1.2.0/historydag/parsimony_utils.py` & `historydag-1.3.0/historydag/parsimony_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,18 +204,19 @@
     between them, for weighted parsimony.
 
     In addition to them methods defined below, there are also attributes which are created by
     the constructor, which should be ensured to be correct in any subclass of TransitionModel:
 
     * ``base_indices`` is a dictionary mapping bases in ``self.bases`` to their indices
     * ``mask_vectors`` is a dictionary mapping ambiguity codes (including non-ambiguous bases)
-    to vectors of floats which are 0 at indices compatible with the ambiguity code, and infinity
-    otherwise.
+        to vectors of floats which are 0 at indices compatible with the ambiguity code, and infinity
+        otherwise.
     * ``bases`` is a tuple recording the correct order of unambiguous bases
 
+
     Args:
         bases: An ordered collection of valid character states
         transition_weights: A matrix describing transition costs between bases, with index order (from_base, to_base)
         ambiguity_map: An :class:`AmbiguityMap` object describing ambiguity codes. If not provided, the default
             mapping depends on the provided bases. If provided bases are ``AGCT``, then
             :class:`standard_nt_ambiguity_map` is used. If bases are ``AGCT-``, then
             :class:`standard_nt_ambiguity_map_gap_as_char` is used. Otherwise, it is assumed that no ambiguity
```

### Comparing `historydag-1.2.0/historydag/sankoff_cli.py` & `historydag-1.3.0/historydag/sankoff_cli.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/sequence_dag.py` & `historydag-1.3.0/historydag/sequence_dag.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/historydag/utils.py` & `historydag-1.3.0/historydag/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,52 @@
 from math import log, exp, isfinite
 from collections import Counter
 from functools import wraps
 import operator
 from collections import UserDict
 from decimal import Decimal
 from warnings import warn
+from itertools import chain, combinations
 from typing import (
     List,
     Any,
     TypeVar,
     Callable,
     Union,
     Iterable,
     Generator,
     Tuple,
     NamedTuple,
     Optional,
 )
 from typing import TYPE_CHECKING
 
+
+try:
+    from math import comb
+except ImportError:
+
+    def comb(n, k):
+        """
+        A fast way to calculate binomial coefficients
+        from https://stackoverflow.com/a/3025547
+        https://en.wikipedia.org/wiki/Binomial_coefficient#Multiplicative_formula
+        """
+        if 0 <= k <= n:
+            ntok = 1
+            ktok = 1
+            for t in range(1, min(k, n - k) + 1):
+                ntok *= n
+                ktok *= t
+                n -= 1
+            return ntok // ktok
+        else:
+            return 0
+
+
 if TYPE_CHECKING:
     from historydag.dag import HistoryDagNode, HistoryDag
 
 Weight = Any
 Label = Union[NamedTuple, "UALabel"]
 F = TypeVar("F", bound=Callable[..., Any])
 
@@ -1127,14 +1151,140 @@
 
     In these topologies, left and right branches are not distinguished,
     and internal nodes are not ranked.
     """
     return prod(range(1, 2 * n - 2, 2))
 
 
+def powerset(iterable, start_size=0, end_size=None):
+    """Produce all subsets of iterable (as tuples of elements), with sizes
+    starting at start_size and ending at end_size (inclusive), or the size of
+    the passed iterable if end_size is None."""
+    items = list(iterable)
+    if end_size is None:
+        end_size = len(items)
+    return chain.from_iterable(
+        combinations(items, r) for r in range(start_size, end_size + 1)
+    )
+
+
+def binary_support(clade_size, total_leaves, normalized=True):
+    """Calculate the fraction of binary trees on total_leaves containing a
+    particular clade containing clade_size leaves.
+
+    If normalized is False, instead returns the number of binary
+    topologies which would contain a particular clade of size
+    clade_size.
+    """
+    if clade_size > total_leaves:
+        raise ValueError("Clade size cannot exceed total number of leaves in tree")
+
+    count = count_labeled_binary_topologies(
+        clade_size
+    ) * count_labeled_binary_topologies(total_leaves - clade_size + 1)
+    # This could certainly be more numerically stable
+    if normalized:
+        return count / count_labeled_binary_topologies(total_leaves)
+    else:
+        return count
+
+
+def count_resolved_clade_supports(
+    n_child_clades, threshold=-1, min_size=1, max_size=None
+):
+    """Returns a generator on clade size, support pairs, for clades which would
+    result from binary resolution of a node posessing child clade sets in
+    node_child_clades.
+
+    Clade size means number of children of this node which are grouped
+    below a node.
+
+    Summing over the first element of yielded tuples gives the number of
+    elements which would be yielded by :meth:`iter_resolved_clade_supports`
+    provided with n_child_clades child clades and the same threshold
+    value.
+
+    Args:
+        n_child_clades: The number of children of the multifurcating node
+        threshold: If a resolved node's clade support value is below this threshold,
+            that clade will not be counted.
+        min_size: The minimum size of a clade to be counted.
+        max_size: The (inclusive) maximum size of a clade to be counted.
+            The maximum value is ``len(node_child_clades)``, which is equivalent
+            to the default value.
+
+    Note that by default, the root clade, including all leaves contained in
+    node_child_clades, as well as all the clades contained in
+    node_child_clades, are included and each have a support of 1. To exclude leaves, pass
+    ``min_size=2``.
+    """
+    num_children = n_child_clades
+    if max_size is None:
+        max_size = num_children
+    elif max_size > num_children:
+        raise ValueError("max_size cannot be greater than n_child_clades")
+    elif max_size < 1:
+        raise ValueError("max_size cannot be less than 1")
+    for unflattened_clade_size in range(min_size, max_size + 1):
+        # support will be the same for all clades of this size...
+        support = binary_support(unflattened_clade_size, num_children)
+        # ... so this check need only be done num_children times
+        if support > threshold:
+            yield (comb(num_children, unflattened_clade_size), support)
+
+
+def iter_resolved_clade_supports(
+    node_child_clades, threshold=-1, min_size=1, max_size=None
+):
+    """Returns a generator on clade, support pairs, for clades which would
+    result from binary resolution of a node posessing child clade sets in
+    node_child_clades. All clades with support > threshold are yielded,
+    avoiding iteration through too many clades on large multifurcations.
+
+    Args:
+        node_child_clades: A set of frozensets containing the clades of the children of a
+            multifurcating node.
+        threshold: If a resolved node's clade support value is below this threshold,
+            that clade will not be yielded.
+        min_size: The minimum size of a clade to be yielded. Note this is NOT simply the
+            size of the clade set, but rather the number of children of the multifurcating
+            node which are below the resolved node corresponding to the clade.
+        max_size: The (inclusive) maximum size of a clade to be yielded. See `min_size`
+            for a description of what size means. The maximum value is ``len(node_child_clades)``,
+            which is equivalent to the default value.
+
+    Note that by default, the root clade, including all leaves contained in
+    node_child_clades, as well as all the clades contained in
+    node_child_clades, are included and each have a support of 1. To exclude leaves, pass
+    ``min_size=2``.
+    """
+    if max_size is None:
+        max_size = len(node_child_clades)
+    elif max_size > len(node_child_clades):
+        raise ValueError("max_size cannot be greater than the number of child clades")
+    elif max_size < 1:
+        raise ValueError("max_size cannot be less than 1")
+
+    num_children = len(node_child_clades)
+    for unflattened_clade_size in range(min_size, max_size + 1):
+        # support will be the same for all clades of this size...
+        support = binary_support(unflattened_clade_size, num_children)
+        # ... so this check need only be done num_children times
+        if support > threshold:
+            for clade in map(
+                lambda ns: frozenset(chain.from_iterable(ns)),
+                powerset(
+                    node_child_clades,
+                    start_size=unflattened_clade_size,
+                    end_size=unflattened_clade_size,
+                ),
+            ):
+                yield (clade, support)
+
+
 def read_fasta(fastapath, sequence_type=str):
     """Load a fasta file as a generator which yields (sequence ID, sequence)
     pairs.
 
     The function ``sequence_type`` will be called on each sequence as it
     is read from the fasta file, and the resulting object will be yielded as the second
     item in each sequence record pair.
```

### Comparing `historydag-1.2.0/historydag.egg-info/PKG-INFO` & `historydag-1.3.0/historydag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historydag
-Version: 1.2.0
+Version: 1.3.0
 Summary: Basic history DAG implementation
 Home-page: https://matsengrp.github.io/historydag
 Author: Will Dumm
 Author-email: wdumm88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `historydag-1.2.0/historydag.egg-info/SOURCES.txt` & `historydag-1.3.0/historydag.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 historydag/sequence_dag.py
 historydag/utils.py
 historydag.egg-info/PKG-INFO
 historydag.egg-info/SOURCES.txt
 historydag.egg-info/dependency_links.txt
 historydag.egg-info/requires.txt
 historydag.egg-info/top_level.txt
+tests/test_binary_tree.py
 tests/test_collapse.py
 tests/test_compact_genome.py
 tests/test_dag_sankoff.py
 tests/test_disambiguate.py
 tests/test_edgeset.py
 tests/test_factory.py
 tests/test_historydag.py
```

### Comparing `historydag-1.2.0/setup.py` & `historydag-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_collapse.py` & `historydag-1.3.0/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_compact_genome.py` & `historydag-1.3.0/tests/test_compact_genome.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_dag_sankoff.py` & `historydag-1.3.0/tests/test_dag_sankoff.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_disambiguate.py` & `historydag-1.3.0/tests/test_disambiguate.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_edgeset.py` & `historydag-1.3.0/tests/test_edgeset.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_factory.py` & `historydag-1.3.0/tests/test_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,45 @@
         ndag._check_valid()
         ndag.trim_optimal_weight()
         ndag._check_valid()
         print(ndag.to_graphviz())
         assert wc == ndag.weight_count()
 
 
+def test_fast_sample_with_node():
+    random.seed(1)
+    dag = dags[-1]
+    dag.make_uniform()
+    node_to_count = dag.count_nodes()
+    min_count = min(node_to_count.values())
+    least_supported_nodes = [
+        node for node, val in node_to_count.items() if val == min_count
+    ]
+    for node in least_supported_nodes:
+        mask_true = dag.nodes_above_node(node)
+
+        def edge_selector(edge):
+            return edge[-1] in mask_true
+
+        dag.make_uniform()
+        dag.set_sample_mask(edge_selector)
+        tree_samples = [dag.fast_sample() for _ in range(min_count * 7)]
+        tree_samples[0]._check_valid()
+        tree_newicks = {tree.to_newick() for tree in tree_samples}
+        # We sampled all trees possible containing the node
+        assert len(tree_newicks) == min_count
+        # All trees sampled contained the node
+        assert all(node in set(tree.preorder()) for tree in tree_samples)
+        # # trees containing the node were sampled uniformly
+        # # (This is slow but seems to work)
+        # norms, avg = normalize_counts(Counter(tree.to_newick() for tree in tree_samples))
+        # print(norms)
+        # assert all(is_close(norm, avg) for norm in norms)
+
+
 def test_sample_with_node():
     random.seed(1)
     dag = dags[-1]
     dag.make_uniform()
     node_to_count = dag.count_nodes()
     min_count = min(node_to_count.values())
     least_supported_nodes = [
```

### Comparing `historydag-1.2.0/tests/test_historydag.py` & `historydag-1.3.0/tests/test_historydag.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,14 +237,26 @@
     for i in range(10):
         assert dag.sample().is_history()
     sample = dag.sample()
     sample._check_valid()
     sample.to_graphviz(namedict=namedict)
 
 
+def test_fast_sample():
+    newicks = ["((a, b)b, c)c;", "((a, b)c, c)c;", "((a, b)a, c)c;", "((a, b)r, c)r;"]
+    newicks = ["((1, 2)2, 3)3;", "((1, 2)3, 3)3;", "((1, 2)1, 3)3;", "((1, 2)4, 3)4;"]
+    namedict = {(str(x),): x for x in range(5)}
+    dag = history_dag_from_newicks(newicks, ["name"])
+    for i in range(10):
+        assert dag.fast_sample().is_history()
+    sample = dag.fast_sample()
+    sample._check_valid()
+    sample.to_graphviz(namedict=namedict)
+
+
 def test_unifurcation():
     # Make sure that unifurcations are handled correctly
     # First make sure the call works when the problem is fixed:
     from_newick("((a, b)b, c)c;", ["name"])
     try:
         from_newick("(((a, b)b, c)d)c;", ["name"])
         from_newick("(((a, b)d)b, c)c;", ["name"])
```

### Comparing `historydag-1.2.0/tests/test_mutation_annotated_dag.py` & `historydag-1.3.0/tests/test_mutation_annotated_dag.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_node_insert.py` & `historydag-1.3.0/tests/test_node_insert.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_subclass_conversion.py` & `historydag-1.3.0/tests/test_subclass_conversion.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_support.py` & `historydag-1.3.0/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/tests/test_utils.py` & `historydag-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `historydag-1.2.0/versioneer.py` & `historydag-1.3.0/versioneer.py`

 * *Files identical despite different names*

