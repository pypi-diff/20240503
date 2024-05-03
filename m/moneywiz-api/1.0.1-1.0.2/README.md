# Comparing `tmp/moneywiz_api-1.0.1.tar.gz` & `tmp/moneywiz_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneywiz_api-1.0.1.tar", last modified: Mon Apr 29 21:20:00 2024, max compression
+gzip compressed data, was "moneywiz_api-1.0.2.tar", last modified: Fri May  3 11:09:26 2024, max compression
```

## Comparing `moneywiz_api-1.0.1.tar` & `moneywiz_api-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.422801 moneywiz_api-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.422801 moneywiz_api-1.0.1/src/moneywiz_api/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.422801 moneywiz_api-1.0.1/src/moneywiz_api/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/database_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/src/moneywiz_api/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/category_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/investment_holding_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/payee_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/tag_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/src/moneywiz_api/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/investment_holding.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/payee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/raw_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/moneywiz_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.448028 moneywiz_api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-03 11:09:26.444028 moneywiz_api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:09:26.448028 moneywiz_api-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.440028 moneywiz_api-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.440028 moneywiz_api-1.0.2/src/moneywiz_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.444028 moneywiz_api-1.0.2/src/moneywiz_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/database_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.444028 moneywiz_api-1.0.2/src/moneywiz_api/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/category_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/investment_holding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/payee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/tag_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/managers/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.444028 moneywiz_api-1.0.2/src/moneywiz_api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/investment_holding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/payee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/raw_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14039 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/moneywiz_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/src/moneywiz_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.444028 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-03 11:09:26.000000 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-03 11:09:26.000000 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:09:26.000000 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 11:09:26.000000 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 11:09:26.000000 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 11:09:26.000000 moneywiz_api-1.0.2/src/moneywiz_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:09:26.444028 moneywiz_api-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 11:09:21.000000 moneywiz_api-1.0.2/tests/test_config.py
```

### Comparing `moneywiz_api-1.0.1/LICENSE` & `moneywiz_api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/PKG-INFO` & `moneywiz_api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.2 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pandas Requires-Dist: pytest Provides-Extra: dev
```

### Comparing `moneywiz_api-1.0.1/README.md` & `moneywiz_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/pyproject.toml` & `moneywiz_api-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "moneywiz-api"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="iLeoDo", email="iLeoDo@gmail.com" },
 ]
 description = "A Python api to access moneywiz sqlite database"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/cli/cli.py` & `moneywiz_api-1.0.2/src/moneywiz_api/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import logging
+import random
+import readline
+import rlcompleter
+from code import InteractiveConsole
 from os.path import expanduser
 from pathlib import Path
-from code import InteractiveConsole
 from typing import Dict, List
 
 import click
