# Comparing `tmp/subproptools-0.4.2.tar.gz` & `tmp/subproptools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subproptools-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "subproptools-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `subproptools-0.4.2.tar` & `subproptools-0.4.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1099 2024-04-10 19:06:06.566991 subproptools-0.4.2/LICENSE
--rw-r--r--   0        0        0     2579 2024-04-10 19:06:06.566991 subproptools-0.4.2/README.md
--rw-r--r--   0        0        0     2875 2024-04-10 19:06:06.574991 subproptools-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      548 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/__init__.py
--rw-r--r--   0        0        0     4519 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/deprecated.txt
--rw-r--r--   0        0        0    44124 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/qtaim_extract.py
--rw-r--r--   0        0        0    15792 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/reference_maps.py
--rw-r--r--   0        0        0    35254 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/sub_reor.py
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 subproptools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-05-03 19:47:56.429536 subproptools-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2579 2024-05-03 19:47:56.429536 subproptools-0.4.3/README.md
+-rw-r--r--   0        0        0     2875 2024-05-03 19:47:56.441536 subproptools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      548 2024-05-03 19:47:56.441536 subproptools-0.4.3/subproptools/__init__.py
+-rw-r--r--   0        0        0     4519 2024-05-03 19:47:56.445536 subproptools-0.4.3/subproptools/deprecated.txt
+-rw-r--r--   0        0        0    44119 2024-05-03 19:47:56.445536 subproptools-0.4.3/subproptools/qtaim_extract.py
+-rw-r--r--   0        0        0    15792 2024-05-03 19:47:56.445536 subproptools-0.4.3/subproptools/reference_maps.py
+-rw-r--r--   0        0        0    35254 2024-05-03 19:47:56.445536 subproptools-0.4.3/subproptools/sub_reor.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 subproptools-0.4.3/PKG-INFO
```

### Comparing `subproptools-0.4.2/LICENSE` & `subproptools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.2/README.md` & `subproptools-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.2/pyproject.toml` & `subproptools-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.2/subproptools/__init__.py` & `subproptools-0.4.3/subproptools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 .. _AIMAll:
     https://aim.tkgristmill.com/index.html
 
 .. _Mawhinney group:
     https://www.lakeheadu.ca/users/M/rmawhinn
 """
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
```

### Comparing `subproptools-0.4.2/subproptools/deprecated.txt` & `subproptools-0.4.3/subproptools/deprecated.txt`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.2/subproptools/qtaim_extract.py` & `subproptools-0.4.3/subproptools/qtaim_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,15 +759,15 @@
                     + groupDict["Mu_Bond_Z"][0] ** 2
                 )
             ]
         }
     )
     groupDict.update(
         {
-            "|Mu_Bond|": [
+            "|Mu|": [
                 math.sqrt(
                     groupDict["Mu_X"][0] ** 2
                     + groupDict["Mu_Y"][0] ** 2
                     + groupDict["Mu_Z"][0] ** 2
                 )
             ]
         }
```

### Comparing `subproptools-0.4.2/subproptools/reference_maps.py` & `subproptools-0.4.3/subproptools/reference_maps.py`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.2/subproptools/sub_reor.py` & `subproptools-0.4.3/subproptools/sub_reor.py`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.2/PKG-INFO` & `subproptools-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subproptools
-Version: 0.4.2
+Version: 0.4.3
 Summary: A plugin for extracting data from .sum files and manipuating them
 Keywords: qtaim,functional groups
 Author-email: Kevin Lefrancois-Gagnon <kgagnon@lakeheadu.ca>, Robert Mawhinney <mawhinn@lakeheadu.ca>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

