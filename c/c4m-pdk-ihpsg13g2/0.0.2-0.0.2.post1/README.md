# Comparing `tmp/c4m_pdk_ihpsg13g2-0.0.2.tar.gz` & `tmp/c4m_pdk_ihpsg13g2-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.2.tar", last modified: Tue Apr 16 15:59:57 2024, max compression
+gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.2.post1.tar", last modified: Fri May  3 15:17:34 2024, max compression
```

## Comparing `c4m_pdk_ihpsg13g2-0.0.2.tar` & `c4m_pdk_ihpsg13g2-0.0.2.post1.tar`

### file list

```diff
@@ -1,10 +1,27 @@
--rw-r--r--   0        0        0      566 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSE.md
--rw-r--r--   0        0        0    34523 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    11358 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/apache-2.0.txt
--rw-r--r--   0        0        0    13419 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     7408 2024-04-16 15:44:57.688258 c4m_pdk_ihpsg13g2-0.0.2/README.md
--rw-r--r--   0        0        0    24621 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/dodo.py
--rw-r--r--   0        0        0     1488 2024-04-16 15:59:57.490877 c4m_pdk_ihpsg13g2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-16 15:59:57.490877 c4m_pdk_ihpsg13g2-0.0.2/version.txt
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      992 2024-04-29 12:22:37.734462 c4m_pdk_ihpsg13g2-0.0.2.post1/LICENSE.md
+-rw-r--r--   0        0        0     5389 2024-05-03 14:55:33.303077 c4m_pdk_ihpsg13g2-0.0.2.post1/README.md
+-rw-r--r--   0        0        0      449 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/__init__.py
+-rw-r--r--   0        0        0     4572 2024-04-29 11:09:33.917013 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/_io_compliance.py
+-rw-r--r--   0        0        0     6918 2024-04-29 11:12:09.911800 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/io.py
+-rw-r--r--   0        0        0      517 2024-04-29 11:12:20.003724 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/klayout.py
+-rw-r--r--   0        0        0       23 2024-05-03 15:17:33.895843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/__init__.py
+-rw-r--r--   0        0        0      775 2024-05-03 15:17:33.915843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/all.spice
+-rw-r--r--   0        0        0    24555 2024-05-03 15:17:33.907843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib
+-rw-r--r--   0        0        0    22926 2024-05-03 15:17:33.903843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib
+-rw-r--r--   0        0        0     2460 2024-05-03 15:17:33.911843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/cornerRES.lib
+-rw-r--r--   0        0        0     3580 2024-05-03 15:17:33.915843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/diodes.lib
+-rw-r--r--   0        0        0     1900 2024-05-03 15:17:33.907843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_mod.lib
+-rw-r--r--   0        0        0     1039 2024-05-03 15:17:33.911843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_parm.lib
+-rw-r--r--   0        0        0     1045 2024-05-03 15:17:33.911843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/resistors_stat.lib
+-rw-r--r--   0        0        0     6144 2024-05-03 15:17:33.903843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib
+-rw-r--r--   0        0        0    40662 2024-05-03 15:17:33.903843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib
+-rw-r--r--   0        0        0     4027 2024-05-03 15:17:33.907843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib
+-rw-r--r--   0        0        0     6110 2024-05-03 15:17:33.895843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib
+-rw-r--r--   0        0        0    40995 2024-05-03 15:17:33.899843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib
+-rw-r--r--   0        0        0     3667 2024-05-03 15:17:33.899843 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib
+-rw-r--r--   0        0        0    18379 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/pdkmaster.py
+-rw-r--r--   0        0        0     2617 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/pyspice.py
+-rw-r--r--   0        0        0     4300 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2.post1/c4m/pdk/ihpsg13g2/stdcell.py
+-rw-r--r--   0        0        0     1563 2024-05-03 15:17:34.827837 c4m_pdk_ihpsg13g2-0.0.2.post1/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-05-03 15:17:34.823837 c4m_pdk_ihpsg13g2-0.0.2.post1/version.txt
+-rw-r--r--   0        0        0     5852 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.2.post1/PKG-INFO
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2/README.md` & `c4m_pdk_ihpsg13g2-0.0.2.post1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: c4m-pdk-ihpsg13g2
+Version: 0.0.2.post1
+Summary: PDKMaster based PDK for open source IHP SG13G2 process
+Author: Chips4Makers contributors
+License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
+Requires-Python: ~=3.8
+Requires-Dist: PDKMaster~=0.11.0.post2
+Requires-Dist: pdkmaster-io-klayout~=0.1.1.post1
+Requires-Dist: c4m-flexcell~=0.4.2.post3
+Requires-Dist: c4m-flexio~=0.4.2.post2
+Description-Content-Type: text/markdown
+
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
 * [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
@@ -10,14 +23,22 @@
 
 This is an alpha version of the IHP SG13G2 PDK, if it breaks you need to keep the pieces. E.g. hiccups are still expected when using this code base. For further discussion you can use the [Chips4Makers matrix channel](https://matrix.to/#/#Chips4Makers_community:gitter.im). Certainly interested to be made aware about usage of this project.
 
 ## Pypi release
 
 A version of this library is also released on PyPI. Currently this release is not expected to be of much use on it's own. Plan is to evolve this PyPI release onto a state the installation of it together with it's dependencies is enough to do P&R for IHP SG13G2.
 
+## Project Arrakeen subproject
+
+This project is part of Chips4Makers' [project Arrakeen](https://gitlab.com/Chips4Makers/c4m-arrakeen). It shares some common guide lines and regulations:
+
+* [Contributing.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/Contributing.md)
+* [LICENSE.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE.md): license of release code
+* [LICENSE_rationale.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE_rationale.md)
+
 # Development
 
 ## Dependencies
 
 Most of the dependencies are handled by [pdm](https://pdm-project.org/) and will this be taken care of when following the [pdm](https://pdm-project.org/) setup below. Only dependency that is not handled by that is [ngspice](https://ngspice.sourceforge.io/index.html) as that tool does not have a python package available yet. The current simulations performed for the docs are only tested with [ngspice](https://ngspice.sourceforge.io/index.html) version 42 with osdi models installed. Following procedure was used on local Linux development machine to get [ngspice](https://ngspice.sourceforge.io/index.html) installed:
 
 * Compiled [ngspice](https://ngspice.sourceforge.io/index.html) version 42 with default options (this includes osdi support for this latest version). Both the command as the shared library were compiled. The shared library is needed by `PySpice` and needs to be in default library search path or the `NGSPICE_LIBRARY_PATH` has to be set pointing to the [ngspice](https://ngspice.sourceforge.io/index.html) shared library.
@@ -37,47 +58,7 @@
 
 ## [Doit](https://pydoit.org/) targets
 
 [Doit](https://pydoit.org/) is used for build task setup and execution; the `pdm doit` command is to be used to call the `doit` command in an environment with the proper dependencies present. [Doit](https://pydoit.org/) can execute tasks in parallel by using the `-n N` option where `N` is the maximum number of parallel tasks. You do a `pdm doit list` to get a list of all the tasks defined in the `dodo.py` file. Highlight of some higher level tasks defined:
 
 * `tarball`: will run most of the tasks as dependency of that task and then generate a tarball in the `tarballs` subdirectory of the generated open PDK.
 * `patch4upstream`: will also run most tasks and then create a patch on top the dev branch in the the `upstream/IHP-Open-PDK` git submodule.
-
-# Licensing Rationale
-
-Open source projects and it's surrounding community can only strive when improvements to the
-code or application of the code itself are released to the public and allowed to be used by
-them. Copyleft type license are using the licensing terms to guarantee this actually happens
-and no party uses a 'take-but-don't-give-back' approach. The
-[GNU Aferro General Public License V3.0](LICENSES/agpl-3.0.txt) is used as main license for
-the code in this project as it is a copyleft type license that is also applicable to cloud
-services without binary distribution of the code.
-
-One of the problems with a strict copyleft license is that it can introduce incompatibilities
-with code released under other open source licenses. In order to improve compatibility and
-thus also re-usability the code in this repo is multi-licensed. Multi-licensing under
-established open source licenses was preferred over custom extension of licenses.
-
-The [GNU General Public License V2.0](LICENSES/gpl-2.0.txt) was added as optional license in
-order to allow derived code not to be bound by the anti-[tivoization](
-  https://en.wikipedia.org/wiki/Tivoization
-) clauses introduced in the [GNU General Public License Version 3](
-  https://www.gnu.org/licenses/gpl-3.0-standalone.html
-). The latter was not deemed necessary for this project and the addition was done to increase
-compatibility with some corporate policies.
-
-The [CERN Open Hardware Licence Version 2 - Strongly Reciprocal](LICENSES/cern_ohl_s_v2.txt) is included as it is a copyleft license specifically targeted for hardware but incompatible
-with the GPL licenses.
-
-The [Apache License Version 2.0](LICENSES/apache-2.0.txt) is included to maximize compatibility
-with existing open source code. One is supposed to not use it to avoid having to release one's
-own derived code to the public. If you plan development of a project in a proprietary way, one
-is kindly asked to not derive one's code from this project's code.
-
-In future the list of allowed licenses may be reduced. A reason could be that such an action
-is deemed necessary by the project maintainers to encourage open sourcing of derived code.
-
-Analog to how the object files and the executables generated by the gcc compiler are not
-necessarily governed by the GPL license, the multi-licensing applies only to code derived
-from code in this repository. Output files generated through the use of the code in this
-repository are not by default bound to the multi-licensing requirements of this project's
-code.
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2/pyproject.toml` & `c4m_pdk_ihpsg13g2-0.0.2.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 name = "c4m-pdk-ihpsg13g2"
 dynamic = []
 description = "PDKMaster based PDK for open source IHP SG13G2 process"
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
-version = "0.0.2"
+version = "0.0.2.post1"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -26,14 +26,19 @@
 
 [tool.pdm]
 distribution = true
 ignore_package_warnings = [
     "*",
 ]
 
+[tool.pdm.build]
+includes = [
+    "c4m/",
+]
+
 [tool.pdm.version]
 source = "scm"
 write_to = "version.txt"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "-e file:///${PROJECT_ROOT}/deps/PySpice#egg=PySpice",
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.2/PKG-INFO` & `c4m_pdk_ihpsg13g2-0.0.2.post1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: c4m-pdk-ihpsg13g2
-Version: 0.0.2
-Summary: PDKMaster based PDK for open source IHP SG13G2 process
-Author: Chips4Makers contributors
-License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
-Requires-Python: ~=3.8
-Requires-Dist: PDKMaster~=0.11.0
-Requires-Dist: pdkmaster-io-klayout~=0.1.1
-Requires-Dist: c4m-flexcell~=0.4.2
-Requires-Dist: c4m-flexio~=0.4.2
-Description-Content-Type: text/markdown
-
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
 * [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
@@ -23,14 +10,22 @@
 
 This is an alpha version of the IHP SG13G2 PDK, if it breaks you need to keep the pieces. E.g. hiccups are still expected when using this code base. For further discussion you can use the [Chips4Makers matrix channel](https://matrix.to/#/#Chips4Makers_community:gitter.im). Certainly interested to be made aware about usage of this project.
 
 ## Pypi release
 
 A version of this library is also released on PyPI. Currently this release is not expected to be of much use on it's own. Plan is to evolve this PyPI release onto a state the installation of it together with it's dependencies is enough to do P&R for IHP SG13G2.
 
+## Project Arrakeen subproject
+
+This project is part of Chips4Makers' [project Arrakeen](https://gitlab.com/Chips4Makers/c4m-arrakeen). It shares some common guide lines and regulations:
+
+* [Contributing.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/Contributing.md)
+* [LICENSE.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE.md): license of release code
+* [LICENSE_rationale.md](https://gitlab.com/Chips4Makers/c4m-arrakeen/-/blob/redtape_v1/LICENSE_rationale.md)
+
 # Development
 
 ## Dependencies
 
 Most of the dependencies are handled by [pdm](https://pdm-project.org/) and will this be taken care of when following the [pdm](https://pdm-project.org/) setup below. Only dependency that is not handled by that is [ngspice](https://ngspice.sourceforge.io/index.html) as that tool does not have a python package available yet. The current simulations performed for the docs are only tested with [ngspice](https://ngspice.sourceforge.io/index.html) version 42 with osdi models installed. Following procedure was used on local Linux development machine to get [ngspice](https://ngspice.sourceforge.io/index.html) installed:
 
 * Compiled [ngspice](https://ngspice.sourceforge.io/index.html) version 42 with default options (this includes osdi support for this latest version). Both the command as the shared library were compiled. The shared library is needed by `PySpice` and needs to be in default library search path or the `NGSPICE_LIBRARY_PATH` has to be set pointing to the [ngspice](https://ngspice.sourceforge.io/index.html) shared library.
@@ -50,47 +45,7 @@
 
 ## [Doit](https://pydoit.org/) targets
 
 [Doit](https://pydoit.org/) is used for build task setup and execution; the `pdm doit` command is to be used to call the `doit` command in an environment with the proper dependencies present. [Doit](https://pydoit.org/) can execute tasks in parallel by using the `-n N` option where `N` is the maximum number of parallel tasks. You do a `pdm doit list` to get a list of all the tasks defined in the `dodo.py` file. Highlight of some higher level tasks defined:
 
 * `tarball`: will run most of the tasks as dependency of that task and then generate a tarball in the `tarballs` subdirectory of the generated open PDK.
 * `patch4upstream`: will also run most tasks and then create a patch on top the dev branch in the the `upstream/IHP-Open-PDK` git submodule.
-
-# Licensing Rationale
-
-Open source projects and it's surrounding community can only strive when improvements to the
-code or application of the code itself are released to the public and allowed to be used by
-them. Copyleft type license are using the licensing terms to guarantee this actually happens
-and no party uses a 'take-but-don't-give-back' approach. The
-[GNU Aferro General Public License V3.0](LICENSES/agpl-3.0.txt) is used as main license for
-the code in this project as it is a copyleft type license that is also applicable to cloud
-services without binary distribution of the code.
-
-One of the problems with a strict copyleft license is that it can introduce incompatibilities
-with code released under other open source licenses. In order to improve compatibility and
-thus also re-usability the code in this repo is multi-licensed. Multi-licensing under
-established open source licenses was preferred over custom extension of licenses.
-
-The [GNU General Public License V2.0](LICENSES/gpl-2.0.txt) was added as optional license in
-order to allow derived code not to be bound by the anti-[tivoization](
-  https://en.wikipedia.org/wiki/Tivoization
-) clauses introduced in the [GNU General Public License Version 3](
-  https://www.gnu.org/licenses/gpl-3.0-standalone.html
-). The latter was not deemed necessary for this project and the addition was done to increase
-compatibility with some corporate policies.
-
-The [CERN Open Hardware Licence Version 2 - Strongly Reciprocal](LICENSES/cern_ohl_s_v2.txt) is included as it is a copyleft license specifically targeted for hardware but incompatible
-with the GPL licenses.
-
-The [Apache License Version 2.0](LICENSES/apache-2.0.txt) is included to maximize compatibility
-with existing open source code. One is supposed to not use it to avoid having to release one's
-own derived code to the public. If you plan development of a project in a proprietary way, one
-is kindly asked to not derive one's code from this project's code.
-
-In future the list of allowed licenses may be reduced. A reason could be that such an action
-is deemed necessary by the project maintainers to encourage open sourcing of derived code.
-
-Analog to how the object files and the executables generated by the gcc compiler are not
-necessarily governed by the GPL license, the multi-licensing applies only to code derived
-from code in this repository. Output files generated through the use of the code in this
-repository are not by default bound to the multi-licensing requirements of this project's
-code.
```

