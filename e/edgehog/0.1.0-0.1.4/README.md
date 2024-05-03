# Comparing `tmp/edgehog-0.1.0.tar.gz` & `tmp/edgehog-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgehog-0.1.0.tar", max compression
+gzip compressed data, was "edgehog-0.1.4.tar", max compression
```

## Comparing `edgehog-0.1.0.tar` & `edgehog-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5132 2023-04-12 13:44:23.289664 edgehog-0.1.0/README.md
--rw-r--r--   0        0        0       78 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/__init__.py
--rw-r--r--   0        0        0     4758 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/add_ons.py
--rw-r--r--   0        0        0     2153 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/characterize_species_tree.py
--rw-r--r--   0        0        0     2266 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/check_args.py
--rw-r--r--   0        0        0     4510 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/edgehog.py
--rw-r--r--   0        0        0    25302 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/infer_ancestral_synteny_graphs.py
--rw-r--r--   0        0        0     8698 2023-04-12 13:44:23.289664 edgehog-0.1.0/edgehog/init_extant_synteny_graphs.py
--rw-r--r--   0        0        0     1979 2023-04-12 13:44:23.293664 edgehog-0.1.0/edgehog/process_hogs.py
--rw-r--r--   0        0        0     7602 2023-04-12 13:44:23.293664 edgehog-0.1.0/edgehog/read_gff.py
--rw-r--r--   0        0        0     7922 2023-04-12 13:44:23.293664 edgehog-0.1.0/edgehog/write_output.py
--rw-r--r--   0        0        0      876 2023-04-12 13:44:23.293664 edgehog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6211 1970-01-01 00:00:00.000000 edgehog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5123 2024-05-03 11:22:07.469913 edgehog-0.1.4/README.md
+-rw-r--r--   0        0        0       78 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/__init__.py
+-rw-r--r--   0        0        0     4512 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/add_ons.py
+-rw-r--r--   0        0        0     2153 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/characterize_species_tree.py
+-rw-r--r--   0        0        0     1895 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/check_args.py
+-rw-r--r--   0        0        0     5041 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/edgehog.py
+-rw-r--r--   0        0        0    25302 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/infer_ancestral_synteny_graphs.py
+-rw-r--r--   0        0        0     8713 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/init_extant_synteny_graphs.py
+-rw-r--r--   0        0        0     1979 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/process_hogs.py
+-rw-r--r--   0        0        0     7602 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/read_gff.py
+-rw-r--r--   0        0        0    11626 2024-05-03 11:22:07.469913 edgehog-0.1.4/edgehog/write_output.py
+-rw-r--r--   0        0        0      884 2024-05-03 11:22:07.469913 edgehog-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6107 1970-01-01 00:00:00.000000 edgehog-0.1.4/PKG-INFO
```

### Comparing `edgehog-0.1.0/README.md` & `edgehog-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ### From sources
 ```edgeHOG``` was built and tested with python 3.6. To set up ```edgeHOG``` on your local machine, please follow the instructions below
 
 ```bash
 git clone https://github.com/dessimozlab/edgehog.git
 cd edgehog
-python setup.py install
+poetry install
 ```
 
 ## Usage
 
 ```
 usage: edgehog [-h] [--version] [--output_directory OUTPUT_DIRECTORY]
                --species_tree SPECIES_TREE --hogs HOGS
```

### Comparing `edgehog-0.1.0/edgehog/add_ons.py` & `edgehog-0.1.4/edgehog/add_ons.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,41 +2,40 @@
 # -*- coding: utf-8 -*-
 import pyham
 
 
 def date_edges(ham):
     print('###################################')
     print('Predicting age of extant edges ...')
-    lca = dict()
     for tree_node in ham.taxonomy.tree.traverse('preorder'):
         try:
             genome = tree_node.genome
         except AttributeError:
             print('No genome stored for {}'.format(tree_node.name))
             continue
         if isinstance(genome, pyham.AncestralGenome):
             graph = tree_node.top_down_synteny
-            for gene, adjacent_gene, edge_attributes in graph.edges.data():
-                edge_key = sorted([gene.get_top_level_hog().hog_id, adjacent_gene.get_top_level_hog().hog_id])
-                if (edge_key[0], edge_key[1]) not in lca:
-                    lca[(edge_key[0], edge_key[1])] = tree_node
         elif isinstance(genome, pyham.ExtantGenome):
             graph = tree_node.bottom_up_synteny
