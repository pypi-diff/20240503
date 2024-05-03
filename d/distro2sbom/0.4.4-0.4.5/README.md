# Comparing `tmp/distro2sbom-0.4.4-py2.py3-none-any.whl.zip` & `tmp/distro2sbom-0.4.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 21301 bytes, number of entries: 15
+Zip file size: 21786 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/__init__.py
--rw-r--r--  2.0 unx     7852 b- defN 24-Mar-24 18:50 distro2sbom/cli.py
+-rw-r--r--  2.0 unx     7852 b- defN 24-May-03 08:50 distro2sbom/cli.py
 -rw-r--r--  2.0 unx      462 b- defN 23-Jul-23 20:45 distro2sbom/test.py
--rw-r--r--  2.0 unx      100 b- defN 24-Mar-24 19:56 distro2sbom/version.py
+-rw-r--r--  2.0 unx      100 b- defN 24-May-03 08:46 distro2sbom/version.py
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/distrobuilder/__init__.py
--rw-r--r--  2.0 unx     3160 b- defN 24-Mar-14 14:30 distro2sbom/distrobuilder/distrobuilder.py
--rw-r--r--  2.0 unx    13584 b- defN 24-Mar-24 19:53 distro2sbom/distrobuilder/dpkgbuilder.py
--rw-r--r--  2.0 unx    13912 b- defN 24-Mar-24 19:54 distro2sbom/distrobuilder/rpmbuilder.py
--rw-r--r--  2.0 unx     4688 b- defN 23-Jul-23 20:45 distro2sbom/distrobuilder/windowsbuilder.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-25 18:49 distro2sbom-0.4.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    10726 b- defN 24-Mar-25 18:49 distro2sbom-0.4.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-25 18:49 distro2sbom-0.4.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-Mar-25 18:49 distro2sbom-0.4.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Mar-25 18:49 distro2sbom-0.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 24-Mar-25 18:49 distro2sbom-0.4.4.dist-info/RECORD
-15 files, 67468 bytes uncompressed, 19127 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx     3246 b- defN 24-May-03 08:46 distro2sbom/distrobuilder/distrobuilder.py
+-rw-r--r--  2.0 unx    13584 b- defN 24-May-03 08:38 distro2sbom/distrobuilder/dpkgbuilder.py
+-rw-r--r--  2.0 unx    14116 b- defN 24-May-03 08:46 distro2sbom/distrobuilder/rpmbuilder.py
+-rw-r--r--  2.0 unx     4688 b- defN 24-May-03 08:39 distro2sbom/distrobuilder/windowsbuilder.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11863 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/RECORD
+15 files, 68895 bytes uncompressed, 19612 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: distro2sbom/distrobuilder/rpmbuilder.py
 Comment: 
 
 Filename: distro2sbom/distrobuilder/windowsbuilder.py
 Comment: 
 
-Filename: distro2sbom-0.4.4.dist-info/LICENSE
+Filename: distro2sbom-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: distro2sbom-0.4.4.dist-info/METADATA
+Filename: distro2sbom-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: distro2sbom-0.4.4.dist-info/WHEEL
+Filename: distro2sbom-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: distro2sbom-0.4.4.dist-info/entry_points.txt
+Filename: distro2sbom-0.4.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: distro2sbom-0.4.4.dist-info/top_level.txt
+Filename: distro2sbom-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: distro2sbom-0.4.4.dist-info/RECORD
+Filename: distro2sbom-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## distro2sbom/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2024 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.4.4"
+VERSION: str = "0.4.5"
```

## distro2sbom/distrobuilder/distrobuilder.py

```diff
@@ -1,21 +1,23 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
+import os
 import re
 import subprocess
 import unicodedata
 from pathlib import Path
 
 
 class DistroBuilder:
     def __init__(self, debug=False):
         self.sbom_packages = {}
         self.sbom_relationships = []
         self.debug = debug
+        self.root = os.environ.get('DISTRO2SBOM_ROOT_PATH', '')
 
     def get_data(self):
         pass
 
     def parse_data(self):
         pass
 
