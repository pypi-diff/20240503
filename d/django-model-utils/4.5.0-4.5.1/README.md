# Comparing `tmp/django-model-utils-4.5.0.tar.gz` & `tmp/django_model_utils-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-model-utils-4.5.0.tar", last modified: Mon Apr  1 19:06:55 2024, max compression
+gzip compressed data, was "django_model_utils-4.5.1.tar", last modified: Thu May  2 11:12:48 2024, max compression
```

## Comparing `django-model-utils-4.5.0.tar` & `django_model_utils-4.5.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.672269 django-model-utils-4.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.672269 django-model-utils-4.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/workflows/issue-manager.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/django_model_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 19:06:55.000000 django-model-utils-4.5.0/django_model_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.672269 django-model-utils-4.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/managers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/setup.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/docs/utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.668269 django-model-utils-4.5.0/model_utils/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.664269 django-model-utils-4.5.0/model_utils/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.676269 django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.668269 django-model-utils-4.5.0/model_utils/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/model_utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/tests/test_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35143 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_field_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_monitor_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_split_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_status_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_urlsafe_token_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_fields/test_uuid_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_inheritance_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.680269 django-model-utils-4.5.0/tests/test_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23165 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_inheritance_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_join_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_softdelete_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_managers/test_status_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_miscellaneous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:55.684269 django-model-utils-4.5.0/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_deferred_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_softdeletable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_timeframed_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_timestamped_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tests/test_models/test_uuid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      870 2024-04-01 19:06:45.000000 django-model-utils-4.5.0/translations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.066402 django_model_utils-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.054401 django_model_utils-4.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.054401 django_model_utils-4.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.github/workflows/issue-manager.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18167 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    21102 2024-05-02 11:12:48.066402 django_model_utils-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.066402 django_model_utils-4.5.1/django_model_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21102 2024-05-02 11:12:47.000000 django_model_utils-4.5.1/django_model_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-02 11:12:48.000000 django_model_utils-4.5.1/django_model_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:12:47.000000 django_model_utils-4.5.1/django_model_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:12:47.000000 django_model_utils-4.5.1/django_model_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 11:12:47.000000 django_model_utils-4.5.1/django_model_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 11:12:47.000000 django_model_utils-4.5.1/django_model_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/managers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/docs/utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.058401 django_model_utils-4.5.1/model_utils/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.062402 django_model_utils-4.5.1/model_utils/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.062402 django_model_utils-4.5.1/model_utils/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.050402 django_model_utils-4.5.1/model_utils/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.062402 django_model_utils-4.5.1/model_utils/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/model_utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 11:12:48.066402 django_model_utils-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.062402 django_model_utils-4.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.062402 django_model_utils-4.5.1/tests/test_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35143 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/test_field_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/test_monitor_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/test_split_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/test_status_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/test_urlsafe_token_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_fields/test_uuid_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_inheritance_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.066402 django_model_utils-4.5.1/tests/test_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23165 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_managers/test_inheritance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_managers/test_join_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_managers/test_query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_managers/test_softdelete_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_managers/test_status_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_miscellaneous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:48.066402 django_model_utils-4.5.1/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/test_deferred_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/test_softdeletable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/test_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/test_timeframed_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/test_timestamped_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tests/test_models/test_uuid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      870 2024-05-02 11:12:37.000000 django_model_utils-4.5.1/translations.py
```

### Comparing `django-model-utils-4.5.0/.github/workflows/issue-manager.yml` & `django_model_utils-4.5.1/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/.github/workflows/release.yml` & `django_model_utils-4.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/.github/workflows/test.yml` & `django_model_utils-4.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/AUTHORS.rst` & `django_model_utils-4.5.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/CHANGES.rst` & `django_model_utils-4.5.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 Changelog
 =========
 