-            for gene, adjacent_gene, edge_attributes in graph.edges.data():
+        if tree_node.up:
+            parent_graph = tree_node.up.top_down_synteny
+        for gene, adjacent_gene, edge_attributes in graph.edges.data():
+            if not tree_node.up:
+                graph[gene][adjacent_gene]["lca_node"] = tree_node
+            else:
                 if gene.parent is None or adjacent_gene.parent is None:
-                    lca_edge = genome.name
-                    age_edge = 0
+                    graph[gene][adjacent_gene]["lca_node"] = tree_node
                 else:
-                    edge_key = sorted([gene.get_top_level_hog().hog_id, adjacent_gene.get_top_level_hog().hog_id])
-                    if (edge_key[0], edge_key[1]) not in lca:
-                        lca[(edge_key[0], edge_key[1])] = tree_node
-                    lca_edge = lca[(edge_key[0], edge_key[1])].genome.name
-                    age_edge = 1 - lca[(edge_key[0], edge_key[1])].red
-                graph[gene][adjacent_gene]["age"] = age_edge
-                graph[gene][adjacent_gene]["lca"] = lca_edge
+                    parent_edge = (gene.parent, adjacent_gene.parent)
+                    if parent_graph.has_edge(*parent_edge):
+                        graph[gene][adjacent_gene]["lca_node"] = parent_graph[gene.parent][adjacent_gene.parent]["lca_node"]
+                    else:
+                        graph[gene][adjacent_gene]["lca_node"] = tree_node
+            graph[gene][adjacent_gene]["lca"] = graph[gene][adjacent_gene]["lca_node"].genome.name
+            graph[gene][adjacent_gene]["age"] = 1 - graph[gene][adjacent_gene]["lca_node"].red
 
 
 def phylostratify(ham):
     print('###################################')
     print('Phylostratigraphy ...')
     for tree_node in ham.taxonomy.tree.traverse('preorder'):
         try:
@@ -87,16 +86,7 @@
                         desc_a = gene.get_at_level(genome)
                         desc_b = adjacent_gene.get_at_level(genome)
                         stratigraphy["lost_edges_due_to_rearrangement"] += 1
                     except:
                         stratigraphy["lost_edges_due_to_gene_loss"] += 1
                     
             tree_node.add_feature('stratigraphy', stratigraphy)      
-                    
-                
-                
-                
-                
-                
-                
-                
-
```

### Comparing `edgehog-0.1.0/edgehog/characterize_species_tree.py` & `edgehog-0.1.4/edgehog/characterize_species_tree.py`

 * *Files identical despite different names*

### Comparing `edgehog-0.1.0/edgehog/check_args.py` & `edgehog-0.1.4/edgehog/check_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,16 @@
 
 import os
 import re
 import sys
 import shutil
 
 
-def check_out_dir(parent_dir):
-    # create a directory 'ansyn_output' in the output directory provided by the user
-    if not os.path.exists(parent_dir):
-        sys.exit('error: Unable to locate \'%s\'. '
-                 'Please provide a correct path to the output directory' % parent_dir)
-    out_dir = os.path.join(parent_dir, 'edgehog_output')
-    if os.path.exists(out_dir):
-        shutil.rmtree(out_dir)
-    os.makedirs(out_dir)
+def check_out_dir(out_dir):
+    os.makedirs(out_dir, exist_ok=True)
     return out_dir
 
 
 def check_path_exists(file):
     if not os.path.exists(file):
         sys.exit('error: Unable to locate \'%s\'' % file)
```

### Comparing `edgehog-0.1.0/edgehog/edgehog.py` & `edgehog-0.1.4/edgehog/edgehog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,103 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
-import edgehog
+from . import __version__ as version
 import argparse
-from edgehog.check_args import check_args
-from edgehog.process_hogs import map_hogs_onto_tree, get_hogxml_entries
-from edgehog.characterize_species_tree import characterize_tree
-from edgehog.init_extant_synteny_graphs import init_extant_graphs, init_extant_graphs_from_hdf5
-from edgehog.infer_ancestral_synteny_graphs import leaves_to_root_synteny_propagation, root_to_leaves_edge_trimming, linearize_graphs
-from edgehog.write_output import write_output
-from edgehog.add_ons import date_edges, phylostratify
+from .check_args import check_args
+from .process_hogs import map_hogs_onto_tree, get_hogxml_entries
+from .characterize_species_tree import characterize_tree
+from .init_extant_synteny_graphs import init_extant_graphs, init_extant_graphs_from_hdf5
+from .infer_ancestral_synteny_graphs import leaves_to_root_synteny_propagation, root_to_leaves_edge_trimming, linearize_graphs
+from .write_output import write_output, write_as_hdf5
+from .add_ons import date_edges, phylostratify
 import time
 
 
 
 def main():
     arg_parser = argparse.ArgumentParser(description='edgehog is a software tool that infers an ancestral synteny graph '
                                          'at each internal node of an input species phylogenetic tree')
