# Comparing `tmp/csaf_tool-0.3.0-py2.py3-none-any.whl.zip` & `tmp/csaf_tool-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17477 bytes, number of entries: 13
+Zip file size: 17596 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-05 22:31 csaf/__init__.py
 -rw-r--r--  2.0 unx    14707 b- defN 24-Mar-16 19:36 csaf/analyser.py
 -rw-r--r--  2.0 unx     6016 b- defN 22-Dec-08 22:33 csaf/cli.py
 -rw-r--r--  2.0 unx      933 b- defN 22-Dec-08 21:36 csaf/config.py
--rw-r--r--  2.0 unx    14318 b- defN 24-Mar-22 08:42 csaf/generator.py
--rw-r--r--  2.0 unx     9681 b- defN 24-Mar-25 18:22 csaf/parser.py
--rw-r--r--  2.0 unx       93 b- defN 24-Mar-24 17:38 csaf/version.py
--rw-r--r--  2.0 unx     1072 b- defN 24-Mar-25 18:31 csaf_tool-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    21726 b- defN 24-Mar-25 18:31 csaf_tool-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-25 18:31 csaf_tool-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-Mar-25 18:31 csaf_tool-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-25 18:31 csaf_tool-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      992 b- defN 24-Mar-25 18:31 csaf_tool-0.3.0.dist-info/RECORD
-13 files, 69697 bytes uncompressed, 15839 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx    14980 b- defN 24-Apr-29 18:57 csaf/generator.py
+-rw-r--r--  2.0 unx     9614 b- defN 24-Apr-29 19:04 csaf/parser.py
+-rw-r--r--  2.0 unx       93 b- defN 24-Apr-29 16:02 csaf/version.py
+-rw-r--r--  2.0 unx     1072 b- defN 24-May-03 16:19 csaf_tool-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    21726 b- defN 24-May-03 16:19 csaf_tool-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-03 16:19 csaf_tool-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-03 16:19 csaf_tool-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-03 16:19 csaf_tool-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      992 b- defN 24-May-03 16:19 csaf_tool-0.3.1.dist-info/RECORD
+13 files, 70292 bytes uncompressed, 15958 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: csaf/parser.py
 Comment: 
 
 Filename: csaf/version.py
 Comment: 
 
-Filename: csaf_tool-0.3.0.dist-info/LICENSE
+Filename: csaf_tool-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: csaf_tool-0.3.0.dist-info/METADATA
+Filename: csaf_tool-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: csaf_tool-0.3.0.dist-info/WHEEL
+Filename: csaf_tool-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: csaf_tool-0.3.0.dist-info/entry_points.txt
+Filename: csaf_tool-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: csaf_tool-0.3.0.dist-info/top_level.txt
+Filename: csaf_tool-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: csaf_tool-0.3.0.dist-info/RECORD
+Filename: csaf_tool-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## csaf/generator.py

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2024 Anthony Harrison
 # SPDX-License-Identifier: MIT
 
 import json
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 
 from csaf.config import CSAFConfig
 from csaf.version import VERSION
 
 CSAF_ENGINE = "csaf-tool"
 CSAF_CONFIG = "csaf.ini"
@@ -39,15 +39,15 @@
             self.publisher_url = self.csaf_config.get_section("publisher")["url"]
         else:
             # set default values
             self.publisher_category = "vendor"
             self.publisher_name = "ACME Inc."
             self.publisher_url = "https://www.example.com"
         self.core_product = None
-        self.revision=1
+        self.revision=0
         self.sbom = None
 
     def add_product(self, product_name, vendor, release, sbom=""):
         if len(self.product_list) == 0:
             # First product is assumed to be core product
             self.core_product = product_name + "_" + release
         if product_name in self.product_list:
@@ -55,15 +55,15 @@
             self.product_list[product_name]["releases"].append(release)
         elif vendor is not None:
             self.product_list[product_name] = {"vendor": vendor, "releases": [release]}
         if len(str(sbom)) > 0:
             self.sbom = Path(sbom)
 
     def add_vulnerability(
-        self, product_name, release, id, description, status, comment, justification=None, created=None
+        self, product_name, release, id, description, status, comment, justification=None, created=None, remediation=None,action=None,
     ):
         vulnerability = {}
         vulnerability["product"] = product_name
         vulnerability["release"] = release
         vulnerability["id"] = id
         if description is not None:
             vulnerability["description"] = description
@@ -96,14 +96,18 @@
         if status == "known_not_affected":
             # Justification required
             if "justification" not in vulnerability:
                 # Need default justification
                 vulnerability["justification"] = "component_not_present"
         if created is not None:
             vulnerability["created"] = created
