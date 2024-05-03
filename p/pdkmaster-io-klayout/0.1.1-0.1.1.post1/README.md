# Comparing `tmp/pdkmaster_io_klayout-0.1.1.tar.gz` & `tmp/pdkmaster_io_klayout-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdkmaster_io_klayout-0.1.1.tar", last modified: Fri Apr 12 08:39:41 2024, max compression
+gzip compressed data, was "pdkmaster_io_klayout-0.1.1.post1.tar", last modified: Fri May  3 12:09:30 2024, max compression
```

## Comparing `pdkmaster_io_klayout-0.1.1.tar` & `pdkmaster_io_klayout-0.1.1.post1.tar`

### file list

```diff
@@ -1,17 +1,8 @@
--rw-r--r--   0        0        0      566 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSE.md
--rw-r--r--   0        0        0    34523 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    11358 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/apache-2.0.txt
--rw-r--r--   0        0        0    13419 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     2914 2024-04-12 08:24:25.396742 pdkmaster_io_klayout-0.1.1/README.md
--rw-r--r--   0        0        0      752 2024-04-12 08:39:41.499227 pdkmaster_io_klayout-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       98 2024-03-26 08:41:13.656299 pdkmaster_io_klayout-0.1.1/test/__init__.py
--rw-r--r--   0        0        0      470 2024-04-12 08:19:15.877302 pdkmaster_io_klayout-0.1.1/test/cover_report.log
--rw-r--r--   0        0        0       98 2024-03-26 08:41:16.144261 pdkmaster_io_klayout-0.1.1/test/unit/__init__.py
--rw-r--r--   0        0        0    13633 2024-04-11 13:54:22.159579 pdkmaster_io_klayout-0.1.1/test/unit/dummy.py
--rw-r--r--   0        0        0       98 2024-03-26 08:42:02.583561 pdkmaster_io_klayout-0.1.1/test/unit/io/__init__.py
--rw-r--r--   0        0        0       98 2024-02-28 17:16:25.382380 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/__init__.py
--rw-r--r--   0        0        0    14184 2024-04-11 13:54:22.159579 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/export.py
--rw-r--r--   0        0        0    20839 2024-02-28 17:16:25.382380 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/merge.py
--rw-r--r--   0        0        0     1576 2024-04-12 08:24:25.396742 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/pcell.py
--rw-r--r--   0        0        0     3253 1970-01-01 00:00:00.000000 pdkmaster_io_klayout-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:19:08.555408 pdkmaster_io_klayout-0.1.1.post1/LICENSE.md
+-rw-r--r--   0        0        0      877 2024-05-03 11:33:15.358710 pdkmaster_io_klayout-0.1.1.post1/README.md
+-rw-r--r--   0        0        0      163 2024-04-16 11:58:37.319788 pdkmaster_io_klayout-0.1.1.post1/pdkmaster/io/klayout/__init__.py
+-rw-r--r--   0        0        0    42663 2024-04-16 11:58:37.319788 pdkmaster_io_klayout-0.1.1.post1/pdkmaster/io/klayout/export.py
+-rw-r--r--   0        0        0    23312 2024-04-16 11:58:37.319788 pdkmaster_io_klayout-0.1.1.post1/pdkmaster/io/klayout/merge_.py
+-rw-r--r--   0        0        0    23033 2024-04-16 11:58:37.319788 pdkmaster_io_klayout-0.1.1.post1/pdkmaster/io/klayout/pcell.py
+-rw-r--r--   0        0        0      797 2024-05-03 12:09:30.226095 pdkmaster_io_klayout-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 pdkmaster_io_klayout-0.1.1.post1/PKG-INFO
```

### Comparing `pdkmaster_io_klayout-0.1.1/pyproject.toml` & `pdkmaster_io_klayout-0.1.1.post1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,36 +7,41 @@
 ]
 dependencies = [
     "PDKMaster~=0.11.0",
     "klayout>=0.27.13",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.1.post1"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
-[tool.pdm.resolution.overrides]
-klayout = "0.27.13"
+[tool.pdm.build]
+includes = [
+    "pdkmaster/",
+]
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "doit",
     "coverage[toml]",
     "-e file:///${PROJECT_ROOT}/deps/PDKMaster#egg=PDKMaster",
 ]
+fixed_deps = [
+    "klayout==0.27.13",
+]
 
 [tool.pdm.scripts]
 doit = "doit"
```