-import logging
-import readline
-import rlcompleter
-import random
+import pandas as pd
 
 from moneywiz_api.cli.helpers import ShellHelper
 from moneywiz_api.moneywiz_api import MoneywizApi
 
 
 def get_default_path() -> Path:
     return Path(
@@ -79,28 +80,28 @@
     helper = ShellHelper(moneywiz_api)
 
     names: Dict[str, str] = {
         f"{moneywiz_api=}".split("=")[0]: "MoneyWiz API",
         f"{accessor=}".split("=")[0]: "MoneyWiz Database Accessor",
         f"{account_manager=}".split("=")[0]: "Account Manager",
         f"{payee_manager=}".split("=")[0]: "Payee Manager",
-        f"{category_manager=}".split("=")[0]: "Category Manageer",
+        f"{category_manager=}".split("=")[0]: "Category Manager",
         f"{transaction_manager=}".split("=")[0]: "Transaction Manager",
         f"{investment_holding_manager=}".split("=")[0]: "Investment Holding Manager",
         f"{tag_manager=}".split("=")[0]: "Tag Manager",
         f"{helper=}".split("=")[0]: "Shell Helper",
     }
 
-    banner: List[str] = (
+    banner: List[str] = [
         f"Read-only MoneyWiz Shell on {db_file_path}",
         "",
-        "Avaliable components:",
+        "Available components:",
         *[f"- {component:30}  {desc}" for component, desc in names.items()],
         "===================================================================",
-    )
+    ]
 
     if demo_dump:
         _users_table = helper.users_table()
         click.secho("Users Table", fg="yellow")
         click.secho("--------------------------------", fg="yellow")
         click.secho(_users_table.to_string(index=False))
         click.secho("--------------------------------\n", fg="yellow")
@@ -122,14 +123,17 @@
         click.secho("--------------------------------", fg="yellow")
         click.secho(_accounts_table[["id", "name"]].sample(5).to_string(index=False))
         click.secho("--------------------------------\n", fg="yellow")
 
     _vars = globals()
     _vars.update(locals())
 
+    pd.options.display.max_rows = None
+    pd.options.display.max_colwidth = None
+
     readline.set_completer(rlcompleter.Completer(_vars).complete)
     readline.parse_and_bind("tab: complete")
     InteractiveConsole(_vars).interact(banner="\n".join(banner))
 
 
 if __name__ == "__main__":
     main()  # pylint: disable=no-value-for-parameter
```

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/cli/helpers.py` & `moneywiz_api-1.0.2/src/moneywiz_api/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/database_accessor.py` & `moneywiz_api-1.0.2/src/moneywiz_api/database_accessor.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/managers/account_manager.py` & `moneywiz_api-1.0.2/src/moneywiz_api/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/managers/category_manager.py` & `moneywiz_api-1.0.2/src/moneywiz_api/managers/category_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/managers/investment_holding_manager.py` & `moneywiz_api-1.0.2/src/moneywiz_api/managers/investment_holding_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/managers/record_manager.py` & `moneywiz_api-1.0.2/src/moneywiz_api/managers/record_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/managers/transaction_manager.py` & `moneywiz_api-1.0.2/src/moneywiz_api/managers/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/__init__.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/account.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/account.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/category.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/category.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/investment_holding.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/investment_holding.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/raw_data_handler.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/raw_data_handler.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/record.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/record.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/model/transaction.py` & `moneywiz_api-1.0.2/src/moneywiz_api/model/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from abc import ABC
 from dataclasses import dataclass
-from typing import Optional
 from datetime import datetime
 from decimal import Decimal
+from typing import Optional
+
+import pytest
 
 from moneywiz_api.model.raw_data_handler import RawDataHandler as RDH
 from moneywiz_api.model.record import Record
 from moneywiz_api.types import ID
 
 
-import pytest
-
-
 @dataclass
 class Transaction(Record, ABC):
     """
     ENT: 36
     """
 
     reconciled: bool
@@ -65,14 +64,18 @@
         self.payee = row["ZPAYEE2"]
         self.original_currency = row["ZORIGINALCURRENCY"]
         self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
         self.original_exchange_rate = RDH.get_nullable_decimal(
             row, "ZORIGINALEXCHANGERATE"
         )
 
+        # Fixes
+        if self.original_exchange_rate == Decimal(0):
+            self.original_exchange_rate = None
+
         # Validate
         self.validate()
 
     def validate(self):
         assert self.account is not None, self.as_dict()
         assert self.amount is not None, self.as_dict()
         # self.payee can be None
@@ -256,14 +259,18 @@
 
         self.original_currency = row["ZORIGINALCURRENCY"]
         self.original_amount = RDH.get_decimal(row, "ZORIGINALAMOUNT")
         self.original_exchange_rate = RDH.get_nullable_decimal(
             row, "ZORIGINALEXCHANGERATE"
         )
 
+        # Fixes
+        if self.original_exchange_rate == Decimal(0):
+            self.original_exchange_rate = None
+
         # Validate
         self.validate()
 
     def validate(self):
         assert self.account is not None
         assert self.amount is not None
         assert self.amount > 0
@@ -461,14 +468,17 @@
             row, "ZORIGINALEXCHANGERATE"
         )
 
         # Fixes
         if self.amount * self.original_amount < 0:
             self.original_amount = -self.original_amount
 
+        if self.original_exchange_rate == Decimal(0):
+            self.original_exchange_rate = None
+
         # Validate
         self.validate()
 
     def validate(self):
         assert self.account is not None
         assert self.amount is not None
         # self.payee can be None
```

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api/moneywiz_api.py` & `moneywiz_api-1.0.2/src/moneywiz_api/moneywiz_api.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api.egg-info/PKG-INFO` & `moneywiz_api-1.0.2/src/moneywiz_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.2 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pandas Requires-Dist: pytest Provides-Extra: dev
```

### Comparing `moneywiz_api-1.0.1/src/moneywiz_api.egg-info/SOURCES.txt` & `moneywiz_api-1.0.2/src/moneywiz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

