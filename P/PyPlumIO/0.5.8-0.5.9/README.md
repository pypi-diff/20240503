# Comparing `tmp/PyPlumIO-0.5.8.tar.gz` & `tmp/PyPlumIO-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPlumIO-0.5.8.tar", last modified: Sun Nov 26 00:55:33 2023, max compression
+gzip compressed data, was "PyPlumIO-0.5.9.tar", last modified: Sun Nov 26 22:31:15 2023, max compression
```

## Comparing `PyPlumIO-0.5.8.tar` & `PyPlumIO-0.5.9.tar`

### file list

```diff
@@ -1,162 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.569501 PyPlumIO-0.5.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.569501 PyPlumIO-0.5.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.569501 PyPlumIO-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.573500 PyPlumIO-0.5.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/PyPlumIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2023-11-26 00:55:33.000000 PyPlumIO-0.5.8/PyPlumIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2023-11-26 00:55:33.000000 PyPlumIO-0.5.8/PyPlumIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 00:55:33.000000 PyPlumIO-0.5.8/PyPlumIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-26 00:55:33.000000 PyPlumIO-0.5.8/PyPlumIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-26 00:55:33.000000 PyPlumIO-0.5.8/PyPlumIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/disagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.573500 PyPlumIO-0.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.573500 PyPlumIO-0.5.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/callbacks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/connecting.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/mixers_thermostats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/reading.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/schedules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/docs/source/writing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.573500 PyPlumIO-0.5.8/images/
--rw-r--r--   0 runner    (1001) docker     (127)    32463 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/images/ecomax.png
--rw-r--r--   0 runner    (1001) docker     (127)   133458 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/images/rs485.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.577500 PyPlumIO-0.5.8/pyplumio/
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-26 00:55:33.000000 PyPlumIO-0.5.8/pyplumio/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.577500 PyPlumIO-0.5.8/pyplumio/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/devices/ecomax.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/devices/ecoster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/devices/mixer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.577500 PyPlumIO-0.5.8/pyplumio/frames/
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/frames/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/frames/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/frames/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.577500 PyPlumIO-0.5.8/pyplumio/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/helpers/uid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.581500 PyPlumIO-0.5.8/pyplumio/structures/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/boiler_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/boiler_power.py
--rw-r--r--   0 runner    (1001) docker     (127)    25931 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/ecomax_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/fan_power.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/frame_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/fuel_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/lambda_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/mixer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/mixer_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/network_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/output_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/pending_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/product_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/program_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/regulator_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/regulator_data_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/temperatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/thermostat_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/structures/thermostat_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyplumio/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.585500 PyPlumIO-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.585500 PyPlumIO-0.5.8/tests/frames/
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/frames/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/frames/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/frames/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/frames/test_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.585500 PyPlumIO-0.5.8/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/helpers/test_uid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25555 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.569501 PyPlumIO-0.5.8/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.585500 PyPlumIO-0.5.8/tests/testdata/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/messages/regulator_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/messages/sensor_data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/tests/testdata/requests/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/alerts.json
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/ecomax_control.json
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/ecomax_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/mixer_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/set_ecomax_parameter.json
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/set_mixer_parameter.json
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/set_schedule.json
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/set_thermostat_parameter.json
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/requests/thermostat_parameters.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/tests/testdata/responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/alerts.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/device_available.json
--rw-r--r--   0 runner    (1001) docker     (127)    18031 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/ecomax_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/mixer_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/password.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/program_version.json
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/regulator_data_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/schedules.json
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/thermostat_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/responses/uid.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 00:55:33.589500 PyPlumIO-0.5.8/tests/testdata/unknown/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/unknown/unknown_ecomax_parameter.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tests/testdata/unknown/unknown_mixer_parameter.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-11-26 00:55:16.000000 PyPlumIO-0.5.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.565639 PyPlumIO-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.541639 PyPlumIO-0.5.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.545639 PyPlumIO-0.5.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.545639 PyPlumIO-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.545639 PyPlumIO-0.5.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2023-11-26 22:31:15.565639 PyPlumIO-0.5.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.565639 PyPlumIO-0.5.9/PyPlumIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2023-11-26 22:31:15.000000 PyPlumIO-0.5.9/PyPlumIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2023-11-26 22:31:15.000000 PyPlumIO-0.5.9/PyPlumIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 22:31:15.000000 PyPlumIO-0.5.9/PyPlumIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-26 22:31:15.000000 PyPlumIO-0.5.9/PyPlumIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-26 22:31:15.000000 PyPlumIO-0.5.9/PyPlumIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.545639 PyPlumIO-0.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.545639 PyPlumIO-0.5.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/callbacks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/connecting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/mixers_thermostats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/reading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/schedules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/docs/source/writing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.549639 PyPlumIO-0.5.9/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    32463 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/images/ecomax.png
+-rw-r--r--   0 runner    (1001) docker     (127)   133458 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/images/rs485.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.549639 PyPlumIO-0.5.9/pyplumio/
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-26 22:31:15.000000 PyPlumIO-0.5.9/pyplumio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.549639 PyPlumIO-0.5.9/pyplumio/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/devices/ecomax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/devices/ecoster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/devices/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.549639 PyPlumIO-0.5.9/pyplumio/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/frames/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/frames/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/frames/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.553639 PyPlumIO-0.5.9/pyplumio/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/helpers/uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.557639 PyPlumIO-0.5.9/pyplumio/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/boiler_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/boiler_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25931 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/ecomax_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/fan_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/frame_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/fuel_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/lambda_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/mixer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/mixer_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/network_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/output_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-11-26 22:30:56.000000 PyPlumIO-0.5.9/pyplumio/structures/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/pending_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/product_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/program_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/regulator_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/regulator_data_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/temperatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/thermostat_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/structures/thermostat_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyplumio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 22:31:15.565639 PyPlumIO-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.557639 PyPlumIO-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.561639 PyPlumIO-0.5.9/tests/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/frames/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/frames/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/frames/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/frames/test_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.561639 PyPlumIO-0.5.9/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/helpers/test_uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25629 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.541639 PyPlumIO-0.5.9/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.561639 PyPlumIO-0.5.9/tests/testdata/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/messages/regulator_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/messages/sensor_data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.561639 PyPlumIO-0.5.9/tests/testdata/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/alerts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/ecomax_control.json
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/ecomax_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/mixer_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/set_ecomax_parameter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/set_mixer_parameter.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/set_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/set_thermostat_parameter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/requests/thermostat_parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.565639 PyPlumIO-0.5.9/tests/testdata/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/alerts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/device_available.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18031 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/ecomax_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/mixer_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/password.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/program_version.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/regulator_data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17437 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/schedules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/thermostat_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/responses/uid.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 22:31:15.565639 PyPlumIO-0.5.9/tests/testdata/unknown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/unknown/unknown_ecomax_parameter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tests/testdata/unknown/unknown_mixer_parameter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-11-26 22:30:57.000000 PyPlumIO-0.5.9/tox.ini
```

### Comparing `PyPlumIO-0.5.8/.github/CODE_OF_CONDUCT.md` & `PyPlumIO-0.5.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `PyPlumIO-0.5.9/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.github/ISSUE_TEMPLATE/feature_request.yml` & `PyPlumIO-0.5.9/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.github/workflows/ci.yml` & `PyPlumIO-0.5.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.github/workflows/codeql-analysis.yml` & `PyPlumIO-0.5.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.github/workflows/deploy.yml` & `PyPlumIO-0.5.9/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.github/workflows/documentation.yml` & `PyPlumIO-0.5.9/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.gitignore` & `PyPlumIO-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/.pre-commit-config.yaml` & `PyPlumIO-0.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/LICENSE` & `PyPlumIO-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/PKG-INFO` & `PyPlumIO-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.5.8
+Version: 0.5.9
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
 Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
```

