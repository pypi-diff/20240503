# Comparing `tmp/btrview-0.6.1.tar.gz` & `tmp/btrview-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.6.1.tar", last modified: Wed May  1 16:04:38 2024, max compression
+gzip compressed data, was "btrview-0.6.2.tar", last modified: Fri May  3 19:17:20 2024, max compression
```

## Comparing `btrview-0.6.1.tar` & `btrview-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 16:04:38.791255 btrview-0.6.1/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.6.1/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     6165 2024-05-01 16:04:38.791255 btrview-0.6.1/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4284 2024-05-01 16:01:58.000000 btrview-0.6.1/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 16:04:38.791255 btrview-0.6.1/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       86 2024-05-01 16:04:32.000000 btrview-0.6.1/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.1/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3665 2024-04-18 01:10:40.000000 btrview-0.6.1/btrview/btr_dict.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7362 2024-04-18 03:01:25.000000 btrview-0.6.1/btrview/btrfs.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6934 2024-04-30 00:45:21.000000 btrview-0.6.1/btrview/rich_output.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5914 2024-04-18 01:10:40.000000 btrview-0.6.1/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.6.1/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-01 16:04:38.791255 btrview-0.6.1/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6165 2024-05-01 16:04:38.000000 btrview-0.6.1/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      361 2024-05-01 16:04:38.000000 btrview-0.6.1/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-01 16:04:38.000000 btrview-0.6.1/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-01 16:04:38.000000 btrview-0.6.1/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-01 16:04:38.000000 btrview-0.6.1/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-01 16:04:38.000000 btrview-0.6.1/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1070 2024-05-01 16:04:32.000000 btrview-0.6.1/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-01 16:04:38.791255 btrview-0.6.1/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 19:17:20.926136 btrview-0.6.2/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.6.2/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-03 19:17:20.926136 btrview-0.6.2/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4284 2024-05-03 19:16:33.000000 btrview-0.6.2/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 19:17:20.926136 btrview-0.6.2/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       86 2024-05-03 19:17:07.000000 btrview-0.6.2/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.2/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3665 2024-05-03 19:13:38.000000 btrview-0.6.2/btrview/btr_dict.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7362 2024-04-18 03:01:25.000000 btrview-0.6.2/btrview/btrfs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-03 19:13:42.000000 btrview-0.6.2/btrview/rich_output.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5914 2024-05-03 19:13:38.000000 btrview-0.6.2/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.6.2/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-03 19:17:20.926136 btrview-0.6.2/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      361 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-03 19:17:20.000000 btrview-0.6.2/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1197 2024-05-03 19:17:07.000000 btrview-0.6.2/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-03 19:17:20.926136 btrview-0.6.2/setup.cfg
```

### Comparing `btrview-0.6.1/LICENSE.md` & `btrview-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/PKG-INFO` & `btrview-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.6.1
+Version: 0.6.2
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Repository, https://github.com/CopOnTheRun/btrview
+Project-URL: Issues, https://github.com/CopOnTheRun/btrview/issues
 Keywords: btrfs
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `btrview-0.6.1/README.md` & `btrview-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/btrview/__main__.py` & `btrview-0.6.2/btrview/__main__.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/btrview/btr_dict.py` & `btrview-0.6.2/btrview/btr_dict.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/btrview/btrfs.py` & `btrview-0.6.2/btrview/btrfs.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/btrview/rich_output.py` & `btrview-0.6.2/btrview/rich_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,24 +111,24 @@
             styles.append(Style(color="grey58"))
 
         style = Style.combine(styles) if styles else ""
         return Text(rich_str, style)
 
 class RichTreeTable:
     """Class to piece together Filesystem and Subvolume trees into a cohesive display"""
-    default_table_stle = {"show_edge": False, "show_lines" : False, "expand" : True, "box" : None, "padding" : 0}
+    default_table_style = {"show_edge": False, "show_lines" : False, "box" : None, }
     def __init__(self, title: str,subvol_forest, snapshot_forest):
         self.title = title
         self.subvol_forest = subvol_forest
         self.snapshot_forest = snapshot_forest
 
     def create_rich_table(self, **kwargs) -> Table:
         """Creates a table from a subvolume forest and snapshot forest"""
         if not kwargs:
-            kwargs = self.default_table_stle
+            kwargs = self.default_table_style
         forest_table = Table(title = f"{self.title}", **kwargs)
         forest_table.add_column("Subvolume Tree:")
         forest_table.add_column("Snapshot Tree:")
         forest_table.add_row(self.subvol_forest,self.snapshot_forest)
         return forest_table
 
 def logic(labels: list[str], remove: tuple[str,...], prop: str,
```

### Comparing `btrview-0.6.1/btrview/subvolume.py` & `btrview-0.6.2/btrview/subvolume.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/btrview/utils.py` & `btrview-0.6.2/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.1/btrview.egg-info/PKG-INFO` & `btrview-0.6.2/btrview.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.6.1
+Version: 0.6.2
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Repository, https://github.com/CopOnTheRun/btrview
+Project-URL: Issues, https://github.com/CopOnTheRun/btrview/issues
 Keywords: btrfs
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `btrview-0.6.1/pyproject.toml` & `btrview-0.6.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.6.1"
+version = "0.6.2"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,20 +20,24 @@
 [project.optional-dependencies]
 build = ["build","twine"]
 dev = ["bumpver","mypy","pip-tools"]
 
 [project.scripts]
 btrview = "btrview.scripts.btrview:main"
 
+[project.urls]
+Repository = "https://github.com/CopOnTheRun/btrview"
+Issues = "https://github.com/CopOnTheRun/btrview/issues"
+
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.6.1"
+current_version = "0.6.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

