# Comparing `tmp/redfish_protocol_validator-1.2.4.tar.gz` & `tmp/redfish_protocol_validator-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_protocol_validator-1.2.4.tar", last modified: Fri Apr 19 19:59:59 2024, max compression
+gzip compressed data, was "redfish_protocol_validator-1.2.5.tar", last modified: Fri May  3 20:41:08 2024, max compression
```

## Comparing `redfish_protocol_validator-1.2.4.tar` & `redfish_protocol_validator-1.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/redfish_protocol_validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/protocol_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/redfish_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    20487 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    52407 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/security_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    45918 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    64194 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/system_under_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:41:08.640838 redfish_protocol_validator-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-03 20:41:08.640838 redfish_protocol_validator-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:41:08.636838 redfish_protocol_validator-1.2.5/redfish_protocol_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16251 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26425 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/protocol_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/redfish_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20259 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51617 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/security_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43149 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/service_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58988 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29628 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/service_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18153 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/system_under_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15306 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:41:08.640838 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-03 20:41:08.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-03 20:41:08.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:41:08.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 20:41:08.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 20:41:08.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 20:41:08.000000 redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:41:08.640838 redfish_protocol_validator-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-03 20:40:59.000000 redfish_protocol_validator-1.2.5/setup.py
```

### Comparing `redfish_protocol_validator-1.2.4/LICENSE.md` & `redfish_protocol_validator-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.4/PKG-INFO` & `redfish_protocol_validator-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_protocol_validator
-Version: 1.2.4
+Version: 1.2.5
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.2.4/README.md` & `redfish_protocol_validator-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/accounts.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,56 +16,56 @@
 
 
 def get_user_names(sut: SystemUnderTest, session,
                    request_type=RequestType.NORMAL):
     users = set()
     response = sut.get_response('GET', sut.accounts_uri)
     if response.status_code == requests.codes.OK:
-        data = response.json()
+        data = utils.get_response_json(response)
         uris = [m.get('@odata.id') for m in data.get('Members', []) if
                 m.get('@odata.id')]
         responses = sut.get_responses_by_method(
             'GET', resource_type=ResourceType.MANAGER_ACCOUNT)
         for uri in uris:
             if uri in responses:
                 response = responses[uri]
             else:
                 response = session.get(sut.rhost + uri)
                 sut.add_response(uri, response,
                                  resource_type=ResourceType.MANAGER_ACCOUNT,
                                  request_type=request_type)
             if response.status_code == requests.codes.OK:
-                data = response.json()
+                data = utils.get_response_json(response)
                 user = data.get('UserName')
                 if user:
                     users.add(user)
     logging.debug('Account usernames: %s' % users)
     return users
 
 
 def get_available_roles(sut: SystemUnderTest, session,
                         request_type=RequestType.NORMAL):
     roles = set()
     response = sut.get_response('GET', sut.roles_uri)
     if response.status_code == requests.codes.OK:
-        data = response.json()
+        data = utils.get_response_json(response)
         uris = [m.get('@odata.id') for m in data.get('Members', []) if
                 m.get('@odata.id')]
         responses = sut.get_responses_by_method(
             'GET', resource_type=ResourceType.ROLE)
         for uri in uris:
             if uri in responses:
                 response = responses[uri]
             else:
                 response = session.get(sut.rhost + uri)
                 sut.add_response(uri, response,
                                  resource_type=ResourceType.ROLE,
                                  request_type=request_type)
             if response.status_code == requests.codes.OK:
-                data = response.json()
+                data = utils.get_response_json(response)
                 role = data.get('Id')
                 if role:
                     roles.add(role)
     logging.debug('Available roles: %s' % roles)
     return roles
 
 
@@ -92,15 +92,15 @@
 def new_password(sut: SystemUnderTest, length=16, upper=1, lower=1,
                  digits=1, symbols=1):
     # Get the min and max password length and override 'length' if needed
     # Use either limit if one is specified
     response = sut.get_response('GET', sut.account_service_uri)
     try:
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             if 'MinPasswordLength' in data and length < data['MinPasswordLength']:
                 length = data['MinPasswordLength']
             elif 'MaxPasswordLength' in data and length > data['MaxPasswordLength']:
                 length = data['MaxPasswordLength']
     except:
         pass
 
@@ -116,15 +116,15 @@
     sut.add_priv_info(pwd)
     return pwd
 
 
 def find_empty_account_slot(sut: SystemUnderTest, session,
                             request_type=RequestType.NORMAL):
     response = sut.get_response('GET', sut.accounts_uri)
-    data = response.json()
+    data = utils.get_response_json(response)
     uris = [m.get('@odata.id') for m in data.get('Members', []) if
             m.get('@odata.id')]
     responses = sut.get_responses_by_method(
         'GET', resource_type=ResourceType.MANAGER_ACCOUNT)
     if uris:
         # first slot may be reserved, so move to end of list
         uris += [uris.pop(0)]
@@ -133,15 +133,15 @@
             response = responses[uri]
         else:
             response = session.get(sut.rhost + uri)
             sut.add_response(uri, response,
                              resource_type=ResourceType.MANAGER_ACCOUNT,
                              request_type=request_type)
         if response.status_code == requests.codes.OK:
-            data = response.json()
+            data = utils.get_response_json(response)
             if data.get('UserName') == '' and not data.get('Enabled', True):
                 return uri
     return None
 
 
 def add_account_via_patch(sut: SystemUnderTest, session, user, role, password,
                           request_type=RequestType.NORMAL):
@@ -158,15 +158,15 @@
     sut.add_response(uri, response, resource_type=ResourceType.MANAGER_ACCOUNT,
                      request_type=request_type)
     success = response.status_code == requests.codes.OK
     if success:
         response = session.get(sut.rhost + uri)
         if response.ok:
             # Enable the account if it not already enabled
-            data = response.json()
+            data = utils.get_response_json(response)
             if 'Enabled' in data and data['Enabled'] is False:
                 headers = utils.get_etag_header(sut, session, uri)
                 payload = {'Enabled': True}
                 sut.patch(uri, json=payload, headers=headers, session=session)
         sut.add_response(uri, response,
                          resource_type=ResourceType.MANAGER_ACCOUNT,
                          request_type=request_type)
@@ -204,15 +204,15 @@
     new_acct_uri = None
     success = response.status_code == requests.codes.CREATED
     if success:
         location = response.headers.get('Location')
         if location:
             new_acct_uri = urlparse(location).path
         else:
-            new_acct_uri = response.json().get('@odata.id')
+            new_acct_uri = utils.get_response_json(response).get('@odata.id')
         response = session.get(sut.rhost + new_acct_uri)
         sut.add_response(new_acct_uri, response,
                          resource_type=ResourceType.MANAGER_ACCOUNT,
                          request_type=request_type)
     elif (response.status_code == requests.codes.METHOD_NOT_ALLOWED
           or 'POST' not in methods):
         return add_account_via_patch(sut, session, user, role, password,
@@ -282,15 +282,15 @@
     return new_pwd
 
 
 def delete_account_via_patch(sut: SystemUnderTest, session, user, acct_uri,
                              request_type=RequestType.NORMAL):
     response = sut.get_response('GET', acct_uri)
     if response.status_code == requests.codes.OK:
-        data = response.json()
+        data = utils.get_response_json(response)
         if data and data.get('UserName') == user:
             payload = {'UserName': ''}
             if data.get('Enabled', False):
                 payload['Enabled'] = False
             headers = utils.get_etag_header(sut, session, acct_uri)
             response = sut.patch(acct_uri, json=payload, headers=headers,
                                  session=session)
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/console_scripts.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/console_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from redfish_protocol_validator import service_requests
 from redfish_protocol_validator import service_responses
 from redfish_protocol_validator import sessions
 from redfish_protocol_validator import utils
 from redfish_protocol_validator.constants import Result
 from redfish_protocol_validator.system_under_test import SystemUnderTest
 
-tool_version = '1.2.4'
+tool_version = '1.2.5'
 
 
 def perform_tests(sut: SystemUnderTest):
     """Perform the protocol validation tests on the resources."""
     protocol_details.test_protocol_details(sut)
     service_requests.test_service_requests(sut)
     service_responses.test_service_responses(sut)
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/constants.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,601 +38,371 @@
     BAD_ETAG = auto()
     MODIFY_OTHER = auto()
     SUBSCRIPTION = auto()
     STREAMING = auto()
     YAML = auto()
     PATCH_MIXED_PROPS = auto()
     PATCH_BAD_PROP = auto()
-    PATCH_RO_RESOURCE = auto()
-    PATCH_COLLECTION = auto()
     PATCH_ODATA_PROPS = auto()
     UNSUPPORTED_REQ = auto()
 
 
 class Assertion(NoValue):
-    # Protocol details assertions (prefix of "PROTO_")
+    # Last sync: 1.20.0
+    # See the wiki for 'shall' statements that are not tested
+
+    # Note: Strings follow the format 'CLAUSE: STATEMENT', where 'CLAUSE' is the section heading and 'STATEMENT' is the
+    # 'shall' statement from the specification.  Copy the 'shall' language as best as possible.  Modify when the
+    # statement is awkward as a standalone sentence in a report.  For example, 'If the Required column contains Yes,
+    # a Redfish interface shall support the HTTP method' doesn't tell the user much information about a test failure.
+
+    # 'Protocol details' assertions (prefix of "PROTO_")
     PROTO_URI_SAFE_CHARS = (
-        'URIs shall not include any RFC1738-defined unsafe characters.')
+        'Universal Resource Identifiers: URIs shall not include any RFC1738-defined unsafe characters.')
     PROTO_URI_NO_ENCODED_CHARS = (
-        'URIs shall not include any percent-encoding of characters.')
+        'Universal Resource Identifiers: URIs shall not include any percent-encoding of characters.')
     PROTO_HTTP_SUPPORTED_METHODS = (
-        'HTTP methods POST, GET, PATCH, and DELETE shall be supported.')
+        'HTTP methods: Services shall support the POST, GET, PATCH, and DELETE HTTP methods.')
     PROTO_HTTP_UNSUPPORTED_METHODS = (
-        'For HTTP methods that the Redfish service does not support or that '
-        'the following table omits, the Redfish service shall return the HTTP '
-        '405 Method Not Allowed status code or the HTTP 501 Not Implemented '
-        'status code.')
+        'HTTP methods: Services shall return the HTTP 405 Method Not Allowed status code or the HTTP 501 Not '
+        'Implemented status code for unsupported and undocumented methods.')
+    PROTO_REDIRECT_ENFORCES_TARGET_PRIVS = (
+        'HTTP redirect: The service for the redirected resource shall enforce the authentication and authorization '
+        'requirements for the redirected resource.')
     PROTO_JSON_ALL_RESOURCES = (
-        'All resources shall be available through the JSON application/json '
-        'media type.')
+        'Media types: All resources shall be available through the JSON application/json media type.')
     PROTO_JSON_RFC = (
-        'Redfish Services shall make every resource available in a JSON-based '
-        'representation, as specified in RFC4627')
+        'Media types: Services shall make every resource available in a JSON-based representation as a JSON object.')
     PROTO_JSON_ACCEPTED = (
-        'Receivers shall not reject a JSON-encoded message, and shall offer '
-        'at least one JSON-based response representation.')
+        'Media types: Receivers shall not reject a JSON-encoded message, and shall offer at least one JSON-based '
+        'response representation.')
     PROTO_ETAG_ON_GET_ACCOUNT = (
-        'Implementations shall support the return of ETag headers for GET '
-        'requests of ManagerAccount resources.')
+        'ETags: Implementations shall support the return of ETag headers for GET requests of ManagerAccount resources.')
     PROTO_ETAG_RFC7232 = (
-        'If a resource supports an ETag, it shall use the RFC7232-defined '
-        'ETag.')
+        'ETags: If a resource supports an ETag, it shall use the RFC7232-defined ETag.')
     PROTO_STD_URI_SERVICE_ROOT = (
-        'The root URI for this version of the Redfish protocol shall be '
-        '/redfish/v1/.')
+        'Protocol version: The root URI for this version of the Redfish protocol shall be /redfish/v1/.')
     PROTO_STD_URI_VERSION = (
-        'A GET operation on the /redfish resource shall return this response '
-        'body: {"v1": "/redfish/v1/"}')
+        'Protocol version: A GET operation on the /redfish resource shall return {"v1": "/redfish/v1/"}')
     PROTO_STD_URIS_SUPPORTED = (
-        'A Redfish Service shall support these Redfish-defined URIs: '
-        '/redfish, /redfish/v1/, /redfish/v1/odata, /redfish/v1/$metadata')
+        'Redfish-defined URIs and relative reference rules: Services shall support the /redfish, /redfish/v1/, '
+        '/redfish/v1/odata, and /redfish/v1/$metadata URIs.')
     PROTO_STD_URI_SERVICE_ROOT_REDIRECT = (
-        'The service shall process the [/redfish/v1] URI without a trailing '
-        'slash in one of these ways: Redirect it to the associated '
-        'Redfish-defined URI, or treat it as the equivalent URI to the '
-        'associated Redfish-defined URI (/redfish/v1/).')
+        'Redfish-defined URIs and relative reference rules: Services shall process /redfish/v1 by redirecting it to '
+        '/redfish/v1/ or treating it as equivalent to /redfish/v1/')
     PROTO_URI_RELATIVE_REFS = (
-        'All relative references (see RFC3986) that the service uses shall '
-        'start with either: A double forward slash (//) and include the '
-        'authority (network-path), such as '
-        '//mgmt.vendor.com/redfish/v1/Systems, or a single forward slash (/) '
-        'and include the absolute-path, such as /redfish/v1/Systems.')
-    # Service requests assertions (prefix of "REQ_")
+        'Redfish-defined URIs and relative reference rules: All relative references shall start with either a double '
+        'forward slash (//) with the authority (network-path) or a single forward slash (/) and include the '
+        'absolute-path.')
+
+    # 'Service requests' assertions (prefix of "REQ_")
     REQ_HEADERS_ACCEPT = (
-        'Redfish Services shall process the [Accept header] in the following '
-        'table as defined by the HTTP 1.1 specification if the value in the '
-        'Service Requirement column is set to "Yes", or if the value is '
-        '"Conditional" under the conditions noted in the Description column.'
-    )
+        'Request headers: Services shall process the Accept header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_AUTHORIZATION = (
-        'Redfish Services shall process the [Authorization header] in the '
-        'following table as defined by the HTTP 1.1 specification if the '
-        'value in the Service Requirement column is set to "Yes", or if the '
-        'value is "Conditional" under the conditions noted in the Description '
-        'column.'
-    )
+        'Request headers: Services shall process the Authorization header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_CONTENT_TYPE = (
-        'Redfish Services shall process the [Content-Type header] in the '
-        'following table as defined by the HTTP 1.1 specification if the '
-        'value in the Service Requirement column is set to "Yes", or if the '
-        'value is "Conditional" under the conditions noted in the Description '
-        'column.'
-    )
+        'Request headers: Services shall process the Content-Type header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_HOST = (
-        'Redfish Services shall process the [Host header] in the following '
-        'table as defined by the HTTP 1.1 specification if the value in the '
-        'Service Requirement column is set to "Yes", or if the value is '
-        '"Conditional" under the conditions noted in the Description column.'
-    )
+        'Request headers: Services shall process the Host header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_IF_MATCH = (
-        'Redfish Services shall process the [If-Match header] in the '
-        'following table as defined by the HTTP 1.1 specification if the '
-        'value in the Service Requirement column is set to "Yes", or if the '
-        'value is "Conditional" under the conditions noted in the Description '
-        'column.'
-    )
+        'Request headers: Services shall process the If-Match header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_ODATA_VERSION = (
-        'Redfish Services shall process the [OData-Version header] in the '
-        'following table as defined by the HTTP 1.1 specification if the '
-        'value in the Service Requirement column is set to "Yes", or if the '
-        'value is "Conditional" under the conditions noted in the Description '
-        'column.'
-    )
+        'Request headers: Services shall process the OData-Version header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_ORIGIN = (
-        'Redfish Services shall process the [Origin header] in the following '
-        'table as defined by the HTTP 1.1 specification if the value in the '
-        'Service Requirement column is set to "Yes", or if the value is '
-        '"Conditional" under the conditions noted in the Description column.'
-    )
+        'Request headers: Services shall process the Origin header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_USER_AGENT = (
-        'Redfish Services shall process the [User-Agent header] in the '
-        'following table as defined by the HTTP 1.1 specification if the '
-        'value in the Service Requirement column is set to "Yes", or if the '
-        'value is "Conditional" under the conditions noted in the Description '
-        'column.'
-    )
+        'Request headers: Services shall process the User-Agent header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_HEADERS_X_AUTH_TOKEN = (
-        'Redfish Services shall process the [X-Auth-Token header] in the '
-        'following table as defined by the HTTP 1.1 specification if the '
-        'value in the Service Requirement column is set to "Yes", or if the '
-        'value is "Conditional" under the conditions noted in the Description '
-        'column.'
-    )
+        'Request headers: Services shall process the X-Auth-Token header with the behaviors defined in the Redfish '
+        'Specification and HTTP 1.1 Specification.')
     REQ_GET_NO_ACCEPT_HEADER = (
-        'If the Accept header is absent, the service shall return the '
-        'resource\'s representation as application/json.'
-    )
+        'GET (read requests) overview: If the Accept header is absent, the service shall return the resource\'s '
+        'representation as application/json.')
     REQ_GET_IGNORE_BODY = (
-        'The service shall ignore the content of the body on a GET.'
-    )
+        'GET (read requests) overview: Services shall ignore the content of the body on a GET.')
     REQ_GET_COLLECTION_COUNT_PROP_REQUIRED = (
-        'Retrieved resource collections shall always include the count '
-        'property to specify the total number of entries in its Members array.'
-    )
+        'Resource collection requests: Retrieved resource collections shall always include the Members@odata.count '
+        'property to specify the total number of entries in its Members array.')
     REQ_GET_COLLECTION_COUNT_PROP_TOTAL = (
-        'Regardless of the next link property or paging, the count property '
-        'shall return the total number of resources that the Members array '
-        'references.'
-    )
+        'Resource collection requests: Regardless of the Members@odata.nextLink property or paging, the '
+        'Members@odata.count property shall return the total number of resources that the Members array references.')
     REQ_GET_SERVICE_ROOT_URL = (
-        'The root URL for Redfish version 1.x services shall be /redfish/v1/.'
-    )
+        'Service root request: The root URL for Redfish version 1.x services shall be /redfish/v1/.')
     REQ_GET_SERVICE_ROOT_NO_AUTH = (
-        'Services shall not require authentication to retrieve the Service '
-        'Root and /redfish resources.'
-    )
+        'Service root request: Services shall not require authentication to retrieve the service root and /redfish '
+        'resources.')
     REQ_GET_METADATA_URI = (
-        'Service shall expose an OData metadata document at the '
-        '/redfish/v1/$metadata URI.'
-    )
+        'OData service and metadata document requests: Services shall expose an OData metadata document at the '
+        '/redfish/v1/$metadata URI.')
     REQ_GET_ODATA_URI = (
-        'Service shall expose an OData service document at the '
-        '/redfish/v1/odata URI.'
-    )
+        'OData service and metadata document requests: Services shall expose an OData service document at the '
+        '/redfish/v1/odata URI')
     REQ_GET_METADATA_ODATA_NO_AUTH = (
-        'Service shall not require authentication to retrieve the OData '
-        'metadata document or the OData service document.'
-    )
+        'OData service and metadata document requests: Services shall not require authentication to retrieve the OData '
+        'metadata document or the OData service document.')
     REQ_QUERY_PROTOCOL_FEATURES_SUPPORTED = (
-        'Services shall include the ProtocolFeaturesSupported object in the '
-        'Service Root, if the service supports query parameters.'
-    )
+        'Query parameter overview: Services shall include the ProtocolFeaturesSupported object in the service root, if '
+        'the service support query parameters.')
     REQ_QUERY_IGNORE_UNSUPPORTED = (
-        'Services shall ignore unknown or unsupported query parameters that '
-        'do not begin with $.'
-    )
+        'Query parameter overview: Services shall ignore unknown or unsupported query parameters that do not begin '
+        'with $.')
     REQ_QUERY_UNSUPPORTED_DOLLAR_PARAMS = (
-        'Services shall return the HTTP 501 Not Implemented status code for '
-        'any unsupported query parameters that start with $.'
-    )
+        'Query parameter overview: Services shall return the HTTP 501 Not Implemented status code for any unsupported '
+        'query parameters that start with $.')
     REQ_QUERY_UNSUPPORTED_PARAMS_EXT_ERROR = (
-        'Services shall return an extended error that indicates the '
-        'unsupported query parameters for this resource.'
-    )
+        'Query parameter overview: Services shall return an extended error that indicates the unsupported query '
+        'parameters for this resource.')
     REQ_QUERY_INVALID_VALUES = (
-        'Services shall return the HTTP 400 Bad Request status code for any '
-        'query parameters that contain values that are invalid, or values '
-        'applied to query parameters without defined values, such as excerpt '
-        'or only.'
-    )
+        'Query parameter overview: Services shall return the HTTP 400 Bad Request status code for any query '
+        'parameters that contain values that are invalid, or values applied to query parameters without defined '
+        'values, such as excerpt or only.')
     REQ_HEAD_DIFFERS_FROM_GET = (
-        'The HEAD method differs from the GET method in that it shall not '
-        'return message body information.'
-    )
+        'HEAD: The HEAD method differs from the GET method in that it shall not return message body information.')
+    REQ_DATA_MOD_NOT_SUPPORTED = (
+        'Modification error responses: If the resource exists but does not support the requested operation, services '
+        'shall return the HTTP 405 Method Not Allowed status code.')
     REQ_DATA_MOD_ERRORS = (
-        'Otherwise, if the service returns a client 4XX or service 5XX status '
-        'code, the service encountered an error and the resource shall not '
-        'have been modified or created as a result of the operation.'
-    )
+        'Modification error responses: If the service returns a client 4XX or service 5XX status code, the service '
+        'encountered an error and the resource shall not have been modified or created as a result of the operation.')
     REQ_PATCH_MIXED_PROPS = (
-        'A partial success of a PATCH operation occurs when a modification '
-        'request for multiple properties results in at least one property '
-        'updated successfully, but one or more properties could not be '
-        'updated. In these cases, the service shall return the HTTP 200 OK '
-        'status code and a resource representation with extended information '
-        'that lists the properties that could not be updated.  The '
-        'implementation may reject the update on certain properties based on '
-        'its own policies and, in this case, not make the requested update.'
-    )
+        'PATCH (update): In cases where at least one property updated successfully, but one or more properties could '
+        'not be updated, the service shall return the HTTP 200 OK status code and a resource representation with '
+        'extended information that lists the properties that could not be updated.')
     REQ_PATCH_BAD_PROP = (
-        'If all properties in the update request are read-only, unknown, or '
-        'unsupported, but the resource can be updated, the service shall '
-        'return the HTTP 400 Bad Request status code and an error response '
-        'with messages that show the non-updatable properties.'
-    )
-    REQ_PATCH_RO_RESOURCE = (
-        'Modify a resource or all properties that can never be updated: '
-        'Services shall return the HTTP 405 status code.'
-    )
-    REQ_PATCH_COLLECTION = (
-        'A client PATCH request against a resource collection: Services shall '
-        'return the HTTP 405 status code.'
-    )
+        'PATCH (update): If all properties in the update request are read-only, unknown, or unsupported, but the '
+        'resource can be updated, the service shall return the HTTP 400 Bad Request status code and an error response '
+        'with messages that show the non-updatable properties.')
     REQ_PATCH_ODATA_PROPS = (
-        'A client only provides OData annotations: Services shall return the '
-        'HTTP 400 Bad Request status code with the NoOperation message from '
-        'the Base Message Registry or one of the modification success '
-        'responses.'
-    )
+        'PATCH (update): If the update request only contains OData annotations, the service shall return the HTTP 400 '
+        'Bad Request status code with the NoOperation message from the Base Message Registry or a modification success '
+        'response.')
     REQ_PATCH_ARRAY_ELEMENT_REMOVE = (
-        'Within a PATCH request, the service shall accept null to remove an '
-        'element.'
-    )
+        'PATCH on array properties: The service shall accept null to remove an element.')
     REQ_PATCH_ARRAY_ELEMENT_UNCHANGED = (
-        'Within a PATCH request, the service shall accept an empty object {} '
-        'to leave an element unchanged'
-    )
+        'PATCH on array properties: The service shall accept an empty object {} to leave an element unchanged.')
     REQ_PATCH_ARRAY_OPERATIONS_ORDER = (
-        'When processing a PATCH request, the order of operations shall be: '
-        'modifications, deletions, additions.'
-    )
+        'PATCH on array properties: The order of operations shall be modifications, then deletions, then additions.')
     REQ_PATCH_ARRAY_TRUNCATE = (
-        'A PATCH request with fewer elements than in the current array shall '
-        'remove the remaining elements of the array.'
-    )
-    REQ_PUT_NOT_IMPLEMENTED = (
-        'If a service does not implement this method, the service shall '
-        'return the HTTP 405 Method Not Allowed status code.'
-    )
+        'PATCH on array properties: A request with fewer elements than in the current array shall remove the remaining '
+        'elements of the array.')
     REQ_POST_CREATE_VIA_COLLECTION = (
-        'To create a resource, services shall support the POST method on '
-        'resource collections.'
-    )
+        'POST (create): To create a resource, services shall support the POST method on resource collections.')
     REQ_POST_CREATE_URI_IN_LOCATION_HDR = (
-        'Additionally, the service shall set the Location header in the '
-        'response to the URI of the new resource.'
-    )
+        'POST (create): Services shall set the Location header in the response to the URI of the new resource.')
     REQ_POST_CREATE_TO_MEMBERS_PROP = (
-        'Submitting a POST request to a resource collection is equivalent to '
-        'submitting the same request to the Members property of that resource '
-        'collection. Services that support the addition of Members to a '
-        'resource collection shall support both forms.'
-    )
-    REQ_POST_CREATE_NOT_SUPPORTED = (
-        'If the service does not enable creation of resources, the service '
-        'shall return the HTTP 405 Method Not Allowed status code.'
-    )
+        'POST (create): Submitting a POST request to a resource collection is equivalent to submitting the same '
+        'request to the Members property of that resource collection. Services that support the addition of Members to '
+        'a resource collection shall support both forms.')
     REQ_POST_CREATE_NOT_IDEMPOTENT = (
-        'The POST operation shall not be idempotent.'
-    )
+        'POST (create): The POST operation shall not be idempotent.')
     REQ_DELETE_METHOD_REQUIRED = (
-        'To remove a resource, the service shall support the DELETE method.'
-    )
-    REQ_DELETE_NON_DELETABLE_RESOURCE = (
-        'If the resource can never be deleted, the service shall return the '
-        'HTTP 405 Method Not Allowed status code.'
-    )
-    # Service responses assertions (prefix of "RESP_")
+        'DELETE (delete): To remove a resource, the service shall support the DELETE method.')
+
+    # 'Service responses' assertions (prefix of "RESP_")
     RESP_HEADERS_ACCESS_CONTROL_ALLOW_ORIGIN = (
-        'Redfish Services shall return the HTTP 1.1 Specification-defined '
-        '[Access-Control-Allow-Origin header] if the value in the Required '
-        'column is Yes.'
-    )
+        'Response headers: Services shall return the Access-Control-Allow-Origin header with the behaviors defined in '
+        'the Redfish Specification and HTTP 1.1 Specification.')
     RESP_HEADERS_ALLOW_METHOD_NOT_ALLOWED = (
-        '[The Allow header] shall be returned with the HTTP 405 (Method Not '
-        'Allowed) status code to indicate the valid methods for the request '
-        'URI.'
-    )
+        'Response headers: Services shall return the Allow header with the HTTP 405 Method Not Allowed status code to '
+        'indicate the valid methods for the URI.')
     RESP_HEADERS_ALLOW_GET_OR_HEAD = (
-        '[The Allow header] shall be returned with any GET or HEAD operation '
-        'to indicate the other allowable operations for this resource.'
-    )
+        'Response headers: Services shall return the Allow header for any GET or HEAD operation to indicate the valid '
+        'methods for the URI.')
     RESP_HEADERS_CACHE_CONTROL = (
-        'Redfish Services shall return the HTTP 1.1 Specification-defined '
-        '[Cache-Control header] if the value in the Required column is Yes.'
-    )
+        'Response headers: Services shall return the Cache-Control header.')
     RESP_HEADERS_CONTENT_TYPE = (
-        'Redfish Services shall return the HTTP 1.1 Specification-defined '
-        '[Content-Type header] if the value in the Required column is Yes.'
-    )
+        'Response headers: Services shall return the Content-Type header.')
     RESP_HEADERS_ETAG = (
-        'The ETag header shall be included on responses to GETs of '
-        'ManagerAccount resources.'
-    )
+        'Response headers: Services shall return the ETag header for all GET operations on ManagerAccount resources.')
     RESP_HEADERS_LINK_REL_DESCRIBED_BY = (
-        'A Link header containing rel=describedby shall be returned on GET '
-        'and HEAD requests.'
-    )
+        'Link header: Services shall return the Link header containing rel=describedby on GET and HEAD requests.')
     RESP_HEADERS_LINK_SCHEMA_VER_MATCH = (
-        'If the referenced JSON Schema is a versioned schema, it shall match '
-        'the version contained in the value of the @odata.type property '
-        'returned in this resource.'
-    )
+        'Link header: If the referenced JSON Schema is a versioned schema, it shall match the version contained in the '
+        'value of the @odata.type property returned in the resource.')
     RESP_HEADERS_LOCATION = (
-        '[The Location header] shall be returned upon creation of a resource. '
-        'Location and X-Auth-Token shall be included on responses that create '
-        'user sessions.'
-    )
+        'Response headers: Service shall return the Location header upon creation of a resource. Location and '
+        'X-Auth-Token shall be included on responses that create user sessions.')
     RESP_HEADERS_ODATA_VERSION = (
-        'Redfish Services shall return the HTTP 1.1 Specification-defined '
-        '[OData-Version header] if the value in the Required column is Yes.'
-    )
+        'Response headers: Services shall return the OData-Version header.')
     RESP_HEADERS_WWW_AUTHENTICATE = (
-        'Redfish Services shall return the HTTP 1.1 Specification-defined '
-        '[WWW-Authenticate header] if the value in the Required column is Yes.'
-    )
+        'Response headers: Services shall return the WWW-Authenticate header when authentication headers in the '
+        'request are missing or invalid.')
     RESP_HEADERS_X_AUTH_TOKEN = (
-        'The token value [from the X-Auth-Token header] shall be '
-        'indistinguishable from random.'
-    )
+        'Response headers: The token value from the X-Auth-Token header shall be indistinguishable from random.')
     RESP_STATUS_BAD_REQUEST = (
-        '[In a 400 Bad Request response] the response body shall return an '
-        'extended error as defined in the Error responses clause.'
-    )
+        'Status codes: The response body for 400 Bad Request status code responses shall contain extended error '
+        'information.')
     RESP_STATUS_INTERNAL_SERVER_ERROR = (
-        '[In a 500 Internal Server Error response] the response body shall '
-        'return an extended error as defined in the Error responses clause.'
-    )
+        'Status codes: The response body for 500 Internal Server Error status code responses shall contain extended '
+        'error information.')
     RESP_ODATA_METADATA_MIME_TYPE = (
-        'The service shall use the application/xml or '
-        'application/xml;charset=utf-8 MIME types to return the OData '
-        'metadata document as an XML document.'
-    )
+        'OData $metadata: Service shall use the application/xml or application/xml;charset=utf-8 MIME types to return '
+        'the OData metadata document as an XML document.')
     RESP_ODATA_METADATA_ENTITY_CONTAINER = (
-        'The service\'s OData metadata document shall include an '
-        'EntityContainer that defines the top-level resources and resource '
-        'collections.'
-    )
+        'Referencing other schemas: The service\'s OData metadata document shall include an EntityContainer that '
+        'defines the top-level resources and resource collections.')
     RESP_ODATA_SERVICE_MIME_TYPE = (
-        'The service shall use the application/json MIME type to return the '
-        'OData service document as a JSON object.'
-    )
+        'OData service document: Service shall use the application/json MIME type to return the OData service document '
+        'as a JSON object.')
     RESP_ODATA_SERVICE_CONTEXT = (
-        'The JSON object shall contain the @odata.context context property '
-        'set to /redfish/v1/$metadata .'
-    )
+        'OData service document: The JSON object shall contain the @odata.context context property set to '
+        '/redfish/v1/$metadata .')
     RESP_ODATA_SERVICE_VALUE_PROP = (
-        'The JSON object shall include a value property set to a JSON array '
-        'that contains an entry for the Service Root and each resource that '
-        'is a direct child of the Service Root.'
-    )
-    # Service details assertions (prefix of "SERV_")
+        'OData service document: The JSON object shall include a value property set to a JSON array that contains an '
+        'entry for the service root and each resource that is a direct child of the service root.')
+
+    # 'Service details' assertions (prefix of "SERV_")
     SERV_EVENT_POST_RESP = (
-        'If the [Event Service] subscription request succeeds, the service '
-        'shall return an HTTP 201 Created status code, and the Location '
-        'header that contains a URI of the newly created subscription '
-        'resource.'
-    )
-    SERV_EVENT_PUSH_STYLE = (
-        'Services shall support push style eventing for all resources that '
-        'can send events.'
-    )
+        'POST to subscription collection: If subscription request succeeds, the service shall return an HTTP 201 '
+        'Created status code, and the Location header that contains a URI of the newly created subscription resource.')
     SERV_EVENT_ERROR_ON_BAD_REQUEST = (
-        'Services shall respond to a request to create a subscription with an '
-        'error if the body of the request is conflicting.'
-    )
-    SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS = (
-        'Services shall respond to a request to create a subscription with an '
-        'error if the body of the request contains both RegistryPrefixes and '
-        'MessageIds, and shall return the HTTP 400 Bad Request status code.'
-    )
+        'POST to subscription collection: Services shall respond to a request to create a subscription with an error '
+        'if the body of the request is conflicting.')
     SERV_SSDP_CAN_BE_DISABLED = (
-        'Use of SSDP is optional, and if implemented, shall enable the user '
-        'to disable the protocol through the ManagerNetworkProtocol resource.'
-    )
+        'Discovery overview: SSDP, if implemented, shall enable the user to disable the protocol through the '
+        'ManagerNetworkProtocol resource.')
     SERV_SSDP_USN_MATCHES_SERVICE_ROOT_UUID = (
-        'The UUID in the USN field of the service shall equal the UUID '
-        'property in the Service Root.'
-    )
-    # NOTE(bdodd): Testing this failover assertion is probably not practical
+        'USN format: The UUID in the USN field of the service shall equal the UUID property in the service root.')
     SERV_SSDP_UUID_STATIC = (
-        'If multiple or redundant managers exist, the UUID of the service '
-        'shall remain static regardless of redundancy failover.'
-    )
+        'USN format: If multiple or redundant managers exist, the UUID of the service shall remain static regardless '
+        'of redundancy failover.')
     SERV_SSDP_UUID_IN_CANONICAL_FORMAT = (
-        'The unique ID shall be in the canonical UUID format, followed by '
-        '::dmtf-org.'
-    )
+        'USN format: The unique ID shall be in the canonical UUID format, followed by ::dmtf-org.')
     SERV_SSDP_MSEARCH_RESPONDS_TO_REDFISH_OR_ALL = (
-        'The managed device shall respond to M-SEARCH queries for Search '
-        'Target (ST) of the Redfish Service, as well as ssdp:all.'
-    )
+        'M-SEARCH response: Services shall respond to M-SEARCH queries for Search Target (ST) of the Redfish Service, '
+        'as well as ssdp:all.')
     SERV_SSDP_ST_HEADER_FORMAT = (
-        'The URN provided in the ST header in the reply shall use the '
-        'redfish-rest: service name followed by the major version of the '
-        'Redfish Specification. If the minor version of the Redfish '
-        'Specification to which the service conforms is a non-zero value, '
-        'that minor version shall be appended with and preceded by a colon '
-        '(:).'
-    )
+        'M-SEARCH response: The URN provided in the ST header in the reply shall use the redfish-rest: service name '
+        'followed by the major version of the Redfish Specification. If the minor version of the Redfish Specification '
+        'to which the service conforms is a non-zero value, that minor version shall be appended with and preceded by '
+        'a colon (:).')
     SERV_SSDP_AL_HEADER_POINTS_TO_SERVICE_ROOT = (
-        'The managed device shall provide clients with the AL header that '
-        'points to the Redfish Service Root URL.'
-    )
+        'M-SEARCH response: Services shall provide clients with the AL header that points to the Redfish service root '
+        'URL.')
     SERV_SSDP_M_SEARCH_RESPONSE_FORMAT = (
-        'The response to an M-SEARCH multicast or unicast query shall use '
-        'the [example format shown].'
-    )
+        'M-SEARCH response: The response to an M-SEARCH multicast or unicast query shall use the format defined in the '
+        'Redfish Specification.')
     SERV_SSE_SUCCESSFUL_RESPONSE = (
-        'Successful resource responses for SSE shall return the HTTP 200 OK '
-        'status code and have a Content-Type header set as '
-        '"text/event-stream" or "text/event-stream;charset=utf-8".'
-    )
+        'Server-sent events: Successful resource responses for SSE shall return the HTTP 200 OK status code and have a '
+        'Content-Type header set as text/event-stream or text/event-stream;charset=utf-8.')
     SERV_SSE_UNSUCCESSFUL_RESPONSE = (
-        'Unsuccessful resource responses for SSE shall return an HTTP status '
-        'code of 400 or greater, have a Content-Type header set as '
-        '"application/json" or "application/json;charset=utf-8", and contain '
-        'a JSON object in the response body, as described in Error responses, '
-        'which details the error or errors.'
-    )
+        'Server-sent events: Unsuccessful resource responses for SSE shall return an HTTP status code of 400 or '
+        'greater, have a Content-Type header set as application/json or application/json;charset=utf-8, and contain a '
+        'JSON object in the response body, as described in Error responses, which details the error or errors.')
     SERV_SSE_BLANK_LINES_BETWEEN_EVENTS = (
-        'Services shall separate events with blank lines. '
-    )
+        'Server-sent events: Services shall separate events with blank lines. ')
     SERV_SSE_CONNECTION_OPEN_UNTIL_CLOSED = (
-        'If a client performs a GET on the URI specified by the '
-        'ServerSentEventUri property, the service shall keep the connection '
-        'open and conform to the HTML5 Specification until the client closes '
-        'the socket.'
-    )
+        'Server-sent events: If a client performs a GET on the URI specified by the ServerSentEventUri property, the '
+        'service shall keep the connection open and conform to the HTML5 Specification until the client closes the '
+        'socket.')
     SERV_SSE_EVENTS_SENT_VIA_OPEN_CONNECTION = (
-        'Service-generated events shall be sent to the client by using the '
-        'open connection.'
-    )
+        'Server-sent events: Service-generated events shall be sent to the client by using the open connection.')
     SERV_SSE_OPEN_CREATES_EVENT_DEST = (
-        'When a client opens an SSE stream for the Event Service, the service '
-        'shall create an EventDestination resource in the Subscriptions '
-        'collection for the Event Service to represent the connection.'
-    )
+        'Server-sent events: When a client opens an SSE stream for the event aervice, the service shall create an '
+        'EventDestination resource in the subscriptions collection for the event service to represent the connection.')
     SERV_SSE_EVENT_DEST_CONTEXT_OPAQUE_STR = (
-        'The Context property in the EventDestination resource shall be a '
-        'service-generated opaque string.'
-    )
+        'Server-sent events: The Context property in the EventDestination resource shall be a service-generated opaque '
+        'string.')
     SERV_SSE_EVENT_DEST_DELETED_ON_CLOSE = (
-        'The service shall delete the corresponding EventDestination resource '
-        'when the connection is closed.'
-    )
+        'Server-sent events: The service shall delete the corresponding EventDestination resource when the connection '
+        'is closed.')
     SERV_SSE_CLOSE_CONNECTION_IF_EVENT_DEST_DELETED = (
-        'The service shall close the connection if the corresponding '
-        'EventDestination resource is deleted.'
-    )
+        'Server-sent events: The service shall close the connection if the corresponding EventDestination resource is '
+        'deleted.')
     SERV_SSE_ID_FIELD_UNIQUELY_IDENTIFIES_PAYLOAD = (
-        'The service shall use the id field in the SSE stream to uniquely '
-        'identify a payload in the SSE stream.'
-    )
+        'Server-sent events: The service shall use the id field in the SSE stream to uniquely identify a payload in '
+        'the SSE stream.')
     SERV_SSE_DATA_FIELD_BASED_ON_PAYLOAD_FORMAT = (
-        'The service shall use the data field in the SSE stream based on the '
-        'payload format. The SSE streams have these formats: [metric report '
-        'SSE stream and event message SSE stream].'
-    )
+        'Server-sent events: The service shall use the data field in the SSE stream based on the payload format. The '
+        'SSE streams have these formats: metric report SSE stream and event message SSE stream.')
     SERV_SSE_JSON_EVENT_MESSAGE_FORMAT = (
-        'The service shall use the data field in the SSE stream to include '
-        'the JSON representation of the Event object.'
-    )
+        'Server-sent events: The service shall use the data field in the SSE stream to include the JSON representation '
+        'of the event object.')
     SERV_SSE_JSON_METRIC_REPORT_FORMAT = (
-        'The service shall use the data field in the SSE stream to include '
-        'the JSON representation of the MetricReport object.'
-    )
-    # Security details assertions (prefix of "SEC_")
+        'Server-sent events: The service shall use the data field in the SSE stream to include the JSON representation '
+        'of the MetricReport object.')
+
+    # 'Security details' assertions (prefix of "SEC_")
     SEC_TLS_1_1 = (
-        'Implementations shall support the Transport Layer Security (TLS) '
-        'protocol v1.1 or later.'
-    )
+        'Transport Layer Security (TLS) protocol overview: Implementations shall support the Transport Layer Security '
+        '(TLS) protocol v1.1 or later.')
     SEC_DEFAULT_CERT_REPLACE = (
-        'Redfish implementations shall support replacement of the default '
-        'certificate if one is provided.'
-    )
+        'Certificates: Implementations shall support replacement of the default certificate if one is provided.')
     SEC_CERTS_CONFORM_X509V3 = (
-        'Redfish implementations shall use certificates that conform to '
-        'X.509-v3, as defined in RFC5280.'
-    )
+        'Certificates: Implementations shall use certificates that conform to X.509-v3, as defined in RFC5280.')
     SEC_BOTH_AUTH_TYPES = (
-        'Service shall support both "Basic authentication" and "Redfish '
-        'session login authentication" (as described below under Session '
-        'Management).'
-    )
+        'Authentication overview: Services shall support both "Basic authentication" and "Redfish session login '
+        'authentication".')
     SEC_BASIC_AUTH_STANDALONE = (
-        'Services shall not require a client that uses HTTP Basic '
-        'authentication to create a session.'
-    )
+        'Authentication overview: Services shall not require a client that uses HTTP Basic authentication to create a '
+        'session.')
     SEC_WRITE_REQUIRES_AUTH = (
-        'Services shall authenticate all write requests to Redfish resources '
-        '[except for the POST operation to the Sessions resource collection '
-        'for authentication.]'
-    )
+        'Resource and operation authentication requirements: Services shall authenticate all write requests to Redfish '
+        'resources, with some exceptions.')
     SEC_READ_REQUIRES_AUTH = (
-        'Redfish resources shall not be available as unauthenticated, except '
-        'for [the service root, $metadata document, OData service document, '
-        'OpenAPI YAML document, and version object].'
-    )
-    SEC_REDIRECT_ENFORCES_TARGET_PRIVS = (
-        'An HTTP redirect shall enforce the privilege requirements for the '
-        'target resource.'
-    )
-    SEC_REDIRECT_TO_HTTPS = (
-        'Generally, if the location is reachable without authentication but '
-        'only over HTTPS, the service shall issue a redirect to the HTTPS '
-        'version of the resource.'
-    )
-    SEC_NO_PRIV_INFO_IN_MSGS = (
-        'When authentication fails, extended error messages shall not provide '
-        'privileged information.'
-    )
+        'Resource and operation authentication requirements: Resources shall not be available as unauthenticated, with '
+        'some exceptions.')
     SEC_HEADERS_FIRST = (
-        'Services shall process HTTP headers for authentication before other '
-        'headers that may affect the response. [e.g., ETag, If-Modified, etc.]'
-    )
+        'HTTP header authentication requirements: Services shall process HTTP headers for authentication before other '
+        'headers that may affect the response.')
     SEC_NO_AUTH_COOKIES = (
-        'Services shall not use HTTP cookies to authenticate any activity, '
-        'such as GET, POST, PUT, PATCH, and DELETE.'
-    )
+        'HTTP header authentication requirements: Services shall not use HTTP cookies to authenticate any activity.')
+    SEC_NO_PRIV_INFO_IN_MSGS = (
+        'Authentication failure requirements: When authentication fails, extended error messages shall not provide '
+        'privileged information.')
     SEC_SUPPORT_BASIC_AUTH = (
-        # Note: Second half of this clause is not testable
-        'Services shall support HTTP Basic authentication, as defined by '
-        'RFC7617, and shall use only connections that conform to TLS to '
-        'transport the data between any third-party authentication service '
-        'and clients.'
-    )
+        'HTTP Basic authentication: Services shall support HTTP Basic authentication and shall use only connections '
+        'that conform to TLS to transport the data between any third-party authentication service and clients.')
     SEC_BASIC_AUTH_OVER_HTTPS = (
-        'All requests that use HTTP Basic authentication shall require HTTPS.'
-    )
+        'HTTP Basic authentication: All requests that use HTTP Basic authentication shall require HTTPS.')
     SEC_REQUIRE_LOGIN_SESSIONS = (
-        'Service shall provide login sessions that conform with this '
-        'specification.'
-    )
+        'Redfish session login authentication: Service shall provide login sessions that conform with this '
+        'specification.')
     SEC_SESSIONS_URI_LOCATION = (
-        'To establish a session, find the URI in either the Session '
-        'Service\'s Sessions property or the Service Root\'s links property '
-        'under the Sessions property. Both URIs shall be the same.'
-    )
-    SEC_SESSION_POST_RESPONSE = (
-        'The response to the POST request to create a session shall include '
-        '[X-Auth-Token header, Location header, and JSON body containing the '
-        'full representation of the new session resource.]'
-    )
+        'Redfish login sessions: The session service\'s Sessions property and the service root\'s Sessions property in '
+        'Links property shall contain the same URI.')
     SEC_SESSION_CREATE_HTTPS_ONLY = (
-        'The POST to create a session shall only be supported with HTTPS.'
-    )
+        'Session login: The POST to create a session shall only be supported with HTTPS.')
+    SEC_SESSION_POST_RESPONSE = (
+        'Session login: The response to the POST request to create a session shall include the X-Auth-Token header, '
+        'the Location header, and a JSON body containing the full representation of the new session resource.')
     SEC_SESSION_TERMINATION_SIDE_EFFECTS = (
-        'When a session is terminated, the service shall not affect '
-        'independent connections established originally by this session for '
-        'other purposes, such as connections for Server-Sent Events or '
-        'transferring an image for the Update Service.'
-    )
-    SEC_ACCOUNTS_SUPPORT_ETAGS = (
-        'User accounts shall support ETags and atomic operations.'
-    )
-    SEC_PWD_CHANGE_REQ_ALLOW_SESSION_LOGIN = (
-        '[When using an account with PasswordChangeRequired set to true] the '
-        'service shall allow a session login and include a '
-        '@Message.ExtendedInfo object in the response containing the '
-        'PasswordChangeRequired message from the Base Message Registry.'
-    )
-    SEC_PWD_CHANGE_REQ_ALLOW_GET_ACCOUNT = (
-        '[When using an account with PasswordChangeRequired set to true] the '
-        'service shall allow a GET operation on the ManagerAccount resource '
-        'associated with the account.'
-    )
-    SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD = (
-        '[When using an account with PasswordChangeRequired set to true] the '
-        'service shall allow a PATCH operation on the ManagerAccount '
-        'resource associated with the account to update the Password '
-        'property. If the value of Password is changed, the service shall '
-        'also set the PasswordChangeRequired property to false.'
-    )
-    SEC_PWD_CHANGE_REQ_DISALLOW_ALL_OTHERS = (
-        'For all other operations [when using an account with '
-        'PasswordChangeRequired set to true], the service shall respond with '
-        'the HTTP 403 Forbidden status code and include a '
-        '@Message.ExtendedInfo object that contains the '
-        'PasswordChangeRequired message from the Base Message Registry.'
-    )
+        'Session termination or logout: When a session is terminated, the service shall not affect independent '
+        'connections established originally by this session for other purposes.')
     SEC_PRIV_ONE_ROLE_PRE_USER = (
-        'Each user shall be assigned exactly one role.'
-    )
+        'Privilege model: Each user shall be assigned exactly one role.')
     SEC_PRIV_SUPPORT_PREDEFINED_ROLES = (
-        'Services shall support the previous predefined roles [Administrator, '
-        'Operator, and ReadOnly].'
-    )
+        'Roles: Services shall support the Administrator, Operator, and ReadOnly standard roles.')
     SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE = (
-        'The AssignedPrivileges property in the Role resource for the '
-        'predefined roles shall not be modifiable.'
-    )
+        'Roles: The AssignedPrivileges property in the Role resource for standard roles shall not be modifiable.')
     SEC_PRIV_ROLE_ASSIGNED_AT_ACCOUNT_CREATE = (
-        'A predefined role or a custom role shall be assigned to a user when '
-        'a manager account is created.'
-    )
+        'Privilege model: A role shall be assigned to a user when a manager account is created.')
     SEC_PRIV_OPERATION_TO_PRIV_MAPPING = (
-        'For every request that a client makes to a service, the service '
-        'shall determine that the authenticated identity of the requester has '
-        'the authorization to complete the requested operation on the '
-        'resource in the request.'
-    )
+        'Redfish service operation-to-privilege mapping: For every request that a client makes to a service, the '
+        'service shall determine that the authenticated identity of the requester has the authorization to complete '
+        'the requested operation on the resource in the request.')
+    SEC_ACCOUNTS_SUPPORT_ETAGS = (
+        'Account service overview: User accounts shall support ETags and atomic operations.')
+    SEC_PWD_CHANGE_REQ_ALLOW_SESSION_LOGIN = (
+        'Password change required handling: When using an account with PasswordChangeRequired set to true, the service '
+        'shall allow a session login and include a @Message.ExtendedInfo object in the response containing the '
+        'PasswordChangeRequired message from the Base Message Registry.')
+    SEC_PWD_CHANGE_REQ_ALLOW_GET_ACCOUNT = (
+        'Password change required handling: When using an account with PasswordChangeRequired set to true, the service '
+        'shall allow a GET operation on the ManagerAccount resource associated with the account.')
+    SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD = (
+        'Password change required handling: When using an account with PasswordChangeRequired set to true, the service '
+        'shall allow a PATCH operation on the ManagerAccount resource associated with the account to update the '
+        'Password property. If the value of Password is changed, the service shall also set the PasswordChangeRequired '
+        'property to false.')
+    SEC_PWD_CHANGE_REQ_DISALLOW_ALL_OTHERS = (
+        'Password change required handling: For all other operations when using an account with PasswordChangeRequired '
+        'set to true, the service shall respond with the HTTP 403 Forbidden status code and include a '
+        '@Message.ExtendedInfo object that contains the PasswordChangeRequired message from the Base Message Registry.')
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/protocol_details.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/protocol_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -199,29 +199,25 @@
                     Assertion.PROTO_HTTP_SUPPORTED_METHODS,
                     'No %s requests had a successful response' % method)
 
 
 def test_http_unsupported_methods(sut: SystemUnderTest):
     """Perform tests on unsupported HTTP methods."""
     # Test Assertion.PROTO_HTTP_UNSUPPORTED_METHODS
