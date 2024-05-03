# Comparing `tmp/reasoner_validator-4.1.2.tar.gz` & `tmp/reasoner_validator-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.2.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.3.tar", max compression
```

## Comparing `reasoner_validator-4.1.2.tar` & `reasoner_validator-4.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/README.md
--rw-r--r--   0        0        0      131 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    42104 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2298 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    94288 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    45890 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/message.py
--rw-r--r--   0        0        0    46755 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35576 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/conftest.py
--rw-r--r--   0        0        0   145790 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41308 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36620 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_validation_report.py
--rw-r--r--   0        0        0     3411 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/README.md
+-rw-r--r--   0        0        0      131 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-03 06:58:05.392860 reasoner_validator-4.1.3/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    42104 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2298 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    94451 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    45890 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46754 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35631 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-03 06:58:05.396860 reasoner_validator-4.1.3/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/conftest.py
+-rw-r--r--   0        0        0   146649 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41831 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36620 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3411 2024-05-03 06:58:05.400860 reasoner_validator-4.1.3/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.3/PKG-INFO
```

### Comparing `reasoner_validator-4.1.2/LICENSE` & `reasoner_validator-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/README.md` & `reasoner_validator-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/docs/Makefile` & `reasoner_validator-4.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/docs/conf.py` & `reasoner_validator-4.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/docs/index.rst` & `reasoner_validator-4.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/docs/make.bat` & `reasoner_validator-4.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.3/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/pyproject.toml` & `reasoner_validator-4.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.2"
+version = "4.1.3"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -56,16 +56,16 @@
 
 [tool.poetry.urls]
 "Change Log" = "https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/NCATSTranslator/reasoner-validator/issues"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^69.5.1"
-pytest = "^7.4.2"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.4"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.group.docs.dependencies]
 numpydoc = "^1.5.0"
 sphinx = "^6.2.1"
 myst-parser = "^2.0.0"
 sphinx-rtd-theme = "^1.2.2"
```

### Comparing `reasoner_validator-4.1.2/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.3/reasoner_validator/biolink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1374,17 +1374,19 @@
                 kp_source, found_kp_knowledge_source, kp_source_type,
                 found_primary_knowledge_source,
                 source_trail=source_trail
             )
 
             return source_trail  # may be empty if required RetrievalSource 'sources' entries are missing
 
