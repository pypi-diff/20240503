# Comparing `tmp/pyegeria-0.3.5.tar.gz` & `tmp/pyegeria-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegeria-0.3.5.tar", last modified: Mon Apr 29 05:50:14 2024, max compression
+gzip compressed data, was "pyegeria-0.3.6.tar", last modified: Fri May  3 11:28:52 2024, max compression
```

## Comparing `pyegeria-0.3.5.tar` & `pyegeria-0.3.6.tar`

### file list

```diff
@@ -1,110 +1,112 @@
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.566147 pyegeria-0.3.5/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.5/LICENSE
--rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-12 00:32:44.000000 pyegeria-0.3.5/MANIFEST.in
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-29 05:50:14.565961 pyegeria-0.3.5/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.5/README.md
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.547383 pyegeria-0.3.5/examples/
--rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:37:23.000000 pyegeria-0.3.5/examples/.DS_Store
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.550418 pyegeria-0.3.5/examples/Coco_config/
--rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-12 00:25:29.000000 pyegeria-0.3.5/examples/Coco_config/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS1.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS2.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS3.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS4.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS5.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDS6.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoMDSx.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_cocoView1.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_exchangeDL01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_governDL01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_monitorDev01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.5/examples/Coco_config/config_monitorGov01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-12 00:25:29.000000 pyegeria-0.3.5/examples/Coco_config/globals.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.550915 pyegeria-0.3.5/examples/Doc_Samples/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11865 2024-04-18 16:25:08.000000 pyegeria-0.3.5/examples/Doc_Samples/Create_Collection_Sample.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5049 2024-04-28 23:10:47.000000 pyegeria-0.3.5/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.551178 pyegeria-0.3.5/examples/Jupyter Notebooks/
--rw-r--r--   0 dwolfson   (501) staff       (20)   118151 2024-04-29 01:16:20.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/P-egeria-server-config.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)      170 2024-04-29 01:25:02.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/README.md
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.552255 pyegeria-0.3.5/examples/Jupyter Notebooks/common/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2914 2024-04-19 21:30:39.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/P-environment-check.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)      408 2024-03-20 02:16:23.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   276801 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/common-functions.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)     1449 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/environment-check.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)     7842 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/globals.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)     5900 2024-04-19 21:30:39.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5849 2024-03-18 16:53:11.000000 pyegeria-0.3.5/examples/Jupyter Notebooks/common/orig_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/__init__.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.552353 pyegeria-0.3.5/examples/__pycache__/
--rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.5/examples/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.556100 pyegeria-0.3.5/examples/widgets/
--rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:47:25.000000 pyegeria-0.3.5/examples/widgets/.DS_Store
--rw-r--r--   0 dwolfson   (501) staff       (20)     1696 2024-04-29 00:22:17.000000 pyegeria-0.3.5/examples/widgets/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-12 00:25:29.000000 pyegeria-0.3.5/examples/widgets/__init__.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.556466 pyegeria-0.3.5/examples/widgets/__pycache__/
--rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.5/examples/widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.5/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3157 2024-04-29 00:14:47.000000 pyegeria-0.3.5/examples/widgets/coco_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3642 2024-04-18 19:49:26.000000 pyegeria-0.3.5/examples/widgets/collection_viewer.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5206 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/engine_action_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5185 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/find_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4947 2024-04-25 14:18:41.000000 pyegeria-0.3.5/examples/widgets/get_relationship_types.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5299 2024-04-24 01:14:00.000000 pyegeria-0.3.5/examples/widgets/get_valid_metadata_values.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/glossary_view.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/gov_engine_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/integration_daemon_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3578 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/list_asset_types.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3704 2024-04-18 13:42:39.000000 pyegeria-0.3.5/examples/widgets/multi-server_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/my_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/open_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5448 2024-04-24 21:32:52.000000 pyegeria-0.3.5/examples/widgets/project_list_viewer.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/server_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-12 00:32:44.000000 pyegeria-0.3.5/examples/widgets/server_status_widget.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4619 2024-04-26 14:50:59.000000 pyegeria-0.3.5/examples/widgets/view_my_profile.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-04-29 05:49:49.000000 pyegeria-0.3.5/pyproject.toml
--rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-29 05:50:14.566185 pyegeria-0.3.5/setup.cfg
--rw-r--r--   0 dwolfson   (501) staff       (20)     2102 2024-04-12 00:32:44.000000 pyegeria-0.3.5/setup.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.546086 pyegeria-0.3.5/src/
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.561116 pyegeria-0.3.5/src/pyegeria/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1769 2024-04-23 16:53:51.000000 pyegeria-0.3.5/src/pyegeria/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/_exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.5/src/pyegeria/_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/_validators.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   100106 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   114200 2024-04-29 01:32:02.000000 pyegeria-0.3.5/src/pyegeria/collection_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    93140 2024-04-23 14:39:07.000000 pyegeria-0.3.5/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/governance_author.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42441 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    77305 2024-04-26 16:10:23.000000 pyegeria-0.3.5/src/pyegeria/project_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8775 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-12 00:32:44.000000 pyegeria-0.3.5/src/pyegeria/server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.5/src/pyegeria/utils.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    29710 2024-04-25 15:33:15.000000 pyegeria-0.3.5/src/pyegeria/valid_metadata_omvs.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.565648 pyegeria-0.3.5/src/pyegeria.egg-info/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     3407 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/SOURCES.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/dependency_links.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/requires.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-29 05:50:14.000000 pyegeria-0.3.5/src/pyegeria.egg-info/top_level.txt
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-29 05:50:14.565452 pyegeria-0.3.5/tests/
--rw-r--r--   0 dwolfson   (501) staff       (20)    18673 2024-04-29 01:39:21.000000 pyegeria-0.3.5/tests/test_automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    51872 2024-04-29 00:11:27.000000 pyegeria-0.3.5/tests/test_collection_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    59270 2024-04-15 22:01:18.000000 pyegeria-0.3.5/tests/test_core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.5/tests/test_full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     9625 2024-04-12 00:32:44.000000 pyegeria-0.3.5/tests/test_my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    40084 2024-04-23 14:27:57.000000 pyegeria-0.3.5/tests/test_platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    28529 2024-04-26 16:12:52.000000 pyegeria-0.3.5/tests/test_project_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4727 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_util_exp.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12782 2024-04-25 15:34:36.000000 pyegeria-0.3.5/tests/test_valid_metadata_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.5/tests/test_validators.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.458484 pyegeria-0.3.6/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.6/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-12 00:32:44.000000 pyegeria-0.3.6/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-05-03 11:28:52.458259 pyegeria-0.3.6/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.6/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.445855 pyegeria-0.3.6/examples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:37:23.000000 pyegeria-0.3.6/examples/.DS_Store
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.447482 pyegeria-0.3.6/examples/Coco_config/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-12 00:25:29.000000 pyegeria-0.3.6/examples/Coco_config/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDS1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDS2.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDS3.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDS4.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDS5.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDS6.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoMDSx.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_cocoView1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_exchangeDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_governDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_monitorDev01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.6/examples/Coco_config/config_monitorGov01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-12 00:25:29.000000 pyegeria-0.3.6/examples/Coco_config/globals.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.447727 pyegeria-0.3.6/examples/Doc_Samples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11865 2024-04-18 16:25:08.000000 pyegeria-0.3.6/examples/Doc_Samples/Create_Collection_Sample.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5049 2024-04-28 23:10:47.000000 pyegeria-0.3.6/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.448283 pyegeria-0.3.6/examples/Jupyter Notebooks/
+-rw-r--r--   0 dwolfson   (501) staff       (20)   118151 2024-04-29 01:16:20.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/P-egeria-server-config.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)      170 2024-04-29 01:25:02.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.449158 pyegeria-0.3.6/examples/Jupyter Notebooks/common/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2914 2024-04-19 21:30:39.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/P-environment-check.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)      408 2024-03-20 02:16:23.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   276801 2024-03-18 16:53:11.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/common-functions.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1449 2024-03-18 16:53:11.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/environment-check.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     7842 2024-03-18 16:53:11.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/globals.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5900 2024-04-19 21:30:39.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5849 2024-03-18 16:53:11.000000 pyegeria-0.3.6/examples/Jupyter Notebooks/common/orig_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.449256 pyegeria-0.3.6/examples/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.6/examples/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.451865 pyegeria-0.3.6/examples/widgets/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:47:25.000000 pyegeria-0.3.6/examples/widgets/.DS_Store
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1696 2024-04-29 00:22:17.000000 pyegeria-0.3.6/examples/widgets/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-12 00:25:29.000000 pyegeria-0.3.6/examples/widgets/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.452086 pyegeria-0.3.6/examples/widgets/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.6/examples/widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.6/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3157 2024-04-29 00:14:47.000000 pyegeria-0.3.6/examples/widgets/coco_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3642 2024-04-18 19:49:26.000000 pyegeria-0.3.6/examples/widgets/collection_viewer.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5234 2024-05-02 12:50:29.000000 pyegeria-0.3.6/examples/widgets/engine_action_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5185 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/find_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4947 2024-04-25 14:18:41.000000 pyegeria-0.3.6/examples/widgets/get_relationship_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     6857 2024-05-01 12:33:39.000000 pyegeria-0.3.6/examples/widgets/get_tech_details.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3938 2024-04-30 15:13:17.000000 pyegeria-0.3.6/examples/widgets/get_tech_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5299 2024-04-24 01:14:00.000000 pyegeria-0.3.6/examples/widgets/get_valid_metadata_values.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/glossary_view.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/gov_engine_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/integration_daemon_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3499 2024-04-29 06:38:46.000000 pyegeria-0.3.6/examples/widgets/list_asset_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3704 2024-04-18 13:42:39.000000 pyegeria-0.3.6/examples/widgets/multi-server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/my_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/open_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5448 2024-04-24 21:32:52.000000 pyegeria-0.3.6/examples/widgets/project_list_viewer.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-12 00:32:44.000000 pyegeria-0.3.6/examples/widgets/server_status_widget.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4619 2024-04-26 14:50:59.000000 pyegeria-0.3.6/examples/widgets/view_my_profile.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-05-03 11:28:48.000000 pyegeria-0.3.6/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-05-03 11:28:52.458528 pyegeria-0.3.6/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2102 2024-04-12 00:32:44.000000 pyegeria-0.3.6/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.445026 pyegeria-0.3.6/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.455299 pyegeria-0.3.6/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1769 2024-04-23 16:53:51.000000 pyegeria-0.3.6/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.6/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.6/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.6/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.6/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   102487 2024-05-02 16:23:06.000000 pyegeria-0.3.6/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   114200 2024-04-29 01:32:02.000000 pyegeria-0.3.6/src/pyegeria/collection_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    93244 2024-05-03 11:21:16.000000 pyegeria-0.3.6/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.6/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42441 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    77305 2024-04-26 16:10:23.000000 pyegeria-0.3.6/src/pyegeria/project_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8775 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-12 00:32:44.000000 pyegeria-0.3.6/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.6/src/pyegeria/utils.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    29710 2024-04-25 15:33:15.000000 pyegeria-0.3.6/src/pyegeria/valid_metadata_omvs.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.457953 pyegeria-0.3.6/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-05-03 11:28:52.000000 pyegeria-0.3.6/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3479 2024-05-03 11:28:52.000000 pyegeria-0.3.6/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-05-03 11:28:52.000000 pyegeria-0.3.6/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-05-03 11:28:52.000000 pyegeria-0.3.6/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-05-03 11:28:52.000000 pyegeria-0.3.6/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 11:28:52.457770 pyegeria-0.3.6/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41409 2024-05-03 11:25:36.000000 pyegeria-0.3.6/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.6/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    51872 2024-04-29 00:11:27.000000 pyegeria-0.3.6/tests/test_collection_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59269 2024-05-02 18:01:47.000000 pyegeria-0.3.6/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.6/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.6/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.6/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9625 2024-04-12 00:32:44.000000 pyegeria-0.3.6/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40084 2024-04-23 14:27:57.000000 pyegeria-0.3.6/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    28529 2024-04-26 16:12:52.000000 pyegeria-0.3.6/tests/test_project_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4712 2024-04-29 06:35:51.000000 pyegeria-0.3.6/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8108 2024-05-02 13:34:44.000000 pyegeria-0.3.6/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.6/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12782 2024-04-25 15:34:36.000000 pyegeria-0.3.6/tests/test_valid_metadata_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.6/tests/test_validators.py
```

### Comparing `pyegeria-0.3.5/LICENSE` & `pyegeria-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/PKG-INFO` & `pyegeria-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.5/README.md` & `pyegeria-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/.DS_Store` & `pyegeria-0.3.6/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/README.md` & `pyegeria-0.3.6/examples/Coco_config/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS1.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDS1.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS2.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDS2.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS3.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDS3.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS4.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDS4.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS5.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDS5.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDS6.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDS6.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoMDSx.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoMDSx.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_cocoView1.py` & `pyegeria-0.3.6/examples/Coco_config/config_cocoView1.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_exchangeDL01.py` & `pyegeria-0.3.6/examples/Coco_config/config_exchangeDL01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_governDL01.py` & `pyegeria-0.3.6/examples/Coco_config/config_governDL01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_monitorDev01.py` & `pyegeria-0.3.6/examples/Coco_config/config_monitorDev01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/config_monitorGov01.py` & `pyegeria-0.3.6/examples/Coco_config/config_monitorGov01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Coco_config/globals.py` & `pyegeria-0.3.6/examples/Coco_config/globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Doc_Samples/Create_Collection_Sample.py` & `pyegeria-0.3.6/examples/Doc_Samples/Create_Collection_Sample.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py` & `pyegeria-0.3.6/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/P-egeria-server-config.ipynb` & `pyegeria-0.3.6/examples/Jupyter Notebooks/P-egeria-server-config.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/common/P-environment-check.ipynb` & `pyegeria-0.3.6/examples/Jupyter Notebooks/common/P-environment-check.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/common/common-functions.ipynb` & `pyegeria-0.3.6/examples/Jupyter Notebooks/common/common-functions.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/common/environment-check.ipynb` & `pyegeria-0.3.6/examples/Jupyter Notebooks/common/environment-check.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/common/globals.ipynb` & `pyegeria-0.3.6/examples/Jupyter Notebooks/common/globals.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/common/globals.py` & `pyegeria-0.3.6/examples/Jupyter Notebooks/common/globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/Jupyter Notebooks/common/orig_globals.py` & `pyegeria-0.3.6/examples/Jupyter Notebooks/common/orig_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/.DS_Store` & `pyegeria-0.3.6/examples/widgets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/README.md` & `pyegeria-0.3.6/examples/widgets/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc` & `pyegeria-0.3.6/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/coco_status.py` & `pyegeria-0.3.6/examples/widgets/coco_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/collection_viewer.py` & `pyegeria-0.3.6/examples/widgets/collection_viewer.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/engine_action_status.py` & `pyegeria-0.3.6/examples/widgets/engine_action_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import argparse
 import json
 import time
 
 from rich import box
 from rich.live import Live
 from rich.table import Table
