# Comparing `tmp/ghga_event_schemas-3.1.0.tar.gz` & `tmp/ghga_event_schemas-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_event_schemas-3.1.0.tar", last modified: Tue Mar 12 11:15:42 2024, max compression
+gzip compressed data, was "ghga_event_schemas-3.2.0.tar", last modified: Fri May  3 09:48:11 2024, max compression
```

## Comparing `ghga_event_schemas-3.1.0.tar` & `ghga_event_schemas-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:15:42.593639 ghga_event_schemas-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-03-12 11:15:42.593639 ghga_event_schemas-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 11:15:42.593639 ghga_event_schemas-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:15:42.589639 ghga_event_schemas-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:15:42.593639 ghga_event_schemas-3.1.0/src/ghga_event_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas/pydantic_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:15:42.593639 ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-03-12 11:15:42.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-12 11:15:42.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 11:15:42.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-12 11:15:42.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-12 11:15:42.000000 ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:15:42.593639 ghga_event_schemas-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-12 11:15:34.000000 ghga_event_schemas-3.1.0/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.571694 ghga_event_schemas-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/src/ghga_event_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15432 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas/pydantic_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/tests/test_validation.py
```

### Comparing `ghga_event_schemas-3.1.0/LICENSE` & `ghga_event_schemas-3.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+   Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
    for the German Human Genome-Phenome Archive (GHGA)
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-3.1.0/PKG-INFO` & `ghga_event_schemas-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: ghga_event_schemas
-Version: 3.1.0
+Version: 3.2.0
 Summary: GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-event-schemas
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema<5.0.0,>=4.17.3
+Requires-Dist: jsonschema<5.0.0,>=4.21.1
 Requires-Dist: pydantic[email]<3,>=2
 
 [![tests](https://github.com/ghga-de/ghga-event-schemas/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/ghga-event-schemas/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-event-schemas/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-event-schemas?branch=main)
 
 # Ghga Event Schemas
 
@@ -35,29 +34,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-event-schemas):
 ```bash
-docker pull ghga/ghga-event-schemas:3.1.0
+docker pull ghga/ghga-event-schemas:3.2.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-event-schemas:3.1.0 .
+docker build -t ghga/ghga-event-schemas:3.2.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-event-schemas:3.1.0 --help
+docker run -p 8080:8080 ghga/ghga-event-schemas:3.2.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_event_schemas-3.1.0/README.md` & `ghga_event_schemas-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-event-schemas):
 ```bash
-docker pull ghga/ghga-event-schemas:3.1.0
+docker pull ghga/ghga-event-schemas:3.2.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-event-schemas:3.1.0 .
+docker build -t ghga/ghga-event-schemas:3.2.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-event-schemas:3.1.0 --help
+docker run -p 8080:8080 ghga/ghga-event-schemas:3.2.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_event_schemas-3.1.0/pyproject.toml` & `ghga_event_schemas-3.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = [
-    "setuptools>=67.7.2",
+    "setuptools>=69",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 readme = "README.md"
 authors = [
     { name = "German Human Genome Phenome Archive (GHGA)", email = "contact@ghga.de" },
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.12"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "ghga_event_schemas"
-version = "3.1.0"
+version = "3.2.0"
 description = "GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service."
 dependencies = [
-    "jsonschema>=4.17.3,<5.0.0",
+    "jsonschema>=4.21.1,<5.0.0",
     "pydantic[email]>=2,<3",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.urls]
@@ -51,38 +50,40 @@
 line-length = 88
 src = [
     "src",
     "tests",
     "examples",
     "scripts",
 ]
-target-version = "py39"
+target-version = "py312"
 
 [tool.ruff.lint]
 fixable = [
     "UP",
     "I",
     "D",
 ]
 ignore = [
-    "E",
-    "W",
+    "E111",
+    "E114",
+    "E116",
     "PLW",
     "RUF001",
     "RUF010",
     "RUF012",
     "N818",
     "B008",
     "PLR2004",
     "D205",
     "D400",
     "D401",
     "D107",
     "D206",
     "D300",
+    "UP040",
 ]
 select = [
     "C90",
     "F",
     "I",
     "S",
     "B",
@@ -134,15 +135,15 @@
 ]
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
 no_site_packages = false
 
 [tool.pytest.ini_options]
-minversion = "7.1"
+minversion = "8.0"
 asyncio_mode = "strict"
 
 [tool.coverage.paths]
 source = [
     "src",
     "/workspace/src",
     "**/lib/python*/site-packages",
```

### Comparing `ghga_event_schemas-3.1.0/src/ghga_event_schemas/__init__.py` & `ghga_event_schemas-3.2.0/src/ghga_event_schemas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-3.1.0/src/ghga_event_schemas/pydantic_.py` & `ghga_event_schemas-3.2.0/src/ghga_event_schemas/pydantic_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -16,15 +16,15 @@
 """Contains pydantic BaseModel-based versions of the schemas.
 
 Please note, these pydantic-based schemas are the source of truth for all other
 schema representations such as json-schema.
 """
 
 from enum import Enum
-from typing import Any, Optional
+from typing import Any
 
 from pydantic import BaseModel, ConfigDict, EmailStr, Field, field_validator
 
 from ghga_event_schemas.validation import validated_upload_date
 
 
 class MetadataDatasetStage(str, Enum):
@@ -37,15 +37,15 @@
 class MetadataDatasetFile(BaseModel):
     """
     A file as that is part of a Dataset.
     Only fields relevant to the WPS are included for now. May be extended.
     """
 
     accession: str = Field(..., description="The file accession.")
-    description: Optional[str] = Field(..., description="The description of the file.")
+    description: str | None = Field(..., description="The description of the file.")
     file_extension: str = Field(
         ..., description="The file extension with a leading dot."
     )
     model_config = ConfigDict(title="metadata_dataset_file", extra="allow")
 
 
 class MetadataDatasetID(BaseModel):
@@ -78,17 +78,15 @@
     Only fields relevant to the WPS are included for now. May be extended.
     """
 
     title: str = Field(..., description="The title of the dataset.")
     stage: MetadataDatasetStage = Field(
         ..., description="The current stage of this dataset."
     )
-    description: Optional[str] = Field(
-        ..., description="The description of the dataset."
-    )
+    description: str | None = Field(..., description="The description of the dataset.")
     files: list[MetadataDatasetFile] = Field(
         ..., description="Files contained in the dataset."
     )
     model_config = ConfigDict(title="metadata_dataset_overview", extra="allow")
 
 
 class UploadDateModel(BaseModel):
@@ -391,21 +389,54 @@
 
     model_config = ConfigDict(title="file_deletion_success")
 
 
 class UserID(BaseModel):
     """Generic event payload to relay a user ID."""
 
-    user_id: str
+    user_id: str = Field(..., description="The user ID")
 
 
 class AccessRequestDetails(UserID):
     """Event used to convey the user ID and dataset ID of an access request."""
 
-    dataset_id: str
+    dataset_id: str = Field(..., description="The dataset ID")
+
+
+class IvaType(str, Enum):
+    """The type of IVA"""
+
+    PHONE = "Phone"
+    FAX = "Fax"
+    POSTAL_ADDRESS = "PostalAddress"
+    IN_PERSON = "InPerson"
+
+
+class IvaState(str, Enum):
+    """The state of an IVA"""
+
+    UNVERIFIED = "Unverified"
+    CODE_REQUESTED = "CodeRequested"
+    CODE_CREATED = "CodeCreated"
+    CODE_TRANSMITTED = "CodeTransmitted"
+    VERIFIED = "Verified"
+
+
+class UserIvaState(UserID):
+    """Notification event for state changes of a user's IVA(s)."""
+
+    value: str | None = Field(
+        default=..., description="The value of the IVA (None = all IVAs of the user)"
+    )
+    type: IvaType | None = Field(
+        default=..., description="The type of the IVA (None = all IVAs of the user"
+    )
+    state: IvaState = Field(..., description="The new state of the IVA")
+
+    model_config = ConfigDict(title="iva_state_change")
 
 
 # Lists event schemas (values) by event types (key):
 schema_registry: dict[str, type[BaseModel]] = {
     "metadata_dataset_deleted": MetadataDatasetID,
     "metadata_dataset_overview": MetadataDatasetOverview,
     "metadata_submission_upserted": MetadataSubmissionUpserted,
@@ -417,9 +448,11 @@
     "non_staged_file_requested": NonStagedFileRequested,
     "file_staged_for_download": FileStagedForDownload,
     "file_download_served": FileDownloadServed,
     "notification": Notification,
     "searchable_resource_deleted": SearchableResourceInfo,
     "searchable_resource_upserted": SearchableResource,
     "user_id": UserID,
+    "second_factor_recreated": UserID,
     "access_request_details": AccessRequestDetails,
+    "iva_state_changed": UserIvaState,
 }
```

### Comparing `ghga_event_schemas-3.1.0/src/ghga_event_schemas/validation.py` & `ghga_event_schemas-3.2.0/src/ghga_event_schemas/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ghga_event_schemas-3.1.0/src/ghga_event_schemas.egg-info/PKG-INFO` & `ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: ghga_event_schemas
-Version: 3.1.0
+Version: 3.2.0
 Summary: GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-event-schemas
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema<5.0.0,>=4.17.3
+Requires-Dist: jsonschema<5.0.0,>=4.21.1
 Requires-Dist: pydantic[email]<3,>=2
 
 [![tests](https://github.com/ghga-de/ghga-event-schemas/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/ghga-event-schemas/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-event-schemas/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-event-schemas?branch=main)
 
 # Ghga Event Schemas
 
@@ -35,29 +34,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-event-schemas):
 ```bash
-docker pull ghga/ghga-event-schemas:3.1.0
+docker pull ghga/ghga-event-schemas:3.2.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-event-schemas:3.1.0 .
+docker build -t ghga/ghga-event-schemas:3.2.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-event-schemas:3.1.0 --help
+docker run -p 8080:8080 ghga/ghga-event-schemas:3.2.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_event_schemas-3.1.0/tests/test_validation.py` & `ghga_event_schemas-3.2.0/tests/test_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 - 2023 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
+# Copyright 2021 - 2024 Universität Tübingen, DKFZ, EMBL, and Universität zu Köln
 # for the German Human Genome-Phenome Archive (GHGA)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