+        if remediation is not None:
+            vulnerability["remediation"] = remediation
+        if action is not None:
+            vulnerability["action"] = action
         self.vulnerabilities_list.append(vulnerability)
 
     def set_title(self, title):
         self.title = title
 
     def set_header_title(self, title):
         if title != "":
@@ -114,15 +118,15 @@
             self.id = id
 
     def set_value(self, attribute, value):
         self.metadata[attribute]=value
 
     def generate_csaf(self):
 
-        time_now = datetime.now().strftime("%Y-%m-%dT%H-%M-%SZ")
+        time_now = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
         header = dict()
         header["category"] = "csaf_vex"
         header["csaf_version"] = "2.0"
         notes = []
         note_info = dict()
         if "notes" in self.metadata:
             for note in self.metadata["notes"]:
@@ -191,20 +195,15 @@
         tracking_info["revision_history"] = revision
         if "status" in self.metadata:
             tracking_info["status"] = self.metadata.get("status")
         elif "tracking_status" in self.metadata:
             tracking_info["status"] = self.metadata.get("tracking_status")
         else:
             tracking_info["status"] = self.metadata.get("status","final")  # Check options
-        if "version" in self.metadata:
-            tracking_info["version"] = self.metadata.get("version")
-        elif "tracking_version" in self.metadata:
-            tracking_info["version"] = self.metadata.get("tracking_version")
-        else:
-            tracking_info["version"] = "1"
+        tracking_info["version"] = str(self.revision+1)
         header["tracking"] = tracking_info
         # Build up a product tree
 
         product_tree = dict()
         vendor_info = dict()
         product_info = dict()
         vendor_info["branches"] = []
@@ -225,15 +224,15 @@
                 product_note["name"] = (
                     self.product_list[p]["vendor"] + " " + p + " " + str(v)
                 )
                 product_note["product_id"] = "CSAFPID_" + str(product_id).rjust(4,'0')
                 product_id += 1
                 if self.sbom is not None:
                     product_helper = dict()
-                    product_helper["sbom_urls"] = Path.as_uri(self.sbom)
+                    product_helper["sbom_urls"] = [Path.as_uri(self.sbom)]
                     product_note["product_identification_helper"]=product_helper
                 version_info["product"] = product_note
                 product_id_list[p + "_" + version_info["name"]] = {
                     "name": product_note["name"],
                     "release": version_info["name"],
                     "id": product_note["product_id"],
                 }
@@ -275,45 +274,57 @@
             #product_info["known_affected"] = []
             product_info[status] = []
             #product_id = product_id_list[product + "_" + version]
             product_info[status].append(product_id["id"])
             vulnerability["product_status"] = product_info
             justification = v.get("justification")
             flag_info = dict()
-            if v.get("created") is not None:
-                # Preserve time
-                flag_info["date"] = v.get("created")
-            else:
-                flag_info["date"] = time_now
+            # Flags only if vulnerability justification provided
             if justification is not None:
-                flag_info["label"] = justification
-            flag_info["product_ids"] = [product_id["id"]]
-            vulnerability["flags"] = [flag_info]
+                if v.get("created") is not None:
+                    # Preserve time
+                    flag_info["date"] = v.get("created")
+                else:
+                    flag_info["date"] = time_now
+                if justification is not None:
+                    flag_info["label"] = justification
+                flag_info["product_ids"] = [product_id["id"]]
+                vulnerability["flags"] = [flag_info]
             if comment is not None:
                 threat_info = dict()
                 threat_info["category"] = "impact"
                 threat_info["details"] = comment
-                threat_info["date"] = flag_info["date"]
+                threat_info["date"] = flag_info.get("date",time_now)
                 product_id_info = []
                 product_id_info.append(product_id["id"])
                 threat_info["product_ids"] = product_id_info
                 vulnerability["threats"] = [threat_info]
+            if status == "known_affected":
+                remediation_info = dict()
+                remediation_info["category"] = v.get("remediation","no_idea")
+                remediation_info["details"] = v.get("action","Go and fix it")
+                product_id_info = []
+                product_id_info.append(product_id["id"])
+                remediation_info["product_ids"] = product_id_info
+                vulnerability["remediations"] = [remediation_info]
             vulnerabilities.append(vulnerability)
 
         # Build up CSAF document
         self.csaf_document["document"] = header
         self.csaf_document["product_tree"] = product_tree
         self.csaf_document["vulnerabilities"] = vulnerabilities
 
     def publish_csaf(self, filename):
         with open(filename, "w") as outfile:
             json.dump(self.csaf_document, outfile, indent="   ")
 
     def get_revision(self):
-        return self.revision
+        if self.revision > 0:
+            return self.revision
+        return 1
 
 if __name__ == "__main__":
     csaf_gen = CSAFGenerator()
     csaf_gen.set_title("Test CSAF document")
     csaf_gen.set_header_title("Example VEX Document Use Case 1 - Affected")
     csaf_gen.set_id("Avendor-advisory-0004")
     csaf_gen.add_product(product_name="product1", vendor="Avendor", release=1)