-from rich import console
+from rich.console import Console
 
 from pyegeria import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
 )
@@ -61,26 +61,26 @@
             show_lines=True,
             box=box.ROUNDED,
             caption=f"Engine Status for Server '{server}' @ Platform - {url}",
             expand=True
         )
         table.add_column("Requested Time")
         table.add_column("Start Time")
-
+        table.add_column("Action GUID", no_wrap=True)
         table.add_column("Engine Name")
         table.add_column("Request Type")
         table.add_column("Action Status")
         table.add_column("Target Element")
         table.add_column("Completion Time")
         table.add_column("Process Name")
         table.add_column("Completion Message")
 
         token = g_client.create_egeria_bearer_token()
         action_status = g_client.get_engine_actions()
-        if action_status is None:
+        if "No Elements" in action_status:
             requested_time = " "
             start_time = " "
             completion_time = " "
             engine_name = " "
             request_type = " "
             action_status = " "
             target_element = " "
@@ -90,15 +90,15 @@
             for action in action_status:
                 requested_time = action["requestedTime"]
                 start_time = action.get("startTime", " ")
                 completion_time = action.get("completionTime", " ")
 
                 engine_name = action["governanceEngineName"]
                 request_type = action["requestType"]
-
+                action_guid = action["elementHeader"]["guid"]
                 if action["actionStatus"] in ("REQUESTED", "APPROVED", "WAITING", "ACTIVATING"):
                     action_status = f"[yellow]{action['actionStatus']}"
                 elif action["actionStatus"] in ("IN_PROGRESS", "ACTIONED"):
                     action_status = f"[green]{action['actionStatus']}"
                 else:
                     action_status = f"[red]{action['actionStatus']}"
 
