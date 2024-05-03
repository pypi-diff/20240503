# Comparing `tmp/cto_cli-0.1.3.tar.gz` & `tmp/cto_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cto_cli-0.1.3.tar", max compression
+gzip compressed data, was "cto_cli-0.2.0.tar", max compression
```

## Comparing `cto_cli-0.1.3.tar` & `cto_cli-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-04-03 10:47:36.966879 cto_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0      233 2024-04-03 10:47:36.966879 cto_cli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/api/__init__.py
--rw-r--r--   0        0        0     7306 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/api/connector.py
--rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/commands/__init__.py
--rw-r--r--   0        0        0     3273 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/commands/config.py
--rw-r--r--   0        0        0     2047 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/commands/users.py
--rw-r--r--   0        0        0        0 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/__init__.py
--rw-r--r--   0        0        0      451 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/commands.py
--rw-r--r--   0        0        0     6279 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/files.py
--rw-r--r--   0        0        0     7277 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/operations.py
--rw-r--r--   0        0        0     2922 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/settings.py
--rw-r--r--   0        0        0     1789 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/local/validators.py
--rw-r--r--   0        0        0     2949 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/ecs/main.py
--rw-r--r--   0        0        0      652 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/main.py
--rw-r--r--   0        0        0      213 2024-04-03 10:47:36.966879 cto_cli-0.1.3/cto_cli/utils/errors.py
--rw-r--r--   0        0        0     1580 2024-04-03 10:47:37.918884 cto_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 11:11:03.634479 cto_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0      233 2024-05-03 11:11:03.634479 cto_cli-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/api/__init__.py
+-rw-r--r--   0        0        0     7715 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/api/connector.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/commands/__init__.py
+-rw-r--r--   0        0        0     3273 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/commands/config.py
+-rw-r--r--   0        0        0     2047 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/commands/users.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/__init__.py
+-rw-r--r--   0        0        0      451 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/commands.py
+-rw-r--r--   0        0        0     6279 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/files.py
+-rw-r--r--   0        0        0     7277 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/operations.py
+-rw-r--r--   0        0        0     3068 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/settings.py
+-rw-r--r--   0        0        0     1832 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/local/validators.py
+-rw-r--r--   0        0        0     3778 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/ecs/main.py
+-rw-r--r--   0        0        0      652 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/main.py
+-rw-r--r--   0        0        0      213 2024-05-03 11:11:03.634479 cto_cli-0.2.0/cto_cli/utils/errors.py
+-rw-r--r--   0        0        0     1580 2024-05-03 11:11:04.342481 cto_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 cto_cli-0.2.0/PKG-INFO
```

### Comparing `cto_cli-0.1.3/LICENSE` & `cto_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.3/cto_cli/ecs/api/connector.py` & `cto_cli-0.2.0/cto_cli/ecs/api/connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,44 +10,54 @@
 from rich import print, print_json
 from rich.syntax import Syntax
 
 from cto_cli.ecs.local.settings import load_ecs_settings, SettingsNotFound
 from cto_cli.utils.errors import print_error
 
 
-class ApiError(Exception):
+class ApiTokenError(Exception):
+    pass
+
+
+class ApiConnectionError(Exception):
     pass
 
 
 class APIConnector:
     def __init__(self, load_settings: bool = True, url: str | None = None, headers: dict | None = None):
         self._headers = headers
         self._url = url
 
         if load_settings:
             self._set_api_details()
 
     @staticmethod
-    def _handle_response(response: requests.Response) -> None:
+    def _handle_error_response(error: requests.exceptions.HTTPError):
+        try:
+            print_error(f'{error.response.json()["detail"]}', exit=True)
+        except Exception:
+            print_error(f'{error.response.text}', exit=True)
+
+    def _handle_response(self, response: requests.Response) -> None:
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
-            try:
-                print_error(f'{e.response.json()["detail"]}', exit=True)
-            except Exception:
-                print_error(f'{e.response.text}', exit=True)
+            self._handle_error_response(e)
 
     def _set_api_details(self) -> None:
         try:
             settings = load_ecs_settings()
         except SettingsNotFound:
             print_error('Credentials not found, run [b]cto ecs init[b]', exit=True)
             sys.exit(1)
 
