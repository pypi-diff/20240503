# Comparing `tmp/mailck-0.3.0.tar.gz` & `tmp/mailck-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailck-0.3.0.tar", max compression
+gzip compressed data, was "mailck-0.3.1.tar", max compression
```

## Comparing `mailck-0.3.0.tar` & `mailck-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32471 2023-12-20 14:28:07.561795 mailck-0.3.0/LICENSE
--rw-r--r--   0        0        0     4222 2024-04-05 09:47:28.352692 mailck-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-12-20 14:09:26.334235 mailck-0.3.0/mailck/__init__.py
--rw-r--r--   0        0        0     7301 2024-04-05 09:48:12.227381 mailck-0.3.0/mailck/main.py
--rw-r--r--   0        0        0      644 2024-04-05 09:41:21.844730 mailck-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 mailck-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-12-20 14:28:07.561795 mailck-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4229 2024-05-03 15:50:48.456584 mailck-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 15:50:22.009071 mailck-0.3.1/mailck/__init__.py
+-rw-r--r--   0        0        0     7273 2024-05-03 15:50:22.005738 mailck-0.3.1/mailck/main.py
+-rw-r--r--   0        0        0      645 2024-05-03 15:49:33.404184 mailck-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4905 1970-01-01 00:00:00.000000 mailck-0.3.1/PKG-INFO
```

### Comparing `mailck-0.3.0/LICENSE` & `mailck-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailck-0.3.0/README.md` & `mailck-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 - light: small size and resource usage
 - low dependencies: low or no external dependencies
 - terminal-focused: terminal usage focused (input and output) - primarily focused on usage through conky
 
 
 ## Latest Changes
 
-- changed --version to use importlib.metadata
+- minor cleanup of --version
+- update copyright date
 
 
 ### Notices
 
 - it does not make much sense to run this more frequently than every 10s as connecting takes ~1-2s
```

### Comparing `mailck-0.3.0/mailck/main.py` & `mailck-0.3.1/mailck/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 import email
 import imaplib
 import json
 import logging
+import importlib.metadata as md
 import sys
 from datetime import datetime
 from enum import Enum
 from optparse import OptionParser
 from os import getenv
 
 
@@ -89,19 +90,16 @@
 
 
 def show_version():
     """
     Show version.
     """
 
-    import importlib.metadata
-
-    _meta = importlib.metadata.metadata("mailck")
-    _name = _meta["Name"]
-    _version = _meta["Version"]
+    _name = md.metadata("mailck")["Name"]
+    _version = md.metadata("mailck")["Version"]
 
     logger.critical(f"{_name} {_version}")
 
 
 def check_mail(r: MCRequest = None):
     """
     Check mail.
```

### Comparing `mailck-0.3.0/pyproject.toml` & `mailck-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [internal]
 created = 2023-12-20
 modified = 2024-01-06
 
+
 [tool.poetry]
 name = "mailck"
-version = "0.3.0"
+version = "0.3.1"
 description = "a simple mail check utility, currently supporting IMAP"
 authors = ["drad <sa@adercon.com>"]
 maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/mailck"
 repository = "https://gitlab.com/drad/mailck"
```

### Comparing `mailck-0.3.0/PKG-INFO` & `mailck-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailck
-Version: 0.3.0
+Version: 0.3.1
 Summary: a simple mail check utility, currently supporting IMAP
 Home-page: https://gitlab.com/drad/mailck
 License: GPL-3.0-only
 Keywords: mail,imap,check,conky,cron,terminal,email
 Author: drad
 Author-email: sa@adercon.com
 Maintainer: drad
@@ -24,15 +24,16 @@
 - light: small size and resource usage
 - low dependencies: low or no external dependencies
 - terminal-focused: terminal usage focused (input and output) - primarily focused on usage through conky
 
 
 ## Latest Changes
 
-- changed --version to use importlib.metadata
+- minor cleanup of --version
+- update copyright date
 
 
 ### Notices
 
 - it does not make much sense to run this more frequently than every 10s as connecting takes ~1-2s
```