@@ -108,27 +108,25 @@
                 else:
                     target_element = " "
 
                 process_name = action.get("processName", " ")
                 completion_message = action.get("completionMessage", " ")
 
                 table.add_row(
-                    requested_time, start_time, engine_name, request_type,
+                    requested_time, start_time, action_guid,engine_name, request_type,
                     action_status, target_element, completion_time, process_name, completion_message
                 )
 
         # g_client.close_session()
         return table
 
     try:
-        with Live(generate_table(), refresh_per_second=4, screen=True) as live:
-            while True:
-                time.sleep(2)
-                live.update(generate_table())
-                live.console.pager()
+        console = Console()
+        with console.pager():
+            console.print(generate_table())
 
     except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
         print_exception_response(e)
         assert e.related_http_code != "200", "Invalid parameters"
 
 
 if __name__ == "__main__":
```

### Comparing `pyegeria-0.3.5/examples/widgets/find_todos.py` & `pyegeria-0.3.6/examples/widgets/find_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/get_relationship_types.py` & `pyegeria-0.3.6/examples/widgets/get_relationship_types.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/get_valid_metadata_values.py` & `pyegeria-0.3.6/examples/widgets/get_valid_metadata_values.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/glossary_view.py` & `pyegeria-0.3.6/examples/widgets/glossary_view.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/gov_engine_status.py` & `pyegeria-0.3.6/examples/widgets/gov_engine_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/integration_daemon_status.py` & `pyegeria-0.3.6/examples/widgets/integration_daemon_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/list_asset_types.py` & `pyegeria-0.3.6/examples/widgets/list_asset_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 good_server_3 = "view-server"
 good_server_4 = "engine-host"
 bad_server_1 = "coco"
 bad_server_2 = ""
 
 
 def display_asset_types(server: str = good_server_3, url: str = good_platform1_url, username: str = good_user_2):
