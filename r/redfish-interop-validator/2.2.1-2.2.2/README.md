# Comparing `tmp/redfish_interop_validator-2.2.1.tar.gz` & `tmp/redfish_interop_validator-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_interop_validator-2.2.1.tar", last modified: Fri Apr 19 19:58:50 2024, max compression
+gzip compressed data, was "redfish_interop_validator-2.2.2.tar", last modified: Fri May  3 20:43:26 2024, max compression
```

## Comparing `redfish_interop_validator-2.2.1.tar` & `redfish_interop_validator-2.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/redfish_interop_validator/
--rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishInteropValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24266 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishLogo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/interop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/redfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/traverseInterop.py
--rw-r--r--   0 runner    (1001) docker     (127)    21798 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:26.175496 redfish_interop_validator-2.2.2/redfish_interop_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishInteropValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24266 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishLogo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39575 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/redfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/traverseInterop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/redfish_interop_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 20:43:26.000000 redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:43:26.179496 redfish_interop_validator-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 20:43:16.000000 redfish_interop_validator-2.2.2/setup.py
```

### Comparing `redfish_interop_validator-2.2.1/LICENSE.md` & `redfish_interop_validator-2.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/PKG-INFO` & `redfish_interop_validator-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_interop_validator
-Version: 2.2.1
+Version: 2.2.2
 Summary: Redfish Interop Validator
 Home-page: https://github.com/DMTF/Redfish-Interop-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_interop_validator-2.2.1/README.md` & `redfish_interop_validator-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishInteropValidator.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishInteropValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from urllib.parse import urlparse
 from collections import Counter
 
 import redfish_interop_validator.traverseInterop as traverseInterop
 from redfish_interop_validator.profile import getProfiles, checkProfileAgainstSchema, hashProfile
 from redfish_interop_validator.validateResource import validateSingleURI, validateURITree
 
-tool_version = '2.2.1'
+tool_version = '2.2.2'
 
 # Set up the custom debug levels
 VERBOSE1 = logging.INFO - 1
 VERBOSE2 = logging.INFO - 2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishLogo.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/config.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/interop.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,15 @@
         return msgInterop('WriteRequirement', profile_entry, expected_str, '@Redfish.WriteableProperties not an array', testResultEnum.WARN), True
 
     is_writeable = item_name in writeable_properties
 
     return msgInterop('WriteRequirement', profile_entry, expected_str, 'Writable' if is_writeable else 'Not Writable',
                       testResultEnum.PASS if is_writeable else result_not_supported), True
 
+
 def checkComparison(val, compareType, target):
     """
     Validate a given comparison option, given a value and a target set
     """
     my_logger.verbose1('Testing a comparison \n\t' + str((val, compareType, target)))
     vallist = val if isinstance(val, list) else [val]
     paramPass = False
@@ -553,15 +554,16 @@
             cnt += 1
 
     else:
         # consider requirement before anything else
         # problem: if dne, skip?
 
         # Read Requirement is default mandatory if not present
-        msg, success = validateRequirement(profile_entry.get('ReadRequirement', 'Mandatory'), redfish_value, parent_object_tuple=redfish_parent_payload)
+        requirement_entry = profile_entry.get('ReadRequirement', 'Mandatory')
+        msg, requirement_success = validateRequirement(requirement_entry, redfish_value, parent_object_tuple=redfish_parent_payload)
         msgs.append(msg)
         msg.name = item_name + '.' + msg.name
 
         if "WriteRequirement" in profile_entry:
             headers = propResourceObj.headers
             msg, success = validateWriteRequirement(profile_entry.get('WriteRequirement', 'Mandatory'), redfish_parent_payload, headers, item_name)
             msgs.append(msg)
@@ -578,15 +580,20 @@
             if not success:
                 my_logger.error("MinSupportValues failed")
 
         if "Values" in profile_entry:
             # Default to AnyOf
 
             my_compare = profile_entry.get("Comparison", "AnyOf")
