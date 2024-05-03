# Comparing `tmp/poetry_plugin_mono_repo_deps-0.2.0.tar.gz` & `tmp/poetry_plugin_mono_repo_deps-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_mono_repo_deps-0.2.0.tar", max compression
+gzip compressed data, was "poetry_plugin_mono_repo_deps-0.2.1.tar", max compression
```

## Comparing `poetry_plugin_mono_repo_deps-0.2.0.tar` & `poetry_plugin_mono_repo_deps-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1070 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/LICENSE
--rw-r--r--   0        0        0     7442 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/README.md
--rw-r--r--   0        0        0       69 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/poetry_plugin_mono_repo_deps/__init__.py
--rw-r--r--   0        0        0       22 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/poetry_plugin_mono_repo_deps/_version.py
--rw-r--r--   0        0        0     8408 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/poetry_plugin_mono_repo_deps/plugin.py
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/poetry_plugin_mono_repo_deps/py.typed
--rw-r--r--   0        0        0     2851 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3044 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1171 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-a/lib_a/__init__.py
--rw-r--r--   0        0        0     1103 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-a/poetry.lock
--rw-r--r--   0        0        0      337 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-a/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-auto-enabled/lib_auto_enabled/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-auto-enabled/poetry.lock
--rw-r--r--   0        0        0      423 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-auto-enabled/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-disabled/lib_disabled/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-disabled/poetry.lock
--rw-r--r--   0        0        0      420 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-disabled/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled/lib_enabled/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled/poetry.lock
--rw-r--r--   0        0        0      433 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-extras/lib_enabled_extras/__init__.py
--rw-r--r--   0        0        0     4883 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-extras/poetry.lock
--rw-r--r--   0        0        0      460 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-extras/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-no-commands/lib_enabled_no_commands/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-no-commands/poetry.lock
--rw-r--r--   0        0        0      459 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-no-commands/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-independent/lib_independent/__init__.py
--rw-r--r--   0        0        0      244 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-independent/poetry.lock
--rw-r--r--   0        0        0      311 2024-04-12 19:20:25.511248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-independent/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 19:20:25.515248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-missing/lib_missing/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-12 19:20:25.515248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-missing/poetry.lock
--rw-r--r--   0        0        0      423 2024-04-12 19:20:25.515248 poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-missing/pyproject.toml
--rw-r--r--   0        0        0     6334 2024-04-12 19:20:25.515248 poetry_plugin_mono_repo_deps-0.2.0/tests/helpers.py
--rw-r--r--   0        0        0     4071 2024-04-12 19:20:25.515248 poetry_plugin_mono_repo_deps-0.2.0/tests/test_commands_e2e.py
--rw-r--r--   0        0        0     2777 2024-04-12 19:20:25.515248 poetry_plugin_mono_repo_deps-0.2.0/tests/test_plugin.py
--rw-r--r--   0        0        0     8518 1970-01-01 00:00:00.000000 poetry_plugin_mono_repo_deps-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 06:40:57.168273 poetry_plugin_mono_repo_deps-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7442 2024-05-03 06:40:57.168273 poetry_plugin_mono_repo_deps-0.2.1/README.md
+-rw-r--r--   0        0        0       69 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/poetry_plugin_mono_repo_deps/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/poetry_plugin_mono_repo_deps/_version.py
+-rw-r--r--   0        0        0     8453 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/poetry_plugin_mono_repo_deps/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/poetry_plugin_mono_repo_deps/py.typed
+-rw-r--r--   0        0        0     2851 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3044 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1171 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-a/lib_a/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-a/poetry.lock
+-rw-r--r--   0        0        0      337 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-a/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-auto-enabled/lib_auto_enabled/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-auto-enabled/poetry.lock
+-rw-r--r--   0        0        0      423 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-auto-enabled/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-disabled/lib_disabled/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-disabled/poetry.lock
+-rw-r--r--   0        0        0      420 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-disabled/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled/lib_enabled/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled/poetry.lock
+-rw-r--r--   0        0        0      433 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-extras/lib_enabled_extras/__init__.py
+-rw-r--r--   0        0        0     4883 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-extras/poetry.lock
+-rw-r--r--   0        0        0      460 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-extras/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-no-commands/lib_enabled_no_commands/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-no-commands/poetry.lock
+-rw-r--r--   0        0        0      459 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-no-commands/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-independent/lib_independent/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-independent/poetry.lock
+-rw-r--r--   0        0        0      311 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-independent/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-missing/lib_missing/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-missing/poetry.lock
+-rw-r--r--   0        0        0      423 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-missing/pyproject.toml
+-rw-r--r--   0        0        0     7261 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/helpers.py
+-rw-r--r--   0        0        0     5204 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/test_commands_e2e.py
+-rw-r--r--   0        0        0     2777 2024-05-03 06:40:57.172273 poetry_plugin_mono_repo_deps-0.2.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     8518 1970-01-01 00:00:00.000000 poetry_plugin_mono_repo_deps-0.2.1/PKG-INFO
```

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/LICENSE` & `poetry_plugin_mono_repo_deps-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/README.md` & `poetry_plugin_mono_repo_deps-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 ```{toml}
 [tool.poetry-monorepo.deps]
 enabled = true
 commands = ["build", "export"]
 constraint = "~="
 source_types = ["file", "directory"]