-    r_client = RegisteredInfo(good_platform1_url, good_user_2, "secret",
-                              server_name=good_server_3, )
+    r_client = RegisteredInfo(server, url, username)
     token = r_client.create_egeria_bearer_token(good_user_2, "secret")
     asset_types = r_client.list_asset_types()
 
     def generate_table() -> Table:
         """Make a new table."""
         table = Table(
             title=f"Asset Types for: {good_platform1_url} @ {time.asctime()}",
@@ -77,15 +76,15 @@
         if len(asset_types) > 0:
             for a_type in asset_types:
                 name = a_type.get("name", "none")
                 description = a_type.get("description", "none")
                 version = a_type.get("version", " ")
                 super_type = a_type.get("superType", "none")
                 table.add_row(
-                    name, description, str(version), super_type
+                    name, description, super_type, str(version)
                 )
         return table
 
     try:
         console = Console()
         with console.pager():
             console.print(generate_table())
```

### Comparing `pyegeria-0.3.5/examples/widgets/multi-server_status.py` & `pyegeria-0.3.6/examples/widgets/multi-server_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/my_todos.py` & `pyegeria-0.3.6/examples/widgets/my_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/open_todos.py` & `pyegeria-0.3.6/examples/widgets/open_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/project_list_viewer.py` & `pyegeria-0.3.6/examples/widgets/project_list_viewer.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/server_status.py` & `pyegeria-0.3.6/examples/widgets/server_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/server_status_widget.py` & `pyegeria-0.3.6/examples/widgets/server_status_widget.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/examples/widgets/view_my_profile.py` & `pyegeria-0.3.6/examples/widgets/view_my_profile.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/pyproject.toml` & `pyegeria-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #requires = ["hatchling"]
 requires = ["setuptools", "wheel"]
 #build-backend = "hatchling.build"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.3.5"
+version = "0.3.6"
 #license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
 dependencies = [
     "requests~=2.31.0",
     "validators~=0.22.0",
```

### Comparing `pyegeria-0.3.5/setup.py` & `pyegeria-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/__init__.py` & `pyegeria-0.3.6/src/pyegeria/__init__.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/_client.py` & `pyegeria-0.3.6/src/pyegeria/_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/_exceptions.py` & `pyegeria-0.3.6/src/pyegeria/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/_globals.py` & `pyegeria-0.3.6/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/_validators.py` & `pyegeria-0.3.6/src/pyegeria/_validators.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/automated_curation_omvs.py` & `pyegeria-0.3.6/src/pyegeria/automated_curation_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             user_id: str,
             user_pwd: str = None,
             verify_flag: bool = False,
     ):
         Client.__init__(self, server_name, platform_url, user_id, user_pwd, verify_flag)
         self.cur_command_root = f"{platform_url}/servers/"
 
+
     async def _async_create_element_from_template(self, body: dict, server: str = None) -> str:
         """ Create a new metadata element from a template.  Async version.
              Parameters
              ----------
              body : str
                  The json body used to instantiate the template.
              server : str, optional
@@ -592,15 +593,15 @@
         """
         server = self.server_name if server is None else server
         validate_name(name)
 
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/engine-actions/by-name?"
                f"startFrom={start_from}&pageSize={page_size}")
         body = {
-            "string": name
+            "filter": name
         }
         response = await self._async_make_request("POST", url, body)
         return response.json().get("elements", "no actions")
 
     def get_engine_actions_by_name(self, name: str, server: str = None, start_from: int = 0,
                                    page_size: int = max_paging_size) -> list | str:
         """ Retrieve the list of engine action metadata elements with a matching qualified or display name.
@@ -812,15 +813,15 @@
             """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_get_governance_action_process_by_guid(process_guid, server)
         )
         return response
 
