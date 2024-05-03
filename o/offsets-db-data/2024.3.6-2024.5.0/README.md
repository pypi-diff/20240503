# Comparing `tmp/offsets-db-data-2024.3.6.tar.gz` & `tmp/offsets_db_data-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offsets-db-data-2024.3.6.tar", last modified: Wed Mar 13 20:53:29 2024, max compression
+gzip compressed data, was "offsets_db_data-2024.5.0.tar", last modified: Fri May  3 18:38:18 2024, max compression
```

## Comparing `offsets-db-data-2024.3.6.tar` & `offsets_db_data-2024.5.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.525635 offsets-db-data-2024.3.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.525635 offsets-db-data-2024.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/TERMS_OF_DATA_ACCESS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.525635 offsets-db-data-2024.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/TERMS-OF-DATA-ACCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.525635 offsets-db-data-2024.3.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/_static/monogram-dark-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/_static/monogram-light-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/data-access.md
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/data-processing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/glossary.md
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/docs/install-offsets-db-data.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/offsets_db_data/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-13 20:53:29.000000 offsets-db-data-2024.3.6/offsets_db_data/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/apx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/arb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/offsets_db_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    84264 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/configs/all-protocol-mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/configs/credits-raw-columns-mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/configs/projects-raw-columns-mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/gld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/offsets_db_data/vcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/offsets_db_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-13 20:53:29.000000 offsets-db-data-2024.3.6/offsets_db_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-13 20:53:29.000000 offsets-db-data-2024.3.6/offsets_db_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 20:53:29.000000 offsets-db-data-2024.3.6/offsets_db_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-13 20:53:29.000000 offsets-db-data-2024.3.6/offsets_db_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-13 20:53:29.000000 offsets-db-data-2024.3.6/offsets_db_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:29.529635 offsets-db-data-2024.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-03-13 20:53:18.000000 offsets-db-data-2024.3.6/tests/test_vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/TERMS_OF_DATA_ACCESS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/TERMS-OF-DATA-ACCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/_static/monogram-dark-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/_static/monogram-light-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/data-access.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/data-processing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/glossary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/install-offsets-db-data.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.803181 offsets_db_data-2024.5.0/offsets_db_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/apx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/arb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.803181 offsets_db_data-2024.5.0/offsets_db_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    84264 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/configs/all-protocol-mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/configs/credits-raw-columns-mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/configs/projects-raw-columns-mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/gld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/offsets_db_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.803181 offsets_db_data-2024.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/tests/test_vcs.py
```

### Comparing `offsets-db-data-2024.3.6/.github/workflows/CI.yaml` & `offsets_db_data-2024.5.0/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/.github/workflows/pypi.yaml` & `offsets_db_data-2024.5.0/.github/workflows/pypi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -76,8 +76,8 @@
       id-token: write
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.12
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `offsets-db-data-2024.3.6/.gitignore` & `offsets_db_data-2024.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/.pre-commit-config.yaml` & `offsets_db_data-2024.5.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - id: check-json
       - id: check-yaml
       - id: double-quote-string-fixer
       - id: debug-statements
       - id: mixed-line-ending
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.0'
+    rev: 'v0.3.5'
     hooks:
       - id: ruff
         args: ['--fix']
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
```

### Comparing `offsets-db-data-2024.3.6/LICENSE` & `offsets_db_data-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/PKG-INFO` & `offsets_db_data-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: offsets-db-data
-Version: 2024.3.6
+Version: 2024.5.0
 Summary: Monitoring the global carbon market
 Author-email: CarbonPlan <tech@carbonplan.org>
 License: MIT
 Project-URL: repository, https://github.com/carbonplan/offsets-db-data
+Project-URL: documentation, https://offsets-db-data.readthedocs.io/
+Project-URL: database web tool, https://carbonplan.org/research/offsets-db
+Project-URL: explainer, https://carbonplan.org/research/offsets-db-explainer
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: country_converter==1.0.0
 Requires-Dist: dask==2023.9.3
 Requires-Dist: fastparquet==2023.10.0
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.3.6 Summary:
+Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.5.0 Summary:
 Monitoring the global carbon market Author-email: CarbonPlan
 carbonplan.org> License: MIT Project-URL: repository, https://github.com/
