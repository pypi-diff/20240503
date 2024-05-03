# Comparing `tmp/edgegap_service-1.5.2.tar.gz` & `tmp/edgegap_service-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.5.2.tar", max compression
+gzip compressed data, was "edgegap_service-1.5.3.tar", max compression
```

## Comparing `edgegap_service-1.5.2.tar` & `edgegap_service-1.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1993 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/LICENSE
--rw-r--r--   0        0        0     2188 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/README.md
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/BUILD
--rw-r--r--   0        0        0      225 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2714 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      735 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      717 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2890 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7730 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      102 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      235 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0      152 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/logging/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/logging/_configuration.py
--rw-r--r--   0        0        0     1656 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/logging/_logger.py
--rw-r--r--   0        0        0     1880 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-05-03 14:42:17.470940 edgegap_service-1.5.2/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      972 2024-05-03 14:42:42.391083 edgegap_service-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/BUILD
+-rw-r--r--   0        0        0      225 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2931 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2890 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     8268 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      102 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      300 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      577 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0      152 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/logging/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/logging/_configuration.py
+-rw-r--r--   0        0        0     1657 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/logging/_logger.py
+-rw-r--r--   0        0        0     1880 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-03 19:51:34.394796 edgegap_service-1.5.3/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      972 2024-05-03 19:52:15.283229 edgegap_service-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.5.3/PKG-INFO
```

### Comparing `edgegap_service-1.5.2/LICENSE` & `edgegap_service-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/README.md` & `edgegap_service-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/_configuration.py` & `edgegap_service-1.5.3/edgegap_service/_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+import os
 from typing import Callable, Optional
 
 from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings, SettingsFactory
 from fastapi import APIRouter
 from pydantic import BaseModel, ConfigDict, Field
 from pydantic_settings import BaseSettings
 
 from ._environment import EnvironmentConfiguration
 from .health.checks import CheckInterface
 from .logging import LoggingConfiguration
 
 
