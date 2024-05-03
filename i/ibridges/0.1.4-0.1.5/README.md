# Comparing `tmp/ibridges-0.1.4.tar.gz` & `tmp/ibridges-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibridges-0.1.4.tar", last modified: Wed Apr 17 12:04:19 2024, max compression
+gzip compressed data, was "ibridges-0.1.5.tar", last modified: Fri May  3 10:03:07 2024, max compression
```

## Comparing `ibridges-0.1.4.tar` & `ibridges-0.1.5.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.295724 ibridges-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:04:10.000000 ibridges-0.1.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.275724 ibridges-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.275724 ibridges-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/integration-tests-irods.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/integration-tests-yoda.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-17 12:04:10.000000 ibridges-0.1.4/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-17 12:04:10.000000 ibridges-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-17 12:04:10.000000 ibridges-0.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 12:04:10.000000 ibridges-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-17 12:04:19.295724 ibridges-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-17 12:04:10.000000 ibridges-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog/init-user-db.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_catalog_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog_provider/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog_provider/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_catalog_provider/setup-4.3.1.input
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.275724 ibridges-0.1.4/docker/irods_client/environments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/environments/plain-irods/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/plain-irods/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/plain-irods/irods_environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/environments/yoda/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/yoda/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/environments/yoda/irods_environment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/beach.rtf
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/bunny.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/example.r
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.279724 ibridges-0.1.4/docker/irods_client/testdata/more_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/more_data/polarbear.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/plant.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/testdata/sun.rtf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.283724 ibridges-0.1.4/docker/irods_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_data_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker/irods_client/tests/test_ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 12:04:10.000000 ibridges-0.1.4/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.283724 ibridges-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.283724 ibridges-0.1.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-17 12:04:10.000000 ibridges-0.1.4/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/ibridges/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/data_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/export_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/icat_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-17 12:04:10.000000 ibridges-0.1.4/ibridges/tickets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.291724 ibridges-0.1.4/ibridges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 12:04:19.000000 ibridges-0.1.4/ibridges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-17 12:04:10.000000 ibridges-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:04:19.295724 ibridges-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 12:04:10.000000 ibridges-0.1.4/tests/test_irodspath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-17 12:04:10.000000 ibridges-0.1.4/tests/testdata/bunny.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tests/testdata/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 12:04:10.000000 ibridges-0.1.4/tests/testdata/subfolder/sun.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/01-Setup-and-connect.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/02-Working-with-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/03-iRODS-Paths.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/04-Metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/05-Data-Sharing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/Data_sync.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24498 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/QuickStart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.287724 ibridges-0.1.4/tutorials/example_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/example_rules/example.r
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/iRODS_paths.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:04:19.291724 ibridges-0.1.4/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject1.png
--rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject2.png
--rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject3.png
--rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject4.png
--rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject5.png
--rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/DataObject6.png
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/Save_json.png
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-17 12:04:10.000000 ibridges-0.1.4/tutorials/img/Yoda_environment.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.931883 ibridges-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:03:00.000000 ibridges-0.1.5/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.907883 ibridges-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.911883 ibridges-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.911883 ibridges-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/integration-tests-irods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/integration-tests-yoda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-03 10:03:00.000000 ibridges-0.1.5/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-03 10:03:00.000000 ibridges-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 10:03:00.000000 ibridges-0.1.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 10:03:00.000000 ibridges-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-03 10:03:07.931883 ibridges-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-03 10:03:00.000000 ibridges-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.911883 ibridges-0.1.5/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog/init-user-db.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_catalog_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/setup-4.3.1.input
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_catalog_provider/setup-4.3.2.input
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.907883 ibridges-0.1.5/docker/irods_client/environments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/environments/plain-irods/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/plain-irods/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/plain-irods/irods_environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/environments/yoda/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/yoda/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/environments/yoda/irods_environment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/beach.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/bunny.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/example.r
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.915883 ibridges-0.1.5/docker/irods_client/testdata/more_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/more_data/polarbear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/plant.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/testdata/sun.rtf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.919883 ibridges-0.1.5/docker/irods_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_data_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker/irods_client/tests/test_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 10:03:00.000000 ibridges-0.1.5/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.919883 ibridges-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.919883 ibridges-0.1.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-03 10:03:00.000000 ibridges-0.1.5/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/ibridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/data_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/export_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/icat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-03 10:03:00.000000 ibridges-0.1.5/ibridges/tickets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.931883 ibridges-0.1.5/ibridges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 10:03:07.000000 ibridges-0.1.5/ibridges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-03 10:03:00.000000 ibridges-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 10:03:07.931883 ibridges-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 10:03:00.000000 ibridges-0.1.5/tests/test_irodspath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-05-03 10:03:00.000000 ibridges-0.1.5/tests/testdata/bunny.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.923883 ibridges-0.1.5/tests/testdata/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 10:03:00.000000 ibridges-0.1.5/tests/testdata/subfolder/sun.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.927883 ibridges-0.1.5/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/01-Setup-and-connect.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/02-Working-with-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/03-iRODS-Paths.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/04-Metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/05-Data-Sharing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/Data_sync.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/QuickStart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.927883 ibridges-0.1.5/tutorials/example_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/example_rules/example.r
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/iRODS_paths.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 10:03:07.931883 ibridges-0.1.5/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/DataObject6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/Save_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-03 10:03:00.000000 ibridges-0.1.5/tutorials/img/Yoda_environment.png
```

### Comparing `ibridges-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `ibridges-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `ibridges-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.github/workflows/integration-tests-irods.yml` & `ibridges-0.1.5/.github/workflows/integration-tests-irods.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.github/workflows/integration-tests-yoda.yml` & `ibridges-0.1.5/.github/workflows/integration-tests-yoda.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.github/workflows/main.yml` & `ibridges-0.1.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.github/workflows/pypi_release.yml` & `ibridges-0.1.5/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.gitignore` & `ibridges-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/.readthedocs.yaml` & `ibridges-0.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/LICENSE` & `ibridges-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/PKG-INFO` & `ibridges-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ibridges-0.1.4/README.md` & `ibridges-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/.gitattributes` & `ibridges-0.1.5/docker/.gitattributes`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/README.md` & `ibridges-0.1.5/docker/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_catalog_provider/Dockerfile` & `ibridges-0.1.5/docker/irods_catalog_provider/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 RUN sudo echo "deb [arch=amd64] https://packages.irods.org/apt/ $(lsb_release -sc) main" |sudo tee /etc/apt/sources.list.d/renci-irods.list
 
 RUN apt-get update
 RUN apt-get install -y python3 unixodbc
 RUN apt-get clean && \
     rm -rf /var/lib/apt/lists/* /tmp/*
 
-ARG irods_version=4.3.1
+ARG irods_version=4.3.2
 ARG irods_package_version_suffix=-0~${os_name}
 ARG irods_package_version=${irods_version}${irods_package_version_suffix}
 #ARG irods_resource_plugin_version=${irods_version}.0${irods_package_version_suffix}
 
 RUN apt-get update && \
     apt-get install -y irods-database-plugin-postgres=$irods_package_version
 RUN apt-get install irods-server=$irods_package_version
```