-        self._headers = {'Authorization': settings.token}
+        self._headers = {
+            'Authorization': settings.token,
+            **({'x-saas-token': settings.saas_token} if settings.saas_token else {}),
+        }
         self._url = settings.url
 
     @staticmethod
     def _print_response(response: requests.Response) -> None:
         if response.headers['content-type'] == 'application/json':
             response_json = response.json()
             print_json(data=response_json)
@@ -231,12 +241,15 @@
 
         return response.json()
 
     def check_api_connectivity(self):
         try:
             response = requests.request('get', f'{self._url}/users', headers=self._headers)
         except (ConnectionError, Timeout):
-            raise ApiError('Could not connect to the API, validate URL')
+            raise ApiConnectionError('Could not connect to the API, validate URL')
         try:
             response.raise_for_status()
-        except HTTPError:
-            raise ApiError('Token is not valid')
+        except HTTPError as e:
+            if e.response.status_code == 401:
+                raise ApiTokenError('Token is not valid')
+            else:
+                self._handle_error_response(e)
```

### Comparing `cto_cli-0.1.3/cto_cli/ecs/commands/config.py` & `cto_cli-0.2.0/cto_cli/ecs/commands/config.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.3/cto_cli/ecs/commands/users.py` & `cto_cli-0.2.0/cto_cli/ecs/commands/users.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.3/cto_cli/ecs/local/files.py` & `cto_cli-0.2.0/cto_cli/ecs/local/files.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.3/cto_cli/ecs/local/operations.py` & `cto_cli-0.2.0/cto_cli/ecs/local/operations.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.3/cto_cli/ecs/local/settings.py` & `cto_cli-0.2.0/cto_cli/ecs/local/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,22 +21,24 @@
 
 
 @dataclass(frozen=True)
 class ECSSettings:
     url: str
     token: str
     ecs_path: str
+    saas_token: None | str = None
 
     @classmethod
     def load_from_env(cls) -> ECSSettings:
         try:
             return cls(
                 url=os.environ['ECS_URL'],
                 token=os.environ['ECS_TOKEN'],
                 ecs_path=os.environ['ECS_LOCAL_PATH'],
+                saas_token=os.getenv('ECS_SAAS_TOKEN')
             )
         except KeyError:
             raise EnvSettingsNotFound
 
 
 def load_ecs_settings() -> ECSSettings:
     try:
@@ -77,19 +79,19 @@
         print_error('The current path is not empty', exit=True)
 
 
 def create_repo_dir() -> None:
     get_repo_path().mkdir(parents=True, exist_ok=True)
 
 
-def store_settings(url: str, token: str) -> None:
+def store_settings(url: str, token: str, saas_token: None | str = None) -> None:
     CTO_DIR.mkdir(parents=True, exist_ok=True)
 
     with open(ECS_SETTINGS_LOCATION, 'w') as f:
-        f.write(json.dumps({'token': token, 'url': url, 'ecs_path': str(WORKING_DIR)}))
+        f.write(json.dumps({'token': token, 'url': url, 'saas_token': saas_token, 'ecs_path': str(WORKING_DIR)}))
 
 
 def _validate_workdir_in_ecs_repo_path():
     ecs_repo_path = get_repo_path()
 
     try:
         WORKING_DIR.relative_to(Path(ecs_repo_path))
```

### Comparing `cto_cli-0.1.3/cto_cli/ecs/local/validators.py` & `cto_cli-0.2.0/cto_cli/ecs/local/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import lru_cache
 from importlib.metadata import version as metadata_version
 from subprocess import CalledProcessError
 
 import typer
 
 from cto_cli.ecs.api.connector import APIConnector
 from cto_cli.ecs.local.commands import run_command
@@ -20,14 +21,15 @@
         print_error('Please install [b]sha256sum[/b]', exit=True)
 
 
 def get_current_cli_version() -> str:
     return metadata_version('cto-cli')
 
 
+@lru_cache
 def check_versions_compatibility() -> None:
     current_cli_version = get_current_cli_version()
     cli_major, cli_minor, cli_patch = current_cli_version.split('.')
 
     server_response = APIConnector().get_version_details()
 
     server_version = server_response['version']
```

### Comparing `cto_cli-0.1.3/cto_cli/ecs/main.py` & `cto_cli-0.2.0/cto_cli/ecs/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typer
 from rich import print
 