-    # TODO: 11-Sept-2023: Certain specific 'mixin' predicates used in Knowledge Graphs are being validated for now
-    #       as 'warnings', for short term validation purposes (see reasoner-validator issue #97)
-    PREDICATE_INCLUSIONS = ["biolink:interacts_with"]
+    # TODO: 11-Sept-2023: Certain specific 'mixin' predicates used in
+    #       Knowledge or Query Graphs are being validated for now
+    #       as 'warnings', for short term validation purposes
+    #       (see reasoner-validator issue #97)
+    PREDICATE_INCLUSIONS = ["biolink:interacts_with", 'biolink:treats']
 
     def validate_predicate(
             self,
             edge_id: str,
             predicate: str,
             graph_type: TRAPIGraphType,
             source_trail: Optional[str] = None
@@ -1395,14 +1397,16 @@
 
         :param edge_id: str, identifier of the edge whose predicate is being validated
         :param predicate: str, putative Biolink Model predicate to be validated
         :param source_trail: str, putative Biolink Model predicate to be validated
         :param graph_type: TRAPIGraphType, type of TRAPI graph component being validated
         :return: None (validation communicated via class instance of method)
         """
+        # PREDICATE_INCLUSIONS provides for selective
+        # override of validation of particular predicates
         if predicate not in self.PREDICATE_INCLUSIONS:
 
             graph_type_context: str = graph_type.name.lower()
             if graph_type_context != "input_edge":
                 graph_type_context += ".edge"
             context: str = f"{graph_type_context}.predicate"
```

### Comparing `reasoner_validator-4.1.2/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.3/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/github.py` & `reasoner_validator-4.1.3/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/message.py` & `reasoner_validator-4.1.3/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/report.py` & `reasoner_validator-4.1.3/reasoner_validator/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,15 +821,15 @@
                                                 print(file=file)
                                         else:
                                             # Since we have already checked if messages is None above,
                                             # then we assume here that 'messages' is a List[MESSAGE_PARAMETERS]
                                             # which records distinct additional context
                                             # for a list of messages associated with a given code.
 
-                                            print(f"\t\t\t\t# {identifier}:", file=file)
+                                            print(f"\t\t\t\t# {identifier}", file=file)
                                             first_message: bool = True
                                             messages_per_row: int = 0
                                             num_messages: int = len(messages)
                                             more_msgs: int = num_messages - msg_rows if num_messages > msg_rows else 0
                                             # 'messages' is an instance List[MESSAGE_PARAMETERS] where every entry of
                                             # 'MESSAGE_PARAMETERS' is a dictionary of additional parameters documenting
                                             # a specific instance of validation message related to the given identifier,
```

### Comparing `reasoner_validator-4.1.2/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.3/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.3/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.3/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.3/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/validator.py` & `reasoner_validator-4.1.3/reasoner_validator/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from reasoner_validator.biolink import (
     BMTWrapper,
     BiolinkValidator,
     get_biolink_model_toolkit
 )
 
 from reasoner_validator.report import TRAPIGraphType
-from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, LATEST_TRAPI_MAJOR_MINOR_RELEASE_SEMVER
+from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, TRAPI_1_4_0_SEMVER
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
 from reasoner_validator.versioning import SemVer, SemVerError, get_latest_version
 from reasoner_validator.sri.util import get_aliases
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -56,27 +56,28 @@
             default_test=default_test,
             default_target=default_target if default_target else "Validate TRAPI Response",
             trapi_version=trapi_version,
             biolink_version=biolink_version,
             target_provenance=target_provenance,
             strict_validation=strict_validation
         )
-        self._is_trapi_1_4: Optional[bool] = None
+        self._is_trapi_1_4_or_later: Optional[bool] = None
         self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
 
-    def is_trapi_1_4(self) -> bool:
+    def is_trapi_1_4_or_later(self) -> bool:
         assert self.trapi_version
         try:  # try block ... Sanity check: in case the trapi_version is somehow invalid?
-            target_major_version: SemVer = SemVer.from_string(self.trapi_version, core_fields=['major', 'minor'])
-            self._is_trapi_1_4 = target_major_version >= LATEST_TRAPI_MAJOR_MINOR_RELEASE_SEMVER
+            target_major_version: SemVer = \
+                SemVer.from_string(self.trapi_version, core_fields=['major', 'minor'],  ext_fields=[])
+            self._is_trapi_1_4_or_later = target_major_version >= TRAPI_1_4_0_SEMVER
         except SemVerError as sve:
             logger.error(f"Current TRAPI release '{self.trapi_version}' seems invalid: {str(sve)}. Reset to latest?")
             self.trapi_version = LATEST_TRAPI_RELEASE
-            self._is_trapi_1_4 = True
-        return self._is_trapi_1_4
+            self._is_trapi_1_4_or_later = True
+        return self._is_trapi_1_4_or_later
 
     def sanitize_workflow(self, response: Dict) -> Dict:
         """
         Workflows in TRAPI Responses cannot be validated further due to missing tags and None values.
         This method is a temporary workaround to sanitize the query for additional validation.
 
         :param response: Dict full TRAPI Response JSON object
@@ -374,15 +375,15 @@
                 results_sample = self.sample_results(results, sample_size=sample_size)
                 for result in results_sample:
 
                     # generally validate against the pertinent schema
                     self.is_valid_trapi_query(instance=result, component="Result")
 
                     # Maybe some additional TRAPI-release specific non-schematic validation here?
-                    if self.is_trapi_1_4():
+                    if self.is_trapi_1_4_or_later():
                         # TODO: implement me!
                         pass
                     else:
                         pass
 
                     # TODO: here, we could try to compare the Results against the contents of the KnowledgeGraph,
                     #       with respect to node input values from the QueryGraph, but this is tricky to do solely
@@ -504,15 +505,15 @@
                         if subject_id == details["id"]:
                             subject_id_found = True
                         if object_id == details["id"]:
                             object_id_found = True
 
             # However, TRAPI 1.4.0 Message 'Results' 'edge_bindings' are reported differently
             #          from 1.3.0, rather, embedded in 'Analysis' objects (and 'Auxiliary Graphs')
-            if self.is_trapi_1_4():
+            if self.is_trapi_1_4_or_later():
                 #
                 #     "auxiliary_graphs": {
                 #         "a0": {
                 #             "edges": [
                 #                 "e02",
                 #                 "e12"
                 #             ]
```

### Comparing `reasoner_validator-4.1.2/reasoner_validator/versioning.py` & `reasoner_validator-4.1.3/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.3/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/__init__.py` & `reasoner_validator-4.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.3/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1000,33 +1000,60 @@
             ""
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 26: Query edge predicate is a mixin; default 'strict_validation' == False for query graphs
             {
                 "nodes": {
-                    "IRS1": {"ids": ["HGNC:6125"], "categories": ["biolink:Gene"]},
                     "drug": {
+                        "ids": ["RXCUI:861026"],
                         "categories": ["biolink:Drug"]
-                    }
+                    },
+                    "gene": {
+                        "categories": ["biolink:Gene"]
+                    },
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:increases_amount_or_activity_of"],
-                        "object": "IRS1"
+                        "predicates": ["biolink:increases amount or activity of"],
+                        "object": "disease"
                     }
                 }
             },
