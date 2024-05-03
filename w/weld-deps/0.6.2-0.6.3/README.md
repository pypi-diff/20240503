# Comparing `tmp/weld_deps-0.6.2.tar.gz` & `tmp/weld_deps-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weld_deps-0.6.2.tar", max compression
+gzip compressed data, was "weld_deps-0.6.3.tar", max compression
```

## Comparing `weld_deps-0.6.2.tar` & `weld_deps-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-05-01 14:36:01.293494 weld_deps-0.6.2/LICENSE
--rw-r--r--   0        0        0      333 2024-05-01 14:36:17.853628 weld_deps-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/__init__.py
--rw-r--r--   0        0        0     5879 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/dep.py
--rw-r--r--   0        0        0      423 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/examples/pack1/beet.yaml
--rw-r--r--   0        0        0        0 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
--rw-r--r--   0        0        0     1858 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/main.py
--rw-r--r--   0        0        0     4855 2024-05-01 14:36:01.293494 weld_deps-0.6.2/weld_deps/utils.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-03 08:27:22.973929 weld_deps-0.6.3/LICENSE
+-rw-r--r--   0        0        0      333 2024-05-03 08:27:40.821929 weld_deps-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-03 08:27:22.977928 weld_deps-0.6.3/weld_deps/__init__.py
+-rw-r--r--   0        0        0     5879 2024-05-03 08:27:22.977928 weld_deps-0.6.3/weld_deps/dep.py
+-rw-r--r--   0        0        0      423 2024-05-03 08:27:22.977928 weld_deps-0.6.3/weld_deps/examples/pack1/beet.yaml
+-rw-r--r--   0        0        0        0 2024-05-03 08:27:22.977928 weld_deps-0.6.3/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
+-rw-r--r--   0        0        0     1858 2024-05-03 08:27:22.977928 weld_deps-0.6.3/weld_deps/main.py
+-rw-r--r--   0        0        0     4867 2024-05-03 08:27:22.977928 weld_deps-0.6.3/weld_deps/utils.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.6.3/PKG-INFO
```

### Comparing `weld_deps-0.6.2/LICENSE` & `weld_deps-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.2/weld_deps/dep.py` & `weld_deps-0.6.3/weld_deps/dep.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.2/weld_deps/main.py` & `weld_deps-0.6.3/weld_deps/main.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.6.2/weld_deps/utils.py` & `weld_deps-0.6.3/weld_deps/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 def resolve_deps(deps: dict[Dep, list[str]], include_prerelease: bool) -> list[VersionedDep]:
     new_deps = dict()
     for dep in deps:
         # sort versions by semver
         versions = sorted(
             dep.get_versions(),
-            key=lambda v: semver.VersionInfo.parse(v.version),
+            key=lambda v: semver.VersionInfo.parse(v.version.lstrip("v")),
             reverse=True,
         )
         if not include_prerelease:
             versions = [
                 v
                 for v in versions
                 if not semver.VersionInfo.parse(v.version).prerelease
```