### Comparing `ibridges-0.1.4/docker/irods_catalog_provider/entrypoint.sh` & `ibridges-0.1.5/docker/irods_catalog_provider/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/Dockerfile` & `ibridges-0.1.5/docker/irods_client/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/entrypoint.sh` & `ibridges-0.1.5/docker/irods_client/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/environments/yoda/config.toml` & `ibridges-0.1.5/docker/irods_client/environments/yoda/config.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 password = "test"
 server_version = "4.2.12"
 can_write_pam_pass = false
 create_session_from_cached_pw = false
-resources = ["bundleResc", "demoResc", "dev001", "dev001_1", "dev001_2", "dev001_p1", "dev001_p2", "dev002", "dev002_1", "dev002_p1", "dev003", "dev003_1", "dev003_p1", "irodsResc", "irodsRescRepl", "irodsRescReplS3"]
+resources = ["demoResc", "dev001", "dev001_1", "dev001_2", "dev001_p1", "dev001_p2", "dev002", "dev002_1", "dev002_p1", "dev003", "dev003_1", "dev003_p1", "irodsResc", "irodsRescRepl", "irodsRescReplS3"]
 free_resources = [false, false, false, false, false, false, false, false, false, false, false, false, false, false, false, false]
 test_user = "researcher"
 test_user_pw = "test"
 ticket_date_only = true
```

### Comparing `ibridges-0.1.4/docker/irods_client/environments/yoda/irods_environment.json` & `ibridges-0.1.5/docker/irods_client/environments/yoda/irods_environment.json`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/testdata/beach.rtf` & `ibridges-0.1.5/docker/irods_client/testdata/beach.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/testdata/bunny.rtf` & `ibridges-0.1.5/docker/irods_client/testdata/bunny.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/testdata/more_data/polarbear.txt` & `ibridges-0.1.5/docker/irods_client/testdata/more_data/polarbear.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/testdata/plant.rtf` & `ibridges-0.1.5/docker/irods_client/testdata/plant.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/testdata/sun.rtf` & `ibridges-0.1.5/docker/irods_client/testdata/sun.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/conftest.py` & `ibridges-0.1.5/docker/irods_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_cli.py` & `ibridges-0.1.5/docker/irods_client/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_data_ops.py` & `ibridges-0.1.5/docker/irods_client/tests/test_data_ops.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_meta.py` & `ibridges-0.1.5/docker/irods_client/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_permissions.py` & `ibridges-0.1.5/docker/irods_client/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_session.py` & `ibridges-0.1.5/docker/irods_client/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_sync.py` & `ibridges-0.1.5/docker/irods_client/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker/irods_client/tests/test_ticket.py` & `ibridges-0.1.5/docker/irods_client/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docker-compose.yml` & `ibridges-0.1.5/docker-compose.yml`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         build:
             context: ./docker/irods_catalog_provider
         depends_on:
             - irods-catalog
 
     irods-client:
         image: irods-client