-carbonplan/offsets-db-data Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Intended Audience :: Science/Research Classifier:
+carbonplan/offsets-db-data Project-URL: documentation, https://offsets-db-
+data.readthedocs.io/ Project-URL: database web tool, https://carbonplan.org/
+research/offsets-db Project-URL: explainer, https://carbonplan.org/research/
+offsets-db-explainer Classifier: Development Status :: 4 - Beta Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: country_converter==1.0.0 Requires-Dist: dask==2023.9.3
-Requires-Dist: fastparquet==2023.10.0 Requires-Dist: fsspec==2023.10.0
-Requires-Dist: intake-parquet>=0.3.0 Requires-Dist: intake<2 Requires-Dist:
-pandas==2.1.1 Requires-Dist: pandera==0.17 Requires-Dist: pydantic==2.5.*
-Requires-Dist: pyjanitor==0.23.* Requires-Dist: requests>=2.31.0 Requires-Dist:
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+country_converter==1.0.0 Requires-Dist: dask==2023.9.3 Requires-Dist:
+fastparquet==2023.10.0 Requires-Dist: fsspec==2023.10.0 Requires-Dist: intake-
+parquet>=0.3.0 Requires-Dist: intake<2 Requires-Dist: pandas==2.1.1 Requires-
+Dist: pandera==0.17 Requires-Dist: pydantic==2.5.* Requires-Dist:
+pyjanitor==0.23.* Requires-Dist: requests>=2.31.0 Requires-Dist:
 s3fs==2023.10.0 Requires-Dist: universal_pathlib>=0.1.3
 _[_h_t_t_p_s_:_/_/_c_a_r_b_o_n_p_l_a_n_-_a_s_s_e_t_s_._s_3_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_o_n_o_g_r_a_m_/_d_a_r_k_-_s_m_a_l_l_._p_n_g_]_[_h_t_t_p_s_:_/_/
 _c_a_r_b_o_n_p_l_a_n_-_a_s_s_e_t_s_._s_3_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_o_n_o_g_r_a_m_/_l_i_g_h_t_-_s_m_a_l_l_._p_n_g_]
 [![CI](https://github.com/carbonplan/offsets-db-data/actions/workflows/CI.yaml/
 badge.svg)](https://github.com/carbonplan/offsets-db-data/actions/workflows/
 CI.yaml) [![PyPI](https://github.com/carbonplan/offsets-db-data/actions/
 workflows/pypi.yaml/badge.svg)](https://github.com/carbonplan/offsets-db-data/
```

### Comparing `offsets-db-data-2024.3.6/README.md` & `offsets_db_data-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/TERMS_OF_DATA_ACCESS` & `offsets_db_data-2024.5.0/TERMS_OF_DATA_ACCESS`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/TERMS-OF-DATA-ACCESS.md` & `offsets_db_data-2024.5.0/docs/TERMS-OF-DATA-ACCESS.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/_static/monogram-dark-cropped.png` & `offsets_db_data-2024.5.0/docs/_static/monogram-dark-cropped.png`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/_static/monogram-light-cropped.png` & `offsets_db_data-2024.5.0/docs/_static/monogram-light-cropped.png`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/api.md` & `offsets_db_data-2024.5.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/conf.py` & `offsets_db_data-2024.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/data-access.md` & `offsets_db_data-2024.5.0/docs/data-access.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/data-processing.md` & `offsets_db_data-2024.5.0/docs/data-processing.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/glossary.md` & `offsets_db_data-2024.5.0/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/index.md` & `offsets_db_data-2024.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/docs/install-offsets-db-data.md` & `offsets_db_data-2024.5.0/docs/install-offsets-db-data.md`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/apx.py` & `offsets_db_data-2024.5.0/offsets_db_data/apx.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/arb.py` & `offsets_db_data-2024.5.0/offsets_db_data/arb.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/catalog.yaml` & `offsets_db_data-2024.5.0/offsets_db_data/catalog.yaml`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/common.py` & `offsets_db_data-2024.5.0/offsets_db_data/common.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/configs/all-protocol-mapping.json` & `offsets_db_data-2024.5.0/offsets_db_data/configs/all-protocol-mapping.json`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/configs/credits-raw-columns-mapping.json` & `offsets_db_data-2024.5.0/offsets_db_data/configs/credits-raw-columns-mapping.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'american-carbon-registry'": "{'cancellations': {'transaction_date': 'Status Effective  (GMT)'}, "*

 * *                               "'issuances': {'transaction_date': 'Date Issued (GMT)'}, "*

 * *                               "'retirements': {'transaction_date': 'Status Effective (GMT)'}}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "american-carbon-registry": {
         "cancellations": {
             "project_id": "Project ID",
             "quantity": "Quantity of Credits",
-            "transaction_date": "Status Effective",
+            "transaction_date": "Status Effective  (GMT)",
             "vintage": "Vintage"
         },
         "issuances": {
             "project_id": "Project ID",
             "quantity": "Total Credits Issued",
-            "transaction_date": "Date Issued",
+            "transaction_date": "Date Issued (GMT)",
             "vintage": "Vintage"
         },
         "retirements": {
             "project_id": "Project ID",
             "quantity": "Quantity of Credits",
-            "transaction_date": "Status Effective",
+            "transaction_date": "Status Effective (GMT)",
             "vintage": "Vintage"
         }
     },
     "art-trees": {
         "cancellations": {
             "project_id": "Program ID",
             "quantity": "Quantity of Credits",
```

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/configs/projects-raw-columns-mapping.json` & `offsets_db_data-2024.5.0/offsets_db_data/configs/projects-raw-columns-mapping.json`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/credits.py` & `offsets_db_data-2024.5.0/offsets_db_data/credits.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/gld.py` & `offsets_db_data-2024.5.0/offsets_db_data/gld.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/models.py` & `offsets_db_data-2024.5.0/offsets_db_data/models.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/projects.py` & `offsets_db_data-2024.5.0/offsets_db_data/projects.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/registry.py` & `offsets_db_data-2024.5.0/offsets_db_data/registry.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data/vcs.py` & `offsets_db_data-2024.5.0/offsets_db_data/vcs.py`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/offsets_db_data.egg-info/PKG-INFO` & `offsets_db_data-2024.5.0/offsets_db_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: offsets-db-data
-Version: 2024.3.6
+Version: 2024.5.0
 Summary: Monitoring the global carbon market
 Author-email: CarbonPlan <tech@carbonplan.org>
 License: MIT
 Project-URL: repository, https://github.com/carbonplan/offsets-db-data
+Project-URL: documentation, https://offsets-db-data.readthedocs.io/
+Project-URL: database web tool, https://carbonplan.org/research/offsets-db
+Project-URL: explainer, https://carbonplan.org/research/offsets-db-explainer
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: country_converter==1.0.0
 Requires-Dist: dask==2023.9.3
 Requires-Dist: fastparquet==2023.10.0
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.3.6 Summary:
+Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.5.0 Summary:
 Monitoring the global carbon market Author-email: CarbonPlan
 carbonplan.org> License: MIT Project-URL: repository, https://github.com/
-carbonplan/offsets-db-data Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Intended Audience :: Science/Research Classifier:
+carbonplan/offsets-db-data Project-URL: documentation, https://offsets-db-
+data.readthedocs.io/ Project-URL: database web tool, https://carbonplan.org/
+research/offsets-db Project-URL: explainer, https://carbonplan.org/research/
+offsets-db-explainer Classifier: Development Status :: 4 - Beta Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: country_converter==1.0.0 Requires-Dist: dask==2023.9.3
-Requires-Dist: fastparquet==2023.10.0 Requires-Dist: fsspec==2023.10.0
-Requires-Dist: intake-parquet>=0.3.0 Requires-Dist: intake<2 Requires-Dist:
-pandas==2.1.1 Requires-Dist: pandera==0.17 Requires-Dist: pydantic==2.5.*
-Requires-Dist: pyjanitor==0.23.* Requires-Dist: requests>=2.31.0 Requires-Dist:
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+country_converter==1.0.0 Requires-Dist: dask==2023.9.3 Requires-Dist:
+fastparquet==2023.10.0 Requires-Dist: fsspec==2023.10.0 Requires-Dist: intake-
+parquet>=0.3.0 Requires-Dist: intake<2 Requires-Dist: pandas==2.1.1 Requires-
+Dist: pandera==0.17 Requires-Dist: pydantic==2.5.* Requires-Dist:
+pyjanitor==0.23.* Requires-Dist: requests>=2.31.0 Requires-Dist:
 s3fs==2023.10.0 Requires-Dist: universal_pathlib>=0.1.3
 _[_h_t_t_p_s_:_/_/_c_a_r_b_o_n_p_l_a_n_-_a_s_s_e_t_s_._s_3_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_o_n_o_g_r_a_m_/_d_a_r_k_-_s_m_a_l_l_._p_n_g_]_[_h_t_t_p_s_:_/_/
 _c_a_r_b_o_n_p_l_a_n_-_a_s_s_e_t_s_._s_3_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_o_n_o_g_r_a_m_/_l_i_g_h_t_-_s_m_a_l_l_._p_n_g_]
 [![CI](https://github.com/carbonplan/offsets-db-data/actions/workflows/CI.yaml/
 badge.svg)](https://github.com/carbonplan/offsets-db-data/actions/workflows/
 CI.yaml) [![PyPI](https://github.com/carbonplan/offsets-db-data/actions/
 workflows/pypi.yaml/badge.svg)](https://github.com/carbonplan/offsets-db-data/
```

### Comparing `offsets-db-data-2024.3.6/offsets_db_data.egg-info/SOURCES.txt` & `offsets_db_data-2024.5.0/offsets_db_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/pyproject.toml` & `offsets_db_data-2024.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -15,28 +15,32 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 
 
 dynamic = ["version", "dependencies"]
 
 [tool.setuptools.dynamic]
 
 dependencies = { file = ["requirements.txt"] }
 optional-dependencies = { dev = { file = ["requirements-dev.txt"] }, docs = { file = ["requirements-docs.txt"] } }
 
 
 [project.urls]
 repository = "https://github.com/carbonplan/offsets-db-data"
+"documentation" = "https://offsets-db-data.readthedocs.io/"
+"database web tool"= "https://carbonplan.org/research/offsets-db"
+"explainer" = "https://carbonplan.org/research/offsets-db-explainer"
 
 [tool.setuptools.packages.find]
 include = ["offsets_db_data*"]
 
 [tool.setuptools.package-data]
 offsets_db_data = ["py.typed", "configs/*.json", "*.yaml"]
 
@@ -121,11 +125,15 @@
 [tool.ruff.format]
 quote-style = "single"
 docstring-code-format = true
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
+[tool.ruff.lint.pyupgrade]
+# Preserve types, even if a file imports `from __future__ import annotations`.
+keep-runtime-typing = true
+
 
 [tool.pytest.ini_options]
 console_output_style = "count"
 addopts = "-n auto --cov=./ --cov-report=xml  --cov-report=term-missing --verbose"
```

### Comparing `offsets-db-data-2024.3.6/readthedocs.yml` & `offsets_db_data-2024.5.0/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `offsets-db-data-2024.3.6/tests/test_integration.py` & `offsets_db_data-2024.5.0/tests/test_integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from offsets_db_data.gld import *  # noqa: F403
 from offsets_db_data.models import credit_without_id_schema, project_schema
 from offsets_db_data.vcs import *  # noqa: F403
 
 
 @pytest.fixture
 def date() -> str:
-    return '2024-02-13'
+    return '2024-05-03'
 
 
 @pytest.fixture
 def bucket() -> str:
     return 's3://carbonplan-offsets-db/raw'
 
 
 @pytest.fixture
 def arb() -> pd.DataFrame:
     data = pd.read_excel(
-        's3://carbonplan-offsets-db/raw/2024-02-13/arb/nc-arboc_issuance.xlsx', sheet_name=3
+        's3://carbonplan-offsets-db/raw/2024-05-03/arb/nc-arboc_issuance.xlsx', sheet_name=3
     )
     return data.process_arb()
 
 
 def test_verra(date, bucket, arb):
     prefix = 'VCS'
     projects = pd.read_csv(f'{bucket}/{date}/verra/projects.csv.gz')
@@ -74,15 +74,15 @@
 ):
     registry = 'gold-standard'
     download_types = ['issuances', 'retirements']
     prefix = 'GLD'
 
     dfs = []
     for key in download_types:
-        credits = pd.read_csv(f'{bucket}/2024-02-13/{registry}/{key}.csv.gz')
+        credits = pd.read_csv(f'{bucket}/{date}/{registry}/{key}.csv.gz')
         p = credits.process_gld_credits(download_type=key)
         dfs.append(p)
 
     df_credits = pd.concat(dfs)
     credit_without_id_schema.validate(df_credits)
 
     assert set(df_credits.columns) == set(credit_without_id_schema.columns.keys())
@@ -99,28 +99,28 @@
 @pytest.mark.parametrize(
     'df_credits',
     [
         pd.DataFrame().process_gld_credits(download_type='issuances'),
         pd.concat(
             [
                 pd.read_csv(
-                    's3://carbonplan-offsets-db/raw/2024-02-13/gold-standard/issuances.csv.gz'
+                    's3://carbonplan-offsets-db/raw/2024-05-03/gold-standard/issuances.csv.gz'
                 ).process_gld_credits(download_type='issuances'),
                 pd.read_csv(
-                    's3://carbonplan-offsets-db/raw/2024-02-13/gold-standard/retirements.csv.gz'
+                    's3://carbonplan-offsets-db/raw/2024-05-03/gold-standard/retirements.csv.gz'
                 ).process_gld_credits(download_type='retirements'),
             ]
         ),
     ],
 )
 @pytest.mark.parametrize(
     'projects',
     [
         pd.DataFrame(),
-        pd.read_csv('s3://carbonplan-offsets-db/raw/2024-02-13/gold-standard/projects.csv.gz'),
+        pd.read_csv('s3://carbonplan-offsets-db/raw/2024-05-03/gold-standard/projects.csv.gz'),
     ],
 )
 def test_gld_empty(df_credits, projects):
     prefix = 'GLD'
 
     credit_without_id_schema.validate(df_credits)
```

### Comparing `offsets-db-data-2024.3.6/tests/test_vcs.py` & `offsets_db_data-2024.5.0/tests/test_vcs.py`

 * *Files identical despite different names*

