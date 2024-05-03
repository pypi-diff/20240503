# Comparing `tmp/yamk-6.1.0.tar.gz` & `tmp/yamk-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamk-6.1.0.tar", max compression
+gzip compressed data, was "yamk-7.0.0.tar", max compression
```

## Comparing `yamk-6.1.0.tar` & `yamk-7.0.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     2836 2024-01-03 22:37:04.548545 yamk-6.1.0/docs/README.md
--rw-r--r--   0        0        0     3086 2024-04-02 11:33:51.761680 yamk-6.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-02 11:33:53.284982 yamk-6.1.0/src/yamk/__init__.py
--rw-r--r--   0        0        0     3942 2024-02-02 16:31:24.557219 yamk-6.1.0/src/yamk/functions.py
--rw-r--r--   0        0        0    15347 2024-04-02 11:19:46.905445 yamk-6.1.0/src/yamk/lib.py
--rw-r--r--   0        0        0     3006 2023-10-18 12:01:10.428210 yamk-6.1.0/src/yamk/main.py
--rw-r--r--   0        0        0    11159 2024-04-02 11:22:17.639095 yamk-6.1.0/src/yamk/make.py
--rw-r--r--   0        0        0        0 2023-10-18 12:01:10.428210 yamk-6.1.0/src/yamk/py.typed
--rw-r--r--   0        0        0       79 2023-10-18 12:01:10.428210 yamk-6.1.0/src/yamk/types.py
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 yamk-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-03 11:21:23.794976 yamk-7.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2840 2024-05-02 11:23:44.516277 yamk-7.0.0/docs/README.md
+-rw-r--r--   0        0        0     3151 2024-05-03 15:10:25.312296 yamk-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 15:08:18.631594 yamk-7.0.0/src/yamk/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-03 15:10:32.688809 yamk-7.0.0/src/yamk/__version__.py
+-rw-r--r--   0        0        0     3942 2024-02-02 16:31:24.557219 yamk-7.0.0/src/yamk/functions.py
+-rw-r--r--   0        0        0    15324 2024-05-03 14:06:05.138454 yamk-7.0.0/src/yamk/lib.py
+-rw-r--r--   0        0        0     3205 2024-05-03 15:08:14.535012 yamk-7.0.0/src/yamk/main.py
+-rw-r--r--   0        0        0    12243 2024-05-03 15:08:53.104213 yamk-7.0.0/src/yamk/make.py
+-rw-r--r--   0        0        0        0 2023-10-18 12:01:10.428210 yamk-7.0.0/src/yamk/py.typed
+-rw-r--r--   0        0        0       79 2023-10-18 12:01:10.428210 yamk-7.0.0/src/yamk/types.py
+-rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 yamk-7.0.0/PKG-INFO
```

### Comparing `yamk-6.1.0/docs/README.md` & `yamk-7.0.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 We realise that the modern development is a team sport, and that developers need the
 freedom to configure something that isn't optimal for their environment. Following the
 great UNIX tradition, everything in a cookbook can be locally overridden by files with
 the same extension inside a directory named `<cookbook_filename>.d/`.
 
 ## Links
 
-- [Documentation]
-- [Changelog]
+-   [Documentation]
+-   [Changelog]
 
 [test_badge]: https://github.com/spapanik/yamk/actions/workflows/tests.yml/badge.svg
 [test_url]: https://github.com/spapanik/yamk/actions/workflows/tests.yml
 [licence_badge]: https://img.shields.io/badge/license-LGPL_v3-blue.svg
 [licence_url]: https://github.com/spapanik/yamk/blob/main/docs/LICENSE.md
 [pypi_badge]: https://img.shields.io/pypi/v/yamk
 [pypi_url]: https://pypi.org/project/yamk
```

### Comparing `yamk-6.1.0/pyproject.toml` & `yamk-7.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "poetry_core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 target-version = [
-    "py38",
+    "py39",
 ]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