### Comparing `PyPlumIO-0.5.8/PyPlumIO.egg-info/PKG-INFO` & `PyPlumIO-0.5.9/PyPlumIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.5.8
+Version: 0.5.9
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
 Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
```

### Comparing `PyPlumIO-0.5.8/PyPlumIO.egg-info/SOURCES.txt` & `PyPlumIO-0.5.9/PyPlumIO.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
-disagnostics.py
 pyproject.toml
 requirements.txt
 requirements_test.txt
 tox.ini
 .github/CODE_OF_CONDUCT.md
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
```

### Comparing `PyPlumIO-0.5.8/README.md` & `PyPlumIO-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/Makefile` & `PyPlumIO-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/make.bat` & `PyPlumIO-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/callbacks.rst` & `PyPlumIO-0.5.9/docs/source/callbacks.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/conf.py` & `PyPlumIO-0.5.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/connecting.rst` & `PyPlumIO-0.5.9/docs/source/connecting.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/index.rst` & `PyPlumIO-0.5.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/mixers_thermostats.rst` & `PyPlumIO-0.5.9/docs/source/mixers_thermostats.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/protocol.rst` & `PyPlumIO-0.5.9/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/reading.rst` & `PyPlumIO-0.5.9/docs/source/reading.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/schedules.rst` & `PyPlumIO-0.5.9/docs/source/schedules.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/docs/source/writing.rst` & `PyPlumIO-0.5.9/docs/source/writing.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/images/ecomax.png` & `PyPlumIO-0.5.9/images/ecomax.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/images/rs485.png` & `PyPlumIO-0.5.9/images/rs485.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/__init__.py` & `PyPlumIO-0.5.9/pyplumio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains connection shortcuts and version information."""
 from __future__ import annotations
 
 from pyplumio._version import __version__, __version_tuple__
-from pyplumio.connection import SerialConnection, TcpConnection
+from pyplumio.connection import Connection, SerialConnection, TcpConnection
 from pyplumio.exceptions import (
     ChecksumError,
     ConnectionFailedError,
     FrameDataError,
     FrameError,
     PyPlumIOError,
     ReadError,
@@ -102,14 +102,15 @@
         reconnect_on_failure=reconnect_on_failure,
         protocol=protocol,
         **kwargs,
     )
 
 
 __all__ = [
+    "Connection",
     "SerialConnection",
     "TcpConnection",
     "Protocol",
     "AsyncProtocol",
     "DummyProtocol",
     "EthernetParameters",
     "WirelessParameters",
```

### Comparing `PyPlumIO-0.5.8/pyplumio/connection.py` & `PyPlumIO-0.5.9/pyplumio/connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/const.py` & `PyPlumIO-0.5.9/pyplumio/const.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/devices/__init__.py` & `PyPlumIO-0.5.9/pyplumio/devices/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,19 +149,15 @@
         ]
 
         await self.dispatch(ATTR_FRAME_ERRORS, errors)
         await self.dispatch(ATTR_LOADED, True)
         return True
 
     async def request(
-        self,
-        name: str,
-        frame_type: FrameType,
-        retries: int = 3,
-        timeout: float = 3.0,
+        self, name: str, frame_type: FrameType, retries: int = 3, timeout: float = 3.0
     ):
         """Send request for a data and wait for a value to become
         available.
 
         If value is not available before timeout, retry request.
         """
         request: Request = factory(
```

### Comparing `PyPlumIO-0.5.8/pyplumio/devices/ecomax.py` & `PyPlumIO-0.5.9/pyplumio/devices/ecomax.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     Request,
     get_frame_handler,
     is_known_frame_type,
 )
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import ParameterValues
 from pyplumio.helpers.schedule import Schedule, ScheduleDay
-from pyplumio.structures.alerts import ATTR_ALERTS
+from pyplumio.structures.alerts import ATTR_TOTAL_ALERTS
 from pyplumio.structures.ecomax_parameters import (
     ATTR_ECOMAX_CONTROL,
     ATTR_ECOMAX_PARAMETERS,
     ECOMAX_CONTROL_PARAMETER,
     ECOMAX_PARAMETERS,
     THERMOSTAT_PROFILE_PARAMETER,
     EcomaxBinaryParameter,
@@ -73,15 +73,17 @@
     DataFrameDescription(frame_type=FrameType.REQUEST_UID, provides=ATTR_PRODUCT),
     DataFrameDescription(
         frame_type=FrameType.REQUEST_REGULATOR_DATA_SCHEMA, provides=ATTR_REGDATA_SCHEMA
     ),
     DataFrameDescription(
         frame_type=FrameType.REQUEST_ECOMAX_PARAMETERS, provides=ATTR_ECOMAX_PARAMETERS
     ),
-    DataFrameDescription(frame_type=FrameType.REQUEST_ALERTS, provides=ATTR_ALERTS),
+    DataFrameDescription(
+        frame_type=FrameType.REQUEST_ALERTS, provides=ATTR_TOTAL_ALERTS
+    ),
     DataFrameDescription(
         frame_type=FrameType.REQUEST_SCHEDULES, provides=ATTR_SCHEDULES
     ),
     DataFrameDescription(
         frame_type=FrameType.REQUEST_MIXER_PARAMETERS, provides=ATTR_MIXER_PARAMETERS
     ),
     DataFrameDescription(
@@ -190,15 +192,15 @@
             try:
                 description = ECOMAX_PARAMETERS[product.type][index]
             except IndexError:
                 _LOGGER.warning(
                     (
                         "Encountered unknown ecoMAX parameter (%i): %s. "
                         "Your device isn't fully compatible with this software and "
-                        "may not work properly."
+                        "may not work properly. "
                         "Please visit the issue tracker and open a feature "
                         "request to support %s"
                     ),
                     index,
                     values,
                     product.model,
                 )
```

### Comparing `PyPlumIO-0.5.8/pyplumio/devices/mixer.py` & `PyPlumIO-0.5.9/pyplumio/devices/mixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             try:
                 description = MIXER_PARAMETERS[product.type][index]
             except IndexError:
                 _LOGGER.warning(
                     (
                         "Encountered unknown mixer parameter (%i): %s. "
                         "Your device isn't fully compatible with this software and "
-                        "may not work properly."
+                        "may not work properly. "
                         "Please visit the issue tracker and open a feature "
                         "request to support %s"
                     ),
                     index,
                     values,
                     product.model,
                 )
```

### Comparing `PyPlumIO-0.5.8/pyplumio/devices/thermostat.py` & `PyPlumIO-0.5.9/pyplumio/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/exceptions.py` & `PyPlumIO-0.5.9/pyplumio/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/filters.py` & `PyPlumIO-0.5.9/pyplumio/filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/frames/__init__.py` & `PyPlumIO-0.5.9/pyplumio/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/frames/messages.py` & `PyPlumIO-0.5.9/pyplumio/frames/messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/frames/requests.py` & `PyPlumIO-0.5.9/pyplumio/frames/requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/frames/responses.py` & `PyPlumIO-0.5.9/pyplumio/frames/responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/data_types.py` & `PyPlumIO-0.5.9/pyplumio/helpers/data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/event_manager.py` & `PyPlumIO-0.5.9/pyplumio/helpers/event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/factory.py` & `PyPlumIO-0.5.9/pyplumio/helpers/factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/parameter.py` & `PyPlumIO-0.5.9/pyplumio/helpers/parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/schedule.py` & `PyPlumIO-0.5.9/pyplumio/helpers/schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/task_manager.py` & `PyPlumIO-0.5.9/pyplumio/helpers/task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/timeout.py` & `PyPlumIO-0.5.9/pyplumio/helpers/timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/helpers/uid.py` & `PyPlumIO-0.5.9/pyplumio/helpers/uid.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/protocol.py` & `PyPlumIO-0.5.9/pyplumio/protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/stream.py` & `PyPlumIO-0.5.9/pyplumio/stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/__init__.py` & `PyPlumIO-0.5.9/pyplumio/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/alerts.py` & `PyPlumIO-0.5.9/pyplumio/structures/alerts.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from pyplumio.const import AlertType
 from pyplumio.helpers.data_types import UnsignedInt
 from pyplumio.structures import StructureDecoder
 from pyplumio.utils import ensure_dict
 
 ATTR_ALERTS: Final = "alerts"
+ATTR_TOTAL_ALERTS: Final = "total_alerts"
 
 
 @lru_cache(maxsize=10)
 def _convert_to_datetime(seconds: int) -> datetime:
     """Convert timestamp to a datetime object."""
 
     def _seconds_to_datetime_args(seconds: int) -> Generator[Any, None, None]:
@@ -72,26 +73,28 @@
 
         return Alert(code, from_dt, to_dt)
 
     def decode(
         self, message: bytearray, offset: int = 0, data: dict[str, Any] | None = None
     ) -> tuple[dict[str, Any], int]:
         """Decode bytes and return message data and offset."""
+        total_alerts = message[offset + 0]
         start = message[offset + 1]
         end = message[offset + 2]
 
         if end == 0:
             # No alerts found.
-            return ensure_dict(data), offset + 1
+            return ensure_dict(data, {ATTR_TOTAL_ALERTS: total_alerts}), offset + 3
 
         self._offset = offset + 3
         return (
             ensure_dict(
                 data,
                 {
                     ATTR_ALERTS: [
                         self._unpack_alert(message) for _ in range(start, start + end)
-                    ]
+                    ],
+                    ATTR_TOTAL_ALERTS: total_alerts,
                 },
             ),
             self._offset,
         )
```

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/boiler_load.py` & `PyPlumIO-0.5.9/pyplumio/structures/boiler_load.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/boiler_power.py` & `PyPlumIO-0.5.9/pyplumio/structures/boiler_power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/ecomax_parameters.py` & `PyPlumIO-0.5.9/pyplumio/structures/ecomax_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/fan_power.py` & `PyPlumIO-0.5.9/pyplumio/structures/fan_power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/frame_versions.py` & `PyPlumIO-0.5.9/pyplumio/structures/frame_versions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/fuel_consumption.py` & `PyPlumIO-0.5.9/pyplumio/structures/fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/fuel_level.py` & `PyPlumIO-0.5.9/pyplumio/structures/fuel_level.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/lambda_sensor.py` & `PyPlumIO-0.5.9/pyplumio/structures/lambda_sensor.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/mixer_parameters.py` & `PyPlumIO-0.5.9/pyplumio/structures/mixer_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/mixer_sensors.py` & `PyPlumIO-0.5.9/pyplumio/structures/mixer_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/modules.py` & `PyPlumIO-0.5.9/pyplumio/structures/modules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/network_info.py` & `PyPlumIO-0.5.9/pyplumio/structures/network_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/output_flags.py` & `PyPlumIO-0.5.9/pyplumio/structures/output_flags.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/outputs.py` & `PyPlumIO-0.5.9/pyplumio/structures/outputs.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/pending_alerts.py` & `PyPlumIO-0.5.9/pyplumio/structures/pending_alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/product_info.py` & `PyPlumIO-0.5.9/pyplumio/structures/product_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/program_version.py` & `PyPlumIO-0.5.9/pyplumio/structures/program_version.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/regulator_data.py` & `PyPlumIO-0.5.9/pyplumio/structures/regulator_data.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/regulator_data_schema.py` & `PyPlumIO-0.5.9/pyplumio/structures/regulator_data_schema.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/schedules.py` & `PyPlumIO-0.5.9/pyplumio/structures/schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     __slots__ = ()
 
     device: AddressableDevice
 
     @property
     def request(self) -> Request:
         """A request to change the parameter."""
-        schedule_name, _ = self.description.name.split("_", 1)
+        schedule_name, _ = self.description.name.split("_schedule_", 1)
         return factory(
             "frames.requests.SetScheduleRequest",
             recipient=self.device.address,
             data=collect_schedule_data(schedule_name, self.device),
         )
```

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/statuses.py` & `PyPlumIO-0.5.9/pyplumio/structures/statuses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/temperatures.py` & `PyPlumIO-0.5.9/pyplumio/structures/temperatures.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/thermostat_parameters.py` & `PyPlumIO-0.5.9/pyplumio/structures/thermostat_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/structures/thermostat_sensors.py` & `PyPlumIO-0.5.9/pyplumio/structures/thermostat_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyplumio/utils.py` & `PyPlumIO-0.5.9/pyplumio/utils.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/pyproject.toml` & `PyPlumIO-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/__init__.py` & `PyPlumIO-0.5.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/conftest.py` & `PyPlumIO-0.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/frames/test_init.py` & `PyPlumIO-0.5.9/tests/frames/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/frames/test_messages.py` & `PyPlumIO-0.5.9/tests/frames/test_messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/frames/test_requests.py` & `PyPlumIO-0.5.9/tests/frames/test_requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/frames/test_responses.py` & `PyPlumIO-0.5.9/tests/frames/test_responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_data_types.py` & `PyPlumIO-0.5.9/tests/helpers/test_data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_event_manager.py` & `PyPlumIO-0.5.9/tests/helpers/test_event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_factory.py` & `PyPlumIO-0.5.9/tests/helpers/test_factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_parameter.py` & `PyPlumIO-0.5.9/tests/helpers/test_parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_schedule.py` & `PyPlumIO-0.5.9/tests/helpers/test_schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_task_manager.py` & `PyPlumIO-0.5.9/tests/helpers/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/helpers/test_timeout.py` & `PyPlumIO-0.5.9/tests/helpers/test_timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_connection.py` & `PyPlumIO-0.5.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_devices.py` & `PyPlumIO-0.5.9/tests/test_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,33 +492,35 @@
     load_json_parameters("responses/schedules.json"),
 )
 async def test_schedule_callback(ecomax: EcoMAX, message, data) -> None:
     """Test callback that is dispatched on receiving schedule data."""
     ecomax.handle_frame(SchedulesResponse(message=message))
     await ecomax.wait_until_done()
     schedules = await ecomax.get(ATTR_SCHEDULES)
-    assert len(schedules) == 1
+    assert len(schedules) == 2
     heating_schedule = schedules["heating"]
     assert isinstance(heating_schedule, Schedule)
 
     heating_schedule_switch = await ecomax.get("heating_schedule_switch")
     assert heating_schedule_switch.value == STATE_OFF
     assert isinstance(heating_schedule_switch, ScheduleBinaryParameter)
 
-    heating_schedule_parameter = await ecomax.get("heating_schedule_parameter")
-    assert isinstance(heating_schedule_parameter, ScheduleParameter)
-    assert isinstance(heating_schedule_parameter.request, SetScheduleRequest)
-    assert heating_schedule_parameter.value == 5
-    assert heating_schedule_parameter.min_value == 0
-    assert heating_schedule_parameter.max_value == 30
-    assert heating_schedule_parameter.request.data == {
-        ATTR_TYPE: "heating",
-        ATTR_SWITCH: ecomax.data[f"heating_{ATTR_SCHEDULE_SWITCH}"],
-        ATTR_PARAMETER: ecomax.data[f"heating_{ATTR_SCHEDULE_PARAMETER}"],
-        ATTR_SCHEDULE: ecomax.data[ATTR_SCHEDULES]["heating"],
+    water_heater_schedule_parameter = await ecomax.get(
+        "water_heater_schedule_parameter"
+    )
+    assert isinstance(water_heater_schedule_parameter, ScheduleParameter)
+    assert isinstance(water_heater_schedule_parameter.request, SetScheduleRequest)
+    assert water_heater_schedule_parameter.value == 5
+    assert water_heater_schedule_parameter.min_value == 0
+    assert water_heater_schedule_parameter.max_value == 30
+    assert water_heater_schedule_parameter.request.data == {
+        ATTR_TYPE: "water_heater",
+        ATTR_SWITCH: ecomax.data[f"water_heater_{ATTR_SCHEDULE_SWITCH}"],
+        ATTR_PARAMETER: ecomax.data[f"water_heater_{ATTR_SCHEDULE_PARAMETER}"],
+        ATTR_SCHEDULE: ecomax.data[ATTR_SCHEDULES]["water_heater"],
     }
 
     schedule_data = data[ATTR_SCHEDULES][0][1]
     for index, weekday in enumerate(
         ("monday", "tuesday", "wednesday", "thursday", "friday", "saturday", "sunday")
     ):
         schedule = getattr(heating_schedule, weekday)
```

### Comparing `PyPlumIO-0.5.8/tests/test_filters.py` & `PyPlumIO-0.5.9/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_init.py` & `PyPlumIO-0.5.9/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_main.py` & `PyPlumIO-0.5.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_protocol.py` & `PyPlumIO-0.5.9/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_stream.py` & `PyPlumIO-0.5.9/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/test_utils.py` & `PyPlumIO-0.5.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/messages/regulator_data.json` & `PyPlumIO-0.5.9/tests/testdata/messages/regulator_data.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/messages/sensor_data.json` & `PyPlumIO-0.5.9/tests/testdata/messages/sensor_data.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/requests/alerts.json` & `PyPlumIO-0.5.9/tests/testdata/requests/alerts.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/requests/ecomax_parameters.json` & `PyPlumIO-0.5.9/tests/testdata/requests/ecomax_parameters.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/requests/mixer_parameters.json` & `PyPlumIO-0.5.9/tests/testdata/requests/mixer_parameters.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/requests/set_schedule.json` & `PyPlumIO-0.5.9/tests/testdata/requests/set_schedule.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/requests/thermostat_parameters.json` & `PyPlumIO-0.5.9/tests/testdata/requests/thermostat_parameters.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/alerts.json` & `PyPlumIO-0.5.9/tests/testdata/responses/alerts.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'0': "{'data': {'total_alerts': 100}}",*

 * * '1': "{'data': {replace: OrderedDict([('total_alerts', 0)])}}"}*

```diff
@@ -41,26 +41,29 @@
                         "hour": 22,
                         "minute": 33,
                         "month": 7,
                         "year": 2022
                     },
                     "to_dt": null
                 }
-            ]
+            ],
+            "total_alerts": 100
         },
         "id": "alerts",
         "message": {
             "__bytearray__": true,
             "items": [
                 "6400021A5493382B9B94382B009C97372B00000000"
             ]
         }
     },
     {
-        "data": {},
+        "data": {
+            "total_alerts": 0
+        },
         "id": "empty_alerts",
         "message": {
             "__bytearray__": true,
             "items": [
                 "000000"
             ]
         }
```

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/device_available.json` & `PyPlumIO-0.5.9/tests/testdata/responses/device_available.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/ecomax_parameters.json` & `PyPlumIO-0.5.9/tests/testdata/responses/ecomax_parameters.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/mixer_parameters.json` & `PyPlumIO-0.5.9/tests/testdata/responses/mixer_parameters.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/regulator_data_schema.json` & `PyPlumIO-0.5.9/tests/testdata/responses/regulator_data_schema.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/schedules.json` & `PyPlumIO-0.5.9/tests/testdata/responses/schedules.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7604166666666666%*

 * *Differences: {'0': "{'id': 'EM_heating_and_water_heater_schedule', 'message': {'items': {insert: [(0, "*

 * *      "'100102000005001E0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0'), (1, "*

 * *      "'000FFFFFFFE0000FFFFFFFE010005001E0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0')], "*

 * *      "delete: [0]}}, 'data': {'schedules': {insert: [(1, OrderedDict([('items', [1, [[False, "*

 * *      'False, False, False, False, False, False, False, False, False, False, False, False, False, '*

 * *      'False, False,  […]*

```diff
@@ -23,14 +23,40 @@
                             "__class__": "ParameterValues",
                             "__module__": "pyplumio.helpers.parameter",
                             "max_value": 30,
                             "min_value": 0,
                             "value": 5
                         }
                     ]
+                },
+                {
+                    "__tuple__": true,
+                    "items": [
+                        2,
+                        {
+                            "__class__": "ParameterValues",
+                            "__module__": "pyplumio.helpers.parameter",
+                            "max_value": 1,
+                            "min_value": 0,
+                            "value": 0
+                        }
+                    ]
+                },
+                {
+                    "__tuple__": true,
+                    "items": [
+                        3,
+                        {
+                            "__class__": "ParameterValues",
+                            "__module__": "pyplumio.helpers.parameter",
+                            "max_value": 30,
+                            "min_value": 0,
+                            "value": 5
+                        }
+                    ]
                 }
             ],
             "schedules": [
                 {
                     "__tuple__": true,
                     "items": [
                         0,
@@ -383,20 +409,379 @@
                                 true,
                                 true,
                                 true,
                                 false
                             ]
                         ]
                     ]
+                },
+                {
+                    "__tuple__": true,
+                    "items": [
+                        1,
+                        [
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ],
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ],
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ],
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ],
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ],
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ],
+                            [
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                false,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                true,
+                                false
+                            ]
+                        ]
+                    ]
                 }
             ]
         },
-        "id": "EM_heating_schedule_and_parameter",
+        "id": "EM_heating_and_water_heater_schedule",
         "message": {
             "__bytearray__": true,
             "items": [
-                "100101000005001E0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0",
+                "100102000005001E0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0",
+                "000FFFFFFFE0000FFFFFFFE010005001E0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0000FFFFFFFE0",
                 "000FFFFFFFE0000FFFFFFFE"
             ]
         }
     }
 ]
```

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/thermostat_parameters.json` & `PyPlumIO-0.5.9/tests/testdata/responses/thermostat_parameters.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/responses/uid.json` & `PyPlumIO-0.5.9/tests/testdata/responses/uid.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tests/testdata/unknown/unknown_ecomax_parameter.json` & `PyPlumIO-0.5.9/tests/testdata/unknown/unknown_ecomax_parameter.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.5.8/tox.ini` & `PyPlumIO-0.5.9/tox.ini`

 * *Files identical despite different names*