@@ -65,15 +67,15 @@
         return self.sbom_relationships
 
     def get_parent(self):
         return self.parent
 
     def get_system(self):
         # Extract metadata from file
-        OS_FILE = "/etc/os-release"
+        OS_FILE = f"{self.root}/etc/os-release"
         metadata = {}
         filePath = Path(OS_FILE)
         # Check path exists and is a valid file
         if filePath.exists() and filePath.is_file():
             os_file = open(OS_FILE)
             lines = os_file.readlines()
             for line in lines:
```

## distro2sbom/distrobuilder/rpmbuilder.py

```diff
@@ -22,14 +22,16 @@
         if name is None and release is None:
             self.name = self.system_data["name"].replace(" ", "-")
             self.release = self.system_data["version_id"]
         else:
             self.name = name.replace(" ", "-")
             self.release = release
         self.parent = f"Distro-{self.name}"
+        self.rpm_options = os.environ.get('DISTRO2SBOM_RPM_OPTIONS', '')
+        self.yum_options = os.environ.get('DISTRO2SBOM_YUM_OPTIONS', '')
 
     def get_data(self):
         pass
 
     def parse_data(self, filename):
         # Process file containing installed applications
         with open(filename) as dir_file:
@@ -108,15 +110,15 @@
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
                 parent, "DEPENDS_ON", package_name.replace("_", "-")
             )
             self.sbom_relationships.append(self.sbom_relationship.get_relationship())
             return 0
         self.distro_packages.append(package_name)
-        out = self.run_program(f"rpm -qi {package_name}")
+        out = self.run_program(f"rpm {self.rpm_options} -qi {package_name}")
         # If package not found, no metadata returned
         if len(out) > 0:
             self.metadata = {}
             for line in out:
                 if ":" in line:
                     line_entry = re.sub(" +", " ", line.strip().rstrip("\n"))
                     entry = line_entry.split(":")
@@ -126,15 +128,15 @@
                         line_entry[len(keyword) + 2 :].strip().rstrip("\n")
                     )
             if len(self.metadata) == 0:
                 # Package not installed so no metadata
                 return False
             # Now find package dependencies
             dependencies_out = self.run_program(
-                f"yum repoquery --deplist {package_name}"
+                f"yum repoquery {self.yum_options} --deplist {package_name}"
             )
             requires = []
             for line in dependencies_out:
                 # Only process lines with provider
                 if "provider:" not in line:
                     continue
                 # Remove keyword from line