-            msg, success = checkComparison(redfish_value, my_compare, profile_entry.get("Values", []))
+            my_values = profile_entry.get("Values", [])
+            # If absent and not comparing for absence...
+            if redfish_value == REDFISH_ABSENT and my_compare not in ['Absent', 'Present']:
+                msg, success = msgInterop('Comparison', my_values, my_compare, REDFISH_ABSENT, testResultEnum.NOT_TESTED), True
+            else:
+                msg, success = checkComparison(redfish_value, my_compare, my_values)
             msgs.append(msg)
             msg.name = item_name + '.' + msg.name
 
             # Embed test results into profile, going forward seems to be the quick option outside of making a proper test object
             if my_compare in ['AnyOf', 'AllOf']:
                 msg.ignore = True
                 if not profile_entry.get('_msgs'):
@@ -616,72 +623,117 @@
     rf_payload_item, rf_payload = rf_payload_tuple
     rf_payload_action = None
     counts = Counter()
     msgs = []
     my_logger.verbose1('actionRequirement \n\tval: ' + str(rf_payload_item if not isinstance(
         rf_payload_item, dict) else 'dict') + ' ' + str(profile_entry))
 
+    action_readrequirement = profile_entry.get('ReadRequirement', "Mandatory")
+    actioninfo_requirement = profile_entry.get('ActionInfo', "None")
+
     if "ReadRequirement" in profile_entry:
         # problem: if dne, skip
-        msg, success = validateRequirement(profile_entry.get('ReadRequirement', "Mandatory"), rf_payload_item)
+        msg, success = validateRequirement(action_readrequirement, rf_payload_item)
         msgs.append(msg)
         msg.name = actionname + '.' + msg.name
         msg.success = testResultEnum.PASS if success else testResultEnum.FAIL
-
+    
     propDoesNotExist = (rf_payload_item == REDFISH_ABSENT)
     if propDoesNotExist:
         return msgs, counts
+
     if "@Redfish.ActionInfo" in rf_payload_item:
         vallink = rf_payload_item['@Redfish.ActionInfo']
         success, rf_payload_action, code, elapsed, _ = callResourceURI(vallink)
         if not success:
             rf_payload_action = None
 
+    if 'ActionInfo' in profile_entry and actioninfo_requirement in ["None"]:
+        # Create message if None is explicitly listed in the profile
+        msg = msgInterop('ActionInfo', 'None', '-', '-', testResultEnum.OK)
+        msg.name = actionname + '.' + msg.name
+        msgs.append(msg)
+
+    if actioninfo_requirement not in ["None"]:
+        if propDoesNotExist:
+            # not tested if action isn't present
+            msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.NOT_TESTED)
+
+        elif actioninfo_requirement == "Mandatory":
+            if rf_payload_action is None:
+                if "@Redfish.ActionInfo" in rf_payload_item:
+                    my_logger.error('Mandatory @Redfish.ActionInfo for {} listed on action but URI get was not successful'.format(actionname))
+                else:
+                    my_logger.error('@Redfish.ActionInfo for {} not listed, but is Mandatory'.format(actionname))
+                msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.FAIL)
+            else:
+                msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.PASS)
+
+        elif actioninfo_requirement == "Recommended":
+            if rf_payload_action is None:
+                if "@Redfish.ActionInfo" in rf_payload_item:
+                    my_logger.warn('Recommended @Redfish.ActionInfo for {} listed on action but URI get was not successful'.format(actionname))
+                    msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.WARN)
+                else:
+                    my_logger.info('Recommended @Redfish.ActionInfo for {} not listed'.format(actionname))
+                    msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.PASS)
+            else:
+                msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.PASS)
+
+        else:
+            my_logger.warn('Term "ActionInfo" has unknown value {}'.format(actioninfo_requirement))
+            msg = msgInterop('ActionInfo', actioninfo_requirement, '-', '-', testResultEnum.WARN)
+        msg.name = actionname + '.' + msg.name
+        msgs.append(msg)
+
     # problem: if dne, skip
     if "Parameters" in profile_entry:
-        innerDict = profile_entry["Parameters"]
+        parameter_dictionary = profile_entry["Parameters"]
         # problem: if dne, skip
         # assume mandatory
-        for k in innerDict:
-            item = innerDict[k]
+        for param in parameter_dictionary:
+            item = parameter_dictionary[param]
+            # Get Allowable Values for parameter
             values_array = None
+            # If our action info exists at all, prefer it
             if rf_payload_action is not None:
