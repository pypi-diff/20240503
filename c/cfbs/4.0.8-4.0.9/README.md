# Comparing `tmp/cfbs-4.0.8.tar.gz` & `tmp/cfbs-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfbs-4.0.8.tar", last modified: Fri Feb  2 15:56:13 2024, max compression
+gzip compressed data, was "cfbs-4.0.9.tar", last modified: Fri May  3 15:29:45 2024, max compression
```

## Comparing `cfbs-4.0.8.tar` & `cfbs-4.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:56:13.077692 cfbs-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-02 15:56:04.000000 cfbs-4.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-02-02 15:56:13.077692 cfbs-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-02-02 15:56:04.000000 cfbs-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:56:13.077692 cfbs-4.0.8/cfbs/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-02 15:56:12.000000 cfbs-4.0.8/cfbs/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      288 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    18928 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/cfbs_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/cfbs_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    40245 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/git_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/internal_file_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-02 15:56:04.000000 cfbs-4.0.8/cfbs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:56:13.077692 cfbs-4.0.8/cfbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-02-02 15:56:13.000000 cfbs-4.0.8/cfbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-02 15:56:13.000000 cfbs-4.0.8/cfbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:56:13.000000 cfbs-4.0.8/cfbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-02 15:56:13.000000 cfbs-4.0.8/cfbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-02 15:56:13.000000 cfbs-4.0.8/cfbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 15:56:13.077692 cfbs-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-02 15:56:04.000000 cfbs-4.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:56:13.077692 cfbs-4.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_validate_index_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_validate_mock_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-02-02 15:56:04.000000 cfbs-4.0.8/tests/test_validate_mock_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.281458 cfbs-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 15:29:37.000000 cfbs-4.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-03 15:29:45.281458 cfbs-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-05-03 15:29:37.000000 cfbs-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.277458 cfbs-4.0.9/cfbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      288 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18928 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/cfbs_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/cfbs_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40229 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/git_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/internal_file_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-03 15:29:37.000000 cfbs-4.0.9/cfbs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.281458 cfbs-4.0.9/cfbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 15:29:45.000000 cfbs-4.0.9/cfbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:29:45.281458 cfbs-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-03 15:29:37.000000 cfbs-4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:29:45.281458 cfbs-4.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_validate_index_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_validate_mock_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-03 15:29:37.000000 cfbs-4.0.9/tests/test_validate_mock_input.py
```

### Comparing `cfbs-4.0.8/LICENSE` & `cfbs-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/PKG-INFO` & `cfbs-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbs
-Version: 4.0.8
+Version: 4.0.9
 Summary: Tooling to build, manage and deploy CFEngine policy
 Home-page: https://github.com/cfengine/cfbs
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfbs-4.0.8/README.md` & `cfbs-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/args.py` & `cfbs-4.0.9/cfbs/args.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/build.py` & `cfbs-4.0.9/cfbs/build.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/cfbs_config.py` & `cfbs-4.0.9/cfbs/cfbs_config.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/cfbs_json.py` & `cfbs-4.0.9/cfbs/cfbs_json.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/commands.py` & `cfbs-4.0.9/cfbs/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,14 @@
             ):
                 print("Failed to set Git user name and email")
                 return 1
 
     config["git"] = do_git
 
     data = pretty(config, CFBS_DEFAULT_SORTING_RULES) + "\n"
