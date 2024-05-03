# Comparing `tmp/lamindb_setup-0.71.0.tar.gz` & `tmp/lamindb_setup-0.71.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.71.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.71.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.71.0.tar` & `lamindb_setup-0.71.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     8451 2024-04-30 14:26:00.291346 lamindb_setup-0.71.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.71.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.71.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.71.0/.gitignore
--rw-r--r--   0        0        0     1474 2024-04-25 16:11:02.471704 lamindb_setup-0.71.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.71.0/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.71.0/README.md
--rw-r--r--   0        0        0    99141 2024-05-01 17:41:01.022816 lamindb_setup-0.71.0/docs/changelog.md
--rw-r--r--   0        0        0     2574 2024-04-29 07:49:33.469384 lamindb_setup-0.71.0/docs/hub-cloud/01-init-local-instance.ipynb
--rw-r--r--   0        0        0     3948 2024-04-27 13:43:14.991516 lamindb_setup-0.71.0/docs/hub-cloud/02-connect-local-instance.ipynb
--rw-r--r--   0        0        0     9828 2024-04-30 14:26:00.292134 lamindb_setup-0.71.0/docs/hub-cloud/03-add-managed-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-04-25 13:58:37.156407 lamindb_setup-0.71.0/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3112 2024-04-26 09:07:16.588255 lamindb_setup-0.71.0/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3806 2024-04-25 13:58:37.138044 lamindb_setup-0.71.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     5454 2024-04-30 14:26:00.292361 lamindb_setup-0.71.0/docs/hub-cloud/07-keep-artifacts-local.ipynb
--rw-r--r--   0        0        0     3160 2024-04-25 13:58:37.156237 lamindb_setup-0.71.0/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472152 lamindb_setup-0.71.0/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-04-29 07:29:41.597110 lamindb_setup-0.71.0/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-04-25 13:58:37.175784 lamindb_setup-0.71.0/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-04-25 13:58:37.157085 lamindb_setup-0.71.0/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2712 2024-04-27 13:43:14.991856 lamindb_setup-0.71.0/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-04-25 13:58:37.174178 lamindb_setup-0.71.0/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-04-25 13:58:37.139783 lamindb_setup-0.71.0/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-04-25 13:58:37.137631 lamindb_setup-0.71.0/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6182 2024-04-27 13:43:14.992063 lamindb_setup-0.71.0/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472299 lamindb_setup-0.71.0/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.71.0/docs/index.md
--rw-r--r--   0        0        0      513 2024-04-30 14:26:00.292603 lamindb_setup-0.71.0/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.71.0/docs/reference.md
--rw-r--r--   0        0        0     1542 2024-05-01 17:38:56.943344 lamindb_setup-0.71.0/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1325 2024-04-30 14:26:00.293225 lamindb_setup-0.71.0/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      846 2024-04-25 16:11:02.473229 lamindb_setup-0.71.0/lamindb_setup/_cache.py
--rw-r--r--   0        0        0      129 2024-04-25 16:11:02.473531 lamindb_setup-0.71.0/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2613 2024-04-25 16:11:02.473724 lamindb_setup-0.71.0/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1186 2024-04-25 16:11:02.473895 lamindb_setup-0.71.0/lamindb_setup/_close.py
--rw-r--r--   0        0        0    11944 2024-04-30 14:26:00.293578 lamindb_setup-0.71.0/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     7267 2024-05-01 05:19:31.568362 lamindb_setup-0.71.0/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1534 2024-04-25 16:11:02.474852 lamindb_setup-0.71.0/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2120 2024-04-25 16:11:02.475059 lamindb_setup-0.71.0/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1874 2024-04-25 16:11:02.475261 lamindb_setup-0.71.0/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11825 2024-05-01 05:38:35.719751 lamindb_setup-0.71.0/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8815 2024-04-27 13:43:14.993255 lamindb_setup-0.71.0/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      940 2024-04-30 14:26:00.294512 lamindb_setup-0.71.0/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      679 2024-04-25 16:11:02.476265 lamindb_setup-0.71.0/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3670 2024-04-25 16:11:02.476440 lamindb_setup-0.71.0/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1568 2024-04-25 16:11:02.476624 lamindb_setup-0.71.0/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      416 2024-04-30 14:26:00.294783 lamindb_setup-0.71.0/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1799 2024-04-25 16:11:02.477005 lamindb_setup-0.71.0/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2520 2024-04-25 16:11:02.477187 lamindb_setup-0.71.0/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      276 2024-04-25 16:11:02.477423 lamindb_setup-0.71.0/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5504 2024-04-25 16:11:02.477677 lamindb_setup-0.71.0/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    15776 2024-05-01 05:19:31.563200 lamindb_setup-0.71.0/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4662 2024-04-30 14:26:00.295410 lamindb_setup-0.71.0/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1875 2024-04-25 16:11:02.478546 lamindb_setup-0.71.0/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3141 2024-04-30 14:26:00.295688 lamindb_setup-0.71.0/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    16588 2024-04-30 14:26:00.296030 lamindb_setup-0.71.0/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3849 2024-04-27 13:43:14.994618 lamindb_setup-0.71.0/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2637 2024-04-27 13:43:14.994895 lamindb_setup-0.71.0/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    12739 2024-04-30 14:26:00.296388 lamindb_setup-0.71.0/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     2043 2024-04-25 16:11:02.480541 lamindb_setup-0.71.0/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1344 2024-04-25 16:11:02.480798 lamindb_setup-0.71.0/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     3002 2024-04-25 16:11:02.481032 lamindb_setup-0.71.0/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6893 2024-04-27 13:43:14.995437 lamindb_setup-0.71.0/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3450 2024-04-30 14:26:00.296696 lamindb_setup-0.71.0/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      305 2024-04-25 16:11:02.481611 lamindb_setup-0.71.0/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2218 2024-04-27 13:43:14.995719 lamindb_setup-0.71.0/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      532 2024-04-25 16:11:02.482026 lamindb_setup-0.71.0/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    27965 2024-04-30 14:26:00.297107 lamindb_setup-0.71.0/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     3325 2024-04-30 14:26:00.297371 lamindb_setup-0.71.0/noxfile.py
--rw-r--r--   0        0        0     4138 2024-04-30 14:26:00.297636 lamindb_setup-0.71.0/pyproject.toml
--rw-r--r--   0        0        0     5410 2024-04-27 13:43:14.996364 lamindb_setup-0.71.0/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      320 2024-04-25 16:11:02.483189 lamindb_setup-0.71.0/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     5590 2024-04-30 14:26:00.297937 lamindb_setup-0.71.0/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      538 2024-04-25 16:11:02.483601 lamindb_setup-0.71.0/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      504 2024-04-25 16:11:02.483785 lamindb_setup-0.71.0/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      355 2024-04-30 14:26:00.298229 lamindb_setup-0.71.0/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      582 2024-04-25 16:11:02.484159 lamindb_setup-0.71.0/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11218 2024-04-30 14:26:00.298556 lamindb_setup-0.71.0/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      734 2024-04-30 14:26:00.298827 lamindb_setup-0.71.0/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      401 2024-04-25 16:11:02.484790 lamindb_setup-0.71.0/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      193 2024-04-25 16:11:02.484963 lamindb_setup-0.71.0/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1469 2024-04-25 16:11:02.485160 lamindb_setup-0.71.0/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0     1109 2024-04-30 14:26:00.299030 lamindb_setup-0.71.0/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1642 2024-04-27 13:43:14.997388 lamindb_setup-0.71.0/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     2023 2024-04-27 13:43:14.997583 lamindb_setup-0.71.0/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      824 2024-04-25 16:11:02.485962 lamindb_setup-0.71.0/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      878 2024-04-25 16:11:02.486161 lamindb_setup-0.71.0/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1058 2024-04-25 16:11:02.486329 lamindb_setup-0.71.0/tests/storage/test_to_url.py
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.0/PKG-INFO
+-rw-r--r--   0        0        0     8451 2024-04-30 14:26:00.291346 lamindb_setup-0.71.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.71.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.71.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.71.1/.gitignore
+-rw-r--r--   0        0        0     1474 2024-04-25 16:11:02.471704 lamindb_setup-0.71.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.71.1/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.71.1/README.md
+-rw-r--r--   0        0        0    99802 2024-05-03 15:45:25.498159 lamindb_setup-0.71.1/docs/changelog.md
+-rw-r--r--   0        0        0     2574 2024-04-29 07:49:33.469384 lamindb_setup-0.71.1/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3948 2024-04-27 13:43:14.991516 lamindb_setup-0.71.1/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0    10279 2024-05-03 10:05:44.384789 lamindb_setup-0.71.1/docs/hub-cloud/03-add-managed-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-04-25 13:58:37.156407 lamindb_setup-0.71.1/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3191 2024-05-03 13:28:51.894897 lamindb_setup-0.71.1/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3886 2024-05-03 13:28:51.895365 lamindb_setup-0.71.1/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     5454 2024-04-30 14:26:00.292361 lamindb_setup-0.71.1/docs/hub-cloud/07-keep-artifacts-local.ipynb
+-rw-r--r--   0        0        0     3160 2024-04-25 13:58:37.156237 lamindb_setup-0.71.1/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472152 lamindb_setup-0.71.1/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-04-29 07:29:41.597110 lamindb_setup-0.71.1/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-04-25 13:58:37.175784 lamindb_setup-0.71.1/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-04-25 13:58:37.157085 lamindb_setup-0.71.1/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2712 2024-04-27 13:43:14.991856 lamindb_setup-0.71.1/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-04-25 13:58:37.174178 lamindb_setup-0.71.1/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-04-25 13:58:37.139783 lamindb_setup-0.71.1/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-04-25 13:58:37.137631 lamindb_setup-0.71.1/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6182 2024-04-27 13:43:14.992063 lamindb_setup-0.71.1/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      177 2024-04-25 16:11:02.472299 lamindb_setup-0.71.1/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.71.1/docs/index.md
+-rw-r--r--   0        0        0      513 2024-04-30 14:26:00.292603 lamindb_setup-0.71.1/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.71.1/docs/reference.md
+-rw-r--r--   0        0        0     1542 2024-05-03 15:45:16.228444 lamindb_setup-0.71.1/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-25 16:11:02.473229 lamindb_setup-0.71.1/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0      129 2024-04-25 16:11:02.473531 lamindb_setup-0.71.1/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2613 2024-04-25 16:11:02.473724 lamindb_setup-0.71.1/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1186 2024-04-25 16:11:02.473895 lamindb_setup-0.71.1/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    12616 2024-05-03 15:45:08.370116 lamindb_setup-0.71.1/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     7232 2024-05-03 15:45:13.866583 lamindb_setup-0.71.1/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1534 2024-04-25 16:11:02.474852 lamindb_setup-0.71.1/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2120 2024-04-25 16:11:02.475059 lamindb_setup-0.71.1/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1874 2024-04-25 16:11:02.475261 lamindb_setup-0.71.1/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11921 2024-05-03 10:05:44.386303 lamindb_setup-0.71.1/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8815 2024-04-27 13:43:14.993255 lamindb_setup-0.71.1/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      940 2024-04-30 14:26:00.294512 lamindb_setup-0.71.1/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      679 2024-04-25 16:11:02.476265 lamindb_setup-0.71.1/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1268 2024-05-03 10:05:44.386575 lamindb_setup-0.71.1/lamindb_setup/_set_managed_storage.py
+-rw-r--r--   0        0        0     3670 2024-04-25 16:11:02.476440 lamindb_setup-0.71.1/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1568 2024-04-25 16:11:02.476624 lamindb_setup-0.71.1/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      416 2024-04-30 14:26:00.294783 lamindb_setup-0.71.1/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-25 16:11:02.477005 lamindb_setup-0.71.1/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2520 2024-04-25 16:11:02.477187 lamindb_setup-0.71.1/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      276 2024-04-25 16:11:02.477423 lamindb_setup-0.71.1/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5504 2024-04-25 16:11:02.477677 lamindb_setup-0.71.1/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    15970 2024-05-03 10:05:44.386959 lamindb_setup-0.71.1/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4859 2024-05-03 10:05:44.387393 lamindb_setup-0.71.1/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1875 2024-04-25 16:11:02.478546 lamindb_setup-0.71.1/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3141 2024-04-30 14:26:00.295688 lamindb_setup-0.71.1/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    16588 2024-04-30 14:26:00.296030 lamindb_setup-0.71.1/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3922 2024-05-03 10:05:44.387683 lamindb_setup-0.71.1/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2704 2024-05-03 10:05:44.387946 lamindb_setup-0.71.1/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    12382 2024-05-03 10:05:44.388316 lamindb_setup-0.71.1/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     2084 2024-05-03 10:05:44.388614 lamindb_setup-0.71.1/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1344 2024-04-25 16:11:02.480798 lamindb_setup-0.71.1/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     3002 2024-04-25 16:11:02.481032 lamindb_setup-0.71.1/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6893 2024-04-27 13:43:14.995437 lamindb_setup-0.71.1/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3450 2024-04-30 14:26:00.296696 lamindb_setup-0.71.1/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      305 2024-04-25 16:11:02.481611 lamindb_setup-0.71.1/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2218 2024-04-27 13:43:14.995719 lamindb_setup-0.71.1/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      532 2024-04-25 16:11:02.482026 lamindb_setup-0.71.1/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    28286 2024-05-03 15:45:13.867035 lamindb_setup-0.71.1/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     3325 2024-04-30 14:26:00.297371 lamindb_setup-0.71.1/noxfile.py
+-rw-r--r--   0        0        0     4138 2024-04-30 14:26:00.297636 lamindb_setup-0.71.1/pyproject.toml
+-rw-r--r--   0        0        0     5410 2024-04-27 13:43:14.996364 lamindb_setup-0.71.1/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      270 2024-05-03 10:05:44.388882 lamindb_setup-0.71.1/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     5716 2024-05-03 10:05:44.389145 lamindb_setup-0.71.1/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      538 2024-04-25 16:11:02.483601 lamindb_setup-0.71.1/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      504 2024-04-25 16:11:02.483785 lamindb_setup-0.71.1/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      482 2024-05-03 10:05:44.389367 lamindb_setup-0.71.1/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      582 2024-04-25 16:11:02.484159 lamindb_setup-0.71.1/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11218 2024-04-30 14:26:00.298556 lamindb_setup-0.71.1/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      734 2024-04-30 14:26:00.298827 lamindb_setup-0.71.1/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      401 2024-04-25 16:11:02.484790 lamindb_setup-0.71.1/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      193 2024-04-25 16:11:02.484963 lamindb_setup-0.71.1/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1469 2024-04-25 16:11:02.485160 lamindb_setup-0.71.1/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0     1109 2024-04-30 14:26:00.299030 lamindb_setup-0.71.1/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1642 2024-04-27 13:43:14.997388 lamindb_setup-0.71.1/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     2023 2024-04-27 13:43:14.997583 lamindb_setup-0.71.1/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      891 2024-05-03 15:45:13.867354 lamindb_setup-0.71.1/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      878 2024-04-25 16:11:02.486161 lamindb_setup-0.71.1/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1058 2024-04-25 16:11:02.486329 lamindb_setup-0.71.1/tests/storage/test_to_url.py
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 lamindb_setup-0.71.1/PKG-INFO
```

### Comparing `lamindb_setup-0.71.0/.github/workflows/build.yml` & `lamindb_setup-0.71.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/.github/workflows/latest-changes.yml` & `lamindb_setup-0.71.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/.gitignore` & `lamindb_setup-0.71.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/.pre-commit-config.yaml` & `lamindb_setup-0.71.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/LICENSE` & `lamindb_setup-0.71.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/changelog.md` & `lamindb_setup-0.71.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Extend valid suffixes to composite suffixes | [746](https://github.com/laminlabs/lamindb-setup/pull/746) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 | 0.71.1
+🐛 Fix test failures | [745](https://github.com/laminlabs/lamindb-setup/pull/745) | [Koncopd](https://github.com/Koncopd) | 2024-05-03 |
+♻️ Persist keep-artifacts-local in settings.env | [743](https://github.com/laminlabs/lamindb-setup/pull/743) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 |
+✅ Expand tests to multi users for managed storage | [742](https://github.com/laminlabs/lamindb-setup/pull/742) | [falexwolf](https://github.com/falexwolf) | 2024-05-03 |
 🐛 Fix delete function | [741](https://github.com/laminlabs/lamindb-setup/pull/741) | [falexwolf](https://github.com/falexwolf) | 2024-04-30 | 0.71.0
 ✨ Manage multiple storage locations with integrity | [738](https://github.com/laminlabs/lamindb-setup/pull/738) | [falexwolf](https://github.com/falexwolf) | 2024-04-30 |
 ✨ Proper progress bars for upload and download | [739](https://github.com/laminlabs/lamindb-setup/pull/739) | [Koncopd](https://github.com/Koncopd) | 2024-04-28 |
 ♻️ Truncate fsspec deps | [740](https://github.com/laminlabs/lamindb-setup/pull/740) | [Koncopd](https://github.com/Koncopd) | 2024-04-28 |
 ♻️ Refactor storage management | [734](https://github.com/laminlabs/lamindb-setup/pull/734) | [falexwolf](https://github.com/falexwolf) | 2024-04-27 |
 ⬆️ Upper and lower bounds for fsspec | [736](https://github.com/laminlabs/lamindb-setup/pull/736) | [Koncopd](https://github.com/Koncopd) | 2024-04-27 |
 ♻️ Capitalize HOSTED | [733](https://github.com/laminlabs/lamindb-setup/pull/733) | [falexwolf](https://github.com/falexwolf) | 2024-04-26 |
```

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/01-init-local-instance.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/01-init-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/02-connect-local-instance.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/03-add-managed-storage.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/03-add-managed-storage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893482574189096%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'from lamindb_setup._set_managed_storage import "*

 * *            "set_managed_storage')], delete: [4]}}, 6: {'source': {insert: [(1, '    "*

 * *            'set_managed_storage("./storage2")\\n\')], delete: [1]}}, 9: {\'source\': '*

 * *            '[\'set_managed_storage("./storage2")\']}, 12: {\'source\': '*

 * *            '[\'set_managed_storage("./storage1")\']}, 15: {\'source\': '*

 * *            '[\'set_managed_storage("./storage1")\']}, 17: {\'source\': '*

 * *            '[\'set_man […]*

```diff
@@ -34,15 +34,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import laminci\n",
                 "import pytest\n",
                 "from pathlib import Path\n",
                 "import lamindb_setup as ln_setup\n",
-                "from lamindb_setup._add_remote_storage import add_managed_storage"
+                "from lamindb_setup._set_managed_storage import set_managed_storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8fd59ad3-04b9-42fb-83cc-ab7beedbec72",
             "metadata": {
@@ -80,15 +80,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "49b9ef11",
             "metadata": {},
             "outputs": [],
             "source": [
                 "with pytest.raises(ValueError) as error:\n",
-                "    add_managed_storage(\"./storage2\")\n",
+                "    set_managed_storage(\"./storage2\")\n",
                 "assert error.exconly() == \"ValueError: Can't add additional managed storage locations for instances that aren't managed through the hub.\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "077da8fe",
@@ -109,15 +109,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e60b272e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "add_managed_storage(\"./storage2\")"
+                "set_managed_storage(\"./storage2\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8e481aa0",
             "metadata": {
@@ -144,15 +144,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4e5cd7b2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "add_managed_storage(\"./storage1\")"
+                "set_managed_storage(\"./storage1\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "53471a8b",
             "metadata": {},
@@ -175,15 +175,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a4183af7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "add_managed_storage(\"./storage1\")"
+                "set_managed_storage(\"./storage1\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "20564200",
             "metadata": {},
@@ -198,15 +198,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d97ea220",
             "metadata": {},
             "outputs": [],
             "source": [
-                "add_managed_storage(\"./storage2\")"
+                "set_managed_storage(\"./storage2\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e20bfc21",
             "metadata": {},
@@ -230,15 +230,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "add_managed_storage(\"s3://lamindb-ci/storage3\")"
+                "set_managed_storage(\"s3://lamindb-ci/storage3\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d2934990",
             "metadata": {
@@ -269,15 +269,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f9294082",
             "metadata": {},
             "outputs": [],
             "source": [
-                "add_managed_storage(\"s3://lamindb-ci/storage3\", cache_regions=False)"
+                "set_managed_storage(\"s3://lamindb-ci/storage3\", cache_regions=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a889ba33",
             "metadata": {},
@@ -298,54 +298,73 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9a4029b0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# from laminhub_rest.core.collaborator._add_collaborator import add_collaborator\n",
-                "# from lamindb_setup.core._hub_client import connect_hub_with_auth\n",
+                "from laminhub_rest.core.collaborator._add_collaborator import add_collaborator\n",
+                "from lamindb_setup.core._hub_client import connect_hub_with_auth\n",
                 "\n",
-                "# admin_hub = connect_hub_with_auth()\n",
-                "# add_collaborator(\n",
-                "#     \"testuser2\",\n",
-                "#     \"testuser1\",\n",
-                "#     \"test-add-managed-storage\",\n",
-                "#     \"write\",\n",
-                "#     admin_hub,\n",
-                "# )\n",
-                "# admin_hub.auth.close()"
+                "admin_hub = connect_hub_with_auth()\n",
+                "add_collaborator(\n",
+                "    \"testuser2\",\n",
+                "    \"testuser1\",\n",
+                "    \"test-add-managed-storage\",\n",
+                "    \"write\",\n",
+                "    admin_hub,\n",
+                ")\n",
+                "admin_hub.auth.close()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e9d64cad",
             "metadata": {},
             "source": [
-                "Another user:"
+                "Sign them in and let them add another storage location:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d6915638-db49-4d3d-bd91-819bb4719ef7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# ln_setup.login(\"testuser2\")\n",
-                "# add_managed_storage(\"./storage4\")\n",
-                "# assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage4\""
+                "ln_setup.login(\"testuser2\")\n",
+                "set_managed_storage(\"./storage4\")\n",
+                "assert ln_setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage4\""
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "60ac7cb2",
+            "metadata": {},
+            "source": [
+                "Attempt to delete instance with testuser2:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6de90900",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "with pytest.raises(PermissionError) as error:\n",
+                "    ln_setup.delete(\"testuser1/test-add-managed-storage\", force=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9d1fd197",
             "metadata": {},
             "source": [
-                "Delete test instance:"
+                "Delete test instance through testuser1:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c6950299",
             "metadata": {},
```

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970734126984127%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(4, 'assert ln_setup.settings.storage.id is not None\\n'), "*

 * *            "(5, '\\n'), (6, 'assert ln_setup.settings.storage._mark_storage_root.exists()')], "*

 * *            'delete: [4]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.17'}}"}*

```diff
@@ -90,15 +90,17 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert ln_setup.settings.instance.storage.type_is_cloud == True\n",
                 "assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle\n",
                 "assert ln_setup.settings.instance.name == \"my-hosted\"\n",
                 "assert ln_setup.settings.storage.root.as_posix().startswith(HOSTED_BUCKETS)\n",
-                "assert ln_setup.settings.storage.id is not None"
+                "assert ln_setup.settings.storage.id is not None\n",
+                "\n",
+                "assert ln_setup.settings.storage._mark_storage_root.exists()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -119,13 +121,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998397435897436%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(7, '\\n'), (8, 'assert "*

 * *            "ln_setup.settings.storage._mark_storage_root.exists()\\n')]}}}"}*

```diff
@@ -141,14 +141,16 @@
                 "\n",
                 "target_path.unlink()\n",
                 "assert not target_path.exists()\n",
                 "\n",
                 "target_dir.rmdir()\n",
                 "assert not target_dir.exists()\n",
                 "\n",
+                "assert ln_setup.settings.storage._mark_storage_root.exists()\n",
+                "\n",
                 "ln_setup.delete(\"my-hosted\", force=True)\n",
                 "delete_instance(f\"testuser1/{instance_name}\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/07-keep-artifacts-local.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/07-keep-artifacts-local.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.71.1/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.71.1/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/docs/notebooks.md` & `lamindb_setup-0.71.1/docs/notebooks.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/__init__.py` & `lamindb_setup-0.71.1/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.71.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.71.1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._check_setup import _check_instance_setup
 from ._close import close
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.71.1/lamindb_setup/_set_managed_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 from .core._settings import settings
 from .core._settings_storage import init_storage
 
 if TYPE_CHECKING:
     from lamindb_setup.core.types import UPathStr
 
 
-def add_managed_storage(root: UPathStr, **fs_kwargs):
-    """Add a remote default storage location to a local instance.
-
-    This can be used to selectively share data.
+def set_managed_storage(root: UPathStr, **fs_kwargs):
+    """Add or switch to another managed storage location.
 
     Args:
         root: `UPathStr` - The new storage root, e.g., an S3 bucket.
         **fs_kwargs: Additional fsspec arguments for cloud root, e.g., profile.
 
     """
     if settings.instance.dialect == "sqlite":
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_cache.py` & `lamindb_setup-0.71.1/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_check_setup.py` & `lamindb_setup-0.71.1/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_close.py` & `lamindb_setup-0.71.1/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.71.1/lamindb_setup/_connect_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING
 from uuid import UUID
 
+from django.db import ProgrammingError
 from lamin_utils import logger
 
 from ._check_setup import _check_instance_setup
 from ._close import close as close_instance
 from ._init_instance import MESSAGE_NO_MULTIPLE_INSTANCE, load_from_isettings
 from ._migrate import check_whether_migrations_in_sync
 from ._silence_loggers import silence_loggers
@@ -154,14 +155,16 @@
                 db_updated = update_db_using_local(
                     instance_result, settings_file, db=db
                 )
                 ssettings = StorageSettings(
                     root=storage_result["root"],
                     region=storage_result["region"],
                     uid=storage_result["lnid"],
+                    uuid=UUID(storage_result["id"]),
+                    instance_id=UUID(instance_result["id"]),
                 )
                 isettings = InstanceSettings(
                     id=UUID(instance_result["id"]),
                     owner=owner,
                     name=name,
                     storage=ssettings,
                     db=db_updated,
@@ -216,14 +219,25 @@
                 return "instance-corrupted-or-deleted", instance_result
         # this is for testing purposes only
         if _TEST_FAILED_LOAD:
             raise RuntimeError("Technical testing error.")
 
         if storage is not None and isettings.dialect == "sqlite":
             update_root_field_in_default_storage(isettings)
+        # below is for backfilling the instance_uid value
+        # we'll enable it once more people migrated to 0.71.0
+        # ssettings_record = isettings.storage.record
+        # if ssettings_record.instance_uid is None:
+        #     ssettings_record.instance_uid = isettings.uid
+        #     # try saving if not read-only access
+        #     try:
+        #         ssettings_record.save()
+        #     # raised by django when the access is denied
+        #     except ProgrammingError:
+        #         pass
         load_from_isettings(isettings)
     except Exception as e:
         if isettings is not None:
             isettings._get_settings_file().unlink(missing_ok=True)  # type: ignore
         raise e
     return None
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_delete.py` & `lamindb_setup-0.71.1/lamindb_setup/_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import shutil
 from typing import TYPE_CHECKING, Optional
 from uuid import UUID
 
 from lamin_utils import logger
 
-from ._connect_instance import INSTANCE_NOT_FOUND_MESSAGE
+from ._connect_instance import (
+    INSTANCE_NOT_FOUND_MESSAGE,
+    InstanceNotFoundError,
+    get_owner_name_from_identifier,
+)
 from .core._hub_core import connect_instance as load_instance_from_hub
 from .core._hub_core import delete_instance as delete_instance_on_hub
 from .core._hub_core import get_storage_records_for_instance
 from .core._settings import settings
 from .core._settings_instance import InstanceSettings
 from .core._settings_load import load_instance_settings
 from .core._settings_storage import StorageSettings
@@ -50,78 +54,71 @@
     # unset the global instance settings
     if settings._instance_exists and isettings.slug == settings.instance.slug:
         if settings._instance_settings_path.exists():
             settings._instance_settings_path.unlink()
         settings._instance_settings = None
 
 
-def delete(
-    instance_name: str, force: bool = False, require_empty: bool = True
-) -> int | None:
+def delete(slug: str, force: bool = False, require_empty: bool = True) -> int | None:
     """Delete a LaminDB instance.
 
     Args:
-        instance_name (str): The name of the instance to delete.
-        force (bool): Whether to skip the confirmation prompt.
-        require_empty (bool): Whether to check if the instance is empty before deleting.
+        slug: The instance slug `account_handle/instance_name` or URL.
+            If the instance is owned by you, it suffices to pass the instance name.
+        force: Whether to skip the confirmation prompt.
+        require_empty: Whether to check if the instance is empty before deleting.
     """
-    if "/" in instance_name:
-        logger.warning(
-            "Deleting the instance of another user is currently not supported with the"
-            " CLI. Please provide only the instance name when deleting an instance ('/'"
-            " delimiter not allowed)."
-        )
-        raise ValueError("Invalid instance name: '/' delimiter not allowed.")
-    instance_slug = f"{settings.user.handle}/{instance_name}"
+    instance_owner, instance_name = get_owner_name_from_identifier(slug)
     if settings._instance_exists and settings.instance.name == instance_name:
         isettings = settings.instance
     else:
-        settings_file = instance_settings_file(instance_name, settings.user.handle)
+        settings_file = instance_settings_file(instance_name, instance_owner)
         if not settings_file.exists():
             hub_result = load_instance_from_hub(
-                owner=settings.user.handle, name=instance_name
+                owner=instance_owner, name=instance_name
             )
             if isinstance(hub_result, str):
                 message = INSTANCE_NOT_FOUND_MESSAGE.format(
-                    owner=settings.user.handle,
+                    owner=instance_owner,
                     name=instance_name,
                     hub_result=hub_result,
                 )
-                logger.warning(message)
-                return None
+                raise InstanceNotFoundError(message)
             instance_result, storage_result = hub_result
             ssettings = StorageSettings(
                 root=storage_result["root"],
                 region=storage_result["region"],
                 uid=storage_result["lnid"],
+                uuid=UUID(storage_result["id"]),
             )
             isettings = InstanceSettings(
                 id=UUID(instance_result["id"]),
-                owner=settings.user.handle,
+                owner=instance_owner,
                 name=instance_name,
                 storage=ssettings,
                 keep_artifacts_local=bool(instance_result["keep_artifacts_local"]),
                 db=instance_result["db"] if "db" in instance_result else None,
                 schema=instance_result["schema_str"],
                 git_repo=instance_result["git_repo"],
+                is_on_hub=True,
             )
         else:
             isettings = load_instance_settings(settings_file)
     if isettings.dialect != "sqlite":
         logger.warning(
             f"delete() does not yet affect your Postgres database at {isettings.db}"
         )
     if isettings.is_on_hub and settings.user.handle == "anonymous":
         logger.warning(
             "won't delete the hub component of this instance because you're not logged in"
         )
     if not force:
         valid_responses = ["y", "yes"]
         user_input = (
-            input(f"Are you sure you want to delete instance {instance_slug}? (y/n) ")
+            input(f"Are you sure you want to delete instance {isettings.slug}? (y/n) ")
             .strip()
             .lower()
         )
         if user_input not in valid_responses:
             return -1
 
     # the actual deletion process begins here
@@ -157,18 +154,20 @@
                 raise_error=require_empty,
             )
             ssettings = StorageSettings(storage_record["root"])  # type: ignore
             if ssettings._mark_storage_root.exists():
                 ssettings._mark_storage_root.unlink(
                     missing_ok=True  # this is totally weird, but needed on Py3.11
                 )
-    logger.info(f"deleting instance {instance_slug}")
+    logger.info(f"deleting instance {isettings.slug}")
     # below we can skip check_storage_is_empty() because we already called
     # it above
-    if settings.user.handle != "anonymous":
+    if settings.user.handle != "anonymous" and isettings.is_on_hub:
+        # start with deleting things on the hub
+        # this will error if the user doesn't have permission
         delete_instance_on_hub(isettings._id, require_empty=False)
     delete_by_isettings(isettings)
     # if .lndb file was delete, then we might count -1
     if n_objects <= 0 and isettings.storage.type == "local":
         # dir is only empty after sqlite file was delete via delete_by_isettings
         if (isettings.storage.root / ".lamindb").exists():
             (isettings.storage.root / ".lamindb").rmdir()
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_django.py` & `lamindb_setup-0.71.1/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_exportdb.py` & `lamindb_setup-0.71.1/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_importdb.py` & `lamindb_setup-0.71.1/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_init_instance.py` & `lamindb_setup-0.71.1/lamindb_setup/_init_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,18 +273,22 @@
         settings.auto_connect = True
     except Exception as e:
         from ._delete import delete_by_isettings
         from .core._hub_core import delete_instance_record, delete_storage_record
 
         if isettings is not None:
             delete_by_isettings(isettings)
-            if settings.user.handle != "anonymous":
+            if settings.user.handle != "anonymous" and isettings.is_on_hub:
                 delete_instance_record(isettings._id)
             isettings._get_settings_file().unlink(missing_ok=True)  # type: ignore
-        if ssettings is not None and settings.user.handle != "anonymous":
+        if (
+            ssettings is not None
+            and settings.user.handle != "anonymous"
+            and ssettings.is_on_hub
+        ):
             delete_storage_record(ssettings._uuid)  # type: ignore
         raise e
     return None
 
 
 def load_from_isettings(
     isettings: InstanceSettings,
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_migrate.py` & `lamindb_setup-0.71.1/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_register_instance.py` & `lamindb_setup-0.71.1/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_schema.py` & `lamindb_setup-0.71.1/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_setup_user.py` & `lamindb_setup-0.71.1/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.71.1/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_hub_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 
 def _delete_storage_record(storage_uuid: UUID, client: Client) -> None:
     if storage_uuid is None:
         return None
     response = client.table("storage").delete().eq("id", storage_uuid.hex).execute()
     if response.data:
         logger.important(f"deleted storage record on hub {storage_uuid.hex}")
+    else:
+        raise PermissionError(
+            f"Deleting of storage with {storage_uuid.hex} was not successful. Probably, you"
+            " don't have sufficient permissions."
+        )
 
 
 def update_instance_record(instance_uuid: UUID, fields: dict) -> None:
     return call_with_fallback_auth(
         _update_instance_record, instance_id=instance_uuid.hex, instance_fields=fields
     )
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_hub_crud.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 def update_instance(instance_id: str, instance_fields: dict, client: Client):
     response = (
         client.table("instance").update(instance_fields).eq("id", instance_id).execute()
     )
     if len(response.data) == 0:
-        raise RuntimeError(
+        raise PermissionError(
             f"Update of instance with {instance_id} was not successful. Probably, you"
             " don't have sufficient permissions."
         )
     return response.data[0]
 
 
 # --------------- COLLABORATOR ----------------------
@@ -183,7 +183,12 @@
 
 def _delete_instance_record(instance_id: UUID, client: Client) -> None:
     if not isinstance(instance_id, UUID):
         instance_id = UUID(instance_id)
     response = client.table("instance").delete().eq("id", instance_id.hex).execute()
     if response.data:
         logger.important(f"deleted instance record on hub {instance_id.hex}")
+    else:
+        raise PermissionError(
+            f"Deleting of instance with {instance_id.hex} was not successful. Probably, you"
+            " don't have sufficient permissions."
+        )
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         id=UUID(store.id),
         owner=store.owner,
         name=store.name,
         storage=ssettings,
         db=store.db if store.db != "null" else None,  # type: ignore
         schema=store.schema_str if store.schema_str != "null" else None,
         git_repo=store.git_repo if store.git_repo != "null" else None,
+        keep_artifacts_local=store.keep_artifacts_local,  # type: ignore
     )
 
 
 def setup_user_from_store(store: UserSettingsStore) -> UserSettings:
     settings = UserSettings()
     settings.email = store.email
     settings.password = store.password if store.password != "null" else None
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings_save.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     type_hints: dict[str, Any],
     prefix: str,
 ):
     with open(settings_file, "w") as f:
         for store_key, type in type_hints.items():
             if type == Optional[str]:
                 type = str
+            if type == Optional[bool]:
+                type = bool
             if "__" not in store_key:
                 if store_key == "storage_root":
                     value = settings.storage.root_as_str
                 elif store_key == "storage_region":
                     value = settings.storage.region
                 else:
                     if store_key in {"db", "schema_str", "name_", "uuid", "id"}:
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,14 @@
             self._cache_dir = None
         # save access_token here for use in self.root
         self.access_token = access_token
 
         # local storage
         self._has_local = False
         self._local = None
-        self._is_on_hub: bool | None = None
 
     @property
     def id(self) -> int:
         """Storage id in current instance."""
         return self.record.id
 
     @property
@@ -316,24 +315,18 @@
 
     @property
     def is_on_hub(self) -> bool:
         """Is this instance on the hub.
 
         Only works if user has access to the instance.
         """
-        if self._is_on_hub is None:
-            from ._hub_client import call_with_fallback_auth
-            from ._hub_crud import select_storage
-
-            response = call_with_fallback_auth(select_storage, id=self._uuid.hex)  # type: ignore
-            if response is None:
-                self._is_on_hub = False
-            else:
-                self._is_on_hub = True
-        return self._is_on_hub
+        if self._uuid is None:
+            return False
+        else:
+            return True
 
     def key_to_filepath(self, filekey: Path | UPath | str) -> UPath:
         """Cloud or local filepath from filekey."""
         return self.root / filekey
 
     def cloud_to_local(self, filepath: Path | UPath, **kwargs) -> UPath:
         """Local (cache) filepath from filepath."""
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     name: str
     storage_root: str
     storage_region: Optional[str]  # take old type annotations here because pydantic
     db: Optional[str]  # doesn't like new types on 3.9 even with future annotations
     schema_str: Optional[str]
     id: str
     git_repo: Optional[str]
+    keep_artifacts_local: Optional[bool]
 
     class Config:
         env_prefix = "lamindb_instance_"
         env_file = ".env"
 
 
 class UserSettingsStore(BaseSettings):
```

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.71.1/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.71.1/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/django.py` & `lamindb_setup-0.71.1/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/hashing.py` & `lamindb_setup-0.71.1/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/types.py` & `lamindb_setup-0.71.1/lamindb_setup/core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/lamindb_setup/core/upath.py` & `lamindb_setup-0.71.1/lamindb_setup/core/upath.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,18 @@
     ".parquet",
     ".csv",
     ".fcs",
     ".xslx",
     ".zarr",
     ".json",
 }
-
+VALID_COMPOSITE_SUFFIXES = {
+    ".anndata.zarr",
+    ".spatialdata.zarr",
+}
 
 TRAILING_SEP = (os.sep, os.altsep) if os.altsep is not None else os.sep
 
 
 def extract_suffix_from_path(path: Path, arg_name: str | None = None) -> str:
     def process_digits(suffix: str):
         if suffix[1:].isdigit():  # :1 to skip the dot
@@ -70,14 +73,20 @@
 
     if len(path.suffixes) <= 1:
         return process_digits(path.suffix)
 
     total_suffix = "".join(path.suffixes)
     if total_suffix in VALID_SUFFIXES:
         return total_suffix
+    elif total_suffix.endswith(tuple(VALID_COMPOSITE_SUFFIXES)):
+        # below seems slow but OK for now
+        for suffix in VALID_COMPOSITE_SUFFIXES:
+            if total_suffix.endswith(suffix):
+                break
+        return suffix
     else:
         print_hint = True
         arg_name = "file" if arg_name is None else arg_name  # for the warning
         msg = f"{arg_name} has more than one suffix (path.suffixes), "
         # first check the 2nd-to-last suffix because it might be followed by .gz
         # or another compression-related suffix
         # Alex thought about adding logic along the lines of path.suffixes[-1]
```

### Comparing `lamindb_setup-0.71.0/noxfile.py` & `lamindb_setup-0.71.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/pyproject.toml` & `lamindb_setup-0.71.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.71.1/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.71.1/tests/hub-cloud/test_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from uuid import UUID
 
 import lamindb_setup as ln_setup
 import pytest
+from lamindb_setup._connect_instance import InstanceNotFoundError
 from lamindb_setup.core._hub_client import connect_hub_with_auth
 from lamindb_setup.core._hub_core import _connect_instance
 from lamindb_setup.core._hub_crud import (
     Client,
     select_account_by_handle,
     select_instance_by_name,
 )
@@ -23,15 +24,18 @@
     yield hub
     hub.auth.sign_out()
 
 
 def test_init_instance_postgres_default_name(get_hub_client):
     hub = get_hub_client
     instance_name = "pgtest"
-    ln_setup.delete(instance_name, force=True)
+    try:
+        ln_setup.delete(instance_name, force=True)
+    except InstanceNotFoundError:
+        pass
     # now, run init
     ln_setup.init(storage="./mydatapg", db=pgurl, _test=True)
     assert ln_setup.settings.instance.slug == "testuser2/pgtest"
     ln_setup.register(_test=True)
     assert ln_setup.settings.instance.slug == "testuser2/pgtest"
     # and check
     instance, storage = _connect_instance(
```

### Comparing `lamindb_setup-0.71.0/tests/hub-cloud/test_login.py` & `lamindb_setup-0.71.1/tests/hub-cloud/test_login.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-local/conftest.py` & `lamindb_setup-0.71.1/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-local/test_all.py` & `lamindb_setup-0.71.1/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-prod/conftest.py` & `lamindb_setup-0.71.1/tests/hub-prod/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.71.1/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/hub-prod/test_upath.py` & `lamindb_setup-0.71.1/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/storage/test_hashing.py` & `lamindb_setup-0.71.1/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/storage/test_storage_access.py` & `lamindb_setup-0.71.1/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/storage/test_storage_basis.py` & `lamindb_setup-0.71.1/tests/storage/test_storage_basis.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,11 +15,12 @@
         ("directory/file", ""),
         ("d.x.y.z/f.b.c", ".c"),
         ("d.x.y.z/f.a.b.c", ".c"),
         ("logs/date.log.txt", ".txt"),
         ("logs/date.log.123", ""),  # digits are no valid suffixes
         ("salmon.merged.gene_counts.tsv", ".tsv"),
         ("salmon.merged.gene_counts.tsv.gz", ".tsv.gz"),
+        ("filename.v1.1.0.spatialdata.zarr", ".spatialdata.zarr"),
     ]
     for path, suffix in collection:
         filepath = Path(path)
         assert suffix == extract_suffix_from_path(filepath)
```

### Comparing `lamindb_setup-0.71.0/tests/storage/test_storage_stats.py` & `lamindb_setup-0.71.1/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/tests/storage/test_to_url.py` & `lamindb_setup-0.71.1/tests/storage/test_to_url.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.71.0/PKG-INFO` & `lamindb_setup-0.71.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.71.0
+Version: 0.71.1
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