-                action_by_name = rf_payload_action['Parameters']
-                my_action = [x for x in action_by_name if x['Name'] == k]
-                if my_action:
-                    values_array = my_action[0].get('AllowableValues')
+                parameter_by_name = rf_payload_action['Parameters']
+                my_parameter = [x for x in parameter_by_name if x['Name'] == param]
+                if my_parameter:
+                    values_array = my_parameter[0].get('AllowableValues')
+            # Otherwise check for AllowableValues as additional property
             if values_array is None:
-                values_array = rf_payload_item.get(str(k) + '@Redfish.AllowableValues', REDFISH_ABSENT)
+                values_array = rf_payload_item.get(str(param) + '@Redfish.AllowableValues', REDFISH_ABSENT)
             if values_array == REDFISH_ABSENT:
-                my_logger.warning('\tNo such ActionInfo exists for this Action, and no AllowableValues exists.  Cannot validate the following parameters: {}'.format(k))
+                my_logger.warning('\tNo such ActionInfo exists for this Action, and no AllowableValues exists.  Cannot validate the following parameters: {}'.format(param))
                 msg = msgInterop('', item, '-', '-', testResultEnum.WARN)
-                msg.name = "{}.{}.{}".format(actionname, k, msg.name)
+                msg.name = "{}.{}.{}".format(actionname, param, msg.name)
                 msgs.append(msg)
             else:
                 msg, success = validateRequirement(item.get('ReadRequirement', "Mandatory"), values_array)
                 msgs.append(msg)
-                msg.name = "{}.{}.{}".format(actionname, k, msg.name)
+                msg.name = "{}.{}.{}".format(actionname, param, msg.name)
                 if "ParameterValues" in item:
                     msg, success = validateSupportedValues(
                             item["ParameterValues"], values_array)
                     msgs.append(msg)
-                    msg.name = "{}.{}.{}".format(actionname, k, msg.name)
+                    msg.name = "{}.{}.{}".format(actionname, param, msg.name)
                 if "RecommendedValues" in item:
                     msg, success = validateSupportedValues(
                             item["RecommendedValues"], values_array)
                     msg.name = msg.name.replace('Supported', 'Recommended')
                     if config['WarnRecommended'] and not success:
                         my_logger.warning('\tRecommended parameters do not all exist, escalating to WARN')
                         msg.success = testResultEnum.WARN
                     elif not success:
                         my_logger.warning('\tRecommended parameters do not all exist, but are not Mandatory')
                         msg.success = testResultEnum.PASS
 
                     msgs.append(msg)
-                    msg.name = "{}.{}.{}".format(actionname, k, msg.name)
+                    msg.name = "{}.{}.{}".format(actionname, param, msg.name)
     # consider requirement before anything else, what if action
     # if the action doesn't exist, you can't check parameters
     # if it doesn't exist, what should not be checked for action
     return msgs, counts
 
 
 URI_ID_REGEX = '\{[A-Za-z0-9]*Id\}'
```

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/profile.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/profile.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/redfish.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/redfish.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/session.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/session.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/tohtml.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/traverseInterop.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/traverseInterop.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator/validateResource.py` & `redfish_interop_validator-2.2.2/redfish_interop_validator/validateResource.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,17 @@
         if any(x in key for x in ['problem', 'fail', 'bad', 'exception']):
             pass_val = False
             break
     my_logger.info("\t {}".format('PASS' if pass_val else ' FAIL...'))
 
     for msg in results[uriName]['messages']:
         msg.parent_results = results
+        if msg.success == interop.testResultEnum.NOT_TESTED:
+            counts['notTested'] += 1
+
 
     return True, counts, results, (links, limited_links), resource_obj
 
 
 urlCheck = re.compile(r"http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+")
 allowable_annotations = ['@odata.id']
```

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/PKG-INFO` & `redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_interop_validator
-Version: 2.2.1
+Version: 2.2.2
 Summary: Redfish Interop Validator
 Home-page: https://github.com/DMTF/Redfish-Interop-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/SOURCES.txt` & `redfish_interop_validator-2.2.2/redfish_interop_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.1/setup.py` & `redfish_interop_validator-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_interop_validator",
-    version="2.2.1",
+    version="2.2.2",
     description="Redfish Interop Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