-    print(data)
     with open(cfbs_filename(), "w") as f:
         f.write(data)
     assert is_cfbs_repo()
 
     if do_git:
         try:
             git_commit_maybe_prompt(
```

### Comparing `cfbs-4.0.8/cfbs/git.py` & `cfbs-4.0.9/cfbs/git.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/git_magic.py` & `cfbs-4.0.9/cfbs/git_magic.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/index.py` & `cfbs-4.0.9/cfbs/index.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/internal_file_management.py` & `cfbs-4.0.9/cfbs/internal_file_management.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/main.py` & `cfbs-4.0.9/cfbs/main.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/module.py` & `cfbs-4.0.9/cfbs/module.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/pretty.py` & `cfbs-4.0.9/cfbs/pretty.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,32 +215,33 @@
 def pretty(o, sorting_rules=None):
     MAX_LEN = 80
     INDENT_SIZE = 2
 
     if sorting_rules is not None:
         _children_sort(o, None, sorting_rules)
 
-    def _should_wrap(parent):
+    def _should_wrap(parent, indent):
         assert isinstance(parent, (tuple, list, dict))
-
+        # We should wrap the top level collection
+        if indent == 0:
+            return True
         if isinstance(parent, dict):
             parent = parent.values()
 
         count = 0
         for child in parent:
             if isinstance(child, (tuple, list, dict)):
                 if len(child) >= 2:
                     count += 1
         return count >= 2
 
     def _encode_list(lst, indent, cursor):
         if not lst:
             return "[]"
-
-        if not _should_wrap(lst):
+        if not _should_wrap(lst, indent):
             buf = json.dumps(lst)
             assert "\n" not in buf
             if indent + cursor + len(buf) <= MAX_LEN:
                 return buf
 
         indent += INDENT_SIZE
         buf = "[\n" + " " * indent
@@ -255,16 +256,15 @@
         buf += "\n" + " " * indent + "]"
 
         return buf
 
     def _encode_dict(dct, indent, cursor):
         if not dct:
             return "{}"
-
-        if not _should_wrap(dct):
+        if not _should_wrap(dct, indent):
             buf = json.dumps(dct)
             buf = "{ " + buf[1 : len(buf) - 1] + " }"
             assert "\n" not in buf
             if indent + cursor + len(buf) <= MAX_LEN:
                 return buf
 
         indent += INDENT_SIZE
```

### Comparing `cfbs-4.0.8/cfbs/prompts.py` & `cfbs-4.0.9/cfbs/prompts.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/utils.py` & `cfbs-4.0.9/cfbs/utils.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs/validate.py` & `cfbs-4.0.9/cfbs/validate.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/cfbs.egg-info/PKG-INFO` & `cfbs-4.0.9/cfbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfbs
-Version: 4.0.8
+Version: 4.0.9
 Summary: Tooling to build, manage and deploy CFEngine policy
 Home-page: https://github.com/cfengine/cfbs
 Author: Northern.tech, Inc.
 Author-email: contact@northern.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfbs-4.0.8/cfbs.egg-info/SOURCES.txt` & `cfbs-4.0.9/cfbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/setup.py` & `cfbs-4.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/tests/test_input.py` & `cfbs-4.0.9/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/tests/test_module.py` & `cfbs-4.0.9/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/tests/test_pretty.py` & `cfbs-4.0.9/tests/test_pretty.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,40 +9,64 @@
     assert pretty(True) == "true"
     assert pretty(False) == "false"
     assert pretty(123) == "123"
     assert pretty(123.456) == "123.456"
     assert pretty("Hello World!") == '"Hello World!"'
 
     # Test collections
-    assert pretty([]) == "[]"
+    assert pretty([]) == ("[]")
     assert pretty(()) == "[]"
     assert pretty({}) == "{}"
 
     test = OrderedDict()
     test["a"] = []
     test["b"] = ()
-    expected = '{ "a": [], "b": [] }'
+    expected = """{
+  "a": [],
+  "b": []
+}"""
     assert pretty(test) == expected
 
     test = [None, True, False, 1, 1.2, "Hello!"]
-    expected = '[null, true, false, 1, 1.2, "Hello!"]'
+    expected = """[
+  null,
+  true,
+  false,
+  1,
+  1.2,
+  "Hello!"
+]"""
     assert pretty(test) == expected
 
     test = (None, True, False, 1, 1.2, "Hello!")
-    expected = '[null, true, false, 1, 1.2, "Hello!"]'
+    expected = """[
+  null,
+  true,
+  false,
+  1,
+  1.2,
+  "Hello!"
+]"""
     assert pretty(test) == expected
 
     test = OrderedDict()
     test["a"] = None
     test["b"] = True
     test["c"] = False
     test["d"] = 1
     test["e"] = 1.2
     test["f"] = "Hello!"
-    expected = '{ "a": null, "b": true, "c": false, "d": 1, "e": 1.2, "f": "Hello!" }'
+    expected = """{
+  "a": null,
+  "b": true,
+  "c": false,
+  "d": 1,
+  "e": 1.2,
+  "f": "Hello!"
+}"""
     assert pretty(test) == expected
 
     # Test that strings are escaped correctly:
 
     test = ""  # Empty string
     expected = '""'  # is represented as "" in JSON, same as python
     assert pretty(test) == expected
@@ -70,54 +94,51 @@
     assert pretty_string('"Hello World!"') == '"Hello World!"'
 
     # Test collections
     assert pretty_string("[]") == "[]"
     assert pretty_string("{}") == "{}"
 
     test = '[null, true, false, 1, 1.2, "Hello!"]'
-    expected = '[null, true, false, 1, 1.2, "Hello!"]'
+    expected = """[
+  null,
+  true,
+  false,
+  1,
+  1.2,
+  "Hello!"
+]"""
     assert pretty_string(test) == expected
 
     test = '{ "a": null, "b": true, "c": false, "d": 1, "e": 1.2, "f": "Hello!" }'
-    expected = '{ "a": null, "b": true, "c": false, "d": 1, "e": 1.2, "f": "Hello!" }'
-    assert pretty_string(test) == expected
-
-    # Test wrapping on dicts based on length
-    test = '{ "This": "line", "is": "less", "than": 80, "characters": "don\'t wrap me..." }'
-    expected = '{ "This": "line", "is": "less", "than": 80, "characters": "don\'t wrap me..." }'
-    assert pretty_string(test) == expected
+    expected = """{
+  "a": null,
+  "b": true,
+  "c": false,
+  "d": 1,
+  "e": 1.2,
+  "f": "Hello!"
+}"""
 
-    test = '{ "This": "line", "is": "equal", "to": 80, "characters": "dont\'t wrap me...." }'
-    expected = '{ "This": "line", "is": "equal", "to": 80, "characters": "dont\'t wrap me...." }'
     assert pretty_string(test) == expected
 
-    test = '{ "This": "line", "is": "greater", "than": 80, "characters": "wrap me ........" }'
+    test = '{ "This": "line", "is": "equal", "to": 80, "characters": "wrap me anyway" }'
     expected = """{
   "This": "line",
-  "is": "greater",
-  "than": 80,
-  "characters": "wrap me ........"
+  "is": "equal",
+  "to": 80,
+  "characters": "wrap me anyway"
 }"""
     assert pretty_string(test) == expected
 
-    # Test wrapping on lists based on length
-    test = '["This", "line", "is", "less", "than", 80, "characters", "don\'t wrap me", "."]'
-    expected = '["This", "line", "is", "less", "than", 80, "characters", "don\'t wrap me", "."]'
-    assert pretty_string(test) == expected
-
-    test = '["This", "line", "is", "less", "than", 80, "characters", "don\'t wrap me", ".."]'
-    expected = '["This", "line", "is", "less", "than", 80, "characters", "don\'t wrap me", ".."]'
-    assert pretty_string(test) == expected
-
-    test = '["This", "line", "is", "less", "than", 80, "characters", "wrap me", ".........."]'
+    test = '["This", "line", "is", "more", "than", 80, "characters", "wrap me", ".........."]'
     expected = """[
   "This",
   "line",
   "is",
-  "less",
+  "more",
   "than",
   80,
   "characters",
   "wrap me",
   ".........."
 ]"""
     assert pretty_string(test) == expected
@@ -190,94 +211,167 @@
     assert (
         pretty_check_string(
             """{
   "name": "lars",
   "age": 27
 }"""
         )
-        == False
+        == True
     )
-    assert pretty_check_string('{ "name": "lars", "age": 27 }') == True
+    assert pretty_check_string('{ "name": "lars", "age": 27 }') == False
 
 
 def test_pretty_sorting_simple_top_level():
     """Show that simple ways of sorting top level keys work"""
 
     lex_sorting = {
         None: (
             "alphabetic",  # Sort keys lexically / alphabetically
             None,
         ),
     }
     assert pretty_string("""{}""", lex_sorting) == """{}"""
-    assert pretty_string("""{"a":1}""", lex_sorting) == """{ "a": 1 }"""
-    assert pretty_string("""{"b":2,"a":1}""", lex_sorting) == """{ "a": 1, "b": 2 }"""
+    assert (
+        pretty_string("""{"a":1}""", lex_sorting)
+        == """{
+  "a": 1
+}"""
+    )
+
+    assert (
+        pretty_string("""{"b":2,"a":1}""", lex_sorting)
+        == """{
+  "a": 1,
+  "b": 2
+}"""
+    )
+
     assert (
         pretty_string("""{"b":2,"a":1,"c":3}""", lex_sorting)
-        == """{ "a": 1, "b": 2, "c": 3 }"""
+        == """{
+  "a": 1,
+  "b": 2,
+  "c": 3
+}"""
     )
 
     length_sorting = {
         None: (
             lambda x: len(x[0]),  # Sort by the length of the key
             None,
         ),
     }
 
     assert pretty_string("""{}""", length_sorting) == """{}"""
-    assert pretty_string("""{"aa":1}""", length_sorting) == """{ "aa": 1 }"""
+    assert (
+        pretty_string("""{"aa":1}""", length_sorting)
+        == """{
+  "aa": 1
+}"""
+    )
+
     assert (
         pretty_string("""{"bbb":2,"aa":1}""", length_sorting)
-        == """{ "aa": 1, "bbb": 2 }"""
+        == """{
+  "aa": 1,
+  "bbb": 2
+}"""
     )
+
     assert (
         pretty_string("""{"bbb":2,"aa":1,"c":3}""", length_sorting)
-        == """{ "c": 3, "aa": 1, "bbb": 2 }"""
+        == """{
+  "c": 3,
+  "aa": 1,
+  "bbb": 2
+}"""
     )
 
     integer_sorting = {
         None: (
             lambda x: x[1],  # Sort by the value (integer)
             None,
         ),
     }
 
     assert pretty_string("""{}""", integer_sorting) == """{}"""
-    assert pretty_string("""{"a":1}""", integer_sorting) == """{ "a": 1 }"""
     assert (
-        pretty_string("""{"b":2,"a":1}""", integer_sorting) == """{ "a": 1, "b": 2 }"""
+        pretty_string("""{"a":1}""", integer_sorting)
+        == """{
+  "a": 1
+}"""
+    )
+
+    assert (
+        pretty_string("""{"b":2,"a":1}""", integer_sorting)
+        == """{
+  "a": 1,
+  "b": 2
+}"""
     )
+
     assert (
         pretty_string("""{"b":2,"a":1,"c":3}""", integer_sorting)
-        == """{ "a": 1, "b": 2, "c": 3 }"""
+        == """{
+  "a": 1,
+  "b": 2,
+  "c": 3
+}"""
     )
+
     assert (
         pretty_string("""{"b":2,"a":1,"c":3,"z":-1}""", integer_sorting)
-        == """{ "z": -1, "a": 1, "b": 2, "c": 3 }"""
+        == """{
+  "z": -1,
+  "a": 1,
+  "b": 2,
+  "c": 3
+}"""
     )
 
     specific_sorting = {
         None: (
             ["z", "b", "a", "c"],
             None,
         ),
     }
 
     assert pretty_string("""{}""", specific_sorting) == """{}"""
-    assert pretty_string("""{"a":1}""", specific_sorting) == """{ "a": 1 }"""
+
     assert (
-        pretty_string("""{"b":2,"a":1}""", specific_sorting) == """{ "b": 2, "a": 1 }"""
+        pretty_string("""{"a":1}""", specific_sorting)
+        == """{
+  "a": 1
+}"""
     )
+
+    assert (
+        pretty_string("""{"b":2,"a":1}""", specific_sorting)
+        == """{
+  "b": 2,
+  "a": 1
+}"""
+    )
+
     assert (
         pretty_string("""{"b":2,"a":1,"c":3}""", specific_sorting)
-        == """{ "b": 2, "a": 1, "c": 3 }"""
+        == """{
+  "b": 2,
+  "a": 1,
+  "c": 3
+}"""
     )
     assert (
         pretty_string("""{"b":2,"a":1,"c":3,"z":-1}""", specific_sorting)
-        == """{ "z": -1, "b": 2, "a": 1, "c": 3 }"""
+        == """{
+  "z": -1,
+  "b": 2,
+  "a": 1,
+  "c": 3
+}"""
     )
 
 
 def test_pretty_sorting_array():
     """Test that we can sort the keys inside objects in an array"""
     data = """{
         "yes":[{"a": 1, "b": 2, "c": 3}, {"a": 4, "c": 5, "b": 6}, {"b": 7, "c": 8, "a": 9}],
```

### Comparing `cfbs-4.0.8/tests/test_utils.py` & `cfbs-4.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/tests/test_validate_index_alias.py` & `cfbs-4.0.9/tests/test_validate_index_alias.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/tests/test_validate_mock_index.py` & `cfbs-4.0.9/tests/test_validate_mock_index.py`

 * *Files identical despite different names*

### Comparing `cfbs-4.0.8/tests/test_validate_mock_input.py` & `cfbs-4.0.9/tests/test_validate_mock_input.py`

 * *Files identical despite different names*

