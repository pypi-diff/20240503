# Comparing `tmp/hbox-0.2.1.tar.gz` & `tmp/hbox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbox-0.2.1.tar", max compression
+gzip compressed data, was "hbox-0.2.2.tar", max compression
```

## Comparing `hbox-0.2.1.tar` & `hbox-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-03 05:14:25.705274 hbox-0.2.1/LICENSE
--rw-r--r--   0        0        0     6344 2024-05-03 05:14:25.705274 hbox-0.2.1/README.md
--rw-r--r--   0        0        0     6635 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/commands.py
--rw-r--r--   0        0        0     2212 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/config.py
--rw-r--r--   0        0        0      684 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/logger.py
--rw-r--r--   0        0        0     3094 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/main.py
--rw-r--r--   0        0        0     2292 2024-05-03 05:14:25.705274 hbox-0.2.1/hbox/utils.py
--rw-r--r--   0        0        0     1861 2024-05-03 05:14:46.761070 hbox-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-03 05:44:32.274102 hbox-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6344 2024-05-03 05:44:32.274102 hbox-0.2.2/README.md
+-rw-r--r--   0        0        0     6635 2024-05-03 05:44:32.274102 hbox-0.2.2/hbox/commands.py
+-rw-r--r--   0        0        0     2212 2024-05-03 05:44:32.274102 hbox-0.2.2/hbox/config.py
+-rw-r--r--   0        0        0      684 2024-05-03 05:44:32.274102 hbox-0.2.2/hbox/logger.py
+-rw-r--r--   0        0        0     3094 2024-05-03 05:44:32.274102 hbox-0.2.2/hbox/main.py
+-rw-r--r--   0        0        0     2292 2024-05-03 05:44:32.274102 hbox-0.2.2/hbox/utils.py
+-rw-r--r--   0        0        0     1963 2024-05-03 05:44:57.645801 hbox-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 hbox-0.2.2/PKG-INFO
```

### Comparing `hbox-0.2.1/LICENSE` & `hbox-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/README.md` & `hbox-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/hbox/commands.py` & `hbox-0.2.2/hbox/commands.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/hbox/config.py` & `hbox-0.2.2/hbox/config.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/hbox/logger.py` & `hbox-0.2.2/hbox/logger.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/hbox/main.py` & `hbox-0.2.2/hbox/main.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/hbox/utils.py` & `hbox-0.2.2/hbox/utils.py`

 * *Files identical despite different names*

### Comparing `hbox-0.2.1/pyproject.toml` & `hbox-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hbox"
-version = "0.2.1"
+version = "0.2.2"
 description = "CLI tool that leverages container technology to manage packages."
 authors = ["Helton Carlos de Souza <heltoncarlossouza@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
@@ -15,32 +15,35 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 assets = []
-commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
+commit_message = "chore: bump version to v{version} [skip ci]\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
 allow_zero_version = true
 tag_format = "v{version}"
 version_toml = ["pyproject.toml:tool.poetry.version"]
-build_command = "poetry build"
+build_command = "poetry build && pwd && ls -alho"
 
 [tool.semantic_release.branches.main]
 match = "(main)"
 prerelease_token = "rc"
 prerelease = false
 
 [tool.semantic_release.changelog]
 template_dir = "templates"
 changelog_file = "CHANGELOG.md"
-exclude_commit_patterns = []
+exclude_commit_patterns = [
+    "^Merge pull request",
+    "^Merge branch",
+]
 
 [tool.semantic_release.changelog.environment]
 block_start_string = "{%"
 block_end_string = "%}"
 variable_start_string = "{{"
 variable_end_string = "}}"
 comment_start_string = "{#"
```

### Comparing `hbox-0.2.1/PKG-INFO` & `hbox-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI tool that leverages container technology to manage packages.
 License: MIT
 Author: Helton Carlos de Souza
 Author-email: heltoncarlossouza@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