+        platform: linux/amd64
         build:
             context: .
             dockerfile: ./docker/irods_client/Dockerfile
         depends_on:
             - irods-catalog-provider
         tty: true
         environment:
```

### Comparing `ibridges-0.1.4/docs/Makefile` & `ibridges-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/make.bat` & `ibridges-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/source/api.rst` & `ibridges-0.1.5/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/source/cli.rst` & `ibridges-0.1.5/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/source/conf.py` & `ibridges-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/source/faq.rst` & `ibridges-0.1.5/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/source/index.rst` & `ibridges-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/docs/source/quickstart.rst` & `ibridges-0.1.5/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/__init__.py` & `ibridges-0.1.5/ibridges/__init__.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/__main__.py` & `ibridges-0.1.5/ibridges/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """CLI pointing to different entrypoints."""
     # show help by default, else consume first argument
     subcommand = "--help" if len(sys.argv) < 2 else sys.argv.pop(1)
 
     if subcommand in ["-h", "--help"]:
         print(MAIN_HELP_MESSAGE)
     elif subcommand in ["-v", "--version"]:
-        print(f"Metasyn CLI version {version('metasyn')}")
+        print(f"iBridges version {version('ibridges')}")
 
     # find the subcommand in this module and run it!
     elif subcommand == "download":
         ibridges_download()
     elif subcommand == "upload":
         ibridges_upload()
     elif subcommand == "sync":
@@ -151,37 +151,34 @@
         nargs="?",
     )
 
     args, _ = parser.parse_known_args()
     with interactive_auth(irods_env_path=_get_ienv_path()) as session:
         _list_coll(session, _parse_remote(args.remote_path, session))
 
-
-def _convert_path(remote_or_local: Union[str, Path]) -> Union[Path, str]:
-    if isinstance(remote_or_local, Path):
-        return remote_or_local
-    if remote_or_local.startswith("irods:"):
-        return remote_or_local[6:]
-    return Path(remote_or_local)
-
-
 def _parse_local(local_path: Union[None, str, Path]) -> Path:
     if local_path is None:
         return Path.cwd()
     if isinstance(local_path, str):
         if local_path.startswith("irods:"):
             raise ValueError("Please provide a local path (not starting with 'irods:')")
         local_path = Path(local_path)
     return local_path
 
 def _parse_remote(remote_path: Union[None, str], session: Session) -> IrodsPath:
     if remote_path is None:
         return IrodsPath(session, session.home)
     if not remote_path.startswith("irods:"):
-        raise ValueError("Please provide a remote path starting with 'irods:'")
+        raise ValueError("Please provide a remote path starting with 'irods:'.")
+    if remote_path.startswith("irods://"):
+        remainder = remote_path[8:]
+        print(remainder)
+        if remainder.startswith("~"):
+            return IrodsPath(session, remainder)
+        return IrodsPath(session, remote_path[7:])
     return IrodsPath(session, remote_path[6:])
 
 def ibridges_download():
     """Download a remote data object or collection."""
     parser = argparse.ArgumentParser(
         prog="ibridges download",
         description="Download a data object or collection from an iRODS server."
```

### Comparing `ibridges-0.1.4/ibridges/data_operations.py` & `ibridges-0.1.5/ibridges/data_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -148,15 +148,14 @@
     obj_exists = IrodsPath(session,
                            irods_path / local_path.name).dataobject_exists() \
                  or irods_path.dataobject_exists()
 
     if options is None:
         options = {}
     options.update({
-        kw.ALL_KW: '',
         kw.NUM_THREADS_KW: NUM_THREADS,
         kw.REG_CHKSUM_KW: '',
         kw.VERIFY_CHKSUM_KW: ''
     })
 
     if resc_name not in ['', None]:
         options[kw.RESC_NAME_KW] = resc_name
@@ -195,14 +194,17 @@
         kw.NUM_THREADS_KW: NUM_THREADS,
         kw.VERIFY_CHKSUM_KW: '',
         })
     if overwrite:
         options[kw.FORCE_FLAG_KW] = ''
     if resc_name not in ['', None]:
         options[kw.RESC_NAME_KW] = resc_name
