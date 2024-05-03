# Comparing `tmp/blueapi-0.4.2a1.tar.gz` & `tmp/blueapi-0.4.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.4.2a1.tar", last modified: Mon Apr 29 15:09:12 2024, max compression
+gzip compressed data, was "blueapi-0.4.2a2.tar", last modified: Wed May  1 16:27:35 2024, max compression
```

## Comparing `blueapi-0.4.2a1.tar` & `blueapi-0.4.2a2.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.773364 blueapi-0.4.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.745364 blueapi-0.4.2a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.745364 blueapi-0.4.2a1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.741364 blueapi-0.4.2a1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.745364 blueapi-0.4.2a1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.745364 blueapi-0.4.2a1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.749364 blueapi-0.4.2a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_container.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/asyncapi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/backstage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.749364 blueapi-0.4.2a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-29 15:09:12.773364 blueapi-0.4.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/codecov.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/container-startup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.749364 blueapi-0.4.2a1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.749364 blueapi-0.4.2a1/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.753364 blueapi-0.4.2a1/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/decisions/0003-no-queues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/decisions/0004-api-case.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations/type_validators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.753364 blueapi-0.4.2a1/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to/add-plans-and-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to/configure-app.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to/run-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to/write-plans.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.753364 blueapi-0.4.2a1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/images/blueapi-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   386340 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/images/blueapi.png
--rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/images/bluesky-events.png
--rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/images/debug-vscode.png
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.757364 blueapi-0.4.2a1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference/asyncapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference/messaging-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference/rest-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.757364 blueapi-0.4.2a1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/tutorials/dev-run.rst
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/tutorials/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/docs/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.741364 blueapi-0.4.2a1/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.757364 blueapi-0.4.2a1/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.757364 blueapi-0.4.2a1/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.757364 blueapi-0.4.2a1/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:09:12.773364 blueapi-0.4.2a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.741364 blueapi-0.4.2a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.757364 blueapi-0.4.2a1/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.761364 blueapi-0.4.2a1/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/cli/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.761364 blueapi-0.4.2a1/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/core/bluesky_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.761364 blueapi-0.4.2a1/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.761364 blueapi-0.4.2a1/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/handler_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/service/subprocess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.765364 blueapi-0.4.2a1/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/startup/example_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/startup/example_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.765364 blueapi-0.4.2a1/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/invalid_config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/ophyd_async_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/utils/thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.765364 blueapi-0.4.2a1/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/src/blueapi/worker/worker_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.773364 blueapi-0.4.2a1/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 15:09:12.000000 blueapi-0.4.2a1/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.765364 blueapi-0.4.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.769364 blueapi-0.4.2a1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/core/fake_device_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/core/fake_plan_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.769364 blueapi-0.4.2a1/tests/example_yaml/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/example_yaml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/example_yaml/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/example_yaml/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/example_yaml/rest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/example_yaml/valid_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/example_yaml/valid_stomp_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.769364 blueapi-0.4.2a1/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.769364 blueapi-0.4.2a1/tests/service/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/service/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/service/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/service/test_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/service/test_subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.769364 blueapi-0.4.2a1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/test_ophyd_async_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/utils/test_thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:09:12.769364 blueapi-0.4.2a1/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/worker/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-29 15:09:09.000000 blueapi-0.4.2a1/tests/worker/test_reworker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.132484 blueapi-0.4.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.096484 blueapi-0.4.2a2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/asyncapi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/backstage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-05-01 16:27:35.132484 blueapi-0.4.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/codecov.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/container-startup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0003-no-queues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0004-api-case.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/type_validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/add-plans-and-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/configure-app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/run-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/write-plans.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/blueapi-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   386340 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/blueapi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/bluesky-events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/debug-vscode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/asyncapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/messaging-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/rest-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials/dev-run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.100484 blueapi-0.4.2a2/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:27:35.132484 blueapi-0.4.2a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.100484 blueapi-0.4.2a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/amq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/bluesky_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/subprocess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/example_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/example_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/invalid_config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/ophyd_async_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/worker_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/fake_device_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/fake_plan_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/tests/example_yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/rest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/valid_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/valid_stomp_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_ophyd_async_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/worker/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/worker/test_reworker.py
```

### Comparing `blueapi-0.4.2a1/.devcontainer/devcontainer.json` & `blueapi-0.4.2a2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/CONTRIBUTING.md` & `blueapi-0.4.2a2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/actions/install_requirements/action.yml` & `blueapi-0.4.2a2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/dependabot.yml` & `blueapi-0.4.2a2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/pages/make_switcher.py` & `blueapi-0.4.2a2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/_check.yml` & `blueapi-0.4.2a2/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/_container.yml` & `blueapi-0.4.2a2/.github/workflows/_container.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/_dist.yml` & `blueapi-0.4.2a2/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/_docs.yml` & `blueapi-0.4.2a2/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/_release.yml` & `blueapi-0.4.2a2/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/_test.yml` & `blueapi-0.4.2a2/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/ci.yml` & `blueapi-0.4.2a2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.github/workflows/helm.yml` & `blueapi-0.4.2a2/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.gitignore` & `blueapi-0.4.2a2/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.pre-commit-config.yaml` & `blueapi-0.4.2a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/.vscode/launch.json` & `blueapi-0.4.2a2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/Dockerfile` & `blueapi-0.4.2a2/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 COPY . /context
 WORKDIR /context
 RUN pip install .
 
 # The runtime stage copies the built venv into a slim runtime container
 FROM python:${PYTHON_VERSION}-slim as runtime
 # Add apt-get system dependecies for runtime here if needed
