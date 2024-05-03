# Comparing `tmp/airbyte-source-shortio-0.2.0.tar.gz` & `tmp/airbyte_source_shortio-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-shortio-0.2.0.tar", last modified: Wed Jan 31 18:00:38 2024, max compression
+gzip compressed data, was "airbyte_source_shortio-0.2.1.tar", max compression
```

## Comparing `airbyte-source-shortio-0.2.0.tar` & `airbyte_source_shortio-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:00:38.356326 airbyte-source-shortio-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4190 2024-01-31 18:00:38.356326 airbyte-source-shortio-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4011 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:00:38.352326 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4190 2024-01-31 18:00:38.000000 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      756 2024-01-31 18:00:38.000000 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 18:00:38.000000 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-01-31 18:00:38.000000 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-01-31 18:00:38.000000 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-01-31 18:00:38.000000 airbyte-source-shortio-0.2.0/airbyte_source_shortio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:00:38.352326 airbyte-source-shortio-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      215 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      546 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       89 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       95 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4051 2024-01-31 18:00:38.356326 airbyte-source-shortio-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      926 2024-01-31 18:00:36.000000 airbyte-source-shortio-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:00:38.352326 airbyte-source-shortio-0.2.0/source_shortio/
--rw-r--r--   0 root         (0) root         (0)      126 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      233 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 18:00:38.352326 airbyte-source-shortio-0.2.0/source_shortio/schemas/
--rw-r--r--   0 root         (0) root         (0)     1543 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/schemas/clicks.json
--rw-r--r--   0 root         (0) root         (0)     3215 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/schemas/links.json
--rw-r--r--   0 root         (0) root         (0)      476 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/source.py
--rw-r--r--   0 root         (0) root         (0)      818 2024-01-31 17:51:56.000000 airbyte-source-shortio-0.2.0/source_shortio/spec.yaml
+-rw-r--r--   0        0        0     4011 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/README.md
+-rw-r--r--   0        0        0      743 2024-05-03 12:30:03.322767 airbyte_source_shortio-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/__init__.py
+-rw-r--r--   0        0        0     2727 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/run.py
+-rw-r--r--   0        0        0     1543 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/schemas/clicks.json
+-rw-r--r--   0        0        0     3216 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/schemas/links.json
+-rw-r--r--   0        0        0      476 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/source.py
+-rw-r--r--   0        0        0      818 2024-05-03 12:12:46.000000 airbyte_source_shortio-0.2.1/source_shortio/spec.yaml
+-rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 airbyte_source_shortio-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-shortio-0.2.0/PKG-INFO` & `airbyte_source_shortio-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,67 @@
-Metadata-Version: 2.1
-Name: airbyte-source-shortio
-Version: 0.2.0
-Summary: Source implementation for Shortio.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: pytest~=6.2.5; extra == "tests"
-
 # Shortio Source
 
 This is the repository for the Shortio configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/shortio).
 
+## Local development
 
+#### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/shortio)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_shortio/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
 **If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source shortio test creds`
 and place them into `secrets/config.json`.
 
+### Locally running the connector docker image
 
 
+#### Build
 **Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
 ```bash
 airbyte-ci connectors --name=source-shortio build
 ```
 
 An image will be built with the tag `airbyte/source-shortio:dev`.
 
 **Via `docker build`:**
 ```bash
 docker build -t airbyte/source-shortio:dev .
 ```
 
+#### Run
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-shortio:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-shortio:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-shortio:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-shortio:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+## Testing
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-shortio test
 ```
 
+### Customizing acceptance Tests
 Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
+## Dependency Management
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
 * required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
 * required for the testing need to go to `TEST_REQUIREMENTS` list
 
+### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-shortio test`
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/shortio.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+
```

### Comparing `airbyte-source-shortio-0.2.0/README.md` & `airbyte_source_shortio-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: airbyte-source-shortio
+Version: 0.2.1
+Summary: Source implementation for Shortio.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/shortio
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
+
 # Shortio Source
 
 This is the repository for the Shortio configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/shortio).
 
 ## Local development
 
@@ -61,7 +80,8 @@
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/shortio.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 
+
```

### Comparing `airbyte-source-shortio-0.2.0/source_shortio/manifest.yaml` & `airbyte_source_shortio-0.2.1/source_shortio/manifest.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: "0.29.0"
+version: "0.86.0"
 
 definitions:
   selector:
     type: RecordSelector
     extractor:
       type: DpathExtractor
       field_path: ["{{ parameters.extractor_path }}"]
@@ -27,15 +27,15 @@
       header: "Authorization"
       api_token: "{{ config['secret_key'] }}"
 
   base_paginator:
     type: "DefaultPaginator"
     pagination_strategy:
       type: "CursorPagination"
-      cursor_value: "{{ last_records['nextPageToken'] }}"
+      cursor_value: "{{ response['nextPageToken'] }}"
     page_token_option:
       type: "RequestPath"
       field_name: "pageToken"
       inject_into: "request_parameter"
 
   v1_base_stream:
     type: DeclarativeStream
@@ -59,22 +59,22 @@
       requester:
         $ref: "#/definitions/v2_api_requester"
 
   incremental_base:
     type: DatetimeBasedCursor
     cursor_field: "updatedAt"
     datetime_format: "%Y-%m-%dT%H:%M:%S.%f%z"
-    cursor_granularity: "PT0.000001S"
+    cursor_granularity: "PT0.001S"
     lookback_window: "P31D"
     start_datetime:
       datetime: "{{ config['start_date'] }}"
       datetime_format: "%Y-%m-%dT%H:%M:%S.%f%z"
     end_datetime:
-      datetime: "{{ today_utc() }}"
-      datetime_format: "%Y-%m-%d"
+      datetime: "{{ now_utc().strftime('%Y-%m-%dT%H:%M:%S.%f%z') }}"
+      datetime_format: "%Y-%m-%dT%H:%M:%S.%f%z"
     step: "P1M"
     end_time_option:
       field_name: "beforeDate"
       inject_into: "request_parameter"
     start_time_option:
       field_name: "afterDate"
       inject_into: "request_parameter"
```

### Comparing `airbyte-source-shortio-0.2.0/source_shortio/schemas/clicks.json` & `airbyte_source_shortio-0.2.1/source_shortio/schemas/clicks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-shortio-0.2.0/source_shortio/schemas/links.json` & `airbyte_source_shortio-0.2.1/source_shortio/schemas/links.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994918699186992%*

 * *Differences: {"'properties'": "{'passwordContact': {'type': {insert: [(1, 'boolean')], delete: [1]}}}"}*

```diff
@@ -181,15 +181,15 @@
                 "null",
                 "string"
             ]
         },
         "passwordContact": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
         "path": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `airbyte-source-shortio-0.2.0/source_shortio/spec.yaml` & `airbyte_source_shortio-0.2.1/source_shortio/spec.yaml`

 * *Files identical despite different names*

