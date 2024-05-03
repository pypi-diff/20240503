# Comparing `tmp/c4m_flexcell-0.4.2.post2.tar.gz` & `tmp/c4m_flexcell-0.4.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexcell-0.4.2.post2.tar", last modified: Wed Mar 27 17:29:18 2024, max compression
+gzip compressed data, was "c4m_flexcell-0.4.2.post3.tar", last modified: Fri May  3 12:37:17 2024, max compression
```

## Comparing `c4m_flexcell-0.4.2.post2.tar` & `c4m_flexcell-0.4.2.post3.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0      782 2024-02-28 17:24:49.897343 c4m_flexcell-0.4.2.post2/LICENSE.md
--rw-r--r--   0        0        0    34523 2024-02-28 17:24:49.897343 c4m_flexcell-0.4.2.post2/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    13419 2024-02-28 17:24:49.897343 c4m_flexcell-0.4.2.post2/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2024-02-28 17:24:49.897343 c4m_flexcell-0.4.2.post2/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     4467 2024-03-25 14:00:57.992581 c4m_flexcell-0.4.2.post2/README.md
--rw-r--r--   0        0        0      711 2024-03-27 17:29:18.301875 c4m_flexcell-0.4.2.post2/pyproject.toml
--rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 c4m_flexcell-0.4.2.post2/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:19:41.615267 c4m_flexcell-0.4.2.post3/LICENSE.md
+-rw-r--r--   0        0        0     4981 2024-05-03 11:33:35.310604 c4m_flexcell-0.4.2.post3/README.md
+-rw-r--r--   0        0        0     2262 2024-04-29 09:32:24.818215 c4m_flexcell-0.4.2.post3/c4m/cell_canvas.ipynb
+-rw-r--r--   0        0        0      143 2024-04-29 09:33:28.149795 c4m_flexcell-0.4.2.post3/c4m/flexcell/__init__.py
+-rw-r--r--   0        0        0     3738 2024-04-29 09:33:38.805725 c4m_flexcell-0.4.2.post3/c4m/flexcell/_waiters.py
+-rw-r--r--   0        0        0    90310 2024-04-29 09:33:50.801646 c4m_flexcell-0.4.2.post3/c4m/flexcell/activecolumnscell.py
+-rw-r--r--   0        0        0    13887 2024-04-29 09:34:00.277583 c4m_flexcell-0.4.2.post3/c4m/flexcell/canvas.py
+-rw-r--r--   0        0        0     4311 2024-04-29 09:35:27.017016 c4m_flexcell-0.4.2.post3/c4m/flexcell/cell.py
+-rw-r--r--   0        0        0   132114 2024-04-29 09:35:36.280955 c4m_flexcell-0.4.2.post3/c4m/flexcell/factory.py
+-rw-r--r--   0        0        0      698 2024-05-03 12:37:17.628607 c4m_flexcell-0.4.2.post3/pyproject.toml
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 c4m_flexcell-0.4.2.post3/PKG-INFO
```

### Comparing `c4m_flexcell-0.4.2.post2/README.md` & `c4m_flexcell-0.4.2.post3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,7 +28,15 @@
 In future options are planned so libraries can be generated for different targets like ,minimum area, maximum performance or minimum power consumption.
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever.  
 Current implementation is based on the topology of the Coriolis nsxlib standard cells with some area improvements but not yet with optimal area use. For v0.1 of this library a total replacement of the layout generation is planned fully based on minimized area for the technology design rules.  
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

### Comparing `c4m_flexcell-0.4.2.post2/pyproject.toml` & `c4m_flexcell-0.4.2.post3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,36 +6,39 @@
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
     "PDKMaster>=0.10.2,<0.12.0",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.4.2.post2"
+version = "0.4.2.post3"
 
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

### Comparing `c4m_flexcell-0.4.2.post2/PKG-INFO` & `c4m_flexcell-0.4.2.post3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexcell
-Version: 0.4.2.post2
+Version: 0.4.2.post3
 Summary: PDKMaster based scalable standard cell library
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster<0.12.0,>=0.10.2
 Description-Content-Type: text/markdown
 
@@ -38,7 +38,15 @@
 In future options are planned so libraries can be generated for different targets like ,minimum area, maximum performance or minimum power consumption.
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever.  
 Current implementation is based on the topology of the Coriolis nsxlib standard cells with some area improvements but not yet with optimal area use. For v0.1 of this library a total replacement of the layout generation is planned fully based on minimized area for the technology design rules.  
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