-    uri = '/redfish/v1/'
-    response = sut.get_response('DELETE', uri, request_type=RequestType.UNSUPPORTED_REQ)
-    if response is None:
-        sut.log(Result.NOT_TESTED, 'DELETE', '', uri,
-                Assertion.PROTO_HTTP_UNSUPPORTED_METHODS,
-                'No response found for DELETE method request')
-    elif (response.status_code == requests.codes.METHOD_NOT_ALLOWED or
-          response.status_code == requests.codes.NOT_IMPLEMENTED):
-        sut.log(Result.PASS, 'DELETE', response.status_code, uri,
-                Assertion.PROTO_HTTP_UNSUPPORTED_METHODS, 'Test passed')
-    else:
-        sut.log(Result.FAIL, 'DELETE', response.status_code, uri,
-                Assertion.PROTO_HTTP_UNSUPPORTED_METHODS,
-                'DELETE method returned status %s; expected status %s' %
-                (response.status_code, requests.codes.METHOD_NOT_ALLOWED))
+    for uri, response in sut.get_all_responses(request_type=RequestType.UNSUPPORTED_REQ):
+        if (response.status_code == requests.codes.METHOD_NOT_ALLOWED or
+            response.status_code == requests.codes.NOT_IMPLEMENTED):
+            sut.log(Result.PASS, response.request.method, response.status_code, uri,
+                    Assertion.PROTO_HTTP_UNSUPPORTED_METHODS, 'Test passed')
+        else:
+            msg = ('The service response returned status code %s; expected %s or %s'
+                   % (response.status_code, requests.codes.METHOD_NOT_ALLOWED,
+                      requests.codes.NOT_IMPLEMENTED))
+            sut.log(Result.FAIL, response.request.method, response.status_code, uri,
+                    Assertion.PROTO_HTTP_UNSUPPORTED_METHODS, msg)
 
 
 def test_media_types(sut: SystemUnderTest, uri, response):
     """Perform tests of the supported media types."""
     if (uri != '/redfish/v1/$metadata' and response.request.method != 'HEAD'
             and response.status_code in [requests.codes.OK,
                                          requests.codes.CREATED]):
