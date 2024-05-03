# Comparing `tmp/workos-4.5.0.tar.gz` & `tmp/workos-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.5.0.tar", last modified: Wed May  1 20:54:18 2024, max compression
+gzip compressed data, was "workos-4.6.0.tar", last modified: Fri May  3 20:17:54 2024, max compression
```

## Comparing `workos-4.5.0.tar` & `workos-4.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.715914 workos-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 20:54:11.000000 workos-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-01 20:54:18.715914 workos-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-01 20:54:11.000000 workos-4.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:54:18.715914 workos-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-01 20:54:11.000000 workos-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.711914 workos-4.5.0/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-01 20:54:11.000000 workos-4.5.0/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 20:54:11.000000 workos-4.5.0/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-01 20:54:11.000000 workos-4.5.0/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-01 20:54:11.000000 workos-4.5.0/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-01 20:54:11.000000 workos-4.5.0/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 20:54:11.000000 workos-4.5.0/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-01 20:54:11.000000 workos-4.5.0/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-01 20:54:11.000000 workos-4.5.0/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-01 20:54:11.000000 workos-4.5.0/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-01 20:54:11.000000 workos-4.5.0/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-01 20:54:11.000000 workos-4.5.0/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.715914 workos-4.5.0/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-01 20:54:11.000000 workos-4.5.0/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-01 20:54:11.000000 workos-4.5.0/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-05-01 20:54:11.000000 workos-4.5.0/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.715914 workos-4.5.0/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 20:54:11.000000 workos-4.5.0/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-01 20:54:11.000000 workos-4.5.0/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:54:18.711914 workos-4.5.0/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:54:17.000000 workos-4.5.0/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 20:54:18.000000 workos-4.5.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:17:46.000000 workos-4.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-03 20:17:54.251297 workos-4.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 20:17:46.000000 workos-4.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:17:54.255297 workos-4.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-03 20:17:46.000000 workos-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 20:17:46.000000 workos-4.6.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-03 20:17:46.000000 workos-4.6.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-03 20:17:46.000000 workos-4.6.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-03 20:17:46.000000 workos-4.6.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-03 20:17:46.000000 workos-4.6.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-03 20:17:46.000000 workos-4.6.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-03 20:17:46.000000 workos-4.6.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-03 20:17:46.000000 workos-4.6.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-03 20:17:46.000000 workos-4.6.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-03 20:17:46.000000 workos-4.6.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 20:17:46.000000 workos-4.6.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-03 20:17:46.000000 workos-4.6.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-03 20:17:46.000000 workos-4.6.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41222 2024-05-03 20:17:46.000000 workos-4.6.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-03 20:17:46.000000 workos-4.6.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-03 20:17:46.000000 workos-4.6.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:17:54.251297 workos-4.6.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:17:52.000000 workos-4.6.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 20:17:54.000000 workos-4.6.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.5.0/LICENSE` & `workos-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/PKG-INFO` & `workos-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.5.0
+Version: 4.6.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.5.0/README.md` & `workos-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/setup.py` & `workos-4.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/audit_logs.py` & `workos-4.6.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/client.py` & `workos-4.6.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/directory_sync.py` & `workos-4.6.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/events.py` & `workos-4.6.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/exceptions.py` & `workos-4.6.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/mfa.py` & `workos-4.6.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/organizations.py` & `workos-4.6.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/passwordless.py` & `workos-4.6.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/portal.py` & `workos-4.6.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/audit_logs_export.py` & `workos-4.6.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/base.py` & `workos-4.6.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/directory_sync.py` & `workos-4.6.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/event.py` & `workos-4.6.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/list.py` & `workos-4.6.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/mfa.py` & `workos-4.6.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/organizations.py` & `workos-4.6.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/passwordless.py` & `workos-4.6.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/sso.py` & `workos-4.6.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/resources/user_management.py` & `workos-4.6.0/workos/resources/user_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,20 +86,39 @@
         "id",
         "email",
         "state",
         "accepted_at",
         "revoked_at",
         "expires_at",
         "token",
+        "accept_invitation_url",
         "organization_id",
         "created_at",
         "updated_at",
     ]
 
 
+class WorkOSMagicAuth(WorkOSBaseResource):
+    """Representation of a MagicAuth object as returned by WorkOS through User Management features.
+
+    Attributes:
+        OBJECT_FIELDS (list): List of fields a WorkOSMagicAuth comprises.
+    """
+
+    OBJECT_FIELDS = [
+        "id",
+        "user_id",
+        "email",
+        "expires_at",
+        "code",
+        "created_at",
+        "updated_at",
+    ]
+
+
 class WorkOSOrganizationMembership(WorkOSBaseResource):
     """Representation of an Organization Membership as returned by WorkOS through User Management features.
 
     Attributes:
         OBJECT_FIELDS (list): List of fields a WorkOSOrganizationMembership comprises.
     """
