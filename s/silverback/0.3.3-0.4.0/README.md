# Comparing `tmp/silverback-0.3.3.tar.gz` & `tmp/silverback-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.3.3.tar", last modified: Sat Apr 27 18:07:03 2024, max compression
+gzip compressed data, was "silverback-0.4.0.tar", last modified: Thu May  2 23:12:00 2024, max compression
```

## Comparing `silverback-0.3.3.tar` & `silverback-0.4.0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.886002 silverback-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-27 18:06:08.000000 silverback-0.3.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-27 18:06:08.000000 silverback-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-27 18:06:08.000000 silverback-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-27 18:06:08.000000 silverback-0.3.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-27 18:06:08.000000 silverback-0.3.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-27 18:06:08.000000 silverback-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-27 18:07:03.886002 silverback-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-27 18:06:08.000000 silverback-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-27 18:06:08.000000 silverback-0.3.3/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.878003 silverback-0.3.3/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 18:06:08.000000 silverback-0.3.3/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-27 18:06:08.000000 silverback-0.3.3/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-27 18:06:08.000000 silverback-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 18:07:03.886002 silverback-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-27 18:06:08.000000 silverback-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-27 18:06:08.000000 silverback-0.3.3/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.882002 silverback-0.3.3/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 18:07:03.000000 silverback-0.3.3/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:07:03.886002 silverback-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:06:08.000000 silverback-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-27 18:06:08.000000 silverback-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-27 18:06:08.000000 silverback-0.3.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.967940 silverback-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-02 23:11:00.000000 silverback-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-02 23:11:00.000000 silverback-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-02 23:11:00.000000 silverback-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-02 23:11:00.000000 silverback-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-02 23:11:00.000000 silverback-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-02 23:12:00.967940 silverback-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-02 23:11:00.000000 silverback-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-02 23:11:00.000000 silverback-0.4.0/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-02 23:11:00.000000 silverback-0.4.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-02 23:11:00.000000 silverback-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 23:12:00.967940 silverback-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-02 23:11:00.000000 silverback-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.967940 silverback-0.4.0/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.967940 silverback-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:11:00.000000 silverback-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 23:11:00.000000 silverback-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 23:11:00.000000 silverback-0.4.0/tests/test_cli.py
```

### Comparing `silverback-0.3.3/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.4.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.4.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.4.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/release-drafter.yml` & `silverback-0.4.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/workflows/codeql.yaml` & `silverback-0.4.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/workflows/commitlint.yaml` & `silverback-0.4.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/workflows/docs.yaml` & `silverback-0.4.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/workflows/prtitle.yaml` & `silverback-0.4.0/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `silverback-0.3.3/.github/workflows/publish.yaml` & `silverback-0.4.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/.github/workflows/test.yaml` & `silverback-0.4.0/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 # TODO: Replace with macos-latest when works again.
                 #   https://github.com/actions/setup-python/issues/808
                 os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                python-version: ["3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
```

### Comparing `silverback-0.3.3/.gitignore` & `silverback-0.4.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -115,11 +115,12 @@
 dmypy.json
 
 # setuptools-scm
 version.py
 
 # Ape stuff
 .build/
+.silverback-sessions/
 
 **/.DS_Store
 *.swp
 *.swo
```

### Comparing `silverback-0.3.3/.pre-commit-config.yaml` & `silverback-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/CONTRIBUTING.md` & `silverback-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/Dockerfile` & `silverback-0.4.0/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #---------------------------------------------------------------------------------------------
 # See LICENSE in the project root for license information.
 #---------------------------------------------------------------------------------------------
 
 # Build with builder image to reduce image size
-FROM python:3.10 as builder
+FROM python:3.11 as builder
 USER root
 WORKDIR /wheels
 COPY . .
 # upgrade pip and install wheel
 RUN pip install --upgrade pip && pip install wheel
 # install silverback
 RUN pip wheel . --wheel-dir=/wheels