@@ -262,15 +264,15 @@
         self.sbom_packages[
             (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
         ] = self.sbom_package.get_package()
         self.sbom_relationship.initialise()
         self.sbom_relationship.set_relationship(self.parent, "DESCRIBES", distro_root)
         self.sbom_relationships.append(self.sbom_relationship.get_relationship())
         # Get installed packages
-        out = self.run_program("rpm -qa")
+        out = self.run_program(f"rpm {self.rpm_options} -qa")
         for line in out:
             # Parse line PRODUCT-VERSION[-Other]?. If pattern not followed ignore...
             item = os.path.splitext(os.path.basename(line.strip().rstrip("\n")))[
                 0
             ].lower()
             # Version assumed to start with digit.
             product_version = re.search(r"-\d[.\d]*[a-z0-9]*", item)
```

## Comparing `distro2sbom-0.4.4.dist-info/LICENSE` & `distro2sbom-0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `distro2sbom-0.4.4.dist-info/METADATA` & `distro2sbom-0.4.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distro2sbom
-Version: 0.4.4
+Version: 0.4.5
 Summary: SBOM generator for system distribution
 Home-page: https://github.com/anthonyharrison/distro2sbom
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -193,14 +193,31 @@
 
 ```bash
 distro2sbom --distro deb --system --format json --output-file <distrooutfile>
 ```
 
 This will generate an SBOM in SPDX JSON value for a distribution file in dpkg format (indicated by the 'deb' option)
 
+#### Specific options for rpm/yum based distro
+
+The following [optional] environment variable are available to customize rpm and yum commands used by the tool. This can be usefull for example to enable/disable some repo or to support *chrooted* environments.
+
+- **DISTRO2SBOM_ROOT_PATH** The path prefix where to get `/etc/os-release`
+- **DISTRO2SBOM_RPM_OPTIONS** Additional options passed to rpm commands (used by `rpm -qa` to list all packages and `rpm -qi <pkg>` to query information on a package)
+- **DISTRO2SBOM_YUM_OPTIONS** Additional options passed to yum commands (used by `yum repoquery --deplist <pkg>` to get dependencies)
+
+```bash
+export DISTRO2SBOM_ROOT_PATH=/path-to-distrib/slash
+export DISTRO2SBOM_RPM_OPTIONS="--root /path-to-distrib/slash"
+export DISTRO2SBOM_YUM_OPTIONS="--installroot=/path-to-distrib/slash --setopt=reposdir=/path-to-distrib/repos --setopt=install_weak_deps=False --repo=my-repo"
+distro2sbom --distro rpm --system --sbom cyclonedx --format json --output-file <distrooutfile>
+```
+
+This will generate an SBOM in CYCLONEDX JSON value for a *chrooted* distribution located at `/path-to-distrib/slash`
+
 ## Licence
 
 Licenced under the Apache 2.0 Licence.
 
 ## Limitations
 
 This tool is meant to support software development and security audit functions. However, the usefulness of the tool is dependent on the SBOM data
```

## Comparing `distro2sbom-0.4.4.dist-info/RECORD` & `distro2sbom-0.4.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 distro2sbom/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 distro2sbom/cli.py,sha256=Yvt0o09GKRhWMnKsjFUbQBUMpHvn0iTCiJxiEZ3tc9c,7852
 distro2sbom/test.py,sha256=m8yYYiZq9QUIqcNAKQOGPvboIvnZ8WrZUH2ELMm4c4E,462
-distro2sbom/version.py,sha256=Uo-pOjyMgPMMC9cVZ1HRsg-eGdoZ4jlet45WBUEW_lU,100
+distro2sbom/version.py,sha256=RhzVdAnIAIeNpoZLjlCpx5ZgkvJyztkiWp-TZKe5hDc,100
 distro2sbom/distrobuilder/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/distrobuilder/distrobuilder.py,sha256=FAMU8l8JacuTbIZhi73ozfsKa14jq4AigjZT4kD2deI,3160
+distro2sbom/distrobuilder/distrobuilder.py,sha256=x_s_YoojCQsV5rUzdzSrzpd1zxXaXXM1G1AaRDZ-N4M,3246
 distro2sbom/distrobuilder/dpkgbuilder.py,sha256=70Et6Su52hUbmMSsL_m0Jf7Oxytsk-OTT1fnabnQLUA,13584
-distro2sbom/distrobuilder/rpmbuilder.py,sha256=03EL_7-vg90cIWd__nc9ejsKClIzVxs9SQ49zc6KfhY,13912
+distro2sbom/distrobuilder/rpmbuilder.py,sha256=p2Kphbayy_C6Vvd86xL2qzWMtRFEm_PIbSFhbt7wLc8,14116
 distro2sbom/distrobuilder/windowsbuilder.py,sha256=P-1xTEqHZHTEGobkbycf_Wgfa2KhlPRx5MqKVcQPLFY,4688
-distro2sbom-0.4.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-distro2sbom-0.4.4.dist-info/METADATA,sha256=Ulz490cq6AVdnxiuuWw4N1dKIE2ZYLjWzp9d-d62c2g,10726
-distro2sbom-0.4.4.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-distro2sbom-0.4.4.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
-distro2sbom-0.4.4.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
-distro2sbom-0.4.4.dist-info/RECORD,,
+distro2sbom-0.4.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+distro2sbom-0.4.5.dist-info/METADATA,sha256=xCHP_ZP-Sw3iQwJHDVz01G41UvKqGbVuvWvKYBDz6eY,11863
+distro2sbom-0.4.5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+distro2sbom-0.4.5.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
+distro2sbom-0.4.5.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
+distro2sbom-0.4.5.dist-info/RECORD,,
```