-            # f"{QUERY_GRAPH_PREFIX}: INFO - Predicate element 'biolink:increases_amount_or_activity_of' is a mixin."
+            # f"{QUERY_GRAPH_PREFIX}: INFO - Predicate element 'biolink:treats' is a mixin."
             "info.query_graph.edge.predicate.mixin"
         ),
         (
+            "4.1.6",
+            # Query 27: Query edge 'treats' predicate is a special case of mixin;
+            #           default 'strict_validation' == False for query graphs
+            {
+                "nodes": {
+                    "drug": {
+                        "ids": ["RXCUI:861026"],
+                        "categories": ["biolink:Drug"]
+                    },
+                    "disease": {
+                        "categories": ["biolink:Disease"]
+                    },
+                },
+                "edges": {
+                    "treats": {
+                        "subject": "drug",
+                        "predicates": ["biolink:treats"],
+                        "object": "disease"
+                    }
+                }
+            },
+            ""
+        ),
+        (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 27: ... but if present, predicates must be valid
+            # Query 28: ... but if present, predicates must be valid
             #           for the specified Biolink Model version, but...
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
@@ -1041,15 +1068,15 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         ),
         (
             SUPPRESS_BIOLINK_MODEL_VALIDATION,
-            # Query 28: Query edge predicate is a mixin...but...
+            # Query 29: Query edge predicate is a mixin...but...
             {
                 "nodes": {
                     "IRS1": {"ids": ["HGNC:6125"], "categories": ["biolink:Gene"]},
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
```

### Comparing `reasoner_validator-4.1.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/test_response_validator.py` & `reasoner_validator-4.1.3/tests/test_response_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
-from typing import Dict
+from typing import Dict, Optional
 from sys import stderr
 
 import logging
 
 from copy import deepcopy
 
 import pytest
 
 from dictdiffer import diff
 
 from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_2
 from reasoner_validator.validator import TRAPIResponseValidator
-from reasoner_validator.report import TRAPIGraphType
 
 from tests import PATCHED_140_SCHEMA_FILEPATH, SAMPLE_NODES_WITH_ATTRIBUTES, DEFAULT_KL_AND_AT_ATTRIBUTES
 from tests.test_validation_report import check_messages
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
@@ -425,14 +424,33 @@
     reference_response = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
     assert input_response == reference_response
     validator.check_compliance_of_trapi_response(response=input_response)
     assert not list(diff(input_response, reference_response))
 
 
 @pytest.mark.parametrize(
+    "trapi_version,outcome",
+    [
+        ("1.3.0", False),
+        ("1.4.0", True),
+        ("1.4.2", True),
+        ("1.5.0-beta", True),
+        ("1.5.0", True),
+
+        # since the latest default (as of test creation)
+        # is 1.5 something, then 'None' should also be true
+        (None, True)
+    ]
+)
+def test_is_trapi_1_4_or_later(trapi_version: Optional[str], outcome: bool):
+    validator: TRAPIResponseValidator = TRAPIResponseValidator(trapi_version=trapi_version)
+    assert validator.is_trapi_1_4_or_later() is outcome
+
+
+@pytest.mark.parametrize(
     "edges_limit,number_of_nodes_returned,number_of_edges_returned",
     [
         (   # Query 0 - unlimited sample whole graph
             0,  # edges_limit
             len(SAMPLE_NODES),  # number of nodes returned
             len(SAMPLE_EDGES)   # number of edges returned
         ),
```

### Comparing `reasoner_validator-4.1.2/tests/test_semver.py` & `reasoner_validator-4.1.3/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.3/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/test_validate.py` & `reasoner_validator-4.1.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/test_validation_report.py` & `reasoner_validator-4.1.3/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/tests/test_workflows.py` & `reasoner_validator-4.1.3/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.2/PKG-INFO` & `reasoner_validator-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.2
+Version: 4.1.3
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

