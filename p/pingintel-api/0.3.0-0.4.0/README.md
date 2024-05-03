# Comparing `tmp/pingintel_api-0.3.0.tar.gz` & `tmp/pingintel_api-0.4.0.tar.gz`

## Comparing `pingintel_api-0.3.0.tar` & `pingintel_api-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/justfile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/requirements.txt
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/examples/create_propel_api_key.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/examples/fix_sov.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/examples/pingvision_activity.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/examples/test_sov.xlsx
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/__about__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/__init__.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/api_client_base.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/constants.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/sovfixerapi_cmd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/utils.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/pingvision/pingvision_api_client.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/pingvision/types.py
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/src/pingintel_api/sov_fixer/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/tests/tests.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pingintel_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/justfile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/requirements.txt
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/examples/fix_sov.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/examples/pingvision_activity.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/examples/test_sov.xlsx
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/__about__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/__init__.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/api_client_base.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/constants.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/sovfixerapi_cmd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/utils.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/pingvision/pingvision_api_client.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/pingvision/types.py
+-rw-r--r--   0        0        0     8414 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/src/pingintel_api/sov_fixer/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/tests/tests.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pingintel_api-0.4.0/PKG-INFO
```

### Comparing `pingintel_api-0.3.0/examples/test_sov.xlsx` & `pingintel_api-0.4.0/examples/test_sov.xlsx`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.3.0/src/pingintel_api/api_client_base.py` & `pingintel_api-0.4.0/src/pingintel_api/api_client_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,31 @@
-import os, requests
-from typing import overload, IO, TypedDict, NotRequired
-from .utils import log
 import configparser
+import os
+from typing import IO, NotRequired, TypedDict, overload
+
+import requests
+
+from .utils import log
+
+from pingintel_api.__about__ import __version__
 
 
 class APIClientBase:
     api_subdomain: str
-    base_domain: str
+    api_base_domain: str
     auth_token_env_name: str
     product: str
 
     @overload
-    def __init__(self, api_url: str, auth_token=None) -> None: ...
+    def __init__(self, api_url: str, auth_token=None) -> None:
+        """Initialize the API client with an API URL and an optional auth token.
+
+        :param api_url: The URL of the API.  e.g. "https://vision.pingintel.com"
+        """
+        pass
 
     @overload
     def __init__(self, environment: str = "prod", auth_token=None) -> None: ...
 
     def __init__(
         self,
         api_url: str | None = None,
@@ -23,28 +33,36 @@
         auth_token=None,
     ):
         if api_url is None:
             if environment is None:
                 raise ValueError("Need either api_url or environment.")
             api_url = self.get_api_url_by_environment(environment)
 
-        if auth_token is None and environment:
+        if not auth_token and environment:
             auth_token = self.get_auth_token_by_environment(environment)
-        if auth_token is None:
+        if not auth_token:
             auth_token = os.environ.get(self.auth_token_env_name)
-
-        if auth_token is None:
+        if not auth_token:
             config = configparser.ConfigParser()
             config.read(os.path.expanduser("~/.pingintel.ini"))
-            try:
-                auth_token = config.get(self.product, self.auth_token_env_name)
-            except (configparser.NoOptionError, configparser.NoSectionError):
-                pass
+            if environment:
+                serverspace = self.get_serverspace_from_environment(environment)
+                try:
+                    auth_token = config.get(
+                        self.product, f"{self.auth_token_env_name}_{serverspace}"
+                    )
+                except (configparser.NoOptionError, configparser.NoSectionError):
+                    pass
+            if not auth_token:
+                try:
+                    auth_token = config.get(self.product, self.auth_token_env_name)
+                except (configparser.NoOptionError, configparser.NoSectionError):
+                    pass
 
-        if auth_token is None:
+        if not auth_token:
             raise ValueError(
                 f"Need --auth-token or {self.auth_token_env_name} environment variable set."
             )
         assert api_url
         self.api_url = api_url
         self.auth_token = auth_token
         self.environment = environment if api_url is None else None
@@ -56,36 +74,42 @@
 
     def _create_session(self):
         session = requests.Session()
 
         session.headers = {
             "Authorization": f"Token {self.auth_token}",
             "Accept-Encoding": "gzip",
+            "User-Agent": f"pingintel_api/{self.__class__.__name__}/{__version__}",
         }
         return session
 
     def get_api_url_by_environment(self, environment: str) -> str:
         if environment == "prod":
-            return f"https://{self.api_subdomain}.{self.base_domain}"
+            return f"https://{self.api_subdomain}.{self.api_base_domain}"
         elif environment == "prod2":
-            return f"https://{self.api_subdomain}2.{self.base_domain}"
+            return f"https://{self.api_subdomain}2.{self.api_base_domain}"
         elif environment == "prodeu":
-            return f"https://{self.api_subdomain}.eu.{self.base_domain}"
+            return f"https://{self.api_subdomain}.eu.{self.api_base_domain}"
         elif environment == "local":
             return "http://api-local.sovfixer.com"
         else:
-            return f"https://{self.api_subdomain}-{environment}.{self.base_domain}"
+            return f"https://{self.api_subdomain}-{environment}.{self.api_base_domain}"
 
     def get_auth_token_by_environment(self, environment: str) -> str:
+        serverspace = self.get_serverspace_from_environment(environment)
+        auth_token = os.environ.get(f"PING_{serverspace}_AUTH_TOKEN".upper())
+
+    def get_serverspace_from_environment(self, environment: str) -> str:
         if environment in ["staging", "staging2"]:
             serverspace = "stg"
         elif environment in ["prod", "prod2"]:
             serverspace = "prd"
         elif environment in ["prodeu", "prodeu2"]:
             serverspace = "prdeu"
         elif environment in ["dev", "dev2"]:
             serverspace = "dev"
         elif environment in ["local", "local2"]:
             serverspace = "local"
         else:
-            raise ValueError("Unknown environment and missing auth_token.")
-        auth_token = os.environ.get(f"PING_{serverspace}_AUTH_TOKEN".upper())
+            raise ValueError("Unknown environment.")
+
+        return serverspace
```