+def get_default_root_dir() -> str:
+    return os.getcwd()
+
+
 class ServiceConfiguration(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     name: str = Field(..., description='The name of the Service')
     version: str = Field(..., description='The version of the Service')
     description: str = Field(..., description='The description of the Service')
     routers: list[APIRouter] = Field([], description='The FastAPI routers')
-    root_dir: str = Field(..., description='The Root Directory of the Service')
+    root_dir: str = Field(default_factory=get_default_root_dir, description='The Root Directory of the Service')
     static_dir: str = Field(default='static', description='The Static Directory of the Service')
     html_index_path: str | None = Field(default=None, description='The full path to the html index file')
     checks: list[type(CheckInterface)] = Field([], description='The list of Checks to run on the Service')
     depend: Optional[Callable] = Field(default=None, description='The Base Depend Attribute for DB Session')
     port: int = Field(default=8000, description='The Port of the Service')
     host: str = Field(default='0.0.0.0', description='The Host of the Service')
     workers: int = Field(default=1, description='Numbers of Workers, (if you use the scheduler, keep to 1)')
     timeout: int = Field(default=300, description='Default Timeout for Connection')
     worker_class: str = Field(default='uvicorn.workers.UvicornWorker', description='The worker class for ASGI')
     scheduler: Scheduler | None = Field(default=None, description='A Scheduler to start at boot')
     startup_functions: list[Callable] = Field(default=[], description='All function will be called on startup')
+    shutdown_functions: list[Callable] = Field(default=[], description='All function will be called on shutdown')
     env_config: EnvironmentConfiguration = Field(
         default=SettingsFactory.from_settings(EnvironmentConfiguration),
         description='The Configuration coming from the Environment Variables',
     )
     log_config: LoggingConfiguration = Field(
         default=LoggingConfiguration(),
         description='The Configuration for the Logging, will be passed as DictConfig to Python logging system',
```

### Comparing `edgegap_service-1.5.2/edgegap_service/_documentation.py` & `edgegap_service-1.5.3/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/_environment.py` & `edgegap_service-1.5.3/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/_scheduling.py` & `edgegap_service-1.5.3/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/_service.py` & `edgegap_service-1.5.3/edgegap_service/_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from logging.config import dictConfig
 from pathlib import Path
 
 from edgegap_logging import Color, Format
 from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings
-from elasticapm.contrib.starlette import ElasticAPM, make_apm_client
+from elasticapm.contrib import starlette
 from fastapi import FastAPI, staticfiles, templating
 
 from ._configuration import ServiceConfiguration
 from ._documentation import DocumentationRoute
 from ._scheduling import SchedulingAPI
 from ._templating import TemplateRenderer
 from .health import HealthCheck
@@ -119,20 +119,24 @@
 
     def __init_apm(self):
         if isinstance(self.__configuration.settings, ProjectBaseSettings):
             apm = self.__configuration.settings.apm
 
             if apm.enabled:
                 self.__logger.info('Apm is enabled')
-                client = make_apm_client({
+                client = starlette.make_apm_client({
                     'SERVICE_NAME': self.__configuration.name,
                     'SECRET_TOKEN': apm.token,
                     'SERVER_URL': f'{apm.scheme}://{apm.server}:{apm.port}',
                 })
-                self.__app.add_middleware(ElasticAPM, client=client)
+                data = {
+                    'middleware_class': starlette.ElasticAPM,
+                    'client': client,
+                }
+                self.__app.add_middleware(**data)
 
     def __init_logstash(self):
         if isinstance(self.__configuration.settings, ProjectBaseSettings):
             logstash = self.__configuration.settings.logstash
 
             if logstash.enabled:
                 formatter = {
@@ -168,22 +172,31 @@
             @self.__app.on_event('startup')
             def start_scheduling():
                 SchedulingAPI().init_scheduling_api(self.__app)
                 asyncio.create_task(self.__configuration.scheduler.start_all())
 
     def __init_sigterm(self):
         @self.__app.on_event('shutdown')
-        def handle():
+        async def handle():
             try:
                 self.__logger.info(f'Shutting down {Format.squared(self.__configuration.name, Color.GREEN)}')
 
                 if isinstance(self.__configuration.scheduler, Scheduler):
                     asyncio.ensure_future(self.__configuration.scheduler.stop_all())
             except Exception as e:
-                self.__logger.exception(e)
+                self.__logger.exception(f'Exception while shutting down: {e}')
+
+            for func in self.__configuration.shutdown_functions:
+                try:
+                    if inspect.iscoroutinefunction(func):
+                        await func()
+                    else:
+                        func()
+                except Exception as e:
+                    self.__logger.exception(f'Could not shutdown correctly one of the shutdown functions: {e}')
 
     def __init_startup_functions(self):
         @self.__app.on_event('startup')
         async def init_startup_functions():
             for func in self.__configuration.startup_functions:
                 try:
                     if inspect.iscoroutinefunction(func):
```

### Comparing `edgegap_service-1.5.2/edgegap_service/_templating.py` & `edgegap_service-1.5.3/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/health/_health.py` & `edgegap_service-1.5.3/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.5.3/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/health/checks/_database.py` & `edgegap_service-1.5.3/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.5.3/edgegap_service/health/checks/_interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,8 +18,7 @@
     def _check(self, **kwargs) -> CheckInstanceModel:
         """
 
         @return: tuple[bool, str]
         bool: if the check is ok
         str: message
         """
-        pass
```

### Comparing `edgegap_service-1.5.2/edgegap_service/logging/_configuration.py` & `edgegap_service-1.5.3/edgegap_service/logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/logging/_logger.py` & `edgegap_service-1.5.3/edgegap_service/logging/_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
             return Format.color(status_phrase, color)
 
         return status_and_phrase
 
     def formatMessage(self, record: logging.LogRecord) -> str:
         record_copy = copy(record)
+
         (
             client_addr,
             method,
             full_path,
             http_version,
             status_code,
         ) = record_copy.args  # type: ignore[misc]
```

### Comparing `edgegap_service-1.5.2/edgegap_service/static/html/index.html` & `edgegap_service-1.5.3/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.5.3/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.2/pyproject.toml` & `edgegap_service-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.5.2"
+version = "1.5.3"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.5.2/PKG-INFO` & `edgegap_service-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.5.2
+Version: 1.5.3
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