@@ -28,15 +28,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 
 [tool.ruff]
 src = [
     "src",
 ]
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.lint]
 select = [
     "A",
     "ARG",
     "ASYNC",
     "B",
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "yamk"
-version = "6.1.0"
+version = "7.0.0"
 description = "Yet another make"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
@@ -153,31 +153,33 @@
 
 [tool.poetry.scripts]
 yamk = "yamk.main:main"
 yam = "yamk.main:main"
 
 [tool.poetry.dependencies]
 # python version
-python = "^3.8"
+python = "^3.9"
 
 # dependencies
 dj_settings = "^5.0"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = { version = "^0.13", python = "^3.10" }
 ipython = { version = "^8.21", python = "^3.10" }
 pickleshare = { version = "^0.7", python = "^3.10" }
 pipdeptree = "^2.13"
 
 [tool.poetry.group.lint.dependencies]
 black = "^24.1"
 mypy = "^1.8"
-ruff = "^0.3"
+ruff = "^0.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0"
 pytest-cov = "^5.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.5"
+mkdocs = "^1.6"
 mkdocs-material = "^9.5"
+mkdocs-material-extensions = "^1.3"
 Pygments = "^2.17"
+pymdown-extensions = "^10.8"
```

### Comparing `yamk-6.1.0/src/yamk/functions.py` & `yamk-7.0.0/src/yamk/functions.py`

 * *Files identical despite different names*

### Comparing `yamk-6.1.0/src/yamk/lib.py` & `yamk-7.0.0/src/yamk/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import math
 import os
 import re
 import shlex
 import warnings
+from collections.abc import Iterator
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from math import ceil, floor
 from pathlib import Path
-from typing import Any, Iterator, Literal, Match, cast
+from re import Match
+from typing import Any, Literal, cast
 
 from yamk.functions import functions
 
 VAR = re.compile(
     r"(?P<dollars>\$+){(?P<variable>[a-zA-Z0-9_.]+)(?P<sep>:)?(?P<key>[a-zA-Z0-9_.]+)?}"
 )
 OPTIONS = re.compile(r"\[(?P<options>.*?)\](?P<string>.*)")
@@ -429,16 +431,16 @@
     for var_type in order:
         var_block = variables.get(var_type, {})
         parser = Parser(output, base_dir)
         for raw_key, raw_value in var_block.items():
             key = parser.evaluate(raw_key)
             key, options = extract_options(key)
             if raw_key.startswith(".") and var_type != "implicit":
-                msg = "Starting at yam 7.0, only implicit vars will be able to start with a dot (`.`)"
-                warnings.warn(msg, RemovedIn70Warning, stacklevel=1)
+                msg = "Only implicit vars can start with a dot (`.`)"
+                raise ValueError(msg)
             if key in strong_keys:
                 continue
             if "weak" in options and key in output:
                 continue
             if "strong" in options:
                 strong_keys.add(key)
             value = parser.evaluate(raw_value)
@@ -470,9 +472,9 @@
     print(
         f"{ANSIEscape.BOLD}{padding * ceil(half)}{report_title}{padding * floor(half)}{ANSIEscape.ENDC}"
     )
     for report in reports:
         report.print(cols)
 
 
-class RemovedIn70Warning(FutureWarning):
+class RemovedIn80Warning(FutureWarning):
     pass
```

### Comparing `yamk-6.1.0/src/yamk/main.py` & `yamk-7.0.0/src/yamk/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import sys
 
-from yamk import __version__
+from yamk.__version__ import __version__
 from yamk.lib import SUPPORTED_FILE_EXTENSIONS
 from yamk.make import MakeCommand
 
 sys.tracebacklimit = 0
 
 
 def parse_args() -> argparse.Namespace:
@@ -41,14 +41,20 @@
         "-d",
         "--directory",
         metavar="dir",
         default=".",
         help="the path to the directory that contains the cookbook",
     )
     parser.add_argument(
+        "-e",
+        "--echo",
+        action=argparse.BooleanOptionalAction,
+        help="a boolean flag to enable or disable the echo of the commands",
+    )
+    parser.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="rebuild all dependencies and the target",
     )
     parser.add_argument(
         "-n",
```

### Comparing `yamk-6.1.0/src/yamk/make.py` & `yamk-7.0.0/src/yamk/make.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 import argparse
 import itertools
 import pathlib
 import re
 import subprocess
 import sys
+from collections.abc import Iterator
 from time import perf_counter_ns, sleep
 from typing import Any, cast
 
 from dj_settings import ConfigParser
 
-from yamk import __version__, lib
+from yamk import lib
+from yamk.__version__ import __version__
 
 
 class MakeCommand:
     def __init__(self, args: argparse.Namespace):
         self.verbosity = args.verbose
         if self.verbosity:
             if self.verbosity > 1:
@@ -26,14 +28,15 @@
         self.aliases: dict[str, str] = {}
         self.target = args.target
         self.bare = args.bare
         self.force_make = args.force
         self.extra = args.extra
         self.retries = args.retries
         self.dry_run = args.dry_run
+        self.echo_override = args.echo
         cookbook = self.find_cookbook(args)
         self.base_dir = cookbook.parent
         self.phony_dir = self.base_dir.joinpath(".yamk")
         self.arg_vars = dict(var.split("=", maxsplit=1) for var in args.variables)
         parsed_cookbook = ConfigParser([cookbook], force_type=args.cookbook_type).data
         self.globals = parsed_cookbook.pop("$globals", {})
         self.version = self._get_version()
@@ -72,15 +75,14 @@
             self._make_target(cast(lib.Recipe, node.recipe))
         if self.print_timing_report:
             lib.print_reports(self.reports)
 
     def _run_command(self, command: str) -> int:
         status = 0
         if self.dry_run:
-            print(command)
             return status
 
         a, b = 1, 1
         total = 0
         for i in range(self.retries + 1):
             start = perf_counter_ns()
             result = subprocess.run(  # noqa: PLW1510
@@ -175,27 +177,33 @@
                 print(f"    required_by: {node.required_by}")
         return dag
 
     def _make_target(self, recipe: lib.Recipe) -> None:
         if self.verbosity > 1:
             print(f"=== target: {recipe.target} ===")
 
-        for raw_command in recipe.commands:
+        n = len(recipe.commands)
+        for i, raw_command in enumerate(recipe.commands):
             command, options = lib.extract_options(raw_command)
-            if recipe.echo or "echo" in options or self.verbosity > 2:
-                print(command)
+            should_echo = any(self._print_reasons(recipe, options))
+            if should_echo:
+                self._print_command(command)
             return_code = self._run_command(command)
+            if should_echo:
+                self._print_result(command, return_code)
             if (
                 return_code
                 and not recipe.allow_failures
                 and "allow_failures" not in options
             ):
                 if self.print_timing_report:
                     lib.print_reports(self.reports)
                 sys.exit(return_code)
+            if i != n - 1:
+                print()
         if recipe.phony and recipe.keep_ts:
             path = self._phony_path(recipe.target)
             self.phony_dir.mkdir(exist_ok=True)
             path.touch()
         if recipe.update and not recipe.phony:
             pathlib.Path(recipe.target).touch()
 
@@ -300,9 +308,29 @@
 
         if not recipe.keep_ts:
             msg = "Existence commands needs either exists_only or keep_ts"
             raise ValueError(msg)
 
         return path.stat().st_mtime
 
+    def _print_reasons(self, recipe: lib.Recipe, options: set[str]) -> Iterator[bool]:
+        yield "echo" in options
+        yield recipe.echo
+        yield self.verbosity > 2
+        yield self.echo_override
+
+    def _print_command(self, command: str) -> None:
+        bold_command = f"{lib.ANSIEscape.BOLD}`{command}`{lib.ANSIEscape.ENDC}"
+        print(f"🔧 Running {bold_command}")
+
+    def _print_result(self, command: str, return_code: int) -> None:
+        bold_command = f"{lib.ANSIEscape.BOLD}`{command}`{lib.ANSIEscape.ENDC}"
+        if return_code:
+            prefix = "❌"
+            suffix = f"failed with exit code {return_code}"
+        else:
+            prefix = "✅"
+            suffix = "run successfully!"
+        print(f"{prefix} {bold_command} {suffix}")
+
     def _get_version(self) -> lib.Version:
         return lib.Version.from_string(self.globals["version"])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yamk-6.1.0/PKG-INFO` & `yamk-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: yamk
-Version: 6.1.0
+Version: 7.0.0
 Summary: Yet another make
 Home-page: https://yamk.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: make,build,cli
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: dj_settings (>=5.0,<6.0)
 Project-URL: Documentation, https://yamk.readthedocs.io/en/stable/
@@ -64,16 +63,16 @@
 We realise that the modern development is a team sport, and that developers need the
 freedom to configure something that isn't optimal for their environment. Following the
 great UNIX tradition, everything in a cookbook can be locally overridden by files with
 the same extension inside a directory named `<cookbook_filename>.d/`.
 
 ## Links
 
-- [Documentation]
-- [Changelog]
+-   [Documentation]
+-   [Changelog]
 
 [test_badge]: https://github.com/spapanik/yamk/actions/workflows/tests.yml/badge.svg
 [test_url]: https://github.com/spapanik/yamk/actions/workflows/tests.yml
 [licence_badge]: https://img.shields.io/badge/license-LGPL_v3-blue.svg
 [licence_url]: https://github.com/spapanik/yamk/blob/main/docs/LICENSE.md
 [pypi_badge]: https://img.shields.io/pypi/v/yamk
 [pypi_url]: https://pypi.org/project/yamk
```

