# Comparing `tmp/robotcode_modifiers-0.80.0.tar.gz` & `tmp/robotcode_modifiers-0.81.0.tar.gz`

## Comparing `robotcode_modifiers-0.80.0.tar` & `robotcode_modifiers-0.81.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/src/robotcode/modifiers/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/src/robotcode/modifiers/__version__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/src/robotcode/modifiers/longname_modifiers.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/src/robotcode/modifiers/py.typed
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/LICENSE.txt
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/README.md
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 robotcode_modifiers-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/src/robotcode/modifiers/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/src/robotcode/modifiers/__version__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/src/robotcode/modifiers/longname_modifiers.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/src/robotcode/modifiers/py.typed
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/LICENSE.txt
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 robotcode_modifiers-0.81.0/PKG-INFO
```

### Comparing `robotcode_modifiers-0.80.0/src/robotcode/modifiers/longname_modifiers.py` & `robotcode_modifiers-0.81.0/src/robotcode/modifiers/longname_modifiers.py`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.80.0/.gitignore` & `robotcode_modifiers-0.81.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.80.0/LICENSE.txt` & `robotcode_modifiers-0.81.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.80.0/README.md` & `robotcode_modifiers-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.80.0/pyproject.toml` & `robotcode_modifiers-0.81.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = ["robotframework>=4.1.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
-Donate = "https://github.com/sponsors/d-biehl"
+Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
 Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/robotcodedev/robotcode/issues"
 Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/modifiers/__version__.py"
```

### Comparing `robotcode_modifiers-0.80.0/PKG-INFO` & `robotcode_modifiers-0.81.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: robotcode-modifiers
-Version: 0.80.0
+Version: 0.81.0
 Summary: Some Robot Framework Modifiers for RobotCode
 Project-URL: Homepage, https://robotcode.io
-Project-URL: Donate, https://github.com/sponsors/d-biehl
+Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
 License: Apache-2.0
 License-File: LICENSE.txt
```

