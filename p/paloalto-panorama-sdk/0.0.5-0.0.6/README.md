# Comparing `tmp/paloalto_panorama_sdk-0.0.5.tar.gz` & `tmp/paloalto_panorama_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paloalto_panorama_sdk-0.0.5.tar", last modified: Tue Apr 30 04:57:35 2024, max compression
+gzip compressed data, was "paloalto_panorama_sdk-0.0.6.tar", last modified: Fri May  3 06:33:16 2024, max compression
```

## Comparing `paloalto_panorama_sdk-0.0.5.tar` & `paloalto_panorama_sdk-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:57:35.964966 paloalto_panorama_sdk-0.0.5/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.5/LICENSE
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.5/MANIFEST.in
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-04-30 04:57:35.964691 paloalto_panorama_sdk-0.0.5/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)      809 2024-04-29 13:58:58.000000 paloalto_panorama_sdk-0.0.5/README.md
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:57:35.946417 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      110 2024-04-30 04:57:31.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/address_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/address_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/key_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:57:35.954989 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/panorama_data_kit/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:16:15.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/panorama_data_kit/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      553 2024-04-30 04:55:44.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1566 2024-04-30 04:11:21.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/panorama_sdk.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     3515 2024-04-29 05:08:50.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/post_rules_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/service_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/service_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:57:35.953608 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-04-30 04:57:35.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)      821 2024-04-30 04:57:35.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-04-30 04:57:35.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-04-30 04:57:35.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/requires.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-04-30 04:57:35.000000 paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/top_level.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-04-30 04:57:35.965037 paloalto_panorama_sdk-0.0.5/setup.cfg
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.5/setup.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:57:35.959944 paloalto_panorama_sdk-0.0.5/tests/
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:57:35.964285 paloalto_panorama_sdk-0.0.5/tests/PanoramaAPIMock/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.5/tests/PanoramaAPIMock/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.5/tests/PanoramaAPIMock/panoramaAPIMock.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.5/tests/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.5/tests/test_service.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.128786 paloalto_panorama_sdk-0.0.6/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.6/LICENSE
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.6/MANIFEST.in
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-03 06:33:16.128521 paloalto_panorama_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      809 2024-04-29 13:58:58.000000 paloalto_panorama_sdk-0.0.6/README.md
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.092019 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      184 2024-05-03 06:30:37.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/key_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.109558 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:16:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      735 2024-04-30 08:19:39.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      926 2024-05-03 05:32:44.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     2244 2024-05-03 05:30:44.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      751 2024-05-03 06:29:49.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/service_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      705 2024-05-03 06:23:45.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     2185 2024-05-03 06:25:49.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_sdk.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     3567 2024-04-30 11:56:00.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/security_post_rules_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.105023 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1070 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/requires.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/top_level.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-05-03 06:33:16.128876 paloalto_panorama_sdk-0.0.6/setup.cfg
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.6/setup.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.116272 paloalto_panorama_sdk-0.0.6/tests/
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.128034 paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/panoramaAPIMock.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.6/tests/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.6/tests/test_service.py
```

### Comparing `paloalto_panorama_sdk-0.0.5/LICENSE` & `paloalto_panorama_sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/PKG-INFO` & `paloalto_panorama_sdk-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloalto_panorama_sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: This SDK is designed to make it easier to work with the Palo Alto Panorama API.
 Author: Timo Riedinger
 Author-email: timo.riedinger@bechtle.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paloalto_panorama_sdk-0.0.5/README.md` & `paloalto_panorama_sdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/address_groups_manager.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/address_manager.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/key_manager.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/key_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from dataclasses import dataclass
-from typing import List, Dict
+import json
+from dataclasses import dataclass, asdict
+
 
 @dataclass
-class AddressGroup:
+class Address:
     location: str
     name: str
     description: str
-    static: 'StaticMembers'
+    ip_netmask: str
 
-    @dataclass
-    class StaticMembers:
-        member: List[str]
+    def to_json(self):
+        data_dict = asdict(self)
+        data_dict['@location'] = data_dict.pop('location')
+        data_dict['@name'] = data_dict.pop('name')
+        data_dict['ip-netmask'] = data_dict.pop('ip_netmask')
+        return json.dumps(data_dict, ensure_ascii=False)
 
     @classmethod
-    def from_json(cls, json_data: Dict):
-        location = json_data.get('@location')
+    def from_json(cls, json_data):
+        location = json_data['@location']
         name = json_data.get('@name')
