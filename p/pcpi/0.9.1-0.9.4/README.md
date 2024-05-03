# Comparing `tmp/pcpi-0.9.1.tar.gz` & `tmp/pcpi-0.9.4.tar.gz`

## Comparing `pcpi-0.9.1.tar` & `pcpi-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pcpi-0.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pcpi-0.9.1/SUPPORT.md
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 pcpi-0.9.1/examples.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pcpi-0.9.1/min_requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pcpi-0.9.1/requirements.txt
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pcpi-0.9.1/run_tests.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pcpi-0.9.1/ssl_gen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/__init__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/_cspm_session.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/_onprem_cwp_session.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/_saas_cwp_session.py
--rw-r--r--   0        0        0    24048 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/_session_base.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/_session_types.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/onprem_session_manager.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/saas_session_manager.py
--rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 pcpi-0.9.1/src/pcpi/session_loader.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcpi-0.9.1/.gitignore
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pcpi-0.9.1/LICENSE
--rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 pcpi-0.9.1/README.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pcpi-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    19983 2020-02-02 00:00:00.000000 pcpi-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pcpi-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pcpi-0.9.4/SUPPORT.md
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 pcpi-0.9.4/examples.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pcpi-0.9.4/min_requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pcpi-0.9.4/requirements.txt
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pcpi-0.9.4/run_tests.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pcpi-0.9.4/ssl_gen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/_cna_session.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/_cspm_session.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/_onprem_cwp_session.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/_saas_cwp_session.py
+-rw-r--r--   0        0        0    24048 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/_session_base.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/_session_types.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/onprem_session_manager.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/saas_session_manager.py
+-rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 pcpi-0.9.4/src/pcpi/session_loader.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcpi-0.9.4/.gitignore
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pcpi-0.9.4/LICENSE
+-rw-r--r--   0        0        0    18396 2020-02-02 00:00:00.000000 pcpi-0.9.4/README.md
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pcpi-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    19993 2020-02-02 00:00:00.000000 pcpi-0.9.4/PKG-INFO
```

### Comparing `pcpi-0.9.1/CONTRIBUTING.md` & `pcpi-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/SUPPORT.md` & `pcpi-0.9.4/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/examples.py` & `pcpi-0.9.4/examples.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/run_tests.py` & `pcpi-0.9.4/run_tests.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/ssl_gen.py` & `pcpi-0.9.4/ssl_gen.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/src/pcpi/_cspm_session.py` & `pcpi-0.9.4/src/pcpi/_cspm_session.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/src/pcpi/_onprem_cwp_session.py` & `pcpi-0.9.4/src/pcpi/_onprem_cwp_session.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/src/pcpi/_saas_cwp_session.py` & `pcpi-0.9.4/src/pcpi/_saas_cwp_session.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/src/pcpi/_session_base.py` & `pcpi-0.9.4/src/pcpi/_session_base.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/src/pcpi/onprem_session_manager.py` & `pcpi-0.9.4/src/pcpi/onprem_session_manager.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/src/pcpi/saas_session_manager.py` & `pcpi-0.9.4/src/pcpi/saas_session_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 logging.basicConfig()
 py_logger = logging.getLogger("pcpi")
 py_logger.setLevel(10)
 
 #Local