```

### Comparing `workos-4.5.0/workos/sso.py` & `workos-4.6.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/user_management.py` & `workos-4.6.0/workos/user_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from requests import Request
+from warnings import warn
 import workos
 from workos.resources.list import WorkOSListResource
 from workos.resources.mfa import WorkOSAuthenticationFactorTotp, WorkOSChallenge
 from workos.resources.user_management import (
     WorkOSAuthenticationResponse,
     WorkOSRefreshTokenAuthenticationResponse,
     WorkOSInvitation,
+    WorkOSMagicAuth,
     WorkOSOrganizationMembership,
     WorkOSPasswordChallengeResponse,
     WorkOSUser,
 )
 from workos.utils.pagination_order import Order
 from workos.utils.um_provider_types import UserManagementProviderType
 from workos.utils.request import (
@@ -28,14 +30,16 @@
 ORGANIZATION_MEMBERSHIP_DETAIL_PATH = "user_management/organization_memberships/{0}"
 USER_AUTHORIZATION_PATH = "user_management/authorize"
 USER_AUTHENTICATE_PATH = "user_management/authenticate"
 USER_SEND_PASSWORD_RESET_PATH = "user_management/password_reset/send"
 USER_RESET_PASSWORD_PATH = "user_management/password_reset/confirm"
 USER_SEND_VERIFICATION_EMAIL_PATH = "user_management/users/{0}/email_verification/send"
 USER_VERIFY_EMAIL_CODE_PATH = "user_management/users/{0}/email_verification/confirm"
+MAGIC_AUTH_DETAIL_PATH = "user_management/magic_auth/{0}"
+MAGIC_AUTH_PATH = "user_management/magic_auth"
 USER_SEND_MAGIC_AUTH_PATH = "user_management/magic_auth/send"
 USER_AUTH_FACTORS_PATH = "user_management/users/{0}/auth_factors"
 INVITATION_PATH = "user_management/invitations"
 INVITATION_DETAIL_PATH = "user_management/invitations/{0}"
 INVITATION_REVOKE_PATH = "user_management/invitations/{0}/revoke"
 
 RESPONSE_LIMIT = 10
@@ -868,24 +872,82 @@
             headers=headers,
             params=payload,
             token=workos.api_key,
         )
 
         return WorkOSUser.construct_from_response(response["user"]).to_dict()
 
+    def get_magic_auth(self, magic_auth_id):
+        """Get the details of a Magic Auth object.
+
+        Args:
+            magic_auth_id (str) -  The unique ID of the Magic Auth object.
+
+        Returns:
+            dict: MagicAuth response from WorkOS.
+        """
+        headers = {}
+
+        response = self.request_helper.request(
+            MAGIC_AUTH_DETAIL_PATH.format(magic_auth_id),
+            method=REQUEST_METHOD_GET,
+            headers=headers,
+            token=workos.api_key,
+        )
+
+        return WorkOSMagicAuth.construct_from_response(response).to_dict()
+
+    def create_magic_auth(
+        self,
+        email,
+        invitation_token=None,
+    ):
+        """Creates a Magic Auth code challenge that can be sent to a user's email for authentication.
+
+        Args:
+            email: The email address of the user.
+            invitation_token: The token of an Invitation, if required. (Optional)
+
+        Returns:
+            dict: MagicAuth response from WorkOS.
+        """
+        headers = {}
+
+        params = {
+            "email": email,
+            "invitation_token": invitation_token,
+        }
+
+        response = self.request_helper.request(
+            MAGIC_AUTH_PATH,
+            method=REQUEST_METHOD_POST,
+            params=params,
+            headers=headers,
+            token=workos.api_key,
+        )
+
+        return WorkOSMagicAuth.construct_from_response(response).to_dict()
+
     def send_magic_auth_code(
         self,
         email,
     ):
         """Creates a one-time Magic Auth code and emails it to the user.
 
+        Deprecated: Please use `create_magic_auth` instead. This method will be removed in a future major version.
+
         Kwargs:
             email (str): The email address the one-time code will be sent to.
         """
 
+        warn(
+            "'send_magic_auth_code' is deprecated. Please use 'create_magic_auth' instead. This method will be removed in a future major version.",
+            DeprecationWarning,
+        )
+
         headers = {}
 
         payload = {
             "email": email,
         }
 
         response = self.request_helper.request(
```

### Comparing `workos-4.5.0/workos/utils/connection_types.py` & `workos-4.6.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/utils/request.py` & `workos-4.6.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/utils/validation.py` & `workos-4.6.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos/webhooks.py` & `workos-4.6.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.5.0/workos.egg-info/PKG-INFO` & `workos-4.6.0/workos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.5.0
+Version: 4.6.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.5.0/workos.egg-info/SOURCES.txt` & `workos-4.6.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

