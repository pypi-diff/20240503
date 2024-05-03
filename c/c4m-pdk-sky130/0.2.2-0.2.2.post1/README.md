# Comparing `tmp/c4m_pdk_sky130-0.2.2.tar.gz` & `tmp/c4m_pdk_sky130-0.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_sky130-0.2.2.tar", last modified: Tue Apr 16 16:58:36 2024, max compression
+gzip compressed data, was "c4m_pdk_sky130-0.2.2.post1.tar", last modified: Fri May  3 14:44:03 2024, max compression
```

## Comparing `c4m_pdk_sky130-0.2.2.tar` & `c4m_pdk_sky130-0.2.2.post1.tar`

### file list

```diff
@@ -1,10 +1,52 @@
--rw-r--r--   0        0        0      526 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSE.md
--rw-r--r--   0        0        0    34523 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    10172 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/apache-2.0.txt
--rw-r--r--   0        0        0    13419 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     2119 2024-04-16 16:55:29.047553 c4m_pdk_sky130-0.2.2/README.md
--rw-r--r--   0        0        0       85 2024-04-16 12:02:53.752097 c4m_pdk_sky130-0.2.2/doitlib/__init__.py
--rw-r--r--   0        0        0      139 2024-04-16 12:02:53.752097 c4m_pdk_sky130-0.2.2/doitlib/libs.py
--rw-r--r--   0        0        0     1369 2024-04-16 16:58:36.316875 c4m_pdk_sky130-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 c4m_pdk_sky130-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:22:23.310531 c4m_pdk_sky130-0.2.2.post1/LICENSE.md
+-rw-r--r--   0        0        0     2633 2024-05-03 14:25:07.572923 c4m_pdk_sky130-0.2.2.post1/README.md
+-rw-r--r--   0        0        0      315 2024-04-29 10:11:31.106732 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/__init__.py
+-rw-r--r--   0        0        0    60159 2024-04-29 10:11:43.994644 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/_layout.py
+-rw-r--r--   0        0        0    11295 2024-04-29 10:12:48.482207 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/_simulation.py
+-rw-r--r--   0        0        0    27934 2024-04-29 10:13:10.066061 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/factory.py
+-rw-r--r--   0        0        0     3753 2024-04-29 10:13:19.969994 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/io.py
+-rw-r--r--   0        0        0      517 2024-04-29 10:13:30.205926 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/klayout.py
+-rw-r--r--   0        0        0     2820 2024-05-03 14:44:02.670764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_all_lib.spice
+-rw-r--r--   0        0        0      518 2024-05-03 14:44:02.638764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_ff_params.spice
+-rw-r--r--   0        0        0      509 2024-05-03 14:44:02.638764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_fs_params.spice
+-rw-r--r--   0        0        0      534 2024-05-03 14:44:02.666764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_lib.spice
+-rw-r--r--   0        0        0     2830 2024-05-03 14:44:02.634764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_model.spice
+-rw-r--r--   0        0        0      504 2024-05-03 14:44:02.642764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_sf_params.spice
+-rw-r--r--   0        0        0      506 2024-05-03 14:44:02.638764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_ss_params.spice
+-rw-r--r--   0        0        0      521 2024-05-03 14:44:02.634764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_diode_tt_params.spice
+-rw-r--r--   0        0        0  1078460 2024-05-03 14:44:02.626764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_io_ff_model.spice
+-rw-r--r--   0        0        0  1072700 2024-05-03 14:44:02.630764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_io_fs_model.spice
+-rw-r--r--   0        0        0      323 2024-05-03 14:44:02.662764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_io_lib.spice
+-rw-r--r--   0        0        0  1073656 2024-05-03 14:44:02.634764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_io_sf_model.spice
+-rw-r--r--   0        0        0  1076533 2024-05-03 14:44:02.626764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_io_ss_model.spice
+-rw-r--r--   0        0        0  1074160 2024-05-03 14:44:02.622764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_io_tt_model.spice
+-rw-r--r--   0        0        0     1003 2024-05-03 14:44:02.670764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_lib.spice
+-rw-r--r--   0        0        0  3790415 2024-05-03 14:44:02.606764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_logic_ff_model.spice
+-rw-r--r--   0        0        0  3787892 2024-05-03 14:44:02.614764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_logic_fs_model.spice
+-rw-r--r--   0        0        0      341 2024-05-03 14:44:02.662764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_logic_lib.spice
+-rw-r--r--   0        0        0  3790740 2024-05-03 14:44:02.618764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_logic_sf_model.spice
+-rw-r--r--   0        0        0  3785053 2024-05-03 14:44:02.610764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_logic_ss_model.spice
+-rw-r--r--   0        0        0  3778265 2024-05-03 14:44:02.602764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_logic_tt_model.spice
+-rw-r--r--   0        0        0     2390 2024-05-03 14:44:02.662764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_mim_model.spice
+-rw-r--r--   0        0        0      148 2024-05-03 14:44:02.650764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_npn_f_params.spice
+-rw-r--r--   0        0        0      417 2024-05-03 14:44:02.666764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_npn_lib.spice
+-rw-r--r--   0        0        0     5668 2024-05-03 14:44:02.646764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_npn_model.spice
+-rw-r--r--   0        0        0      149 2024-05-03 14:44:02.650764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_npn_s_params.spice
+-rw-r--r--   0        0        0      145 2024-05-03 14:44:02.650764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_npn_t_params.spice
+-rw-r--r--   0        0        0      149 2024-05-03 14:44:02.646764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_pnp_f_params.spice
+-rw-r--r--   0        0        0      309 2024-05-03 14:44:02.666764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_pnp_lib.spice
+-rw-r--r--   0        0        0     4887 2024-05-03 14:44:02.642764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_pnp_model.spice
+-rw-r--r--   0        0        0      144 2024-05-03 14:44:02.646764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_pnp_s_params.spice
+-rw-r--r--   0        0        0      144 2024-05-03 14:44:02.642764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_pnp_t_params.spice
+-rw-r--r--   0        0        0      823 2024-05-03 14:44:02.654764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_common_params.spice
+-rw-r--r--   0        0        0      527 2024-05-03 14:44:02.658764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_hh_params.spice
+-rw-r--r--   0        0        0      492 2024-05-03 14:44:02.658764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_hl_params.spice
+-rw-r--r--   0        0        0      483 2024-05-03 14:44:02.658764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_lh_params.spice
+-rw-r--r--   0        0        0      509 2024-05-03 14:44:02.654764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_ll_params.spice
+-rw-r--r--   0        0        0     1351 2024-05-03 14:44:02.658764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_model.spice
+-rw-r--r--   0        0        0      449 2024-05-03 14:44:02.654764 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/models/C4M.Sky130_rc_tt_params.spice
+-rw-r--r--   0        0        0    20591 2024-04-29 10:13:40.421857 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/pdkmaster.py
+-rw-r--r--   0        0        0     4095 2024-04-29 10:14:19.181597 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/pyspice.py
+-rw-r--r--   0        0        0     1265 2024-04-29 10:14:29.957525 c4m_pdk_sky130-0.2.2.post1/c4m/pdk/sky130/stdcell.py
+-rw-r--r--   0        0        0     1444 2024-05-03 14:44:03.838758 c4m_pdk_sky130-0.2.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 c4m_pdk_sky130-0.2.2.post1/PKG-INFO
```

### Comparing `c4m_pdk_sky130-0.2.2/README.md` & `c4m_pdk_sky130-0.2.2.post1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,7 +15,15 @@
 * v0.1.4: No code changes; update dependencies for latest bug fixes
 * v0.1.3: No code change; use PDKMaster 0.9.2 to get Coriolis export compatible with namespace of
   latest Coriolis release.
 * v0.1.2: Fix Coriolis export.
 * v0.1.1: No code change; release files now built by CI.
 * v0.1.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * no notes for older releases