-    arg_parser.add_argument('--version', action='version', help='print version number and exit', version=edgehog.__version__)
-    arg_parser.add_argument('--output_directory', default='./', type = str, help='path to output directory (default is current directory)')
+    arg_parser.add_argument('--version', action='version', help='print version number and exit', version=version)
+    arg_parser.add_argument('--output_directory', default='./edgehog_output', type=str, help='path to output directory (default is ./edgehog_output)')
     arg_parser.add_argument('--species_tree', type=str, required=True, help='path to species/genomes phylogenetic tree (newick format)')
     arg_parser.add_argument('--hogs', type=str, required=True, help='path to the HierarchicalGroups.orthoxml file in which HOGs are stored')
     arg_parser.add_argument('--gff_directory', type=str, help='path to directory with the gffs of extant genomes '
                             '(each gff file must be named according to the name of an extant genome / leaf on the species tree)')
     arg_parser.add_argument('--hdf5', type=str, help='path to the hdf5 file (alternative to gff_directory to run edgeHOG on the entire OMA database)')
     arg_parser.add_argument('--date_edges', action='store_true', help='whether the age of edges in extant species should be predicted')
     arg_parser.add_argument('--phylostratify', action='store_true', help='whether the number of edge retention, gain and loss should be analyzed for each node of the species tree')
     arg_parser.add_argument('--max_gaps', type=int, help='max_gaps can be seen as the theoritical maximal number of consecutive novel genes that can emerge between two older genes (default = 3), '
                             'e.g.  if max_gaps = 2: the probabilistic A-b-c-D-E-f-g-h-I-J graph will be turn into A-D-E ; I-J in the ancestor'
                             'while if max_gaps = 3: the probabilistic A-b-c-D-E-f-g-h-I-J graph will be turn into A-D-E-I-J   in the ancestor', default=3)
     # arg_parser.add_argument('--cpu', type=str, default='1', help='number of CPUs to use (default is 1)')
+    arg_parser.add_argument('--include_extant_genes', action='store_true', help='include extant genes in output file for ancestral reconstructions.')
+    arg_parser.add_argument("--out-format", choices=("TSV", "HDF5"), default="TSV",
+                            help="define output format. Can be TSV (tab seperated files) or HDF5 (compatible for integration into oma hdf5)")
     args = arg_parser.parse_args()
-    
+
     timer = dict()
-    
+
     start_time = time.time()
     out_dir = check_args(args)
-    
+
     ham = map_hogs_onto_tree(args.hogs, args.species_tree, args.hdf5)
     hogxml_entries, protein_id_to_hogxml_entry = get_hogxml_entries(ham)
-    
     characterize_tree(ham.taxonomy.tree)
-    
+    end_time = time.time()
+    timer["preprocessing - loading orthoxml"] = end_time - start_time
+
+    start_time = time.time()
     if args.gff_directory:
         init_extant_graphs(1, ham, args.hogs, args.gff_directory, hogxml_entries, protein_id_to_hogxml_entry)
     elif args.hdf5:
         init_extant_graphs_from_hdf5(ham, args.hdf5)
-      
+
     end_time = time.time()
-    timer["preprocessing"] = end_time - start_time
-   
+    timer["preprocessing - loading extant synteny"] = end_time - start_time
+
     start_time = time.time()
     leaves_to_root_synteny_propagation(ham, args.max_gaps)
     end_time = time.time()
     timer["bottom-up phase"] = end_time - start_time
-    
+
     start_time = time.time()
     root_to_leaves_edge_trimming(ham)
     end_time = time.time()
     timer["top-down phase"] = end_time - start_time
-        
-    start_time = time.time()
-    linearize_graphs(ham)
-    end_time = time.time()
-    timer["linearization"] = end_time - start_time
-    
+
     if args.date_edges:
         start_time = time.time()
         date_edges(ham)
         end_time = time.time()
         timer["edge datation"] = end_time - start_time