-    async def _async_gov_action_process_graph(self, process_guid: str, server: str = None) -> dict | str:
+    async def _async_get_gov_action_process_graph(self, process_guid: str, server: str = None) -> dict | str:
         """ Retrieve the governance action process metadata element with the supplied unique
             identifier along with the flow definition describing its implementation. Async Version.
         Parameters
         ----------
         process_guid : str
             The process GUID to retrieve the graph for.
         server : str, optional
@@ -844,15 +845,15 @@
 
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/"
                f"governance-action-processes/{process_guid}/graph")
 
         response = await self._async_make_request("GET", url)
         return response.json().get("element", "no actions")
 
-    def gov_action_process_graph(self, process_guid: str, server: str = None) -> dict | str:
+    def get_gov_action_process_graph(self, process_guid: str, server: str = None) -> dict | str:
         """ Retrieve the governance action process metadata element with the supplied unique
             identifier along with the flow definition describing its implementation.
            Parameters
            ----------
            process_guid : str
                The process GUID to retrieve the graph for.
            server : str, optional
@@ -911,15 +912,15 @@
 
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-processes/"
                f"by-name?startFrom={start_from}&pageSize={page_size}")
         body = {
             "class": "NameRequestBody",
             "name": name
         }
-        response = await self._async_make_request("GET", url, body)
+        response = await self._async_make_request("POST", url, body)
         return response.json().get("elements", "no actions")
 
     def get_gov_action_processes_by_name(self, name: str, server: str = None, start_from: int = 0,
                                          page_size: int = max_paging_size) -> list | str:
         """ Retrieve the list of governance action process metadata elements with a matching qualified or display name.
             There are no wildcards supported on this request.
 
@@ -1005,15 +1006,15 @@
                f"by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
                f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}"
                )
         body = {
             "class": "SearchStringRequestBody",
             "name": search_string
         }
-        response = await self._async_make_request("GET", url, body)
+        response = await self._async_make_request("POST", url, body)
         return response.json().get("elements", "no actions")
 
     def find_gov_action_processes(self, search_string: str = "*", server: str = None, starts_with: bool = False,
                                   ends_with: bool = False, ignore_case: bool = False, start_from: int = 0,
                                   page_size: int = max_paging_size) -> list | str:
         """ Retrieve the list of governance action process metadata elements that contain the search string.
 
@@ -1106,15 +1107,15 @@
             "originatorServiceName": orig_service_name,
             "originatorEngineName": orig_engine_name
         }
         new_body = body_slimmer(body)
         response = await self._async_make_request("POST", url, new_body)
         return response.json().get("guid", "Action not initiated")
 
-    def initiate_governance_action_process(self, action_type_qualified_name: str, request_source_guids: [str],
+    def initiate_gov_action_process(self, action_type_qualified_name: str, request_source_guids: [str],
                                            action_targets: [str], start_time: datetime, request_parameters: dict,
                                            orig_service_name: str, orig_engine_name: str, server: str = None) -> str:
         """ Using the named governance action process as a template, initiate a chain of engine actions.
 
         Parameters
         ----------
         action_type_qualified_name: str
@@ -1149,15 +1150,15 @@
         response = loop.run_until_complete(
             self._async_initiate_gov_action_process(action_type_qualified_name, request_source_guids,
                                                     action_targets, start_time, request_parameters,
                                                     orig_service_name, orig_engine_name, server)
         )
         return response
 
-    async def _async_get_gov_action_type_by_guid(self, gov_action_type_guid: str, server: str = None) -> dict | str:
+    async def _async_get_gov_action_types_by_guid(self, gov_action_type_guid: str, server: str = None) -> dict | str:
         """ Retrieve the governance action type metadata element with the supplied unique identifier. Async version.
 
         Parameters:
         ----------
             gov_action_type_guid: str
               The GUID (Globally Unique Identifier) of the governance action type to retrieve.
             server: str, optional
@@ -1178,15 +1179,15 @@
 
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/"
                f"governance-action-types/{gov_action_type_guid}")
 
         response = await self._async_make_request("GET", url)
         return response.json().get("element", "no actions")
 
-    def get_gov_action_type_by_guid(self, gov_action_type_guid: str, server: str = None) -> dict | str:
+    def get_gov_action_types_by_guid(self, gov_action_type_guid: str, server: str = None) -> dict | str:
         """ Retrieve the governance action type metadata element with the supplied unique identifier.
 
         Parameters:
         ----------
             gov_action_type_guid: str
               The GUID (Globally Unique Identifier) of the governance action type to retrieve.
             server: str, optional
@@ -1272,15 +1273,15 @@
             self._async_get_gov_action_types_by_name(action_type_name, server,
                                                      start_from, page_size)
         )
         return response
 
     async def _async_find_gov_action_types(self, search_string: str = "*", server: str = None,
                                            starts_with: bool = False,
-                                           ends_with: bool = False, ignore_case: bool = False, start_from: int = 0,
+                                           ends_with: bool = False, ignore_case: bool = True, start_from: int = 0,
                                            page_size: int = max_paging_size) -> list | str:
         """ Retrieve the list of governance action type metadata elements that contain the search string.
             Async Version.
 
            Parameters
            ----------
            search_string : str