+
+## Project Arrakeen subproject
+
+This project is part of Chips4Makers' [project Arrakeen](https://gitlab.com/Chips4Makers/c4m-arrakeen). It shares some common guide lines and regulations:
+
+* [Contributing.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/Contributing.md)
+* [LICENSE.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE.md): license of release code
+* [LICENSE_rationale.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE_rationale.md)
```

### Comparing `c4m_pdk_sky130-0.2.2/pyproject.toml` & `c4m_pdk_sky130-0.2.2.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 name = "c4m-pdk-sky130"
 dynamic = []
 description = "PDKMaster based PDK for open source GF180MCU process"
 authors = [
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
-    "PDKMaster~=0.11.0",
-    "pdkmaster-io-klayout~=0.1.1",
-    "c4m-flexcell~=0.4.2",
-    "c4m-flexio~=0.4.2",
+    "PDKMaster~=0.11.0.post2",
+    "pdkmaster-io-klayout~=0.1.1.post1",
+    "c4m-flexcell~=0.4.2.post3",
+    "c4m-flexio~=0.4.2.post2",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.2.post1"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -26,14 +26,19 @@
 
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
 source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "-e file:///${PROJECT_ROOT}/deps/PySpice#egg=PySpice",
     "-e file:///${PROJECT_ROOT}/deps/PDKMaster#egg=PDKMaster",
```

### Comparing `c4m_pdk_sky130-0.2.2/PKG-INFO` & `c4m_pdk_sky130-0.2.2.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-sky130
-Version: 0.2.2
+Version: 0.2.2.post1
 Summary: PDKMaster based PDK for open source GF180MCU process
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
-Requires-Dist: PDKMaster~=0.11.0
-Requires-Dist: pdkmaster-io-klayout~=0.1.1
-Requires-Dist: c4m-flexcell~=0.4.2
-Requires-Dist: c4m-flexio~=0.4.2
+Requires-Dist: PDKMaster~=0.11.0.post2
+Requires-Dist: pdkmaster-io-klayout~=0.1.1.post1
+Requires-Dist: c4m-flexcell~=0.4.2.post3
+Requires-Dist: c4m-flexio~=0.4.2.post2
 Description-Content-Type: text/markdown
 
 # PDKMaster based Sky130 PDK
 
 This is the PDK for Sky130 based on the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It currently is basically undocumented. Development is driven by sky130 MPW shuttle development.
 A little more information on what is possible can be found in the `.gitlab-ci.yml` file.
 
@@ -28,7 +28,15 @@
 * v0.1.4: No code changes; update dependencies for latest bug fixes
 * v0.1.3: No code change; use PDKMaster 0.9.2 to get Coriolis export compatible with namespace of
   latest Coriolis release.
 * v0.1.2: Fix Coriolis export.
 * v0.1.1: No code change; release files now built by CI.
 * v0.1.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * no notes for older releases
+
+## Project Arrakeen subproject
+
+This project is part of Chips4Makers' [project Arrakeen](https://gitlab.com/Chips4Makers/c4m-arrakeen). It shares some common guide lines and regulations:
+
+* [Contributing.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/Contributing.md)
+* [LICENSE.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE.md): license of release code
+* [LICENSE_rationale.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE_rationale.md)
```