-        
+
+    start_time = time.time()
+    linearize_graphs(ham)
+    end_time = time.time()
+    timer["linearization"] = end_time - start_time
+
     if args.phylostratify:
         start_time = time.time()
         phylostratify(ham)
         end_time = time.time()
         timer["phylostratigraphy"] = end_time - start_time
-    
+
     start_time = time.time()
-    write_output(args, ham, out_dir)
+    if args.out_format == "HDF5":
+        write_as_hdf5(args, ham, out_dir)
+    else:
+        write_output(args, ham, out_dir)
     end_time = time.time()
     timer["writing output"] = end_time - start_time
-    
+
     print('Completed!')
-    
+
     print('###################################')
     for step in timer:
-        print("%s:\tdone in %.3f seconds" % (step, timer[step]))
-    
+        print("%30s:\tdone in %.3f seconds" % (step, timer[step]))
+
 
-if __name__=='__main__': 
+if __name__=='__main__':
     main()
-    
+
```

### Comparing `edgehog-0.1.0/edgehog/infer_ancestral_synteny_graphs.py` & `edgehog-0.1.4/edgehog/infer_ancestral_synteny_graphs.py`

 * *Files identical despite different names*

### Comparing `edgehog-0.1.0/edgehog/init_extant_synteny_graphs.py` & `edgehog-0.1.4/edgehog/init_extant_synteny_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,11 +174,12 @@
         #     if len(cc > 1):
         #         for i in range(0, len(cc)):
         #             for j in range(i+1, len(cc)): 
         #                 node_a, node_b = cc[i], cc[j]
         #                 contiguity_dict[(node_a, node_b)] = contiguity_dict[(node_b, node_a)] = 1
         gene.genome.taxon.add_feature('bottom_up_synteny', graph)
         gene.genome.taxon.add_feature('contiguity_dict', contiguity_dict)
+    h5.close()
     return ham
```

### Comparing `edgehog-0.1.0/edgehog/process_hogs.py` & `edgehog-0.1.4/edgehog/process_hogs.py`

 * *Files identical despite different names*

### Comparing `edgehog-0.1.0/edgehog/read_gff.py` & `edgehog-0.1.4/edgehog/read_gff.py`

 * *Files identical despite different names*

### Comparing `edgehog-0.1.0/pyproject.toml` & `edgehog-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "edgehog"
-version = "0.1.0"
+version = "0.1.4"
 description = "Infering ancestral synteny with hierarchical orthologous groups"
 authors = ["Charles Bernard <charles.bernard@unil.ch>",
            "Adrian Altenhoff <adrian.altenhoff@inf.ethz.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DessimozLab/edgehog"
 keywords = ["bioinformatics", "synteny", "ancestral gene order"]
 classifiers = [
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.10,<3.13"
 numpy = "^1.20.0"
 pandas = ">1.3.0,<2.0.0"
 networkx = "^2.8"
 pyham = "^1.1.11"
 ete3 = "^3.1.2"
 pyoma = "^0.12.1"
```

### Comparing `edgehog-0.1.0/PKG-INFO` & `edgehog-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: edgehog
-Version: 0.1.0
+Version: 0.1.4
 Summary: Infering ancestral synteny with hierarchical orthologous groups
 Home-page: https://github.com/DessimozLab/edgehog
 License: MIT
 Keywords: bioinformatics,synteny,ancestral gene order
 Author: Charles Bernard
 Author-email: charles.bernard@unil.ch
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: ete3 (>=3.1.2,<4.0.0)
 Requires-Dist: networkx (>=2.8,<3.0)
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas (>1.3.0,<2.0.0)
 Requires-Dist: pyham (>=1.1.11,<2.0.0)
 Requires-Dist: pyoma (>=0.12.1,<0.13.0)
@@ -42,15 +40,15 @@
 
 ### From sources
 ```edgeHOG``` was built and tested with python 3.6. To set up ```edgeHOG``` on your local machine, please follow the instructions below
 
 ```bash
 git clone https://github.com/dessimozlab/edgehog.git
 cd edgehog
-python setup.py install
+poetry install
 ```
 
 ## Usage
 
 ```
 usage: edgehog [-h] [--version] [--output_directory OUTPUT_DIRECTORY]
                --species_tree SPECIES_TREE --hogs HOGS
```

