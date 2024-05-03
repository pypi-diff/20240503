# Comparing `tmp/lektor_fixedlang-0.4.tar.gz` & `tmp/lektor_fixedlang-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor_fixedlang-0.4.tar", last modified: Mon Apr 29 20:19:27 2024, max compression
+gzip compressed data, was "lektor_fixedlang-0.5.tar", last modified: Fri May  3 11:33:10 2024, max compression
```

## Comparing `lektor_fixedlang-0.4.tar` & `lektor_fixedlang-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-29 20:19:27.778492 lektor_fixedlang-0.4/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1491 2024-02-21 13:50:36.000000 lektor_fixedlang-0.4/LICENSE.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     4448 2024-04-29 20:19:27.778492 lektor_fixedlang-0.4/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)     1443 2024-04-29 20:18:05.000000 lektor_fixedlang-0.4/README.rst
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-29 20:19:27.774492 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     4448 2024-04-29 20:19:27.000000 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/PKG-INFO
--rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-04-29 20:19:27.000000 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/SOURCES.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-04-29 20:19:27.000000 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/dependency_links.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-04-29 20:19:27.000000 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/entry_points.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)      106 2024-04-29 20:19:27.000000 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/requires.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-04-29 20:19:27.000000 lektor_fixedlang-0.4/lektor_fixedlang.egg-info/top_level.txt
--rw-r--r--   0 uyar      (1000) uyar      (1000)     2750 2024-04-29 20:18:31.000000 lektor_fixedlang-0.4/lektor_fixedlang.py
--rw-r--r--   0 uyar      (1000) uyar      (1000)     2109 2024-04-29 20:18:16.000000 lektor_fixedlang-0.4/pyproject.toml
--rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-04-29 20:19:27.778492 lektor_fixedlang-0.4/setup.cfg
-drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-04-29 20:19:27.774492 lektor_fixedlang-0.4/tests/
--rw-r--r--   0 uyar      (1000) uyar      (1000)     3055 2024-04-29 20:12:54.000000 lektor_fixedlang-0.4/tests/test_fixedlang.py
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-05-03 11:33:10.364956 lektor_fixedlang-0.5/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1491 2024-02-21 13:50:36.000000 lektor_fixedlang-0.5/LICENSE.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     4448 2024-05-03 11:33:10.364956 lektor_fixedlang-0.5/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     1443 2024-04-29 20:30:46.000000 lektor_fixedlang-0.5/README.rst
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-05-03 11:33:10.364956 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     4448 2024-05-03 11:33:10.000000 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/PKG-INFO
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      323 2024-05-03 11:33:10.000000 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/SOURCES.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)        1 2024-05-03 11:33:10.000000 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/dependency_links.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       62 2024-05-03 11:33:10.000000 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/entry_points.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)      106 2024-05-03 11:33:10.000000 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/requires.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       17 2024-05-03 11:33:10.000000 lektor_fixedlang-0.5/lektor_fixedlang.egg-info/top_level.txt
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2624 2024-05-03 11:31:57.000000 lektor_fixedlang-0.5/lektor_fixedlang.py
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     2109 2024-05-03 11:31:52.000000 lektor_fixedlang-0.5/pyproject.toml
+-rw-r--r--   0 uyar      (1000) uyar      (1000)       38 2024-05-03 11:33:10.364956 lektor_fixedlang-0.5/setup.cfg
+drwxr-xr-x   0 uyar      (1000) uyar      (1000)        0 2024-05-03 11:33:10.364956 lektor_fixedlang-0.5/tests/
+-rw-r--r--   0 uyar      (1000) uyar      (1000)     3055 2024-04-29 20:30:46.000000 lektor_fixedlang-0.5/tests/test_fixedlang.py
```

### Comparing `lektor_fixedlang-0.4/LICENSE.txt` & `lektor_fixedlang-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lektor_fixedlang-0.4/PKG-INFO` & `lektor_fixedlang-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-fixedlang
-Version: 0.4
+Version: 0.5
 Summary: Set fixed languages for patterns in Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `lektor_fixedlang-0.4/README.rst` & `lektor_fixedlang-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `lektor_fixedlang-0.4/lektor_fixedlang.egg-info/PKG-INFO` & `lektor_fixedlang-0.5/lektor_fixedlang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-fixedlang
-Version: 0.4
+Version: 0.5
 Summary: Set fixed languages for patterns in Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2024 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `lektor_fixedlang-0.4/lektor_fixedlang.py` & `lektor_fixedlang-0.5/lektor_fixedlang.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2024 H. Turgut Uyar <uyar@tekir.org>
 #
 # lektor-fixedlang is released under the BSD license.
 # Read the included LICENSE.txt file for details.
 
-__version__ = "0.4"
+__version__ = "0.5"
 
 import re
 from functools import partial
 from pathlib import Path
 
 from lektor.db import Page
 from lektor.pluginsystem import Plugin
@@ -37,29 +37,25 @@
 
     def on_setup_env(self, **extra):
         config = self.get_config()
         self.patterns = []
         for lang in config.sections():
             for _, pattern in config.section_as_dict(lang).items():
                 self.patterns.append((pattern, lang))
-        self.processed = set()
 
     def on_before_build_all(self, builder, **extra):
         reporter.report_generic("Starting setting fixed languages")
 
     def on_after_build(self, builder, build_state, source, prog, **extra):
         if not isinstance(source, Page):
             return
         artifact = prog.primary_artifact
-        if artifact is None:
+        if (artifact is None) or (not artifact.updated):
             return
-        filename = artifact.dst_filename
-        if filename in self.processed:
-            return
-        dst_file = Path(filename)
+        dst_file = Path(artifact.dst_filename)
         content = dst_file.read_text()
         tree = from_html(content)
         modified = False
         for pattern, lang in self.patterns:
             nodes = tree.xpath(f"""//body//*[re:test(text(), '{pattern}')]""",
                                namespaces=_NAMESPACES)
             if len(nodes) > 0:
@@ -76,11 +72,10 @@
                         node.remove(child)
                     node.text = new_node.text
                     for child in new_node:
                         node.append(child)
                 modified = True
         if modified:
             dst_file.write_text(to_html(tree))
-        self.processed.add(filename)
 
     def on_after_build_all(self, builder, **extra):
         reporter.report_generic("Finished setting fixed languages")
```

### Comparing `lektor_fixedlang-0.4/pyproject.toml` & `lektor_fixedlang-0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lektor-fixedlang"
-version = "0.4"
+version = "0.5"
 description = "Set fixed languages for patterns in Lektor."
 readme = "README.rst"
 
 authors = [{name = "H. Turgut Uyar", email = "uyar@tekir.org"}]
 license = {file = "LICENSE.txt"}
 
 keywords = ["lektor", "plugin"]
```

### Comparing `lektor_fixedlang-0.4/tests/test_fixedlang.py` & `lektor_fixedlang-0.5/tests/test_fixedlang.py`

 * *Files identical despite different names*