+    #Quick fix for #126
+    if Path(local_path).is_dir():
+        local_path = Path(local_path).joinpath(irods_path.parts[-1])
     session.irods_session.data_objects.get(str(irods_path), local_path, **options)
 
 def _create_irods_dest(local_path: Path, irods_path: IrodsPath
                        ) -> list[tuple[Path, IrodsPath]]:
     """Assembles the irods destination paths for upload of a folder."""
     upload_path = irods_path.joinpath(local_path.name)
     paths = [(str(Path(root).relative_to(local_path)), f)
@@ -210,18 +212,26 @@
 
     source_to_dest = [(local_path.joinpath(folder.lstrip(os.sep), file_name),
                        upload_path.joinpath(folder.lstrip(os.sep), file_name))
                        for folder, file_name in paths]
 
     return source_to_dest
 
+def _create_irods_subtree(local_path: Path, irods_path: IrodsPath):
+    # create all collections from folders including empty ones
+    folders = [Path(root).relative_to(local_path).joinpath(f)
+               for root, folders, _ in os.walk(local_path) for f in folders]
+    for folder in folders:
+        IrodsPath.create_collection(irods_path.session,
+                                    irods_path.joinpath(local_path.parts[-1], *folder.parts))
+
 def _upload_collection(session: Session, local_path: Union[str, Path],
                        irods_path: Union[str, IrodsPath],
                        overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
-                       options: Optional[dict] = None):
+                       copy_empty_folders: bool = True, options: Optional[dict] = None):
     """Upload a local directory to iRODS.
 
     Parameters
     ----------
     session :
         Session to upload the collection to.
     local_path : Path
@@ -232,24 +242,28 @@
         If data already exists on iRODS, overwrite
     ignore_err : bool
         If an error occurs during upload, and ignore_err is set to True, any errors encountered
         will be transformed into warnings and iBridges will continue to upload the remaining files.
         By default all errors will stop the process of uploading.
     resc_name : str
         Name of the resource to which data is uploaded, by default the server will decide
+    copy_empty_folders : bool
+        Create collection even if the corresponding source folder is empty.
     options : dict
         More options for the upload
 
     """
     local_path = Path(local_path)
     irods_path = IrodsPath(session, irods_path)
     # get all files and their relative path to local_path
     if not local_path.is_dir():
         raise ValueError("local_path must be a directory.")
 
+    if copy_empty_folders:
+        _create_irods_subtree(local_path, irods_path)
     source_to_dest = _create_irods_dest(local_path, irods_path)
     for source, dest in source_to_dest:
         _ = create_collection(session, dest.parent)
         try:
             _obj_put(session, source, dest, overwrite, resc_name, options)
         except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG:
             warnings.warn(f'Object already exists\tSkipping {source}')
@@ -271,18 +285,27 @@
     for subcoll_path, obj_name, _, _ in all_objs:
         cur_ipath = IrodsPath(session, subcoll_path, obj_name)
         cur_lpath = (download_path / IrodsPath(session, subcoll_path).relative_to(irods_path)
                                    / obj_name)
         source_to_dest.append((cur_ipath, cur_lpath))
     return source_to_dest
 
+def _create_local_subtree(session: Session, irods_path: IrodsPath, local_path: Path):
+
+    coll = get_collection(session, irods_path)
+    subcolls = _get_subcoll_paths(session, coll)
+    # create all folders from collections including empty ones
+    folders = [local_path.joinpath(coll.name, *sc.relative_to(irods_path).parts)
+               for sc in subcolls]
+    for folder in folders:
+        folder.mkdir(parents=True, exist_ok=True)
 
 def _download_collection(session: Session, irods_path: Union[str, IrodsPath], local_path: Path,
                          overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
-                         options: Optional[dict] = None):
+                         copy_empty_folders: bool = True, options: Optional[dict] = None):
     """Download a collection to the local filesystem.
 
     Parameters
     ----------
     session :
         Session to download the collection from.
     irods_path : IrodsPath
@@ -294,22 +317,26 @@
     ignore_err : bool
         If an error occurs during download, and ignore_err is set to True, any errors encountered
         will be transformed into warnings and iBridges will continue to download the remaining
         files.
         By default all errors will stop the process of uploading.
     resc_name : str
         Name of the resource from which data is downloaded, by default the server will decide
+    copy_empty_folders : bool 
+        Create a respective folder for empty colletions.
     options : dict
         More options for the download
 
     """
     irods_path = IrodsPath(session, irods_path)
     if not irods_path.collection_exists():
         raise ValueError("irods_path must be a collection.")
 
+    if copy_empty_folders:
+        _create_local_subtree(session, irods_path, local_path)
     source_to_dest = _create_local_dest(session, irods_path, local_path)
 
     for source, dest in source_to_dest:
         # ensure local folder exists
         if not dest.parent.is_dir():
             os.makedirs(dest.parent)
         try:
@@ -320,15 +347,15 @@
             if ignore_err is True:
                 warnings.warn(f'Download failed: {source}i\n'+repr(e))
             else:
                 raise ValueError(f'Download failed: {source}: '+repr(e)) from e
 
 def upload(session: Session, local_path: Union[str, Path], irods_path: Union[str, IrodsPath],
            overwrite: bool = False, ignore_err: bool = False,
-           resc_name: str = '', options: Optional[dict] = None):
+           resc_name: str = '', copy_empty_folders: bool = True, options: Optional[dict] = None):
     """Upload a local directory or file to iRODS.
 
     Parameters
     ----------
     session :
         Session to upload the data to.
     local_path : Path
@@ -339,44 +366,46 @@
         If data object or collection already exists on iRODS, overwrite
     ignore_err : bool
         If an error occurs during upload, and ignore_err is set to True, any errors encountered
         will be transformed into warnings and iBridges will continue to upload the remaining files.
         By default all errors will stop the process of uploading.
     resc_name : str
         Name of the resource to which data is uploaded, by default the server will decide
+    copy_empty_folders : bool
+        Create respective iRODS collection for empty folders. Default: True.
     options : dict
         More options for the upload
 
     Raises
     ------
     ValueError:
         If the local_path is not a valid filename of directory.
     PermissionError:
-        If the iRods server does not allow the collection or data object to be created.
+        If the iRODS server does not allow the collection or data object to be created.
 
     """
     local_path = Path(local_path)
     try:
         if local_path.is_dir():
             _upload_collection(session, local_path, irods_path, overwrite, ignore_err,
-                               resc_name, options)
+                               resc_name, copy_empty_folders, options)
         elif local_path.is_file():
             _obj_put(session, local_path, irods_path, overwrite, resc_name, options)
         else:
             raise FileNotFoundError(f"Cannot find local file '{local_path}', check the path.")
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
         raise PermissionError(
             f"During upload operation to '{irods_path}': iRODS server forbids action.") from exc
     except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG as exc:
         raise FileExistsError(f"Dataset or collection (in) {irods_path} already exists. "
                               "Use overwrite=True to overwrite the existing file(s).") from exc
 
 def download(session: Session, irods_path: Union[str, IrodsPath], local_path: Union[str, Path],
              overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
-             options: Optional[dict] = None):
+             copy_empty_folders: bool = True, options: Optional[dict] = None):
     """Download a collection or data object to the local filesystem.
 
     Parameters
     ----------
     session :
         Session to download the collection from.
     irods_path : IrodsPath
@@ -388,32 +417,34 @@
         will be transformed into warnings and iBridges will continue to download the remaining
         files.
         By default all errors will stop the process of downloading.
     ignore_err : bool
         Collections: If download of an item fails print error and continue with next item.
     resc_name : str
         Name of the resource from which data is downloaded, by default the server will decide.
+    copy_empty_folders : bool
+        Create respective local directory for empty collections.
     options : dict
         More options for the download
 
     Raises
     ------
     PermissionError:
-        If the iRods server (for whatever reason) forbids downloading the file or
+        If the iRODS server (for whatever reason) forbids downloading the file or
         (part of the) collection.
     ValueError:
         If the irods_path is not pointing to either a collection or a data object.
 
     """
     irods_path = IrodsPath(session, irods_path)
     local_path = Path(local_path)
     try:
         if irods_path.collection_exists():
             _download_collection(session, irods_path, local_path, overwrite, ignore_err, resc_name,
-                                 options)
+                                 copy_empty_folders, options)
         elif irods_path.dataobject_exists():
             _obj_get(session, irods_path, local_path, overwrite, resc_name, options)
         else:
             raise ValueError(f"Data object or collection not found: '{irods_path}'")
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
         raise PermissionError(
             f"During download operation from '{irods_path}': iRODS server forbids action."
@@ -471,14 +502,24 @@
     data_query = data_query.filter(icat.LIKE(icat.COLL_NAME, coll.path+"/%"))
     for res in data_query.get_results():
         path, name, size, checksum = res.values()
         objs.append((path, name, size, checksum))
 
     return objs
 
+def _get_subcoll_paths(session: Session,
+                     coll: irods.collection.iRODSCollection) -> list:
+    """
+    Retrieves all sub collections in a sub tree starting at coll and returns their IrodsPaths.
+    """
+    coll_query = session.irods_session.query(icat.COLL_NAME)
+    coll_query = coll_query.filter(icat.LIKE(icat.COLL_NAME, coll.path+"/%"))
+
+    return [IrodsPath(session, p) for r in coll_query.get_results() for p in r.values()]
+
 def create_collection(session: Session,
                       coll_path: Union[IrodsPath, str]) -> irods.collection.iRODSCollection:
     """Create a collection and all collections in its path.
 
     Parameters
     ----------
     session:
```

### Comparing `ibridges-0.1.4/ibridges/export_metadata.py` & `ibridges-0.1.5/ibridges/export_metadata.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/icat_columns.py` & `ibridges-0.1.5/ibridges/icat_columns.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/interactive.py` & `ibridges-0.1.5/ibridges/interactive.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/meta.py` & `ibridges-0.1.5/ibridges/meta.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/path.py` & `ibridges-0.1.5/ibridges/path.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/permissions.py` & `ibridges-0.1.5/ibridges/permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/resources.py` & `ibridges-0.1.5/ibridges/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
         """
         if self._resources is None or update:
             query = self.session.irods_session.query(
                 icat.RESC_NAME, icat.RESC_PARENT, icat.RESC_STATUS, icat.RESC_CONTEXT)
             resc_list = []
             for item in query.get_results():
                 name, parent, status, context = item.values()
+                if name == 'bundleResc':
+                    continue
                 free_space = 0
                 if parent is None:
                     free_space = self.get_free_space(name)
                 metadata = {
                     'parent': parent,
                     'status': status,
                     'context': context,
```

### Comparing `ibridges-0.1.4/ibridges/rules.py` & `ibridges-0.1.5/ibridges/rules.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Rule operations."""
 import logging
-
+from typing import Optional
 import irods.exception
 import irods.rule
 
 from ibridges.session import Session
 
 
-def execute_rule(session: Session, rule_file: str, params: dict,
-                 output: str = 'ruleExecOut') -> tuple:
+def execute_rule(session: Session,
+                 rule_file: Optional[str],
+                 params: Optional[dict],
+                 output: str = 'ruleExecOut',
+                 instance_name: str = 'irods_rule_engine_plugin-irods_rule_language-instance',
+                 **kwargs) -> tuple:
     """Execute an iRODS rule.
 
     params format example:
     >>> # Notice extra quotes for string literals
     >>> params = {
     >>>     '*obj': '"/zone/home/user"',
     >>>     '*name': '"attr_name"',
@@ -21,29 +25,37 @@
 
     Parameters
     ----------
     session : ibridges.session
         The irods session
     rule_file : str
         Name of the iRODS rule file, or a file-like object representing it.
-    params : dict
-        Rule arguments.
+    params: dict
+        Rule input variable(s).
     output : str
         Rule output variable(s).
+    instance_name : str
+        Changes between irods rule language and python rules.
+    kwargs : dict
+        optional irods rule parameters.
+        For more information: https://github.com/irods/python-irodsclient
 
     Returns
     -------
     tuple
         (stdout, stderr)
 
     """
     try:
         rule = irods.rule.Rule(
-            session.irods_session, rule_file=rule_file, params=params, output=output,
-            instance_name='irods_rule_engine_plugin-irods_rule_language-instance')
+            session.irods_session,
+            rule_file=rule_file,
+            params=params,
+            instance_name=instance_name,
+            output=output, **kwargs)
         out = rule.execute()
     except irods.exception.NetworkException as error:
         logging.info('Lost connection to iRODS server.')
         return '', repr(error)
     except irods.exception.SYS_HEADER_READ_LEN_ERR as error:
         logging.info('iRODS server hiccuped.  Check the results and try again.')
         return '', repr(error)
```

### Comparing `ibridges-0.1.4/ibridges/search.py` & `ibridges-0.1.5/ibridges/search.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/session.py` & `ibridges-0.1.5/ibridges/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     PAM_AUTH_PASSWORD_FAILED,
     NetworkException,
 )
 from irods.session import NonAnonymousLoginWithoutPassword, iRODSSession
 
 from ibridges import icat_columns as icat
 
+APP_NAME="ibridges"
+
 class Session:
     """Irods session authentication."""
 
     def __init__(self,
                  irods_env: Union[dict, str, Path],
                  password: Optional[str] = None,
                  irods_home: Optional[str] = None):
@@ -43,15 +45,15 @@
         Raises
         ------
         FileNotFoundError:
             If the irods_env parameter is interpreted as a file name and not found.
         TypeError:
             If the irods_env parameter is not a dict, str or Path.
         LoginError:
-            If the connection to the iRods server fails to establish.
+            If the connection to the iRODS server fails to establish.
 
         """
         irods_env_path = None
         if isinstance(irods_env, (str, Path)):
             irods_env_path = Path(irods_env)
             if not irods_env_path.is_file():
                 raise FileNotFoundError(f"Cannot find irods environment file '{irods_env}'")
@@ -67,28 +69,28 @@
         self.irods_session = self.connect()
         if irods_home is not None:
             self.home = irods_home
         if "irods_home" not in self._irods_env:
             self.home = '/'+self.zone+'/home/'+self.username
 
     def __enter__(self):
-        """Connect to the iRods server if not already connected."""
+        """Connect to the iRODS server if not already connected."""
         if not self.has_valid_irods_session():
             self.connect()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_trace_back):
-        """Disconnect from the iRods server."""
+        """Disconnect from the iRODS server."""
         self.close()
 
     @property
     def home(self) -> str:
         """Current working directory for irods.
 
-        In the iRods community this is known as 'irods_home', in file system terms
+        In the iRODS community this is known as 'irods_home', in file system terms
         it would be the current working directory.
 
         Returns
         -------
             The current working directory in the current session.
 
         """
@@ -167,37 +169,38 @@
         """
         if self.irods_session is not None:
             self.irods_session.do_configure = {}
             self.irods_session.cleanup()
             self.irods_session = None
 
     def authenticate_using_password(self) -> iRODSSession:
-        """Authenticate with the iRods server using a password."""
+        """Authenticate with the iRODS server using a password."""
         try:
             irods_session = irods.session.iRODSSession(password=self._password,
-                                                             **self._irods_env)
+                                                             **self._irods_env,
+                                                       application_name=APP_NAME)
             _ = irods_session.server_version
         except Exception as e:
             raise _translate_irods_error(e) from e
         if irods_session.server_version == ():
-            raise LoginError("iRodsServer does not return a server version.")
+            raise LoginError("iRODS server does not return a server version.")
         return irods_session
 
     def authenticate_using_auth_file(self) -> iRODSSession:
         """Authenticate with an authentication file."""
         try:
             irods_session = irods.session.iRODSSession(
-                irods_env_file=self._irods_env_path)
+                irods_env_file=self._irods_env_path, application_name=APP_NAME)
             _ = irods_session.server_version
         except NonAnonymousLoginWithoutPassword as e:
             raise ValueError("No cached password found.") from e
         except Exception as e:
             raise _translate_irods_error(e) from e
         if irods_session.server_version == ():
-            raise LoginError("iRodsServer does not return a server version.")
+            raise LoginError("iRODS server does not return a server version.")
         return irods_session
 
 
     def write_pam_password(self):
         """Store the password in the iRODS authentication file in obfuscated form."""
         connection = self.irods_session.pool.get_connection()
         pam_passwords = self.irods_session.pam_pw_negotiated
@@ -227,15 +230,15 @@
                 pass
         raise ValueError("'irods_default_resource' not set in iRODS configuration.")
 
     def __getattr__(self, item):
         """Pass through a few attributes from irods_session."""
         if item in ["host", "port", "username", "zone"]:
             if self.irods_session is None:
-                raise AttributeError("Need a valid iRods session to get '{item}'.")
+                raise AttributeError("Need a valid iRODS session to get '{item}'.")
             return getattr(self.irods_session, item)
         return super().__getattribute__(item)
 
     @property
     def server_version(self) -> tuple:
         """Retrieve version of the iRODS server.
 
@@ -287,15 +290,15 @@
 def _translate_irods_error(exc) -> Exception:  # pylint: disable=too-many-return-statements
     if isinstance(exc, NetworkException):
         if any((a.startswith('Client-Server negotiation failure') for a in exc.args)):
             return LoginError("Host, port, irods_client_server_policy or "
                               "irods_client_server_negotiation not set correctly in "
                               "irods_environment.json")
     if isinstance(exc, CAT_INVALID_USER):
-        return LoginError("User credentials are not accepted")
+        return PasswordError("User credentials are not accepted")
     if isinstance(exc, PAM_AUTH_PASSWORD_FAILED):
         return PasswordError("Wrong password")
     if isinstance(exc, CAT_PASSWORD_EXPIRED):
         return PasswordError("Cached password is expired")
     if isinstance(exc, CAT_INVALID_AUTHENTICATION):
         return PasswordError("Cached password is wrong")
     if isinstance(exc, ValueError):
```

### Comparing `ibridges-0.1.4/ibridges/sync.py` & `ibridges-0.1.5/ibridges/sync.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges/tickets.py` & `ibridges-0.1.5/ibridges/tickets.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/ibridges.egg-info/PKG-INFO` & `ibridges-0.1.5/ibridges.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibridges
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for accessing data and metadata on iRods servers.
 Author-email: Christine Staiger <c.staiger@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 Utrecht University
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ibridges-0.1.4/ibridges.egg-info/SOURCES.txt` & `ibridges-0.1.5/ibridges.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docker/.gitattributes
 docker/README.md
 docker/irods_catalog/Dockerfile
 docker/irods_catalog/init-user-db.sh
 docker/irods_catalog_provider/Dockerfile
 docker/irods_catalog_provider/entrypoint.sh
 docker/irods_catalog_provider/setup-4.3.1.input
+docker/irods_catalog_provider/setup-4.3.2.input
 docker/irods_client/Dockerfile
 docker/irods_client/entrypoint.sh
 docker/irods_client/environments/plain-irods/config.toml
 docker/irods_client/environments/plain-irods/irods_environment.json
 docker/irods_client/environments/plain-irods/irods_environment_testuser.json
 docker/irods_client/environments/yoda/config.toml
 docker/irods_client/environments/yoda/irods_environment.json
```

### Comparing `ibridges-0.1.4/pyproject.toml` & `ibridges-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tests/test_irodspath.py` & `ibridges-0.1.5/tests/test_irodspath.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tests/testdata/bunny.txt` & `ibridges-0.1.5/tests/testdata/bunny.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tests/testdata/subfolder/sun.csv` & `ibridges-0.1.5/tests/testdata/subfolder/sun.csv`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/01-Setup-and-connect.ipynb` & `ibridges-0.1.5/tutorials/01-Setup-and-connect.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/02-Working-with-data.ipynb` & `ibridges-0.1.5/tutorials/02-Working-with-data.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/03-iRODS-Paths.ipynb` & `ibridges-0.1.5/tutorials/03-iRODS-Paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/04-Metadata.ipynb` & `ibridges-0.1.5/tutorials/04-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/05-Data-Sharing.ipynb` & `ibridges-0.1.5/tutorials/05-Data-Sharing.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/Data_sync.ipynb` & `ibridges-0.1.5/tutorials/Data_sync.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/QuickStart.ipynb` & `ibridges-0.1.5/tutorials/QuickStart.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951011904761905%*

 * *Differences: {"'cells'": "{76: {'source': {insert: [(1, '### Execute an iRODS rule from a rule file:')], "*

 * *            "delete: [1]}}, 77: {'source': {insert: [(2, 'params = {}\\n'), (3, 'stdout, stderr = "*

 * *            "execute_rule(session, rule_file, params)')], delete: [2]}}, insert: [(79, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', '0a64b6b1'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['### Executing a rule or a microservice on the "*

 * *            "server.\\n', 'The variable `instance_n […]*

```diff
@@ -803,27 +803,28 @@
         },
         {
             "cell_type": "markdown",
             "id": "e99c08e5",
             "metadata": {},
             "source": [
                 "## Rules\n",
-                "Execute an iRODS rule from a rule file:"
+                "### Execute an iRODS rule from a rule file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3913b742",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges.rules import execute_rule\n",
                 "rule_file = \"example_rules/example.r\"\n",
-                "stdout, stderr = execute_rule(session, rule_file, {})"
+                "params = {}\n",
+                "stdout, stderr = execute_rule(session, rule_file, params)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "900f8ab2",
             "metadata": {},
@@ -831,14 +832,37 @@
             "source": [
                 "print(stdout)\n",
                 "print(stderr)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "0a64b6b1",
+            "metadata": {},
+            "source": [
+                "### Executing a rule or a microservice on the server.\n",
+                "The variable `instance_name` denotes which rule engine to use. Here we take the standard irods rule engine. Another possibility is the python rule engine. Please consult the [iRODS manual](https://docs.irods.org/4.3.2). The rule `printHello` is a standard microservice on all iRODS servers in the core rule engine."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6001026c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "rule_file  = None\n",
+                "params = None\n",
+                "std_out, std_err = execute_rule(session, rule_file, params, body = 'printHello',\n",
+                "                                instance_name = 'irods_rule_engine_plugin-irods_rule_language-instance')\n",
+                "print(stdout)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "97970ce3",
             "metadata": {},
             "source": [
                 "### Overwrite parameters in iRODS rules\n",
                 "iRODS rule files end with a line like `input *in=\"This is a string or a path or etc\"`. In this example there is an input parameter called `'*in'` and it takes the value `\"This is a string or a path or etc\"`. We can overwrite these values by passing a python dictionary:"
             ]
         },
@@ -1044,13 +1068,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.9.18"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ibridges-0.1.4/tutorials/iRODS_paths.ipynb` & `ibridges-0.1.5/tutorials/iRODS_paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/DataObject1.png` & `ibridges-0.1.5/tutorials/img/DataObject1.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/DataObject2.png` & `ibridges-0.1.5/tutorials/img/DataObject2.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/DataObject3.png` & `ibridges-0.1.5/tutorials/img/DataObject3.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/DataObject4.png` & `ibridges-0.1.5/tutorials/img/DataObject4.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/DataObject5.png` & `ibridges-0.1.5/tutorials/img/DataObject5.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/DataObject6.png` & `ibridges-0.1.5/tutorials/img/DataObject6.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/Save_json.png` & `ibridges-0.1.5/tutorials/img/Save_json.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.4/tutorials/img/Yoda_environment.png` & `ibridges-0.1.5/tutorials/img/Yoda_environment.png`

 * *Files identical despite different names*