-only_develop = False
+only_develop = false
 ```
 
 Possible alternative values can be found in the following section:
 
 ## Configuration:
 
 ### `enabled`
```

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/poetry_plugin_mono_repo_deps/plugin.py` & `poetry_plugin_mono_repo_deps-0.2.1/poetry_plugin_mono_repo_deps/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Any, Dict, List, TypeVar, cast
 
 from cleo.events.console_event import ConsoleEvent
 from cleo.events.console_events import COMMAND
 from cleo.events.event import Event
 from cleo.events.event_dispatcher import EventDispatcher
 from cleo.io.io import IO
-from cleo.io.null_io import NullIO
 from poetry.console.application import Application
 from poetry.core.packages.dependency import Dependency
 from poetry.core.packages.package import Package
 from poetry.plugins.application_plugin import ApplicationPlugin
 from poetry.poetry import Poetry
 from poetry.repositories.lockfile_repository import LockfileRepository
 from poetry.utils.helpers import merge_dicts
@@ -80,70 +79,72 @@
     else:
         return None
 
 
 class MonoRepoDepsPlugin(ApplicationPlugin):
     def __init__(self) -> None:
         super().__init__()
-        self._config: Config | None = None
 
     def activate(self, application: Application) -> None:
         self._application = application
-        self._poetry = self._application.poetry
-        self._config = load_config(self._poetry)
-        self._is_disabled = self._config is None
-
-        io = self._application._io or NullIO()
-        if self._is_disabled:
-            if io.is_debug():  # pragma: no cover
-                io.write_line(
-                    "<debug>Not replacing path dependencies by named dependencies as no tool configuration section "
-                    "found.</debug>"
-                )
-            return
         dispatcher = application.event_dispatcher
         if dispatcher is not None:
             dispatcher.add_listener(COMMAND, self.handle_command)
         else:  # pragma: no cover
             pass
 
     def handle_command(self, event: Event, _event_name: str, _dispatcher: EventDispatcher) -> None:
-        if self._config is None:  # pragma: no cover
+        try:
+            poetry = self._application.poetry
+        except RuntimeError:
+            # should only happen if poetry runs outside poetry folder structure
+            # as we modify poetry lock files, the plugin can only work in poetry folders
+            # and is only relevant for commands that work in poetry folders
+            # thus, either the command is not relevant
+            # or, the command would fail itself
             return
+
+        config = load_config(poetry)
+
         event = cast(ConsoleEvent, event)  # because we listen to COMMANDs
         io = event.io
