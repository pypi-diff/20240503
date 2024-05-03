# Comparing `tmp/iam_actions-1.2.20240501.tar.gz` & `tmp/iam_actions-1.2.20240502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240501.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240502.tar", max compression
```

## Comparing `iam_actions-1.2.20240501.tar` & `iam_actions-1.2.20240502.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/README.md
--rw-r--r--   0        0        0      228 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/__init__.py
--rw-r--r--   0        0        0  4821473 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-01 02:23:20.151558 iam_actions-1.2.20240501/iam_actions/generate/services.py
--rw-r--r--   0        0        0   627134 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/policies.json
--rw-r--r--   0        0        0   209154 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   608541 2024-05-01 02:24:40.735637 iam_actions-1.2.20240501/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-01 02:24:41.391637 iam_actions-1.2.20240501/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240501/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240501/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/README.md
+-rw-r--r--   0        0        0      228 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4824523 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-02 02:18:40.934717 iam_actions-1.2.20240502/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   627645 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/policies.json
+-rw-r--r--   0        0        0   209154 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   609039 2024-05-02 02:20:22.234313 iam_actions-1.2.20240502/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-02 02:20:22.894311 iam_actions-1.2.20240502/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240502/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240502/PKG-INFO
```

### Comparing `iam_actions-1.2.20240501/LICENSE` & `iam_actions-1.2.20240502/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/README.md` & `iam_actions-1.2.20240502/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/actions.json` & `iam_actions-1.2.20240502/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998098914919131%*

 * *Differences: {"'sms-voice'": "{'DescribeProtectConfigurations': OrderedDict([('access_level', 'Undocumented'), "*

 * *                "('action', 'DescribeProtectConfigurations'), ('condition_keys', []), "*

 * *                "('description', 'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *                "'SendMediaMessage': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                "'SendMediaMessage'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *                "AWS'), ('o […]*

```diff
@@ -151936,14 +151936,22 @@
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "Pool",
                 "SenderId"
             ]
         },
+        "AssociateProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "AssociateProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateConfigurationSet": {
             "access_level": "Write",
             "action": "CreateConfigurationSet",
             "condition_keys": [],
             "description": "Create a new configuration set. After you create the configuration set, you can add one or more event destinations to it.",
             "orphan": false,
             "resources": []
@@ -151987,14 +151995,22 @@
             "description": "Grants permission to create a pool",
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "SenderId"
             ]
         },
+        "CreateProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "CreateProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateRegistration": {
             "access_level": "Write",
             "action": "CreateRegistration",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -152041,14 +152057,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a verified destination number",
             "orphan": false,
             "resources": []
         },
+        "DeleteAccountDefaultProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "DeleteAccountDefaultProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteConfigurationSet": {
             "access_level": "Write",
             "action": "DeleteConfigurationSet",
             "condition_keys": [],
             "description": "Deletes an existing configuration set.",
             "orphan": false,
             "resources": []
@@ -152098,14 +152122,22 @@
             "description": "Grants permission to delete a keyword for a pool or origination phone number",
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "Pool"
             ]
         },
+        "DeleteMediaMessageSpendLimitOverride": {
+            "access_level": "Undocumented",
+            "action": "DeleteMediaMessageSpendLimitOverride",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteOptOutList": {
             "access_level": "Write",
             "action": "DeleteOptOutList",
             "condition_keys": [],
             "description": "Grants permission to delete an opt-out list",
             "orphan": false,
             "resources": [
@@ -152128,14 +152160,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a pool",
             "orphan": false,
             "resources": [
                 "Pool"
             ]
         },
+        "DeleteProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "DeleteProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteRegistration": {
             "access_level": "Write",
             "action": "DeleteRegistration",
             "condition_keys": [],
             "description": "Grants permission to delete a registration",
             "orphan": false,
             "resources": [
@@ -152261,14 +152301,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe the pools in your account",
             "orphan": false,
             "resources": [
                 "Pool"
             ]
         },
+        "DescribeProtectConfigurations": {
+            "access_level": "Undocumented",
+            "action": "DescribeProtectConfigurations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeRegistrationAttachments": {
             "access_level": "Read",
             "action": "DescribeRegistrationAttachments",
             "condition_keys": [],
             "description": "Grants permission to describe the registration attachments in your account",
             "orphan": false,
             "resources": [
@@ -152365,14 +152413,22 @@
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "Pool",
                 "SenderId"
             ]
         },
+        "DisassociateProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "DisassociateProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DiscardRegistrationVersion": {
             "access_level": "Write",
             "action": "DiscardRegistrationVersion",
             "condition_keys": [],
             "description": "Grants permission to discard the latest version of a given registration",
             "orphan": false,
             "resources": [
@@ -152383,14 +152439,22 @@
             "access_level": "Read",
             "action": "GetConfigurationSetEventDestinations",
             "condition_keys": [],
             "description": "Obtain information about an event destination, including the types of events it reports, the Amazon Resource Name (ARN) of the destination, and the name of the event destination.",
             "orphan": false,
             "resources": []
         },
+        "GetProtectConfigurationCountryRuleSet": {
+            "access_level": "Undocumented",
+            "action": "GetProtectConfigurationCountryRuleSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListConfigurationSets": {
             "access_level": "Read",
             "action": "ListConfigurationSets",
             "condition_keys": [],
             "description": "Return a list of configuration sets. This operation only returns the configuration sets that are associated with your account in the current AWS Region.",
             "orphan": false,
             "resources": []
@@ -152512,14 +152576,22 @@
             "orphan": false,
             "resources": [
                 "PhoneNumber",
                 "Pool",
                 "SenderId"
             ]
         },
+        "SendMediaMessage": {
+            "access_level": "Undocumented",
+            "action": "SendMediaMessage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SendTextMessage": {
             "access_level": "Write",
             "action": "SendTextMessage",
             "condition_keys": [],
             "description": "Grants permission to send a text message to a destination phone number",
             "orphan": false,
             "resources": [
@@ -152532,14 +152604,22 @@
             "access_level": "Write",
             "action": "SendVoiceMessage",
             "condition_keys": [],
             "description": "Create a new voice message and send it to a recipient's phone number.",
             "orphan": false,
             "resources": []
         },
+        "SetAccountDefaultProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "SetAccountDefaultProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SetDefaultMessageType": {
             "access_level": "Write",
             "action": "SetDefaultMessageType",
             "condition_keys": [],
             "description": "Grants permission to set the default message type for a configuration set",
             "orphan": false,
             "resources": [
@@ -152552,14 +152632,22 @@
             "condition_keys": [],
             "description": "Grants permission to set the default sender ID for a configuration set",
             "orphan": false,
             "resources": [
                 "ConfigurationSet"
             ]
         },
+        "SetMediaMessageSpendLimitOverride": {
+            "access_level": "Undocumented",
+            "action": "SetMediaMessageSpendLimitOverride",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SetTextMessageSpendLimitOverride": {
             "access_level": "Write",
             "action": "SetTextMessageSpendLimitOverride",
             "condition_keys": [],
             "description": "Grants permission to set an override for your account's text messaging monthly spend limit",
             "orphan": false,
             "resources": []
@@ -152655,14 +152743,30 @@
             "condition_keys": [],
             "description": "Grants permission to update a pool's configuration",
             "orphan": false,
             "resources": [
                 "Pool"
             ]
         },
+        "UpdateProtectConfiguration": {
+            "access_level": "Undocumented",
+            "action": "UpdateProtectConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateProtectConfigurationCountryRuleSet": {
+            "access_level": "Undocumented",
+            "action": "UpdateProtectConfigurationCountryRuleSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateSenderId": {
             "access_level": "Write",
             "action": "UpdateSenderId",
             "condition_keys": [],
             "description": "Grants permission to update a sender ID's configuration",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20240501/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240502/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240502/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/generate/generate.py` & `iam_actions-1.2.20240502/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240502/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240502/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/generate/services.py` & `iam_actions-1.2.20240502/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/policies.json` & `iam_actions-1.2.20240502/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999983927758986%*

 * *Differences: {"'serviceMap'": "{'Amazon Pinpoint SMS Voice V2': {'Actions': {insert: [(1, "*

 * *                 "'AssociateProtectConfiguration'), (6, 'CreateProtectConfiguration'), (12, "*

 * *                 "'DeleteAccountDefaultProtectConfiguration'), (18, "*

 * *                 "'DeleteMediaMessageSpendLimitOverride'), (22, 'DeleteProtectConfiguration'), "*

 * *                 "(37, 'DescribeProtectConfigurations'), (49, 'DisassociateProtectConfiguration'), "*

 * *                 "(51, 'GetProtectConfigurationCountryRuleSet'), (63, ' […]*

```diff
@@ -18707,80 +18707,93 @@
             ]
         },
         "Amazon Pinpoint SMS Voice V2": {
             "ARNFormat": "arn:aws:sms-voice:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:sms-voice:.+",
             "Actions": [
                 "AssociateOriginationIdentity",
+                "AssociateProtectConfiguration",
                 "CreateConfigurationSet",
                 "CreateEventDestination",
                 "CreateOptOutList",
                 "CreatePool",
+                "CreateProtectConfiguration",
                 "CreateRegistration",
                 "CreateRegistrationAssociation",
                 "CreateRegistrationAttachment",
                 "CreateRegistrationVersion",
                 "CreateVerifiedDestinationNumber",
+                "DeleteAccountDefaultProtectConfiguration",
                 "DeleteConfigurationSet",
                 "DeleteDefaultMessageType",
                 "DeleteDefaultSenderId",
                 "DeleteEventDestination",
                 "DeleteKeyword",
+                "DeleteMediaMessageSpendLimitOverride",
                 "DeleteOptOutList",
                 "DeleteOptedOutNumber",
                 "DeletePool",
+                "DeleteProtectConfiguration",
                 "DeleteRegistration",
                 "DeleteRegistrationAttachment",
                 "DeleteRegistrationFieldValue",
                 "DeleteTextMessageSpendLimitOverride",
                 "DeleteVerifiedDestinationNumber",
                 "DeleteVoiceMessageSpendLimitOverride",
                 "DescribeAccountAttributes",
                 "DescribeAccountLimits",
                 "DescribeConfigurationSets",
                 "DescribeKeywords",
                 "DescribeOptOutLists",
                 "DescribeOptedOutNumbers",
                 "DescribePhoneNumbers",
                 "DescribePools",
+                "DescribeProtectConfigurations",
                 "DescribeRegistrationAttachments",
                 "DescribeRegistrationFieldDefinitions",
                 "DescribeRegistrationFieldValues",
                 "DescribeRegistrationSectionDefinitions",
                 "DescribeRegistrationTypeDefinitions",
                 "DescribeRegistrationVersions",
                 "DescribeRegistrations",
                 "DescribeSenderIds",
                 "DescribeSpendLimits",
                 "DescribeVerifiedDestinationNumbers",
                 "DisassociateOriginationIdentity",
+                "DisassociateProtectConfiguration",
                 "DiscardRegistrationVersion",
+                "GetProtectConfigurationCountryRuleSet",
                 "ListPoolOriginationIdentities",
                 "ListRegistrationAssociations",
                 "ListTagsForResource",
                 "PutKeyword",
                 "PutOptedOutNumber",
                 "PutRegistrationFieldValue",
                 "ReleasePhoneNumber",
                 "ReleaseSenderId",
                 "RequestPhoneNumber",
                 "RequestSenderId",
                 "SendDestinationNumberVerificationCode",
+                "SendMediaMessage",
                 "SendTextMessage",
                 "SendVoiceMessage",
+                "SetAccountDefaultProtectConfiguration",
                 "SetDefaultMessageType",
                 "SetDefaultSenderId",
+                "SetMediaMessageSpendLimitOverride",
                 "SetTextMessageSpendLimitOverride",
                 "SetVoiceMessageSpendLimitOverride",
                 "SubmitRegistrationVersion",
                 "TagResource",
                 "UntagResource",
                 "UpdateEventDestination",
                 "UpdatePhoneNumber",
                 "UpdatePool",
+                "UpdateProtectConfiguration",
+                "UpdateProtectConfigurationCountryRuleSet",
                 "UpdateSenderId",
                 "VerifyDestinationNumber"
             ],
             "HasResource": true,
             "StringPrefix": "sms-voice",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
```

### Comparing `iam_actions-1.2.20240501/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240502/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240501/iam_actions/services.json` & `iam_actions-1.2.20240502/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999984157624326%*

 * *Differences: {"'sms-voice'": "{'Actions': {insert: [(1, 'AssociateProtectConfiguration'), (7, "*

 * *                "'CreateProtectConfiguration'), (13, 'DeleteAccountDefaultProtectConfiguration'), "*

 * *                "(20, 'DeleteMediaMessageSpendLimitOverride'), (24, 'DeleteProtectConfiguration'), "*

 * *                "(39, 'DescribeProtectConfigurations'), (51, 'DisassociateProtectConfiguration'), "*

 * *                "(54, 'GetProtectConfigurationCountryRuleSet'), (67, 'SendMediaMessage'), (70, "*

 * *                "'SetAccountDef […]*

```diff
@@ -21198,85 +21198,98 @@
         ],
         "ARNRegexes": [
             "^arn:aws:sms-voice:.+",
             "^arn:aws:sms-voice:.+:.+:.+"
         ],
         "Actions": [
             "AssociateOriginationIdentity",
+            "AssociateProtectConfiguration",
             "CreateConfigurationSet",
             "CreateConfigurationSetEventDestination",
             "CreateEventDestination",
             "CreateOptOutList",
             "CreatePool",
+            "CreateProtectConfiguration",
             "CreateRegistration",
             "CreateRegistrationAssociation",
             "CreateRegistrationAttachment",
             "CreateRegistrationVersion",
             "CreateVerifiedDestinationNumber",
+            "DeleteAccountDefaultProtectConfiguration",
             "DeleteConfigurationSet",
             "DeleteConfigurationSetEventDestination",
             "DeleteDefaultMessageType",
             "DeleteDefaultSenderId",
             "DeleteEventDestination",
             "DeleteKeyword",
+            "DeleteMediaMessageSpendLimitOverride",
             "DeleteOptOutList",
             "DeleteOptedOutNumber",
             "DeletePool",
+            "DeleteProtectConfiguration",
             "DeleteRegistration",
             "DeleteRegistrationAttachment",
             "DeleteRegistrationFieldValue",
             "DeleteTextMessageSpendLimitOverride",
             "DeleteVerifiedDestinationNumber",
             "DeleteVoiceMessageSpendLimitOverride",
             "DescribeAccountAttributes",
             "DescribeAccountLimits",
             "DescribeConfigurationSets",
             "DescribeKeywords",
             "DescribeOptOutLists",
             "DescribeOptedOutNumbers",
             "DescribePhoneNumbers",
             "DescribePools",
+            "DescribeProtectConfigurations",
             "DescribeRegistrationAttachments",
             "DescribeRegistrationFieldDefinitions",
             "DescribeRegistrationFieldValues",
             "DescribeRegistrationSectionDefinitions",
             "DescribeRegistrationTypeDefinitions",
             "DescribeRegistrationVersions",
             "DescribeRegistrations",
             "DescribeSenderIds",
             "DescribeSpendLimits",
             "DescribeVerifiedDestinationNumbers",
             "DisassociateOriginationIdentity",
+            "DisassociateProtectConfiguration",
             "DiscardRegistrationVersion",
             "GetConfigurationSetEventDestinations",
+            "GetProtectConfigurationCountryRuleSet",
             "ListConfigurationSets",
             "ListPoolOriginationIdentities",
             "ListRegistrationAssociations",
             "ListTagsForResource",
             "PutKeyword",
             "PutOptedOutNumber",
             "PutRegistrationFieldValue",
             "ReleasePhoneNumber",
             "ReleaseSenderId",
             "RequestPhoneNumber",
             "RequestSenderId",
             "SendDestinationNumberVerificationCode",
+            "SendMediaMessage",
             "SendTextMessage",
             "SendVoiceMessage",
+            "SetAccountDefaultProtectConfiguration",
             "SetDefaultMessageType",
             "SetDefaultSenderId",
+            "SetMediaMessageSpendLimitOverride",
             "SetTextMessageSpendLimitOverride",
             "SetVoiceMessageSpendLimitOverride",
             "SubmitRegistrationVersion",
             "TagResource",
             "UntagResource",
             "UpdateConfigurationSetEventDestination",
             "UpdateEventDestination",
             "UpdatePhoneNumber",
             "UpdatePool",
+            "UpdateProtectConfiguration",
+            "UpdateProtectConfigurationCountryRuleSet",
             "UpdateSenderId",
             "VerifyDestinationNumber"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20240501/pyproject.toml` & `iam_actions-1.2.20240502/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240501"
+version = "1.2.20240502"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240501/setup.py` & `iam_actions-1.2.20240502/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240501',
+    'version': '1.2.20240502',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240501/PKG-INFO` & `iam_actions-1.2.20240502/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240501
+Version: 1.2.20240502
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

