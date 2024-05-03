# Comparing `tmp/edgegap_service-1.5.0.tar.gz` & `tmp/edgegap_service-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_service-1.5.0.tar", max compression
+gzip compressed data, was "edgegap_service-1.5.1.tar", max compression
```

## Comparing `edgegap_service-1.5.0.tar` & `edgegap_service-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/LICENSE
--rw-r--r--   0        0        0     2188 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/README.md
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/BUILD
--rw-r--r--   0        0        0      225 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/__init__.py
--rw-r--r--   0        0        0     2656 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_configuration.py
--rw-r--r--   0        0        0      735 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_documentation.py
--rw-r--r--   0        0        0      717 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_environment.py
--rw-r--r--   0        0        0     2890 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_scheduling.py
--rw-r--r--   0        0        0     7661 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_service.py
--rw-r--r--   0        0        0      739 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/_templating.py
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/BUILD
--rw-r--r--   0        0        0      102 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/_health.py
--rw-r--r--   0        0        0      394 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/_model.py
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/BUILD
--rw-r--r--   0        0        0      235 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/__init__.py
--rw-r--r--   0        0        0      594 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_consul.py
--rw-r--r--   0        0        0      740 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_database.py
--rw-r--r--   0        0        0      590 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_interface.py
--rw-r--r--   0        0        0      329 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/health/checks/_model.py
--rw-r--r--   0        0        0      152 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/logging/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/logging/_configuration.py
--rw-r--r--   0        0        0     1656 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/logging/_logger.py
--rw-r--r--   0        0        0     1880 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/static/html/index.html
--rw-r--r--   0        0        0     4286 2024-05-02 18:20:19.991672 edgegap_service-1.5.0/edgegap_service/static/images/favicon.ico
--rw-r--r--   0        0        0      972 2024-05-02 18:20:24.167778 edgegap_service-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 edgegap_service-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 03:42:53.867748 edgegap_service-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2188 2024-05-03 03:42:53.868068 edgegap_service-1.5.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.868233 edgegap_service-1.5.1/edgegap_service/BUILD
+-rw-r--r--   0        0        0      225 2024-05-03 03:42:53.868393 edgegap_service-1.5.1/edgegap_service/__init__.py
+-rw-r--r--   0        0        0     2714 2024-05-03 03:42:53.868723 edgegap_service-1.5.1/edgegap_service/_configuration.py
+-rw-r--r--   0        0        0      735 2024-05-03 03:42:53.868968 edgegap_service-1.5.1/edgegap_service/_documentation.py
+-rw-r--r--   0        0        0      717 2024-05-03 03:42:53.869201 edgegap_service-1.5.1/edgegap_service/_environment.py
+-rw-r--r--   0        0        0     2890 2024-05-03 03:42:53.869412 edgegap_service-1.5.1/edgegap_service/_scheduling.py
+-rw-r--r--   0        0        0     7730 2024-05-03 03:42:53.869744 edgegap_service-1.5.1/edgegap_service/_service.py
+-rw-r--r--   0        0        0      739 2024-05-03 03:42:53.870116 edgegap_service-1.5.1/edgegap_service/_templating.py
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.870255 edgegap_service-1.5.1/edgegap_service/health/BUILD
+-rw-r--r--   0        0        0      102 2024-05-03 03:42:53.870652 edgegap_service-1.5.1/edgegap_service/health/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-03 03:42:53.870964 edgegap_service-1.5.1/edgegap_service/health/_health.py
+-rw-r--r--   0        0        0      394 2024-05-03 03:42:53.871251 edgegap_service-1.5.1/edgegap_service/health/_model.py
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.871410 edgegap_service-1.5.1/edgegap_service/health/checks/BUILD
+-rw-r--r--   0        0        0      235 2024-05-03 03:42:53.872044 edgegap_service-1.5.1/edgegap_service/health/checks/__init__.py
+-rw-r--r--   0        0        0      594 2024-05-03 03:42:53.874803 edgegap_service-1.5.1/edgegap_service/health/checks/_consul.py
+-rw-r--r--   0        0        0      740 2024-05-03 03:42:53.875504 edgegap_service-1.5.1/edgegap_service/health/checks/_database.py
+-rw-r--r--   0        0        0      590 2024-05-03 03:42:53.876240 edgegap_service-1.5.1/edgegap_service/health/checks/_interface.py
+-rw-r--r--   0        0        0      329 2024-05-03 03:42:53.876818 edgegap_service-1.5.1/edgegap_service/health/checks/_model.py
+-rw-r--r--   0        0        0      152 2024-05-03 03:42:53.877565 edgegap_service-1.5.1/edgegap_service/logging/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-03 03:42:53.878319 edgegap_service-1.5.1/edgegap_service/logging/_configuration.py
+-rw-r--r--   0        0        0     1656 2024-05-03 03:42:53.878916 edgegap_service-1.5.1/edgegap_service/logging/_logger.py
+-rw-r--r--   0        0        0     1880 2024-05-03 03:42:53.881539 edgegap_service-1.5.1/edgegap_service/static/html/index.html
+-rw-r--r--   0        0        0     4286 2024-05-03 03:42:53.883224 edgegap_service-1.5.1/edgegap_service/static/images/favicon.ico
+-rw-r--r--   0        0        0      972 2024-05-03 14:08:49.033945 edgegap_service-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 edgegap_service-1.5.1/PKG-INFO
```

### Comparing `edgegap_service-1.5.0/LICENSE` & `edgegap_service-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/README.md` & `edgegap_service-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/_configuration.py` & `edgegap_service-1.5.1/edgegap_service/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Optional
 
 from edgegap_scheduling import Scheduler
 from edgegap_settings import ProjectBaseSettings, SettingsFactory
 from fastapi import APIRouter
 from pydantic import BaseModel, ConfigDict, Field
