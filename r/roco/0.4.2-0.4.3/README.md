# Comparing `tmp/roco-0.4.2.tar.gz` & `tmp/roco-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roco-0.4.2.tar", max compression
+gzip compressed data, was "roco-0.4.3.tar", max compression
```

## Comparing `roco-0.4.2.tar` & `roco-0.4.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10231 2024-03-26 06:21:04.206698 roco-0.4.2/LICENSE
--rw-r--r--   0        0        0     1689 2024-03-26 06:21:04.206698 roco-0.4.2/README.md
--rw-r--r--   0        0        0      744 2024-03-26 06:21:04.206698 roco-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 06:21:04.206698 roco-0.4.2/roco/__init__.py
--rw-r--r--   0        0        0      426 2024-03-26 06:21:04.206698 roco-0.4.2/roco/bin/cli.py
--rw-r--r--   0        0        0     1387 2024-03-26 06:21:04.206698 roco-0.4.2/roco/config.py
--rw-r--r--   0        0        0      572 2024-03-26 06:21:04.206698 roco-0.4.2/roco/main.py
--rw-r--r--   0        0        0      459 2024-03-26 06:21:04.206698 roco-0.4.2/roco/templates/runtime-config.js.jinja2
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 roco-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10207 2024-05-03 04:19:43.281459 roco-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1776 2024-05-03 04:19:43.281459 roco-0.4.3/README.md
+-rw-r--r--   0        0        0      743 2024-05-03 04:19:43.281459 roco-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 04:19:43.281459 roco-0.4.3/roco/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-03 04:19:43.281459 roco-0.4.3/roco/bin/cli.py
+-rw-r--r--   0        0        0      874 2024-05-03 04:19:43.281459 roco-0.4.3/roco/config.py
+-rw-r--r--   0        0        0      572 2024-05-03 04:19:43.281459 roco-0.4.3/roco/main.py
+-rw-r--r--   0        0        0      527 2024-05-03 04:19:43.281459 roco-0.4.3/roco/templates/runtime-config.js.jinja2
+-rw-r--r--   0        0        0     2617 1970-01-01 00:00:00.000000 roco-0.4.3/PKG-INFO
```

### Comparing `roco-0.4.2/LICENSE` & `roco-0.4.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
-   Copyright 2020-2024 Eugen Ciur <eugen@papermerge.com>
+   Copyright (c) 2020 Eugen Ciur
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
       "License" shall mean the terms and conditions for use, reproduction,
       and distribution as defined by Sections 1 through 9 of this document.
```

### Comparing `roco-0.4.2/README.md` & `roco-0.4.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Roco - Runtime config generator
 
-Command line utility tool which prints to the standard output javascript valid 
+Command line utility which prints to the standard output javascript valid 
 text generated from environment variables.
 
 For example, given following environment variables:
 
     PAPERMERGE__AUTH__OIDC_CLIENT_ID=papermerge
     PAPERMERGE__AUTH__OIDC_AUTHORIZE_URL=http://keycloak.trusel.net:8080/realms/myrealm/protocol/openid-connect/auth
     PAPERMERGE__AUTH__OIDC_REDIRECT_URL=http://demo.trusel.net:12000/oidc/callback
@@ -46,8 +46,10 @@
 The above command will also show the env var prefix i.e. `PAPERMERGE__AUTH__`.
 
 Roco reads from following environment variables:
 
 * `PAPERMERGE__AUTH__OIDC_AUTHORIZE_URL`
 * `PAPERMERGE__AUTH__OIDC_CLIENT_ID`
 * `PAPERMERGE__AUTH__OIDC_REDIRECT_URL`