@@ -262,15 +258,15 @@
     # Test Assertion.PROTO_ETAG_RFC7232
     if (response.request.method != 'HEAD' and response.status_code
             in [requests.codes.OK, requests.codes.CREATED]):
         etag = response.headers.get('ETag')
         source = 'header'
         if (etag is None and utils.get_response_media_type(response)
                 == 'application/json'):
-            data = response.json()
+            data = utils.get_response_json(response)
             if '@odata.etag' in data:
                 source = 'property'
                 etag = data.get('@odata.etag')
         if etag is not None:
             if check_etag_valid(etag):
                 sut.log(Result.PASS, response.request.method,
                         response.status_code, uri,
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/redfish_logo.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/redfish_logo.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/report.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/report.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/resources.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 
 def find_certificates(sut: SystemUnderTest, data):
     if 'NetworkProtocol' in data:
         uri = data['NetworkProtocol']['@odata.id']
         r = sut.session.get(sut.rhost + uri)
         yield {'uri': uri, 'response': r}
         if r.ok:
-            d = r.json()
+            d = utils.get_response_json(r)
             if 'HTTPS' in d and 'Certificates' in d['HTTPS']:
                 coll_uri = d['HTTPS']['Certificates']['@odata.id']
                 r = sut.session.get(sut.rhost + coll_uri)
                 yield {'uri': coll_uri, 'response': r}
                 if r.ok:
-                    d = r.json()
+                    d = utils.get_response_json(r)
                     if 'Members' in d and len(d['Members']):
                         for m in d['Members']:
                             uri = m['@odata.id']
                             # uncomment next 2 lines if we need to read certs
                             # r = session.get(sut.rhost + uri)
                             # yield {'uri': uri, 'response': r}
                             sut.add_cert(coll_uri, uri)
@@ -81,121 +81,121 @@
 
     # do HEAD on the service root
     r = sut.session.head(sut.rhost + uri)
     yield {'uri': uri, 'response': r}
     # do GET on the service root
     r = sut.session.get(sut.rhost + uri)
     yield {'uri': uri, 'response': r}
-    root = r.json() if r.status_code == requests.codes.OK else {}
+    root = utils.get_response_json(r) if r.status_code == requests.codes.OK else {}
 
     sut.set_version(root.get('RedfishVersion', '1.0.0'))
     sut.set_product(root.get('Product', 'N/A'))
     sut.set_service_uuid(root.get('UUID'))
     sut.set_supported_query_params(root.get('ProtocolFeaturesSupported', {}))
 
     for prop in ['Systems', 'Chassis']:
         if prop in root:
             uri = root[prop]['@odata.id']
             sut.set_nav_prop_uri(prop, uri)
             r = sut.session.get(sut.rhost + uri)
             yield {'uri': uri, 'response': r}
             if r.ok:
-                data = r.json()
+                data = utils.get_response_json(r)
                 if 'Members' in data and len(data['Members']):
                     uri = data['Members'][0]['@odata.id']
                     r = sut.session.get(sut.rhost + uri)
                     yield {'uri': uri, 'response': r}
 
     if 'Managers' in root:
         uri = root['Managers']['@odata.id']
         sut.set_nav_prop_uri('Managers', uri)
         r = sut.session.get(sut.rhost + uri)
         yield {'uri': uri, 'response': r}
         if r.ok:
-            data = r.json()
+            data = utils.get_response_json(r)
             if 'Members' in data and len(data['Members']):
                 for m in data['Members']:
                     uri = m['@odata.id']
                     r = sut.session.get(sut.rhost + uri)
                     yield {'uri': uri, 'response': r}
                     if r.ok:
-                        d = r.json()
+                        d = utils.get_response_json(r)
                         set_mfr_model_fw(sut, d)
                         set_mgr_net_proto_uri(sut, d)
                         for c in find_certificates(sut, d):
                             yield c
 
     if 'AccountService' in root:
         uri = root['AccountService']['@odata.id']
         sut.set_nav_prop_uri('AccountService', uri)
         r = sut.session.get(sut.rhost + uri)
         yield {'uri': uri, 'response': r}
         if r.ok:
-            data = r.json()
+            data = utils.get_response_json(r)
             if 'PrivilegeMap' in data:
                 uri = data['PrivilegeMap']['@odata.id']
                 sut.set_nav_prop_uri('PrivilegeMap', uri)
             for prop in ['Accounts', 'Roles']:
                 if prop in data:
                     uri = data[prop]['@odata.id']
                     r = sut.session.get(sut.rhost + uri)
                     yield {'uri': uri, 'response': r}
                     sut.set_nav_prop_uri(prop, uri)
                     if r.ok:
-                        d = r.json()
+                        d = utils.get_response_json(r)
                         if 'Members' in d and len(d['Members']):
                             if prop == 'Accounts':
                                 resource_type = ResourceType.MANAGER_ACCOUNT
                                 # get accounts up to sut.username
                                 for m in d['Members']:
                                     uri = m['@odata.id']
                                     r = sut.session.get(sut.rhost + uri)
                                     yield {'uri': uri, 'response': r,
                                            'resource_type': resource_type}
                                     if r.ok:
-                                        sut.add_user(r.json())
-                                        if (r.json().get('UserName')
+                                        sut.add_user(utils.get_response_json(r))
+                                        if (utils.get_response_json(r).get('UserName')
                                                 == sut.username):
                                             break
 
                             else:
                                 resource_type = ResourceType.ROLE
                                 # get all the roles
                                 for m in d['Members']:
                                     uri = m['@odata.id']
                                     r = sut.session.get(sut.rhost + uri)
                                     yield {'uri': uri, 'response': r,
                                            'resource_type': resource_type}
                                     if r.ok:
-                                        sut.add_role(r.json())
+                                        sut.add_role(utils.get_response_json(r))
 
     if 'SessionService' in root:
         uri = root['SessionService']['@odata.id']
         r = sut.session.get(sut.rhost + uri)
         yield {'uri': uri, 'response': r}
         if r.ok:
-            data = r.json()
+            data = utils.get_response_json(r)
             if 'Sessions' in data:
                 uri = data['Sessions']['@odata.id']
                 r = sut.session.get(sut.rhost + uri)
                 yield {'uri': uri, 'response': r}
                 if r.ok:
-                    data = r.json()
+                    data = utils.get_response_json(r)
                     if 'Members' in data and len(data['Members']):
                         uri = data['Members'][0]['@odata.id']
                         r = sut.session.get(sut.rhost + uri)
                         yield {'uri': uri, 'response': r}
 
     if 'EventService' in root:
         uri = root['EventService']['@odata.id']
         sut.set_nav_prop_uri('EventService', uri)
         r = sut.session.get(sut.rhost + uri)
         yield {'uri': uri, 'response': r}
         if r.ok:
-            data = r.json()
+            data = utils.get_response_json(r)
             if 'Subscriptions' in data:
                 sut.set_nav_prop_uri(
                     'Subscriptions', data['Subscriptions']['@odata.id'])
             if 'ServerSentEventUri' in data:
                 uri = data['ServerSentEventUri']
                 sut.set_server_sent_event_uri(uri)
                 r, event_dest_uri = utils.get_sse_stream(sut)
@@ -263,58 +263,38 @@
                 new_password = pwd
     except Exception as e:
         logging.error('Caught exception while creating or patching other '
                       'account; Exception: %s; continuing with test' % str(e))
     return new_user, new_password, new_acct_uri
 
 
-def patch_session(sut: SystemUnderTest, session_uri):
-    """PATCH a session; should fail, sessions are not updatable"""
-    payload = {'UserName': 'pRoToVAl'}
-    headers = utils.get_etag_header(sut, sut.session, session_uri)
-    response = sut.patch(session_uri, json=payload, headers=headers)
-    sut.add_response(session_uri, response,
-                     request_type=RequestType.PATCH_RO_RESOURCE)
-
-
-def patch_collection(sut: SystemUnderTest, collection_uri):
-    """PATCH a collection; should fail, collections are not updatable"""
-    payload = {'Name': 'My Collection'}
-    headers = utils.get_etag_header(sut, sut.session, collection_uri)
-    response = sut.patch(collection_uri, json=payload, headers=headers)
-    sut.add_response(collection_uri, response,
-                     request_type=RequestType.PATCH_COLLECTION)
-
-
 def delete_account(sut: SystemUnderTest, session, user, acct_uri,
                    request_type=RequestType.NORMAL):
     # DELETE account
     if acct_uri:
         acct.delete_account(sut, session, user, acct_uri,
                             request_type=request_type)
 
 
 def data_modification_requests(sut: SystemUnderTest):
     new_session_uri, _ = sessions.create_session(sut)
     if new_session_uri:
-        patch_session(sut, new_session_uri)
         sessions.delete_session(sut, sut.session, new_session_uri,
                                 request_type=RequestType.NORMAL)
-    patch_collection(sut, sut.sessions_uri)
     new_user, new_pwd, new_uri = None, None, None
     other_user, other_pwd, other_uri = None, None, None
     try:
         new_user, new_pwd, new_uri = create_account(
             sut, sut.session, request_type=RequestType.NORMAL)
         if new_uri:
             response = sut.session.get(sut.rhost + new_uri)
             sut.add_response(new_uri, response)
             if response.ok:
                 etag = utils.get_response_etag(response)
-                data = response.json()
+                data = utils.get_response_json(response)
                 if 'PasswordChangeRequired' in data:
                     acct.password_change_required(sut, sut.session, new_user,
                                                   new_pwd, new_uri, data, etag)
             pwd = patch_account(sut, sut.session, new_uri,
                                 request_type=RequestType.NORMAL)
             if pwd:
                 new_pwd = pwd
@@ -351,17 +331,24 @@
         delete_account(sut, no_auth_session, user, new_acct_uri,
                        request_type=RequestType.NO_AUTH)
         delete_account(sut, sut.session, user, new_acct_uri,
                        request_type=RequestType.NORMAL)
 
 
 def unsupported_requests(sut: SystemUnderTest):
-    # DELETE on service root is never allowed
+    # Data modification requests on the service root are never allowed
     uri = '/redfish/v1/'
-    response = sut.session.request('DELETE', sut.rhost + uri)
+    response = sut.delete(uri)
+    sut.add_response(uri, response, request_type=RequestType.UNSUPPORTED_REQ)
+    response = sut.patch(uri, json={})
+    sut.add_response(uri, response, request_type=RequestType.UNSUPPORTED_REQ)
+    response = sut.post(uri, json={})
+    sut.add_response(uri, response, request_type=RequestType.UNSUPPORTED_REQ)
+    # Unsupported HTTP methods return HTTP 501
+    response = sut.session.request('FAKEMETHODFORTEST', sut.rhost + uri)
     sut.add_response(uri, response, request_type=RequestType.UNSUPPORTED_REQ)
 
 
 def basic_auth_requests(sut: SystemUnderTest):
     headers = {
         'OData-Version': '4.0'
     }
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/security_details.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/security_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SEC_DEFAULT_CERT_REPLACE, msg)
         return
 
     if sut.certificate_service_uri is not None:
         response = sut.get_response('GET', sut.certificate_service_uri)
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             if ('Actions' in data and '#CertificateService.ReplaceCertificate'
                     in data['Actions']):
                 sut.log(Result.PASS, 'GET', response.status_code,
                         sut.certificate_service_uri,
                         Assertion.SEC_DEFAULT_CERT_REPLACE, 'Test passed')
                 return
 
@@ -238,71 +238,41 @@
                 else:
                     sut.log(Result.PASS, response.request.method,
                             response.status_code, uri,
                             Assertion.SEC_READ_REQUIRES_AUTH, 'Test passed')
 
 
 def test_redirect_enforces_target_privs(sut: SystemUnderTest):
-    """Perform test for Assertion.SEC_REDIRECT_ENFORCES_TARGET_PRIVS."""
+    """Perform test for Assertion.PROTO_REDIRECT_ENFORCES_TARGET_PRIVS."""
     uri = sut.sessions_uri
     redirect_found = False
     response = sut.get_response('GET', uri,
                                 request_type=RequestType.HTTP_NO_AUTH)
     if response is not None:
         if len(response.history):
             # HTTP redirect occurred if there is a response.history
             # check the final status and expect a 401
             redirect_found = True
             if response.status_code == requests.codes.UNAUTHORIZED:
                 sut.log(Result.PASS, response.request.method,
                         response.status_code, uri,
-                        Assertion.SEC_REDIRECT_ENFORCES_TARGET_PRIVS,
+                        Assertion.PROTO_REDIRECT_ENFORCES_TARGET_PRIVS,
                         'Test passed')
             else:
                 msg = ('After HTTP redirect from %s to %s, response status '
                        'was %s, expected 401' % (
                         response.history[0].url, response.url,
                         response.status_code))
                 sut.log(Result.FAIL, response.request.method,
                         response.status_code, uri,
-                        Assertion.SEC_REDIRECT_ENFORCES_TARGET_PRIVS, msg)
+                        Assertion.PROTO_REDIRECT_ENFORCES_TARGET_PRIVS, msg)
     if not redirect_found:
         msg = 'No response found with an HTTP redirect'
         sut.log(Result.NOT_TESTED, 'GET', '', uri,
-                Assertion.SEC_REDIRECT_ENFORCES_TARGET_PRIVS, msg)
-
-
-def test_redirect_to_https(sut: SystemUnderTest):
-    """Perform test for Assertion.SEC_REDIRECT_TO_HTTPS."""
-    uri = '/redfish/v1/'
-    redirect_found = False
-    response = sut.get_response('GET', uri,
-                                request_type=RequestType.HTTP_NO_AUTH)
-    if response is not None:
-        if len(response.history):
-            # HTTP redirect occurred if there is a response.history
-            # check the final status and expect a 200
-            redirect_found = True
-            if response.status_code == requests.codes.OK:
-                sut.log(Result.PASS, response.request.method,
-                        response.status_code, uri,
-                        Assertion.SEC_REDIRECT_TO_HTTPS,
-                        'Test passed')
-            else:
-                msg = ('After HTTP redirect from %s to %s, response status '
-                       'was %s, expected 200' % (
-                           response.history[0].url, response.url,
-                           response.status_code))
-                sut.log(Result.FAIL, response.request.method,
-                        response.status_code, uri,
-                        Assertion.SEC_REDIRECT_TO_HTTPS, msg)
-    if not redirect_found:
-        msg = 'No response found with an HTTP redirect'
-        sut.log(Result.NOT_TESTED, 'GET', '', uri,
-                Assertion.SEC_REDIRECT_TO_HTTPS, msg)
+                Assertion.PROTO_REDIRECT_ENFORCES_TARGET_PRIVS, msg)
 
 
 def test_no_priv_info_in_msgs(sut: SystemUnderTest):
     """"Perform test for Assertion.SEC_NO_PRIV_INFO_IN_MSGS."""
     for uri, response in sut.get_all_responses(
             request_type=RequestType.BAD_AUTH):
         if not response.ok:
