# Comparing `tmp/ibm-eventnotifications-0.4.0.tar.gz` & `tmp/ibm-eventnotifications-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-eventnotifications-0.4.0.tar", last modified: Fri Mar  1 05:24:48 2024, max compression
+gzip compressed data, was "ibm-eventnotifications-0.5.0.tar", last modified: Fri May  3 07:39:11 2024, max compression
```

## Comparing `ibm-eventnotifications-0.4.0.tar` & `ibm-eventnotifications-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-01 05:24:48.176469 ibm-eventnotifications-0.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    30612 2024-03-01 05:24:48.176469 ibm-eventnotifications-0.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    29573 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-01 05:24:48.176469 ibm-eventnotifications-0.4.0/ibm_eventnotifications/
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   459168 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications/event_notifications_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      667 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-01 05:24:48.176469 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    30612 2024-03-01 05:24:48.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2024-03-01 05:24:48.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-01 05:24:48.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-03-01 05:24:48.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2024-03-01 05:24:48.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-01 05:23:15.000000 ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      149 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-03-01 05:24:48.176469 ibm-eventnotifications-0.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2680 2024-03-01 05:22:47.000000 ibm-eventnotifications-0.4.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37297 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36258 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/ibm_eventnotifications/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   534941 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/event_notifications_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      667 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)    37297 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      512 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-03 07:37:18.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      149 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2680 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/setup.py
```

### Comparing `ibm-eventnotifications-0.4.0/LICENSE` & `ibm-eventnotifications-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.4.0/PKG-INFO` & `ibm-eventnotifications-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-eventnotifications
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python server SDK for IBM Cloud Event Notifications service
 Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
 Author: IBM
 Author-email: Notifications-prod@ibm.com
 License: Apache 2.0
 Keywords: ibm_eventnotifications
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IBM Cloud Event Notifications Python Admin SDK 0.4.0
+# IBM Cloud Event Notifications Python Admin SDK 0.5.0
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -62,19 +62,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.4.0"
+pip install --upgrade "ibm_eventnotifications>=0.5.0"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.4.0"
+easy_install --upgrade "ibm_eventnotifications>=0.5.0"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
@@ -139,28 +139,42 @@
 - [Templates](#templates)
     - [Create Template](#create-template)
     - [List Templates](#list-templates)
     - [Get Template](#get-template)
     - [Update Template](#update-template)
     - [Delete Template](#delete-template)
 - [Push Destination APIs](#push-destination-apis)
-  - [Create Destination tag subscription](#create-destination-tag-subscription)
-  - [List Destination tag subscription](#list-destination-tag-subscription)
-  - [Delete Destination device tag subscription](#delete-destination-device-tag-subscription)
+    - [Create Destination tag subscription](#create-destination-tag-subscription)
+    - [List Destination tag subscription](#list-destination-tag-subscription)
+    - [Delete Destination device tag subscription](#delete-destination-device-tag-subscription)
 - [Subscriptions](#subscriptions)
     - [Create Subscription](#create-subscription)
     - [List Subscriptions](#list-subscriptions)
     - [Get Subscription](#get-subscription)
     - [Update Subscription](#update-subscription)
     - [Delete Subscription](#delete-subscription)
 - [Integration](#integration)
-  - [Create Integration](#create-integration)
-  - [List Integrations](#list-integrations)
-  - [Get Integrations](#get-integration)
-  - [Update Integration](#update-integration)  
+    - [Create Integration](#create-integration)
+    - [List Integrations](#list-integrations)
+    - [Get Integrations](#get-integration)
+    - [Update Integration](#update-integration)
+- [SMTP Configurations](#SMTPConfigurations)
+	- [Create SMTP Configuration](#create-smtp-configuration)
+	- [Create SMTP User](#create-smtp-user)
+	- [Get SMTP Configuration](#get-smtp-configuration)
+	- [Get SMTP User](#get-smtp-user)	
+	- [Get SMTP Allowed Ips](#get-smtp-allowed-ips)
+	- [List SMTP Configurations](#list-smtp-configurations)
+	- [List SMTP Users](#list-smtp-users)
+	- [Update SMTP Configuration](#update-smtp-configuration)
+	- [Update SMTP User](#update-smtp-user)
+	- [Update SMTP Allowed Ips](#update-smtp-allowed-ips)
+	- [Delete SMTP User](#delete-smtp-user)
+	- [Delete SMTP Configuration](#delete-smtp-user)
+	- [Verify SMTP](#verify-smtp)
 - [Send Notifications](#send-notifications)
 
 ## Source 
 
 ### Create Source
 
 ```py
@@ -444,28 +458,48 @@
 Template is a pre-defined layout, that may include content like images, text and dynamic content based on event. Rather than creating a new content from scratch each time, you can use a template as a base and configure them in subscription. 
 supports the following templates:
 
 - Custom Email notification
 - Custom Email invitation
 
 ### Create Template
+
+#### Custom Email Template
 ```py
 template_config_model = {
     'body': 'base 64 encoded html content',
     'subject': 'Hi this is invitation for invitation message',
 }
 
 create_template_response = event_notifications_service.create_template(
     instance_id=<instance-id>,
     name=<template-name>,
     type=<template-type>,
     params=template_config_model,
     description=<template-description>
 ).get_result()
 ```
+For custom email supported template type values: smtp_custom.invitation, smtp_custom.notification 
+
+#### Slack Template
+```py
+template_config_model = {
+    'body': 'base 64 encoded json body',
+}
+
+create_template_response = event_notifications_service.create_template(
+    instance_id=<instance-id>,
+    name=<template-name>,
+    type=<template-type>,
+    params=template_config_model,
+    description=<template-description>
+).get_result()
+```
+For slack template supported template type value: slack.notification
+
 ### List Templates
 ```py
 list_templates_response = event_notifications_service.list_templates(
     instance_id=<instance-id>,
     limit=<limit>,
     offset=<offset>,
     search=<search>
@@ -691,14 +725,203 @@
   id=<integration_id>,
   metadata=integration_metadata
 )
 
 integration_response = update_integration_response.get_result()
 ```
 
+## SMTPConfigurations
+
+### Create SMTP Configuration
+
+```py
+
+create_smtp_config_response = self.event_notifications_service.create_smtp_configuration(
+    instance_id=<instance_id>,
+    name=<smtp-config-name>,
+    domain=<smtp-domain-name>,
+    description=<smtp-description>
+)
+
+smtp_response = create_smtp_config_response.get_result()
+
+```
+
+### Create SMTP User
+
+```py
+
+create_smtp_user_response = self.event_notifications_service.create_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp-config-id>,
+    description=<smtp-description>
+)
+
+create_user_response = create_smtp_user_response.get_result()
+
+```
+
+### Get SMTP Configuration
+
+```py
+
+get_smtp_config_response = self.event_notifications_service.get_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+get_smtp_config_response = get_smtp_config_response.get_result()
+
+```
+
+### Get SMTP User
+
+```py
+
+get_smtp_user_response = self.event_notifications_service.get_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<smtp_user_id>
+)
+
+get_smtp_user_response = get_smtp_user_response.get_result()
+
+```
+
+### Get SMTP Allowed Ips
+
+```py
+
+get_smtp_allowed_ip_response = self.event_notifications_service.get_smtp_allowed_ips(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+get_smtp_allowed_ip_response = get_smtp_allowed_ip_response.get_result()
+
+```
+
+### List SMTP Configurations
+
+```py
+
+list_smtp_config_response = self.event_notifications_service.list_smtp_configurations(
+    instance_id=<instance-id>,
+    limit=<limit>,
+    offset=<offset>,
+    search=<search>,
+)
+
+list_smtp_config_response = list_smtp_config_response.get_result()
+
+```
+
+### List SMTP Users
+
+```py
+
+list_smtp_user_response = self.event_notifications_service.list_smtp_users(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    limit=<limit>,
+    offset=<offset>,
+    search=<search>,
+)
+
+list_smtp_user_response = list_smtp_user_response.get_result()
+
+```
+
+### Update SMTP Configuration
+
+```py
+
+update_smtp_config_response = self.event_notifications_service.update_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    name=<smtp-name>,
+    description=<smtp-description>,
+)
+
+update_smtp_config_response = update_smtp_config_response.get_result()
+
+```
+
+### Update SMTP User
+
+```py
+
+update_smtp_user_response = self.event_notifications_service.update_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<smtp_user_id>,
+    description=<smtp-description>,
+)
+
+update_smtp_user_response = update_smtp_user_response.get_result()
+
+```
+
+### Update SMTP Allowed IPs
+
+```py
+
+subnets = ['<subnet-ips>']
+update_smtp_allowed_ip_response = self.event_notifications_service.update_smtp_allowed_ips(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    subnets=subnets
+)
+
+allowed_ip_response = update_smtp_allowed_ip_response.get_result()
+
+```
+
+### Delete SMTP User
+
+```py
+
+delete_smtp_user_response = self.event_notifications_service.delete_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<user-id>
+)
+
+print(json.dumps(delete_smtp_user_response, indent=2))
+
+```
+
+### Delete SMTP Configuration
+
+```py
+
+delete_smtp_config_response = self.event_notifications_service.delete_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+print(json.dumps(delete_smtp_config_response, indent=2))
+
+```
+
+### Verify SMTP
+
+```py
+
+update_verify_smtp_response = self.event_notifications_service.update_verify_smtp(
+    instance_id=<instance-id>,
+    type=<verification-type>,
+    id=<smtp_config_id>
+)
+
+verify_response = update_verify_smtp_response.get_result()
+
+```
+supported verification types are dkim,spf and en_authorization.
+
 ### Send Notifications
 
 
 ```py
 notification_devices_model = {
   'fcm_devices': ['<fcm-device-ids>'],
   'apns_devices': ['<apns-device-ids>'],
@@ -744,28 +967,30 @@
 type_value = "<notification-type>"
 notifications_source = "<notification-source>"
 htmlbody = '"Hi  ,<br/>Certificate expiring in 90 days.<br/><br/>Please login to ' \
            '<a href="https: //cloud.ibm.com/security-compliance/dashboard">' \
            'Security and Complaince dashboard</a> to find more information<br/>"'
 mailto = '[\"abc@ibm.com\", \"def@us.ibm.com\"]'
 smsto = '[\"+911234567890\", \"+911224567890\"]'
+templates = '["149b0e11-8a7c-4fda-a847-5d79e01b71dc"]'
 
 notification_create_model = {
     'ibmenseverity': notification_severity,
     'ibmenfcmbody': json.dumps(notification_fcm_body_model),
     'ibmenpushto': json.dumps(notification_devices_model),
     'ibmenapnsbody': json.dumps(notification_apns_body_model),
     'ibmensourceid': source_id,
     'ibmendefaultshort': 'short info',
     'ibmendefaultlong': 'long info',
     'ibmensafaribody': json.dumps(notificationSafariBodymodel),
     'ibmenhtmlbody': htmlbody,
     'ibmensubject': 'Findings on IBM Cloud Security Advisor',
     'ibmenmailto': mailto,
     'ibmensmsto': smsto,
+    "ibmentemplates": templates,
     'id': notification_id,
     'source': notifications_source,
     'type': type_value,
     'specversion': '1.0',
     'time': '2019-01-01T12:00:00.000Z',
 }
 
@@ -814,30 +1039,58 @@
   - **ibmenfirefoxheaders** (_string_) - Headers for the Firefox notifications. Refer [this official documentation](https://developer.mozilla.org/en-US/docs/Web/API/Notification/Notification) for more.
   - **ibmendefaultshort*** (_string_) - Default short text for the message.
   - **ibmendefaultlong*** (_string_) - Default long text for the message.
   - **specversion*** (_string_) - Spec version of the Event Notifications. Default value is `1.0`. 
   - **ibmenhtmlbody*** (_string_) - The html body of notification for email.
   - **ibmenmailto*** (_Array of string_) - Array of email ids to which the notification to be sent.
   - **ibmensmsto*** (_Array of string_) - Array of SMS numbers to which the notification to be sent.
+  - **ibmentemplates*** (_Array of string_) - Array of template IDs that needs to be applied while sending notificatin for custom domain email and slack destination.
 
 Note: variable with * represents the mandatory attribute.
 </details>
 
 ## Set Environment
 
 Find `event_notifications_v1.env.hide` in the repo and rename it to `event_notifications_v1.env`. After that add the values for,
 
 - `EVENT_NOTIFICATIONS_URL` - Add the Event Notifications service instance Url.
 - `EVENT_NOTIFICATIONS_APIKEY` - Add the Event Notifications service instance apikey.
 - `EVENT_NOTIFICATIONS_GUID` - Add the Event Notifications service instance GUID.
 
-Optional 
+**Optional**
 - `EVENT_NOTIFICATIONS_AUTH_URL` - Add the IAM url if you are using IBM test cloud.
 - `EVENT_NOTIFICATIONS_FCM_KEY` - Add firebase server key for Android FCM destination.
 - `EVENT_NOTIFICATIONS_FCM_ID` - Add firebase sender Id for Android FCM destination.
+- `EVENT_NOTIFICATIONS_FCM_PROJECT_ID` - fcm project id
+- `EVENT_NOTIFICATIONS_FCM_CLIENT_EMAIL` - fcm client email
+- `EVENT_NOTIFICATIONS_FCM_PRIVATE_KEY` - fcm private key
+- `EVENT_NOTIFICATIONS_SAFARI_CERTIFICATE` - safari certificate path
+
+- `EVENT_NOTIFICATIONS_SNOW_CLIENT_ID` - service now client id
+- `EVENT_NOTIFICATIONS_SNOW_CLIENT_SECRET` - service now client secret
+- `EVENT_NOTIFICATIONS_SNOW_USER_NAME` - service now user name
+- `EVENT_NOTIFICATIONS_SNOW_PASSWORD` - service now password
+- `EVENT_NOTIFICATIONS_SNOW_INSTANCE_NAME` - service now instance name
+
+- `EVENT_NOTIFICATIONS_COS_BUCKET_NAME` - cloud object storage bucket name
+- `EVENT_NOTIFICATIONS_COS_INSTANCE` - cloud object storage instance id
+- `EVENT_NOTIFICATIONS_COS_INSTANCE_CRN` - cloud object storage instance crn
+- `EVENT_NOTIFICATIONS_COS_ENDPOINT` - cloud object storage end point
+
+- `EVENT_NOTIFICATIONS_CODE_ENGINE_URL` - code engine app url
+- `EVENT_NOTIFICATIONS_CODE_ENGINE_PROJECT_CRN` - code engine project crn
+- `EVENT_NOTIFICATIONS_HUAWEI_CLIENT_SECRET` - huawei client secret
+- `EVENT_NOTIFICATIONS_HUAWEI_CLIENT_ID` - huawei client id
+
+- `EVENT_NOTIFICATIONS_SLACK_URL` - slack webhook url
+- `EVENT_NOTIFICATIONS_MS_TEAMS_URL` - msteams webhook url
+- `EVENT_NOTIFICATIONS_PD_ROUTING_KEY` - pagerduty routing key
+- `EVENT_NOTIFICATIONS_PD_API_KEY` - pagerduty api key
+- `EVENT_NOTIFICATIONS_TEMPLATE_BODY` - base 64 encoded html content
+- `EVENT_NOTIFICATIONS_SLACK_TEMPLATE_BODY` - base 64 encoded json body
 
 ## Questions
 
 If you are having difficulties using this SDK or have a question about the IBM Cloud services,
 please ask a question
 [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).
```

### Comparing `ibm-eventnotifications-0.4.0/README.md` & `ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,33 @@
-# IBM Cloud Event Notifications Python Admin SDK 0.4.0
+Metadata-Version: 2.1
+Name: ibm-eventnotifications
+Version: 0.5.0
+Summary: Python server SDK for IBM Cloud Event Notifications service
+Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
+Author: IBM
+Author-email: Notifications-prod@ibm.com
+License: Apache 2.0
+Keywords: ibm_eventnotifications
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IBM Cloud Event Notifications Python Admin SDK 0.5.0
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -37,19 +62,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.4.0"
+pip install --upgrade "ibm_eventnotifications>=0.5.0"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.4.0"
+easy_install --upgrade "ibm_eventnotifications>=0.5.0"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
@@ -114,28 +139,42 @@
 - [Templates](#templates)
     - [Create Template](#create-template)
     - [List Templates](#list-templates)
     - [Get Template](#get-template)
     - [Update Template](#update-template)
     - [Delete Template](#delete-template)
 - [Push Destination APIs](#push-destination-apis)
-  - [Create Destination tag subscription](#create-destination-tag-subscription)
-  - [List Destination tag subscription](#list-destination-tag-subscription)
-  - [Delete Destination device tag subscription](#delete-destination-device-tag-subscription)
+    - [Create Destination tag subscription](#create-destination-tag-subscription)
+    - [List Destination tag subscription](#list-destination-tag-subscription)
+    - [Delete Destination device tag subscription](#delete-destination-device-tag-subscription)
 - [Subscriptions](#subscriptions)
     - [Create Subscription](#create-subscription)
     - [List Subscriptions](#list-subscriptions)
     - [Get Subscription](#get-subscription)
     - [Update Subscription](#update-subscription)
     - [Delete Subscription](#delete-subscription)
 - [Integration](#integration)
-  - [Create Integration](#create-integration)
-  - [List Integrations](#list-integrations)
-  - [Get Integrations](#get-integration)
-  - [Update Integration](#update-integration)  
+    - [Create Integration](#create-integration)
+    - [List Integrations](#list-integrations)
+    - [Get Integrations](#get-integration)
+    - [Update Integration](#update-integration)
+- [SMTP Configurations](#SMTPConfigurations)
+	- [Create SMTP Configuration](#create-smtp-configuration)
+	- [Create SMTP User](#create-smtp-user)
+	- [Get SMTP Configuration](#get-smtp-configuration)
+	- [Get SMTP User](#get-smtp-user)	
+	- [Get SMTP Allowed Ips](#get-smtp-allowed-ips)
+	- [List SMTP Configurations](#list-smtp-configurations)
+	- [List SMTP Users](#list-smtp-users)
+	- [Update SMTP Configuration](#update-smtp-configuration)
+	- [Update SMTP User](#update-smtp-user)
+	- [Update SMTP Allowed Ips](#update-smtp-allowed-ips)
+	- [Delete SMTP User](#delete-smtp-user)
+	- [Delete SMTP Configuration](#delete-smtp-user)
+	- [Verify SMTP](#verify-smtp)
 - [Send Notifications](#send-notifications)
 
 ## Source 
 
 ### Create Source
 
 ```py
@@ -419,28 +458,48 @@
 Template is a pre-defined layout, that may include content like images, text and dynamic content based on event. Rather than creating a new content from scratch each time, you can use a template as a base and configure them in subscription. 
 supports the following templates:
 
 - Custom Email notification
 - Custom Email invitation
 
 ### Create Template
+
+#### Custom Email Template
 ```py
 template_config_model = {
     'body': 'base 64 encoded html content',
     'subject': 'Hi this is invitation for invitation message',
 }
 
 create_template_response = event_notifications_service.create_template(
     instance_id=<instance-id>,
     name=<template-name>,
     type=<template-type>,
     params=template_config_model,
     description=<template-description>
 ).get_result()
 ```
+For custom email supported template type values: smtp_custom.invitation, smtp_custom.notification 
+
+#### Slack Template
+```py
+template_config_model = {
+    'body': 'base 64 encoded json body',
+}
+
+create_template_response = event_notifications_service.create_template(
+    instance_id=<instance-id>,
+    name=<template-name>,
+    type=<template-type>,
+    params=template_config_model,
+    description=<template-description>
+).get_result()
+```
+For slack template supported template type value: slack.notification
+
 ### List Templates
 ```py
 list_templates_response = event_notifications_service.list_templates(
     instance_id=<instance-id>,
     limit=<limit>,
     offset=<offset>,
     search=<search>
@@ -666,14 +725,203 @@
   id=<integration_id>,
   metadata=integration_metadata
 )
 
 integration_response = update_integration_response.get_result()
 ```
 
+## SMTPConfigurations
+
+### Create SMTP Configuration
+
+```py
+
+create_smtp_config_response = self.event_notifications_service.create_smtp_configuration(
+    instance_id=<instance_id>,
+    name=<smtp-config-name>,
+    domain=<smtp-domain-name>,
+    description=<smtp-description>
+)
+
+smtp_response = create_smtp_config_response.get_result()
+
+```
+
+### Create SMTP User
+
+```py
+
+create_smtp_user_response = self.event_notifications_service.create_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp-config-id>,
+    description=<smtp-description>
+)
+
+create_user_response = create_smtp_user_response.get_result()
+
+```
+
+### Get SMTP Configuration
+
+```py
+
+get_smtp_config_response = self.event_notifications_service.get_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+get_smtp_config_response = get_smtp_config_response.get_result()
+
+```
+
+### Get SMTP User
+
+```py
+
+get_smtp_user_response = self.event_notifications_service.get_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<smtp_user_id>
+)
+
+get_smtp_user_response = get_smtp_user_response.get_result()
+
+```
+
+### Get SMTP Allowed Ips
+
+```py
+
+get_smtp_allowed_ip_response = self.event_notifications_service.get_smtp_allowed_ips(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+get_smtp_allowed_ip_response = get_smtp_allowed_ip_response.get_result()
+
+```
+
+### List SMTP Configurations
+
+```py
+
+list_smtp_config_response = self.event_notifications_service.list_smtp_configurations(
+    instance_id=<instance-id>,
+    limit=<limit>,
+    offset=<offset>,
+    search=<search>,
+)
+
+list_smtp_config_response = list_smtp_config_response.get_result()
+
+```
+
+### List SMTP Users
+
+```py
+
+list_smtp_user_response = self.event_notifications_service.list_smtp_users(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    limit=<limit>,
+    offset=<offset>,
+    search=<search>,
+)
+
+list_smtp_user_response = list_smtp_user_response.get_result()
+
+```
+
+### Update SMTP Configuration
+
+```py
+
+update_smtp_config_response = self.event_notifications_service.update_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    name=<smtp-name>,
+    description=<smtp-description>,
+)
+
+update_smtp_config_response = update_smtp_config_response.get_result()
+
+```
+
+### Update SMTP User
+
+```py
+
+update_smtp_user_response = self.event_notifications_service.update_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<smtp_user_id>,
+    description=<smtp-description>,
+)
+
+update_smtp_user_response = update_smtp_user_response.get_result()
+
+```
+
+### Update SMTP Allowed IPs
+
+```py
+
+subnets = ['<subnet-ips>']
+update_smtp_allowed_ip_response = self.event_notifications_service.update_smtp_allowed_ips(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    subnets=subnets
+)
+
+allowed_ip_response = update_smtp_allowed_ip_response.get_result()
+
+```
+
+### Delete SMTP User
+
+```py
+
+delete_smtp_user_response = self.event_notifications_service.delete_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<user-id>
+)
+
+print(json.dumps(delete_smtp_user_response, indent=2))
+
+```
+
+### Delete SMTP Configuration
+
+```py
+
+delete_smtp_config_response = self.event_notifications_service.delete_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+print(json.dumps(delete_smtp_config_response, indent=2))
+
+```
+
+### Verify SMTP
+
+```py
+
+update_verify_smtp_response = self.event_notifications_service.update_verify_smtp(
+    instance_id=<instance-id>,
+    type=<verification-type>,
+    id=<smtp_config_id>
+)
+
+verify_response = update_verify_smtp_response.get_result()
+
+```
+supported verification types are dkim,spf and en_authorization.
+
 ### Send Notifications
 
 
 ```py
 notification_devices_model = {
   'fcm_devices': ['<fcm-device-ids>'],
   'apns_devices': ['<apns-device-ids>'],
@@ -719,28 +967,30 @@
 type_value = "<notification-type>"
 notifications_source = "<notification-source>"
 htmlbody = '"Hi  ,<br/>Certificate expiring in 90 days.<br/><br/>Please login to ' \
            '<a href="https: //cloud.ibm.com/security-compliance/dashboard">' \
            'Security and Complaince dashboard</a> to find more information<br/>"'
 mailto = '[\"abc@ibm.com\", \"def@us.ibm.com\"]'
 smsto = '[\"+911234567890\", \"+911224567890\"]'
+templates = '["149b0e11-8a7c-4fda-a847-5d79e01b71dc"]'
 
 notification_create_model = {
     'ibmenseverity': notification_severity,
     'ibmenfcmbody': json.dumps(notification_fcm_body_model),
     'ibmenpushto': json.dumps(notification_devices_model),
     'ibmenapnsbody': json.dumps(notification_apns_body_model),
     'ibmensourceid': source_id,
     'ibmendefaultshort': 'short info',
     'ibmendefaultlong': 'long info',
     'ibmensafaribody': json.dumps(notificationSafariBodymodel),
     'ibmenhtmlbody': htmlbody,
     'ibmensubject': 'Findings on IBM Cloud Security Advisor',
     'ibmenmailto': mailto,
     'ibmensmsto': smsto,
+    "ibmentemplates": templates,
     'id': notification_id,
     'source': notifications_source,
     'type': type_value,
     'specversion': '1.0',
     'time': '2019-01-01T12:00:00.000Z',
 }
 
@@ -789,30 +1039,58 @@
   - **ibmenfirefoxheaders** (_string_) - Headers for the Firefox notifications. Refer [this official documentation](https://developer.mozilla.org/en-US/docs/Web/API/Notification/Notification) for more.
   - **ibmendefaultshort*** (_string_) - Default short text for the message.
   - **ibmendefaultlong*** (_string_) - Default long text for the message.
   - **specversion*** (_string_) - Spec version of the Event Notifications. Default value is `1.0`. 
   - **ibmenhtmlbody*** (_string_) - The html body of notification for email.
   - **ibmenmailto*** (_Array of string_) - Array of email ids to which the notification to be sent.
   - **ibmensmsto*** (_Array of string_) - Array of SMS numbers to which the notification to be sent.
+  - **ibmentemplates*** (_Array of string_) - Array of template IDs that needs to be applied while sending notificatin for custom domain email and slack destination.
 
 Note: variable with * represents the mandatory attribute.
 </details>
 
 ## Set Environment
 
 Find `event_notifications_v1.env.hide` in the repo and rename it to `event_notifications_v1.env`. After that add the values for,
 
 - `EVENT_NOTIFICATIONS_URL` - Add the Event Notifications service instance Url.
 - `EVENT_NOTIFICATIONS_APIKEY` - Add the Event Notifications service instance apikey.
 - `EVENT_NOTIFICATIONS_GUID` - Add the Event Notifications service instance GUID.
 
-Optional 
+**Optional**
 - `EVENT_NOTIFICATIONS_AUTH_URL` - Add the IAM url if you are using IBM test cloud.
 - `EVENT_NOTIFICATIONS_FCM_KEY` - Add firebase server key for Android FCM destination.
 - `EVENT_NOTIFICATIONS_FCM_ID` - Add firebase sender Id for Android FCM destination.
+- `EVENT_NOTIFICATIONS_FCM_PROJECT_ID` - fcm project id
+- `EVENT_NOTIFICATIONS_FCM_CLIENT_EMAIL` - fcm client email
+- `EVENT_NOTIFICATIONS_FCM_PRIVATE_KEY` - fcm private key
+- `EVENT_NOTIFICATIONS_SAFARI_CERTIFICATE` - safari certificate path
+
+- `EVENT_NOTIFICATIONS_SNOW_CLIENT_ID` - service now client id
+- `EVENT_NOTIFICATIONS_SNOW_CLIENT_SECRET` - service now client secret
+- `EVENT_NOTIFICATIONS_SNOW_USER_NAME` - service now user name
+- `EVENT_NOTIFICATIONS_SNOW_PASSWORD` - service now password
+- `EVENT_NOTIFICATIONS_SNOW_INSTANCE_NAME` - service now instance name
+
+- `EVENT_NOTIFICATIONS_COS_BUCKET_NAME` - cloud object storage bucket name
+- `EVENT_NOTIFICATIONS_COS_INSTANCE` - cloud object storage instance id
+- `EVENT_NOTIFICATIONS_COS_INSTANCE_CRN` - cloud object storage instance crn
+- `EVENT_NOTIFICATIONS_COS_ENDPOINT` - cloud object storage end point
+
+- `EVENT_NOTIFICATIONS_CODE_ENGINE_URL` - code engine app url
+- `EVENT_NOTIFICATIONS_CODE_ENGINE_PROJECT_CRN` - code engine project crn
+- `EVENT_NOTIFICATIONS_HUAWEI_CLIENT_SECRET` - huawei client secret
+- `EVENT_NOTIFICATIONS_HUAWEI_CLIENT_ID` - huawei client id
+
+- `EVENT_NOTIFICATIONS_SLACK_URL` - slack webhook url
+- `EVENT_NOTIFICATIONS_MS_TEAMS_URL` - msteams webhook url
+- `EVENT_NOTIFICATIONS_PD_ROUTING_KEY` - pagerduty routing key
+- `EVENT_NOTIFICATIONS_PD_API_KEY` - pagerduty api key
+- `EVENT_NOTIFICATIONS_TEMPLATE_BODY` - base 64 encoded html content
+- `EVENT_NOTIFICATIONS_SLACK_TEMPLATE_BODY` - base 64 encoded json body
 
 ## Questions
 
 If you are having difficulties using this SDK or have a question about the IBM Cloud services,
 please ask a question
 [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).
 
@@ -827,7 +1105,9 @@
 ## Contributing
 See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## License
 
 This SDK is released under the Apache 2.0 license.
 The license's full text can be found in [LICENSE](LICENSE).
+
+
```

### Comparing `ibm-eventnotifications-0.4.0/ibm_eventnotifications/__init__.py` & `ibm-eventnotifications-0.5.0/ibm_eventnotifications/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.4.0/ibm_eventnotifications/common.py` & `ibm-eventnotifications-0.5.0/ibm_eventnotifications/common.py`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.4.0/ibm_eventnotifications/event_notifications_v1.py` & `ibm-eventnotifications-0.5.0/ibm_eventnotifications/event_notifications_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -732,29 +732,29 @@
     #########################
 
     def create_template(
         self,
         instance_id: str,
         name: str,
         type: str,
-        params: 'TemplateConfig',
+        params: 'TemplateConfigOneOf',
         *,
         description: str = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Create a new Template.
 
         Create a new Template.
 
         :param str instance_id: Unique identifier for IBM Cloud Event Notifications
                instance.
         :param str name: The Message Template.
         :param str type: The type of template.
-        :param TemplateConfig params: Payload describing a template configuration.
+        :param TemplateConfigOneOf params:
         :param str description: (optional) The Template description.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `TemplateResponse` object
         """
 
         if not instance_id:
@@ -915,30 +915,29 @@
         self,
         instance_id: str,
         id: str,
         *,
         name: str = None,
         description: str = None,
         type: str = None,
-        params: 'TemplateConfig' = None,
+        params: 'TemplateConfigOneOf' = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Update details of a Template.
 
         Update details of a Template.
 
         :param str instance_id: Unique identifier for IBM Cloud Event Notifications
                instance.
         :param str id: Unique identifier for Template.
         :param str name: (optional) Template name.
         :param str description: (optional) Template description.
         :param str type: (optional) The type of template.
-        :param TemplateConfig params: (optional) Payload describing a template
-               configuration.
+        :param TemplateConfigOneOf params: (optional)
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Template` object
         """
 
         if not instance_id:
             raise ValueError('instance_id must be provided')
@@ -2354,14 +2353,763 @@
             headers=headers,
             data=data,
         )
 
         response = self.send(request, **kwargs)
         return response
 
+    #########################
+    # SMTP Configurations
+    #########################
+
+    def create_smtp_configuration(
+        self,
+        instance_id: str,
+        name: str,
+        domain: str,
+        *,
+        description: str = None,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Create a new SMTP Configuration.
+
+        Create a new SMTP Configuration.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str name: The name of SMTP configuration.
+        :param str domain: Domain Name.
+        :param str description: (optional) The description of SMTP configuration.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPCreateResponse` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if name is None:
+            raise ValueError('name must be provided')
+        if domain is None:
+            raise ValueError('domain must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='create_smtp_configuration',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'name': name,
+            'domain': domain,
+            'description': description,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id']
+        path_param_values = self.encode_path_vars(instance_id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def list_smtp_configurations(
+        self,
+        instance_id: str,
+        *,
+        limit: int = None,
+        offset: int = None,
+        search: str = None,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        List all SMTP Configurations.
+
+        List all SMTP Configurations.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param int limit: (optional) Page limit for paginated results.
+        :param int offset: (optional) offset for paginated results.
+        :param str search: (optional) Search string for filtering results.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPConfigurationsList` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='list_smtp_configurations',
+        )
+        headers.update(sdk_headers)
+
+        params = {
+            'limit': limit,
+            'offset': offset,
+            'search': search,
+        }
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id']
+        path_param_values = self.encode_path_vars(instance_id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def create_smtp_user(
+        self,
+        instance_id: str,
+        id: str,
+        *,
+        description: str = None,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Create a new SMTP User.
+
+        Create a new SMTP User.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param str description: (optional) The description of SMTP configuration.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPUserResponse` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='create_smtp_user',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'description': description,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/users'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def list_smtp_users(
+        self,
+        instance_id: str,
+        id: str,
+        *,
+        limit: int = None,
+        offset: int = None,
+        search: str = None,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        List all SMTP users.
+
+        List all SMTP users.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param int limit: (optional) Page limit for paginated results.
+        :param int offset: (optional) offset for paginated results.
+        :param str search: (optional) Search string for filtering results.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPUsersList` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='list_smtp_users',
+        )
+        headers.update(sdk_headers)
+
+        params = {
+            'limit': limit,
+            'offset': offset,
+            'search': search,
+        }
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/users'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+            params=params,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def get_smtp_configuration(
+        self,
+        instance_id: str,
+        id: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Get details of a SMTP Configuration.
+
+        Get details of a SMTP Configuration.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPConfiguration` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_smtp_configuration',
+        )
+        headers.update(sdk_headers)
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def update_smtp_configuration(
+        self,
+        instance_id: str,
+        id: str,
+        *,
+        name: str = None,
+        description: str = None,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Update details of SMTP.
+
+        Update details of SMTP.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param str name: (optional) SMTP name.
+        :param str description: (optional) SMTP description.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPConfiguration` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='update_smtp_configuration',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'name': name,
+            'description': description,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='PATCH',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def delete_smtp_configuration(
+        self,
+        instance_id: str,
+        id: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Delete a SMTP Configuration.
+
+        Delete a SMTP Configuration.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_smtp_configuration',
+        )
+        headers.update(sdk_headers)
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def get_smtp_user(
+        self,
+        instance_id: str,
+        id: str,
+        user_id: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Get details of a SMTP User.
+
+        Get details of a SMTP User.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param str user_id: UserID.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPUser` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if not user_id:
+            raise ValueError('user_id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_smtp_user',
+        )
+        headers.update(sdk_headers)
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id', 'user_id']
+        path_param_values = self.encode_path_vars(instance_id, id, user_id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/users/{user_id}'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def update_smtp_user(
+        self,
+        instance_id: str,
+        id: str,
+        user_id: str,
+        *,
+        description: str = None,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Update details of SMTP User.
+
+        Update details of SMTP User.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param str user_id: UserID.
+        :param str description: (optional) SMTP user description.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPUser` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if not user_id:
+            raise ValueError('user_id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='update_smtp_user',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'description': description,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id', 'user_id']
+        path_param_values = self.encode_path_vars(instance_id, id, user_id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/users/{user_id}'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='PATCH',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def delete_smtp_user(
+        self,
+        instance_id: str,
+        id: str,
+        user_id: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Delete a SMTP user.
+
+        Delete a SMTP user.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param str user_id: UserID.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if not user_id:
+            raise ValueError('user_id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='delete_smtp_user',
+        )
+        headers.update(sdk_headers)
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+
+        path_param_keys = ['instance_id', 'id', 'user_id']
+        path_param_values = self.encode_path_vars(instance_id, id, user_id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/users/{user_id}'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='DELETE',
+            url=url,
+            headers=headers,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def get_smtp_allowed_ips(
+        self,
+        instance_id: str,
+        id: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Get details of a SMTP allowed IPs.
+
+        Get details of a SMTP allowed IPs.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPAllowedIPs` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_smtp_allowed_ips',
+        )
+        headers.update(sdk_headers)
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/allowed_ips'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def update_smtp_allowed_ips(
+        self,
+        instance_id: str,
+        id: str,
+        subnets: List[str],
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Update details of SMTP allowed IP.
+
+        Update details of SMTP.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param List[str] subnets: The SMTP allowed Ips.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPAllowedIPs` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if subnets is None:
+            raise ValueError('subnets must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='update_smtp_allowed_ips',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'subnets': subnets,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/allowed_ips'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='PATCH',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def update_verify_smtp(
+        self,
+        instance_id: str,
+        id: str,
+        type: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Verify SPF and DKIM records of SMTP.
+
+        Verify SPF and DKIM records of SMTP.
+
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param str type: SMTP Verification type.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `SMTPVerificationUpdateResponse` object
+        """
+
+        if not instance_id:
+            raise ValueError('instance_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if not type:
+            raise ValueError('type must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='update_verify_smtp',
+        )
+        headers.update(sdk_headers)
+
+        params = {
+            'type': type,
+        }
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['instance_id', 'id']
+        path_param_values = self.encode_path_vars(instance_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/instances/{instance_id}/smtp/config/{id}/verify'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='PATCH',
+            url=url,
+            headers=headers,
+            params=params,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
 
 class CreateDestinationEnums:
     """
     Enums for create_destination parameters.
     """
 
     class Type(str, Enum):
@@ -3256,14 +4004,72 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'DestinationTagsSubscriptionResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ENAuthAttributes:
+    """
+    The en_authorization attributes.
+
+    :attr str verification: (optional) en_authorization verification.
+    """
+
+    def __init__(
+        self,
+        *,
+        verification: str = None,
+    ) -> None:
+        """
+        Initialize a ENAuthAttributes object.
+
+        :param str verification: (optional) en_authorization verification.
+        """
+        self.verification = verification
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ENAuthAttributes':
+        """Initialize a ENAuthAttributes object from a json dictionary."""
+        args = {}
+        if 'verification' in _dict:
+            args['verification'] = _dict.get('verification')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ENAuthAttributes object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'verification') and self.verification is not None:
+            _dict['verification'] = self.verification
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ENAuthAttributes object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ENAuthAttributes') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ENAuthAttributes') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class EmailAttributesResponseInvitedItems:
     """
     EmailAttributesResponseInvitedItems.
 
     :attr str email: (optional) email address.
     :attr datetime updated_at: (optional) last updated time.
     :attr datetime expires_at: (optional) time of expiration.
@@ -4076,16 +4882,17 @@
     :attr str source: The source of notifications.
     :attr str type: The notifications type.
     :attr str ibmenseverity: (optional) The severity of the notification.
     :attr str ibmensourceid: The source id of the notification.
     :attr str ibmendefaultshort: Default short text for the message.
     :attr str ibmendefaultlong: Default long text for the message.
     :attr str ibmensubject: (optional) The subject of the notification.
-    :attr str ibmensmsto: (optional) The SMS number string.
+    :attr str ibmentemplates: (optional) The template id Array of string.
     :attr str ibmenmailto: (optional) The email id string.
+    :attr str ibmensmsto: (optional) The SMS number string.
     :attr str ibmenhtmlbody: (optional) The html body of notification.
     :attr str subject: (optional) The subject of the notification.
     :attr dict data: (optional) The payload for webhook notification.
     :attr str datacontenttype: (optional) The notification content type.
     :attr str ibmenpushto: (optional) If platforms or tags or user_ids is used then
           do not use fcm_devices / apns_devices / chrome_devices / firefox_devices /
           safari_devices with it. Value should be stringified.
@@ -4118,16 +4925,17 @@
             'source',
             'type',
             'ibmenseverity',
             'ibmensourceid',
             'ibmendefaultshort',
             'ibmendefaultlong',
             'ibmensubject',
-            'ibmensmsto',
+            'ibmentemplates',
             'ibmenmailto',
+            'ibmensmsto',
             'ibmenhtmlbody',
             'subject',
             'data',
             'datacontenttype',
             'ibmenpushto',
             'ibmenfcmbody',
             'ibmenapnsbody',
@@ -4150,16 +4958,17 @@
         ibmensourceid: str,
         ibmendefaultshort: str,
         ibmendefaultlong: str,
         *,
         time: datetime = None,
         ibmenseverity: str = None,
         ibmensubject: str = None,
-        ibmensmsto: str = None,
+        ibmentemplates: str = None,
         ibmenmailto: str = None,
+        ibmensmsto: str = None,
         ibmenhtmlbody: str = None,
         subject: str = None,
         data: dict = None,
         datacontenttype: str = None,
         ibmenpushto: str = None,
         ibmenfcmbody: str = None,
         ibmenapnsbody: str = None,
@@ -4181,16 +4990,17 @@
         :param str type: The notifications type.
         :param str ibmensourceid: The source id of the notification.
         :param str ibmendefaultshort: Default short text for the message.
         :param str ibmendefaultlong: Default long text for the message.
         :param datetime time: (optional) The time notification was created.
         :param str ibmenseverity: (optional) The severity of the notification.
         :param str ibmensubject: (optional) The subject of the notification.
-        :param str ibmensmsto: (optional) The SMS number string.
+        :param str ibmentemplates: (optional) The template id Array of string.
         :param str ibmenmailto: (optional) The email id string.
+        :param str ibmensmsto: (optional) The SMS number string.
         :param str ibmenhtmlbody: (optional) The html body of notification.
         :param str subject: (optional) The subject of the notification.
         :param dict data: (optional) The payload for webhook notification.
         :param str datacontenttype: (optional) The notification content type.
         :param str ibmenpushto: (optional) If platforms or tags or user_ids is used
                then do not use fcm_devices / apns_devices / chrome_devices /
                firefox_devices / safari_devices with it. Value should be stringified.
@@ -4220,16 +5030,17 @@
         self.source = source
         self.type = type
         self.ibmenseverity = ibmenseverity
         self.ibmensourceid = ibmensourceid
         self.ibmendefaultshort = ibmendefaultshort
         self.ibmendefaultlong = ibmendefaultlong
         self.ibmensubject = ibmensubject
-        self.ibmensmsto = ibmensmsto
+        self.ibmentemplates = ibmentemplates
         self.ibmenmailto = ibmenmailto
+        self.ibmensmsto = ibmensmsto
         self.ibmenhtmlbody = ibmenhtmlbody
         self.subject = subject
         self.data = data
         self.datacontenttype = datacontenttype
         self.ibmenpushto = ibmenpushto
         self.ibmenfcmbody = ibmenfcmbody
         self.ibmenapnsbody = ibmenapnsbody
@@ -4277,18 +5088,20 @@
             raise ValueError('Required property \'ibmendefaultshort\' not present in NotificationCreate JSON')
         if 'ibmendefaultlong' in _dict:
             args['ibmendefaultlong'] = _dict.get('ibmendefaultlong')
         else:
             raise ValueError('Required property \'ibmendefaultlong\' not present in NotificationCreate JSON')
         if 'ibmensubject' in _dict:
             args['ibmensubject'] = _dict.get('ibmensubject')
-        if 'ibmensmsto' in _dict:
-            args['ibmensmsto'] = _dict.get('ibmensmsto')
+        if 'ibmentemplates' in _dict:
+            args['ibmentemplates'] = _dict.get('ibmentemplates')
         if 'ibmenmailto' in _dict:
             args['ibmenmailto'] = _dict.get('ibmenmailto')
+        if 'ibmensmsto' in _dict:
+            args['ibmensmsto'] = _dict.get('ibmensmsto')
         if 'ibmenhtmlbody' in _dict:
             args['ibmenhtmlbody'] = _dict.get('ibmenhtmlbody')
         if 'subject' in _dict:
             args['subject'] = _dict.get('subject')
         if 'data' in _dict:
             args['data'] = _dict.get('data')
         if 'datacontenttype' in _dict:
@@ -4340,18 +5153,20 @@
             _dict['ibmensourceid'] = self.ibmensourceid
         if hasattr(self, 'ibmendefaultshort') and self.ibmendefaultshort is not None:
             _dict['ibmendefaultshort'] = self.ibmendefaultshort
         if hasattr(self, 'ibmendefaultlong') and self.ibmendefaultlong is not None:
             _dict['ibmendefaultlong'] = self.ibmendefaultlong
         if hasattr(self, 'ibmensubject') and self.ibmensubject is not None:
             _dict['ibmensubject'] = self.ibmensubject
-        if hasattr(self, 'ibmensmsto') and self.ibmensmsto is not None:
-            _dict['ibmensmsto'] = self.ibmensmsto
+        if hasattr(self, 'ibmentemplates') and self.ibmentemplates is not None:
+            _dict['ibmentemplates'] = self.ibmentemplates
         if hasattr(self, 'ibmenmailto') and self.ibmenmailto is not None:
             _dict['ibmenmailto'] = self.ibmenmailto
+        if hasattr(self, 'ibmensmsto') and self.ibmensmsto is not None:
+            _dict['ibmensmsto'] = self.ibmensmsto
         if hasattr(self, 'ibmenhtmlbody') and self.ibmenhtmlbody is not None:
             _dict['ibmenhtmlbody'] = self.ibmenhtmlbody
         if hasattr(self, 'subject') and self.subject is not None:
             _dict['subject'] = self.subject
         if hasattr(self, 'data') and self.data is not None:
             _dict['data'] = self.data
         if hasattr(self, 'datacontenttype') and self.datacontenttype is not None:
@@ -4913,14 +5728,1020 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SMSInviteAttributesItems') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class SMTPAllowedIPs:
+    """
+    Payload describing a SMTP allowed Ips.
+
+    :attr List[str] subnets: The SMTP allowed Ips.
+    :attr datetime updated_at: Updated at.
+    """
+
+    def __init__(
+        self,
+        subnets: List[str],
+        updated_at: datetime,
+    ) -> None:
+        """
+        Initialize a SMTPAllowedIPs object.
+
+        :param List[str] subnets: The SMTP allowed Ips.
+        :param datetime updated_at: Updated at.
+        """
+        self.subnets = subnets
+        self.updated_at = updated_at
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPAllowedIPs':
+        """Initialize a SMTPAllowedIPs object from a json dictionary."""
+        args = {}
+        if 'subnets' in _dict:
+            args['subnets'] = _dict.get('subnets')
+        else:
+            raise ValueError('Required property \'subnets\' not present in SMTPAllowedIPs JSON')
+        if 'updated_at' in _dict:
+            args['updated_at'] = string_to_datetime(_dict.get('updated_at'))
+        else:
+            raise ValueError('Required property \'updated_at\' not present in SMTPAllowedIPs JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPAllowedIPs object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'subnets') and self.subnets is not None:
+            _dict['subnets'] = self.subnets
+        if hasattr(self, 'updated_at') and self.updated_at is not None:
+            _dict['updated_at'] = datetime_to_string(self.updated_at)
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPAllowedIPs object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPAllowedIPs') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPAllowedIPs') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPConfig:
+    """
+    Payload describing a SMTP configuration.
+
+    :attr DKIMAttributes dkim: (optional) The DKIM attributes.
+    :attr ENAuthAttributes en_authorization: (optional) The en_authorization
+          attributes.
+    :attr SPFAttributes spf: (optional) The SPF attributes.
+    """
+
+    def __init__(
+        self,
+        *,
+        dkim: 'DKIMAttributes' = None,
+        en_authorization: 'ENAuthAttributes' = None,
+        spf: 'SPFAttributes' = None,
+    ) -> None:
+        """
+        Initialize a SMTPConfig object.
+
+        :param DKIMAttributes dkim: (optional) The DKIM attributes.
+        :param ENAuthAttributes en_authorization: (optional) The en_authorization
+               attributes.
+        :param SPFAttributes spf: (optional) The SPF attributes.
+        """
+        self.dkim = dkim
+        self.en_authorization = en_authorization
+        self.spf = spf
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPConfig':
+        """Initialize a SMTPConfig object from a json dictionary."""
+        args = {}
+        if 'dkim' in _dict:
+            args['dkim'] = DKIMAttributes.from_dict(_dict.get('dkim'))
+        if 'en_authorization' in _dict:
+            args['en_authorization'] = ENAuthAttributes.from_dict(_dict.get('en_authorization'))
+        if 'spf' in _dict:
+            args['spf'] = SPFAttributes.from_dict(_dict.get('spf'))
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPConfig object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'dkim') and self.dkim is not None:
+            if isinstance(self.dkim, dict):
+                _dict['dkim'] = self.dkim
+            else:
+                _dict['dkim'] = self.dkim.to_dict()
+        if hasattr(self, 'en_authorization') and self.en_authorization is not None:
+            if isinstance(self.en_authorization, dict):
+                _dict['en_authorization'] = self.en_authorization
+            else:
+                _dict['en_authorization'] = self.en_authorization.to_dict()
+        if hasattr(self, 'spf') and self.spf is not None:
+            if isinstance(self.spf, dict):
+                _dict['spf'] = self.spf
+            else:
+                _dict['spf'] = self.spf.to_dict()
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPConfig object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPConfig') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPConfig') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPConfiguration:
+    """
+    Payload describing a SMTP List response.
+
+    :attr str id: SMTP ID.
+    :attr str name: SMTP name.
+    :attr str description: (optional) SMTP description.
+    :attr str domain: Domain Name.
+    :attr SMTPConfig config: Payload describing a SMTP configuration.
+    :attr datetime updated_at: Created time.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        name: str,
+        domain: str,
+        config: 'SMTPConfig',
+        updated_at: datetime,
+        *,
+        description: str = None,
+    ) -> None:
+        """
+        Initialize a SMTPConfiguration object.
+
+        :param str id: SMTP ID.
+        :param str name: SMTP name.
+        :param str domain: Domain Name.
+        :param SMTPConfig config: Payload describing a SMTP configuration.
+        :param datetime updated_at: Created time.
+        :param str description: (optional) SMTP description.
+        """
+        self.id = id
+        self.name = name
+        self.description = description
+        self.domain = domain
+        self.config = config
+        self.updated_at = updated_at
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPConfiguration':
+        """Initialize a SMTPConfiguration object from a json dictionary."""
+        args = {}
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        else:
+            raise ValueError('Required property \'id\' not present in SMTPConfiguration JSON')
+        if 'name' in _dict:
+            args['name'] = _dict.get('name')
+        else:
+            raise ValueError('Required property \'name\' not present in SMTPConfiguration JSON')
+        if 'description' in _dict:
+            args['description'] = _dict.get('description')
+        if 'domain' in _dict:
+            args['domain'] = _dict.get('domain')
+        else:
+            raise ValueError('Required property \'domain\' not present in SMTPConfiguration JSON')
+        if 'config' in _dict:
+            args['config'] = SMTPConfig.from_dict(_dict.get('config'))
+        else:
+            raise ValueError('Required property \'config\' not present in SMTPConfiguration JSON')
+        if 'updated_at' in _dict:
+            args['updated_at'] = string_to_datetime(_dict.get('updated_at'))
+        else:
+            raise ValueError('Required property \'updated_at\' not present in SMTPConfiguration JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPConfiguration object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'domain') and self.domain is not None:
+            _dict['domain'] = self.domain
+        if hasattr(self, 'config') and self.config is not None:
+            if isinstance(self.config, dict):
+                _dict['config'] = self.config
+            else:
+                _dict['config'] = self.config.to_dict()
+        if hasattr(self, 'updated_at') and self.updated_at is not None:
+            _dict['updated_at'] = datetime_to_string(self.updated_at)
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPConfiguration object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPConfiguration') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPConfiguration') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPConfigurationsList:
+    """
+    Payload describing a SMTP Configurations list.
+
+    :attr int total_count: Total number of SMTP configurations.
+    :attr int offset: Current offset.
+    :attr int limit: limit to show configurations.
+    :attr List[SMTPConfiguration] smtp_configurations: List of SMTP Configurations.
+    :attr PageHrefResponse first: (optional) Response having URL of the page.
+    :attr PageHrefResponse previous: (optional) Response having URL of the page.
+    :attr PageHrefResponse next: (optional) Response having URL of the page.
+    """
+
+    def __init__(
+        self,
+        total_count: int,
+        offset: int,
+        limit: int,
+        smtp_configurations: List['SMTPConfiguration'],
+        *,
+        first: 'PageHrefResponse' = None,
+        previous: 'PageHrefResponse' = None,
+        next: 'PageHrefResponse' = None,
+    ) -> None:
+        """
+        Initialize a SMTPConfigurationsList object.
+
+        :param int total_count: Total number of SMTP configurations.
+        :param int offset: Current offset.
+        :param int limit: limit to show configurations.
+        :param List[SMTPConfiguration] smtp_configurations: List of SMTP
+               Configurations.
+        :param PageHrefResponse first: (optional) Response having URL of the page.
+        :param PageHrefResponse previous: (optional) Response having URL of the
+               page.
+        :param PageHrefResponse next: (optional) Response having URL of the page.
+        """
+        self.total_count = total_count
+        self.offset = offset
+        self.limit = limit
+        self.smtp_configurations = smtp_configurations
+        self.first = first
+        self.previous = previous
+        self.next = next
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPConfigurationsList':
+        """Initialize a SMTPConfigurationsList object from a json dictionary."""
+        args = {}
+        if 'total_count' in _dict:
+            args['total_count'] = _dict.get('total_count')
+        else:
+            raise ValueError('Required property \'total_count\' not present in SMTPConfigurationsList JSON')
+        if 'offset' in _dict:
+            args['offset'] = _dict.get('offset')
+        else:
+            raise ValueError('Required property \'offset\' not present in SMTPConfigurationsList JSON')
+        if 'limit' in _dict:
+            args['limit'] = _dict.get('limit')
+        else:
+            raise ValueError('Required property \'limit\' not present in SMTPConfigurationsList JSON')
+        if 'smtp_configurations' in _dict:
+            args['smtp_configurations'] = [SMTPConfiguration.from_dict(v) for v in _dict.get('smtp_configurations')]
+        else:
+            raise ValueError('Required property \'smtp_configurations\' not present in SMTPConfigurationsList JSON')
+        if 'first' in _dict:
+            args['first'] = PageHrefResponse.from_dict(_dict.get('first'))
+        if 'previous' in _dict:
+            args['previous'] = PageHrefResponse.from_dict(_dict.get('previous'))
+        if 'next' in _dict:
+            args['next'] = PageHrefResponse.from_dict(_dict.get('next'))
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPConfigurationsList object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'total_count') and self.total_count is not None:
+            _dict['total_count'] = self.total_count
+        if hasattr(self, 'offset') and self.offset is not None:
+            _dict['offset'] = self.offset
+        if hasattr(self, 'limit') and self.limit is not None:
+            _dict['limit'] = self.limit
+        if hasattr(self, 'smtp_configurations') and self.smtp_configurations is not None:
+            smtp_configurations_list = []
+            for v in self.smtp_configurations:
+                if isinstance(v, dict):
+                    smtp_configurations_list.append(v)
+                else:
+                    smtp_configurations_list.append(v.to_dict())
+            _dict['smtp_configurations'] = smtp_configurations_list
+        if hasattr(self, 'first') and self.first is not None:
+            if isinstance(self.first, dict):
+                _dict['first'] = self.first
+            else:
+                _dict['first'] = self.first.to_dict()
+        if hasattr(self, 'previous') and self.previous is not None:
+            if isinstance(self.previous, dict):
+                _dict['previous'] = self.previous
+            else:
+                _dict['previous'] = self.previous.to_dict()
+        if hasattr(self, 'next') and self.next is not None:
+            if isinstance(self.next, dict):
+                _dict['next'] = self.next
+            else:
+                _dict['next'] = self.next.to_dict()
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPConfigurationsList object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPConfigurationsList') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPConfigurationsList') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPCreateResponse:
+    """
+    Payload describing a SMTP create response.
+
+    :attr str id: SMTP ID.
+    :attr str name: SMTP name.
+    :attr str description: (optional) SMTP description.
+    :attr str domain: Domain Name.
+    :attr SMTPConfig config: Payload describing a SMTP configuration.
+    :attr datetime created_at: Created time.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        name: str,
+        domain: str,
+        config: 'SMTPConfig',
+        created_at: datetime,
+        *,
+        description: str = None,
+    ) -> None:
+        """
+        Initialize a SMTPCreateResponse object.
+
+        :param str id: SMTP ID.
+        :param str name: SMTP name.
+        :param str domain: Domain Name.
+        :param SMTPConfig config: Payload describing a SMTP configuration.
+        :param datetime created_at: Created time.
+        :param str description: (optional) SMTP description.
+        """
+        self.id = id
+        self.name = name
+        self.description = description
+        self.domain = domain
+        self.config = config
+        self.created_at = created_at
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPCreateResponse':
+        """Initialize a SMTPCreateResponse object from a json dictionary."""
+        args = {}
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        else:
+            raise ValueError('Required property \'id\' not present in SMTPCreateResponse JSON')
+        if 'name' in _dict:
+            args['name'] = _dict.get('name')
+        else:
+            raise ValueError('Required property \'name\' not present in SMTPCreateResponse JSON')
+        if 'description' in _dict:
+            args['description'] = _dict.get('description')
+        if 'domain' in _dict:
+            args['domain'] = _dict.get('domain')
+        else:
+            raise ValueError('Required property \'domain\' not present in SMTPCreateResponse JSON')
+        if 'config' in _dict:
+            args['config'] = SMTPConfig.from_dict(_dict.get('config'))
+        else:
+            raise ValueError('Required property \'config\' not present in SMTPCreateResponse JSON')
+        if 'created_at' in _dict:
+            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        else:
+            raise ValueError('Required property \'created_at\' not present in SMTPCreateResponse JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPCreateResponse object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'domain') and self.domain is not None:
+            _dict['domain'] = self.domain
+        if hasattr(self, 'config') and self.config is not None:
+            if isinstance(self.config, dict):
+                _dict['config'] = self.config
+            else:
+                _dict['config'] = self.config.to_dict()
+        if hasattr(self, 'created_at') and self.created_at is not None:
+            _dict['created_at'] = datetime_to_string(self.created_at)
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPCreateResponse object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPCreateResponse') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPCreateResponse') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPUser:
+    """
+    Payload describing a SMTP User.
+
+    :attr str id: Id.
+    :attr str smtp_config_id: SMTP confg Id.
+    :attr str description: SMTP User description.
+    :attr str domain: Domain Name.
+    :attr str username: SMTP user name.
+    :attr datetime created_at: Updated time.
+    :attr datetime updated_at: Updated time.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        smtp_config_id: str,
+        description: str,
+        domain: str,
+        username: str,
+        created_at: datetime,
+        updated_at: datetime,
+    ) -> None:
+        """
+        Initialize a SMTPUser object.
+
+        :param str id: Id.
+        :param str smtp_config_id: SMTP confg Id.
+        :param str description: SMTP User description.
+        :param str domain: Domain Name.
+        :param str username: SMTP user name.
+        :param datetime created_at: Updated time.
+        :param datetime updated_at: Updated time.
+        """
+        self.id = id
+        self.smtp_config_id = smtp_config_id
+        self.description = description
+        self.domain = domain
+        self.username = username
+        self.created_at = created_at
+        self.updated_at = updated_at
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPUser':
+        """Initialize a SMTPUser object from a json dictionary."""
+        args = {}
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        else:
+            raise ValueError('Required property \'id\' not present in SMTPUser JSON')
+        if 'smtp_config_id' in _dict:
+            args['smtp_config_id'] = _dict.get('smtp_config_id')
+        else:
+            raise ValueError('Required property \'smtp_config_id\' not present in SMTPUser JSON')
+        if 'description' in _dict:
+            args['description'] = _dict.get('description')
+        else:
+            raise ValueError('Required property \'description\' not present in SMTPUser JSON')
+        if 'domain' in _dict:
+            args['domain'] = _dict.get('domain')
+        else:
+            raise ValueError('Required property \'domain\' not present in SMTPUser JSON')
+        if 'username' in _dict:
+            args['username'] = _dict.get('username')
+        else:
+            raise ValueError('Required property \'username\' not present in SMTPUser JSON')
+        if 'created_at' in _dict:
+            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        else:
+            raise ValueError('Required property \'created_at\' not present in SMTPUser JSON')
+        if 'updated_at' in _dict:
+            args['updated_at'] = string_to_datetime(_dict.get('updated_at'))
+        else:
+            raise ValueError('Required property \'updated_at\' not present in SMTPUser JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPUser object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'smtp_config_id') and self.smtp_config_id is not None:
+            _dict['smtp_config_id'] = self.smtp_config_id
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'domain') and self.domain is not None:
+            _dict['domain'] = self.domain
+        if hasattr(self, 'username') and self.username is not None:
+            _dict['username'] = self.username
+        if hasattr(self, 'created_at') and self.created_at is not None:
+            _dict['created_at'] = datetime_to_string(self.created_at)
+        if hasattr(self, 'updated_at') and self.updated_at is not None:
+            _dict['updated_at'] = datetime_to_string(self.updated_at)
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPUser object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPUser') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPUser') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPUserResponse:
+    """
+    Payload describing a SMTP User create response.
+
+    :attr str id: SMTP Id.
+    :attr str description: (optional) SMTP User description.
+    :attr str domain: (optional) Domain Name.
+    :attr str smtp_config_id: SMTP confg Id.
+    :attr str username: SMTP user name.
+    :attr str password: password.
+    :attr datetime created_at: Created time.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        smtp_config_id: str,
+        username: str,
+        password: str,
+        created_at: datetime,
+        *,
+        description: str = None,
+        domain: str = None,
+    ) -> None:
+        """
+        Initialize a SMTPUserResponse object.
+
+        :param str id: SMTP Id.
+        :param str smtp_config_id: SMTP confg Id.
+        :param str username: SMTP user name.
+        :param str password: password.
+        :param datetime created_at: Created time.
+        :param str description: (optional) SMTP User description.
+        :param str domain: (optional) Domain Name.
+        """
+        self.id = id
+        self.description = description
+        self.domain = domain
+        self.smtp_config_id = smtp_config_id
+        self.username = username
+        self.password = password
+        self.created_at = created_at
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPUserResponse':
+        """Initialize a SMTPUserResponse object from a json dictionary."""
+        args = {}
+        if 'id' in _dict:
+            args['id'] = _dict.get('id')
+        else:
+            raise ValueError('Required property \'id\' not present in SMTPUserResponse JSON')
+        if 'description' in _dict:
+            args['description'] = _dict.get('description')
+        if 'domain' in _dict:
+            args['domain'] = _dict.get('domain')
+        if 'smtp_config_id' in _dict:
+            args['smtp_config_id'] = _dict.get('smtp_config_id')
+        else:
+            raise ValueError('Required property \'smtp_config_id\' not present in SMTPUserResponse JSON')
+        if 'username' in _dict:
+            args['username'] = _dict.get('username')
+        else:
+            raise ValueError('Required property \'username\' not present in SMTPUserResponse JSON')
+        if 'password' in _dict:
+            args['password'] = _dict.get('password')
+        else:
+            raise ValueError('Required property \'password\' not present in SMTPUserResponse JSON')
+        if 'created_at' in _dict:
+            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        else:
+            raise ValueError('Required property \'created_at\' not present in SMTPUserResponse JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPUserResponse object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'domain') and self.domain is not None:
+            _dict['domain'] = self.domain
+        if hasattr(self, 'smtp_config_id') and self.smtp_config_id is not None:
+            _dict['smtp_config_id'] = self.smtp_config_id
+        if hasattr(self, 'username') and self.username is not None:
+            _dict['username'] = self.username
+        if hasattr(self, 'password') and self.password is not None:
+            _dict['password'] = self.password
+        if hasattr(self, 'created_at') and self.created_at is not None:
+            _dict['created_at'] = datetime_to_string(self.created_at)
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPUserResponse object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPUserResponse') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPUserResponse') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPUsersList:
+    """
+    Payload describing a SMTP users list request.
+
+    :attr int total_count: Total number of destinations.
+    :attr int offset: Current offset.
+    :attr int limit: limit to show destinations.
+    :attr List[SMTPUser] users: List of users.
+    :attr PageHrefResponse first: (optional) Response having URL of the page.
+    :attr PageHrefResponse previous: (optional) Response having URL of the page.
+    :attr PageHrefResponse next: (optional) Response having URL of the page.
+    """
+
+    def __init__(
+        self,
+        total_count: int,
+        offset: int,
+        limit: int,
+        users: List['SMTPUser'],
+        *,
+        first: 'PageHrefResponse' = None,
+        previous: 'PageHrefResponse' = None,
+        next: 'PageHrefResponse' = None,
+    ) -> None:
+        """
+        Initialize a SMTPUsersList object.
+
+        :param int total_count: Total number of destinations.
+        :param int offset: Current offset.
+        :param int limit: limit to show destinations.
+        :param List[SMTPUser] users: List of users.
+        :param PageHrefResponse first: (optional) Response having URL of the page.
+        :param PageHrefResponse previous: (optional) Response having URL of the
+               page.
+        :param PageHrefResponse next: (optional) Response having URL of the page.
+        """
+        self.total_count = total_count
+        self.offset = offset
+        self.limit = limit
+        self.users = users
+        self.first = first
+        self.previous = previous
+        self.next = next
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPUsersList':
+        """Initialize a SMTPUsersList object from a json dictionary."""
+        args = {}
+        if 'total_count' in _dict:
+            args['total_count'] = _dict.get('total_count')
+        else:
+            raise ValueError('Required property \'total_count\' not present in SMTPUsersList JSON')
+        if 'offset' in _dict:
+            args['offset'] = _dict.get('offset')
+        else:
+            raise ValueError('Required property \'offset\' not present in SMTPUsersList JSON')
+        if 'limit' in _dict:
+            args['limit'] = _dict.get('limit')
+        else:
+            raise ValueError('Required property \'limit\' not present in SMTPUsersList JSON')
+        if 'users' in _dict:
+            args['users'] = [SMTPUser.from_dict(v) for v in _dict.get('users')]
+        else:
+            raise ValueError('Required property \'users\' not present in SMTPUsersList JSON')
+        if 'first' in _dict:
+            args['first'] = PageHrefResponse.from_dict(_dict.get('first'))
+        if 'previous' in _dict:
+            args['previous'] = PageHrefResponse.from_dict(_dict.get('previous'))
+        if 'next' in _dict:
+            args['next'] = PageHrefResponse.from_dict(_dict.get('next'))
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPUsersList object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'total_count') and self.total_count is not None:
+            _dict['total_count'] = self.total_count
+        if hasattr(self, 'offset') and self.offset is not None:
+            _dict['offset'] = self.offset
+        if hasattr(self, 'limit') and self.limit is not None:
+            _dict['limit'] = self.limit
+        if hasattr(self, 'users') and self.users is not None:
+            users_list = []
+            for v in self.users:
+                if isinstance(v, dict):
+                    users_list.append(v)
+                else:
+                    users_list.append(v.to_dict())
+            _dict['users'] = users_list
+        if hasattr(self, 'first') and self.first is not None:
+            if isinstance(self.first, dict):
+                _dict['first'] = self.first
+            else:
+                _dict['first'] = self.first.to_dict()
+        if hasattr(self, 'previous') and self.previous is not None:
+            if isinstance(self.previous, dict):
+                _dict['previous'] = self.previous
+            else:
+                _dict['previous'] = self.previous.to_dict()
+        if hasattr(self, 'next') and self.next is not None:
+            if isinstance(self.next, dict):
+                _dict['next'] = self.next
+            else:
+                _dict['next'] = self.next.to_dict()
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPUsersList object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPUsersList') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPUsersList') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPVerificationResponse:
+    """
+    verification object.
+
+    :attr str type: verification type.
+    :attr str verification: verification status.
+    """
+
+    def __init__(
+        self,
+        type: str,
+        verification: str,
+    ) -> None:
+        """
+        Initialize a SMTPVerificationResponse object.
+
+        :param str type: verification type.
+        :param str verification: verification status.
+        """
+        self.type = type
+        self.verification = verification
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPVerificationResponse':
+        """Initialize a SMTPVerificationResponse object from a json dictionary."""
+        args = {}
+        if 'type' in _dict:
+            args['type'] = _dict.get('type')
+        else:
+            raise ValueError('Required property \'type\' not present in SMTPVerificationResponse JSON')
+        if 'verification' in _dict:
+            args['verification'] = _dict.get('verification')
+        else:
+            raise ValueError('Required property \'verification\' not present in SMTPVerificationResponse JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPVerificationResponse object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
+        if hasattr(self, 'verification') and self.verification is not None:
+            _dict['verification'] = self.verification
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPVerificationResponse object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPVerificationResponse') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPVerificationResponse') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class SMTPVerificationUpdateResponse:
+    """
+    Payload describing SMTP verification response.
+
+    :attr List[SMTPVerificationResponse] status: SMTP verification status.
+    """
+
+    def __init__(
+        self,
+        status: List['SMTPVerificationResponse'],
+    ) -> None:
+        """
+        Initialize a SMTPVerificationUpdateResponse object.
+
+        :param List[SMTPVerificationResponse] status: SMTP verification status.
+        """
+        self.status = status
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPVerificationUpdateResponse':
+        """Initialize a SMTPVerificationUpdateResponse object from a json dictionary."""
+        args = {}
+        if 'status' in _dict:
+            args['status'] = [SMTPVerificationResponse.from_dict(v) for v in _dict.get('status')]
+        else:
+            raise ValueError('Required property \'status\' not present in SMTPVerificationUpdateResponse JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPVerificationUpdateResponse object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'status') and self.status is not None:
+            status_list = []
+            for v in self.status:
+                if isinstance(v, dict):
+                    status_list.append(v)
+                else:
+                    status_list.append(v.to_dict())
+            _dict['status'] = status_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPVerificationUpdateResponse object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPVerificationUpdateResponse') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPVerificationUpdateResponse') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class SPFAttributes:
     """
     The SPF attributes.
 
     :attr str txt_name: (optional) spf text name.
     :attr str txt_value: (optional) spf text value.
     :attr str verification: (optional) spf verification.
@@ -6578,81 +8399,31 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Template') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
-class TemplateConfig:
+class TemplateConfigOneOf:
     """
-    Payload describing a template configuration.
+    TemplateConfigOneOf.
 
-    :attr str body: Template body.
-    :attr str subject: The template subject.
     """
 
     def __init__(
         self,
-        body: str,
-        subject: str,
     ) -> None:
         """
-        Initialize a TemplateConfig object.
+        Initialize a TemplateConfigOneOf object.
 
-        :param str body: Template body.
-        :param str subject: The template subject.
         """
-        self.body = body
-        self.subject = subject
-
-    @classmethod
-    def from_dict(cls, _dict: Dict) -> 'TemplateConfig':
-        """Initialize a TemplateConfig object from a json dictionary."""
-        args = {}
-        if 'body' in _dict:
-            args['body'] = _dict.get('body')
-        else:
-            raise ValueError('Required property \'body\' not present in TemplateConfig JSON')
-        if 'subject' in _dict:
-            args['subject'] = _dict.get('subject')
-        else:
-            raise ValueError('Required property \'subject\' not present in TemplateConfig JSON')
-        return cls(**args)
-
-    @classmethod
-    def _from_dict(cls, _dict):
-        """Initialize a TemplateConfig object from a json dictionary."""
-        return cls.from_dict(_dict)
-
-    def to_dict(self) -> Dict:
-        """Return a json dictionary representing this model."""
-        _dict = {}
-        if hasattr(self, 'body') and self.body is not None:
-            _dict['body'] = self.body
-        if hasattr(self, 'subject') and self.subject is not None:
-            _dict['subject'] = self.subject
-        return _dict
-
-    def _to_dict(self):
-        """Return a json dictionary representing this model."""
-        return self.to_dict()
-
-    def __str__(self) -> str:
-        """Return a `str` version of this TemplateConfig object."""
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __eq__(self, other: 'TemplateConfig') -> bool:
-        """Return `true` when self and other are equal, false otherwise."""
-        if not isinstance(other, self.__class__):
-            return False
-        return self.__dict__ == other.__dict__
-
-    def __ne__(self, other: 'TemplateConfig') -> bool:
-        """Return `true` when self and other are not equal, false otherwise."""
-        return not self == other
+        msg = "Cannot instantiate base class. Instead, instantiate one of the defined subclasses: {0}".format(
+            ", ".join(['TemplateConfigOneOfEmailTemplateConfig', 'TemplateConfigOneOfSlackTemplateConfig'])
+        )
+        raise Exception(msg)
 
 
 class TemplateList:
     """
     Payload describing a template list request.
 
     :attr int total_count: Total number of templates.
@@ -6785,35 +8556,35 @@
     """
     Payload describing a template get request.
 
     :attr str id: Template ID.
     :attr str name: Template name.
     :attr str description: (optional) Template description.
     :attr str type: The type of template.
-    :attr TemplateConfig params: Payload describing a template configuration.
+    :attr TemplateConfigOneOf params:
     :attr datetime created_at: Created time.
     """
 
     def __init__(
         self,
         id: str,
         name: str,
         type: str,
-        params: 'TemplateConfig',
+        params: 'TemplateConfigOneOf',
         created_at: datetime,
         *,
         description: str = None,
     ) -> None:
         """
         Initialize a TemplateResponse object.
 
         :param str id: Template ID.
         :param str name: Template name.
         :param str type: The type of template.
-        :param TemplateConfig params: Payload describing a template configuration.
+        :param TemplateConfigOneOf params:
         :param datetime created_at: Created time.
         :param str description: (optional) Template description.
         """
         self.id = id
         self.name = name
         self.description = description
         self.type = type
@@ -6835,15 +8606,15 @@
         if 'description' in _dict:
             args['description'] = _dict.get('description')
         if 'type' in _dict:
             args['type'] = _dict.get('type')
         else:
             raise ValueError('Required property \'type\' not present in TemplateResponse JSON')
         if 'params' in _dict:
-            args['params'] = TemplateConfig.from_dict(_dict.get('params'))
+            args['params'] = _dict.get('params')
         else:
             raise ValueError('Required property \'params\' not present in TemplateResponse JSON')
         if 'created_at' in _dict:
             args['created_at'] = string_to_datetime(_dict.get('created_at'))
         else:
             raise ValueError('Required property \'created_at\' not present in TemplateResponse JSON')
         return cls(**args)
@@ -9849,56 +11620,66 @@
 
 
 class SubscriptionAttributesSlackAttributesResponse(SubscriptionAttributes):
     """
     The attributes for a Slack notification.
 
     :attr str attachment_color: (optional) Attachment Color for Slack Notification.
+    :attr str template_id_notification: (optional) ID of Base64 converted JSON Slack
+          Blocks w/o Handlebars.
     """
 
     # The set of defined properties for the class
-    _properties = frozenset(['attachment_color'])
+    _properties = frozenset(['attachment_color', 'template_id_notification'])
 
     def __init__(
         self,
         *,
         attachment_color: str = None,
+        template_id_notification: str = None,
         **kwargs,
     ) -> None:
         """
         Initialize a SubscriptionAttributesSlackAttributesResponse object.
 
         :param str attachment_color: (optional) Attachment Color for Slack
                Notification.
+        :param str template_id_notification: (optional) ID of Base64 converted JSON
+               Slack Blocks w/o Handlebars.
         :param **kwargs: (optional) Any additional properties.
         """
         # pylint: disable=super-init-not-called
         self.attachment_color = attachment_color
+        self.template_id_notification = template_id_notification
         for _key, _value in kwargs.items():
             setattr(self, _key, _value)
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'SubscriptionAttributesSlackAttributesResponse':
         """Initialize a SubscriptionAttributesSlackAttributesResponse object from a json dictionary."""
         args = {}
         if 'attachment_color' in _dict:
             args['attachment_color'] = _dict.get('attachment_color')
+        if 'template_id_notification' in _dict:
+            args['template_id_notification'] = _dict.get('template_id_notification')
         args.update({k: v for (k, v) in _dict.items() if k not in cls._properties})
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a SubscriptionAttributesSlackAttributesResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
         if hasattr(self, 'attachment_color') and self.attachment_color is not None:
             _dict['attachment_color'] = self.attachment_color
+        if hasattr(self, 'template_id_notification') and self.template_id_notification is not None:
+            _dict['template_id_notification'] = self.template_id_notification
         for _key in [
             k for k in vars(self).keys() if k not in SubscriptionAttributesSlackAttributesResponse._properties
         ]:
             _dict[_key] = getattr(self, _key)
         return _dict
 
     def _to_dict(self):
@@ -10549,48 +12330,58 @@
 
 
 class SubscriptionCreateAttributesSlackAttributes(SubscriptionCreateAttributes):
     """
     The attributes for a slack notification.
 
     :attr str attachment_color: (optional) Attachment Color for the slack message.
+    :attr str template_id_notification: (optional) ID of Base64 converted JSON Slack
+          Blocks w/o Handlebars.
     """
 
     def __init__(
         self,
         *,
         attachment_color: str = None,
+        template_id_notification: str = None,
     ) -> None:
         """
         Initialize a SubscriptionCreateAttributesSlackAttributes object.
 
         :param str attachment_color: (optional) Attachment Color for the slack
                message.
+        :param str template_id_notification: (optional) ID of Base64 converted JSON
+               Slack Blocks w/o Handlebars.
         """
         # pylint: disable=super-init-not-called
         self.attachment_color = attachment_color
+        self.template_id_notification = template_id_notification
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'SubscriptionCreateAttributesSlackAttributes':
         """Initialize a SubscriptionCreateAttributesSlackAttributes object from a json dictionary."""
         args = {}
         if 'attachment_color' in _dict:
             args['attachment_color'] = _dict.get('attachment_color')
+        if 'template_id_notification' in _dict:
+            args['template_id_notification'] = _dict.get('template_id_notification')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a SubscriptionCreateAttributesSlackAttributes object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
         if hasattr(self, 'attachment_color') and self.attachment_color is not None:
             _dict['attachment_color'] = self.attachment_color
+        if hasattr(self, 'template_id_notification') and self.template_id_notification is not None:
+            _dict['template_id_notification'] = self.template_id_notification
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
@@ -11232,48 +13023,58 @@
 
 
 class SubscriptionUpdateAttributesSlackAttributes(SubscriptionUpdateAttributes):
     """
     The attributes for a slack notification.
 
     :attr str attachment_color: (optional) Attachment Color for the slack message.
+    :attr str template_id_notification: (optional) ID of Base64 converted JSON Slack
+          Blocks w/o Handlebars.
     """
 
     def __init__(
         self,
         *,
         attachment_color: str = None,
+        template_id_notification: str = None,
     ) -> None:
         """
         Initialize a SubscriptionUpdateAttributesSlackAttributes object.
 
         :param str attachment_color: (optional) Attachment Color for the slack
                message.
+        :param str template_id_notification: (optional) ID of Base64 converted JSON
+               Slack Blocks w/o Handlebars.
         """
         # pylint: disable=super-init-not-called
         self.attachment_color = attachment_color
+        self.template_id_notification = template_id_notification
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'SubscriptionUpdateAttributesSlackAttributes':
         """Initialize a SubscriptionUpdateAttributesSlackAttributes object from a json dictionary."""
         args = {}
         if 'attachment_color' in _dict:
             args['attachment_color'] = _dict.get('attachment_color')
+        if 'template_id_notification' in _dict:
+            args['template_id_notification'] = _dict.get('template_id_notification')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a SubscriptionUpdateAttributesSlackAttributes object from a json dictionary."""
         return cls.from_dict(_dict)
 
     def to_dict(self) -> Dict:
         """Return a json dictionary representing this model."""
         _dict = {}
         if hasattr(self, 'attachment_color') and self.attachment_color is not None:
             _dict['attachment_color'] = self.attachment_color
+        if hasattr(self, 'template_id_notification') and self.template_id_notification is not None:
+            _dict['template_id_notification'] = self.template_id_notification
         return _dict
 
     def _to_dict(self):
         """Return a json dictionary representing this model."""
         return self.to_dict()
 
     def __str__(self) -> str:
@@ -11349,14 +13150,143 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SubscriptionUpdateAttributesWebhookAttributes') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class TemplateConfigOneOfEmailTemplateConfig(TemplateConfigOneOf):
+    """
+    Payload describing an email template configuration.
+
+    :attr str body: Template body.
+    :attr str subject: (optional) The template subject.
+    """
+
+    def __init__(
+        self,
+        body: str,
+        *,
+        subject: str = None,
+    ) -> None:
+        """
+        Initialize a TemplateConfigOneOfEmailTemplateConfig object.
+
+        :param str body: Template body.
+        :param str subject: (optional) The template subject.
+        """
+        # pylint: disable=super-init-not-called
+        self.body = body
+        self.subject = subject
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'TemplateConfigOneOfEmailTemplateConfig':
+        """Initialize a TemplateConfigOneOfEmailTemplateConfig object from a json dictionary."""
+        args = {}
+        if 'body' in _dict:
+            args['body'] = _dict.get('body')
+        else:
+            raise ValueError('Required property \'body\' not present in TemplateConfigOneOfEmailTemplateConfig JSON')
+        if 'subject' in _dict:
+            args['subject'] = _dict.get('subject')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a TemplateConfigOneOfEmailTemplateConfig object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'body') and self.body is not None:
+            _dict['body'] = self.body
+        if hasattr(self, 'subject') and self.subject is not None:
+            _dict['subject'] = self.subject
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this TemplateConfigOneOfEmailTemplateConfig object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'TemplateConfigOneOfEmailTemplateConfig') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'TemplateConfigOneOfEmailTemplateConfig') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class TemplateConfigOneOfSlackTemplateConfig(TemplateConfigOneOf):
+    """
+    Payload describing a slack template configuration.
+
+    :attr str body: Template body.
+    """
+
+    def __init__(
+        self,
+        body: str,
+    ) -> None:
+        """
+        Initialize a TemplateConfigOneOfSlackTemplateConfig object.
+
+        :param str body: Template body.
+        """
+        # pylint: disable=super-init-not-called
+        self.body = body
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'TemplateConfigOneOfSlackTemplateConfig':
+        """Initialize a TemplateConfigOneOfSlackTemplateConfig object from a json dictionary."""
+        args = {}
+        if 'body' in _dict:
+            args['body'] = _dict.get('body')
+        else:
+            raise ValueError('Required property \'body\' not present in TemplateConfigOneOfSlackTemplateConfig JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a TemplateConfigOneOfSlackTemplateConfig object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'body') and self.body is not None:
+            _dict['body'] = self.body
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this TemplateConfigOneOfSlackTemplateConfig object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'TemplateConfigOneOfSlackTemplateConfig') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'TemplateConfigOneOfSlackTemplateConfig') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 ##############################################################################
 # Pagers
 ##############################################################################
 
 
 class SourcesPager:
     """
@@ -11880,7 +13810,157 @@
         :rtype: List[dict]
         """
         results = []
         while self.has_next():
             next_page = self.get_next()
             results.extend(next_page)
         return results
+
+
+class SmtpConfigurationsPager:
+    """
+    SmtpConfigurationsPager can be used to simplify the use of the "list_smtp_configurations" method.
+    """
+
+    def __init__(
+        self,
+        *,
+        client: EventNotificationsV1,
+        instance_id: str,
+        limit: int = None,
+        search: str = None,
+    ) -> None:
+        """
+        Initialize a SmtpConfigurationsPager object.
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param int limit: (optional) Page limit for paginated results.
+        :param str search: (optional) Search string for filtering results.
+        """
+        self._has_next = True
+        self._client = client
+        self._page_context = {'next': None}
+        self._instance_id = instance_id
+        self._limit = limit
+        self._search = search
+
+    def has_next(self) -> bool:
+        """
+        Returns true if there are potentially more results to be retrieved.
+        """
+        return self._has_next
+
+    def get_next(self) -> List[dict]:
+        """
+        Returns the next page of results.
+        :return: A List[dict], where each element is a dict that represents an instance of SMTPConfiguration.
+        :rtype: List[dict]
+        """
+        if not self.has_next():
+            raise StopIteration(message='No more results available')
+
+        result = self._client.list_smtp_configurations(
+            instance_id=self._instance_id,
+            limit=self._limit,
+            search=self._search,
+            offset=self._page_context.get('next'),
+        ).get_result()
+
+        next = None
+        next_page_link = result.get('next')
+        if next_page_link is not None:
+            next = get_query_param(next_page_link.get('href'), 'offset')
+        self._page_context['next'] = next
+        if next is None:
+            self._has_next = False
+
+        return result.get('smtp_configurations')
+
+    def get_all(self) -> List[dict]:
+        """
+        Returns all results by invoking get_next() repeatedly
+        until all pages of results have been retrieved.
+        :return: A List[dict], where each element is a dict that represents an instance of SMTPConfiguration.
+        :rtype: List[dict]
+        """
+        results = []
+        while self.has_next():
+            next_page = self.get_next()
+            results.extend(next_page)
+        return results
+
+
+class SmtpUsersPager:
+    """
+    SmtpUsersPager can be used to simplify the use of the "list_smtp_users" method.
+    """
+
+    def __init__(
+        self,
+        *,
+        client: EventNotificationsV1,
+        instance_id: str,
+        id: str,
+        limit: int = None,
+        search: str = None,
+    ) -> None:
+        """
+        Initialize a SmtpUsersPager object.
+        :param str instance_id: Unique identifier for IBM Cloud Event Notifications
+               instance.
+        :param str id: Unique identifier for SMTP.
+        :param int limit: (optional) Page limit for paginated results.
+        :param str search: (optional) Search string for filtering results.
+        """
+        self._has_next = True
+        self._client = client
+        self._page_context = {'next': None}
+        self._instance_id = instance_id
+        self._id = id
+        self._limit = limit
+        self._search = search
+
+    def has_next(self) -> bool:
+        """
+        Returns true if there are potentially more results to be retrieved.
+        """
+        return self._has_next
+
+    def get_next(self) -> List[dict]:
+        """
+        Returns the next page of results.
+        :return: A List[dict], where each element is a dict that represents an instance of SMTPUser.
+        :rtype: List[dict]
+        """
+        if not self.has_next():
+            raise StopIteration(message='No more results available')
+
+        result = self._client.list_smtp_users(
+            instance_id=self._instance_id,
+            id=self._id,
+            limit=self._limit,
+            search=self._search,
+            offset=self._page_context.get('next'),
+        ).get_result()
+
+        next = None
+        next_page_link = result.get('next')
+        if next_page_link is not None:
+            next = get_query_param(next_page_link.get('href'), 'offset')
+        self._page_context['next'] = next
+        if next is None:
+            self._has_next = False
+
+        return result.get('users')
+
+    def get_all(self) -> List[dict]:
+        """
+        Returns all results by invoking get_next() repeatedly
+        until all pages of results have been retrieved.
+        :return: A List[dict], where each element is a dict that represents an instance of SMTPUser.
+        :rtype: List[dict]
+        """
+        results = []
+        while self.has_next():
+            next_page = self.get_next()
+            results.extend(next_page)
+        return results
```

### Comparing `ibm-eventnotifications-0.4.0/ibm_eventnotifications/version.py` & `ibm-eventnotifications-0.5.0/ibm_eventnotifications/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_eventnotifications
 """
-__version__ = '0.4.0'
+__version__ = '0.5.0'
```

### Comparing `ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/PKG-INFO` & `ibm-eventnotifications-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,8 @@
-Metadata-Version: 2.1
-Name: ibm-eventnotifications
-Version: 0.4.0
-Summary: Python server SDK for IBM Cloud Event Notifications service
-Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
-Author: IBM
-Author-email: Notifications-prod@ibm.com
-License: Apache 2.0
-Keywords: ibm_eventnotifications
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# IBM Cloud Event Notifications Python Admin SDK 0.4.0
+# IBM Cloud Event Notifications Python Admin SDK 0.5.0
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -62,19 +37,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.4.0"
+pip install --upgrade "ibm_eventnotifications>=0.5.0"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.4.0"
+easy_install --upgrade "ibm_eventnotifications>=0.5.0"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
@@ -139,28 +114,42 @@
 - [Templates](#templates)
     - [Create Template](#create-template)
     - [List Templates](#list-templates)
     - [Get Template](#get-template)
     - [Update Template](#update-template)
     - [Delete Template](#delete-template)
 - [Push Destination APIs](#push-destination-apis)
-  - [Create Destination tag subscription](#create-destination-tag-subscription)
-  - [List Destination tag subscription](#list-destination-tag-subscription)
-  - [Delete Destination device tag subscription](#delete-destination-device-tag-subscription)
+    - [Create Destination tag subscription](#create-destination-tag-subscription)
+    - [List Destination tag subscription](#list-destination-tag-subscription)
+    - [Delete Destination device tag subscription](#delete-destination-device-tag-subscription)
 - [Subscriptions](#subscriptions)
     - [Create Subscription](#create-subscription)
     - [List Subscriptions](#list-subscriptions)
     - [Get Subscription](#get-subscription)
     - [Update Subscription](#update-subscription)
     - [Delete Subscription](#delete-subscription)
 - [Integration](#integration)
-  - [Create Integration](#create-integration)
-  - [List Integrations](#list-integrations)
-  - [Get Integrations](#get-integration)
-  - [Update Integration](#update-integration)  
+    - [Create Integration](#create-integration)
+    - [List Integrations](#list-integrations)
+    - [Get Integrations](#get-integration)
+    - [Update Integration](#update-integration)
+- [SMTP Configurations](#SMTPConfigurations)
+	- [Create SMTP Configuration](#create-smtp-configuration)
+	- [Create SMTP User](#create-smtp-user)
+	- [Get SMTP Configuration](#get-smtp-configuration)
+	- [Get SMTP User](#get-smtp-user)	
+	- [Get SMTP Allowed Ips](#get-smtp-allowed-ips)
+	- [List SMTP Configurations](#list-smtp-configurations)
+	- [List SMTP Users](#list-smtp-users)
+	- [Update SMTP Configuration](#update-smtp-configuration)
+	- [Update SMTP User](#update-smtp-user)
+	- [Update SMTP Allowed Ips](#update-smtp-allowed-ips)
+	- [Delete SMTP User](#delete-smtp-user)
+	- [Delete SMTP Configuration](#delete-smtp-user)
+	- [Verify SMTP](#verify-smtp)
 - [Send Notifications](#send-notifications)
 
 ## Source 
 
 ### Create Source
 
 ```py
@@ -444,28 +433,48 @@
 Template is a pre-defined layout, that may include content like images, text and dynamic content based on event. Rather than creating a new content from scratch each time, you can use a template as a base and configure them in subscription. 
 supports the following templates:
 
 - Custom Email notification
 - Custom Email invitation
 
 ### Create Template
+
+#### Custom Email Template
 ```py
 template_config_model = {
     'body': 'base 64 encoded html content',
     'subject': 'Hi this is invitation for invitation message',
 }
 
 create_template_response = event_notifications_service.create_template(
     instance_id=<instance-id>,
     name=<template-name>,
     type=<template-type>,
     params=template_config_model,
     description=<template-description>
 ).get_result()
 ```
+For custom email supported template type values: smtp_custom.invitation, smtp_custom.notification 
+
+#### Slack Template
+```py
+template_config_model = {
+    'body': 'base 64 encoded json body',
+}
+
+create_template_response = event_notifications_service.create_template(
+    instance_id=<instance-id>,
+    name=<template-name>,
+    type=<template-type>,
+    params=template_config_model,
+    description=<template-description>
+).get_result()
+```
+For slack template supported template type value: slack.notification
+
 ### List Templates
 ```py
 list_templates_response = event_notifications_service.list_templates(
     instance_id=<instance-id>,
     limit=<limit>,
     offset=<offset>,
     search=<search>
@@ -691,14 +700,203 @@
   id=<integration_id>,
   metadata=integration_metadata
 )
 
 integration_response = update_integration_response.get_result()
 ```
 
+## SMTPConfigurations
+
+### Create SMTP Configuration
+
+```py
+
+create_smtp_config_response = self.event_notifications_service.create_smtp_configuration(
+    instance_id=<instance_id>,
+    name=<smtp-config-name>,
+    domain=<smtp-domain-name>,
+    description=<smtp-description>
+)
+
+smtp_response = create_smtp_config_response.get_result()
+
+```
+
+### Create SMTP User
+
+```py
+
+create_smtp_user_response = self.event_notifications_service.create_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp-config-id>,
+    description=<smtp-description>
+)
+
+create_user_response = create_smtp_user_response.get_result()
+
+```
+
+### Get SMTP Configuration
+
+```py
+
+get_smtp_config_response = self.event_notifications_service.get_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+get_smtp_config_response = get_smtp_config_response.get_result()
+
+```
+
+### Get SMTP User
+
+```py
+
+get_smtp_user_response = self.event_notifications_service.get_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<smtp_user_id>
+)
+
+get_smtp_user_response = get_smtp_user_response.get_result()
+
+```
+
+### Get SMTP Allowed Ips
+
+```py
+
+get_smtp_allowed_ip_response = self.event_notifications_service.get_smtp_allowed_ips(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+get_smtp_allowed_ip_response = get_smtp_allowed_ip_response.get_result()
+
+```
+
+### List SMTP Configurations
+
+```py
+
+list_smtp_config_response = self.event_notifications_service.list_smtp_configurations(
+    instance_id=<instance-id>,
+    limit=<limit>,
+    offset=<offset>,
+    search=<search>,
+)
+
+list_smtp_config_response = list_smtp_config_response.get_result()
+
+```
+
+### List SMTP Users
+
+```py
+
+list_smtp_user_response = self.event_notifications_service.list_smtp_users(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    limit=<limit>,
+    offset=<offset>,
+    search=<search>,
+)
+
+list_smtp_user_response = list_smtp_user_response.get_result()
+
+```
+
+### Update SMTP Configuration
+
+```py
+
+update_smtp_config_response = self.event_notifications_service.update_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    name=<smtp-name>,
+    description=<smtp-description>,
+)
+
+update_smtp_config_response = update_smtp_config_response.get_result()
+
+```
+
+### Update SMTP User
+
+```py
+
+update_smtp_user_response = self.event_notifications_service.update_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<smtp_user_id>,
+    description=<smtp-description>,
+)
+
+update_smtp_user_response = update_smtp_user_response.get_result()
+
+```
+
+### Update SMTP Allowed IPs
+
+```py
+
+subnets = ['<subnet-ips>']
+update_smtp_allowed_ip_response = self.event_notifications_service.update_smtp_allowed_ips(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    subnets=subnets
+)
+
+allowed_ip_response = update_smtp_allowed_ip_response.get_result()
+
+```
+
+### Delete SMTP User
+
+```py
+
+delete_smtp_user_response = self.event_notifications_service.delete_smtp_user(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+    user_id=<user-id>
+)
+
+print(json.dumps(delete_smtp_user_response, indent=2))
+
+```
+
+### Delete SMTP Configuration
+
+```py
+
+delete_smtp_config_response = self.event_notifications_service.delete_smtp_configuration(
+    instance_id=<instance-id>,
+    id=<smtp_config_id>,
+)
+
+print(json.dumps(delete_smtp_config_response, indent=2))
+
+```
+
+### Verify SMTP
+
+```py
+
+update_verify_smtp_response = self.event_notifications_service.update_verify_smtp(
+    instance_id=<instance-id>,
+    type=<verification-type>,
+    id=<smtp_config_id>
+)
+
+verify_response = update_verify_smtp_response.get_result()
+
+```
+supported verification types are dkim,spf and en_authorization.
+
 ### Send Notifications
 
 
 ```py
 notification_devices_model = {
   'fcm_devices': ['<fcm-device-ids>'],
   'apns_devices': ['<apns-device-ids>'],
@@ -744,28 +942,30 @@
 type_value = "<notification-type>"
 notifications_source = "<notification-source>"
 htmlbody = '"Hi  ,<br/>Certificate expiring in 90 days.<br/><br/>Please login to ' \
            '<a href="https: //cloud.ibm.com/security-compliance/dashboard">' \
            'Security and Complaince dashboard</a> to find more information<br/>"'
 mailto = '[\"abc@ibm.com\", \"def@us.ibm.com\"]'
 smsto = '[\"+911234567890\", \"+911224567890\"]'
+templates = '["149b0e11-8a7c-4fda-a847-5d79e01b71dc"]'
 
 notification_create_model = {
     'ibmenseverity': notification_severity,
     'ibmenfcmbody': json.dumps(notification_fcm_body_model),
     'ibmenpushto': json.dumps(notification_devices_model),
     'ibmenapnsbody': json.dumps(notification_apns_body_model),
     'ibmensourceid': source_id,
     'ibmendefaultshort': 'short info',
     'ibmendefaultlong': 'long info',
     'ibmensafaribody': json.dumps(notificationSafariBodymodel),
     'ibmenhtmlbody': htmlbody,
     'ibmensubject': 'Findings on IBM Cloud Security Advisor',
     'ibmenmailto': mailto,
     'ibmensmsto': smsto,
+    "ibmentemplates": templates,
     'id': notification_id,
     'source': notifications_source,
     'type': type_value,
     'specversion': '1.0',
     'time': '2019-01-01T12:00:00.000Z',
 }
 
@@ -814,30 +1014,58 @@
   - **ibmenfirefoxheaders** (_string_) - Headers for the Firefox notifications. Refer [this official documentation](https://developer.mozilla.org/en-US/docs/Web/API/Notification/Notification) for more.
   - **ibmendefaultshort*** (_string_) - Default short text for the message.
   - **ibmendefaultlong*** (_string_) - Default long text for the message.
   - **specversion*** (_string_) - Spec version of the Event Notifications. Default value is `1.0`. 
   - **ibmenhtmlbody*** (_string_) - The html body of notification for email.
   - **ibmenmailto*** (_Array of string_) - Array of email ids to which the notification to be sent.
   - **ibmensmsto*** (_Array of string_) - Array of SMS numbers to which the notification to be sent.
+  - **ibmentemplates*** (_Array of string_) - Array of template IDs that needs to be applied while sending notificatin for custom domain email and slack destination.
 
 Note: variable with * represents the mandatory attribute.
 </details>
 
 ## Set Environment
 
 Find `event_notifications_v1.env.hide` in the repo and rename it to `event_notifications_v1.env`. After that add the values for,
 
 - `EVENT_NOTIFICATIONS_URL` - Add the Event Notifications service instance Url.
 - `EVENT_NOTIFICATIONS_APIKEY` - Add the Event Notifications service instance apikey.
 - `EVENT_NOTIFICATIONS_GUID` - Add the Event Notifications service instance GUID.
 
-Optional 
+**Optional**
 - `EVENT_NOTIFICATIONS_AUTH_URL` - Add the IAM url if you are using IBM test cloud.
 - `EVENT_NOTIFICATIONS_FCM_KEY` - Add firebase server key for Android FCM destination.
 - `EVENT_NOTIFICATIONS_FCM_ID` - Add firebase sender Id for Android FCM destination.
+- `EVENT_NOTIFICATIONS_FCM_PROJECT_ID` - fcm project id
+- `EVENT_NOTIFICATIONS_FCM_CLIENT_EMAIL` - fcm client email
+- `EVENT_NOTIFICATIONS_FCM_PRIVATE_KEY` - fcm private key
+- `EVENT_NOTIFICATIONS_SAFARI_CERTIFICATE` - safari certificate path
+
+- `EVENT_NOTIFICATIONS_SNOW_CLIENT_ID` - service now client id
+- `EVENT_NOTIFICATIONS_SNOW_CLIENT_SECRET` - service now client secret
+- `EVENT_NOTIFICATIONS_SNOW_USER_NAME` - service now user name
+- `EVENT_NOTIFICATIONS_SNOW_PASSWORD` - service now password
+- `EVENT_NOTIFICATIONS_SNOW_INSTANCE_NAME` - service now instance name
+
+- `EVENT_NOTIFICATIONS_COS_BUCKET_NAME` - cloud object storage bucket name
+- `EVENT_NOTIFICATIONS_COS_INSTANCE` - cloud object storage instance id
+- `EVENT_NOTIFICATIONS_COS_INSTANCE_CRN` - cloud object storage instance crn
+- `EVENT_NOTIFICATIONS_COS_ENDPOINT` - cloud object storage end point
+
+- `EVENT_NOTIFICATIONS_CODE_ENGINE_URL` - code engine app url
+- `EVENT_NOTIFICATIONS_CODE_ENGINE_PROJECT_CRN` - code engine project crn
+- `EVENT_NOTIFICATIONS_HUAWEI_CLIENT_SECRET` - huawei client secret
+- `EVENT_NOTIFICATIONS_HUAWEI_CLIENT_ID` - huawei client id
+
+- `EVENT_NOTIFICATIONS_SLACK_URL` - slack webhook url
+- `EVENT_NOTIFICATIONS_MS_TEAMS_URL` - msteams webhook url
+- `EVENT_NOTIFICATIONS_PD_ROUTING_KEY` - pagerduty routing key
+- `EVENT_NOTIFICATIONS_PD_API_KEY` - pagerduty api key
+- `EVENT_NOTIFICATIONS_TEMPLATE_BODY` - base 64 encoded html content
+- `EVENT_NOTIFICATIONS_SLACK_TEMPLATE_BODY` - base 64 encoded json body
 
 ## Questions
 
 If you are having difficulties using this SDK or have a question about the IBM Cloud services,
 please ask a question
 [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-cloud).
 
@@ -852,9 +1080,7 @@
 ## Contributing
 See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## License
 
 This SDK is released under the Apache 2.0 license.
 The license's full text can be found in [LICENSE](LICENSE).
-
-
```

### Comparing `ibm-eventnotifications-0.4.0/ibm_eventnotifications.egg-info/SOURCES.txt` & `ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.4.0/setup.py` & `ibm-eventnotifications-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 PACKAGE_NAME = 'ibm_eventnotifications'
 PACKAGE_DESC = 'Python server SDK for IBM Cloud Event Notifications service'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