@@ -1330,15 +1331,15 @@
                f"by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
                f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}"
                )
         body = {
             "class": "SearchStringRequestBody",
             "name": search_string
         }
-        response = await self._async_make_request("GET", url, body)
+        response = await self._async_make_request("POST", url, body)
         return response.json().get("elements", "no action types")
 
     def find_gov_action_types(self, search_string: str = "*", server: str = None, starts_with: bool = False,
                               ends_with: bool = False, ignore_case: bool = False, start_from: int = 0,
                               page_size: int = max_paging_size) -> list | str:
         """ Retrieve the list of governance action type metadata elements that contain the search string.
 
@@ -1477,14 +1478,38 @@
         response = loop.run_until_complete(
             self._async_initiate_gov_action_type(action_type_qualified_name, request_source_guids,
                                                  action_targets, start_time, request_parameters,
                                                  orig_service_name, orig_engine_name, server)
         )
         return response
 
+    async def _async_initiate_postgres_database_survey(self, postgres_database_guid: str, server: str = None) -> str:
+        server = self.server_name if server is None else server
+        url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
+               f"initiate")
+
+        body = {
+            "class": "InitiateGovernanceActionTypeRequestBody",
+            "governanceActionTypeQualifiedName": "Egeria:GovernanceActionType:2adeb8f1-0f59-4970-b6f2-6cc25d4d2402survey-postgres-database",
+            "actionTargets": [{
+                "class": "NewActionTarget",
+                "actionTargetName": "serverToSurvey",
+                "actionTargetGUID": postgres_database_guid
+            }]
+        }
+        response = await self._async_make_request("POST", url, body)
+        return response.json().get("guid", "Action not initiated")
+
+    def initiate_postgres_database_survey(self, postgres_database_guid: str, server: str = None) -> str:
+        loop = asyncio.get_event_loop()
+        response = loop.run_until_complete(
+            self._async_initiate_postgres_server_survey(postgres_database_guid, server)
+        )
+        return response
+
     async def _async_initiate_postgres_server_survey(self, postgres_server_guid: str, server: str = None) -> str:
         server = self.server_name if server is None else server
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
                f"initiate")
 
         body = {
             "class": "InitiateGovernanceActionTypeRequestBody",
@@ -1504,14 +1529,16 @@
     def initiate_postgres_server_survey(self, postgres_server_guid: str, server: str = None) -> str:
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_initiate_postgres_server_survey(postgres_server_guid, server)
         )
         return response
 
+
+
     async def _async_initiate_file_folder_survey(self, file_folder_guid: str,
                                                  server: str = None) -> str:
         server = self.server_name if server is None else server
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
                f"initiate")
 
         body = {
@@ -1523,21 +1550,47 @@
                 "actionTargetName": "folderToSurvey",
                 "actionTargetGUID": file_folder_guid
             }]
         }
         response = await self._async_make_request("POST", url, body)
         return response.json().get("guid", "Action not initiated")
 
-    def initiate_file_folder_survey(self, file_folder_guid: str, server: str = None) -> str:
+    def initiate_file_folder_survey(self, file_folder_guid:str, server: str = None) -> str:
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
             self._async_initiate_file_folder_survey(file_folder_guid, server)
         )
         return response
 
+    async def _async_initiate_file_survey(self, file_guid: str,
+                                                 server: str = None) -> str:
+        server = self.server_name if server is None else server
+        url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
+               f"initiate")
+
+        body = {
+            "class": "InitiateGovernanceActionTypeRequestBody",
+            "governanceActionTypeQualifiedName":
+                "Egeria:GovernanceActionType:2adeb8f1-0f59-4970-b6f2-6cc25d4d2402survey-folder",
+            "actionTargets": [{
+                "class": "NewActionTarget",
+                "actionTargetName": "fileToSurvey",
+                "actionTargetGUID": file_guid
+            }]
+        }
+        response = await self._async_make_request("POST", url, body)
+        return response.json().get("guid", "Action not initiated")
+
+    def initiate_file_survey(self, file_guid:str, server: str = None) -> str:
+        loop = asyncio.get_event_loop()
+        response = loop.run_until_complete(
+            self._async_initiate_file_survey(file_guid, server)
+        )
+        return response
+
     async def _async_initiate_kafka_server_survey(self, kafka_server_guid: str, server: str = None) -> str:
         server = self.server_name if server is None else server
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/governance-action-types/"
                f"initiate")
 
         body = {
             "class": "InitiateGovernanceActionTypeRequestBody",
@@ -1806,15 +1859,15 @@
         response = loop.run_until_complete(
             self._async_get_catalog_target(integ_connector_guid, metadata_element_guid,
                                            server)
         )
         return response
 
     async def _async_add_catalog_target(self, integ_connector_guid: str, metadata_element_guid: str,
-                                        catalog_target_name: str, metadata_src_qual_name: str, config_properties: dict
+                                        catalog_target_name: str, metadata_src_qual_name: str = None, config_properties: dict = None
                                         , server: str = None) -> None:
         """ Add a catalog target to an integration connector.
             Async version.
 
             Parameters:
             ----------
             integ_connector_guid: str
