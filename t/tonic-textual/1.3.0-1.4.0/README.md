# Comparing `tmp/tonic_textual-1.3.0.tar.gz` & `tmp/tonic_textual-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_textual-1.3.0.tar", max compression
+gzip compressed data, was "tonic_textual-1.4.0.tar", max compression
```

## Comparing `tonic_textual-1.3.0.tar` & `tonic_textual-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-1.3.0/LICENSE
--rw-r--r--   0        0        0      972 2024-02-17 17:17:54.164871 tonic_textual-1.3.0/README.md
--rw-r--r--   0        0        0      598 2024-04-26 22:23:38.075685 tonic_textual-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       19 2024-04-26 22:23:38.076054 tonic_textual-1.3.0/tonic_textual/__init__.py
--rw-r--r--   0        0        0    16432 2024-04-26 22:23:38.076252 tonic_textual-1.3.0/tonic_textual/api.py
--rw-r--r--   0        0        0        0 2024-02-17 17:17:54.168806 tonic_textual-1.3.0/tonic_textual/classes/__init__.py
--rw-r--r--   0        0        0      789 2024-02-17 17:17:54.168921 tonic_textual-1.3.0/tonic_textual/classes/api_responses/redaction_response.py
--rw-r--r--   0        0        0      668 2024-02-23 23:38:13.865340 tonic_textual-1.3.0/tonic_textual/classes/api_responses/single_detection_result.py
--rw-r--r--   0        0        0      348 2024-02-17 17:17:54.169331 tonic_textual-1.3.0/tonic_textual/classes/custom_model.py
--rw-r--r--   0        0        0     8183 2024-04-19 18:36:12.557423 tonic_textual-1.3.0/tonic_textual/classes/dataset.py
--rw-r--r--   0        0        0     1633 2024-02-17 17:17:54.169557 tonic_textual-1.3.0/tonic_textual/classes/datasetfile.py
--rw-r--r--   0        0        0     4845 2024-04-26 22:23:38.076471 tonic_textual-1.3.0/tonic_textual/classes/httpclient.py
--rw-r--r--   0        0        0     1864 2024-04-19 18:36:12.557633 tonic_textual-1.3.0/tonic_textual/classes/tonic_exception.py
--rw-r--r--   0        0        0      121 2024-04-26 22:23:38.076887 tonic_textual-1.3.0/tonic_textual/enums/pii_state.py
--rw-r--r--   0        0        0        0 2024-02-17 17:17:54.170004 tonic_textual-1.3.0/tonic_textual/services/__init__.py
--rw-r--r--   0        0        0      610 2024-02-17 17:17:54.170141 tonic_textual-1.3.0/tonic_textual/services/dataset.py
--rw-r--r--   0        0        0      552 2024-02-17 17:17:54.170230 tonic_textual-1.3.0/tonic_textual/services/datasetfile.py
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 tonic_textual-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-17 17:17:54.164782 tonic_textual-1.4.0/LICENSE
+-rw-r--r--   0        0        0      972 2024-02-17 17:17:54.164871 tonic_textual-1.4.0/README.md
+-rw-r--r--   0        0        0      598 2024-05-01 21:45:49.547180 tonic_textual-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-05-01 21:45:49.547299 tonic_textual-1.4.0/tonic_textual/__init__.py
+-rw-r--r--   0        0        0    17451 2024-05-01 21:45:49.547439 tonic_textual-1.4.0/tonic_textual/api.py
+-rw-r--r--   0        0        0        0 2024-02-17 17:17:54.168806 tonic_textual-1.4.0/tonic_textual/classes/__init__.py
+-rw-r--r--   0        0        0      789 2024-02-17 17:17:54.168921 tonic_textual-1.4.0/tonic_textual/classes/api_responses/redaction_response.py
+-rw-r--r--   0        0        0      668 2024-02-23 23:38:13.865340 tonic_textual-1.4.0/tonic_textual/classes/api_responses/single_detection_result.py
+-rw-r--r--   0        0        0      348 2024-02-17 17:17:54.169331 tonic_textual-1.4.0/tonic_textual/classes/custom_model.py
+-rw-r--r--   0        0        0     8183 2024-05-01 21:45:49.547665 tonic_textual-1.4.0/tonic_textual/classes/dataset.py
+-rw-r--r--   0        0        0     1633 2024-02-17 17:17:54.169557 tonic_textual-1.4.0/tonic_textual/classes/datasetfile.py
+-rw-r--r--   0        0        0     4845 2024-05-01 21:45:49.547986 tonic_textual-1.4.0/tonic_textual/classes/httpclient.py
+-rw-r--r--   0        0        0     1864 2024-05-01 21:45:49.548117 tonic_textual-1.4.0/tonic_textual/classes/tonic_exception.py
+-rw-r--r--   0        0        0      121 2024-05-01 21:45:49.548424 tonic_textual-1.4.0/tonic_textual/enums/pii_state.py
+-rw-r--r--   0        0        0        0 2024-02-17 17:17:54.170004 tonic_textual-1.4.0/tonic_textual/services/__init__.py
+-rw-r--r--   0        0        0      610 2024-02-17 17:17:54.170141 tonic_textual-1.4.0/tonic_textual/services/dataset.py
+-rw-r--r--   0        0        0      552 2024-02-17 17:17:54.170230 tonic_textual-1.4.0/tonic_textual/services/datasetfile.py
+-rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 tonic_textual-1.4.0/PKG-INFO
```

### Comparing `tonic_textual-1.3.0/LICENSE` & `tonic_textual-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/README.md` & `tonic_textual-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/pyproject.toml` & `tonic_textual-1.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-textual"
-version = "1.3.0"
+version = "1.4.0"
 description = "Wrappers around the Tonic Textual API"
 authors = ["Adam Kamor <adam@tonic.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.tonic.ai/"
 keywords = ["tonic.ai", "tonic", "tonic textual"]
```

### Comparing `tonic_textual-1.3.0/tonic_textual/api.py` & `tonic_textual-1.4.0/tonic_textual/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,46 +114,65 @@
         Returns
         ------
         List[DatasetFile]
         A list of all of the files in the dataset.
         """
         return self.datasetfile_service.get_files(dataset_id)
 
-    def unredact_bulk(self, redacted_strings: List[str]) -> List[str]:
+    def unredact_bulk(self, redacted_strings: List[str], random_seed: Optional[int] = None) -> List[str]:
             """Removes redaction from a list of strings. Returns the strings with the original values.
 
             Parameters
             ----------
             redacted_strings : List[str]
                 The list of redacted strings from which to remove the redaction.
 
+            random_seed: Optional[int] = None
+                An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+
             Returns
             -------
             List[str]
                 The list of strings with the redaction removed.
             """
 
-            response = self.client.http_post("/api/unredact", data=redacted_strings)
+            if random_seed is not None:
+                additional_headers = {'textual-random-seed':str(random_seed)}
+            else:
+                additional_headers = {}
+                
+            response = self.client.http_post("/api/unredact", data=redacted_strings, additional_headers=additional_headers)
             return response
 
-    def unredact(self, redacted_string: str) -> str:
+    def unredact(self, redacted_string: str, random_seed: Optional[int] = None) -> str:
             """Removes the redaction from a provided string. Returns the string with the original values.
 
             Parameters
             ----------
             redacted_string : str
                 The redacted string from which to remove the redaction.
 
+            random_seed: Optional[int] = None
+                An optional value to use to override Textual's default random number seeding.  Can be used to ensure that different API calls use the same or different random seeds.
+            
             Returns
             -------
             str
                 The string with the redaction removed.
             """
 
-            response = self.client.http_post("/api/unredact", data=[redacted_string])
+
+            if random_seed is not None:
+                additional_headers = {'textual-random-seed':str(random_seed)}
+            else:
+                additional_headers = {}
+                
+            response = self.client.http_post("/api/unredact", data=[redacted_string], additional_headers=additional_headers)
+
+            
             return response
 
     def redact(self, string: str, generator_config: Dict[str, PiiState] = dict(), generator_default: PiiState = PiiState.Redaction, custom_models: List[str] = [], random_seed: Optional[int] = None) -> RedactionResponse:
             """Redacts a string. Depending on the configured handling for each sensitive data type, values can be either redacted, synthesized, or ignored.
 
             Parameters
             ----------
```

### Comparing `tonic_textual-1.3.0/tonic_textual/classes/api_responses/redaction_response.py` & `tonic_textual-1.4.0/tonic_textual/classes/api_responses/redaction_response.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/classes/api_responses/single_detection_result.py` & `tonic_textual-1.4.0/tonic_textual/classes/api_responses/single_detection_result.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/classes/dataset.py` & `tonic_textual-1.4.0/tonic_textual/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/classes/datasetfile.py` & `tonic_textual-1.4.0/tonic_textual/classes/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/classes/httpclient.py` & `tonic_textual-1.4.0/tonic_textual/classes/httpclient.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/classes/tonic_exception.py` & `tonic_textual-1.4.0/tonic_textual/classes/tonic_exception.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/services/dataset.py` & `tonic_textual-1.4.0/tonic_textual/services/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/tonic_textual/services/datasetfile.py` & `tonic_textual-1.4.0/tonic_textual/services/datasetfile.py`

 * *Files identical despite different names*

### Comparing `tonic_textual-1.3.0/PKG-INFO` & `tonic_textual-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-textual
-Version: 1.3.0
+Version: 1.4.0
 Summary: Wrappers around the Tonic Textual API
 Home-page: https://www.tonic.ai/
 License: MIT
 Keywords: tonic.ai,tonic,tonic textual
 Author: Adam Kamor
 Author-email: adam@tonic.ai
 Requires-Python: >=3.7,<4.0
```

