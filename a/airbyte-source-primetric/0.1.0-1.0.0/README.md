# Comparing `tmp/airbyte-source-primetric-0.1.0.tar.gz` & `tmp/airbyte_source_primetric-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-primetric-0.1.0.tar", last modified: Wed Jan 31 16:51:45 2024, max compression
+gzip compressed data, was "airbyte_source_primetric-1.0.0.tar", max compression
```

## Comparing `airbyte-source-primetric-0.1.0.tar` & `airbyte_source_primetric-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.151239 airbyte-source-primetric-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     5426 2024-01-31 16:51:45.151239 airbyte-source-primetric-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5411 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.147238 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5426 2024-01-31 16:51:45.000000 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1742 2024-01-31 16:51:45.000000 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 16:51:45.000000 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 16:51:45.000000 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 16:51:45.000000 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-01-31 16:51:45.000000 airbyte-source-primetric-0.1.0/airbyte_source_primetric.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.143238 airbyte-source-primetric-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)      160 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      381 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)    27354 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      205 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)     5316 2024-01-31 16:51:45.151239 airbyte-source-primetric-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      930 2024-01-31 16:51:43.000000 airbyte-source-primetric-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.143238 airbyte-source-primetric-0.1.0/source_primetric/
--rw-r--r--   0 root         (0) root         (0)      130 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/__init__.py
--rw-r--r--   0 root         (0) root         (0)      239 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.147238 airbyte-source-primetric-0.1.0/source_primetric/schemas/
--rw-r--r--   0 root         (0) root         (0)     5953 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/assignments.json
--rw-r--r--   0 root         (0) root         (0)     1063 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/employees.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/hashtags.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_clients.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_company_groups.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_departments.json
--rw-r--r--   0 root         (0) root         (0)      252 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_identity_providers.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_positions.json
--rw-r--r--   0 root         (0) root         (0)      346 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_rag_scopes.json
--rw-r--r--   0 root         (0) root         (0)      250 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_roles.json
--rw-r--r--   0 root         (0) root         (0)      203 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_seniorities.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_tags.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_teams.json
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/organization_timeoff_types.json
--rw-r--r--   0 root         (0) root         (0)      558 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/people.json
--rw-r--r--   0 root         (0) root         (0)     1696 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/projects.json
--rw-r--r--   0 root         (0) root         (0)      579 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/projects_vacancies.json
--rw-r--r--   0 root         (0) root         (0)      257 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/rag_ratings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.147238 airbyte-source-primetric-0.1.0/source_primetric/schemas/shared/
--rw-r--r--   0 root         (0) root         (0)      254 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/shared/custom_attributes.json
--rw-r--r--   0 root         (0) root         (0)      232 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/shared/money_object.json
--rw-r--r--   0 root         (0) root         (0)      512 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/skills.json
--rw-r--r--   0 root         (0) root         (0)      797 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/timeoffs.json
--rw-r--r--   0 root         (0) root         (0)      778 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/schemas/worklogs.json
--rw-r--r--   0 root         (0) root         (0)     7055 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/source.py
--rw-r--r--   0 root         (0) root         (0)      908 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/source_primetric/spec.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:51:45.147238 airbyte-source-primetric-0.1.0/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-01-31 16:34:25.000000 airbyte-source-primetric-0.1.0/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4551 2024-05-03 20:41:43.000000 airbyte_source_primetric-1.0.0/README.md
+-rw-r--r--   0        0        0      137 2024-05-03 20:41:43.000000 airbyte_source_primetric-1.0.0/main.py
+-rw-r--r--   0        0        0      773 2024-05-03 21:09:10.543828 airbyte_source_primetric-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-03 20:41:43.000000 airbyte_source_primetric-1.0.0/source_primetric/__init__.py
+-rw-r--r--   0        0        0    35894 2024-05-03 20:41:43.000000 airbyte_source_primetric-1.0.0/source_primetric/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-03 20:41:43.000000 airbyte_source_primetric-1.0.0/source_primetric/run.py
+-rw-r--r--   0        0        0      478 2024-05-03 20:41:43.000000 airbyte_source_primetric-1.0.0/source_primetric/source.py
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_primetric-1.0.0/PKG-INFO
```

### Comparing `airbyte-source-primetric-0.1.0/PKG-INFO` & `airbyte_source_primetric-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-primetric
-Version: 0.1.0
-Summary: Source implementation for Primetric.
+Version: 1.0.0
+Summary: Source implementation for primetric.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/primetric
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Primetric Source
 
-This is the repository for the Primetric source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/primetric).
+This is the repository for the Primetric configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/primetric).
 
+## Local development
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+### Prerequisites
 
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/primetric)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_primetric/spec.yaml` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/primetric)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source primetric test creds`
-and place them into `secrets/config.json`.
+
+### Locally running the connector
 
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-primetric spec
+poetry run source-primetric check --config secrets/config.json
+poetry run source-primetric discover --config secrets/config.json
+poetry run source-primetric read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-primetric build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-primetric:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-primetric:dev .
+airbyte-ci connectors --name=source-primetric build
 ```
 
+An image will be available on your host with the tag `airbyte/source-primetric:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-primetric:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-primetric:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-primetric:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-primetric:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-primetric test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-primetric test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/primetric.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/primetric.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-primetric-0.1.0/README.md` & `airbyte_source_primetric-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,103 @@
 # Primetric Source
 
-This is the repository for the Primetric source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/primetric).
+This is the repository for the Primetric configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/primetric).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
 
-#### Minimum Python version required `= 3.9.0`
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/primetric)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_primetric/spec.yaml` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/primetric)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source primetric test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
+
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-primetric spec
+poetry run source-primetric check --config secrets/config.json
+poetry run source-primetric discover --config secrets/config.json
+poetry run source-primetric read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
-### Locally running the connector docker image
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-primetric build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-primetric:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-primetric:dev .
+airbyte-ci connectors --name=source-primetric build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-primetric:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-primetric:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-primetric:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-primetric:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-primetric:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-primetric test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
-### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-primetric test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/primetric.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/primetric.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

