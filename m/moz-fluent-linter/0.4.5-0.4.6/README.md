# Comparing `tmp/moz-fluent-linter-0.4.5.tar.gz` & `tmp/moz_fluent_linter-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moz-fluent-linter-0.4.5.tar", last modified: Sat Oct 14 07:41:45 2023, max compression
+gzip compressed data, was "moz_fluent_linter-0.4.6.tar", last modified: Fri May  3 06:38:09 2024, max compression
```

## Comparing `moz-fluent-linter-0.4.5.tar` & `moz_fluent_linter-0.4.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2023-10-14 07:41:45.213562 moz-fluent-linter-0.4.5/
--rw-r--r--   0 flodolo    (502) staff       (20)    16725 2022-08-24 16:27:23.000000 moz-fluent-linter-0.4.5/LICENSE.md
--rw-r--r--   0 flodolo    (502) staff       (20)     2121 2023-10-14 07:41:45.213506 moz-fluent-linter-0.4.5/PKG-INFO
--rw-r--r--   0 flodolo    (502) staff       (20)     1290 2023-10-14 07:41:13.000000 moz-fluent-linter-0.4.5/README.md
--rw-r--r--   0 flodolo    (502) staff       (20)       85 2022-06-29 13:14:02.000000 moz-fluent-linter-0.4.5/pyproject.toml
--rw-r--r--   0 flodolo    (502) staff       (20)      988 2023-10-14 07:41:45.213844 moz-fluent-linter-0.4.5/setup.cfg
--rw-r--r--   0 flodolo    (502) staff       (20)       69 2022-06-29 13:14:02.000000 moz-fluent-linter-0.4.5/setup.py
-drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2023-10-14 07:41:45.210547 moz-fluent-linter-0.4.5/src/
-drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2023-10-14 07:41:45.211447 moz-fluent-linter-0.4.5/src/fluent_linter/
--rw-r--r--   0 flodolo    (502) staff       (20)       18 2023-10-14 07:41:23.000000 moz-fluent-linter-0.4.5/src/fluent_linter/__init__.py
--rw-r--r--   0 flodolo    (502) staff       (20)    24969 2023-10-14 07:40:54.000000 moz-fluent-linter-0.4.5/src/fluent_linter/linter.py
-drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2023-10-14 07:41:45.212139 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/
--rw-r--r--   0 flodolo    (502) staff       (20)     2121 2023-10-14 07:41:45.000000 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/PKG-INFO
--rw-r--r--   0 flodolo    (502) staff       (20)      582 2023-10-14 07:41:45.000000 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/SOURCES.txt
--rw-r--r--   0 flodolo    (502) staff       (20)        1 2023-10-14 07:41:45.000000 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/dependency_links.txt
--rw-r--r--   0 flodolo    (502) staff       (20)       62 2023-10-14 07:41:45.000000 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/entry_points.txt
--rw-r--r--   0 flodolo    (502) staff       (20)       39 2023-10-14 07:41:45.000000 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/requires.txt
--rw-r--r--   0 flodolo    (502) staff       (20)       14 2023-10-14 07:41:45.000000 moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/top_level.txt
-drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2023-10-14 07:41:45.213287 moz-fluent-linter-0.4.5/tests/
--rw-r--r--   0 flodolo    (502) staff       (20)     1981 2022-07-26 16:25:04.000000 moz-fluent-linter-0.4.5/tests/test_banned_words.py
--rw-r--r--   0 flodolo    (502) staff       (20)     2575 2022-11-22 09:25:46.000000 moz-fluent-linter-0.4.5/tests/test_brands.py
--rw-r--r--   0 flodolo    (502) staff       (20)     3273 2022-06-29 13:14:02.000000 moz-fluent-linter-0.4.5/tests/test_comments.py
--rw-r--r--   0 flodolo    (502) staff       (20)     3104 2023-01-26 12:24:24.000000 moz-fluent-linter-0.4.5/tests/test_comments_variables.py
--rw-r--r--   0 flodolo    (502) staff       (20)     1866 2022-07-26 12:13:29.000000 moz-fluent-linter-0.4.5/tests/test_ids.py
--rw-r--r--   0 flodolo    (502) staff       (20)     2091 2023-03-15 14:54:31.000000 moz-fluent-linter-0.4.5/tests/test_placeable_style.py
--rw-r--r--   0 flodolo    (502) staff       (20)     1905 2023-01-25 13:11:12.000000 moz-fluent-linter-0.4.5/tests/test_syntax.py
--rw-r--r--   0 flodolo    (502) staff       (20)     3358 2022-07-26 12:13:29.000000 moz-fluent-linter-0.4.5/tests/test_typography.py
+drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2024-05-03 06:38:09.112327 moz_fluent_linter-0.4.6/
+-rw-r--r--   0 flodolo    (502) staff       (20)    16725 2022-08-24 16:27:23.000000 moz_fluent_linter-0.4.6/LICENSE
+-rw-r--r--   0 flodolo    (502) staff       (20)     2118 2024-05-03 06:38:09.112262 moz_fluent_linter-0.4.6/PKG-INFO
+-rw-r--r--   0 flodolo    (502) staff       (20)     1290 2024-05-03 06:36:35.000000 moz_fluent_linter-0.4.6/README.md
+-rw-r--r--   0 flodolo    (502) staff       (20)       85 2022-06-29 13:14:02.000000 moz_fluent_linter-0.4.6/pyproject.toml
+-rw-r--r--   0 flodolo    (502) staff       (20)      988 2024-05-03 06:38:09.112571 moz_fluent_linter-0.4.6/setup.cfg
+-rw-r--r--   0 flodolo    (502) staff       (20)       69 2022-06-29 13:14:02.000000 moz_fluent_linter-0.4.6/setup.py
+drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2024-05-03 06:38:09.109207 moz_fluent_linter-0.4.6/src/
+drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2024-05-03 06:38:09.110134 moz_fluent_linter-0.4.6/src/fluent_linter/
+-rw-r--r--   0 flodolo    (502) staff       (20)       18 2024-05-03 06:36:45.000000 moz_fluent_linter-0.4.6/src/fluent_linter/__init__.py
+-rw-r--r--   0 flodolo    (502) staff       (20)    25204 2024-05-03 06:22:15.000000 moz_fluent_linter-0.4.6/src/fluent_linter/linter.py
+drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2024-05-03 06:38:09.112062 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/
+-rw-r--r--   0 flodolo    (502) staff       (20)     2118 2024-05-03 06:38:09.000000 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/PKG-INFO
+-rw-r--r--   0 flodolo    (502) staff       (20)      579 2024-05-03 06:38:09.000000 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/SOURCES.txt
+-rw-r--r--   0 flodolo    (502) staff       (20)        1 2024-05-03 06:38:09.000000 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/dependency_links.txt
+-rw-r--r--   0 flodolo    (502) staff       (20)       62 2024-05-03 06:38:09.000000 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/entry_points.txt
+-rw-r--r--   0 flodolo    (502) staff       (20)       39 2024-05-03 06:38:09.000000 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/requires.txt
+-rw-r--r--   0 flodolo    (502) staff       (20)       14 2024-05-03 06:38:09.000000 moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/top_level.txt
+drwxr-xr-x   0 flodolo    (502) staff       (20)        0 2024-05-03 06:38:09.111895 moz_fluent_linter-0.4.6/tests/
+-rw-r--r--   0 flodolo    (502) staff       (20)     1981 2022-07-26 16:25:04.000000 moz_fluent_linter-0.4.6/tests/test_banned_words.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     2854 2024-05-03 06:23:59.000000 moz_fluent_linter-0.4.6/tests/test_brands.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     3273 2022-06-29 13:14:02.000000 moz_fluent_linter-0.4.6/tests/test_comments.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     3104 2023-01-26 12:24:24.000000 moz_fluent_linter-0.4.6/tests/test_comments_variables.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     1866 2022-07-26 12:13:29.000000 moz_fluent_linter-0.4.6/tests/test_ids.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     2091 2023-03-15 14:54:31.000000 moz_fluent_linter-0.4.6/tests/test_placeable_style.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     1905 2023-01-25 13:11:12.000000 moz_fluent_linter-0.4.6/tests/test_syntax.py
+-rw-r--r--   0 flodolo    (502) staff       (20)     3358 2022-07-26 12:13:29.000000 moz_fluent_linter-0.4.6/tests/test_typography.py
```

### Comparing `moz-fluent-linter-0.4.5/LICENSE.md` & `moz_fluent_linter-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/PKG-INFO` & `moz_fluent_linter-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: moz-fluent-linter
-Version: 0.4.5
+Version: 0.4.6
 Summary: Linter package used to check Fluent files
 Home-page: https://github.com/mozilla-l10n/moz-fluent-linter
 Author: Francesco Lodolo
 Author-email: flod@mozilla.com
 Project-URL: Bug Tracker, https://github.com/mozilla-l10n/moz-fluent-linter/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Localization
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+License-File: LICENSE
 Requires-Dist: fluent.syntax<0.19,>=0.18.0
 Requires-Dist: pyyaml
 Requires-Dist: six
 
 # Fluent Linter
 
 [![PyPI version](https://badge.fury.io/py/moz-fluent-linter.svg)](https://badge.fury.io/py/moz-fluent-linter)
@@ -37,15 +37,15 @@
 ## Version control integration
 
 Using [pre-commit](https://pre-commit.com/), add this to the `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/mozilla-l10n/moz-fluent-linter
-    rev: v0.4.5
+    rev: v0.4.6
     hooks:
       - id: fluent_linter
         files: \.ftl$
         args: [--config, l10n/linter_config.yml, l10n/en/]
 ```
 
 This is just an example to get you started, you may need to update the `rev` and `args` depending on your specific needs and configuration.
```

### Comparing `moz-fluent-linter-0.4.5/README.md` & `moz_fluent_linter-0.4.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ## Version control integration
 
 Using [pre-commit](https://pre-commit.com/), add this to the `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/mozilla-l10n/moz-fluent-linter
-    rev: v0.4.5
+    rev: v0.4.6
     hooks:
       - id: fluent_linter
         files: \.ftl$
         args: [--config, l10n/linter_config.yml, l10n/en/]
 ```
 
 This is just an example to get you started, you may need to update the `rev` and `args` depending on your specific needs and configuration.
```

### Comparing `moz-fluent-linter-0.4.5/setup.cfg` & `moz_fluent_linter-0.4.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = moz-fluent-linter
-version = 0.4.5
+version = 0.4.6
 author = Francesco Lodolo
 author_email = flod@mozilla.com
 description = Linter package used to check Fluent files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mozilla-l10n/moz-fluent-linter
 project_urls =
```

### Comparing `moz-fluent-linter-0.4.5/src/fluent_linter/linter.py` & `moz_fluent_linter-0.4.6/src/fluent_linter/linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,57 +132,81 @@
         parts.append("\n")
 
         # Analyze message for issues with quotes, after removing HTML markup
         html_stripper = MLStripper()
         html_stripper.feed("".join(parts))
         cleaned_str = html_stripper.get_data()
 
+        message_id = node.id.name
+
+        # Check brand names here, so it's possible to also look for combination
+        # of text and terms.
+        if message_id is not None and not self.exclude_message(
+            "CO01", message_id, self.path
+        ):
+            found_brands = []
+            for brand in self.brand_names:
+                if brand == re.escape(brand):
+                    brand_re = re.compile(r"\b" + brand + r"\b")
+                else:
+                    brand_re = re.compile(brand)
+                if brand_re.search(cleaned_str):
+                    found_brands.append(brand)
+            if found_brands:
+                self.add_error(
+                    node,
+                    message_id,
+                    "CO01",
+                    "Strings should use the corresponding terms instead of"
+                    f" hard-coded brand names ({', '.join(found_brands)})",
+                )
+
         if self.apostrophe_re.search(cleaned_str):
-            if not self.exclude_message("TE01", node.id.name):
+            if not self.exclude_message("TE01", message_id):
                 self.add_error(
                     node,
-                    node.id.name,
+                    message_id,
                     "TE01",
                     "Strings with apostrophes should use foo\u2019s instead of foo's.",
                 )
         if self.incorrect_apostrophe_re.search(cleaned_str):
-            if not self.exclude_message("TE02", node.id.name):
+            if not self.exclude_message("TE02", message_id):
                 self.add_error(
                     node,
-                    node.id.name,
+                    message_id,
                     "TE02",
                     "Strings with apostrophes should use foo\u2019s instead of foo\u2018s.",
                 )
         if self.single_quote_re.search(cleaned_str):
-            if not self.exclude_message("TE03", node.id.name):
+            if not self.exclude_message("TE03", message_id):
                 self.add_error(
                     node,
-                    node.id.name,
+                    message_id,
                     "TE03",
                     "Single-quoted strings should use Unicode \u2018foo\u2019 instead of 'foo'.",
                 )
         if self.double_quote_re.search(cleaned_str):
             # Ignore parameterized terms and other functions
             for regex in self.ftl_syntax_re:
                 cleaned_str = regex.sub("", cleaned_str)
 
             if self.double_quote_re.search(cleaned_str) and not self.exclude_message(
-                "TE04", node.id.name
+                "TE04", message_id
             ):
                 self.add_error(
                     node,
-                    node.id.name,
+                    message_id,
                     "TE04",
                     'Double-quoted strings should use Unicode \u201cfoo\u201d instead of "foo".',
                 )
         if self.ellipsis_re.search(cleaned_str):
-            if not self.exclude_message("TE05", node.id.name):
+            if not self.exclude_message("TE05", message_id):
                 self.add_error(
                     node,
-                    node.id.name,
+                    message_id,
                     "TE05",
                     "Strings with an ellipsis should use the Unicode \u2026 character"
                     " instead of three periods",
                 )
 
     def generic_visit(self, node):
         node_name = type(node).__name__
@@ -294,34 +318,17 @@
         self.state["variables"] = []
 
     def visit_TextElement(self, node):
         html_stripper = MLStripper()
         html_stripper.feed(node.value)
         cleaned_str = html_stripper.get_data()
 
-        # If part of a message, check for brand and banned words
+        # If part of a message, check for banned words
         message_id = self.last_message_id
         if message_id is not None and not self.exclude_message(
-            "CO01", message_id, self.path
-        ):
-            found_brands = []
-            for brand in self.brand_names:
-                brand_re = re.compile(r"\b" + brand + r"\b")
-                if brand_re.search(cleaned_str):
-                    found_brands.append(brand)
-            if found_brands:
-                self.add_error(
-                    node,
-                    message_id,
-                    "CO01",
-                    "Strings should use the corresponding terms instead of"
-                    f" hard-coded brand names ({', '.join(found_brands)})",
-                )
-
-        if message_id is not None and not self.exclude_message(
             "CO02", message_id, self.path
         ):
             found_banned_words = []
             for word in self.banned_words:
                 bannedword_re = re.compile(r"\b" + word + r"\b")
                 if bannedword_re.search(cleaned_str.lower()):
                     found_banned_words.append(word)
```

### Comparing `moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/PKG-INFO` & `moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: moz-fluent-linter
-Version: 0.4.5
+Version: 0.4.6
 Summary: Linter package used to check Fluent files
 Home-page: https://github.com/mozilla-l10n/moz-fluent-linter
 Author: Francesco Lodolo
 Author-email: flod@mozilla.com
 Project-URL: Bug Tracker, https://github.com/mozilla-l10n/moz-fluent-linter/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Localization
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+License-File: LICENSE
 Requires-Dist: fluent.syntax<0.19,>=0.18.0
 Requires-Dist: pyyaml
 Requires-Dist: six
 
 # Fluent Linter
 
 [![PyPI version](https://badge.fury.io/py/moz-fluent-linter.svg)](https://badge.fury.io/py/moz-fluent-linter)
@@ -37,15 +37,15 @@
 ## Version control integration
 
 Using [pre-commit](https://pre-commit.com/), add this to the `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/mozilla-l10n/moz-fluent-linter
-    rev: v0.4.5
+    rev: v0.4.6
     hooks:
       - id: fluent_linter
         files: \.ftl$
         args: [--config, l10n/linter_config.yml, l10n/en/]
 ```
 
 This is just an example to get you started, you may need to update the `rev` and `args` depending on your specific needs and configuration.
```

### Comparing `moz-fluent-linter-0.4.5/src/moz_fluent_linter.egg-info/SOURCES.txt` & `moz_fluent_linter-0.4.6/src/moz_fluent_linter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.md
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/fluent_linter/__init__.py
 src/fluent_linter/linter.py
 src/moz_fluent_linter.egg-info/PKG-INFO
```

### Comparing `moz-fluent-linter-0.4.5/tests/test_banned_words.py` & `moz_fluent_linter-0.4.6/tests/test_banned_words.py`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/tests/test_brands.py` & `moz_fluent_linter-0.4.6/tests/test_brands.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,40 +32,45 @@
 
 good-mozilla1 = Welcome to { -brand-mozilla }
 good-mozilla2 = Welcome to { mozilla-message }
 
 bad-monitor = Monitor your email
 good-monitor = Monitored emails
 good-monitor2 = Set up your monitor.
+
+bad-account = Set up your { -brand-short-name } account
+good-account = Set up your { -brand-short-name }. Account.
+good-account2 = Set up your { -brand-short-name } Account.
 """
 
         config = {
             "CO01": {
                 "enabled": False,
             }
         }
         results = self.checkContent(config, content)
         self.assertEqual(len(results), 0)
 
         config = {
             "CO01": {
                 "enabled": True,
-                "brands": ["Firefox", "Mozilla"],
+                "brands": ["Firefox", "Mozilla", "{ -brand-short-name } account"],
                 "exclusions": {
                     "messages": ["bad-firefox-excluded"],
                 },
             }
         }
         results = self.checkContent(config, content)
-        self.assertEqual(len(results), 8)
+        self.assertEqual(len(results), 9)
         self.assertTrue("CO01" in results[0])
         self.assertTrue("Firefox" in results[0])
-        self.assertTrue("line 5" in results[1])
+        self.assertTrue("line 4" in results[1])
         self.assertTrue("bad-firefox2" in results[1])
         self.assertTrue("Mozilla" in results[5])
+        self.assertTrue("{ -brand-short-name } account" in results[8])
 
         config = {
             "CO01": {
                 "enabled": True,
                 "brands": ["Firefox", "Mozilla"],
                 "exclusions": {
                     "files": ["file.ftl"],
```

### Comparing `moz-fluent-linter-0.4.5/tests/test_comments.py` & `moz_fluent_linter-0.4.6/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/tests/test_comments_variables.py` & `moz_fluent_linter-0.4.6/tests/test_comments_variables.py`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/tests/test_ids.py` & `moz_fluent_linter-0.4.6/tests/test_ids.py`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/tests/test_placeable_style.py` & `moz_fluent_linter-0.4.6/tests/test_placeable_style.py`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/tests/test_syntax.py` & `moz_fluent_linter-0.4.6/tests/test_syntax.py`

 * *Files identical despite different names*

### Comparing `moz-fluent-linter-0.4.5/tests/test_typography.py` & `moz_fluent_linter-0.4.6/tests/test_typography.py`

 * *Files identical despite different names*