-from cto_cli.ecs.api.connector import APIConnector, ApiError
+from cto_cli.ecs.api.connector import APIConnector, ApiTokenError, ApiConnectionError
 from cto_cli.ecs.commands import users, config
 from cto_cli.ecs.local.settings import (
     store_settings,
     load_ecs_settings,
     SettingsNotFound,
     check_working_dir_is_empty,
     create_repo_dir,
@@ -31,55 +31,73 @@
 
 def ask_and_store_settings() -> None:
     try:
         settings = load_ecs_settings()
     except SettingsNotFound:
         settings = None
 
-    api_url = typer.prompt("What's the API url?", default=settings.url if settings else None)
+    saas_token = None
 
-    while not (api_url.startswith('http://') or api_url.startswith('https://')):
-        print_error("URL doesn't include the protocol")
+    saas = typer.confirm(
+        'If you\'re using ECS Cloud type Y, if you\'re using your own on-prem ECS server, type N', abort=False
+    )
+    if saas:
+        saas_token = typer.prompt(
+            "What's your ECS SaaS token?", default=settings.saas_token if settings and settings.saas_token else None
+        )
+        api_url = 'https://api.enterpriseconfigurationservice.com'
+        api_connector = APIConnector(
+            load_settings=False, url=api_url, headers={'Authorization': 'very_first_user', 'x-saas-token': saas_token}
+        )
+    else:
         api_url = typer.prompt("What's the API url?", default=settings.url if settings else None)
 
-    api_connector = APIConnector(load_settings=False, url=api_url, headers={'Authorization': 'very_first_user'})
+        while not (api_url.startswith('http://') or api_url.startswith('https://')):
+            print_error("URL doesn't include the protocol")
+            api_url = typer.prompt("What's the API url?", default=settings.url if settings else None)
+        api_connector = APIConnector(load_settings=False, url=api_url, headers={'Authorization': 'very_first_user'})
+
     try:
         api_connector.check_api_connectivity()
-    except ApiError:
+    except ApiConnectionError as e:
+        print_error(str(e))
+        ask_and_store_settings()
+    except ApiTokenError:
         # admin account already exist
-        token = typer.prompt("What's your token?", default=settings.token if settings else None)
-        store_settings(api_url, token)
+        user_token = typer.prompt("What's your User token?", default=settings.token if settings else None)
+        store_settings(api_url, user_token, saas_token)
     else:
         # create admin account
-        token = create_admin_account(api_connector)
-        store_settings(api_url, token)
+        user_token = create_admin_account(api_connector)
+        store_settings(api_url, user_token, saas_token)
 
 
 def store_and_validate_settings() -> None:
     ask_and_store_settings()
     try:
         APIConnector().check_api_connectivity()
-    except ApiError as e:
+    except ApiTokenError as e:
         print_error(str(e))
         store_and_validate_settings()
 
 
 @app.command(name='init')
 def init() -> None:
     check_installed_tools()
-    check_versions_compatibility()
     reinit = False
 
     try:
         current_settings = load_ecs_settings()
     except SettingsNotFound:
         current_settings = None
 
     if current_settings:
+        check_versions_compatibility()
         print(f'ECS has been already inited in path: [b]{current_settings.ecs_path}[/b]')
         reinit = typer.confirm('Do you want to re-init it?', abort=True)
 
     if reinit is True or current_settings is None:
         check_working_dir_is_empty()
         store_and_validate_settings()
+        check_versions_compatibility()
         create_repo_dir()
         print('[green]Your credentials were saved, run [b]cto ecs config pull[/b] to start[/green]')
```

### Comparing `cto_cli-0.1.3/cto_cli/main.py` & `cto_cli-0.2.0/cto_cli/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.3/pyproject.toml` & `cto_cli-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cto-cli"
-version = "0.1.3"
+version = "0.2.0"
 description = "The CTO cli"
 authors = ["CTO <support@cloudtechnologyoffice.com>"]
 readme = "README.md"
 homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest"
 repository = "https://github.com/Cloud-Technology-Office/cto-cli"
 license = "Apache-2.0"
```

### Comparing `cto_cli-0.1.3/PKG-INFO` & `cto_cli-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cto-cli
-Version: 0.1.3
+Version: 0.2.0
 Summary: The CTO cli
 Home-page: https://doc.cloudtechnologyoffice.com/ecs/latest
 License: Apache-2.0
 Author: CTO
 Author-email: support@cloudtechnologyoffice.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