```

## csaf/parser.py

```diff
@@ -178,17 +178,16 @@
                 for threat in vulnerability["threats"]:
                     vuln_info.set_value(threat["category"], threat["details"])
             if "product_status" in vulnerability:
                 for product_status in vulnerability["product_status"]:
                     vuln_info.set_value("status", product_status)
             if "remediations" in vulnerability:
                 for remediation in vulnerability["remediations"]:
-                    fix = remediation["category"].upper()
-                    details = remediation["details"]
-                    vuln_info.set_value(fix, [details, remediation.get("product_ids","-")])
+                    vuln_info.set_remediation(remediation["category"])
+                    vuln_info.set_action(remediation["details"])
             self.vulnerabilities.append(vuln_info.get_vulnerability())
 
     def get_metadata(self):
         return self.metadata
 
     def get_product(self):
         return self.product
```

## csaf/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2024 Anthony Harrison
 # SPDX-License-Identifier: MIT
 
-VERSION: str = "0.3.0"
+VERSION: str = "0.3.1"
```

## Comparing `csaf_tool-0.3.0.dist-info/LICENSE` & `csaf_tool-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `csaf_tool-0.3.0.dist-info/METADATA` & `csaf_tool-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csaf-tool
-Version: 0.3.0
+Version: 0.3.1
 Summary: CSAF generator and analyser
 Home-page: https://github.com/anthonyharrison/csaf
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: MIT
```

## Comparing `csaf_tool-0.3.0.dist-info/RECORD` & `csaf_tool-0.3.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 csaf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csaf/analyser.py,sha256=jlqdmqEGibrMwyFfjM6s0GxL9uhlvvevuPWhSz59Aas,14707
 csaf/cli.py,sha256=jxr3ip8JnuvGwZBJAa3-otcsvYqMswKaMUHtRHC76fI,6016
 csaf/config.py,sha256=5E3fE0gcbi5NueFELRHun9tAwsKbzs9ca2ltLrilwwc,933
-csaf/generator.py,sha256=lATZ7z28v--Wxa0VQzj7Av51Ms8J_92TBcKWQ1wtKtA,14318
-csaf/parser.py,sha256=v8dwNy6WHo7GNCSVrVQLcjMRMVfJUSC-y3NVcGRl-Ek,9681
-csaf/version.py,sha256=gQxQLIvUPLAr_h0GTnRwmsNuIvLg_aA2WKDv7TLDErM,93
-csaf_tool-0.3.0.dist-info/LICENSE,sha256=RDxASdupnGe4zcNXLT7tl7BbIdpK2d15NmWIFUf_rjw,1072
-csaf_tool-0.3.0.dist-info/METADATA,sha256=kB3wasg3C3Vqdx3XOejhCI7UtsSlY1ukTW-sOU3EV3g,21726
-csaf_tool-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-csaf_tool-0.3.0.dist-info/entry_points.txt,sha256=IE71_uSBh29bpTJPeL9QYn7KDu7ubZ-JYbM1e3SYc3k,44
-csaf_tool-0.3.0.dist-info/top_level.txt,sha256=LS3fIaygrsIMdkUdUFkvPE_Ljqq97T7cIl-fwCYnQDg,5
-csaf_tool-0.3.0.dist-info/RECORD,,
+csaf/generator.py,sha256=zu0P1rcYkqelP6IIk8_Zim9I1zjQSOpeOj8JBbk4HNk,14980
+csaf/parser.py,sha256=8gc2RI5aWHYvmp2Mhi98dchXqOym5KVGHe8-yjpcOLA,9614
+csaf/version.py,sha256=l5kwng4c4PTySeq5d84MNcgTacBH1drFTDOg1-VCxrM,93
+csaf_tool-0.3.1.dist-info/LICENSE,sha256=RDxASdupnGe4zcNXLT7tl7BbIdpK2d15NmWIFUf_rjw,1072
+csaf_tool-0.3.1.dist-info/METADATA,sha256=4oKluqdJBDKblGaEp5Efy6g5brKVSffNV9XixzIL2N0,21726
+csaf_tool-0.3.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+csaf_tool-0.3.1.dist-info/entry_points.txt,sha256=IE71_uSBh29bpTJPeL9QYn7KDu7ubZ-JYbM1e3SYc3k,44
+csaf_tool-0.3.1.dist-info/top_level.txt,sha256=LS3fIaygrsIMdkUdUFkvPE_Ljqq97T7cIl-fwCYnQDg,5
+csaf_tool-0.3.1.dist-info/RECORD,,
```