+from pydantic_settings import BaseSettings
 
 from ._environment import EnvironmentConfiguration
 from .health.checks import CheckInterface
 from .logging import LoggingConfiguration
 
 
 class ServiceConfiguration(BaseModel):
@@ -32,15 +33,15 @@
         default=SettingsFactory.from_settings(EnvironmentConfiguration),
         description='The Configuration coming from the Environment Variables',
     )
     log_config: LoggingConfiguration = Field(
         default=LoggingConfiguration(),
         description='The Configuration for the Logging, will be passed as DictConfig to Python logging system',
     )
-    settings: ProjectBaseSettings | None = Field(
+    settings: ProjectBaseSettings | BaseSettings | None = Field(
         default=None,
         description='Project Specific Settings to hold in the Service',
     )
     tags_definition: list[dict] = Field(
         default=[],
         description='See https://fastapi.tiangolo.com/tutorial/metadata/#use-your-tags for details',
     )
```

### Comparing `edgegap_service-1.5.0/edgegap_service/_documentation.py` & `edgegap_service-1.5.1/edgegap_service/_documentation.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/_environment.py` & `edgegap_service-1.5.1/edgegap_service/_environment.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/_scheduling.py` & `edgegap_service-1.5.1/edgegap_service/_scheduling.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/_service.py` & `edgegap_service-1.5.1/edgegap_service/_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,18 @@
     def __init_logging(self) -> logging.Logger:
         self.__init_logstash()
 
         dictConfig(self.__configuration.log_config.model_dump())
         logger = logging.getLogger(self.__configuration.name)
         logger.info(f'Logging for service {Format.squared(self.__configuration.name, Color.GREEN)} is configured')
 
-        if self.__configuration.settings and self.__configuration.settings.logstash.enabled:
+        if (
+            isinstance(self.__configuration.settings, ProjectBaseSettings)
+            and self.__configuration.settings.logstash.enabled
+        ):
             logger.info('Logstash is enabled')
 
         return logger
 
     def __init_apm(self):
         if isinstance(self.__configuration.settings, ProjectBaseSettings):
             apm = self.__configuration.settings.apm
```

### Comparing `edgegap_service-1.5.0/edgegap_service/_templating.py` & `edgegap_service-1.5.1/edgegap_service/_templating.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/health/_health.py` & `edgegap_service-1.5.1/edgegap_service/health/_health.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/health/checks/_consul.py` & `edgegap_service-1.5.1/edgegap_service/health/checks/_consul.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/health/checks/_database.py` & `edgegap_service-1.5.1/edgegap_service/health/checks/_database.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/health/checks/_interface.py` & `edgegap_service-1.5.1/edgegap_service/health/checks/_interface.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/logging/_configuration.py` & `edgegap_service-1.5.1/edgegap_service/logging/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/logging/_logger.py` & `edgegap_service-1.5.1/edgegap_service/logging/_logger.py`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/static/html/index.html` & `edgegap_service-1.5.1/edgegap_service/static/html/index.html`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/edgegap_service/static/images/favicon.ico` & `edgegap_service-1.5.1/edgegap_service/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `edgegap_service-1.5.0/pyproject.toml` & `edgegap_service-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-service"
-version = "1.5.0"
+version = "1.5.1"
 description = "The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 include = ["static/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `edgegap_service-1.5.0/PKG-INFO` & `edgegap_service-1.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-service
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Edgegap Service library includes various tools and helpers for creating FastAPI Service with easy integration. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-database (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-scheduling (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-settings (>=1.0.0,<2.0.0)
 Requires-Dist: elastic-apm (>=6.22.0,<7.0.0)
```