-        description = json_data.get('description')
-        static = json_data.get('static', {}).get('member')
-        return cls(location, name, description, static)
+        description = json_data.get('@description')
+        ip_netmask = json_data.get('ip-netmask')
+        return cls(location, name, description, ip_netmask)
```

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/panorama_sdk.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_sdk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import os
+from pprint import pprint
+
 from paloalto_panorama_sdk.address_groups_manager import AddressGroupsManager
 from paloalto_panorama_sdk.address_manager import AddressManager
 from paloalto_panorama_sdk.key_manager import KeyManager
-from paloalto_panorama_sdk.post_rules_manager import PostRulesManager
+from paloalto_panorama_sdk.panorama_data_kit.adress_data import Address
+from paloalto_panorama_sdk.panorama_data_kit.adress_group_data import AddressGroup
+from paloalto_panorama_sdk.panorama_data_kit.security_post_rule_data import SecurityPostRule
+from paloalto_panorama_sdk.panorama_data_kit.service_data import Service
+from paloalto_panorama_sdk.panorama_data_kit.service_group_data import ServiceGroup
+from paloalto_panorama_sdk.security_post_rules_manager import SecurityPostRulesManager
 from paloalto_panorama_sdk.service_groups_manager import ServiceGroupsManager
 from paloalto_panorama_sdk.service_manager import ServiceManager
 from dotenv import load_dotenv
 
 load_dotenv()
 
 
@@ -17,21 +24,26 @@
         self.password = password
         self.apikey = KeyManager.get_api_key(
             panorama_url=self.url,
             user=self.username,
             password=self.password,
             verify=verify
         )
-        self.address_groups = AddressGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
+        self.address_group = AddressGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
         self.address = AddressManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
-        self.security_post_rules = PostRulesManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
-        self.service_groups = ServiceGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
+        self.security_post_rule = SecurityPostRulesManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
+        self.service_group = ServiceGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
         self.service = ServiceManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
 
 
 if __name__ == '__main__':
     panSDK = PanoramaSDK(
         url=os.getenv("url", ""),
         username=os.getenv("user", "test"),
-        password=os.getenv("password", "testpass")
+        password=os.getenv("password", "testpass"),
+        verify=False
     )
-    print(panSDK.apikey)
+    serOutput = panSDK.service.list_services()
+    se = Service.from_json(serOutput['result']['entry'][0])
+    pprint(serOutput)
+    print(se)
+    pprint(se.to_json())
```

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/post_rules_manager.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/security_post_rules_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import requests
 
 
-class PostRulesManager:
+class SecurityPostRulesManager:
     def __init__(self, panorama_url, api_key, verify=True):
         self.panorama_url = panorama_url
         self.api_key = api_key
         self.verify = verify
         self.url = f"{self.panorama_url}/restapi/v10.2/Policies/SecurityPostRules"
         self.headers = {'Content-Type': 'application/json',
                         'X-PAN-KEY': f"{self.api_key}"}
 
-    def list_post_rules(self):
-        params = {'location': 'shared', 'device-group': 'TestGroup'}
+    def list_post_rules(self, location='shared', devicegroup='TestGroup'):
+        params = {'location': location, 'device-group': devicegroup}
         response = requests.get(url=self.url, headers=self.headers, params=params, verify=self.verify)
         post_rules = json.loads(response.content.decode('utf-8'))
         return post_rules
 
     def create_post_rules(self, device_group, name, action, description, from_zone, source_group,
                           to_zone, destination_group, service, profile_type, profile):
         location = "shared" if device_group == 'shared' else "device-group"
```

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/service_groups_manager.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk/service_manager.py` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/PKG-INFO` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloalto-panorama-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: This SDK is designed to make it easier to work with the Palo Alto Panorama API.
 Author: Timo Riedinger
 Author-email: timo.riedinger@bechtle.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/SOURCES.txt` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 README.md
 setup.py
 paloalto_panorama_sdk/__init__.py
 paloalto_panorama_sdk/address_groups_manager.py
 paloalto_panorama_sdk/address_manager.py
 paloalto_panorama_sdk/key_manager.py
 paloalto_panorama_sdk/panorama_sdk.py
-paloalto_panorama_sdk/post_rules_manager.py
+paloalto_panorama_sdk/security_post_rules_manager.py
 paloalto_panorama_sdk/service_groups_manager.py
 paloalto_panorama_sdk/service_manager.py
 paloalto_panorama_sdk.egg-info/PKG-INFO
 paloalto_panorama_sdk.egg-info/SOURCES.txt
 paloalto_panorama_sdk.egg-info/dependency_links.txt
 paloalto_panorama_sdk.egg-info/requires.txt
 paloalto_panorama_sdk.egg-info/top_level.txt
 paloalto_panorama_sdk/panorama_data_kit/__init__.py
+paloalto_panorama_sdk/panorama_data_kit/adress_data.py
 paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py
+paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
+paloalto_panorama_sdk/panorama_data_kit/service_data.py
+paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
 tests/__init__.py
 tests/test_service.py
 tests/PanoramaAPIMock/__init__.py
 tests/PanoramaAPIMock/panoramaAPIMock.py
```

### Comparing `paloalto_panorama_sdk-0.0.5/paloalto_panorama_sdk.egg-info/requires.txt` & `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/setup.py` & `paloalto_panorama_sdk-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/tests/PanoramaAPIMock/panoramaAPIMock.py` & `paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/panoramaAPIMock.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.5/tests/test_service.py` & `paloalto_panorama_sdk-0.0.6/tests/test_service.py`

 * *Files identical despite different names*