-* `PAPERMERGE__AUTH__LDAP_URL`
+* `PAPERMERGE__AUTH__OIDC_LOGOUT_URL`
+* `PAPERMERGE__AUTH__OIDC_POST_LOGOUT_REDIRECT_URL`
+* `PAPERMERGE__AUTH__OIDC_SCOPE`
```

### Comparing `roco-0.4.2/pyproject.toml` & `roco-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "roco"
-version = "0.4.2"
+version = "0.4.3"
 description = "Runtime Config Generator"
 authors = ["Eugen Ciur <eugen@papermerge.com>"]
 readme = "README.md"
 homepage = "https://github.com/papermerge/roco"
 license = "Apache 2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3"
 ]
 
-
 [tool.poetry.dependencies]
 python = "^3.10"
 jinja2 = "^3.1.2"
 typer = "^0.9.0"
 pydantic = "^2.5"
 pydantic-settings = "^2.1.0"
```

### Comparing `roco-0.4.2/roco/config.py` & `roco-0.4.3/roco/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,43 +7,25 @@
 class Settings(BaseSettings):
     model_config = SettingsConfigDict(env_prefix='PAPERMERGE__AUTH__')
 
     oidc_client_id: str | None = None
     oidc_authorize_url: str | None = None
     oidc_redirect_url: str | None = None
     oidc_logout_url: str | None = None
+    oidc_post_logout_redirect_url: str | None = None
     oidc_scope: str = 'openid email'
 
     login_provider: Literal['db', 'ldap'] = 'db'
     remote: bool = False
     remote_logout_endpoint: str | None = None
 
     @field_validator('login_provider')
     @classmethod
     def db_or_ldap(cls, v: str) -> str:
         if os.environ.get('PAPERMERGE__AUTH__LDAP_URL'):
             return 'ldap'
 
         return 'db'
 
-    @model_validator(mode='after')
-    def check_oidc_params(self):
-        three_values = [
-            self.oidc_client_id,
-            self.oidc_authorize_url,
-            self.oidc_redirect_url,
-            self.oidc_logout_url
-        ]
-        count = len([v for v in three_values if v])
-
-        if count not in (0, 4):
-            raise ValueError(
-                'oidc_client_id, oidc_authorize_url, oidc_redirect_url'
-                ' and oidc_logout_url'
-                ' should be either all absent or all present'
-            )
-
-        return self
-
 
 def get_settings():
     return Settings()
```

### Comparing `roco-0.4.2/roco/main.py` & `roco-0.4.3/roco/main.py`

 * *Files identical despite different names*

### Comparing `roco-0.4.2/PKG-INFO` & `roco-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roco
-Version: 0.4.2
+Version: 0.4.3
 Summary: Runtime Config Generator
 Home-page: https://github.com/papermerge/roco
 License: Apache 2.0
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,15 +19,15 @@
 Requires-Dist: pydantic (>=2.5,<3.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Roco - Runtime config generator
 
-Command line utility tool which prints to the standard output javascript valid 
+Command line utility which prints to the standard output javascript valid 
 text generated from environment variables.
 
 For example, given following environment variables:
 
     PAPERMERGE__AUTH__OIDC_CLIENT_ID=papermerge
     PAPERMERGE__AUTH__OIDC_AUTHORIZE_URL=http://keycloak.trusel.net:8080/realms/myrealm/protocol/openid-connect/auth
     PAPERMERGE__AUTH__OIDC_REDIRECT_URL=http://demo.trusel.net:12000/oidc/callback
@@ -69,9 +69,11 @@
 The above command will also show the env var prefix i.e. `PAPERMERGE__AUTH__`.
 
 Roco reads from following environment variables:
 
 * `PAPERMERGE__AUTH__OIDC_AUTHORIZE_URL`
 * `PAPERMERGE__AUTH__OIDC_CLIENT_ID`
 * `PAPERMERGE__AUTH__OIDC_REDIRECT_URL`
-* `PAPERMERGE__AUTH__LDAP_URL`
+* `PAPERMERGE__AUTH__OIDC_LOGOUT_URL`
+* `PAPERMERGE__AUTH__OIDC_POST_LOGOUT_REDIRECT_URL`
+* `PAPERMERGE__AUTH__OIDC_SCOPE`
```