### Comparing `pingintel_api-0.3.0/src/pingintel_api/sovfixerapi_cmd.py` & `pingintel_api-0.4.0/src/pingintel_api/sovfixerapi_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 #!/usr/bin/env python
 
 # Copyright 2021-2024 Ping Data Intelligence
 
-import base64
-import enum
-import gzip
-import hashlib
-import io
-import json
 import logging
-import os
 import pathlib
 import pprint
-import random
 import time
-import zipfile
 from timeit import default_timer as timer
 
 import click
-import requests
-from requests.exceptions import HTTPError
 
 from pingintel_api import SOVFixerAPIClient
 
 logger = logging.getLogger(__name__)
 
 
 global start_time
@@ -33,24 +22,29 @@
 """
 sovfixerapi.py
 
 Example Python commandline script for using the Ping Data Technologies sovfixer API to process SOVs.
 """
 
 
+@click.group()
+def cli():
+    pass
+
+
 def log(msg):
     global start_time
     if start_time is None:
         start_time = timer()
     elapsed = timer() - start_time
     timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
     click.echo(f"[{timestamp} T+{elapsed:.1f}s] {msg}")
 
 
-@click.command()
+@cli.command()
 @click.argument(
     "filename", nargs=-1, required=True, type=click.Path(exists=True, dir_okay=False)
 )
 @click.option(
     "-e",
     "--environment",
     type=click.Choice(
@@ -96,15 +90,15 @@
 @click.option(
     "--write",
     "--no-write",
     is_flag=True,
     default=False,
     help="If set, actually write the output. Otherwise, download as a test but do not write.",
 )
-def main(
+def fix(
     filename,
     environment,
     document_type,
     auth_token,
     callback_url,
     output_format,
     client_ref,
@@ -122,9 +116,40 @@
             callback_url=callback_url,
             actually_write=write,
             output_formats=output_format,
             client_ref=client_ref,
         )
 
 
+@cli.command()
+@click.option(
+    "-e",
+    "--environment",
+    type=click.Choice(
+        [
+            "staging",
+            "staging2",
+            "prod",
+            "prod2",
+            "prodeu",
+            "prodeu2",
+            "local",
+            "local2",
+            "dev",
+            "dev2",
+        ],
+        case_sensitive=False,
+    ),
+    default="staging",
+)
+@click.option(
+    "--auth-token",
+    help="Provide auth token via --auth-token or SOVFIXER_AUTH_TOKEN environment variable.",
+)
+def activity(environment, auth_token):
+    client = SOVFixerAPIClient(environment=environment, auth_token=auth_token)
+    results = client.list_activity()
+    pprint.pprint(results)
+
+
 if __name__ == "__main__":
-    main()
+    cli()
```

### Comparing `pingintel_api-0.3.0/src/pingintel_api/utils.py` & `pingintel_api-0.4.0/src/pingintel_api/utils.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import requests
 import time
-import click
 from timeit import default_timer as timer
-from requests.exceptions import HTTPError
 
+import click
+import requests
+from requests.exceptions import HTTPError
 
 global start_time
 start_time = None
 
 
 def log(msg):
     global start_time
```

### Comparing `pingintel_api-0.3.0/src/pingintel_api/pingvision/pingvision_api_client.py` & `pingintel_api-0.4.0/src/pingintel_api/pingvision/pingvision_api_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,44 +3,36 @@
 # Copyright 2021-2024 Ping Data Intelligence
 
 import logging
 import os
 import pprint
 import time
 from timeit import default_timer as timer
-from typing import overload, IO, TypedDict, NotRequired
+from typing import IO, NotRequired, TypedDict, overload
+
 import click
 import requests
 
 from pingintel_api.api_client_base import APIClientBase
+
 from .. import constants as c
+from ..utils import is_fileobj, log, raise_for_status
 from . import types as t
-from ..utils import is_fileobj, raise_for_status, log
 
 logger = logging.getLogger(__name__)
 
 
 class PingVisionAPIClient(APIClientBase):
     api_subdomain = "api"
-    base_domain = "vision.pingintel.com"
+    api_base_domain = "vision.pingintel.com"
     auth_token_env_name = "PINGVISION_AUTH_TOKEN"
     product = "pingvision"
 
-    def _create_session(self):
-        session = requests.Session()
-
-        session.headers = {
-            "Authorization": f"Bearer {self.auth_token}",
-            "Accept-Encoding": "gzip",
-        }
-        breakpoint()
-
-        return session
-
-    def list_activity(
+   
+    def list_submission_activity(
         self,
         cursor_id: str | None = None,
         prev_cursor_id: str | None = None,
         page_size: int | None = None,
         fields: list[str] | None = None,
         search: str | None = None,
         organization__short_name: str | None = None,
@@ -59,16 +51,11 @@
         if search:
             data["search"] = search
         if organization__short_name:
             data["organization__short_name"] = organization__short_name
 
         response = self.get(url, data=data)
 
-        if response.status_code == 200:
-            pprint.pprint(response.json())
-        else:
-            pprint.pprint(response.text)
-
         raise_for_status(response)
 
         response_data = response.json()
         return response_data
```

### Comparing `pingintel_api-0.3.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py` & `pingintel_api-0.4.0/src/pingintel_api/sov_fixer/sov_fixer_api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 # Copyright 2021-2024 Ping Data Intelligence
 
 import logging
 import os
 import pprint
 import time
-from typing import overload, IO, TypedDict, NotRequired
+from typing import IO, NotRequired, TypedDict, overload
+
 import click
 import requests
 
 from pingintel_api.api_client_base import APIClientBase
+
 from .. import constants as c
+from ..utils import is_fileobj, log, raise_for_status
 from . import types as t
-from ..utils import is_fileobj, raise_for_status, log
 
 logger = logging.getLogger(__name__)
 
 
 class SOVFixerAPIClient(APIClientBase):
     api_subdomain = "api"
     api_base_domain = "sovfixer.com"
@@ -202,7 +204,41 @@
                     output_path=output_path,
                 )
             return True
         else:
             log("* Parsing failed!  Raw API output:")
             log(response_data)
             return False
+
+    def list_activity(
+        self,
+        cursor_id=None,
+        prev_cursor_id=None,
+        page_size=50,
+        fields=None,
+        search=None,
+        origin=None,
+        status=None,
+        organization__short_name=None,
+    ) -> t.ActivityResponse:
+        parameters = {}
+        if cursor_id:
+            parameters["cursor_id"] = cursor_id
+        elif prev_cursor_id:
+            parameters["prev_cursor_id"] = prev_cursor_id
+        if page_size:
+            parameters["page_size"] = page_size
+        if fields:
+            parameters["fields"] = fields
+        if search:
+            parameters["search"] = search
+        if origin:
+            parameters["origin"] = origin
+        if status:
+            parameters["status"] = status
+        if organization__short_name:
+            parameters["organization__short_name"] = organization__short_name
+
+        url = self.api_url + "/api/v1/sov/activity"
+        response = self.session.get(url, params=parameters)
+        raise_for_status(response)
+        return response.json()
```

### Comparing `pingintel_api-0.3.0/.gitignore` & `pingintel_api-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.3.0/LICENSE` & `pingintel_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.3.0/pyproject.toml` & `pingintel_api-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.3.0/PKG-INFO` & `pingintel_api-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pingintel-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python-based client to Ping Data Intelligence APIs
 Project-URL: Homepage, https://github.com/pingintel/pingintel-api
 Project-URL: Issues, https://github.com/pingintel/pingintel-api/issues
 Author-email: Scott Stafford <scott@pingintel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