@@ -1851,15 +1904,15 @@
             "metadataSourceQualifiedName": metadata_src_qual_name,
             "configProperties": config_properties
         }
         await self._async_make_request("POST", url, body)
         return
 
     def add_catalog_target(self, integ_connector_guid: str, metadata_element_guid: str, catalog_target_name: str,
-                           metadata_src_qual_name: str, config_properties: dict, server: str = None) -> None:
+                           metadata_src_qual_name: str = None, config_properties: dict = None, server: str = None) -> None:
         """ Add a catalog target to an integration connector.
 
             Parameters:
             ----------
             integ_connector_guid: str
                 The GUID (Globally Unique Identifier) of the integration connector used to retrieve catalog targets.
             metadata_element_guid: str
@@ -1888,15 +1941,15 @@
             self._async_add_catalog_target(integ_connector_guid, metadata_element_guid,
                                            metadata_src_qual_name, metadata_src_qual_name,
                                            config_properties, server)
         )
         return
 
     async def _async_remove_catalog_target(self, integ_connector_guid: str, metadata_element_guid: str,
-                                           catalog_target_name: str, server: str = None) -> None:
+                                            server: str = None) -> None:
         """ Remove a catalog target to an integration connector. Async version.
 
             Parameters:
             ----------
             integ_connector_guid: str
                 The GUID (Globally Unique Identifier) of the integration connector used to retrieve catalog targets.
             metadata_element_guid: str
@@ -1921,15 +1974,15 @@
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/integration-connectors/"
                f"{integ_connector_guid}/catalog-targets/{metadata_element_guid}/remove")
 
         await self._async_make_request("POST", url)
         return
 
     def remove_catalog_target(self, integ_connector_guid: str, metadata_element_guid: str,
-                              catalog_target_name: str, server: str = None) -> None:
+                               server: str = None) -> None:
         """ Remove a catalog target to an integration connector.
 
             Parameters:
             ----------
             integ_connector_guid: str
                 The GUID (Globally Unique Identifier) of the integration connector used to retrieve catalog targets.
             metadata_element_guid: str
@@ -1989,15 +2042,15 @@
             More information can be found at: https://egeria-project.org/types
         """
         server = self.server_name if server is None else server
         # validate_name(type_name)
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/open-metadata-types/"
                f"{type_name}/technology-types?startFrom={start_from}&pageSize={page_size}")
         body = {
-            "string": tech_name
+            "filter": tech_name
         }
 
         response = await self._async_make_request("GET", url, body)
         return response.json().get("elements", "no tech found")
 
     def get_tech_types_for_open_metadata_type(self, type_name: str, tech_name: str, server: str = None,
                                               start_from: int = 0, page_size: int = max_paging_size) -> list | str:
@@ -2060,15 +2113,15 @@
         -----
         More information can be found at: https://egeria-project.org/concepts/deployed-implementation-type
         """
         server = self.server_name if server is None else server
         validate_name(type_name)
         url = f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/technology-types/by-name"
 
-        body = {"string": type_name}
+        body = {"filter": type_name}
 
         response = await self._async_make_request("POST", url, body)
         return response.json().get("element", "no type found")
 
     def get_technology_type_detail(self, type_name: str, server: str = None) -> list | str:
         """ Retrieve the details of the named technology type. This name should be the name of the technology type
             and contain no wild cards.
@@ -2151,20 +2204,20 @@
         validate_name(search_string)
         if search_string == "*":
             search_string = ""
 
         url = (f"{self.platform_url}/servers/{server}/api/open-metadata/automated-curation/technology-types/"
                f"by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
                f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}")
-        body = {"string": search_string}
+        body = {"filter": search_string}
 
         response = await self._async_make_request("POST", url, body)
         return response.json().get("elements", "no tech found")
 