+RUN apt-get update && apt-get install -y --no-install-recommends \
+    # Git required for installing packages at runtime
+    git \
+    && rm -rf /var/lib/apt/lists/*
 COPY --from=build /venv/ /venv/
 COPY ./container-startup.sh /container-startup.sh
 ENV PATH=/venv/bin:$PATH
 
 
 RUN mkdir -p /.cache/pip; chmod -R 777 /venv /.cache/pip
```

### Comparing `blueapi-0.4.2a1/LICENSE` & `blueapi-0.4.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/PKG-INFO` & `blueapi-0.4.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.2a1
+Version: 0.4.2a2
 Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.4.2a1/README.md` & `blueapi-0.4.2a2/README.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/catalog-info.yaml` & `blueapi-0.4.2a2/catalog-info.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/conf.py` & `blueapi-0.4.2a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/architecture.rst` & `blueapi-0.4.2a2/docs/explanations/architecture.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `blueapi-0.4.2a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/decisions/0003-no-queues.rst` & `blueapi-0.4.2a2/docs/explanations/decisions/0003-no-queues.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/decisions/0004-api-case.rst` & `blueapi-0.4.2a2/docs/explanations/decisions/0004-api-case.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/events.rst` & `blueapi-0.4.2a2/docs/explanations/events.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/lifecycle.rst` & `blueapi-0.4.2a2/docs/explanations/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/explanations/type_validators.rst` & `blueapi-0.4.2a2/docs/explanations/type_validators.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/how-to/add-plans-and-devices.rst` & `blueapi-0.4.2a2/docs/how-to/add-plans-and-devices.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/how-to/configure-app.rst` & `blueapi-0.4.2a2/docs/how-to/configure-app.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/how-to/run-cli.rst` & `blueapi-0.4.2a2/docs/how-to/run-cli.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/how-to/run-container.rst` & `blueapi-0.4.2a2/docs/how-to/run-container.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/how-to/write-plans.rst` & `blueapi-0.4.2a2/docs/how-to/write-plans.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/images/blueapi-architecture.png` & `blueapi-0.4.2a2/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/images/blueapi-logo.svg` & `blueapi-0.4.2a2/docs/images/blueapi-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/images/blueapi.png` & `blueapi-0.4.2a2/docs/images/blueapi.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/images/bluesky-events.png` & `blueapi-0.4.2a2/docs/images/bluesky-events.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/images/debug-vscode.png` & `blueapi-0.4.2a2/docs/images/debug-vscode.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/index.md` & `blueapi-0.4.2a2/docs/index.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/reference/asyncapi.yaml` & `blueapi-0.4.2a2/docs/reference/asyncapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/reference/openapi.yaml` & `blueapi-0.4.2a2/docs/reference/openapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/tutorials/dev-run.rst` & `blueapi-0.4.2a2/docs/tutorials/dev-run.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/tutorials/installation.md` & `blueapi-0.4.2a2/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/docs/tutorials/quickstart.rst` & `blueapi-0.4.2a2/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/helm/blueapi/Chart.yaml` & `blueapi-0.4.2a2/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.4.2a2/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/helm/blueapi/templates/deployment.yaml` & `blueapi-0.4.2a2/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/helm/blueapi/templates/ingress.yaml` & `blueapi-0.4.2a2/helm/blueapi/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.4.2a2/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/helm/blueapi/values.yaml` & `blueapi-0.4.2a2/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/pyproject.toml` & `blueapi-0.4.2a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/cli/amq.py` & `blueapi-0.4.2a2/src/blueapi/cli/amq.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/cli/cli.py` & `blueapi-0.4.2a2/src/blueapi/cli/cli.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/cli/rest.py` & `blueapi-0.4.2a2/src/blueapi/cli/rest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/cli/updates.py` & `blueapi-0.4.2a2/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/config.py` & `blueapi-0.4.2a2/src/blueapi/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/core/__init__.py` & `blueapi-0.4.2a2/src/blueapi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/core/bluesky_types.py` & `blueapi-0.4.2a2/src/blueapi/core/bluesky_types.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/core/context.py` & `blueapi-0.4.2a2/src/blueapi/core/context.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/core/device_lookup.py` & `blueapi-0.4.2a2/src/blueapi/core/device_lookup.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/core/event.py` & `blueapi-0.4.2a2/src/blueapi/core/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/messaging/base.py` & `blueapi-0.4.2a2/src/blueapi/messaging/base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.4.2a2/src/blueapi/messaging/stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/messaging/utils.py` & `blueapi-0.4.2a2/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/service/handler.py` & `blueapi-0.4.2a2/src/blueapi/service/handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/service/handler_base.py` & `blueapi-0.4.2a2/src/blueapi/service/handler_base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/service/main.py` & `blueapi-0.4.2a2/src/blueapi/service/main.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/service/model.py` & `blueapi-0.4.2a2/src/blueapi/service/model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/service/openapi.py` & `blueapi-0.4.2a2/src/blueapi/service/openapi.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/service/subprocess_handler.py` & `blueapi-0.4.2a2/src/blueapi/service/subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/startup/example_devices.py` & `blueapi-0.4.2a2/src/blueapi/startup/example_devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/startup/example_plans.py` & `blueapi-0.4.2a2/src/blueapi/startup/example_plans.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/startup/simmotor.py` & `blueapi-0.4.2a2/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/utils/__init__.py` & `blueapi-0.4.2a2/src/blueapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/utils/base_model.py` & `blueapi-0.4.2a2/src/blueapi/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/utils/modules.py` & `blueapi-0.4.2a2/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/utils/ophyd_async_connect.py` & `blueapi-0.4.2a2/src/blueapi/utils/ophyd_async_connect.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/utils/serialization.py` & `blueapi-0.4.2a2/src/blueapi/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/utils/thread_exception.py` & `blueapi-0.4.2a2/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/worker/__init__.py` & `blueapi-0.4.2a2/src/blueapi/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/worker/event.py` & `blueapi-0.4.2a2/src/blueapi/worker/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/worker/multithread.py` & `blueapi-0.4.2a2/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/worker/reworker.py` & `blueapi-0.4.2a2/src/blueapi/worker/reworker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/worker/task.py` & `blueapi-0.4.2a2/src/blueapi/worker/task.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi/worker/worker.py` & `blueapi-0.4.2a2/src/blueapi/worker/worker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.4.2a2/src/blueapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.2a1
+Version: 0.4.2a2
 Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.4.2a1/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.4.2a2/src/blueapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/conftest.py` & `blueapi-0.4.2a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/core/fake_device_module.py` & `blueapi-0.4.2a2/tests/core/fake_device_module.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/core/test_context.py` & `blueapi-0.4.2a2/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/core/test_event.py` & `blueapi-0.4.2a2/tests/core/test_event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/messaging/test_stomptemplate.py` & `blueapi-0.4.2a2/tests/messaging/test_stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/messaging/test_utils.py` & `blueapi-0.4.2a2/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/service/test_handler.py` & `blueapi-0.4.2a2/tests/service/test_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/service/test_openapi.py` & `blueapi-0.4.2a2/tests/service/test_openapi.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/service/test_rest_api.py` & `blueapi-0.4.2a2/tests/service/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/service/test_subprocess_handler.py` & `blueapi-0.4.2a2/tests/service/test_subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/test_cli.py` & `blueapi-0.4.2a2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/test_config.py` & `blueapi-0.4.2a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/utils/test_ophyd_async_connect.py` & `blueapi-0.4.2a2/tests/utils/test_ophyd_async_connect.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/utils/test_thread_exception.py` & `blueapi-0.4.2a2/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/worker/devices.py` & `blueapi-0.4.2a2/tests/worker/devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a1/tests/worker/test_reworker.py` & `blueapi-0.4.2a2/tests/worker/test_reworker.py`

 * *Files identical despite different names*

