# Comparing `tmp/dictrule-0.4.3.tar.gz` & `tmp/dictrule-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictrule-0.4.3.tar", last modified: Wed May  1 17:02:44 2024, max compression
+gzip compressed data, was "dictrule-0.4.4.tar", last modified: Fri May  3 17:12:09 2024, max compression
```

## Comparing `dictrule-0.4.3.tar` & `dictrule-0.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.837292 dictrule-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-01 17:02:38.000000 dictrule-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-01 17:02:44.837292 dictrule-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-01 17:02:38.000000 dictrule-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:02:44.837292 dictrule-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-01 17:02:38.000000 dictrule-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.829292 dictrule-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.833292 dictrule-0.4.3/src/dictrule/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.833292 dictrule-0.4.3/src/dictrule/built_in_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/comment_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/for_in_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/format_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/indent_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/inline_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/join_block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/join_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/built_in_rules/stringify_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/dr_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/eo_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/eval_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-01 17:02:38.000000 dictrule-0.4.3/src/dictrule/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:44.833292 dictrule-0.4.3/src/dictrule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 17:02:44.000000 dictrule-0.4.3/src/dictrule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:12:09.143674 dictrule-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 17:12:06.000000 dictrule-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-05-03 17:12:09.143674 dictrule-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-03 17:12:06.000000 dictrule-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:12:09.143674 dictrule-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-03 17:12:06.000000 dictrule-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:12:09.139674 dictrule-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:12:09.143674 dictrule-0.4.4/src/dictrule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:12:09.143674 dictrule-0.4.4/src/dictrule/built_in_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/comment_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/for_in_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/format_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/indent_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/inline_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/join_block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/join_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/built_in_rules/stringify_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/dr_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/eo_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/eval_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-03 17:12:06.000000 dictrule-0.4.4/src/dictrule/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:12:09.143674 dictrule-0.4.4/src/dictrule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13123 2024-05-03 17:12:09.000000 dictrule-0.4.4/src/dictrule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-03 17:12:09.000000 dictrule-0.4.4/src/dictrule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:12:09.000000 dictrule-0.4.4/src/dictrule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:12:09.000000 dictrule-0.4.4/src/dictrule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 17:12:09.000000 dictrule-0.4.4/src/dictrule.egg-info/top_level.txt
```

### Comparing `dictrule-0.4.3/LICENSE` & `dictrule-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/PKG-INFO` & `dictrule-0.4.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: dictrule
-Version: 0.4.3
-Summary: Python rules defined by a dict and a text generator from the rules
-Home-page: https://github.com/elhoangvu/dictrule
-Author: Zooxy Le
-Author-email: elhoangvu@gmail.com
-License: MIT License
-Project-URL: Documentation, https://github.com/elhoangvu/dictrule
-Project-URL: Source, https://github.com/elhoangvu/dictrule
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dictrule
 
 [![PyPI version](https://badge.fury.io/py/dictrule.svg)](https://badge.fury.io/py/dictrule)
 [![Python package](https://github.com/elhoangvu/dictrule/actions/workflows/python-package.yml/badge.svg)](https://github.com/elhoangvu/dictrule/actions/workflows/python-package.yml)
 [![codecov](https://codecov.io/gh/elhoangvu/dictrule/graph/badge.svg?token=CPE82M9GVB)](https://codecov.io/gh/elhoangvu/dictrule)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/elhoangvu/dictrule/blob/main/LICENSE)
 
@@ -172,15 +142,15 @@
 Building `Context` with `CommentRule.ContextCase` to define the comment style.
 
 **Example**
 
 ```python
 >>> context = build_singleline_context("#")
 >>> dictrule.Generator({
-...     "comment": "This is a single-line comment"
+...     "comment": "This is a single-line comment",
 ... }).generate(context)
 # This is a single-line comment
 
 >>> context = build_multiline_context('"""')
 >>> dictrule.Generator({
 ...     "style": "multiline",
 ...     "comment": [
@@ -203,21 +173,21 @@
 | eval | Yes      | string     | Variable name or keypath or command are provided from your generator. |
 
 **Example**
 
 ```python
 >>> git_author = "Zooxy Le"
 >>> dictrule.Generator({
-...     "eval": "git_author"
+...     "eval": "git_author",
 ... }).generate()
 Zooxy Le
 
 >>> project_id = "123456789"
 >>> dictrule.Generator({
-...     "eval": "project_id"
+...     "eval": "project_id",
 ... }).generate()
 123456789
 ```
 
 ### ForInRule
 
 This rule executes generatable rules in a `for-in-block` loop with a provided iterable variable.
@@ -234,19 +204,19 @@
 
 ```python
 >>> context = build_saved_lines_context([
 ...     Line(content="This is the line_1 content"),
 ...     Line(content="This is the line_2 content"),
 ... ])
 >>> dictrule.Generator({
-...     "for": "line"
-...     "in": "saved_lines"
+...     "for": "line",
+...     "in": "saved_lines",
 ...     "block: [
 ...         "line.index",
-...         "line.content"
+...         "line.content",
 ...     ]
 ... }).generate()
 1
 This is the line_1 content
 2
 This is the line_2 content
 ```
@@ -261,21 +231,29 @@
 | format_uppercase  | string/list/dict | A text or rules generated to format text in uppercase.                |
 | format_upper_head | string/list/dict | A text or rules generated to format the first character to uppercase. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...     "format_lowercase": "UPPERCASE TITLE"
-...     "format_uppercase": "lowercase content"
-...     "format_upper_head": "camelVariable"
+...     "format_lowercase": "UPPERCASE TITLE",
+...     "format_uppercase": "lowercase content",
+...     "format_upper_head": "camelVariable",
+...     "format_camel_case": "Camel case",
+...     "format_pascal_case": "pascal case",
+...     "format_kabab_case": "Kebab case",
+...     "format_snake_case": "Snake case",
 ... }).generated()
 uppercase title
 LOWERCASE CONTENT
 CamelVariable
+camelCase
+PascalCase
+kebab-case
+snake_case
 ```
 
 ### IndentRule
 
 This rule indents generated text from provided rules by a specified number of indent spaces.
 
 | Key prefix | Required | Value type       | Value description                                                                                                                                        |
@@ -285,17 +263,17 @@
 Defines the number of spaces for text indentation by providing `IndentRule.ContextCase` within the `Context`.
 
 **Example**
 
 ```python
 >>> context = build_number_spaces_context(4)
 >>> dictrule.Generator({
-...     "class Menu:"
-...     "indent_1": "def content(self):"
-...     "indent_2": "return 'Empty'"
+...     "class Menu:",
+...     "indent_1": "def content(self):",
+...     "indent_2": "return 'Empty'",
 ... }).generate(context)
 class Menu:
     def content(self):
         return 'Empty'
 ```
 
 ### InlineRule
@@ -306,15 +284,15 @@
 | ------ |:--------:| ---------- | ------------------------------------------ |
 | inline | Yes      | list       | A list of other rules that join in a line. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...    "inline": ["This", " is", " the", " text", " in", " a", " line"]
+...    "inline": ["This", " is", " the", " text", " in", " a", " line"],
 ... }).generate()
 This is the text in a line
 ```
 
 ### JoinBlockRule
 
 This rule joins generated texts for a block of rules by a specified separator.
@@ -324,16 +302,16 @@
 | join  | Yes      | string     | Separator for joining.                                            |
 | block | Yes      | list       | A list of other rules that generates a list of texts for joining. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...     "join": "-"
-...     "block": ["This", "is", "the", "snake", "line"]
+...     "join": "-",
+...     "block": ["This", "is", "the", "snake", "line"],
 ... }).generate()
 This-is-the-snake-line
 ```
 
 ### JoinEvalRule
 
 This rule joins generated texts from the value of `EvalRule` by a specified separator.
@@ -352,16 +330,16 @@
 ...     "Bayern Munchen",
 ...     "PSG",
 ...     "MC",
 ...     "MU",
 ...     "AC Milan",
 ... ])
 >>> dictrule.Generator({
-...     "join": ", "
-...     "eval": "football_teams"
+...     "join": ", ",
+...     "eval": "football_teams",
 ... }).generate(context)
 Real Madrid, Barcelona, Bayern Munchen, PSG, MC, MU, AC Milan
 ```
 
 ### StringifyRule
 
 This rule wraps content by quotes.
@@ -370,16 +348,16 @@
 | --------- |:--------:| ---------------- | -------------------------------------------------- |
 | stringify | Yes      | string/list/dict | A text or other rules quoted after generated text. |
 
 **Examples:**
 
 ```python
 >>> dictrule.Generator({
-...    "stringify": "This is the 1st text"
-...    "stringify": "This is the 2nd text"
+...    "stringify": "This is the 1st text",
+...    "stringify": "This is the 2nd text",
 ... }).generate()
 "This is the 1st text"
 "This is the 2nd text"
 ```
 
 ## Testing
```

### Comparing `dictrule-0.4.3/README.md` & `dictrule-0.4.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: dictrule
+Version: 0.4.4
+Summary: Python rules defined by a dict and a text generator from the rules
+Home-page: https://github.com/elhoangvu/dictrule
+Author: Zooxy Le
+Author-email: elhoangvu@gmail.com
+License: MIT License
+Project-URL: Documentation, https://github.com/elhoangvu/dictrule
+Project-URL: Source, https://github.com/elhoangvu/dictrule
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing :: Markup
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dictrule
 
 [![PyPI version](https://badge.fury.io/py/dictrule.svg)](https://badge.fury.io/py/dictrule)
 [![Python package](https://github.com/elhoangvu/dictrule/actions/workflows/python-package.yml/badge.svg)](https://github.com/elhoangvu/dictrule/actions/workflows/python-package.yml)
 [![codecov](https://codecov.io/gh/elhoangvu/dictrule/graph/badge.svg?token=CPE82M9GVB)](https://codecov.io/gh/elhoangvu/dictrule)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/elhoangvu/dictrule/blob/main/LICENSE)
 
@@ -142,15 +172,15 @@
 Building `Context` with `CommentRule.ContextCase` to define the comment style.
 
 **Example**
 
 ```python
 >>> context = build_singleline_context("#")
 >>> dictrule.Generator({
-...     "comment": "This is a single-line comment"
+...     "comment": "This is a single-line comment",
 ... }).generate(context)
 # This is a single-line comment
 
 >>> context = build_multiline_context('"""')
 >>> dictrule.Generator({
 ...     "style": "multiline",
 ...     "comment": [
@@ -173,21 +203,21 @@
 | eval | Yes      | string     | Variable name or keypath or command are provided from your generator. |
 
 **Example**
 
 ```python
 >>> git_author = "Zooxy Le"
 >>> dictrule.Generator({
-...     "eval": "git_author"
+...     "eval": "git_author",
 ... }).generate()
 Zooxy Le
 
 >>> project_id = "123456789"
 >>> dictrule.Generator({
-...     "eval": "project_id"
+...     "eval": "project_id",
 ... }).generate()
 123456789
 ```
 
 ### ForInRule
 
 This rule executes generatable rules in a `for-in-block` loop with a provided iterable variable.
@@ -204,19 +234,19 @@
 
 ```python
 >>> context = build_saved_lines_context([
 ...     Line(content="This is the line_1 content"),
 ...     Line(content="This is the line_2 content"),
 ... ])
 >>> dictrule.Generator({
-...     "for": "line"
-...     "in": "saved_lines"
+...     "for": "line",
+...     "in": "saved_lines",
 ...     "block: [
 ...         "line.index",
-...         "line.content"
+...         "line.content",
 ...     ]
 ... }).generate()
 1
 This is the line_1 content
 2
 This is the line_2 content
 ```
@@ -231,21 +261,29 @@
 | format_uppercase  | string/list/dict | A text or rules generated to format text in uppercase.                |
 | format_upper_head | string/list/dict | A text or rules generated to format the first character to uppercase. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...     "format_lowercase": "UPPERCASE TITLE"
-...     "format_uppercase": "lowercase content"
-...     "format_upper_head": "camelVariable"
+...     "format_lowercase": "UPPERCASE TITLE",
+...     "format_uppercase": "lowercase content",
+...     "format_upper_head": "camelVariable",
+...     "format_camel_case": "Camel case",
+...     "format_pascal_case": "pascal case",
+...     "format_kabab_case": "Kebab case",
+...     "format_snake_case": "Snake case",
 ... }).generated()
 uppercase title
 LOWERCASE CONTENT
 CamelVariable
+camelCase
+PascalCase
+kebab-case
+snake_case
 ```
 
 ### IndentRule
 
 This rule indents generated text from provided rules by a specified number of indent spaces.
 
 | Key prefix | Required | Value type       | Value description                                                                                                                                        |
@@ -255,17 +293,17 @@
 Defines the number of spaces for text indentation by providing `IndentRule.ContextCase` within the `Context`.
 
 **Example**
 
 ```python
 >>> context = build_number_spaces_context(4)
 >>> dictrule.Generator({
-...     "class Menu:"
-...     "indent_1": "def content(self):"
-...     "indent_2": "return 'Empty'"
+...     "class Menu:",
+...     "indent_1": "def content(self):",
+...     "indent_2": "return 'Empty'",
 ... }).generate(context)
 class Menu:
     def content(self):
         return 'Empty'
 ```
 
 ### InlineRule
@@ -276,15 +314,15 @@
 | ------ |:--------:| ---------- | ------------------------------------------ |
 | inline | Yes      | list       | A list of other rules that join in a line. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...    "inline": ["This", " is", " the", " text", " in", " a", " line"]
+...    "inline": ["This", " is", " the", " text", " in", " a", " line"],
 ... }).generate()
 This is the text in a line
 ```
 
 ### JoinBlockRule
 
 This rule joins generated texts for a block of rules by a specified separator.
@@ -294,16 +332,16 @@
 | join  | Yes      | string     | Separator for joining.                                            |
 | block | Yes      | list       | A list of other rules that generates a list of texts for joining. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...     "join": "-"
-...     "block": ["This", "is", "the", "snake", "line"]
+...     "join": "-",
+...     "block": ["This", "is", "the", "snake", "line"],
 ... }).generate()
 This-is-the-snake-line
 ```
 
 ### JoinEvalRule
 
 This rule joins generated texts from the value of `EvalRule` by a specified separator.
@@ -322,16 +360,16 @@
 ...     "Bayern Munchen",
 ...     "PSG",
 ...     "MC",
 ...     "MU",
 ...     "AC Milan",
 ... ])
 >>> dictrule.Generator({
-...     "join": ", "
-...     "eval": "football_teams"
+...     "join": ", ",
+...     "eval": "football_teams",
 ... }).generate(context)
 Real Madrid, Barcelona, Bayern Munchen, PSG, MC, MU, AC Milan
 ```
 
 ### StringifyRule
 
 This rule wraps content by quotes.
@@ -340,16 +378,16 @@
 | --------- |:--------:| ---------------- | -------------------------------------------------- |
 | stringify | Yes      | string/list/dict | A text or other rules quoted after generated text. |
 
 **Examples:**
 
 ```python
 >>> dictrule.Generator({
-...    "stringify": "This is the 1st text"
-...    "stringify": "This is the 2nd text"
+...    "stringify": "This is the 1st text",
+...    "stringify": "This is the 2nd text",
 ... }).generate()
 "This is the 1st text"
 "This is the 2nd text"
 ```
 
 ## Testing
```

### Comparing `dictrule-0.4.3/setup.py` & `dictrule-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule/__init__.py` & `dictrule-0.4.4/src/dictrule/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule/__version__.py` & `dictrule-0.4.4/src/dictrule/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/    |___/\___/_/  /____/_/\____/_/ /_/ 
                                                                           
 """
 
 __title__ = "dictrule"
 __description__ = "Python rules defined by a dict and a text generator from the rules"
 __url__ = "https://github.com/elhoangvu/dictrule"
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 __author__ = "Zooxy Le"
 __author_email__ = "elhoangvu@gmail.com"
 __license__ = "MIT License"
 __copyright__ = "Copyright Zooxy Le"
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/__init__.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/block_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/comment_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/comment_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from enum import Enum
 from ..dr_property import dr_property
 from ..rule import Rule
 from ..context import Context
 from ..exceptions import (
     NoneValueException,
     InvalidTypeException,
-    InvalidValueException,
 )
 
 
 class CommentRule(Rule):
     """This rule allows generating comment text based on single-line and multi-line rules.
 
     Building `Context` with `CommentRule.ContextCase` to define the comment style.
@@ -95,15 +94,15 @@
             @staticmethod
             @property
             def style() -> "CommentRule.Style":
                 return CommentRule.Style.SINGLELINE
 
             @property
             def prefix(self) -> str:
-                """Getter for `prefix` property"""
+                """Get the `prefix` property"""
 
                 return self._prefix
 
         class MultilineComment(Comment):
             """Multiline comment by comment open, comment close, and prefix for each line"""
 
             def __init__(
@@ -127,33 +126,33 @@
             @staticmethod
             @property
             def style() -> "CommentRule.Style":
                 return CommentRule.Style.MULTILINE
 
             @property
             def prefix(self) -> str:
-                """Getter for `prefix` property"""
+                """Get the `prefix` property"""
 
                 return self._prefix
 
             @property
             def open_comment(self) -> str:
-                """Getter for `open_comment` property"""
+                """Get the `open_comment` property"""
 
                 return self._open_comment
 
             @property
             def close_comment(self) -> str:
-                """Getter for `close_comment` property"""
+                """Get the `close_comment` property"""
 
                 return self._close_comment
 
         @property
         def name(self) -> str:
-            """Getter for `name` property"""
+            """Get the `name` property"""
 
             return CommentRule.CONTEXT_NAME
 
         def __init__(
             self,
             singleline: Optional[SinglelineComment] = None,
             multiline: Optional[MultilineComment] = None,
@@ -168,21 +167,21 @@
             """
 
             self._singleline = singleline
             self._multiline = multiline
 
         @property
         def singleline(self) -> SinglelineComment:
-            """Getter for `singleline` property"""
+            """Get the `singleline` property"""
 
             return self._singleline
 
         @property
         def multiline(self) -> MultilineComment:
-            """Getter for `multiline` property"""
+            """Get the `multiline` property"""
 
             return self._multiline
 
     class Style(Enum):
         """Enumeration defining comment styles"""
 
         SINGLELINE = "singleline"
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/eval_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/eval_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 class EvalRule(Rule):
     """This rule evaluates the value of provied variable or command.
 
     Examples:
     ---------
     >>> git_author = "Zooxy Le"
     >>> dictrule.Generator({
-    ...     "eval": "git_author"
+    ...     "eval": "git_author",
     ... }).generate()
     Zooxy Le
 
     >>> project_id = "123456789"
     >>> dictrule.Generator({
-    ...     "eval": "project_id"
+    ...     "eval": "project_id",
     ... }).generate()
     123456789
     """
 
     CONTEXT_NAME = "eval"
 
     @dr_property()
@@ -113,36 +113,36 @@
             evaluators (List["EvalRule.Evaluable"]): The list of evaluators.
             fallback (Optional["EvalRule.Evaluable"], optional): The fallback evaluator
                 for other rules. Defaults to None.
         """
 
         @property
         def name(self) -> str:
-            """Getter for `name` property"""
+            """Get the `name` property"""
 
             return EvalRule.CONTEXT_NAME
 
         @property
         def evaluator_list(self) -> List["EvalRule.Evaluable"]:
-            """Getter for `evaluator_list` property"""
+            """Get the `evaluator_list` property"""
 
             return self._evaluator_list
 
         @property
         def fallback(self) -> Optional["EvalRule.Evaluable"]:
-            """Getter for `fallback` property"""
+            """Get the `fallback` property"""
 
             return self._fallback
 
         def __init__(
             self,
             evaluators: List["EvalRule.Evaluable"],
             fallback: Optional["EvalRule.Evaluable"] = None,
         ):
-            """Initialization method for `EvalRule.ContextCase`.
+            """Constructor method for `EvalRule.ContextCase`.
 
             Args:
                 evaluators (List["EvalRule.Evaluable"]): List of evaluators.
                 fallback (Optional["EvalRule.Evaluable"], optional): Fallback for other rules.
                     Defaults to None.
             """
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/for_in_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/for_in_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     Examples:
     ---------
     >>> context = build_saved_lines_context([
     ...     Line(content="This is the line_1 content"),
     ...     Line(content="This is the line_2 content"),
     ... ])
     >>> dictrule.Generator({
-    ...     "for": "line"
-    ...     "in": "saved_lines"
+    ...     "for": "line",
+    ...     "in": "saved_lines",
     ...     "block: [
     ...         "line.index",
-    ...         "line.content"
+    ...         "line.content",
     ...     ]
     ... }).generate()
     1
     This is the line_1 content
     2
     This is the line_2 content
     """
@@ -83,21 +83,21 @@
         and this is the description
         are_created_at
         2024-01-01
         """
 
         @property
         def name(self) -> str:
-            """Getter for `name` property"""
+            """Get the `name` property"""
 
             return self._var_name
 
         @property
         def prefix_matching(self) -> bool:
-            """Getter for `prefix_matching` property"""
+            """Get the `prefix_matching` property"""
 
             return True
 
         def __init__(
             self,
             var_name: str,
             var: Any,
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/format_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/indent_rule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,135 @@
-"""Format rule module"""
+"""Indent rule module"""
 
 from typing import (
     Dict,
     Any,
     Callable,
     Optional,
 )
 
-from enum import Enum
 from ..rule import Rule
 from ..dr_property import dr_property
 from ..context import Context
 from ..exceptions import (
     NoneValueException,
     InvalidValueException,
     InvalidTypeException,
 )
 
 
-class FormatRule(Rule):
-    """This rule formats text according to specified rules.
+class IndentRule(Rule):
+    """This rule indents generated text from provided rules by a specified number of indent spaces.
+
+    Defines the number of spaces for text indentation by providing `IndentRule.ContextCase`
+    within the `Context`.
 
     Examples:
     ---------
+    >>> context = build_number_spaces_context(4)
     >>> dictrule.Generator({
-    ...     "format_lowercase": "UPPERCASE TITLE"
-    ...     "format_uppercase": "lowercase content"
-    ...     "format_upper_head": "camelVariable"
-    ... }).generated()
-    uppercase title
-    LOWERCASE CONTENT
-    CamelVariable
+    ...     "class Menu:",
+    ...     "indent_1": "def content(self):",
+    ...     "indent_2": "return 'Empty'",
+    ... }).generate(context)
+    class Menu:
+        def content(self):
+            return 'Empty'
     """
 
-    @dr_property(prefix_matching=True)
-    def _format(self, props: Dict[str, Any]) -> Any:
-        """Property method for retrieving the `format` attribute."""
-
-    class Type(Enum):
-        """Enum representing different formatting types for `FormatRule`."""
-
-        LOWERCASE = "lowercase"
-        UPPERCASE = "uppercase"
-        UPPER_HEAD = "upper_head"
-
-        @staticmethod
-        def from_str(string: str) -> Optional["FormatRule.Type"]:
-            """Creates a `FormatRule.Type` enum from a string.
-
-            Args:
-                string (str): The string value representing the formatting type.
+    DEFAULT_SPACES = 2
+    CONTEXT_NAME = "indent"
 
-            Returns:
-                Optional[FormatRule.Type]: The corresponding enum value.
-            """
+    class ContextCase(Context.Case):
+        """`Context.Case` for `IndentRule`."""
 
-            try:
-                return FormatRule.Type(string)
-            except ValueError:
-                pass
+        @property
+        def name(self) -> str:
+            """Get the `name` property"""
 
-            return None
+            return "indent"
 
-        def format(
+        def __init__(
             self,
-            text: str,
-        ) -> str:
-            """Formats the provided text based on the formatting type.
+            num_spaces: int,
+        ):
+            """Initializes the context case.
 
             Args:
-                text (str): The text to be formatted.
-
-            Returns:
-                str: The formatted text.
+                num_spaces (int): The number of spaces for each level of indentation.
             """
 
-            if self == FormatRule.Type.LOWERCASE:
-                return text.lower()
+            self._num_spaces = num_spaces
 
-            if self == FormatRule.Type.UPPERCASE:
-                return text.upper()
+        @property
+        def num_spaces(self) -> int:
+            """Get the `num_spaces` property"""
 
-            if self == FormatRule.Type.UPPER_HEAD:
-                return (text[0].upper() + text[1:]) if len(text) > 0 else ""
+            return self._num_spaces
 
-            return text
+    @dr_property(prefix_matching=True)
+    def _indent(self, props: Dict[str, Any]) -> Any:
+        """Property method for retrieving the `indent` attribute."""
 
     def parse(
         self,
         rule_dict: Dict[str, Any],
         rule_callback: Callable[[Optional[Context], Any], str],
         context: Optional[Context] = None,
     ) -> str:
-        """Parses the format rule and applies formatting to the provided text.
+        """Parses the indent rule and applies indentation to the provided text.
 
         Args:
-            rule_dict (Dict[str, Any]): The dictionary containing the format rule.
+            rule_dict (Dict[str, Any]): The dictionary containing the indent rule.
             rule_callback (Callable[[Optional[Context], Any], str]): A callback function
                 for processing rules.
             context (Optional[Context], optional): The context for the rule. Defaults to None.
 
         Returns:
-            str: The formatted text.
+            str: The indented text.
         """
 
-        format_name, format_rule = self._format(rule_dict)
-        if not format_name.startswith("format_"):
-            raise InvalidValueException(f"Invalid format {format_name}")
-
-        format_type = FormatRule.Type.from_str(format_name[len("format_") :])
-        if format_type is None:
-            raise NoneValueException(
-                "`format:` type {format_type} in invalid with format {format_name}"
-            )
-
-        format_text = rule_callback(
-            context,
-            format_rule,
-        )
-
-        if not isinstance(format_text, str):
-            raise InvalidTypeException(
-                f"`format:` text {format_text} for rule {format_rule} must be a str"
-            )
+        if context is None:
+            raise NoneValueException("param `context` must not be None")
+
+        context_case: IndentRule.ContextCase = context.get(IndentRule.CONTEXT_NAME)
+
+        indent_spaces = IndentRule.DEFAULT_SPACES
+        if context_case:
+            if not isinstance(context_case, IndentRule.ContextCase):
+                raise InvalidTypeException(
+                    f"Invalid {type(context_case)} type for {IndentRule.CONTEXT_NAME} in context"
+                )
+
+            indent_spaces = context_case.num_spaces
+
+        indent, value = self._indent(rule_dict)
+        if not indent.startswith("indent_"):
+            raise InvalidValueException(f"Invalid indent {indent}")
+
+        if not indent_spaces or indent_spaces <= 0:
+            indent_spaces = IndentRule.DEFAULT_SPACES
+
+        if not isinstance(indent_spaces, int) and not (
+            isinstance(indent_spaces, str) and str.isdigit(indent_spaces)
+        ):
+            raise InvalidTypeException("`indent_spaces` must be a digit")
+
+        indent_spaces: int = int(indent_spaces)
+
+        if not indent_spaces:
+            print("`indent_spaces` is not found in `context`, using default spaces")
+            indent_spaces = 4
+
+        if not isinstance(value, str):
+            value = rule_callback(context, value)
+
+        indent_prefix = indent_spaces
+        if indent != "indent":
+            indent_count = indent[len("indent_") :]
+            if not indent_count.isdigit():
+                raise InvalidValueException("`indent_` suffix must be a digit str")
+
+            indent_prefix = indent_spaces * int(indent_count) * " "
 
-        return format_type.format(format_text)
+        value = indent_prefix + value.replace("\n", f"\n{indent_prefix}")
+        return value
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/inline_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/inline_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class InlineRule(Rule):
     """This rule builds generated text of a list of rules that are in a line.
 
     Examples:
     ---------
     >>> dictrule.Generator({
-    ...    "inline": ["This", " is", " the", " text", " in", " a", " line"]
+    ...    "inline": ["This", " is", " the", " text", " in", " a", " line"],
     ... }).generate()
     This is the text in a line
     """
 
     @dr_property()
     def _inline(self, props: Dict[str, Any]) -> Any:
         """Property method for retrieving the `inline` attribute."""
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/join_block_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/join_block_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 class JoinBlockRule(BlockRule):
     """This rule joins generated texts for a block of rules by a specified separator.
 
     Examples:
     ---------
     >>> dictrule.Generator({
-    ...     "join": "-"
-    ...     "block": ["This", "is", "the", "snake", "line"]
+    ...     "join": "-",
+    ...     "block": ["This", "is", "the", "snake", "line"],
     ... }).generate()
     This-is-the-snake-line
     """
 
     @dr_property()
     def _join(self, props: Dict[str, Any]) -> Any:
         """Property method for retrieving the `join` attribute."""
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/join_eval_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/join_eval_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     ...     "Bayern Munchen",
     ...     "PSG",
     ...     "MC",
     ...     "MU",
     ...     "AC Milan",
     ... ])
     >>> dictrule.Generator({
-    ...     "join": ", "
-    ...     "eval": "football_teams"
+    ...     "join": ", ",
+    ...     "eval": "football_teams",
     ... }).generate(context)
     Real Madrid, Barcelona, Bayern Munchen, PSG, MC, MU, AC Milan
     """
 
     @dr_property()
     def _join(self, props: Dict[str, Any]) -> Any:
         """Property method for retrieving the `join` attribute."""
```

### Comparing `dictrule-0.4.3/src/dictrule/built_in_rules/stringify_rule.py` & `dictrule-0.4.4/src/dictrule/built_in_rules/stringify_rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 class StringifyRule(Rule):
     """This rule wraps content by quotes.
 
     Examples:
     ---------
     >>> dictrule.Generator({
-    ...    "stringify": "This is the 1st text"
-    ...    "stringify": "This is the 2nd text"
+    ...    "stringify": "This is the 1st text",
+    ...    "stringify": "This is the 2nd text",
     ... }).generate()
     "This is the 1st text"
     "This is the 2nd text"
     """
 
     QUOTE = '"'
```

### Comparing `dictrule-0.4.3/src/dictrule/context.py` & `dictrule-0.4.4/src/dictrule/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     """Context class contains information for rule generation"""
 
     class Case(ABC):
         """Base class for each rule, providing information for rule generation"""
 
         @property
         def name(self) -> str:
-            """Getter for case name, matching the defined rule
+            """Get the case name, matching the defined rule
 
             Returns:
                 str: A rule name
             """
 
             return ""
 
     def __init__(
         self,
         cases: List[Case],
     ) -> None:
-        """Initialization method of `Context` class
+        """Constructor method of `Context` class
 
         Args:
             cases (List[Case]): List of `Context.Case` to build the case map
         """
 
         self._cases = list(cases)
         case_map: Dict[str, Context.Case] = {}
@@ -51,24 +51,24 @@
 
             case_map[case.name] = case
 
         self._case_map = case_map
 
     @property
     def cases(self) -> List[Case]:
-        """Getter for `cases` property
+        """Get the `cases` property
 
         Returns:
             List[Case]: list of cases
         """
         return self._cases
 
     @property
     def case_map(self) -> Dict[str, Case]:
-        """Getter for `case_map` property
+        """Get the `case_map` property
 
         Returns:
             Dict[str, Case]: map of cases [name: str, case: Context.Case]
         """
 
         return self._case_map
```

### Comparing `dictrule-0.4.3/src/dictrule/dr_property.py` & `dictrule-0.4.4/src/dictrule/dr_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     _optional_key = "_dr_optional"
 
     def __init__(
         self,
         optional: bool = False,
         prefix_matching: bool = False,
     ):
-        """Initialization method of `dr_property`
+        """Constructor method of `dr_property`
 
         Args:
             optional (bool, optional): Indicates if the property is optional
                 and used for detecting rules. Defaults to False.
             prefix_matching (bool, optional): Indicates if the property matches the rule prefix.
                 Defaults to False.
         """
```

### Comparing `dictrule-0.4.3/src/dictrule/eo_property.py` & `dictrule-0.4.4/src/dictrule/eo_property.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule/eval_object.py` & `dictrule-0.4.4/src/dictrule/eval_object.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule/generator.py` & `dictrule-0.4.4/src/dictrule/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     ]
 
     def __init__(
         self,
         gen_rules: List[Union[str, Dict[str, Any]]],
         parse_rules: Optional[List[Rule]] = None,
     ):
-        """Initialization method for DictRule.
+        """Constructor method for DictRule.
 
         Args:
             gen_rules (List[Union[str, Dict[str, Any]]]): List or dictionary of rules
             parse_rules (Optional[List[Rule]], optional):
                 List of rule parsers bases on `Rule`.
                 Defaults to `DictRule.STD_RULES`.
         """
@@ -72,21 +72,21 @@
         self._cache_rules: Dict[str, Rule] = {}
         self._gen_rules = list(gen_rules)
         self._parse_rules: List[Rule] = []
         self.add_parse_rules(parse_rules)
 
     @property
     def parse_rules(self) -> List[Rule]:
-        """Getter for `parse_rules` property"""
+        """Get the `parse_rules` property"""
 
         return self._parse_rules
 
     @property
     def gen_rules(self) -> List[Union[str, Dict[str, Any]]]:
-        """Getter for `gen_rules` property"""
+        """Get the `gen_rules` property"""
 
         return self._gen_rules
 
     def add_parse_rule(
         self,
         rule: Rule,
     ):
```

### Comparing `dictrule-0.4.3/src/dictrule/rule.py` & `dictrule-0.4.4/src/dictrule/rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.3/src/dictrule.egg-info/PKG-INFO` & `dictrule-0.4.4/src/dictrule.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
@@ -172,15 +172,15 @@
 Building `Context` with `CommentRule.ContextCase` to define the comment style.
 
 **Example**
 
 ```python
 >>> context = build_singleline_context("#")
 >>> dictrule.Generator({
-...     "comment": "This is a single-line comment"
+...     "comment": "This is a single-line comment",
 ... }).generate(context)
 # This is a single-line comment
 
 >>> context = build_multiline_context('"""')
 >>> dictrule.Generator({
 ...     "style": "multiline",
 ...     "comment": [
@@ -203,21 +203,21 @@
 | eval | Yes      | string     | Variable name or keypath or command are provided from your generator. |
 
 **Example**
 
 ```python
 >>> git_author = "Zooxy Le"
 >>> dictrule.Generator({
-...     "eval": "git_author"
+...     "eval": "git_author",
 ... }).generate()
 Zooxy Le
 
 >>> project_id = "123456789"
 >>> dictrule.Generator({
-...     "eval": "project_id"
+...     "eval": "project_id",
 ... }).generate()
 123456789
 ```
 
 ### ForInRule
 
 This rule executes generatable rules in a `for-in-block` loop with a provided iterable variable.
@@ -234,19 +234,19 @@
 
 ```python
 >>> context = build_saved_lines_context([
 ...     Line(content="This is the line_1 content"),
 ...     Line(content="This is the line_2 content"),
 ... ])
 >>> dictrule.Generator({
-...     "for": "line"
-...     "in": "saved_lines"
+...     "for": "line",
+...     "in": "saved_lines",
 ...     "block: [
 ...         "line.index",
-...         "line.content"
+...         "line.content",
 ...     ]
 ... }).generate()
 1
 This is the line_1 content
 2
 This is the line_2 content
 ```
@@ -261,21 +261,29 @@
 | format_uppercase  | string/list/dict | A text or rules generated to format text in uppercase.                |
 | format_upper_head | string/list/dict | A text or rules generated to format the first character to uppercase. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...     "format_lowercase": "UPPERCASE TITLE"
-...     "format_uppercase": "lowercase content"
-...     "format_upper_head": "camelVariable"
+...     "format_lowercase": "UPPERCASE TITLE",
+...     "format_uppercase": "lowercase content",
+...     "format_upper_head": "camelVariable",
+...     "format_camel_case": "Camel case",
+...     "format_pascal_case": "pascal case",
+...     "format_kabab_case": "Kebab case",
+...     "format_snake_case": "Snake case",
 ... }).generated()
 uppercase title
 LOWERCASE CONTENT
 CamelVariable
+camelCase
+PascalCase
+kebab-case
+snake_case
 ```
 
 ### IndentRule
 
 This rule indents generated text from provided rules by a specified number of indent spaces.
 
 | Key prefix | Required | Value type       | Value description                                                                                                                                        |
@@ -285,17 +293,17 @@
 Defines the number of spaces for text indentation by providing `IndentRule.ContextCase` within the `Context`.
 
 **Example**
 
 ```python
 >>> context = build_number_spaces_context(4)
 >>> dictrule.Generator({
-...     "class Menu:"
-...     "indent_1": "def content(self):"
-...     "indent_2": "return 'Empty'"
+...     "class Menu:",
+...     "indent_1": "def content(self):",
+...     "indent_2": "return 'Empty'",
 ... }).generate(context)
 class Menu:
     def content(self):
         return 'Empty'
 ```
 
 ### InlineRule
@@ -306,15 +314,15 @@
 | ------ |:--------:| ---------- | ------------------------------------------ |
 | inline | Yes      | list       | A list of other rules that join in a line. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...    "inline": ["This", " is", " the", " text", " in", " a", " line"]
+...    "inline": ["This", " is", " the", " text", " in", " a", " line"],
 ... }).generate()
 This is the text in a line
 ```
 
 ### JoinBlockRule
 
 This rule joins generated texts for a block of rules by a specified separator.
@@ -324,16 +332,16 @@
 | join  | Yes      | string     | Separator for joining.                                            |
 | block | Yes      | list       | A list of other rules that generates a list of texts for joining. |
 
 **Example**
 
 ```python
 >>> dictrule.Generator({
-...     "join": "-"
-...     "block": ["This", "is", "the", "snake", "line"]
+...     "join": "-",
+...     "block": ["This", "is", "the", "snake", "line"],
 ... }).generate()
 This-is-the-snake-line
 ```
 
 ### JoinEvalRule
 
 This rule joins generated texts from the value of `EvalRule` by a specified separator.
@@ -352,16 +360,16 @@
 ...     "Bayern Munchen",
 ...     "PSG",
 ...     "MC",
 ...     "MU",
 ...     "AC Milan",
 ... ])
 >>> dictrule.Generator({
-...     "join": ", "
-...     "eval": "football_teams"
+...     "join": ", ",
+...     "eval": "football_teams",
 ... }).generate(context)
 Real Madrid, Barcelona, Bayern Munchen, PSG, MC, MU, AC Milan
 ```
 
 ### StringifyRule
 
 This rule wraps content by quotes.
@@ -370,16 +378,16 @@
 | --------- |:--------:| ---------------- | -------------------------------------------------- |
 | stringify | Yes      | string/list/dict | A text or other rules quoted after generated text. |
 
 **Examples:**
 
 ```python
 >>> dictrule.Generator({
-...    "stringify": "This is the 1st text"
-...    "stringify": "This is the 2nd text"
+...    "stringify": "This is the 1st text",
+...    "stringify": "This is the 2nd text",
 ... }).generate()
 "This is the 1st text"
 "This is the 2nd text"
 ```
 
 ## Testing
```

### Comparing `dictrule-0.4.3/src/dictrule.egg-info/SOURCES.txt` & `dictrule-0.4.4/src/dictrule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