@@ -476,22 +446,22 @@
 
 
 def test_sessions_uri_location(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_SESSIONS_URI_LOCATION."""
     sessions_uri1, sessions_uri2 = None, None
     response1 = sut.get_response('GET', '/redfish/v1/')
     if response1.ok:
-        data = response1.json()
+        data = utils.get_response_json(response1)
         if 'Links' in data and 'Sessions' in data['Links']:
             sessions_uri1 = data['Links']['Sessions']['@odata.id']
         if 'SessionService' in data:
             uri = data['SessionService']['@odata.id']
             response2 = sut.get_response('GET', uri)
             if response2.ok:
-                data = response2.json()
+                data = utils.get_response_json(response2)
                 if 'Sessions' in data:
                     sessions_uri2 = data['Sessions']['@odata.id']
         if sessions_uri1 and sessions_uri2:
             if sessions_uri1 == sessions_uri2:
                 sut.log(Result.PASS, 'GET', response1.status_code,
                         sessions_uri1, Assertion.SEC_SESSIONS_URI_LOCATION,
                         'Test passed')
@@ -522,15 +492,15 @@
                 failed = True
                 msg = ('Response for POST to %s did not contain required '
                        '%s header' % (sut.sessions_uri, header))
                 sut.log(Result.FAIL, 'POST', response.status_code,
                         sut.sessions_uri, Assertion.SEC_SESSION_POST_RESPONSE,
                         msg)
         if response.status_code == requests.codes.CREATED:
-            data = response.json()
+            data = utils.get_response_json(response)
             missing_props = []
             for prop in ['@odata.id', '@odata.type', 'Id', 'Name', 'UserName']:
                 if prop not in data:
                     missing_props.append(prop)
             if missing_props:
                 failed = True
                 msg = ('Response payload for POST to %s did not contain full '
@@ -743,15 +713,15 @@
     if response is None:
         msg = ('PasswordChangeRequired property not found in account '
                'resource; unable to test this assertion')
         sut.log(Result.NOT_TESTED, 'POST', '', sut.sessions_uri,
                 Assertion.SEC_PWD_CHANGE_REQ_ALLOW_SESSION_LOGIN, msg)
     else:
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             keys = utils.get_extended_info_message_keys(data)
             if 'PasswordChangeRequired' in keys:
                 sut.log(Result.PASS, 'POST', response.status_code,
                         sut.sessions_uri,
                         Assertion.SEC_PWD_CHANGE_REQ_ALLOW_SESSION_LOGIN,
                         'Test passed')
             else:
@@ -801,15 +771,15 @@
         msg = ('No GET request to %s found using account with '
                'PasswordChangeRequired set; unable to test this assertion'
                % sut.sessions_uri)
         sut.log(Result.NOT_TESTED, 'GET', '', sut.sessions_uri,
                 Assertion.SEC_PWD_CHANGE_REQ_DISALLOW_ALL_OTHERS, msg)
     else:
         if response.status_code == requests.codes.FORBIDDEN:
-            data = response.json()
+            data = utils.get_response_json(response)
             keys = utils.get_extended_info_message_keys(data)
             if 'PasswordChangeRequired' in keys:
                 sut.log(Result.PASS, 'GET', response.status_code,
                         sut.sessions_uri,
                         Assertion.SEC_PWD_CHANGE_REQ_DISALLOW_ALL_OTHERS,
                         'Test passed')
             else:
@@ -834,16 +804,16 @@
         if response is None:
             msg = ('No PATCH request to %s found using account with '
                    'PasswordChangeRequired set; unable to test this assertion'
                    % account_uri)
             sut.log(Result.NOT_TESTED, 'PATCH', '', account_uri,
                     Assertion.SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD, msg)
         else:
-            if response.ok:
-                data = response.json()
+            if response.status_code == requests.codes.OK:
+                data = utils.get_response_json(response)
                 if ('PasswordChangeRequired' in data and
                         data['PasswordChangeRequired'] is False):
                     sut.log(Result.PASS, 'PATCH', response.status_code,
                             account_uri,
                             Assertion.SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD,
                             'Test passed')
                 else:
@@ -851,14 +821,21 @@
                            'but response payload did not have '
                            'PasswordChangeRequired property set to false' %
                            (response.status_code, account_uri))
                     sut.log(Result.FAIL, 'PATCH', response.status_code,
                             account_uri,
                             Assertion.SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD,
                             msg)
+            elif response.ok:
+                # No response body; treat as a pass; may want to consider
+                # adding a follow-up GET to perform an additional check
+                sut.log(Result.PASS, 'PATCH', response.status_code,
+                        account_uri,
+                        Assertion.SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD,
+                        'Test passed')
             else:
                 msg = ('Password change to %s failed with status %s; '
                        'expected it to succeed' %
                        (account_uri, response.status_code))
                 sut.log(Result.FAIL, 'PATCH', response.status_code,
                         account_uri,
                         Assertion.SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD,
@@ -871,15 +848,15 @@
 
 
 def test_priv_one_role_per_user(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_PRIV_ONE_ROLE_PRE_USER."""
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.MANAGER_ACCOUNT).items():
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             role = data.get('RoleId')
             if role is not None:
                 sut.log(Result.PASS, 'GET', response.status_code, uri,
                         Assertion.SEC_PRIV_ONE_ROLE_PRE_USER,
                         'Test passed')
             else:
                 msg = ('Account URI %s does not have a RoleId property' % uri)