```

### Comparing `silverback-0.3.3/LICENSE` & `silverback-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/PKG-INFO` & `silverback-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.3.3
+Version: 0.4.0
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
@@ -42,15 +41,15 @@
 
 ## Documentation
 
 Read the [development userguide](https://docs.apeworx.io/silverback/stable/userguides/development.html) to learn more how to develop an application.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.10 or greater, python3-dev
 
 ## Installation
 
 Silverback relies heavily on the Ape development framework, so it's worth it to familarize yourself with how to install Ape and it's plugins using the [Ape installation userguide](https://docs.apeworx.io/ape/latest/userguides/quickstart#installation).
 
 ### via `pip`
 
@@ -76,20 +75,22 @@
 
 To run your bot against a live network, this SDK includes a simple runner you can use via:
 
 ```sh
 $ silverback run "example:app" --network :mainnet:alchemy
 ```
 
-**NOTE**: The example is designed to work with Python 3.9+, and we suggest using 3.11+ for speed.
+**NOTE**: The example is designed to work with Python 3.10+, and we suggest using 3.11+ for speed.
 
 ## Docker Usage
 
 ```sh
 $ docker run --volume $PWD:/home/harambe/project --volume ~/.tokenlists:/home/harambe/.tokenlists apeworx/silverback:latest run "example:app" --network :mainnet:alchemy
 ```
 
+**NOTE**: The Docker image we publish uses Python 3.11
+
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.3.3/README.md` & `silverback-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ## Documentation
 
 Read the [development userguide](https://docs.apeworx.io/silverback/stable/userguides/development.html) to learn more how to develop an application.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.10 or greater, python3-dev
 
 ## Installation
 
 Silverback relies heavily on the Ape development framework, so it's worth it to familarize yourself with how to install Ape and it's plugins using the [Ape installation userguide](https://docs.apeworx.io/ape/latest/userguides/quickstart#installation).
 
 ### via `pip`
 
@@ -47,20 +47,22 @@
 
 To run your bot against a live network, this SDK includes a simple runner you can use via:
 
 ```sh
 $ silverback run "example:app" --network :mainnet:alchemy
 ```
 
-**NOTE**: The example is designed to work with Python 3.9+, and we suggest using 3.11+ for speed.
+**NOTE**: The example is designed to work with Python 3.10+, and we suggest using 3.11+ for speed.
 
 ## Docker Usage
 
 ```sh
 $ docker run --volume $PWD:/home/harambe/project --volume ~/.tokenlists:/home/harambe/.tokenlists apeworx/silverback:latest run "example:app" --network :mainnet:alchemy
 ```
 
+**NOTE**: The Docker image we publish uses Python 3.11
+
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.3.3/build_docs.py` & `silverback-0.4.0/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/docs/_static/custom.css` & `silverback-0.4.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/docs/_static/custom.js` & `silverback-0.4.0/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/docs/_templates/layout.html` & `silverback-0.4.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/docs/conf.py` & `silverback-0.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import re
 import sys
 from functools import lru_cache
 from pathlib import Path
-from typing import List
 
 import requests
 from semantic_version import Version  # type: ignore
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- Project information -----------------------------------------------------
@@ -39,15 +38,15 @@
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns: List[str] = ["_build", ".DS_Store"]
+exclude_patterns: list[str] = ["_build", ".DS_Store"]
 
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 source_suffix = [".rst", ".md"]
 
 # The master toctree document.
@@ -90,15 +89,15 @@
     if suffix:
         new = str(Path(new) / suffix.lstrip("/"))
 
     return new
 
 
 @lru_cache(maxsize=None)
-def get_versions() -> List[str]:
+def get_versions() -> list[str]:
     """
     Get all the versions from the Web.
     """
     api_url = "https://api.github.com/repos/ApeWorx/silverback/git/trees/gh-pages?recursive=1"
     response = requests.get(api_url)
     response.raise_for_status()
     pattern = re.compile(r"v\d+.?\d+.?\d+$")
```

### Comparing `silverback-0.3.3/docs/favicon.ico` & `silverback-0.4.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/docs/logo.gif` & `silverback-0.4.0/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/docs/userguides/development.md` & `silverback-0.4.0/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/example.py` & `silverback-0.4.0/example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,84 @@
-from typing import Annotated  # NOTE: Only Python 3.9+
+from typing import Annotated
 
 from ape import chain
 from ape.api import BlockAPI
 from ape.types import ContractLog
 from ape_tokens import tokens  # type: ignore[import]
 from taskiq import Context, TaskiqDepends, TaskiqState
 
-from silverback import CircuitBreaker, SilverbackApp, SilverbackStartupState
+from silverback import AppState, CircuitBreaker, SilverbackApp
 
-# Do this to initialize your app
+# Do this first to initialize your app
 app = SilverbackApp()
 
 # NOTE: Don't do any networking until after initializing app
 USDC = tokens["USDC"]
 YFI = tokens["YFI"]
 
 
 @app.on_startup()
-def app_startup(startup_state: SilverbackStartupState):
-    return {"message": "Starting...", "block_number": startup_state.last_block_seen}
+def app_startup(startup_state: AppState):
+    # NOTE: This is called just as the app is put into "run" state,
+    #       and handled by the first available worker
+    # raise Exception  # NOTE: Any exception raised on startup aborts immediately
+    return {"block_number": startup_state.last_block_seen}
+
+
+# Can handle some resource initialization for each worker, like LLMs or database connections
+class MyDB:
+    def execute(self, query: str):
+        pass
 
 
-# Can handle some initialization on startup, like models or network connections
 @app.on_worker_startup()
-def worker_startup(state: TaskiqState):
+def worker_startup(state: TaskiqState):  # NOTE: You need the type hint here
+    # NOTE: Can put anything here, any python object works
+    state.db = MyDB()
     state.block_count = 0
-    # state.db = MyDB()
-    return {"message": "Worker started."}
+    # raise Exception  # NOTE: Any exception raised on worker startup aborts immediately
 
 
 # This is how we trigger off of new blocks
 @app.on_(chain.blocks)
-# context must be a type annotated kwarg to be provided to the task
+# NOTE: The type hint for block is `BlockAPI`, but we parse it using `EcosystemAPI`
+# NOTE: If you need something from worker state, you have to use taskiq context
 def exec_block(block: BlockAPI, context: Annotated[Context, TaskiqDepends()]):
-    context.state.block_count += 1
+    context.state.db.execute(f"some query {block.number}")
     return len(block.transactions)
 
 
 # This is how we trigger off of events
 # Set new_block_timeout to adjust the expected block time.
-@app.on_(USDC.Transfer, start_block=18588777, new_block_timeout=25)
-# NOTE: Typing isn't required
+@app.on_(USDC.Transfer, start_block=19784367, new_block_timeout=25)
+# NOTE: Typing isn't required, it will still be an Ape `ContractLog` type
 def exec_event1(log):
     if log.log_index % 7 == 3:
-        # If you ever want the app to shutdown under some scenario, call this exception
-        raise CircuitBreaker("Oopsie!")
+        # If you raise any exception, Silverback will track the failure and keep running
+        # NOTE: By default, if you have 3 tasks fail in a row, the app will shutdown itself
+        raise ValueError("I don't like the number 3.")
+
     return {"amount": log.amount}
 
 
 @app.on_(YFI.Approval)
 # Any handler function can be async too
 async def exec_event2(log: ContractLog):
-    return log.amount
-
+    if log.log_index % 7 == 6:
+        # If you ever want the app to immediately shutdown under some scenario, raise this exception
+        raise CircuitBreaker("Oopsie!")
 
-# Just in case you need to release some resources or something
-@app.on_worker_shutdown()
-def worker_shutdown(state):
-    return {
-        "message": f"Worker stopped after handling {state.block_count} blocks.",
-        "block_count": state.block_count,
-    }
+    return log.amount
 
 
 # A final job to execute on Silverback shutdown
 @app.on_shutdown()
-def app_shutdown(state):
-    return {"message": "Stopping..."}
+def app_shutdown():
+    # raise Exception  # NOTE: Any exception raised on shutdown is ignored
+    return {"some_metric": 123}
+
+
+# Just in case you need to release some resources or something inside each worker
+@app.on_worker_shutdown()
+def worker_shutdown(state: TaskiqState):  # NOTE: You need the type hint here
+    state.db = None
+    # raise Exception  # NOTE: Any exception raised on worker shutdown is ignored
```

### Comparing `silverback-0.3.3/pyproject.toml` & `silverback-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `silverback-0.3.3/setup.py` & `silverback-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,24 +64,24 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/silverback",
     include_package_data=True,
     install_requires=[
         "click",  # Use same version as eth-ape
-        "eth-ape>=0.7.0,<1.0",
+        "eth-ape>=0.7,<1.0",
         "ethpm-types>=0.6.10",  # lower pin only, `eth-ape` governs upper pin
         "eth-pydantic-types",  # Use same version as eth-ape
         "pydantic_settings",  # Use same version as eth-ape
         "taskiq[metrics]>=0.10.4,<0.11.0",
     ],
     entry_points={
         "console_scripts": ["silverback=silverback._cli:cli"],
     },
-    python_requires=">=3.8,<4",
+    python_requires=">=3.10,<4",
     extras_require=extras_require,
     py_modules=["silverback"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"silverback": ["py.typed"]},
@@ -89,13 +89,12 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `silverback-0.3.3/silverback/_cli.py` & `silverback-0.4.0/silverback/_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,14 +30,24 @@
 
     elif runner := import_from_string(val):
         return runner
 
     raise ValueError(f"Failed to import runner '{val}'.")
 
 
+def _recorder_callback(ctx, param, val):
+    if not val:
+        return None
+
+    elif recorder := import_from_string(val):
+        return recorder()
+
+    raise ValueError(f"Failed to import recorder '{val}'.")
+
+
 def _account_callback(ctx, param, val):
     if val:
         val = val.alias.replace("dev_", "TEST::")
         os.environ["SILVERBACK_SIGNER_ALIAS"] = val
 
     return val
 
@@ -88,19 +98,24 @@
 )
 @click.option("--account", type=AccountAliasPromptChoice(), callback=_account_callback)
 @click.option(
     "--runner",
     help="An import str in format '<module>:<CustomRunner>'",
     callback=_runner_callback,
 )
+@click.option(
+    "--recorder",
+    help="An import string in format '<module>:<CustomRecorder>'",
+    callback=_recorder_callback,
+)
 @click.option("-x", "--max-exceptions", type=int, default=3)
 @click.argument("path")
-def run(cli_ctx, account, runner, max_exceptions, path):
+def run(cli_ctx, account, runner, recorder, max_exceptions, path):
     app = import_from_string(path)
-    runner = runner(app, max_exceptions=max_exceptions)
+    runner = runner(app, recorder=recorder, max_exceptions=max_exceptions)
     asyncio.run(runner.run())
 
 
 @cli.command(cls=ConnectedProviderCommand, help="Run Silverback application task workers")
 @ape_cli_context()
 @verbosity_option()
 @network_option(
```

### Comparing `silverback-0.3.3/silverback/_importer.py` & `silverback-0.4.0/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/silverback/application.py` & `silverback-0.4.0/silverback/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import atexit
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import timedelta
-from typing import Callable, Dict, Optional, Union
+from typing import Callable
 
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.contracts import ContractEvent, ContractInstance
 from ape.logging import logger
 from ape.managers.chain import BlockContainer
 from ape.utils import ManagerAccessMixin
 from taskiq import AsyncTaskiqDecoratedTask, TaskiqEvents
 
 from .exceptions import ContainerTypeMismatchError, InvalidContainerTypeError
 from .settings import Settings
-from .types import TaskType
+from .types import SilverbackID, TaskType
 
 
 @dataclass
 class TaskData:
-    container: Union[BlockContainer, ContractEvent, None]
+    container: BlockContainer | ContractEvent | None
     handler: AsyncTaskiqDecoratedTask
 
 
 class SilverbackApp(ManagerAccessMixin):
     """
     The application singleton. Must be initialized prior to use.
 
@@ -31,71 +31,78 @@
         from silverback import SilverbackApp
 
         app = SilverbackApp()
 
         ...  # Connection has been initialized, can call broker methods e.g. `app.on_(...)`
     """
 
-    def __init__(self, settings: Optional[Settings] = None):
+    def __init__(self, settings: Settings | None = None):
         """
         Create app
 
         Args:
-            settings (Optional[~:class:`silverback.settings.Settings`]): Settings override.
+            settings (~:class:`silverback.settings.Settings` | None): Settings override.
                 Defaults to environment settings.
         """
         if not settings:
             settings = Settings()
 
-        self.network = settings.get_provider_context()
+        provider_context = settings.get_provider_context()
         # NOTE: This allows using connected ape methods e.g. `Contract`
-        provider = self.network.__enter__()
+        provider = provider_context.__enter__()
+
+        self.identifier = SilverbackID(
+            name=settings.APP_NAME,
+            network=provider.network.name,
+            ecosystem=provider.network.ecosystem.name,
+        )
 
         # Adjust defaults from connection
         if settings.NEW_BLOCK_TIMEOUT is None and (
             provider.network.name.endswith("-fork") or provider.network.name == LOCAL_NETWORK_NAME
         ):
             settings.NEW_BLOCK_TIMEOUT = int(timedelta(days=1).total_seconds())
 
         settings_str = "\n  ".join(f'{key}="{val}"' for key, val in settings.dict().items() if val)
         logger.info(f"Loading Silverback App with settings:\n  {settings_str}")
 
         self.broker = settings.get_broker()
         # NOTE: If no tasks registered yet, defaults to empty list instead of raising KeyError
         self.tasks: defaultdict[TaskType, list[TaskData]] = defaultdict(list)
-        self.poll_settings: Dict[str, Dict] = {}
+        self.poll_settings: dict[str, dict] = {}
 
-        atexit.register(self.network.__exit__, None, None, None)
+        atexit.register(provider_context.__exit__, None, None, None)
 
         self.signer = settings.get_signer()
         self.new_block_timeout = settings.NEW_BLOCK_TIMEOUT
         self.start_block = settings.START_BLOCK
 
-        network_str = f'\n  NETWORK="{provider.network.ecosystem.name}:{provider.network.name}"'
         signer_str = f"\n  SIGNER={repr(self.signer)}"
         start_block_str = f"\n  START_BLOCK={self.start_block}" if self.start_block else ""
         new_block_timeout_str = (
             f"\n  NEW_BLOCK_TIMEOUT={self.new_block_timeout}" if self.new_block_timeout else ""
         )
-        logger.info(
-            f"Loaded Silverback App:{network_str}"
+
+        network_choice = f"{self.identifier.ecosystem}:{self.identifier.network}"
+        logger.success(
+            f'Loaded Silverback App:\n  NETWORK="{network_choice}"'
             f"{signer_str}{start_block_str}{new_block_timeout_str}"
         )
 
     def broker_task_decorator(
         self,
         task_type: TaskType,
-        container: Union[BlockContainer, ContractEvent, None] = None,
+        container: BlockContainer | ContractEvent | None = None,
     ) -> Callable[[Callable], AsyncTaskiqDecoratedTask]:
         """
         Dynamically create a new broker task that handles tasks of ``task_type``.
 
         Args:
             task_type: :class:`~silverback.types.TaskType`: The type of task to create.
-            container: (Union[BlockContainer, ContractEvent]): The event source to watch.
+            container: (BlockContainer | ContractEvent): The event source to watch.
 
         Returns:
             Callable[[Callable], :class:`~taskiq.AsyncTaskiqDecoratedTask`]:
                 A function wrapper that will register the task handler.
 
         Raises:
             :class:`~silverback.exceptions.ContainerTypeMismatchError`:
@@ -116,19 +123,22 @@
         ):
             raise ContainerTypeMismatchError(task_type, container)
 
         # Register user function as task handler with our broker
         def add_taskiq_task(handler: Callable) -> AsyncTaskiqDecoratedTask:
             labels = {"task_type": str(task_type)}
 
-            if container and isinstance(container, ContractEvent):
+            # NOTE: Do *not* do `if container` because that does a `len(container)` call,
+            #       which for ContractEvent queries *every single log* ever emitted, and really
+            #       we only want to determine if it is not None
+            if container is not None and isinstance(container, ContractEvent):
                 # Address is almost a certainty if the container is being used as a filter here.
                 if contract_address := getattr(container.contract, "address", None):
                     labels["contract_address"] = contract_address
-                labels["event_signature"] = container.abi.signature
+                labels["event_signature"] = f"{container.abi.signature}"
 
             broker_task = self.broker.register_task(
                 handler,
                 task_name=handler.__name__,
                 **labels,
             )
 
@@ -183,26 +193,26 @@
             def do_something_on_shutdown(state):
                 ...  # Update some external service, perhaps using information from `state`.
         """
         return self.broker.on_event(TaskiqEvents.WORKER_SHUTDOWN)
 
     def on_(
         self,
-        container: Union[BlockContainer, ContractEvent],
-        new_block_timeout: Optional[int] = None,
-        start_block: Optional[int] = None,
+        container: BlockContainer | ContractEvent,
+        new_block_timeout: int | None = None,
+        start_block: int | None = None,
     ):
         """
         Create task to handle events created by `container`.
 
         Args:
-            container: (Union[BlockContainer, ContractEvent]): The event source to watch.
-            new_block_timeout: (Optional[int]): Override for block timeout that is acceptable.
+            container: (BlockContainer | ContractEvent): The event source to watch.
+            new_block_timeout: (int | None): Override for block timeout that is acceptable.
                 Defaults to whatever the app's settings are for default polling timeout are.
-            start_block (Optional[int]): block number to start processing events from.
+            start_block (int | None): block number to start processing events from.
                 Defaults to whatever the latest block is.
 
         Raises:
             :class:`~silverback.exceptions.InvalidContainerTypeError`:
                 If the type of `container` is not configurable for the app.
         """
         if isinstance(container, BlockContainer):
```

### Comparing `silverback-0.3.3/silverback/exceptions.py` & `silverback-0.4.0/silverback/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Any
+from typing import Any, Sequence
 
 from ape.exceptions import ApeException
-from ape.logging import logger
 
 from .types import TaskType
 
 
 class ImportFromStringError(Exception):
     pass
 
@@ -27,18 +26,31 @@
         )
 
 
 class SilverbackException(ApeException):
     """Base Exception for any Silverback runtime faults."""
 
 
+# TODO: `ExceptionGroup` added in Python 3.11
+class StartupFailure(SilverbackException):
+    def __init__(self, *exceptions: Sequence[Exception]):
+        if error_str := "\n".join(str(e) for e in exceptions):
+            super().__init__(f"Startup failure(s):\n{error_str}")
+        else:
+            super().__init__("Startup failure(s) detected. See logs for details.")
+
+
+class NoTasksAvailableError(SilverbackException):
+    def __init__(self):
+        super().__init__("No tasks to execute")
+
+
 class Halt(SilverbackException):
     def __init__(self):
         super().__init__("App halted, must restart manually")
 
 
-class CircuitBreaker(SilverbackException):
+class CircuitBreaker(Halt):
     """Custom exception (created by user) that will trigger an application shutdown."""
 
     def __init__(self, message: str):
-        logger.error(message)
-        super().__init__(message)
+        super(SilverbackException, self).__init__(message)
```

### Comparing `silverback-0.3.3/silverback/middlewares.py` & `silverback-0.4.0/silverback/middlewares.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,35 +2,30 @@
 
 from ape.logging import logger
 from ape.types import ContractLog
 from ape.utils import ManagerAccessMixin
 from eth_utils.conversions import to_hex
 from taskiq import TaskiqMessage, TaskiqMiddleware, TaskiqResult
 
-from silverback.persistence import HandlerResult
-from silverback.types import SilverbackID, TaskType
+from silverback.types import TaskType
 from silverback.utils import hexbytes_dict
 
 
 class SilverbackMiddleware(TaskiqMiddleware, ManagerAccessMixin):
     def __init__(self, *args, **kwargs):
         def compute_block_time() -> int:
             genesis = self.chain_manager.blocks[0]
             head = self.chain_manager.blocks.head
 
             if not head.number or head.number == 0:
                 return 10
 
             return int((head.timestamp - genesis.timestamp) / head.number)
 
-        settings = kwargs.pop("silverback_settings")
-
         self.block_time = self.chain_manager.provider.network.block_time or compute_block_time()
-        self.ident = SilverbackID.from_settings(settings)
-        self.persistence = settings.get_persistent_store()
 
     def pre_send(self, message: TaskiqMessage) -> TaskiqMessage:
         # TODO: Necessary because bytes/HexBytes doesn't encode/deocde well for some reason
         def fix_dict(data: dict, recurse_count: int = 0) -> dict:
             fixed_data: dict[str, Any] = {}
             for name, value in data.items():
                 if isinstance(value, bytes):
@@ -45,28 +40,36 @@
             return fixed_data
 
         message.args = [(fix_dict(arg) if isinstance(arg, dict) else arg) for arg in message.args]
 
         return message
 
     def _create_label(self, message: TaskiqMessage) -> str:
-        if labels_str := ",".join(f"{k}={v}" for k, v in message.labels.items()):
+        if labels_str := ",".join(
+            # NOTE: Have to add extra quotes around event signatures so they display as a string
+            f"{k}={v}" if k != "event_signature" else f'{k}="{v}"'
+            for k, v in message.labels.items()
+            if k != "task_name"
+        ):
             return f"{message.task_name}[{labels_str}]"
 
         else:
             return message.task_name
 
     def pre_execute(self, message: TaskiqMessage) -> TaskiqMessage:
+        # NOTE: Ensure we always have this, no matter what
+        message.labels["task_name"] = message.task_name
+
         if "task_type" not in message.labels:
             return message  # Not a silverback task
 
-        task_type = message.labels.pop("task_type")
+        task_type_str = message.labels.pop("task_type")
 
         try:
-            task_type = TaskType(task_type)
+            task_type = TaskType(task_type_str)
         except ValueError:
             return message  # Not a silverback task
 
         # Add extra labels for our task to see what their source was
         if task_type is TaskType.NEW_BLOCKS:
             # NOTE: Necessary because we don't know the exact block class
             block = message.args[0] = self.provider.network.ecosystem.decode_block(
@@ -93,25 +96,8 @@
         else:
             percent_display = ""
 
         (logger.error if result.error else logger.success)(
             f"{self._create_label(message)} " f"- {result.execution_time:.3f}s{percent_display}"
         )
 
-    async def post_save(self, message: TaskiqMessage, result: TaskiqResult):
-        if not self.persistence:
-            return
-
-        handler_result = HandlerResult.from_taskiq(
-            self.ident,
-            message.task_name,
-            message.labels.get("block_number"),
-            message.labels.get("log_index"),
-            result,
-        )
-
-        try:
-            await self.persistence.add_result(handler_result)
-        except Exception as err:
-            logger.error(f"Error storing result: {err}")
-
     # NOTE: Unless stdout is ignored, error traceback appears in stdout, no need for `on_error`
```

### Comparing `silverback-0.3.3/silverback/subscriptions.py` & `silverback-0.4.0/silverback/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import json
 from enum import Enum
-from typing import AsyncGenerator, Dict, List, Optional
+from typing import AsyncGenerator
 
 from ape.logging import logger
 from websockets import ConnectionClosedError
 from websockets import client as ws_client
 
 
 class SubscriptionType(Enum):
@@ -22,18 +22,18 @@
         # TODO: Temporary until a more permanent solution is added to ProviderAPI
         if "infura" in ws_provider_uri and "ws/v3" not in ws_provider_uri:
             ws_provider_uri = ws_provider_uri.replace("v3", "ws/v3")
 
         self._ws_provider_uri = ws_provider_uri
 
         # Stateful
-        self._connection: Optional[ws_client.WebSocketClientProtocol] = None
+        self._connection: ws_client.WebSocketClientProtocol | None = None
         self._last_request: int = 0
-        self._subscriptions: Dict[str, asyncio.Queue] = {}
-        self._rpc_msg_buffer: List[dict] = []
+        self._subscriptions: dict[str, asyncio.Queue] = {}
+        self._rpc_msg_buffer: list[dict] = []
         self._ws_lock = asyncio.Lock()
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} uri={self._ws_provider_uri}>"
 
     async def __aenter__(self) -> "Web3SubscriptionsManager":
         self.connection = await ws_client.connect(self._ws_provider_uri)
```

### Comparing `silverback-0.3.3/silverback/utils.py` & `silverback-0.4.0/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.3.3/silverback.egg-info/PKG-INFO` & `silverback-0.4.0/silverback.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.3.3
+Version: 0.4.0
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
@@ -42,15 +41,15 @@
 
 ## Documentation
 
 Read the [development userguide](https://docs.apeworx.io/silverback/stable/userguides/development.html) to learn more how to develop an application.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.10 or greater, python3-dev
 
 ## Installation
 
 Silverback relies heavily on the Ape development framework, so it's worth it to familarize yourself with how to install Ape and it's plugins using the [Ape installation userguide](https://docs.apeworx.io/ape/latest/userguides/quickstart#installation).
 
 ### via `pip`
 
@@ -76,20 +75,22 @@
 
 To run your bot against a live network, this SDK includes a simple runner you can use via:
 
 ```sh
 $ silverback run "example:app" --network :mainnet:alchemy
 ```
 
-**NOTE**: The example is designed to work with Python 3.9+, and we suggest using 3.11+ for speed.
+**NOTE**: The example is designed to work with Python 3.10+, and we suggest using 3.11+ for speed.
 
 ## Docker Usage
 
 ```sh
 $ docker run --volume $PWD:/home/harambe/project --volume ~/.tokenlists:/home/harambe/.tokenlists apeworx/silverback:latest run "example:app" --network :mainnet:alchemy
 ```
 
+**NOTE**: The Docker image we publish uses Python 3.11
+
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `silverback-0.3.3/silverback.egg-info/SOURCES.txt` & `silverback-0.4.0/silverback.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 docs/userguides/quickstart.md
 silverback/__init__.py
 silverback/_cli.py
 silverback/_importer.py
 silverback/application.py
 silverback/exceptions.py
 silverback/middlewares.py
-silverback/persistence.py
 silverback/py.typed
+silverback/recorder.py
 silverback/runner.py
 silverback/settings.py
+silverback/state.py
 silverback/subscriptions.py
 silverback/types.py
 silverback/utils.py
 silverback/version.py
 silverback.egg-info/PKG-INFO
 silverback.egg-info/SOURCES.txt
 silverback.egg-info/dependency_links.txt
```

### Comparing `silverback-0.3.3/silverback.egg-info/requires.txt` & `silverback-0.4.0/silverback.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 click
-eth-ape<1.0,>=0.7.0
+eth-ape<1.0,>=0.7
 ethpm-types>=0.6.10
 eth-pydantic-types
 pydantic_settings
 taskiq[metrics]<0.11.0,>=0.10.4
 
 [dev]
 pytest>=6.0
```

