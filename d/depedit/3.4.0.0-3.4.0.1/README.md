# Comparing `tmp/depedit-3.4.0.0.tar.gz` & `tmp/depedit-3.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depedit-3.4.0.0.tar", last modified: Wed May  1 21:23:17 2024, max compression
+gzip compressed data, was "depedit-3.4.0.1.tar", last modified: Thu May  2 22:20:37 2024, max compression
```

## Comparing `depedit-3.4.0.0.tar` & `depedit-3.4.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 21:23:17.174068 depedit-3.4.0.0/
--rw-rw-rw-   0        0        0    11560 2015-10-19 14:53:17.000000 depedit-3.4.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      728 2024-05-01 21:23:17.173093 depedit-3.4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3047 2022-08-20 14:24:59.000000 depedit-3.4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 21:23:17.156068 depedit-3.4.0.0/depedit/
--rw-rw-rw-   0        0        0       48 2019-01-05 19:27:46.000000 depedit-3.4.0.0/depedit/__init__.py
--rw-rw-rw-   0        0        0       93 2021-04-30 14:53:22.000000 depedit-3.4.0.0/depedit/__main__.py
--rw-rw-rw-   0        0        0    42152 2021-03-03 19:46:21.000000 depedit-3.4.0.0/depedit/depedit - Copy.py
--rw-rw-rw-   0        0        0    69748 2024-05-01 21:20:01.000000 depedit-3.4.0.0/depedit/depedit.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:23:17.171069 depedit-3.4.0.0/depedit.egg-info/
--rw-rw-rw-   0        0        0      728 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-05-01 21:23:17.000000 depedit-3.4.0.0/depedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-01 21:23:16.000000 depedit-3.4.0.0/depedit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 21:23:17.175069 depedit-3.4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-05-01 21:19:38.000000 depedit-3.4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 22:20:37.357604 depedit-3.4.0.1/
+-rw-rw-rw-   0        0        0    11560 2015-10-19 14:53:17.000000 depedit-3.4.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      728 2024-05-02 22:20:37.356604 depedit-3.4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3047 2022-08-20 14:24:59.000000 depedit-3.4.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 22:20:37.348604 depedit-3.4.0.1/depedit/
+-rw-rw-rw-   0        0        0       48 2019-01-05 19:27:46.000000 depedit-3.4.0.1/depedit/__init__.py
+-rw-rw-rw-   0        0        0       93 2021-04-30 14:53:22.000000 depedit-3.4.0.1/depedit/__main__.py
+-rw-rw-rw-   0        0        0    42152 2021-03-03 19:46:21.000000 depedit-3.4.0.1/depedit/depedit - Copy.py
+-rw-rw-rw-   0        0        0    69757 2024-05-01 22:23:40.000000 depedit-3.4.0.1/depedit/depedit.py
+drwxrwxrwx   0        0        0        0 2024-05-02 22:20:37.355604 depedit-3.4.0.1/depedit.egg-info/
+-rw-rw-rw-   0        0        0      728 2024-05-02 22:20:37.000000 depedit-3.4.0.1/depedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-05-02 22:20:37.000000 depedit-3.4.0.1/depedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 22:20:37.000000 depedit-3.4.0.1/depedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-02 22:20:37.000000 depedit-3.4.0.1/depedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 22:20:37.000000 depedit-3.4.0.1/depedit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 22:20:37.357604 depedit-3.4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-02 22:18:31.000000 depedit-3.4.0.1/setup.py
```

### Comparing `depedit-3.4.0.0/LICENSE.txt` & `depedit-3.4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `depedit-3.4.0.0/PKG-INFO` & `depedit-3.4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depedit
-Version: 3.4.0.0
+Version: 3.4.0.1
 Summary: A simple configurable tool for manipulating dependency trees
 Home-page: https://github.com/amir-zeldes/depedit
-Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.0
+Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.1
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
 Keywords: NLP,parsing,syntax,dependencies,dependency,tree,treebank,conll,conllu,ud,enhanced
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `depedit-3.4.0.0/README.md` & `depedit-3.4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `depedit-3.4.0.0/depedit/depedit - Copy.py` & `depedit-3.4.0.1/depedit/depedit - Copy.py`

 * *Files identical despite different names*

### Comparing `depedit-3.4.0.0/depedit/depedit.py` & `depedit-3.4.0.1/depedit/depedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from decimal import Decimal
 from collections import defaultdict
 from copy import copy, deepcopy
 from glob import glob
 import io
 from six import iteritems, iterkeys
 
-__version__ = "3.4.0.0"
+__version__ = "3.4.0.1"
 
 ALIASES = {"form":"text","upostag":"pos","xpostag":"cpos","feats":"morph","deprel":"func","deps":"head2","misc":"func2",
            "xpos": "cpos","upos":"pos"}
 
 
 def escape(string, symbol_to_mask, border_marker):
     inside = False
@@ -992,15 +992,15 @@
                                 new_vals = sorted(value.split("|"))
                                 new_vals_keys = defaultdict(set)
                                 for pair in new_vals:
                                     this_key, this_val = pair.split("=")
                                     new_vals_keys[this_key].add(this_val)
                                 if old_val != "_" and isinstance(old_val,str):  # Some values already exist
                                     kv = []
-                                    for ov in sorted(old_val.split("|")):
+                                    for ov in sorted(old_val.split("|")+new_vals):
                                         this_key, this_val = ov.split("=")
                                         if this_key not in new_vals_keys:  # Else this needs to be overwritten
                                             kv.append(ov)
                                         else:
                                             kv.append(this_key + "=" + ",".join(sorted(list(new_vals_keys[this_key].union(set(this_val.split(",")))))))
                                     value = "|".join(sorted(kv,key=lambda x:x.lower()))
                                 else:
```

### Comparing `depedit-3.4.0.0/depedit.egg-info/PKG-INFO` & `depedit-3.4.0.1/depedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: depedit
-Version: 3.4.0.0
+Version: 3.4.0.1
 Summary: A simple configurable tool for manipulating dependency trees
 Home-page: https://github.com/amir-zeldes/depedit
-Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.0
+Download-URL: https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.1
 Author: Amir Zeldes
 Author-email: amir.zeldes@georgetown.edu
 License: Apache License, Version 2.0
 Keywords: NLP,parsing,syntax,dependencies,dependency,tree,treebank,conll,conllu,ud,enhanced
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `depedit-3.4.0.0/setup.py` & `depedit-3.4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 
 setup(
   name = 'depedit',
   packages = ['depedit'],
-  version = '3.4.0.0',
+  version = '3.4.0.1',
   description = 'A simple configurable tool for manipulating dependency trees',
   author = 'Amir Zeldes',
   author_email = 'amir.zeldes@georgetown.edu',
   url = 'https://github.com/amir-zeldes/depedit',
   install_requires=["six"],
   license='Apache License, Version 2.0',
-  download_url = 'https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.0',
+  download_url = 'https://github.com/amir-zeldes/depedit/releases/tag/3.4.0.1',
   keywords = ['NLP', 'parsing', 'syntax', 'dependencies', 'dependency', 'tree', 'treebank', 'conll', 'conllu', 'ud', 'enhanced'],
   classifiers = ['Programming Language :: Python',
 'Programming Language :: Python :: 2',
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: Apache Software License',
 'Operating System :: OS Independent'],
 )
```