@@ -903,15 +880,15 @@
             'privs': {'Login', 'ConfigureSelf'},
             'found': False
         }
     }
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.ROLE).items():
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             role = data.get('Id')
             if role in role_map:
                 role_map[role]['found'] = True
                 privs = set(data.get('AssignedPrivileges', []))
                 if privs == role_map[role]['privs']:
                     sut.log(Result.PASS, 'GET', response.status_code, uri,
                             Assertion.SEC_PRIV_SUPPORT_PREDEFINED_ROLES,
@@ -937,15 +914,15 @@
     role = 'ReadOnly'
     test_priv = ['Login', 'ConfigureManager', 'ConfigureUsers',
                  'ConfigureComponents', 'ConfigureSelf']
     # locate the ReadOnly role
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.ROLE).items():
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             if data.get('Id') == role:
                 read_only_found = True
                 break
     if read_only_found:
         # Save the current privileges in case the PATCH is accepted
         privs = data.get('AssignedPrivileges')
         if privs:
@@ -985,15 +962,15 @@
 
 
 def test_priv_roles_assigned_at_account_create(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_PRIV_ROLE_ASSIGNED_AT_ACCOUNT_CREATE."""
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.MANAGER_ACCOUNT).items():
         if response.ok:
-            data = response.json()
+            data = utils.get_response_json(response)
             username = data.get('UserName', '')
             if username.startswith('rfpv'):
                 role = data.get('RoleId')
                 if role is not None:
                     sut.log(Result.PASS, 'GET', response.status_code, uri,
                             Assertion.SEC_PRIV_ROLE_ASSIGNED_AT_ACCOUNT_CREATE,
                             'Test passed')
@@ -1052,15 +1029,14 @@
 def test_authentication(sut: SystemUnderTest):
     """Perform authentication tests"""
     test_basic_auth_standalone(sut)
     test_both_auth_types(sut)
     test_write_requires_auth(sut)
     test_read_requires_auth(sut)
     test_redirect_enforces_target_privs(sut)
-    test_redirect_to_https(sut)
     test_no_priv_info_in_msgs(sut)
     test_headers_auth_before_etag(sut)
     test_no_auth_cookies(sut)
     test_support_basic_auth(sut)
     test_basic_auth_over_https(sut)
     test_require_login_sessions(sut)
     test_sessions_uri_location(sut)
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_details.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/service_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,19 +56,14 @@
     else:
         msg = ('No event subscriptions URI found on the service; unable to '
                'test this assertion')
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SERV_EVENT_POST_RESP, msg)
 
 
-def test_push_style_eventing(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_PUSH_STYLE."""
-    pass
-
-
 def test_event_error_on_bad_request(sut: SystemUnderTest):
     """Perform tests for Assertion.SERV_EVENT_ERROR_ON_BAD_REQUEST."""
     if sut.subscriptions_uri:
         payload = {
             'Context': 'RPV test subscription',
             'Protocol': 'FTP',  # invalid EventDestinationProtocol
             'Destination': 'https://192.168.1.50/Destination1'
@@ -105,68 +100,14 @@
     else:
         msg = ('No event subscriptions URI found on the service; unable to '
                'test this assertion')
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SERV_EVENT_ERROR_ON_BAD_REQUEST, msg)
 
 
-def test_event_error_on_mutually_excl_props(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS."""
-    if sut.subscriptions_uri:
-        payload = {
-            'Context': 'RPV test subscription',
-            'Protocol': 'Redfish',
-            'Destination': 'https://192.168.1.50/Destination1',
-            'RegistryPrefixes': [
-                'Base'
-            ],
-            'MessageIds': [
-                'Base.1.0.Success',
-                'Base.1.0.GeneralError'
-            ]
-        }
-        response = sut.post(sut.subscriptions_uri, json=payload)
-        sut.add_response(sut.subscriptions_uri, response,
-                         request_type=RequestType.SUBSCRIPTION)
-        if response.ok:
-            msg = ('Event subscription request with mutually exclusive '
-                   'properties (RegistryPrefixes and MessageIds) to %s '
-                   'returned status code %s; expected %s' % (
-                       sut.subscriptions_uri, response.status_code,
-                       requests.codes.BAD_REQUEST))
-            sut.log(Result.FAIL, response.request.method,
-                    response.status_code, sut.subscriptions_uri,
-                    Assertion.SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS, msg)
-            location = response.headers.get('Location')
-            if location:
-                # cleanup
-                uri = urlparse(location).path
-                r = sut.delete(uri)
-                sut.add_response(uri, r, request_type=RequestType.SUBSCRIPTION)
-        elif response.status_code == requests.codes.BAD_REQUEST:
-            sut.log(Result.PASS, response.request.method,
-                    response.status_code, sut.subscriptions_uri,
-                    Assertion.SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS,
-                    'Test passed')
-        else:
-            msg = ('Event subscription request with mutually exclusive '
-                   'properties (RegistryPrefixes and MessageIds) to %s '
-                   'returned status code %s; expected %s' % (
-                       sut.subscriptions_uri, response.status_code,
-                       requests.codes.BAD_REQUEST))
-            sut.log(Result.WARN, response.request.method,
-                    response.status_code, sut.subscriptions_uri,
-                    Assertion.SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS, msg)
-    else:
-        msg = ('No event subscriptions URI found on the service; unable to '
-               'test this assertion')
-        sut.log(Result.NOT_TESTED, '', '', '',
-                Assertion.SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS, msg)
-
-
 def pre_ssdp(sut: SystemUnderTest):
     """Perform prerequisite SSDP steps"""
     # discover using the redfish search target
     services = utils.discover_ssdp(search_target=SSDP_REDFISH)
     sut.add_ssdp_services(SSDP_REDFISH, services)
 
     # discover using the ssdp:all search target
@@ -174,15 +115,15 @@
     sut.add_ssdp_services(SSDP_ALL, services)
 
     # determine SSDP enabled/disabled state
     if sut.mgr_net_proto_uri:
         r = sut.session.get(sut.rhost + sut.mgr_net_proto_uri)
         if r.ok:
             sut.add_response(sut.mgr_net_proto_uri, r)
-            d = r.json()
+            d = utils.get_response_json(r)
             if 'SSDP' in d and 'ProtocolEnabled' in d['SSDP']:
                 enabled = d['SSDP']['ProtocolEnabled']
                 sut.set_ssdp_enabled(enabled)
 
 
 def test_ssdp_can_be_disabled(sut: SystemUnderTest):
     """Perform tests for Assertion.SERV_SSDP_CAN_BE_DISABLED."""
@@ -587,15 +528,15 @@
                        )
                 sut.log(Result.FAIL, 'GET', response.status_code,
                         sut.server_sent_event_uri,
                         Assertion.SERV_SSE_UNSUCCESSFUL_RESPONSE, msg)
                 failed = True
             else:
                 errors = ''
-                data = response.json()
+                data = utils.get_response_json(response)
                 if 'error' in data and isinstance(data['error'], dict):
                     if 'code' not in data['error']:
                         errors += (' Property "code" missing from "error" '
                                    'complex property.')
                     elif not isinstance(data['error']['code'], str):
                         errors += ' Property "code" is not a string.'
                     if 'message' not in data['error']:
@@ -792,15 +733,15 @@
         msg = 'No EventDestination URI found; unable to test this assertion'
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SERV_SSE_EVENT_DEST_CONTEXT_OPAQUE_STR, msg)
         return
 
     r = sut.session.get(sut.rhost + event_dest)
     if r.status_code == requests.codes.OK:
-        data = r.json()
+        data = utils.get_response_json(r)
         if 'Context' in data:
             context = data.get('Context')
             if isinstance(context, str):
                 sut.log(Result.PASS, 'GET', r.status_code, event_dest,
                         Assertion.SERV_SSE_EVENT_DEST_CONTEXT_OPAQUE_STR,
                         'Test passed')
             else:
@@ -999,17 +940,15 @@
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SERV_SSE_JSON_METRIC_REPORT_FORMAT, msg)
 
 
 def test_eventing(sut: SystemUnderTest):
     """Perform eventing tests"""
     test_event_service_subscription(sut)
-    test_push_style_eventing(sut)
     test_event_error_on_bad_request(sut)
-    test_event_error_on_mutually_excl_props(sut)
 
 
 def test_discovery(sut: SystemUnderTest):
     """Perform service discovery tests"""
     pre_ssdp(sut)
     test_ssdp_can_be_disabled(sut)
     test_ssdp_usn_matches_service_root_uuid(sut)
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_requests.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/service_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         msg = ('Successful response for GET request to URI %s not found; '
                'unable to test this assertion' % uri)
         sut.log(Result.NOT_TESTED, 'GET',
                 response.status_code if response is not None else '',
                 uri, Assertion.REQ_GET_COLLECTION_COUNT_PROP_REQUIRED, msg)
         return
 
-    data = response.json()
+    data = utils.get_response_json(response)
     if 'Members@odata.count' in data:
         count = data.get('Members@odata.count')
         if not isinstance(count, int):
             msg = ('The count property was present but the type was %s; '
                    'expected int' % count.__class__.__name__)
             sut.log(Result.FAIL, 'GET', response.status_code, uri,
                     Assertion.REQ_GET_COLLECTION_COUNT_PROP_REQUIRED, msg)
@@ -354,15 +354,15 @@
         msg = ('Successful response for GET request to URI %s not found; '
                'unable to test this assertion' % uri)
         sut.log(Result.NOT_TESTED, 'GET',
                 response.status_code if response is not None else '',
                 uri, Assertion.REQ_GET_COLLECTION_COUNT_PROP_TOTAL, msg)
         return
 
-    data = response.json()
+    data = utils.get_response_json(response)
     if 'Members@odata.count' not in data:
         msg = ('The collection resource at URI %s did not include the '
                'required count property' % uri)
         sut.log(Result.FAIL, 'GET', response.status_code, uri,
                 Assertion.REQ_GET_COLLECTION_COUNT_PROP_TOTAL, msg)
         return
 
@@ -528,15 +528,15 @@
     """Perform tests for Assertion.REQ_QUERY_UNSUPPORTED_PARAMS_EXT_ERROR."""
 
     # Removing test for now; there are no standard messages that allow a service to specify the query parameter not supported
 
     """
     if ('application/json' in response.headers.get('Content-Type', '') and
             '@Message.ExtendedInfo' in response.text):
-        data = response.json()
+        data = utils.get_response_json(response)
         if utils.is_text_in_extended_error('rpvunknown', data):
             sut.log(Result.PASS, 'GET', response.status_code, uri,
                     Assertion.REQ_QUERY_UNSUPPORTED_PARAMS_EXT_ERROR,
                     'Test passed')
         else:
             msg = ('The response contained an extended error, but the '
                    'unsupported query parameter $rpvunknown was not '
@@ -629,14 +629,30 @@
     else:
         msg = ('HEAD request to uri %s failed with status %s'
                % (uri, response.status_code))
         sut.log(Result.FAIL, 'HEAD', response.status_code, uri,
                 Assertion.REQ_HEAD_DIFFERS_FROM_GET, msg)
 
 
+def test_data_mod_not_supported(sut: SystemUnderTest):
+    """Perform tests for Assertion.REQ_DATA_MOD_NOT_SUPPORTED."""
+    for uri, response in sut.get_all_responses(request_type=RequestType.UNSUPPORTED_REQ):
+        if response.request.method == 'FAKEMETHODFORTEST':
+            # Not applicable for this clause; skip
+            continue
+        if response.status_code == requests.codes.METHOD_NOT_ALLOWED:
+            sut.log(Result.PASS, response.request.method, response.status_code, uri,
+                    Assertion.REQ_DATA_MOD_NOT_SUPPORTED, 'Test passed')
+        else:
+            msg = ('The service response returned status code %s; expected %s'
+                   % (response.status_code, requests.codes.METHOD_NOT_ALLOWED))
+            sut.log(Result.FAIL, response.request.method, response.status_code, uri,
+                    Assertion.REQ_DATA_MOD_NOT_SUPPORTED, msg)
+
+
 def test_data_mod_errors(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_DATA_MOD_ERRORS."""
     found_error = False
     for uri, response in sut.get_responses_by_method('POST').items():
         if (not response.ok and
                 response.status_code != requests.codes.METHOD_NOT_ALLOWED):
             found_error = True
@@ -661,15 +677,15 @@
 def test_patch_mixed_props(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_PATCH_MIXED_PROPS."""
     found_response = False
     for uri, response in sut.get_responses_by_method(
             'PATCH', request_type=RequestType.PATCH_MIXED_PROPS).items():
         found_response = True
         if response.status_code == requests.codes.OK:
-            data = response.json()
+            data = utils.get_response_json(response)
             if '@odata.id' in data:
                 if '@Message.ExtendedInfo' in data:
                     sut.log(Result.PASS, 'PATCH', response.status_code, uri,
                             Assertion.REQ_PATCH_MIXED_PROPS, 'Test passed')
                 else:
                     msg = ('The service response did not include a message '
                            'annotation that lists the non-updatable '
@@ -702,15 +718,15 @@
 def test_patch_bad_prop(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_PATCH_BAD_PROP."""
     found_response = False
     for uri, response in sut.get_responses_by_method(
             'PATCH', request_type=RequestType.PATCH_BAD_PROP).items():
         found_response = True
         if response.status_code == requests.codes.BAD_REQUEST:
-            data = response.json()
+            data = utils.get_response_json(response)
             if ('error' in data and
                     utils.is_text_in_extended_error('BogusProp', data)):
                 sut.log(Result.PASS, 'PATCH', response.status_code, uri,
                         Assertion.REQ_PATCH_BAD_PROP, 'Test passed')
             else:
                 msg = ('The service response did not include a message '
                        'that lists the non-updatable property; extended '
@@ -728,66 +744,22 @@
     if not found_response:
         msg = ('No PATCH responses found for this condition; unable to test '
                'this assertion')
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.REQ_PATCH_BAD_PROP, msg)
 
 
-def test_patch_ro_resource(sut: SystemUnderTest):
-    """Perform tests for Assertion.REQ_PATCH_RO_RESOURCE."""
-    found_response = False
-    for uri, response in sut.get_responses_by_method(
-            'PATCH', request_type=RequestType.PATCH_RO_RESOURCE).items():
-        found_response = True
-        if response.status_code == requests.codes.METHOD_NOT_ALLOWED:
-            sut.log(Result.PASS, 'PATCH', response.status_code, uri,
-                    Assertion.REQ_PATCH_RO_RESOURCE, 'Test passed')
-        else:
-            msg = ('The service response returned status code %s; expected %s'
-                   % (response.status_code, requests.codes.METHOD_NOT_ALLOWED))
-            sut.log(Result.FAIL, 'PATCH', response.status_code, uri,
-                    Assertion.REQ_PATCH_RO_RESOURCE, msg)
-
-    if not found_response:
-        msg = ('No PATCH responses found for this condition; unable to test '
-               'this assertion')
-        sut.log(Result.NOT_TESTED, '', '', '',
-                Assertion.REQ_PATCH_RO_RESOURCE, msg)
-
-
-def test_patch_collection(sut: SystemUnderTest):
-    """Perform tests for Assertion.REQ_PATCH_COLLECTION."""
-    found_response = False
-    for uri, response in sut.get_responses_by_method(
-            'PATCH', request_type=RequestType.PATCH_COLLECTION).items():
-        found_response = True
-        if response.status_code == requests.codes.METHOD_NOT_ALLOWED:
-            sut.log(Result.PASS, 'PATCH', response.status_code, uri,
-                    Assertion.REQ_PATCH_COLLECTION, 'Test passed')
-        else:
-            msg = ('The service response returned status code %s; expected %s'
-                   % (response.status_code, requests.codes.METHOD_NOT_ALLOWED))
-            sut.log(Result.FAIL, 'PATCH', response.status_code, uri,
-                    Assertion.REQ_PATCH_COLLECTION, msg)
-
-    if not found_response:
-        msg = ('No PATCH responses found for this condition; unable to test '
-               'this assertion')
-        sut.log(Result.NOT_TESTED, '', '', '',
-                Assertion.REQ_PATCH_COLLECTION, msg)
-
-
 def test_patch_odata_props(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_PATCH_ODATA_PROPS."""
     found_response = False
     for uri, response in sut.get_responses_by_method(
             'PATCH', request_type=RequestType.PATCH_ODATA_PROPS).items():
         found_response = True
         if response.status_code == requests.codes.BAD_REQUEST:
-            data = response.json()
+            data = utils.get_response_json(response)
             if ('error' in data and 'NoOperation' in
                     utils.get_extended_info_message_keys(data)):
                 sut.log(Result.PASS, 'PATCH', response.status_code, uri,
                         Assertion.REQ_PATCH_ODATA_PROPS, 'Test passed')
             else:
                 msg = ('The service response did not include the NoOperation '
                        'message from the Base Message Registry; extended '
@@ -818,15 +790,20 @@
 
 def patch_array_save(sut: SystemUnderTest):
     """Save the original array, if found."""
     array = None
     if sut.mgr_net_proto_uri:
         response = sut.get_response('GET', sut.mgr_net_proto_uri)
         if response is not None and response.ok:
-            a = response.json().get('NTP', {}).get('NTPServers', None)
+            try:
+                a = utils.get_response_json(response).get('NTP', {}).get('NTPServers', None)
+            except:
+                logging.error('%s response does not match schema definition'
+                              % (sut.mgr_net_proto_uri))
+                return None
             if isinstance(a, list):
                 array = a
     return array
 
 
 def test_patch_array_element_remove(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_PATCH_ARRAY_ELEMENT_REMOVE."""
@@ -850,18 +827,22 @@
     headers = utils.get_etag_header(sut, sut.session, uri)
     response = sut.patch(uri, json=payload1, headers=headers)
     if response.ok:
         headers = utils.get_etag_header(sut, sut.session, uri)
         response = sut.patch(uri, json=payload2, headers=headers)
         if response.ok:
             get_resp = sut.session.get(sut.rhost + uri)
-            if get_resp.ok:
-                array = get_resp.json().get('NTP', {}).get('NTPServers', None)
-            else:
-                array = response.json().get('NTP', {}).get('NTPServers', None)
+            try:
+                if get_resp.ok:
+                    array = utils.get_response_json(get_resp).get('NTP', {}).get('NTPServers', None)
+                else:
+                    array = utils.get_response_json(response).get('NTP', {}).get('NTPServers', None)
+            except:
+                logging.error('%s response does not match schema definition' % (uri))
+                array = None
             if isinstance(array, list):
                 if 'time-a-b.nist.gov' in array:
                     msg = ('Array element %s was not removed; resource: %s; '
                            'PATCH payload: %s; resulting array: %s' %
                            ('time-a-b.nist.gov', payload1,
                             payload2, array))
                     sut.log(Result.FAIL, 'PATCH', response.status_code, uri,
@@ -913,18 +894,22 @@
     headers = utils.get_etag_header(sut, sut.session, uri)
     response = sut.patch(uri, json=payload1, headers=headers)
     if response.ok:
         headers = utils.get_etag_header(sut, sut.session, uri)
         response = sut.patch(uri, json=payload2, headers=headers)
         if response.ok:
             get_resp = sut.session.get(sut.rhost + uri)
-            if get_resp.ok:
-                array = get_resp.json().get('NTP', {}).get('NTPServers', None)
-            else:
-                array = response.json().get('NTP', {}).get('NTPServers', None)
+            try:
+                if get_resp.ok:
+                    array = utils.get_response_json(get_resp).get('NTP', {}).get('NTPServers', None)
+                else:
+                    array = utils.get_response_json(response).get('NTP', {}).get('NTPServers', None)
+            except:
+                logging.error('%s response does not match schema definition' % (uri))
+                array = None
             if isinstance(array, list):
                 if 'time-a-b.nist.gov' in array:
                     sut.log(Result.PASS, 'PATCH', response.status_code, uri,
                             Assertion.REQ_PATCH_ARRAY_ELEMENT_UNCHANGED,
                             'Test passed')
                 else:
                     missing = []
@@ -984,18 +969,22 @@
     headers = utils.get_etag_header(sut, sut.session, uri)
     response = sut.patch(uri, json=payload1, headers=headers)
     if response.ok:
         headers = utils.get_etag_header(sut, sut.session, uri)
         response = sut.patch(uri, json=payload2, headers=headers)
         if response.ok:
             get_resp = sut.session.get(sut.rhost + uri)
-            if get_resp.ok:
-                array = get_resp.json().get('NTP', {}).get('NTPServers', None)
-            else:
-                array = response.json().get('NTP', {}).get('NTPServers', None)
+            try:
+                if get_resp.ok:
+                    array = utils.get_response_json(get_resp).get('NTP', {}).get('NTPServers', None)
+                else:
+                    array = utils.get_response_json(response).get('NTP', {}).get('NTPServers', None)
+            except:
+                logging.error('%s response does not match schema definition' % (uri))
+                array = None
             if isinstance(array, list):
                 # Remove trailing "null" instance; services might implement
                 # this as a fixed array and show the array size by padding with
                 # null entries
                 while array and array[-1] is None:
                     array.pop()
                 if array == expected_array:
@@ -1042,19 +1031,14 @@
     response = sut.patch(uri, json=payload, headers=headers)
     if not response.ok:
         logging.warning('Attempt to PATCH %s to restore the original '
                         'NTPServers array failed with status %s; PATCH '
                         'payload: %s' % (uri, response.status_code, payload))
 
 
-def test_put_not_implemented(sut: SystemUnderTest):
-    """Perform tests for Assertion.REQ_PUT_NOT_IMPLEMENTED."""
-    # TODO(bdodd): Need a good resource to try to replace
-
-
 def test_post_create_via_collection(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_POST_CREATE_VIA_COLLECTION."""
     response = sut.get_response('POST', sut.sessions_uri)
     if response is None:
         msg = ('Not response found for POST to Sessions URI; unable to test '
                'this assertion')
         sut.log(Result.NOT_TESTED, 'POST', '', sut.sessions_uri,
@@ -1123,65 +1107,14 @@
                'extended error: %s' %
                (uri, response.status_code, utils.get_extended_error(response)))
         sut.log(Result.FAIL, 'POST', response.status_code, uri,
                 Assertion.REQ_POST_CREATE_TO_MEMBERS_PROP,
                 msg)
 
 
-def test_post_create_not_supported(sut: SystemUnderTest):
-    """Perform tests for Assertion.REQ_POST_CREATE_NOT_SUPPORTED."""
-    response = sut.get_response('POST', sut.accounts_uri)
-    if response is None:
-        msg = ('No response found for POST to Accounts URI; unable to test '
-               'this assertion')
-        sut.log(Result.NOT_TESTED, 'POST', '', sut.accounts_uri,
-                Assertion.REQ_POST_CREATE_NOT_SUPPORTED, msg)
-    elif response.ok:
-        sut.log(Result.PASS, 'POST', response.status_code, sut.accounts_uri,
-                Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
-                'Service supports creation of resources')
-    elif response.status_code == requests.codes.METHOD_NOT_ALLOWED:
-        sut.log(Result.PASS, 'POST', response.status_code, sut.accounts_uri,
-                Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
-                'Test passed')
-    else:
-        try:
-            allow = sut.get_response('GET', sut.accounts_uri).headers.get('Allow')
-        except:
-            allow = None
-        if allow:
-            if 'POST' in allow.upper():
-                msg = ('POST request to URI %s failed with %s; extended '
-                       'error: %s; GET response contains an Allow header '
-                       'with POST specified' %
-                       (sut.accounts_uri, response.status_code,
-                        utils.get_extended_error(response)))
-                sut.log(Result.WARN, 'POST', response.status_code,
-                        sut.accounts_uri,
-                        Assertion.REQ_POST_CREATE_NOT_SUPPORTED, msg)
-            else:
-                msg = ('POST request to URI %s failed with %s; expected %s; '
-                       'extended error: %s' %
-                       (sut.accounts_uri, response.status_code,
-                        requests.codes.METHOD_NOT_ALLOWED,
-                        utils.get_extended_error(response)))
-                sut.log(Result.FAIL, 'POST', response.status_code,
-                        sut.accounts_uri,
-                        Assertion.REQ_POST_CREATE_NOT_SUPPORTED, msg)
-        else:
-            msg = ('POST request to URI %s failed with %s; expected %s; '
-                   'extended error: %s; GET response does not contain an '
-                   'Allow header to verify' %
-                   (sut.accounts_uri, response.status_code,
-                    requests.codes.METHOD_NOT_ALLOWED,
-                    utils.get_extended_error(response)))
-            sut.log(Result.WARN, 'POST', response.status_code,
-                    sut.accounts_uri, Assertion.REQ_POST_CREATE_NOT_SUPPORTED,
-                    msg)
-
 def test_post_create_not_idempotent(sut: SystemUnderTest):
     """Perform tests for Assertion.REQ_POST_CREATE_NOT_IDEMPOTENT."""
     uri = sut.sessions_uri
     payload = {
         'UserName': sut.username,
         'Password': sut.password
     }
@@ -1258,54 +1191,14 @@
                     Assertion.REQ_DELETE_METHOD_REQUIRED, msg)
         else:
             msg = 'No DELETE responses found; unable to test this assertion'
             sut.log(Result.NOT_TESTED, 'DELETE', '', '',
                     Assertion.REQ_DELETE_METHOD_REQUIRED, msg)
 
 
-def test_delete_non_deletable_resource(sut: SystemUnderTest):
-    """Perform tests for Assertion.REQ_DELETE_NON_DELETABLE_RESOURCE."""
-    passed = False
-    warn_uri, warn_response = None, None
-    fail_uri, fail_response = None, None
-    for uri, response in sut.get_responses_by_method('DELETE',
-                                                     request_type=RequestType.UNSUPPORTED_REQ).items():
-        if response.status_code == requests.codes.METHOD_NOT_ALLOWED:
-            sut.log(Result.PASS, 'DELETE', response.status_code, uri,
-                    Assertion.REQ_DELETE_NON_DELETABLE_RESOURCE, 'Test passed')
-            passed = True
-            break
-        elif not response.ok:
-            warn_uri, warn_response = uri, response
-        else:
-            fail_uri, fail_response = uri, response
-
-    if not passed:
-        if warn_uri or fail_uri:
-            if fail_uri:
-                msg = ('DELETE request for resource %s failed with status %s; '
-                       'extended error: %s' %
-                       (fail_uri, fail_response.status_code,
-                        utils.get_extended_error(fail_response)))
-                sut.log(Result.FAIL, 'DELETE', fail_response.status_code, fail_uri,
-                        Assertion.REQ_DELETE_NON_DELETABLE_RESOURCE, msg)
-            else:
-                msg = ('DELETE request for resource %s failed with status %s; '
-                       'extended error: %s' %
-                       (warn_uri, warn_response.status_code,
-                        utils.get_extended_error(warn_response)))
-                sut.log(Result.WARN, 'DELETE', warn_response.status_code, warn_uri,
-                        Assertion.REQ_DELETE_NON_DELETABLE_RESOURCE, msg)
-        else:
-            msg = ('No failed DELETE responses found; unable to test this '
-                   'assertion')
-            sut.log(Result.NOT_TESTED, 'DELETE', '', '',
-                    Assertion.REQ_DELETE_NON_DELETABLE_RESOURCE, msg)
-
-
 def test_request_headers(sut: SystemUnderTest):
     """Perform tests from the 'Request headers' sub-section of the spec."""
     test_accept_header(sut)
     test_authorization_header(sut)
     test_content_type_header(sut)
     test_host_header(sut)
     test_if_match_header(sut)
@@ -1346,23 +1239,22 @@
     """Perform tests from the 'HEAD' sub-section of the spec."""
     test_head_differ_from_get(sut)
 
 
 def test_data_modification(sut: SystemUnderTest):
     """Perform tests from the 'Data modification requests' sub-section of the
     spec."""
+    test_data_mod_not_supported(sut)
     test_data_mod_errors(sut)
 
 
 def test_patch_update(sut: SystemUnderTest):
     """Perform tests from the 'PATCH (update)' sub-section of the spec."""
     test_patch_mixed_props(sut)
     test_patch_bad_prop(sut)
-    test_patch_ro_resource(sut)
-    test_patch_collection(sut)
     test_patch_odata_props(sut)
 
 
 def test_patch_array_props(sut: SystemUnderTest):
     """Perform tests from the 'PATCH on array properties' sub-section of the
     spec."""
     orig_array = patch_array_save(sut)
@@ -1372,30 +1264,27 @@
         test_patch_array_operations_order(sut)
         test_patch_array_truncate(sut)
         patch_array_restore(sut, orig_array)
 
 
 def test_put(sut: SystemUnderTest):
     """Perform tests from the 'PUT (replace)' sub-section of the spec."""
-    test_put_not_implemented(sut)
 
 
 def test_post_create(sut: SystemUnderTest):
     """Perform tests from the 'POST (create)' sub-section of the spec."""
     test_post_create_via_collection(sut)
     test_post_create_uri_in_location_hdr(sut)
     test_post_create_to_members_prop(sut)
-    test_post_create_not_supported(sut)
     test_post_create_not_idempotent(sut)
 
 
 def test_delete(sut: SystemUnderTest):
     """Perform tests from the 'DELETE (delete)' sub-section of the spec."""
     test_delete_method_required(sut)
-    test_delete_non_deletable_resource(sut)
 
 
 def test_post_action(sut: SystemUnderTest):
     """Perform tests from the 'POST (Action)' sub-section of the spec."""
     # NOTE(bdodd): Actions better tested in the Redfish-Usecase-Checkers
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_responses.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/service_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
             sut.log(Result.FAIL, response.request.method,
                     response.status_code, uri, assertion, msg)
 
 
 def test_allow_header_method_not_allowed(sut: SystemUnderTest):
     """Perform tests for Assertion.RESP_HEADERS_ALLOW_METHOD_NOT_ALLOWED."""
     found_method_not_allowed = False
-    for req_type in [RequestType.NORMAL, RequestType.PATCH_COLLECTION,
-                     RequestType.PATCH_RO_RESOURCE, RequestType.UNSUPPORTED_REQ]:
+    for req_type in [RequestType.NORMAL, RequestType.UNSUPPORTED_REQ]:
         for uri, response in sut.get_all_responses(request_type=req_type):
             if response.status_code == requests.codes.METHOD_NOT_ALLOWED:
                 found_method_not_allowed = True
                 val = response.headers.get('Allow')
                 if val:
                     msg = 'Test passed for header %s: %s' % ('Allow', val)
                     sut.log(Result.PASS, response.request.method,
@@ -195,15 +194,15 @@
         base = base[:-5]
     base = base.split('.')
     if len(base) == 2 and base[1].startswith('v'):
         ver = base[1]
 
     # get the version from the @odata.type
     ot_ver = None
-    data = response.json()
+    data = utils.get_response_json(response)
     odata_type = data.get('@odata.type')
     if odata_type:
         t = odata_type.lstrip('#').split('.')
         if len(t) == 3:
             ot_ver = t[1]
 
     if ver:
@@ -295,15 +294,15 @@
                       Assertion.RESP_HEADERS_ODATA_VERSION)
 
 def test_www_authenticate_requirement(sut: SystemUnderTest):
     """Check for HTTPBasicAuth Property"""
     response = sut.get_response('GET', sut.account_service_uri)
 
     if (response is not None and response.ok):
-        data = response.json()
+        data = utils.get_response_json(response)
         key = 'HTTPBasicAuth'
         if key in data:
             if data[key] != "Enabled":
                 #  could be either Disabled or Unadvertised
                 return False
             else:
                 return True
@@ -392,15 +391,15 @@
                         'application/json'):
                     msg = ('The response payload type was %s; expected %s' %
                            (response.headers.get('Content-Type', '<missing>'),
                             'application/json'))
                     sut.log(Result.FAIL, response.request.method,
                             response.status_code, uri, assertion, msg)
                     continue
-                data = response.json()
+                data = utils.get_response_json(response)
                 if 'error' in data:
                     if 'code' in data['error'] and 'message' in data['error']:
                         sut.log(Result.PASS, response.request.method,
                                 response.status_code, uri, assertion,
                                 'Test passed')
                     else:
                         msg = ('The required "code" or "message" properties '
@@ -544,15 +543,15 @@
                 Assertion.RESP_ODATA_SERVICE_CONTEXT, msg)
     elif not response.ok:
         msg = ('%s request to URI %s failed with status %s'
                % ('GET', uri, response.status_code))
         sut.log(Result.FAIL, 'GET', response.status_code, uri,
                 Assertion.RESP_ODATA_SERVICE_CONTEXT, msg)
     else:
-        data = response.json()
+        data = utils.get_response_json(response)
         context = data.get('@odata.context')
         if context == '/redfish/v1/$metadata':
             sut.log(Result.PASS, 'GET', response.status_code, uri,
                     Assertion.RESP_ODATA_SERVICE_CONTEXT, 'Test passed')
         else:
             msg = ('The @odata.context property for the OData service '
                    'document is %s; expected %s' %
@@ -572,15 +571,15 @@
                 Assertion.RESP_ODATA_SERVICE_VALUE_PROP, msg)
     elif not response.ok:
         msg = ('%s request to URI %s failed with status %s'
                % ('GET', uri, response.status_code))
         sut.log(Result.FAIL, 'GET', response.status_code, uri,
                 Assertion.RESP_ODATA_SERVICE_VALUE_PROP, msg)
     else:
-        data = response.json()
+        data = utils.get_response_json(response)
         value = data.get('value')
         if value is not None:
             if isinstance(value, list):
                 sut.log(Result.PASS, 'GET', response.status_code, uri,
                         Assertion.RESP_ODATA_SERVICE_VALUE_PROP, 'Test passed')
             else:
                 msg = ('The value property for the OData service '
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/sessions.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/sessions.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/system_under_test.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/system_under_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # https://github.com/DMTF/Redfish-Protocol-Validator/blob/main/LICENSE.md
 
 import logging
 from urllib.parse import urlparse
 
 import requests
 
-from redfish_protocol_validator.utils import redfish_version_to_tuple, poll_task
+from redfish_protocol_validator.utils import redfish_version_to_tuple, poll_task, get_response_json
 from redfish_protocol_validator.constants import RequestType, Result
 
 
 class SystemUnderTest(object):
     def __init__(self, rhost, username, password, verify=True):
         self._rhost = rhost
         self._username = username
@@ -424,24 +424,24 @@
 
         :param headers: HTTP headers to pass to the GET requests
         :return: the Sessions URI
         """
         r = requests.get(self.rhost + '/redfish/v1/', headers=headers,
                          verify=self.verify)
         if r.status_code == requests.codes.OK:
-            data = r.json()
+            data = get_response_json(r)
             if 'Links' in data and 'Sessions' in data['Links']:
                 return data['Links']['Sessions']['@odata.id']
             elif 'SessionService' in data:
                 uri = data['SessionService']['@odata.id']
                 r = requests.get(self.rhost + uri, headers=headers,
                                  auth=(self.username, self.password),
                                  verify=self.verify)
                 if r.status_code == requests.codes.OK:
-                    data = r.json()
+                    data = get_response_json(r)
                     if 'Sessions' in data:
                         return data['Sessions']['@odata.id']
         return '/redfish/v1/SessionService/Sessions'
 
     def post(self, uri, json=None, headers=None, session=None):
         """
         Performs a POST request with task polling
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator/utils.py` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,23 +47,23 @@
 
 def get_response_etag(response: requests.Response):
     etag = None
     if response.ok:
         etag = response.headers.get('ETag')
         if not etag:
             if get_response_media_type(response) == 'application/json':
-                data = response.json()
+                data = get_response_json(response)
                 etag = data.get('@odata.etag')
     return etag
 
 
 def get_extended_error(response: requests.Response):
     message = ''
     try:
-        data = response.json()
+        data = get_response_json(response)
         if 'error' in data:
             error = data['error']
             if 'message' in error:
                 message = error['message']
             elif 'code' in error:
                 message = error['code']
             ext_info = error.get('@Message.ExtendedInfo', [])
@@ -73,14 +73,30 @@
                 elif 'MessageId' in ext_info[0]:
                     message = ext_info[0]['MessageId']
     except Exception:
         pass
     return message
 
 
+def get_response_json(response: requests.Response):
+    try:
+        data = response.json()
+        if not isinstance(data, dict):
+            data = {}
+            logging.error('%s on %s did not return a JSON object; assuming '
+                          'an empty object' % (response.request.method,
+                                               response.request.path_url))
+    except:
+        data = {}
+        logging.error('%s on %s did not return valid JSON; assuming '
+                      'an empty object' % (response.request.method,
+                                           response.request.path_url))
+    return data
+
+
 def get_extended_info_message_keys(body: dict):
     data = []
     if 'error' in body and '@Message.ExtendedInfo' in body['error']:
         data = body['error']['@Message.ExtendedInfo']
     elif '@Message.ExtendedInfo' in body:
         data = body['@Message.ExtendedInfo']
     return {d['MessageId'].split('.')[-1] for d in data if 'MessageId' in d}
@@ -138,26 +154,26 @@
     event_dest_uri = None
     subs = set()
     try:
         # get the "before" set of EventDestination URIs
         if sut.subscriptions_uri:
             r = sut.session.get(sut.rhost + sut.subscriptions_uri)
             if r.status_code == requests.codes.OK:
-                data = r.json()
+                data = get_response_json(r)
                 subs = set([m.get('@odata.id') for m in data.get('Members', [])
                             if '@odata.id' in m])
 
         if sut.server_sent_event_uri:
             response = sut.session.get(sut.rhost + sut.server_sent_event_uri,
                                        stream=True)
         if response is not None and response.ok and sut.subscriptions_uri:
             # get the "after" set of EventDestination URIs
             r = sut.session.get(sut.rhost + sut.subscriptions_uri)
             if r.status_code == requests.codes.OK:
-                data = r.json()
+                data = get_response_json(r)
                 new_subs = set([m.get('@odata.id') for m in
                                 data.get('Members', []) if '@odata.id' in m])
                 diff = new_subs.difference(subs)
                 if len(diff) == 1:
                     event_dest_uri = diff.pop()
                 elif len(diff) == 0:
                     logging.debug('No EventDestination resource created when '
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/PKG-INFO` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_protocol_validator
-Version: 1.2.4
+Version: 1.2.5
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/SOURCES.txt` & `redfish_protocol_validator-1.2.5/redfish_protocol_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.4/setup.py` & `redfish_protocol_validator-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_protocol_validator",
-    version="1.2.4",
+    version="1.2.5",
     description="Redfish Protocol Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

