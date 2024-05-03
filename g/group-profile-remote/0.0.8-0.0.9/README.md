# Comparing `tmp/group-profile-remote-0.0.8.tar.gz` & `tmp/group-profile-remote-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group-profile-remote-0.0.8.tar", last modified: Wed Sep 13 16:39:28 2023, max compression
+gzip compressed data, was "group-profile-remote-0.0.9.tar", last modified: Sat Nov 11 16:11:07 2023, max compression
```

## Comparing `group-profile-remote-0.0.8.tar` & `group-profile-remote-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:39:28.612234 group-profile-remote-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-09-13 16:39:28.612234 group-profile-remote-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-09-13 16:39:07.000000 group-profile-remote-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:39:28.612234 group-profile-remote-0.0.8/group_profile_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:39:28.612234 group-profile-remote-0.0.8/group_profile_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:39:07.000000 group-profile-remote-0.0.8/group_profile_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2023-09-13 16:39:07.000000 group-profile-remote-0.0.8/group_profile_remote/src/group_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:39:28.612234 group-profile-remote-0.0.8/group_profile_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-09-13 16:39:28.000000 group-profile-remote-0.0.8/group_profile_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-09-13 16:39:28.000000 group-profile-remote-0.0.8/group_profile_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 16:39:28.000000 group-profile-remote-0.0.8/group_profile_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-13 16:39:28.000000 group-profile-remote-0.0.8/group_profile_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-13 16:39:28.000000 group-profile-remote-0.0.8/group_profile_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-09-13 16:39:07.000000 group-profile-remote-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 16:39:28.612234 group-profile-remote-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-09-13 16:39:07.000000 group-profile-remote-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 16:11:07.036668 group-profile-remote-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-11-11 16:11:07.036668 group-profile-remote-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-11-11 16:10:36.000000 group-profile-remote-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 16:11:07.032668 group-profile-remote-0.0.9/group_profile_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 16:11:07.032668 group-profile-remote-0.0.9/group_profile_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-11 16:10:36.000000 group-profile-remote-0.0.9/group_profile_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-11-11 16:10:36.000000 group-profile-remote-0.0.9/group_profile_remote/src/group_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 16:11:07.032668 group-profile-remote-0.0.9/group_profile_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-11-11 16:11:07.000000 group-profile-remote-0.0.9/group_profile_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2023-11-11 16:11:07.000000 group-profile-remote-0.0.9/group_profile_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 16:11:07.000000 group-profile-remote-0.0.9/group_profile_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-11 16:11:07.000000 group-profile-remote-0.0.9/group_profile_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-11 16:11:07.000000 group-profile-remote-0.0.9/group_profile_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2023-11-11 16:10:36.000000 group-profile-remote-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-11 16:11:07.036668 group-profile-remote-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-11-11 16:10:36.000000 group-profile-remote-0.0.9/setup.py
```

### Comparing `group-profile-remote-0.0.8/README.md` & `group-profile-remote-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `group-profile-remote-0.0.8/group_profile_remote/src/group_profile.py` & `group-profile-remote-0.0.9/group_profile_remote/src/group_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,163 +1,176 @@
 # TODO: This is an example file which you should delete after impenting
 import requests
-from our_url.src.index import UrlCirclez
-import os, sys
+from url_local.url_circlez import OurUrl
+import os
+import sys
 import json
 from logger_local.Logger import Logger
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
-from our_url.src.component_name_enum import ComponentName
-from our_url.src.entity_name_enum import EntityName
-from our_url.src.action_name_enum import ActionName
+from url_local.component_name_enum import ComponentName
+from url_local.entity_name_enum import EntityName
+from url_local.action_name_enum import ActionName
+from user_context_remote.user_context import UserContext
 from dotenv import load_dotenv
 load_dotenv()
 
 
 GROUP_PROFILE_COMPONENT_ID = 211
-GROUP_PROFILE_COMPONENT_NAME="Group Profile Remote Python"
-COMPONENT_CATEGORY=LoggerComponentEnum.ComponentCategory.Code.value
-COMPONENT_TYPE=LoggerComponentEnum.ComponentType.Remote.value
-DEVELOPER_EMAIL="yarden.d@circ.zone"
-
-obj={
-    'component_id':GROUP_PROFILE_COMPONENT_ID,
-    'component_name':GROUP_PROFILE_COMPONENT_NAME,
-    'component_category':COMPONENT_CATEGORY,
-    'component_type':COMPONENT_TYPE,
-    "developer_email":DEVELOPER_EMAIL
+GROUP_PROFILE_COMPONENT_NAME = "Group Profile Remote Python"
+COMPONENT_CATEGORY = LoggerComponentEnum.ComponentCategory.Code.value
+COMPONENT_TYPE = LoggerComponentEnum.ComponentType.Remote.value
+DEVELOPER_EMAIL = "yarden.d@circ.zone"
+
+obj = {
+    'component_id': GROUP_PROFILE_COMPONENT_ID,
+    'component_name': GROUP_PROFILE_COMPONENT_NAME,
+    'component_category': COMPONENT_CATEGORY,
+    'component_type': COMPONENT_TYPE,
+    "developer_email": DEVELOPER_EMAIL
 }
 
 BRAND_NAME = os.getenv("BRAND_NAME")
 ENVIRONMENT_NAME = os.getenv("ENVIRONMENT_NAME")
 GROUP_PROFILE_API_VERSION = 1
 
+
 class GroupProfile:
 
     def __init__(self):
-        self.url_circlez = UrlCirclez()
+        self.url_circlez = OurUrl()
         self.logger = Logger.create_logger(object=obj)
         self.brand_name = BRAND_NAME
         self.env_name = ENVIRONMENT_NAME
-        
-
 
-    def create_group_profile(self, group_id: str, relationship_type_id: str):
+    def create_group_profile(self, group_id: str, relationship_type_id: str, jwt_token: str):
         self.logger.start("Start create group-rofile-remote")
+        user = UserContext.login_using_jwt(jwt_token)
+        profile_id = str(user.get_real_profile_id())
         try:
             url = self.url_circlez.endpoint_url(
-                brand_name = self.brand_name,
-                environment_name = self.env_name,
-                component = ComponentName.GROUP_PROFILE.value,
-                entity = EntityName.GROUP_PROFILE.value,
-                version = GROUP_PROFILE_API_VERSION,
-                action = ActionName.CREATE_GROUP_PROFILE.value, # "createGroupProfile",
+                brand_name=self.brand_name,
+                environment_name=self.env_name,
+                component_name=ComponentName.GROUP_PROFILE.value,
+                entity_name=EntityName.GROUP_PROFILE.value,
+                version=GROUP_PROFILE_API_VERSION,
+                action_name=ActionName.CREATE_GROUP_PROFILE.value,  # "createGroupProfile",
             )
-            self.logger.info("Endpoint group profile - createGroupProfile action: " + url)
-        
+            self.logger.info(
+                "Endpoint group profile - createGroupProfile action: " + url)
+
             payload = {
-                'groupId': group_id,
-                'profileId': str(self.logger.userContext.get_real_profile_id()),
-                'relationshipTypeId': relationship_type_id
+                "groupId": f"{group_id}",
+                "profileId": f"{profile_id}",
+                "relationshipTypeId": f"{relationship_type_id}"
             }
 
             headers = {
-                'Content-Type': 'application/json',
-                'Authorization': f'Bearer {self.logger.userContext.get_jwt_token()}',
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {jwt_token}",
             }
 
-            
-            response = requests.post(url, json=payload, headers=headers)
-            self.logger.end(f"End create group-profile-remote, response: {str(response)}")
+            print(payload)
+            print(headers)
+            response = requests.post(url=url, json=payload, headers=headers)
+            print(response.text)
+            self.logger.end(
+                f"End create group-profile-remote, response: {str(response)}")
             return response
-        
+
         except requests.ConnectionError as e:
-            self.logger.exception("Network problem (e.g. failed to connect)", e)
+            self.logger.exception(
+                "Network problem (e.g. failed to connect)", object=e)
         except requests.Timeout as e:
             self.logger.exception("Request timed out", e)
         except requests.RequestException as e:
-            self.logger.exception(f"General error: {str(e)}", e)
+            self.logger.exception(f"General error: {str(e)}", object=e)
         except Exception as e:
-            self.logger.exception(f"An unexpected error occurred: {str(e)}", e)
-        
-        self.logger.end(f"End create group-profile-remote")
-
+            self.logger.exception(
+                f"An unexpected error occurred: {str(e)}", object=e)
 
+        self.logger.end(f"End create group-profile-remote")
 
     def get_group_profile(self, group_id: str, relationship_type_id: str):
         self.logger.start("Start get group-profile-remote")
         try:
             url = self.url_circlez.endpoint_url(
-                brand_name = self.brand_name,
-                environment_name = self.env_name,
-                component = ComponentName.GROUP_PROFILE.value,
-                entity = EntityName.GROUP_PROFILE.value,
-                version = GROUP_PROFILE_API_VERSION,
-                action = ActionName.GET_GROUP_PROFILE.value, # "getGroupProfileByGroupIdProfileId",
+                brand_name=self.brand_name,
+                environment_name=self.env_name,
+                component_name=ComponentName.GROUP_PROFILE.value,
+                entity_name=EntityName.GROUP_PROFILE.value,
+                version=GROUP_PROFILE_API_VERSION,
+                # "getGroupProfileByGroupIdProfileId",
+                action_name=ActionName.GET_GROUP_PROFILE.value,
                 query_parameters={
                     'groupId': group_id,
                     'profileId': str(self.logger.userContext.get_real_profile_id()),
                 }
             )
-            self.logger.info("Endpoint group profile - getGroupProfileByGroupIdProfileId action: " + url)
+            self.logger.info(
+                "Endpoint group profile - getGroupProfileByGroupIdProfileId action: " + url)
 
             headers = {
                 'Content-Type': 'application/json',
-                'Authorization': f'Bearer {self.logger.userContext.get_jwt_token()}',
+                'Authorization': f'Bearer {self.logger.userContext.get_user_JWT()}',
             }
 
             response = requests.get(url, headers=headers)
-            self.logger.end(f"End get group-profile-remote, response: {str(response)}")
+            self.logger.end(
+                f"End get group-profile-remote, response: {str(response)}")
             return response
 
         except requests.ConnectionError as e:
-            self.logger.exception("Network problem (e.g. failed to connect)", e)
+            self.logger.exception(
+                "Network problem (e.g. failed to connect)", object=e)
         except requests.Timeout as e:
-            self.logger.exception("Request timed out", e)
+            self.logger.exception("Request timed out", object=e)
         except requests.RequestException as e:
-            self.logger.exception(f"General error: {str(e)}", e)
+            self.logger.exception(f"General error: {str(e)}", object=e)
         except Exception as e:
-            self.logger.exception(f"An unexpected error occurred: {str(e)}", e)
+            self.logger.exception(
+                f"An unexpected error occurred: {str(e)}", object=e)
 
         self.logger.end(f"End get group-profile-remote")
 
-
-
     def delete_group_profile(self, group_id: str, relationship_type_id: str):
         self.logger.start("Start delete group-profile-remote")
         try:
             url = self.url_circlez.endpoint_url(
-                brand_name = self.brand_name,
-                environment_name = self.env_name,
-                component = ComponentName.GROUP_PROFILE.value,
-                entity = EntityName.GROUP_PROFILE.value,
-                version = GROUP_PROFILE_API_VERSION,
-                action = ActionName.DELETE_GROUP_PROFILE.value, # "deleteGroupProfile",
+                brand_name=self.brand_name,
+                environment_name=self.env_name,
+                component_name=ComponentName.GROUP_PROFILE.value,
+                entity_name=EntityName.GROUP_PROFILE.value,
+                version=GROUP_PROFILE_API_VERSION,
+                action_name=ActionName.DELETE_GROUP_PROFILE.value,  # "deleteGroupProfile",
             )
 
-            self.logger.info("Endpoint group profile - deleteGroupProfile action: " + url)
+            self.logger.info(
+                "Endpoint group profile - deleteGroupProfile action: " + url)
 
             payload = {
                 'groupId': group_id,
                 'profileId': str(self.logger.userContext.get_real_profile_id()),
                 'relationshipTypeId': relationship_type_id
             }
 
             headers = {
                 'Content-Type': 'application/json',
-                'Authorization': f'Bearer {self.logger.userContext.get_jwt_token()}',
+                'Authorization': f'Bearer {self.logger.userContext.get_user_JWT()}',
             }
 
             response = requests.put(url, json=payload, headers=headers)
-            self.logger.end(f"End delete group-profile-remote, response: {str(response)}")
+            self.logger.end(
+                f"End delete group-profile-remote, response: {str(response)}")
             return response
-        
+
         except requests.ConnectionError as e:
-            self.logger.exception("Network problem (e.g. failed to connect)", e)
+            self.logger.exception(
+                "Network problem (e.g. failed to connect)", object=e)
         except requests.Timeout as e:
-            self.logger.exception("Request timed out", e)
+            self.logger.exception("Request timed out", object=e)
         except requests.RequestException as e:
-            self.logger.exception(f"General error: {str(e)}", e)
+            self.logger.exception(f"General error: {str(e)}", object=e)
         except Exception as e:
-            self.logger.exception(f"An unexpected error occurred: {str(e)}", e)
+            self.logger.exception(
+                f"An unexpected error occurred: {str(e)}", object=e)
 
         self.logger.end(f"End delete group-profile-remote")
-
```

### Comparing `group-profile-remote-0.0.8/pyproject.toml` & `group-profile-remote-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `group-profile-remote-0.0.8/setup.py` & `group-profile-remote-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix). Only lowercase, no underlines.
      name=PACKAGE_NAME,  
      # TODO: Please update the URL bellow
-     version='0.0.8', # https://pypi.org/project/group-profile-remote/
+     version='0.0.9', # https://pypi.org/project/group-profile-remote/
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles Group-Profile-Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common Group-Profile-Remote function used in different repositories",
      long_description_content_type="text/markdown",
```

