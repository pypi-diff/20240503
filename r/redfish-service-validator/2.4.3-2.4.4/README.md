# Comparing `tmp/redfish_service_validator-2.4.3.tar.gz` & `tmp/redfish_service_validator-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_service_validator-2.4.3.tar", last modified: Fri Apr 12 19:43:46 2024, max compression
+gzip compressed data, was "redfish_service_validator-2.4.4.tar", last modified: Fri May  3 20:42:44 2024, max compression
```

## Comparing `redfish_service_validator-2.4.3.tar` & `redfish_service_validator-2.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.766147 redfish_service_validator-2.4.3/redfish_service_validator/
--rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/RedfishLogo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16498 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidatorGui.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50066 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/schema_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/traverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/validateRedfish.py
--rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/tests/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/redfish_service_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/RedfishLogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16498 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidatorGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50066 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/schema_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30785 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/validateRedfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/tests/test_catalog.py
```

### Comparing `redfish_service_validator-2.4.3/LICENSE.md` & `redfish_service_validator-2.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/PKG-INFO` & `redfish_service_validator-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.4.3
+Version: 2.4.4
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.4.3/README.md` & `redfish_service_validator-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/RedfishLogo.py` & `redfish_service_validator-2.4.4/redfish_service_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidator.py` & `redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from redfish_service_validator.metadata import getSchemaDetails
 from redfish_service_validator.config import convert_config_to_args, convert_args_to_config
 from redfish_service_validator.validateResource import validateSingleURI, validateURITree
 from redfish_service_validator import tohtml, schema_pack, traverse
 from urllib.parse import urlparse
 from collections import Counter
 
-tool_version = '2.4.3'
+tool_version = '2.4.4'
 
 # Set up the custom debug levels
 VERBOSE1 = logging.INFO-1
 VERBOSE2 = logging.INFO-2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidatorGui.py` & `redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidatorGui.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/catalog.py` & `redfish_service_validator-2.4.4/redfish_service_validator/catalog.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/config.py` & `redfish_service_validator-2.4.4/redfish_service_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/helper.py` & `redfish_service_validator-2.4.4/redfish_service_validator/helper.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/metadata.py` & `redfish_service_validator-2.4.4/redfish_service_validator/metadata.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/schema_pack.py` & `redfish_service_validator-2.4.4/redfish_service_validator/schema_pack.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/tohtml.py` & `redfish_service_validator-2.4.4/redfish_service_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/traverse.py` & `redfish_service_validator-2.4.4/redfish_service_validator/traverse.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/validateRedfish.py` & `redfish_service_validator-2.4.4/redfish_service_validator/validateRedfish.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
     if not oem_check:
         if 'Oem' in prop_name or 'Resource.OemObject' in prop.Type.getTypeTree():
             my_logger.verbose1('\tOem is skipped')
             counts['skipOem'] += 1
             return {prop_name: ('-', '-', 'Yes' if prop.Exists else 'No', 'OEM')}, counts
 
     # Parameter Passes
-    paramPass = propMandatoryPass = propNullablePass = deprecatedPassOrSinceVersion = nullValid = True
+    paramPass = propMandatoryPass = propNullablePass = deprecatedPassOrSinceVersion = nullValid = permissionValid = True
 
     if prop.Type.IsMandatory:
         propMandatoryPass = True if prop.Exists else False
         my_logger.verbose1("\tMandatory Test: {}".format('OK' if propMandatoryPass else 'FAIL'))
     else:
         my_logger.verbose1("\tis Optional")
         if not prop.Exists:
@@ -546,14 +546,22 @@
                     nullValid = False
                 if val.lower() == 'null':
                     my_logger.warning('{}: "null" string found - Did you mean to use an actual null value?'.format(sub_item))
                     nullValid = False
 
             if prop.Exists:
                 paramPass = propNullablePass = True
+
+                #   <Annotation Term="OData.Permissions" EnumMember="OData.Permission/ReadWrite"/>
+                if prop.Type.Permissions == "OData.Permission/Write" or prop.Type.Permissions == "OData.Permission/None":
+                    if val is not None:
+                        my_logger.error('{}: Permissions for this property are Write only, reading this property should be null!!!'.format(sub_item))
+                        permissionValid = False
+                        counts['failWriteOnly'] += 1
+
                 if val is None:
                     if propNullable:
                         my_logger.debug('Property {} is nullable and is null, so Nullable checking passes'.format(sub_item))
                     else:
                         propNullablePass = False
                 
                 if isinstance(prop.Type, str) and 'Edm.' in prop.Type:
@@ -573,15 +581,15 @@
                     paramPass = validateEntity(service, prop, val)
                 
 
 
             # Render our result
             my_type = prop.Type.fulltype
 
-            if all([paramPass, propMandatoryPass, propNullablePass, excerptPass]):
+            if all([paramPass, propMandatoryPass, propNullablePass, excerptPass, permissionValid]):
                 my_logger.verbose1("\tSuccess")
                 counts['pass'] += 1
                 result_str = 'PASS'
                 if deprecatedPassOrSinceVersion is False:
                     result_str = 'Deprecated'
                 if isinstance(deprecatedPassOrSinceVersion, str):
                     result_str = 'Deprecated/{}'.format(deprecatedPassOrSinceVersion)
```

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator/validateResource.py` & `redfish_service_validator-2.4.4/redfish_service_validator/validateResource.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator.egg-info/PKG-INFO` & `redfish_service_validator-2.4.4/redfish_service_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.4.3
+Version: 2.4.4
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.4.3/redfish_service_validator.egg-info/SOURCES.txt` & `redfish_service_validator-2.4.4/redfish_service_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.3/setup.py` & `redfish_service_validator-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_service_validator",
-    version="2.4.3",
+    version="2.4.4",
     description="Redfish Service Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `redfish_service_validator-2.4.3/tests/test_catalog.py` & `redfish_service_validator-2.4.4/tests/test_catalog.py`

 * *Files identical despite different names*