-from ._session_types import CSPMSession, SaaSCWPSession
+from ._session_types import CSPMSession, SaaSCWPSession, CNASession
 
 class SaaSSessionManager:
     def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify=True, proxies:dict=None, logger=py_logger):
         """
         Initializes a Prisma Cloud API Session Manager.
 
         Keyword Arguments:
@@ -28,14 +28,15 @@
         self.api_url = api_url
 
         self.verify = verify
         self.proxies = proxies
 
         self.cspm_session = {}
         self.saas_cwp_session = {}
+        self.cna_session = {}
         
 
 
 #==============================================================================
     def create_cspm_session(self):
         session = CSPMSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger)
         self.cspm_session = session
@@ -47,10 +48,22 @@
             self.saas_cwp_session = session
             return session
         else:
             self.create_cspm_session()
             session = SaaSCWPSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger, cspm_session=self.cspm_session)
             self.saas_cwp_session = session
             return session
+        
+    def create_cna_session(self):
+        if self.cspm_session:
+            session = CNASession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger, cspm_session=self.cspm_session)
+            self.cna_session = session
+            return session
+        else:
+            self.create_cspm_session()
+            session = CNASession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger, cspm_session=self.cspm_session)
+            self.cna_session = session
+            return session
+
 
 
 #==============================================================================
```

### Comparing `pcpi-0.9.1/src/pcpi/session_loader.py` & `pcpi-0.9.4/src/pcpi/session_loader.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/.gitignore` & `pcpi-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/LICENSE` & `pcpi-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pcpi-0.9.1/README.md` & `pcpi-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,16 @@
 
 ## Session Managers
 
 If you want to take control on how credentials are stored/loaded into your scripts, use the session managers directly and skip the session loader module. Session manager objects directly accept Prisma Cloud credentials into the object constructor. 
 
 This still creates the same Prisma Cloud session object that you use for API requests.
 
+The logger object is optional. You can use PyLogger or Loguru with PCPI
+
 **EXAMPLES**
 
 ```python
 from pcpi import saas_session_manager
 import logging
 
 py_logger = logging.getLogger()
@@ -282,26 +284,23 @@
 )
 
 cspm_session = session_manager.create_cspm_session()
 cwp_session = session_manager.create_cwp_session()
 ```
 
 ```python
-from pcpi import session_manager
+from pcpi import onprem_session_manager
 import logging
 
-py_logger = logging.getLogger()
-py_logger.setLevel(10)
 
-session_manager = session_manager.CWPSessionManager(
+session_manager = onprem_session_manager.CWPSessionManager(
     tenant_name='My PC Tenant',
     uname='xxxxxxxxxxxxxxxxxxxxxxxxxx',
     passwd='xxxxxxxxxxxxxxxxxxxxxxxxxx',
-    api_url='https://<yourselfhostedurl>',
-    logger=py_logger
+    api_url='https://<yourselfhostedurl>'
 )
 
 onprem_cwp_session = session_manager.create_cwp_session()
 ```
 
 ## Requests
```

### Comparing `pcpi-0.9.1/pyproject.toml` & `pcpi-0.9.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcpi"
-version = "0.9.1"
+version = "0.9.4"
 authors = [
   { name="Adam Hamilton-Sutherland", email="ahamiltonsut@paloaltonetworks.com" },
 ]
 description = "Python Package for making API calls to the Prisma Cloud API using best practices."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -21,8 +21,8 @@
     "License :: OSI Approved :: ISC License (ISCL)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/PaloAltoNetworks/pc-python-integration"
-"Bug Tracker" = "https://github.com/PaloAltoNetworks/pc-python-integration/issues"
+"Bug Tracker" = "https://github.com/PaloAltoNetworks/pc-python-integration/issues"
```

### Comparing `pcpi-0.9.1/PKG-INFO` & `pcpi-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pcpi
-Version: 0.9.1
+Version: 0.9.4
 Summary: Python Package for making API calls to the Prisma Cloud API using best practices.
 Project-URL: Homepage, https://github.com/PaloAltoNetworks/pc-python-integration
 Project-URL: Bug Tracker, https://github.com/PaloAltoNetworks/pc-python-integration/issues
 Author-email: Adam Hamilton-Sutherland <ahamiltonsut@paloaltonetworks.com>
 License: ISC License
         
         Copyright (c) 2020, Palo Alto Networks Inc.
@@ -292,14 +292,16 @@
 
 ## Session Managers
 
 If you want to take control on how credentials are stored/loaded into your scripts, use the session managers directly and skip the session loader module. Session manager objects directly accept Prisma Cloud credentials into the object constructor. 
 
 This still creates the same Prisma Cloud session object that you use for API requests.
 
+The logger object is optional. You can use PyLogger or Loguru with PCPI
+
 **EXAMPLES**
 
 ```python
 from pcpi import saas_session_manager
 import logging
 
 py_logger = logging.getLogger()
@@ -314,26 +316,23 @@
 )
 
 cspm_session = session_manager.create_cspm_session()
 cwp_session = session_manager.create_cwp_session()
 ```
 
 ```python
-from pcpi import session_manager
+from pcpi import onprem_session_manager
 import logging
 
-py_logger = logging.getLogger()
-py_logger.setLevel(10)
 
-session_manager = session_manager.CWPSessionManager(
+session_manager = onprem_session_manager.CWPSessionManager(
     tenant_name='My PC Tenant',
     uname='xxxxxxxxxxxxxxxxxxxxxxxxxx',
     passwd='xxxxxxxxxxxxxxxxxxxxxxxxxx',
-    api_url='https://<yourselfhostedurl>',
-    logger=py_logger
+    api_url='https://<yourselfhostedurl>'
 )
 
 onprem_cwp_session = session_manager.create_cwp_session()
 ```
 
 ## Requests
```

