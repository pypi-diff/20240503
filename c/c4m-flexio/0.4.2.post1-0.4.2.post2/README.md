# Comparing `tmp/c4m_flexio-0.4.2.post1.tar.gz` & `tmp/c4m_flexio-0.4.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexio-0.4.2.post1.tar", last modified: Wed Mar 27 17:31:15 2024, max compression
+gzip compressed data, was "c4m_flexio-0.4.2.post2.tar", last modified: Fri May  3 12:54:42 2024, max compression
```

## Comparing `c4m_flexio-0.4.2.post1.tar` & `c4m_flexio-0.4.2.post2.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0      336 2024-02-28 17:27:49.862357 c4m_flexio-0.4.2.post1/LICENSE.md
--rw-r--r--   0        0        0    18009 2024-02-28 17:27:49.862357 c4m_flexio-0.4.2.post1/LICENSES/GPL-2.0.txt
--rw-r--r--   0        0        0    13419 2024-02-28 17:27:49.862357 c4m_flexio-0.4.2.post1/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0     1998 2024-03-25 14:00:58.076579 c4m_flexio-0.4.2.post1/README.md
--rw-r--r--   0        0        0      725 2024-03-27 17:31:15.976111 c4m_flexio-0.4.2.post1/pyproject.toml
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 c4m_flexio-0.4.2.post1/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:19:56.775201 c4m_flexio-0.4.2.post2/LICENSE.md
+-rw-r--r--   0        0        0     2611 2024-05-03 11:33:55.090498 c4m_flexio-0.4.2.post2/README.md
+-rw-r--r--   0        0        0      170 2024-04-29 09:44:39.473491 c4m_flexio-0.4.2.post2/c4m/flexio/__init__.py
+-rw-r--r--   0        0        0    18938 2024-04-29 09:49:22.507719 c4m_flexio-0.4.2.post2/c4m/flexio/_helpers.py
+-rw-r--r--   0        0        0   104325 2024-04-29 09:48:37.619999 c4m_flexio-0.4.2.post2/c4m/flexio/cell.py
+-rw-r--r--   0        0        0   236159 2024-04-29 09:49:02.035846 c4m_flexio-0.4.2.post2/c4m/flexio/factory.py
+-rw-r--r--   0        0        0    37990 2024-04-29 09:49:14.995766 c4m_flexio-0.4.2.post2/c4m/flexio/specification.py
+-rw-r--r--   0        0        0      712 2024-05-03 12:54:42.446697 c4m_flexio-0.4.2.post2/pyproject.toml
+-rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 c4m_flexio-0.4.2.post2/PKG-INFO
```

### Comparing `c4m_flexio-0.4.2.post1/README.md` & `c4m_flexio-0.4.2.post2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: c4m-flexio
+Version: 0.4.2.post2
+Summary: PDKMaster based scalable IO library
+Author: Chips4Makers contributors
+License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
+Requires-Python: ~=3.8
+Requires-Dist: PDKMaster<0.12.0,>=0.10.2
+Requires-Dist: c4m-flexcell~=0.4.2
+Description-Content-Type: text/markdown
+
 # Flexible, scalable, IO library
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
@@ -21,9 +32,18 @@
   and updated for the latest version of PDKMaster and c4m-flexcell.
 * v0.3.1: no code change; mark IO cell code compatible with dev v0.4.0 of c4m-flexcell
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * no notes for older releases
 
 ## Status
 
-This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever. The library now progresses at the need of tape-outs.
+This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever. The library now progresses at the need of other related projects. It has been used to generate
+a set of IO cells for the open source IHPSG13G2 process.
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
+
+## Project Arrakeen subproject
+
+This project is part of Chips4Makers' [project Arrakeen](https://gitlab.com/Chips4Makers/c4m-arrakeen). It shares some common guide lines and regulations:
+
+* [Contributing.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/Contributing.md)
+* [LICENSE.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE.md): license of release code
+* [LICENSE_rationale.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE_rationale.md)
```

### Comparing `c4m_flexio-0.4.2.post1/pyproject.toml` & `c4m_flexio-0.4.2.post2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 ]
 dependencies = [
     "PDKMaster>=0.10.2,<0.12.0",
     "c4m-flexcell~=0.4.2",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.4.2.post1"
+version = "0.4.2.post2"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
-    "dunamai",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 ignore_package_warnings = [
     "*",
 ]
 distribution = true
 
+[tool.pdm.build]
+includes = [
+    "c4m/",
+]
+
 [tool.pdm.version]
-source = "call"
-getter = "scripts.version:get_version"
+source = "scm"
 
 [tool.pdm.dev-dependencies]
-dev = [
-    "dunamai",
+dev = []
+vscode = [
     "pip",
     "docutils",
     "esbonio",
 ]
```

### Comparing `c4m_flexio-0.4.2.post1/PKG-INFO` & `c4m_flexio-0.4.2.post2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: c4m-flexio
-Version: 0.4.2.post1
-Summary: PDKMaster based scalable IO library
-Author: Chips4Makers contributors
-License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
-Requires-Python: ~=3.8
-Requires-Dist: PDKMaster<0.12.0,>=0.10.2
-Requires-Dist: c4m-flexcell~=0.4.2
-Description-Content-Type: text/markdown
-
 # Flexible, scalable, IO library
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
@@ -32,9 +21,18 @@
   and updated for the latest version of PDKMaster and c4m-flexcell.
 * v0.3.1: no code change; mark IO cell code compatible with dev v0.4.0 of c4m-flexcell
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * no notes for older releases
 
 ## Status
 
-This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever. The library now progresses at the need of tape-outs.
+This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever. The library now progresses at the need of other related projects. It has been used to generate
+a set of IO cells for the open source IHPSG13G2 process.
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
+
+## Project Arrakeen subproject
+
+This project is part of Chips4Makers' [project Arrakeen](https://gitlab.com/Chips4Makers/c4m-arrakeen). It shares some common guide lines and regulations:
+
+* [Contributing.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/Contributing.md)
+* [LICENSE.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE.md): license of release code
+* [LICENSE_rationale.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE_rationale.md)
```