-    def find_technology_types(self, type_name: str = "*", server: str = None, start_from: int = 0,
+    def find_technology_types(self, search_string: str = "*", server: str = None, start_from: int = 0,
                               page_size: int = max_paging_size, starts_with: bool = False,
                               ends_with: bool = False, ignore_case: bool = True) -> list | str:
         """ Retrieve the list of technology types that contain the search string. Async version.
 
             Parameters:
             ----------
             type_name: str
@@ -2185,15 +2238,15 @@
             Notes
             -----
             For more information see: https://egeria-project.org/concepts/deployed-implementation-type
         """
 
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(
-            self._async_find_technology_types(type_name, server, start_from,
+            self._async_find_technology_types(search_string, server, start_from,
                                               page_size, starts_with, ends_with, ignore_case)
         )
         return response
 
     async def _async_get_all_technology_types(self, server: str = None, start_from: int = 0,
                                               page_size: int = max_paging_size) -> list | str:
         return await self._async_find_technology_types("*", server, start_from, page_size)
```

### Comparing `pyegeria-0.3.5/src/pyegeria/collection_manager_omvs.py` & `pyegeria-0.3.6/src/pyegeria/collection_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.6/src/pyegeria/core_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,16 @@
         if severities is None:
             severities = []
 
         url = (f"{self.admin_command_root}/servers/{server_name}/audit-log-destinations/event-topic?topicName="
                f"{topic_name}")
         self.make_request("POST", url, severities)
 
-    def add_file_log_destinations(self, directory_name: str, severities: [str] = None, server_name: str = None) -> None:
+    def add_file_log_destinations(self, directory_name: str, severities=None,
+                                  server_name: str = None) -> None:
         """ Adds a file log destination to a server. Each message is a separate file in the directory
             indicated by the directory name.
 
         Parameters
         ----------
         directory_name : str
             Path to the audit files.
@@ -781,14 +782,16 @@
         NotAuthorizedException:
             The principle specified by the user_id does not have authorization for the requested action
         ConfigurationErrorException:
             Raised when configuration parameters passed on earlier calls turn out to be
             invalid or make the new call invalid.
 
         """
+        if severities is None:
+            severities = ["Error", "Exception"]
         if server_name is None:
             server_name = self.server_name
 
         validate_name(directory_name)
 
         if severities is None:
             severities = []
```

### Comparing `pyegeria-0.3.5/src/pyegeria/full_omag_server_config.py` & `pyegeria-0.3.6/src/pyegeria/full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.6/src/pyegeria/glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/gov_engine.py` & `pyegeria-0.3.6/src/pyegeria/gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/governance_author.py` & `pyegeria-0.3.6/src/pyegeria/governance_author.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/my_profile_omvs.py` & `pyegeria-0.3.6/src/pyegeria/my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/platform_services.py` & `pyegeria-0.3.6/src/pyegeria/platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/project_manager_omvs.py` & `pyegeria-0.3.6/src/pyegeria/project_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/registered_info.py` & `pyegeria-0.3.6/src/pyegeria/registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/server_operations.py` & `pyegeria-0.3.6/src/pyegeria/server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/utils.py` & `pyegeria-0.3.6/src/pyegeria/utils.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria/valid_metadata_omvs.py` & `pyegeria-0.3.6/src/pyegeria/valid_metadata_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/src/pyegeria.egg-info/PKG-INFO` & `pyegeria-0.3.6/src/pyegeria.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.5/src/pyegeria.egg-info/SOURCES.txt` & `pyegeria-0.3.6/src/pyegeria.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 examples/widgets/README.md
 examples/widgets/__init__.py
 examples/widgets/coco_status.py
 examples/widgets/collection_viewer.py
 examples/widgets/engine_action_status.py
 examples/widgets/find_todos.py
 examples/widgets/get_relationship_types.py
+examples/widgets/get_tech_details.py
+examples/widgets/get_tech_types.py
 examples/widgets/get_valid_metadata_values.py
 examples/widgets/glossary_view.py
 examples/widgets/gov_engine_status.py
 examples/widgets/integration_daemon_status.py
 examples/widgets/list_asset_types.py
 examples/widgets/multi-server_status.py
 examples/widgets/my_todos.py
```

### Comparing `pyegeria-0.3.5/tests/test_client.py` & `pyegeria-0.3.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_collection_manager_omvs.py` & `pyegeria-0.3.6/tests/test_collection_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_core_omag_server_config.py` & `pyegeria-0.3.6/tests/test_core_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
                 InvalidParameterException,
                 PropertyServerException,
                 UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
-    def test_add_file_log_destinations(self, server: str = good_server_1):
+    def test_add_file_log_destinations(self, server: str = good_integ_1):
 
         try:
             o_client: CoreServerConfig = CoreServerConfig(
                 server, self.good_platform1_url,
                 self.good_user_1)
 
             o_client.add_file_log_destinations("./logs", [])
```

### Comparing `pyegeria-0.3.5/tests/test_full_omag_server_config.py` & `pyegeria-0.3.6/tests/test_full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_glossary_omvs.py` & `pyegeria-0.3.6/tests/test_glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_gov_engine.py` & `pyegeria-0.3.6/tests/test_gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_my_profile_omvs.py` & `pyegeria-0.3.6/tests/test_my_profile_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_platform_services.py` & `pyegeria-0.3.6/tests/test_platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_project_manager_omvs.py` & `pyegeria-0.3.6/tests/test_project_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_registered_info.py` & `pyegeria-0.3.6/tests/test_registered_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,16 @@
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
     def test_list_asset_types(self):
         user = self.good_user_2
         try:
-            r_client = RegisteredInfo(self.good_platform1_url, user, "secret",
-                                      server_name =self.good_server_2,)
+            r_client = RegisteredInfo(self.good_server_2,self.good_platform1_url, user,
+                                      "secret")
             token = r_client.create_egeria_bearer_token(user, "secret")
             response = r_client.list_asset_types()
 
             assert type(response) is list, "No services found"
             if type(response) is list:
                 print(f"\n\nAsset types are: \n\n")
                 print(json.dumps(response, indent=4))
```

### Comparing `pyegeria-0.3.5/tests/test_server_operations.py` & `pyegeria-0.3.6/tests/test_server_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,33 +146,34 @@
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
 
 
     def test_get_connector_config(self, server:str = good_server_2):
         try:
             server_name = server
-            connector = "FilesMonitor"
+            connector = "JDBCDatabaseCataloguer"
             s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
             response = s_client.get_connector_config(connector,server)
             print(f"\n\n\tConnector configuration for connector {connector} is \n{json.dumps(response, indent=4)}")
 
             assert True, "Invalid URL or server"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
 
 # todo - review with Mandy?
     def test_restart_integration_connector(self, server:str = good_server_2):
         try:
             server_name = server
-            connector = "FilesMonitor"
+            # connector = "FilesMonitor"
+            connector = "DataFilesMonitorIntegrationConnector"
             s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
             # response = s_client.restart_integration_connector(connector,server)
-            s_client.restart_integration_connector(None, server)
+            s_client.restart_integration_connector(connector, server)
 
             assert True, "Invalid URL or server"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
```

### Comparing `pyegeria-0.3.5/tests/test_util_exp.py` & `pyegeria-0.3.6/tests/test_util_exp.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_valid_metadata_omvs.py` & `pyegeria-0.3.6/tests/test_valid_metadata_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.5/tests/test_validators.py` & `pyegeria-0.3.6/tests/test_validators.py`

 * *Files identical despite different names*