+        if config is None:  # pragma: no cover
+            if io.is_debug():  # pragma: no cover
+                io.write_line(
+                    "<debug>Not replacing path dependencies by named dependencies as no tool configuration section "
+                    "found.</debug>"
+                )
+            return
         command = event.command
-        if command.name not in self._config.commands:
+        if command.name not in config.commands:
             if io.is_debug():  # pragma: no cover
                 io.write_line(
                     "<debug>Not replacing path dependencies with named dependencies for command "
                     f"{command.name}.</debug>"
                 )
             return
 
         if io.is_debug():  # pragma: no cover
             io.write_line("<debug>Replacing path dependencies with named dependencies.</debug>")
 
         # for build
-        self.update_locked_repository(io)
+        self.update_locked_repository(io, config)
         # for export
-        self.update_lock_data()
+        self.update_lock_data(config)
         return None
 
-    def update_locked_repository(self, io: IO) -> None:
+    def update_locked_repository(self, io: IO, config: Config) -> None:
         """Updates the lockers locked repository, necessary for commands like `build`"""
-        if self._config is None:  # pragma: no cover
-            return
-        constraint = self._config.constraint
+        constraint = config.constraint
         poetry = self._application.poetry
         locked_repository = poetry._locker.locked_repository()
         for name in poetry.package.dependency_group_names():
             group = poetry.package.dependency_group(name)
             for dep in group.dependencies:
-                if is_to_be_replaced_dependency(self._config, dep):
+                if is_to_be_replaced_dependency(config, dep):
                     name = dep.name
                     # get the locked package to retrieve the current version
                     package = find_package(locked_repository, name)
                     if package is not None:
                         new = create_named_dependency(constraint, dep, package)
                         # new = Dependency(name, version or "*", extras=dep.extras)
                         io.write_line(
@@ -151,22 +152,20 @@
                             f"{group.name} with {new.to_pep_508()}"
                         )
                         group.remove_dependency(name)
                         group.add_dependency(new)
                     else:  # pragma: no cover
                         io.write_error_line(f"Failed to find version for path dependency {name}")
 
-    def update_lock_data(self) -> None:
+    def update_lock_data(self, config: Config) -> None:
         """Updates the lockers internal lock data, necessary for commands like `export`"""
-        if self._config is None:  # pragma: no cover
-            return
         poetry = self._application.poetry
         locked_packages = cast(List[Dict[str, Any]], poetry._locker.lock_data["package"])
         for info in locked_packages:
-            if is_to_be_replaced_package(self._config, info):
+            if is_to_be_replaced_package(config, info):
                 modify_locked_package_to_named(info)
 
 
 def is_to_be_replaced_package(config: Config, locked_package_data: dict[str, Any]) -> bool:
     source = locked_package_data.get("source", {})
     source_type = source.get("type")
     can_be_develop = source_type == "directory"
```

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/pyproject.toml` & `poetry_plugin_mono_repo_deps-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.commitizen]
 bump_message = "bump: $current_version → $new_version"
 changelog_incremental = true
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.2.0"
+version = "0.2.1"
 version_files = [
   "VERSION",
   "pyproject.toml:^version = ",
   "poetry_plugin_mono_repo_deps/_version.py:^__version"
 ]
 
 [tool.coverage.report]
@@ -71,15 +71,15 @@
 license = "MIT"
 name = "poetry-plugin-mono-repo-deps"
 packages = [
   {include = "poetry_plugin_mono_repo_deps"}
 ]
 readme = "README.md"
 repository = "https://github.com/gerbenoostra/poetry-plugin-mono-repo-deps"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 poetry = "^1.7.0"
 poetry-core = "^1.7.0"
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/conftest.py` & `poetry_plugin_mono_repo_deps-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/__init__.py` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-a/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-a/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-auto-enabled/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-auto-enabled/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-disabled/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-disabled/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-extras/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-extras/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-enabled-no-commands/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-enabled-no-commands/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/fixtures/simple_a/lib-missing/poetry.lock` & `poetry_plugin_mono_repo_deps-0.2.1/tests/fixtures/simple_a/lib-missing/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/helpers.py` & `poetry_plugin_mono_repo_deps-0.2.1/tests/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from io import StringIO
 from pathlib import Path
 from typing import Any
 
 from cleo.commands.command import Command
 from cleo.io.inputs.argv_input import ArgvInput