-To be released
---------------
-- Add deprecation warning for MonitorField. The default value will be `None`
-  instead of `django.utils.timezone.now` - when nullable and without a default.
-- Add Brazilian Portuguese translation (GH-#578)
-- Don't use `post_init` signal for initialize tracker
+4.5.1 (2024-05-02)
+------------------
+- Remove `JoinQueryset.get_quoted_query()` by @mthuurne (GH-#618)
+
+4.5.0 (2024-04-01)
+------------------
+- Don't use `post_init` signal for initialize tracker by @meanmail in -  (GH-#556)
+- clarify docs for managers of SoftDeletableModel by @tadamcz in -  (GH-#589)
+- [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in -  (GH-#575)
+- `Language Support` - Add translations for Brazilian Portuguese by @gmcrocetti in -  (GH-#578)
+- Remove dead `init_deferred_fields` method by @joecox in -  (GH-#580)
+- Update where `ConnectionDoesNotExist` is imported from by @mthuurne in -  (GH-#566)
+- Remove arguments from `InheritanceQuerySetMixin._clone()` by @mthuurne in -  (GH-#567)
+- Allow running tests using sqlite by @jayvdb in -  (GH-#516)
+- `MonitorField` - Change default to None when the field is nullable  by @gmcrocetti in -  (GH-#577)
+- Explicitly re-export names from `__init__` module by @mthuurne in - (GH-#591)
+- Switch from freezegun to time-machine. by @adamchainz in -  (GH-#510)
+- USE_TZ = True by @foarsitter in -  (GH-#593)
+- Remove redundant definition of `JoinManager` from tests by @mthuurne in -  (GH-#594)
+- Pass reason to `@skip` decorator by @mthuurne in -  (GH-#595)
+- Resolve name clash among test models by @mthuurne in -  (GH-#596)
+- Remove obsolete `tests.signals` module by @mthuurne in -  (GH-#597)
+- Remove obsolete test models by @mthuurne in -  (GH-#598)
+- Postgresql docker container for local development by @foarsitter in -  (GH-#563)
+- [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in -  (GH-#602)
+- Add issue-manager by @foarsitter in -  (GH-#600)
+- Translation files by @foarsitter in -  (GH-#608)
 
 4.4.0 (2024-02-10)
 ------------------
 
 - Add support for `Python 3.11` (GH-#545)
 - Add support for `Python 3.12` (GH-#545)
 - Drop support for `Python 3.7` (GH-#545)
```

### Comparing `django-model-utils-4.5.0/CODE_OF_CONDUCT.md` & `django_model_utils-4.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/CONTRIBUTING.rst` & `django_model_utils-4.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/LICENSE.txt` & `django_model_utils-4.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/Makefile` & `django_model_utils-4.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/PKG-INFO` & `django_model_utils-4.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-utils
-Version: 4.5.0
+Version: 4.5.1
 Summary: Django model mixins and utilities
 Home-page: https://github.com/jazzband/django-model-utils
 Author: Carl Meyer
 Author-email: carl@oddbird.net
 Maintainer: JazzBand
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
@@ -86,20 +86,41 @@
 .. _issue tracker: https://github.com/jazzband/django-model-utils/issues
 .. _CONTRIBUTING.rst: https://github.com/jazzband/django-model-utils/blob/master/CONTRIBUTING.rst
 
 
 Changelog
 =========
 
-To be released
---------------
-- Add deprecation warning for MonitorField. The default value will be `None`
-  instead of `django.utils.timezone.now` - when nullable and without a default.
-- Add Brazilian Portuguese translation (GH-#578)
-- Don't use `post_init` signal for initialize tracker
+4.5.1 (2024-05-02)
+------------------
+- Remove `JoinQueryset.get_quoted_query()` by @mthuurne (GH-#618)
+
+4.5.0 (2024-04-01)
+------------------
+- Don't use `post_init` signal for initialize tracker by @meanmail in -  (GH-#556)
+- clarify docs for managers of SoftDeletableModel by @tadamcz in -  (GH-#589)
+- [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in -  (GH-#575)
+- `Language Support` - Add translations for Brazilian Portuguese by @gmcrocetti in -  (GH-#578)
+- Remove dead `init_deferred_fields` method by @joecox in -  (GH-#580)
+- Update where `ConnectionDoesNotExist` is imported from by @mthuurne in -  (GH-#566)
+- Remove arguments from `InheritanceQuerySetMixin._clone()` by @mthuurne in -  (GH-#567)
+- Allow running tests using sqlite by @jayvdb in -  (GH-#516)
+- `MonitorField` - Change default to None when the field is nullable  by @gmcrocetti in -  (GH-#577)
+- Explicitly re-export names from `__init__` module by @mthuurne in - (GH-#591)
+- Switch from freezegun to time-machine. by @adamchainz in -  (GH-#510)
+- USE_TZ = True by @foarsitter in -  (GH-#593)
+- Remove redundant definition of `JoinManager` from tests by @mthuurne in -  (GH-#594)
+- Pass reason to `@skip` decorator by @mthuurne in -  (GH-#595)
+- Resolve name clash among test models by @mthuurne in -  (GH-#596)
+- Remove obsolete `tests.signals` module by @mthuurne in -  (GH-#597)
+- Remove obsolete test models by @mthuurne in -  (GH-#598)
+- Postgresql docker container for local development by @foarsitter in -  (GH-#563)
+- [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in -  (GH-#602)
+- Add issue-manager by @foarsitter in -  (GH-#600)
+- Translation files by @foarsitter in -  (GH-#608)
 
 4.4.0 (2024-02-10)
 ------------------
 
 - Add support for `Python 3.11` (GH-#545)
 - Add support for `Python 3.12` (GH-#545)
 - Drop support for `Python 3.7` (GH-#545)
```

### Comparing `django-model-utils-4.5.0/README.rst` & `django_model_utils-4.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/django_model_utils.egg-info/PKG-INFO` & `django_model_utils-4.5.1/django_model_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-utils
-Version: 4.5.0
+Version: 4.5.1
 Summary: Django model mixins and utilities
 Home-page: https://github.com/jazzband/django-model-utils
 Author: Carl Meyer
 Author-email: carl@oddbird.net
 Maintainer: JazzBand
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
@@ -86,20 +86,41 @@
 .. _issue tracker: https://github.com/jazzband/django-model-utils/issues
 .. _CONTRIBUTING.rst: https://github.com/jazzband/django-model-utils/blob/master/CONTRIBUTING.rst
 
 
 Changelog
 =========
 
-To be released
---------------
-- Add deprecation warning for MonitorField. The default value will be `None`
-  instead of `django.utils.timezone.now` - when nullable and without a default.
-- Add Brazilian Portuguese translation (GH-#578)
-- Don't use `post_init` signal for initialize tracker
+4.5.1 (2024-05-02)
+------------------
+- Remove `JoinQueryset.get_quoted_query()` by @mthuurne (GH-#618)
+
+4.5.0 (2024-04-01)
+------------------
+- Don't use `post_init` signal for initialize tracker by @meanmail in -  (GH-#556)
+- clarify docs for managers of SoftDeletableModel by @tadamcz in -  (GH-#589)
+- [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in -  (GH-#575)
+- `Language Support` - Add translations for Brazilian Portuguese by @gmcrocetti in -  (GH-#578)
+- Remove dead `init_deferred_fields` method by @joecox in -  (GH-#580)
+- Update where `ConnectionDoesNotExist` is imported from by @mthuurne in -  (GH-#566)
+- Remove arguments from `InheritanceQuerySetMixin._clone()` by @mthuurne in -  (GH-#567)
+- Allow running tests using sqlite by @jayvdb in -  (GH-#516)
+- `MonitorField` - Change default to None when the field is nullable  by @gmcrocetti in -  (GH-#577)
+- Explicitly re-export names from `__init__` module by @mthuurne in - (GH-#591)
+- Switch from freezegun to time-machine. by @adamchainz in -  (GH-#510)
+- USE_TZ = True by @foarsitter in -  (GH-#593)
+- Remove redundant definition of `JoinManager` from tests by @mthuurne in -  (GH-#594)
+- Pass reason to `@skip` decorator by @mthuurne in -  (GH-#595)
+- Resolve name clash among test models by @mthuurne in -  (GH-#596)
+- Remove obsolete `tests.signals` module by @mthuurne in -  (GH-#597)
+- Remove obsolete test models by @mthuurne in -  (GH-#598)
+- Postgresql docker container for local development by @foarsitter in -  (GH-#563)
+- [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in -  (GH-#602)
+- Add issue-manager by @foarsitter in -  (GH-#600)
+- Translation files by @foarsitter in -  (GH-#608)
 
 4.4.0 (2024-02-10)
 ------------------
 
 - Add support for `Python 3.11` (GH-#545)
 - Add support for `Python 3.12` (GH-#545)
 - Drop support for `Python 3.7` (GH-#545)
```

### Comparing `django-model-utils-4.5.0/django_model_utils.egg-info/SOURCES.txt` & `django_model_utils-4.5.1/django_model_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/Makefile` & `django_model_utils-4.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/conf.py` & `django_model_utils-4.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/fields.rst` & `django_model_utils-4.5.1/docs/fields.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/index.rst` & `django_model_utils-4.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/make.bat` & `django_model_utils-4.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/managers.rst` & `django_model_utils-4.5.1/docs/managers.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/models.rst` & `django_model_utils-4.5.1/docs/models.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/docs/utilities.rst` & `django_model_utils-4.5.1/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/choices.py` & `django_model_utils-4.5.1/model_utils/choices.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/fields.py` & `django_model_utils-4.5.1/model_utils/fields.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/cs/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/de/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/es/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/fa/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/fr/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/pt_BR/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/ru/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/sv/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_model_utils-4.5.1/model_utils/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/locale/zh_Hans/LC_MESSAGES/django.po` & `django_model_utils-4.5.1/model_utils/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/managers.py` & `django_model_utils-4.5.1/model_utils/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,29 +299,14 @@
 
 class SoftDeletableManager(SoftDeletableManagerMixin, models.Manager):
     pass
 
 
 class JoinQueryset(models.QuerySet):
 
-    def get_quoted_query(self, query):
-        query, params = query.sql_with_params()
-
-        # Put additional quotes around string.
-        params = [
-            f'\'{p}\''
-            if isinstance(p, str) else p
-            for p in params
-        ]
-
-        # Cast list of parameters to tuple because I got
-        # "not enough format characters" otherwise.
-        params = tuple(params)
-        return query % params
-
     def join(self, qs=None):
         '''
         Join one queryset together with another using a temporary table. If
         no queryset is used, it will use the current queryset and join that
         to itself.
 
         `Join` either uses the current queryset and effectively does a self-join to
@@ -355,24 +340,24 @@
             new_qs = self
         else:
             fk_column = 'id'
             qs = self.only(fk_column)
             new_qs = self.model.objects.all()
 
         TABLE_NAME = 'temp_stuff'
-        query = self.get_quoted_query(qs.query)
+        query, params = qs.query.sql_with_params()
         sql = '''
             DROP TABLE IF EXISTS {table_name};
             DROP INDEX IF EXISTS {table_name}_id;
             CREATE TEMPORARY TABLE {table_name} AS {query};
             CREATE INDEX {table_name}_{fk_column} ON {table_name} ({fk_column});
         '''.format(table_name=TABLE_NAME, fk_column=fk_column, query=str(query))
 
         with connection.cursor() as cursor:
-            cursor.execute(sql)
+            cursor.execute(sql, params)
 
         class TempModel(models.Model):
             temp_key = models.ForeignKey(
                 self.model,
                 on_delete=models.DO_NOTHING,
                 db_column=fk_column,
                 to_field=to_field
```

### Comparing `django-model-utils-4.5.0/model_utils/models.py` & `django_model_utils-4.5.1/model_utils/models.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/model_utils/tracker.py` & `django_model_utils-4.5.1/model_utils/tracker.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/setup.py` & `django_model_utils-4.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/fields.py` & `django_model_utils-4.5.1/tests/fields.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/models.py` & `django_model_utils-4.5.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/settings.py` & `django_model_utils-4.5.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_choices.py` & `django_model_utils-4.5.1/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_fields/test_field_tracker.py` & `django_model_utils-4.5.1/tests/test_fields/test_field_tracker.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_fields/test_monitor_field.py` & `django_model_utils-4.5.1/tests/test_fields/test_monitor_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_fields/test_split_field.py` & `django_model_utils-4.5.1/tests/test_fields/test_split_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_fields/test_status_field.py` & `django_model_utils-4.5.1/tests/test_fields/test_status_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_fields/test_urlsafe_token_field.py` & `django_model_utils-4.5.1/tests/test_fields/test_urlsafe_token_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_fields/test_uuid_field.py` & `django_model_utils-4.5.1/tests/test_fields/test_uuid_field.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_inheritance_iterable.py` & `django_model_utils-4.5.1/tests/test_inheritance_iterable.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_managers/test_inheritance_manager.py` & `django_model_utils-4.5.1/tests/test_managers/test_inheritance_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_managers/test_join_manager.py` & `django_model_utils-4.5.1/tests/test_managers/test_join_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_managers/test_query_manager.py` & `django_model_utils-4.5.1/tests/test_managers/test_query_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_managers/test_softdelete_manager.py` & `django_model_utils-4.5.1/tests/test_managers/test_softdelete_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_managers/test_status_manager.py` & `django_model_utils-4.5.1/tests/test_managers/test_status_manager.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_miscellaneous.py` & `django_model_utils-4.5.1/tests/test_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_models/test_deferred_fields.py` & `django_model_utils-4.5.1/tests/test_models/test_deferred_fields.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_models/test_softdeletable_model.py` & `django_model_utils-4.5.1/tests/test_models/test_softdeletable_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_models/test_status_model.py` & `django_model_utils-4.5.1/tests/test_models/test_status_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_models/test_timeframed_model.py` & `django_model_utils-4.5.1/tests/test_models/test_timeframed_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_models/test_timestamped_model.py` & `django_model_utils-4.5.1/tests/test_models/test_timestamped_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tests/test_models/test_uuid_model.py` & `django_model_utils-4.5.1/tests/test_models/test_uuid_model.py`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/tox.ini` & `django_model_utils-4.5.1/tox.ini`

 * *Files identical despite different names*

### Comparing `django-model-utils-4.5.0/translations.py` & `django_model_utils-4.5.1/translations.py`

 * *Files identical despite different names*