+from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
 from cleo.io.outputs.stream_output import StreamOutput
 from cleo.testers.command_tester import CommandTester
 from poetry.console.application import Application
 from poetry.core.packages.package import Package
 from poetry.factory import Factory
 from poetry.installation import Installer
@@ -174,25 +175,57 @@
     poetry._locker = locker
     return poetry
 
 
 export_warning = "Warning: poetry-plugin-export will not be installed by default in a future version of Poetry.\nIn order to avoid a breaking change and make your automation forward-compatible, please install poetry-plugin-export explicitly. See https://python-poetry.org/docs/plugins/#using-plugins for details on how to install a plugin.\nTo disable this warning run 'poetry config warnings.export false'.\n"  # noqa: E501 Line too long
 
 
+def run_test_app(args: list[str]) -> tuple[str, str]:
+    test_app = Application()
+
+    out = StringIO()
+    err = StringIO()
+    out_stream = StreamOutput(out)
+    out_stream.set_verbosity(Verbosity.DEBUG)
+    err_stream = StreamOutput(err)
+    instr = ArgvInput(args)
+    io = IO(instr, out_stream, err_stream)
+    test_app._load_plugins(io)
+    test_app.auto_exits(False)
+    test_app.run(
+        instr,
+        out_stream,
+        err_stream,
+    )
+    out_stream.flush()
+    err_stream.flush()
+    out_value = out.getvalue()
+    _logger.info(out_value)
+    err_value = err.getvalue()
+    _logger.error(err_value)
+    err_value = err_value.replace(export_warning, "")
+    err_value = os.linesep.join(
+        [line for line in err_value.splitlines() if not line.startswith("Creating virtualenv ")]
+    )
+    return out_value, err_value
+
+
 class AppRunner:
-    def __init__(self, app: PoetryTestApplication) -> None:
+    def __init__(self, app: Application) -> None:
         self._test_app = app
 
     def run(self, args: list[str]) -> tuple[str, str]:
         out = StringIO()
         err = StringIO()
         out_stream = StreamOutput(out)
         err_stream = StreamOutput(err)
+        instr = ArgvInput(args)
+        instr.bind(self._test_app.definition)
         self._test_app.run(
-            ArgvInput(args),
+            instr,
             out_stream,
             err_stream,
         )
         out_stream.flush()
         err_stream.flush()
         out_value = out.getvalue()
         _logger.info(out_value)
```

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/tests/test_plugin.py` & `poetry_plugin_mono_repo_deps-0.2.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_mono_repo_deps-0.2.0/PKG-INFO` & `poetry_plugin_mono_repo_deps-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-mono-repo-deps
-Version: 0.2.0
+Version: 0.2.1
 Summary: Poetry plugin to replace path dependencies in mono repos with named dependency specifications at build time
 Home-page: https://github.com/gerbenoostra/poetry-plugin-mono-repo-deps
 License: MIT
 Keywords: packaging,poetry
 Author: Gerben Oostra
 Author-email: ynnx1wmd@duck.com
 Requires-Python: >=3.8,<4.0
@@ -132,15 +132,15 @@
 
 ```{toml}
 [tool.poetry-monorepo.deps]
 enabled = true
 commands = ["build", "export"]
 constraint = "~="
 source_types = ["file", "directory"]
-only_develop = False
+only_develop = false
 ```
 
 Possible alternative values can be found in the following section:
 
 ## Configuration:
 
 ### `enabled`
```

