# Comparing `tmp/adafruit-circuitpython-azureiot-2.5.9.tar.gz` & `tmp/adafruit_circuitpython_azureiot-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-azureiot-2.5.9.tar", last modified: Tue Aug  9 19:32:49 2022, max compression
+gzip compressed data, was "adafruit_circuitpython_azureiot-2.6.0.tar", last modified: Fri May  3 01:50:47 2024, max compression
```

## Comparing `adafruit-circuitpython-azureiot-2.5.9.tar` & `adafruit_circuitpython_azureiot-2.6.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.985276 adafruit-circuitpython-azureiot-2.5.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.989276 adafruit-circuitpython-azureiot-2.5.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.989276 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16261 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.993276 adafruit-circuitpython-azureiot-2.5.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12524 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11740 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.993276 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/base64.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/device_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)    17792 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/hmac.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    17202 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     8889 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iotcentral_device.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15024 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iothub_device.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:48.997276 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12524 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-09 19:32:48.000000 adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.001276 adafruit-circuitpython-azureiot-2.5.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.001276 adafruit-circuitpython-azureiot-2.5.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5570 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    19120 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-button.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-button.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    74478 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-dialog.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-dialog.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    72070 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device-keys.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device-keys.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    70638 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device.png.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.001276 adafruit-circuitpython-azureiot-2.5.9/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.005276 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_notconnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     5092 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     4707 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_directmethods.py
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5198 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_notconnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_directmethods.py
--rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4076 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_twin_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_secrets_example.py
--rw-r--r--   0 runner    (1001) docker     (121)    19120 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-button.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-button.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    74478 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-dialog.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-dialog.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    72070 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device-keys.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device-keys.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    70638 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device.png
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/iot-hub-device.png.license
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-09 19:32:41.000000 adafruit-circuitpython-azureiot-2.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-08-09 19:32:34.000000 adafruit-circuitpython-azureiot-2.5.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:32:49.009276 adafruit-circuitpython-azureiot-2.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.226134 adafruit_circuitpython_azureiot-2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.214134 adafruit_circuitpython_azureiot-2.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.218134 adafruit_circuitpython_azureiot-2.6.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.218134 adafruit_circuitpython_azureiot-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.218134 adafruit_circuitpython_azureiot-2.6.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-05-03 01:50:47.226134 adafruit_circuitpython_azureiot-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.218134 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/device_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iot_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iot_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iotcentral_device.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15222 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iothub_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.226134 adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-05-03 01:50:47.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-03 01:50:47.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:50:47.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 01:50:47.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 01:50:47.000000 adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.222134 adafruit_circuitpython_azureiot-2.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.222134 adafruit_circuitpython_azureiot-2.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-central-connect-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-central-connect-button.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)    74478 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-central-connect-dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-central-connect-dialog.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)    72070 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-hub-device-keys.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-hub-device-keys.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)    70638 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-hub-device.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/iot-hub-device.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.222134 adafruit_circuitpython_azureiot-2.6.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.226134 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_notconnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_directmethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:50:47.226134 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_notconnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_directmethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_twin_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_secrets_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-central-connect-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-central-connect-button.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)    74478 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-central-connect-dialog.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-central-connect-dialog.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)    72070 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-hub-device-keys.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-hub-device-keys.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)    70638 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-hub-device.png
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/iot-hub-device.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 01:50:44.000000 adafruit_circuitpython_azureiot-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-03 01:50:38.000000 adafruit_circuitpython_azureiot-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:50:47.226134 adafruit_circuitpython_azureiot-2.6.0/setup.cfg
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_azureiot-2.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/.gitignore` & `adafruit_circuitpython_azureiot-2.6.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/.pre-commit-config.yaml` & `adafruit_circuitpython_azureiot-2.6.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/.pylintrc` & `adafruit_circuitpython_azureiot-2.6.0/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,similarities,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -216,25 +216,19 @@
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
-max-line-length=140
+max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -394,19 +357,19 @@
 # List of valid names for the first argument in a metaclass class method.
 valid-metaclass-classmethod-first-arg=mcs
 
 
 [DESIGN]
 
 # Maximum number of arguments for function / method
-max-args=6
+max-args=5
 
 # Maximum number of attributes for a class (see R0902).
 # max-attributes=7
-max-attributes=13
+max-attributes=11
 
 # Maximum number of boolean expressions in a if statement
 max-bool-expr=5
 
 # Maximum number of branch for function / method body
 max-branches=12
 
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_azureiot-2.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/LICENSE` & `adafruit_circuitpython_azureiot-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_azureiot-2.6.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/LICENSES/MIT.txt` & `adafruit_circuitpython_azureiot-2.6.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_azureiot-2.6.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/PKG-INFO` & `adafruit_circuitpython_azureiot-2.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-azureiot
-Version: 2.5.9
+Version: 2.6.0
 Summary: Access to Microsoft Azure IoT from CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT
 Keywords: adafruit,blinka,circuitpython,micropython,azureiot,azure,iot,device,services,,iothub,,iotcentral
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-logging>=4.0.1
+Requires-Dist: adafruit-circuitpython-minimqtt
+Requires-Dist: adafruit-circuitpython-binascii
+Provides-Extra: optional
 
 Adafruit_CircuitPython_AzureIoT
 ================================
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-azureiot/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/azureiot/en/latest/
     :alt: Documentation Status
@@ -62,22 +66,24 @@
     pip3 install adafruit-circuitpython-azureiot
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-* `Adafruit CircuitPython MiniMQTT <https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT>`_
-* `Adafruit CircuitPython Requests <https://github.com/adafruit/Adafruit_CircuitPython_Requests>`_
 * `Adafruit CircuitPython BinASCII <https://github.com/adafruit/Adafruit_CircuitPython_Binascii>`_
+* `Adafruit CircuitPython Logging <https://github.com/adafruit/Adafruit_CircuitPython_Logging>`_
+* `Adafruit CircuitPython MiniMQTT <https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
 
+**Board Compatibility:** The following built-in modules must be available: gc, json, time
+
 Usage Example
 =============
 
 This library supports both `Azure IoT Hub <https://azure.microsoft.com/services/iot-hub/?WT.mc_id=academic-3168-jabenn>`_ and `Azure IoT Central <https://azure.microsoft.com/services/iot-central/?WT.mc_id=academic-3168-jabenn>`__.
 
 To create an Azure IoT Hub instance or an Azure IoT Central app, you will need an Azure subscription. If you don't have an Azure subscription, you can sign up for free:
 
@@ -104,15 +110,15 @@
 
 Native Networking
 =================
 To use this library, with boards that have native networking support, you need to be connected to a network. You will also need to set the current time, as this is used to generate time-based authentication keys. One way to do this is the `Adafruit NTP library <https://github.com/adafruit/Adafruit_CircuitPython_NTP>`_ with the following code:
 
 .. code-block:: python
 
-    pool = socketpool.SocketPool(wifi.radio)
+    pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 
 Azure IoT Hub
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/README.rst` & `adafruit_circuitpython_azureiot-2.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,24 @@
     pip3 install adafruit-circuitpython-azureiot
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-* `Adafruit CircuitPython MiniMQTT <https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT>`_
-* `Adafruit CircuitPython Requests <https://github.com/adafruit/Adafruit_CircuitPython_Requests>`_
 * `Adafruit CircuitPython BinASCII <https://github.com/adafruit/Adafruit_CircuitPython_Binascii>`_
+* `Adafruit CircuitPython Logging <https://github.com/adafruit/Adafruit_CircuitPython_Logging>`_
+* `Adafruit CircuitPython MiniMQTT <https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
 
+**Board Compatibility:** The following built-in modules must be available: gc, json, time
+
 Usage Example
 =============
 
 This library supports both `Azure IoT Hub <https://azure.microsoft.com/services/iot-hub/?WT.mc_id=academic-3168-jabenn>`_ and `Azure IoT Central <https://azure.microsoft.com/services/iot-central/?WT.mc_id=academic-3168-jabenn>`__.
 
 To create an Azure IoT Hub instance or an Azure IoT Central app, you will need an Azure subscription. If you don't have an Azure subscription, you can sign up for free:
 
@@ -86,15 +88,15 @@
 
 Native Networking
 =================
 To use this library, with boards that have native networking support, you need to be connected to a network. You will also need to set the current time, as this is used to generate time-based authentication keys. One way to do this is the `Adafruit NTP library <https://github.com/adafruit/Adafruit_CircuitPython_NTP>`_ with the following code:
 
 .. code-block:: python
 
-    pool = socketpool.SocketPool(wifi.radio)
+    pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 
 Azure IoT Hub
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/__init__.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,26 +17,24 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 **With ESP32 Airlift Networking**
 
-* Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's ESP32SPI library: https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
-* Adafruit's NTP library: https://github.com/adafruit/Adafruit_CircuitPython_NTP
 
 **With Native Networking**
 
-* CircuitPython's Wifi Module: https://docs.circuitpython.org/en/latest/shared-bindings/wifi/index.html
-* Adafruit's Requests Library: https://github.com/adafruit/Adafruit_CircuitPython_Requests/
+* CircuitPython's Wifi Module:
+    https://docs.circuitpython.org/en/latest/shared-bindings/wifi/index.html
 """
 
 from .iot_error import IoTError
 from .iot_mqtt import IoTResponse
 from .iotcentral_device import IoTCentralDevice
 from .iothub_device import IoTHubDevice
 
-__version__ = "2.5.9"
+__version__ = "2.6.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT.git"
 
 __all__ = ["IoTHubDevice", "IoTCentralDevice", "IoTResponse", "IoTError"]
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/base64.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/base64.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/constants.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 #
 # SPDX-License-Identifier: MIT
 
 """
 `constants`
 ================================================================================
 
-This file is for maintaining Microsoft Azure IoT constants that could be changed or added to over time for different scenarios
+This file is for maintaining Microsoft Azure IoT constants that could be changed or added to over
+time for different scenarios
 
 * Author(s): Jim Bennett, Elena Horton
 """
 
 # The version of the IoT Central MQTT API this code is built against
 IOTC_API_VERSION = "2019-10-01"
 
 # The version of the Azure Device Provisioning Service this code is built against
 DPS_API_VERSION = "2019-03-31"
 
-# The Azure Device Provisioning service endpoint that this library uses to provision IoT Central devices
+# The Azure Device Provisioning service endpoint that this library uses to provision IoT Central
+# devices
 DPS_END_POINT = "global.azure-devices-provisioning.net"
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/device_registration.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/device_registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 Handles registration of IoT Central devices, and gets the hostname to use when connecting
 to IoT Central over MQTT
 
 * Author(s): Jim Bennett, Elena Horton
 """
 
 import json
-import ssl
 import time
 
 import adafruit_logging as logging
 from adafruit_logging import Logger
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 
 from . import constants
@@ -41,16 +40,16 @@
     Handles registration of IoT Central devices, and gets the hostname to use when connecting
     to IoT Central over MQTT
     """
 
     # pylint: disable=R0913
     def __init__(
         self,
-        socket,
-        iface,
+        socket_pool,
+        ssl_context,
         id_scope: str,
         device_id: str,
         device_sas_key: str,
         logger: Logger = None,
     ):
         """Creates an instance of the device registration service
 
@@ -70,16 +69,16 @@
             self._logger.addHandler(logging.StreamHandler())
 
         self._mqtt = None
         self._auth_response_received = False
         self._operation_id = None
         self._hostname = None
 
-        self._socket = socket
-        self._iface = iface
+        self._socket_pool = socket_pool
+        self._ssl_context = ssl_context
 
     # pylint: disable=W0613
     # pylint: disable=C0103
     def _on_connect(self, client, userdata, _, rc) -> None:
         self._logger.info(
             f"- device_registration :: _on_connect :: rc = {rc}, userdata = {userdata}"
         )
@@ -108,18 +107,19 @@
 
         self._mqtt.connect()
 
         self._logger.info(
             " - device_registration :: connect :: created mqtt client. connecting.."
         )
         while not self._auth_response_received:
-            self._mqtt.loop()
+            self._mqtt.loop(2)
 
         self._logger.info(
-            f" - device_registration :: connect :: on_connect must be fired. Connected ? {self._mqtt.is_connected()}"
+            " - device_registration :: connect :: on_connect must be fired. Connected ?"
+            f"{self._mqtt.is_connected()}"
         )
 
         if not self._mqtt.is_connected():
             raise DeviceRegistrationError("Cannot connect to MQTT")
 
     def _start_registration(self) -> None:
         self._mqtt.add_topic_callback(
@@ -134,34 +134,35 @@
         )
 
         retry = 0
 
         while self._operation_id is None and retry < 10:
             time.sleep(1)
             retry += 1
-            self._mqtt.loop()
+            self._mqtt.loop(2)
 
         if self._operation_id is None:
             raise DeviceRegistrationError(
                 "Cannot register device - no response from broker for registration result"
             )
 
     def _wait_for_operation(self) -> None:
         message = json.dumps({"operationId": self._operation_id})
         self._mqtt.publish(
-            f"$dps/registrations/GET/iotdps-get-operationstatus/?$rid={self._device_id}&operationId={self._operation_id}",
+            "$dps/registrations/GET/iotdps-get-operationstatus/?$rid="
+            f"{self._device_id}&operationId={self._operation_id}",
             message,
         )
 
         retry = 0
 
         while self._hostname is None and retry < 10:
             time.sleep(1)
             retry += 1
-            self._mqtt.loop()
+            self._mqtt.loop(2)
 
         if self._hostname is None:
             raise DeviceRegistrationError(
                 "Cannot register device - no response from broker for operation status"
             )
 
     def register_device(self, expiry: int) -> str:
@@ -172,34 +173,40 @@
         :param int expiry: The expiry time for the registration
         :returns: The underlying IoT Hub that this device should connect to
         :rtype: str
         :raises DeviceRegistrationError: if the device cannot be registered successfully
         :raises RuntimeError: if the internet connection is not responding or is unable to connect
         """
 
-        username = f"{self._id_scope}/registrations/{self._device_id}/api-version={constants.DPS_API_VERSION}"
+        username = (
+            f"{self._id_scope}/registrations/{self._device_id}/api-version="
+            + f"{constants.DPS_API_VERSION}"
+        )
 
         # pylint: disable=C0103
         sr = self._id_scope + "%2Fregistrations%2F" + self._device_id
         sig_no_encode = compute_derived_symmetric_key(
             self._device_sas_key, sr + "\n" + str(expiry)
         )
         sig_encoded = quote(sig_no_encode, "~()*!.'")
-        auth_string = f"SharedAccessSignature sr={sr}&sig={sig_encoded}&se={expiry}&skn=registration"
-
-        MQTT.set_socket(self._socket, self._iface)
+        auth_string = (
+            f"SharedAccessSignature sr={sr}&sig={sig_encoded}&se={expiry}"
+            "&skn=registration"
+        )
 
         self._mqtt = MQTT.MQTT(
             broker=constants.DPS_END_POINT,
+            port=8883,
             username=username,
             password=auth_string,
-            port=8883,
-            keep_alive=120,
             client_id=self._device_id,
-            ssl_context=ssl.create_default_context(),
+            is_ssl=True,
+            keep_alive=120,
+            socket_pool=self._socket_pool,
+            ssl_context=self._ssl_context,
         )
 
         self._mqtt.enable_logger(logging, self._logger.getEffectiveLevel())
 
         self._connect_to_mqtt()
         self._start_registration()
         self._wait_for_operation()
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/hmac.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/hmac.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Implements the HMAC algorithm as described by RFC 2104.
 
 This is here as code instead of using https://github.com/jimbobbennett/CircuitPython_HMAC.git
 as we only need sha256, so just having the code we need saves 19k of RAM
 
 """
 
-# pylint: disable=C0103, W0108, R0915, C0116, C0115
+# pylint: disable=C0103, W0108, R0915, C0116, C0115, unnecessary-lambda-assignment
 
 try:
     from typing import Union
 except ImportError:
     pass
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_error.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iot_error.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iot_mqtt.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iot_mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 An MQTT client for Azure IoT
 
 * Author(s): Jim Bennett, Elena Horton
 """
 
 import gc
 import json
-import ssl
 import time
 
 import adafruit_minimqtt.adafruit_minimqtt as MQTT
 import adafruit_logging as logging
 from adafruit_logging import Logger
 
 from .iot_error import IoTError
 from .keys import compute_derived_symmetric_key
 from .quote import quote
 from . import constants
 
+
 # pylint: disable=R0903
 class IoTResponse:
     """A response from a direct method call"""
 
     def __init__(self, code: int, message: str):
         """Creates an IoT Response object
 
-        :param int code: The HTTP response code for this method call, for example 200 if the method was handled successfully
+        :param int code: The HTTP response code for this method call, for example 200 if the method
+            was handled successfully
         :param str message: The HTTP response message for this method call
         """
         self.response_code = code
         self.response_message = message
 
 
 class IoTMQTTCallback:
@@ -114,32 +115,35 @@
         ):  # somewhere along the crypto chain a newline is inserted
             signature = signature[:-1]
         return "SharedAccessSignature sr={}&sig={}&se={}".format(
             uri, signature, token_expiry
         )
 
     def _create_mqtt_client(self) -> None:
-        MQTT.set_socket(self._socket, self._iface)
-
+        log_text = (
+            f"- iot_mqtt :: _on_connect :: username = {self._username}, password = "
+            + f"{self._passwd}"
+        )
         self._logger.debug(
-            str.replace(
-                f"- iot_mqtt :: _on_connect :: username = {self._username}, password = {self._passwd}",
+            log_text.replace(
                 "%",
                 "%%",
             )
         )
 
         self._mqtts = MQTT.MQTT(
             broker=self._hostname,
+            port=8883,
             username=self._username,
             password=self._passwd,
-            port=8883,
-            keep_alive=120,
             client_id=self._device_id,
-            ssl_context=ssl.create_default_context(),
+            is_ssl=True,
+            keep_alive=120,
+            socket_pool=self._socket_pool,
+            ssl_context=self._ssl_context,
         )
 
         self._mqtts.enable_logger(logging, self._logger.getEffectiveLevel())
 
         # set actions to take throughout connection lifecycle
         self._mqtts.on_connect = self._on_connect
         self._mqtts.on_publish = self._on_publish
@@ -317,36 +321,37 @@
         self.loop()
         self._send_common("$iothub/twin/GET/?$rid=0", " ")
 
     # pylint: disable=R0913
     def __init__(
         self,
         callback: IoTMQTTCallback,
-        socket,
-        iface,
+        socket_pool,
+        ssl_context,
         hostname: str,
         device_id: str,
         device_sas_key: str,
         token_expires: int = 21600,
         logger: Logger = None,
     ):
         """Create the Azure IoT MQTT client
 
         :param IoTMQTTCallback callback: A callback class
         :param socket: The socket to communicate over
         :param iface: The network interface to communicate over
-        :param str hostname: The hostname of the MQTT broker to connect to, get this by registering the device
+        :param str hostname: The hostname of the MQTT broker to connect to, get this by registering
+            the device
         :param str device_id: The device ID of the device to register
         :param str device_sas_key: The primary or secondary key of the device to register
         :param int token_expires: The number of seconds till the token expires, defaults to 6 hours
         :param Logger logger: The logger
         """
         self._callback = callback
-        self._socket = socket
-        self._iface = iface
+        self._socket_pool = socket_pool
+        self._ssl_context = ssl_context
         self._auth_response_received = False
         self._mqtts = None
         self._device_id = device_id
         self._hostname = hostname
         self._device_sas_key = device_sas_key
         self._token_expires = token_expires
         self._username = "{}/{}/?api-version={}".format(
@@ -447,15 +452,15 @@
         return self._mqtts.is_connected()
 
     def loop(self) -> None:
         """Listens for MQTT messages"""
         if not self.is_connected():
             return
 
-        self._mqtts.loop()
+        self._mqtts.loop(2)
         gc.collect()
 
     def send_device_to_cloud_message(
         self, message, system_properties: dict = None
     ) -> None:
         """Send a device to cloud message from this device to Azure IoT Hub
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iotcentral_device.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iotcentral_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import adafruit_logging as logging
 from adafruit_logging import Logger
 from .device_registration import DeviceRegistration
 from .iot_error import IoTError
 from .iot_mqtt import IoTMQTT, IoTMQTTCallback, IoTResponse
 
 
-class IoTCentralDevice(IoTMQTTCallback):
+class IoTCentralDevice(IoTMQTTCallback):  # pylint: disable=too-many-instance-attributes
     """A device client for the Azure IoT Central service"""
 
     def connection_status_change(self, connected: bool) -> None:
         """Called when the connection status changes
 
         :param bool connected: True if the device is connected, otherwise false
         """
@@ -116,31 +116,35 @@
         else:
             self._logger = logging.getLogger("log")
             self._logger.addHandler(logging.StreamHandler())
         self._device_registration = None
         self._mqtt = None
 
         self.on_connection_status_changed = None
-        """A callback method that is called when the connection status is changed. This method should have the following signature:
+        """A callback method that is called when the connection status is changed.
+        This method should have the following signature:
         def connection_status_changed(connected: bool) -> None
         """
 
         self.on_command_executed = None
-        """A callback method that is called when a command is executed on the device. This method should have the following signature:
+        """A callback method that is called when a command is executed on the device.
+        This method should have the following signature:
         def connection_status_changed(method_name: str, payload: str) -> IoTResponse:
 
-        This method returns an IoTResponse containing a status code and message from the command call. Set this appropriately
-        depending on if the command was successfully handled or not. For example, if the command was handled successfully, set
-        the code to 200 and message to "OK":
+        This method returns an IoTResponse containing a status code and message from the command
+        call. Set this appropriately depending on if the command was successfully handled or not.
+        For example, if the command was handled successfully, set the code to 200 and message to
+        "OK":
 
         return IoTResponse(200, "OK")
         """
 
         self.on_property_changed = None
-        """A callback method that is called when property values are updated. This method should have the following signature:
+        """A callback method that is called when property values are updated.
+        This method should have the following signature:
         def property_changed(_property_name: str, property_value, version: int) -> None
         """
 
     def connect(self) -> None:
         """Connects to Azure IoT Central
 
         :raises DeviceRegistrationError: if the device cannot be registered successfully
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/iothub_device.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/iothub_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     SHARED_ACCESS_SIGNATURE,
     DEVICE_ID,
     MODULE_ID,
     GATEWAY_HOST_NAME,
 ]
 
 
-class IoTHubDevice(IoTMQTTCallback):
+class IoTHubDevice(IoTMQTTCallback):  # pylint: disable=too-many-instance-attributes
     """A device client for the Azure IoT Hub service"""
 
     def connection_status_change(self, connected: bool) -> None:
         """Called when the connection status changes
 
         :param bool connected: True if the device is connected, otherwise false
         """
@@ -131,15 +131,15 @@
         """
         if self._on_device_twin_reported_updated is not None:
             # pylint: disable=E1102
             self._on_device_twin_reported_updated(
                 reported_property_name, reported_property_value, reported_version
             )
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         socket,
         iface,
         device_connection_string: str,
         token_expires: int = 21600,
         logger: Logger = None,
     ):
@@ -164,15 +164,16 @@
         try:
             cs_args = device_connection_string.split(DELIMITER)
             connection_string_values = dict(
                 arg.split(VALUE_SEPARATOR, 1) for arg in cs_args
             )
         except (ValueError, AttributeError) as e:
             raise ValueError(
-                "Connection string is required and should not be empty or blank and must be supplied as a string"
+                "Connection string is required and should not be empty or blank and must be"
+                "supplied as a string"
             ) from e
 
         if len(cs_args) != len(connection_string_values):
             raise ValueError("Invalid Connection String - Unable to parse")
 
         _validate_keys(connection_string_values)
 
@@ -190,108 +191,120 @@
         self._on_device_twin_desired_updated = None
         self._on_device_twin_reported_updated = None
 
         self._mqtt = None
 
     @property
     def on_connection_status_changed(self) -> Callable:
-        """A callback method that is called when the connection status is changed. This method should have the following signature:
+        """A callback method that is called when the connection status is changed.
+        This method should have the following signature:
         def connection_status_changed(connected: bool) -> None
         """
         return self._on_connection_status_changed
 
     @on_connection_status_changed.setter
     def on_connection_status_changed(
         self, new_on_connection_status_changed: Callable
     ) -> None:
-        """A callback method that is called when the connection status is changed. This method should have the following signature:
+        """A callback method that is called when the connection status is changed.
+        This method should have the following signature:
         def connection_status_changed(connected: bool) -> None
         """
         self._on_connection_status_changed = new_on_connection_status_changed
 
     @property
     def on_direct_method_invoked(self) -> Callable:
-        """A callback method that is called when a direct method is invoked.  This method should have the following signature:
+        """A callback method that is called when a direct method is invoked.
+        This method should have the following signature:
         def direct_method_invoked(method_name: str, payload: str) -> IoTResponse:
 
-        This method returns an IoTResponse containing a status code and message from the method invocation. Set this appropriately
-        depending on if the method was successfully handled or not. For example, if the method was handled successfully, set
-        the code to 200 and message to "OK":
+        This method returns an IoTResponse containing a status code and message from the method
+        invocation. Set this appropriately depending on if the method was successfully handled or
+        not. For example, if the method was handled successfully, set the code to 200 and message
+        to "OK":
 
         return IoTResponse(200, "OK")
         """
         return self._on_direct_method_invoked
 
     @on_direct_method_invoked.setter
     def on_direct_method_invoked(self, new_on_direct_method_invoked: Callable) -> None:
-        """A callback method that is called when a direct method is invoked.  This method should have the following signature:
+        """A callback method that is called when a direct method is invoked.
+        This method should have the following signature:
         def direct_method_invoked(method_name: str, payload: str) -> IoTResponse:
 
-        This method returns an IoTResponse containing a status code and message from the method invocation. Set this appropriately
-        depending on if the method was successfully handled or not. For example, if the method was handled successfully, set
-        the code to 200 and message to "OK":
+        This method returns an IoTResponse containing a status code and message from the method
+        invocation. Set this appropriately depending on if the method was successfully handled or
+        not. For example, if the method was handled successfully, set the code to 200 and message
+        to "OK":
 
         return IoTResponse(200, "OK")
         """
         self._on_direct_method_invoked = new_on_direct_method_invoked
 
     @property
     def on_cloud_to_device_message_received(self) -> Callable:
-        """A callback method that is called when a cloud to device message is received. This method should have the following signature:
+        """A callback method that is called when a cloud to device message is received.
+        This method should have the following signature:
         def cloud_to_device_message_received(body: str, properties: dict) -> None:
         """
         return self._on_cloud_to_device_message_received
 
     @on_cloud_to_device_message_received.setter
     def on_cloud_to_device_message_received(
         self, new_on_cloud_to_device_message_received: Callable
     ) -> None:
-        """A callback method that is called when a cloud to device message is received. This method should have the following signature:
+        """A callback method that is called when a cloud to device message is received.
+        This method should have the following signature:
         def cloud_to_device_message_received(body: str, properties: dict) -> None:
         """
         self._on_cloud_to_device_message_received = (
             new_on_cloud_to_device_message_received
         )
 
     @property
     def on_device_twin_desired_updated(self) -> Callable:
-        """A callback method that is called when the desired properties of the devices device twin are updated.
-        This method should have the following signature:
-        def device_twin_desired_updated(desired_property_name: str, desired_property_value, desired_version: int) -> None:
+        """A callback method that is called when the desired properties of the devices device twin
+        are updated. This method should have the following signature:
+        def device_twin_desired_updated(desired_property_name: str, desired_property_value,
+        desired_version: int) -> None:
         """
         return self._on_device_twin_desired_updated
 
     @on_device_twin_desired_updated.setter
     def on_device_twin_desired_updated(
         self, new_on_device_twin_desired_updated: Callable
     ) -> None:
-        """A callback method that is called when the desired properties of the devices device twin are updated.
-        This method should have the following signature:
-        def device_twin_desired_updated(desired_property_name: str, desired_property_value, desired_version: int) -> None:
+        """A callback method that is called when the desired properties of the devices device twin
+        are updated. This method should have the following signature:
+        def device_twin_desired_updated(desired_property_name: str, desired_property_value,
+        desired_version: int) -> None:
         """
         self._on_device_twin_desired_updated = new_on_device_twin_desired_updated
 
         if self._mqtt is not None:
             self._mqtt.subscribe_to_twins()
 
     @property
     def on_device_twin_reported_updated(self) -> Callable:
-        """A callback method that is called when the reported properties of the devices device twin are updated.
-        This method should have the following signature:
-        def device_twin_reported_updated(reported_property_name: str, reported_property_value, reported_version: int) -> None:
+        """A callback method that is called when the reported properties of the devices device twin
+        are updated. This method should have the following signature:
+        def device_twin_reported_updated(reported_property_name: str, reported_property_value,
+        reported_version: int) -> None:
         """
         return self._on_device_twin_reported_updated
 
     @on_device_twin_reported_updated.setter
     def on_device_twin_reported_updated(
         self, new_on_device_twin_reported_updated: Callable
     ) -> None:
-        """A callback method that is called when the reported properties of the devices device twin are updated.
-        This method should have the following signature:
-        def device_twin_reported_updated(reported_property_name: str, reported_property_value, reported_version: int) -> None:
+        """A callback method that is called when the reported properties of the devices device twin
+        are updated. This method should have the following signature:
+        def device_twin_reported_updated(reported_property_name: str, reported_property_value,
+        reported_version: int) -> None:
         """
         self._on_device_twin_reported_updated = new_on_device_twin_reported_updated
 
         if self._mqtt is not None:
             self._mqtt.subscribe_to_twins()
 
     def connect(self) -> None:
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/keys.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/keys.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_azureiot/quote.py` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_azureiot/quote.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/PKG-INFO` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-azureiot
-Version: 2.5.9
+Version: 2.6.0
 Summary: Access to Microsoft Azure IoT from CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT
 Keywords: adafruit,blinka,circuitpython,micropython,azureiot,azure,iot,device,services,,iothub,,iotcentral
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-logging>=4.0.1
+Requires-Dist: adafruit-circuitpython-minimqtt
+Requires-Dist: adafruit-circuitpython-binascii
+Provides-Extra: optional
 
 Adafruit_CircuitPython_AzureIoT
 ================================
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-azureiot/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/azureiot/en/latest/
     :alt: Documentation Status
@@ -62,22 +66,24 @@
     pip3 install adafruit-circuitpython-azureiot
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-* `Adafruit CircuitPython MiniMQTT <https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT>`_
-* `Adafruit CircuitPython Requests <https://github.com/adafruit/Adafruit_CircuitPython_Requests>`_
 * `Adafruit CircuitPython BinASCII <https://github.com/adafruit/Adafruit_CircuitPython_Binascii>`_
+* `Adafruit CircuitPython Logging <https://github.com/adafruit/Adafruit_CircuitPython_Logging>`_
+* `Adafruit CircuitPython MiniMQTT <https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
 
+**Board Compatibility:** The following built-in modules must be available: gc, json, time
+
 Usage Example
 =============
 
 This library supports both `Azure IoT Hub <https://azure.microsoft.com/services/iot-hub/?WT.mc_id=academic-3168-jabenn>`_ and `Azure IoT Central <https://azure.microsoft.com/services/iot-central/?WT.mc_id=academic-3168-jabenn>`__.
 
 To create an Azure IoT Hub instance or an Azure IoT Central app, you will need an Azure subscription. If you don't have an Azure subscription, you can sign up for free:
 
@@ -104,15 +110,15 @@
 
 Native Networking
 =================
 To use this library, with boards that have native networking support, you need to be connected to a network. You will also need to set the current time, as this is used to generate time-based authentication keys. One way to do this is the `Adafruit NTP library <https://github.com/adafruit/Adafruit_CircuitPython_NTP>`_ with the following code:
 
 .. code-block:: python
 
-    pool = socketpool.SocketPool(wifi.radio)
+    pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 
 Azure IoT Hub
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt` & `adafruit_circuitpython_azureiot-2.6.0/adafruit_circuitpython_azureiot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 iot-hub-device.png.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_azureiot/__init__.py
 adafruit_azureiot/base64.py
 adafruit_azureiot/constants.py
 adafruit_azureiot/device_registration.py
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/_static/favicon.ico` & `adafruit_circuitpython_azureiot-2.6.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/conf.py` & `adafruit_circuitpython_azureiot-2.6.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
@@ -44,15 +46,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit AzureIoT Library"
-copyright = "2019 Brent Rubell, Jim Bennett, Elena Horton"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Brent Rubell, Jim Bennett, Elena Horton"
 author = "Brent Rubell, Jim Bennett, Elena Horton"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -93,27 +102,18 @@
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import sphinx_rtd_theme
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme = "sphinx_rtd_theme"
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to use as a favicon of
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/examples.rst` & `adafruit_circuitpython_azureiot-2.6.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/index.rst` & `adafruit_circuitpython_azureiot-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-button.png` & `adafruit_circuitpython_azureiot-2.6.0/docs/iot-central-connect-button.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/iot-central-connect-dialog.png` & `adafruit_circuitpython_azureiot-2.6.0/docs/iot-central-connect-dialog.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device-keys.png` & `adafruit_circuitpython_azureiot-2.6.0/docs/iot-hub-device-keys.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/docs/iot-hub-device.png` & `adafruit_circuitpython_azureiot-2.6.0/docs/iot-hub-device.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_commands.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -75,41 +75,49 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 # pylint: disable=wrong-import-position
 from adafruit_azureiot import IoTCentralDevice
 from adafruit_azureiot.iot_mqtt import IoTResponse
 
 # pylint: enable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
 device = IoTCentralDevice(
-    socket, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
+
 # Subscribe to commands
 # Commands can be sent from the devices Dashboard in IoT Central, assuming
 # the device template and view has been set up with the commands
 # Command handlers need to return a response to show if the command was handled
 # successfully or not, returning an HTTP status code and message
 def command_executed(command_name: str, payload) -> IoTResponse:
     print("Command", command_name, "executed with payload", str(payload))
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_notconnected.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_notconnected.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -69,41 +69,48 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 # pylint: disable=wrong-import-position
 from adafruit_azureiot import (
     IoTCentralDevice,
     IoTError,
 )
 
 # pylint: enable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
 device = IoTCentralDevice(
-    socket, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
 # don't connect
 # device.connect()
 
 try:
     message = {"Temperature": random.randint(0, 50)}
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_properties.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -76,37 +76,45 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 from adafruit_azureiot import IoTCentralDevice  # pylint: disable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
 device = IoTCentralDevice(
-    socket, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
+
 # Subscribe to property changes
 # Properties can be updated either in code, or by adding a form to the view
 # in the device template, and setting the value on the dashboard for the device
 def property_changed(property_name, property_value, version):
     print(
         "Property",
         property_name,
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_central_simpletest.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_central_simpletest.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -77,35 +77,42 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 from adafruit_azureiot import IoTCentralDevice  # pylint: disable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
 device = IoTCentralDevice(
-    socket, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
 print("Connecting to Azure IoT Central...")
 
 # Connect to IoT Central
 device.connect()
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_directmethods.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_directmethods.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -72,36 +72,39 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 # pylint: disable=wrong-import-position
 from adafruit_azureiot import IoTHubDevice
 from adafruit_azureiot.iot_mqtt import IoTResponse
 
 # pylint: enable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(socket, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
+
 
 # Subscribe to direct method calls
 # To invoke a method on the device, select it in the Azure Portal, select Direct Method,
 # fill in the method name and payload, then select Invoke Method
 # Direct method handlers need to return a response to show if the method was handled
 # successfully or not, returning an HTTP status code and message
 def direct_method_invoked(method_name: str, payload) -> IoTResponse:
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_messages.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_simpletest.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -74,42 +74,34 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 from adafruit_azureiot import IoTHubDevice  # pylint: disable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(socket, esp, secrets["device_connection_string"])
-
-# Subscribe to cloud to device messages
-# To send a message to the device, select it in the Azure Portal, select Message To Device,
-# fill in the message and any properties you want to add, then select Send Message
-def cloud_to_device_message_received(body: str, properties: dict):
-    print("Received message with body", body, "and properties", json.dumps(properties))
-
-
-# Subscribe to the cloud to device message received events
-device.on_cloud_to_device_message_received = cloud_to_device_message_received
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
 
 print("Connecting to Azure IoT Hub...")
 
 # Connect to IoT Central
 device.connect()
 
 print("Connected to Azure IoT Hub!")
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_simpletest.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_messages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,88 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import json
 import random
 import time
-import board
-import busio
-from digitalio import DigitalInOut
-import neopixel
+
 import rtc
-from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import wifi
+
+import adafruit_connection_manager
+import adafruit_ntp
+from adafruit_azureiot import IoTHubDevice
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
-# ESP32 Setup
-try:
-    esp32_cs = DigitalInOut(board.ESP_CS)
-    esp32_ready = DigitalInOut(board.ESP_BUSY)
-    esp32_reset = DigitalInOut(board.ESP_RESET)
-except AttributeError:
-    esp32_cs = DigitalInOut(board.D13)
-    esp32_ready = DigitalInOut(board.D11)
-    esp32_reset = DigitalInOut(board.D12)
-
-spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
-esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
-
-"""Use below for Most Boards"""
-status_light = neopixel.NeoPixel(
-    board.NEOPIXEL, 1, brightness=0.2
-)  # Uncomment for Most Boards
-"""Uncomment below for ItsyBitsy M4"""
-# status_light = dotstar.DotStar(board.APA102_SCK, board.APA102_MOSI, 1, brightness=0.2)
-# Uncomment below for an externally defined RGB LED
-# import adafruit_rgbled
-# from adafruit_esp32spi import PWMOut
-# RED_LED = PWMOut.PWMOut(esp, 26)
-# GREEN_LED = PWMOut.PWMOut(esp, 27)
-# BLUE_LED = PWMOut.PWMOut(esp, 25)
-# status_light = adafruit_rgbled.RGBLED(RED_LED, BLUE_LED, GREEN_LED)
-wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
-
 print("Connecting to WiFi...")
+wifi.radio.connect(secrets["ssid"], secrets["password"])
 
-wifi.connect()
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
 
 print("Connected to WiFi!")
 
-print("Getting the time...")
-
-# get_time will raise ValueError if the time isn't available yet so loop until
-# it works.
-now_utc = None
-while now_utc is None:
-    try:
-        now_utc = time.localtime(esp.get_time()[0])
-    except ValueError:
-        pass
-rtc.RTC().datetime = now_utc
-
-print("Time:", str(time.time()))
+if time.localtime().tm_year < 2022:
+    print("Setting System Time in UTC")
+    ntp = adafruit_ntp.NTP(pool, tz_offset=0)
+
+    # NOTE: This changes the system time so make sure you aren't assuming that time
+    # doesn't jump.
+    rtc.RTC().datetime = ntp.datetime
+else:
+    print("Year seems good, skipping set time.")
 
 # You will need an Azure subscription to create an Azure IoT Hub resource
 #
 # If you don't have an Azure subscription:
 #
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
-from adafruit_azureiot import IoTHubDevice  # pylint: disable=wrong-import-position
+
 
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(socket, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
 
-print("Connecting to Azure IoT Hub...")
 
-# Connect to IoT Central
+# Subscribe to cloud to device messages
+# To send a message to the device, select it in the Azure Portal, select Message To Device,
+# fill in the message and any properties you want to add, then select Send Message
+def cloud_to_device_message_received(body: str, properties: dict):
+    print("Received message with body", body, "and properties", json.dumps(properties))
+
+
+# Subscribe to the cloud to device message received events
+device.on_cloud_to_device_message_received = cloud_to_device_message_received
+
+print("Connecting to Azure IoT Hub...")
 device.connect()
 
 print("Connected to Azure IoT Hub!")
 
 message_counter = 60
 
 while True:
@@ -118,12 +97,14 @@
         else:
             message_counter += 1
 
         # Poll every second for messages from the cloud
         device.loop()
     except (ValueError, RuntimeError) as e:
         print("Connection error, reconnecting\n", str(e))
-        wifi.reset()
-        wifi.connect()
+        # If we lose connectivity, reset the wifi and reconnect
+        wifi.radio.enabled = False
+        wifi.radio.enabled = True
+        wifi.radio.connect(secrets["ssid"], secrets["password"])
         device.reconnect()
         continue
     time.sleep(1)
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_twin_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import board
 import busio
 from digitalio import DigitalInOut
 import neopixel
 import rtc
 from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
-import adafruit_esp32spi.adafruit_esp32spi_socket as socket
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
@@ -73,35 +73,38 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # To us twins, you will need either a free or standard tier IoT Hub. Basic tier doesn't
 # support twins
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 from adafruit_azureiot import IoTHubDevice  # pylint: disable=wrong-import-position
 
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(socket, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
+
 
 # Subscribe to device twin desired property updates
 # To see these changes, update the desired properties for the device either in code
 # or in the Azure portal by selecting the device in the IoT Hub blade, selecting
 # Device Twin then adding or amending an entry in the 'desired' section
 def device_twin_desired_updated(
     desired_property_name: str, desired_property_value, desired_version: int
@@ -128,16 +131,16 @@
 
 message_counter = 60
 
 while True:
     try:
         if message_counter >= 60:
             # Send a reported property twin update every minute
-            # You can see these in the portal by selecting the device in the IoT Hub blade, selecting
-            # Device Twin then looking for the updates in the 'reported' section
+            # You can see these in the portal by selecting the device in the IoT Hub blade,
+            # selecting device Twin then looking for the updates in the 'reported' section
             patch = {"Temperature": random.randint(0, 50)}
             device.update_twin(patch)
             message_counter = 0
         else:
             message_counter += 1
 
         # Poll every second for messages from the cloud
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_commands.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import time
 
 import rtc
-import socketpool
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import IoTCentralDevice
 from adafruit_azureiot.iot_mqtt import IoTResponse
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -44,39 +46,43 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
 # Create an IoT Hub device client and connect
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 device = IoTCentralDevice(
-    pool, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
+
 # Subscribe to commands
 # Commands can be sent from the devices Dashboard in IoT Central, assuming
 # the device template and view has been set up with the commands
 # Command handlers need to return a response to show if the command was handled
 # successfully or not, returning an HTTP status code and message
 def command_executed(command_name: str, payload) -> IoTResponse:
     print("Command", command_name, "executed with payload", str(payload))
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_notconnected.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_notconnected.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # SPDX-License-Identifier: MIT
 
 import json
 import random
 import time
 
 import rtc
-import socketpool
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import (
     IoTCentralDevice,
     IoTError,
 )
 
 # Get wifi details and more from a secrets.py file
@@ -21,19 +21,21 @@
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -48,37 +50,40 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
 # Create an IoT Hub device client and connect
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 device = IoTCentralDevice(
-    pool, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
 # don't connect
 # device.connect()
 
 try:
     message = {"Temperature": random.randint(0, 50)}
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_properties.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import random
 import time
 
 import rtc
-import socketpool
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import IoTCentralDevice
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -44,39 +46,43 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
 # Create an IoT Hub device client and connect
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 device = IoTCentralDevice(
-    pool, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
+
 # Subscribe to property changes
 # Properties can be updated either in code, or by adding a form to the view
 # in the device template, and setting the value on the dashboard for the device
 def property_changed(property_name, property_value, version):
     print(
         "Property",
         property_name,
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_central_simpletest.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_central_simpletest.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 # SPDX-License-Identifier: MIT
 
 import json
 import random
 import time
 
 import rtc
-import socketpool
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import IoTCentralDevice
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -45,37 +47,40 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Central app by following these instructions: https://aka.ms/CreateIoTCentralApp
+# Create an Azure IoT Central app by following these instructions:
+# https://aka.ms/CreateIoTCentralApp
 # Add a device template with telemetry, properties and commands, as well as a view to visualize the
 # telemetry and execute commands, and a form to set properties.
 #
-# Next create a device using the device template, and select Connect to get the device connection details.
+# Next create a device using the device template, and select Connect to get the device connection
+# details.
 # Add the connection details to your secrets.py file, using the following values:
 #
 # 'id_scope' - the devices ID scope
 # 'device_id' - the devices device id
 # 'device_sas_key' - the devices primary key
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
 # Create an IoT Hub device client and connect
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 device = IoTCentralDevice(
-    pool, esp, secrets["id_scope"], secrets["device_id"], secrets["device_sas_key"]
+    pool,
+    ssl_context,
+    secrets["id_scope"],
+    secrets["device_id"],
+    secrets["device_sas_key"],
 )
 
 print("Connecting to Azure IoT Central...")
 device.connect()
 
 print("Connected to Azure IoT Central!")
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_directmethods.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_directmethods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import time
 
-import socketpool
 import rtc
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import IoTHubDevice
 from adafruit_azureiot.iot_mqtt import IoTResponse
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -41,34 +43,33 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(pool, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
+
 
 # Subscribe to direct method calls
 # To invoke a method on the device, select it in the Azure Portal, select Direct Method,
 # fill in the method name and payload, then select Invoke Method
 # Direct method handlers need to return a response to show if the method was handled
 # successfully or not, returning an HTTP status code and message
 def direct_method_invoked(method_name: str, payload) -> IoTResponse:
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_messages.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_twin_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-import json
 import random
 import time
 
-import socketpool
 import rtc
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import IoTHubDevice
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -42,60 +43,69 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(pool, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
+
 
-# Subscribe to cloud to device messages
-# To send a message to the device, select it in the Azure Portal, select Message To Device,
-# fill in the message and any properties you want to add, then select Send Message
-def cloud_to_device_message_received(body: str, properties: dict):
-    print("Received message with body", body, "and properties", json.dumps(properties))
+# Subscribe to device twin desired property updates
+# To see these changes, update the desired properties for the device either in code
+# or in the Azure portal by selecting the device in the IoT Hub blade, selecting
+# Device Twin then adding or amending an entry in the 'desired' section
+def device_twin_desired_updated(
+    desired_property_name: str, desired_property_value, desired_version: int
+):
+    print(
+        "Property",
+        desired_property_name,
+        "updated to",
+        str(desired_property_value),
+        "version",
+        desired_version,
+    )
 
 
-# Subscribe to the cloud to device message received events
-device.on_cloud_to_device_message_received = cloud_to_device_message_received
+# Subscribe to the device twin desired property updated event
+device.on_device_twin_desired_updated = device_twin_desired_updated
 
 print("Connecting to Azure IoT Hub...")
 device.connect()
 
 print("Connected to Azure IoT Hub!")
 
 message_counter = 60
 
 while True:
     try:
-        # Send a device to cloud message every minute
-        # You can see the overview of messages sent from the device in the Overview tab
-        # of the IoT Hub in the Azure Portal
         if message_counter >= 60:
-            message = {"Temperature": random.randint(0, 50)}
-            device.send_device_to_cloud_message(json.dumps(message))
+            # Send a reported property twin update every minute
+            # You can see these in the portal by selecting the device in the IoT Hub blade,
+            # selecting device Twin then looking for the updates in the 'reported' section
+            patch = {"Temperature": random.randint(0, 50)}
+            device.update_twin(patch)
             message_counter = 0
         else:
             message_counter += 1
 
         # Poll every second for messages from the cloud
         device.loop()
     except (ValueError, RuntimeError) as e:
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_simpletest.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_native_networking/azureiot_hub_simpletest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import json
 import random
 import time
 
-import socketpool
 import rtc
 import wifi
 
+import adafruit_connection_manager
 import adafruit_ntp
 from adafruit_azureiot import IoTHubDevice
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
 print("Connecting to WiFi...")
 wifi.radio.connect(secrets["ssid"], secrets["password"])
 
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+
 print("Connected to WiFi!")
 
 if time.localtime().tm_year < 2022:
     print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     # NOTE: This changes the system time so make sure you aren't assuming that time
     # doesn't jump.
     rtc.RTC().datetime = ntp.datetime
 else:
     print("Year seems good, skipping set time.")
@@ -42,34 +44,32 @@
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
 
 
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(pool, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
 
 print("Connecting to Azure IoT Hub...")
 
 # Connect to IoT Central
 device.connect()
 
 print("Connected to Azure IoT Hub!")
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_native_networking/azureiot_hub_twin_operations.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_esp32spi/azureiot_hub_messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,142 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
+import json
 import random
 import time
-
-import socketpool
+import board
+import busio
+from digitalio import DigitalInOut
+import neopixel
 import rtc
-import wifi
-
-import adafruit_ntp
-from adafruit_azureiot import IoTHubDevice
+from adafruit_esp32spi import adafruit_esp32spi, adafruit_esp32spi_wifimanager
+import adafruit_connection_manager
 
 # Get wifi details and more from a secrets.py file
 try:
     from secrets import secrets
 except ImportError:
     print("WiFi secrets are kept in secrets.py, please add them there!")
     raise
 
+# ESP32 Setup
+try:
+    esp32_cs = DigitalInOut(board.ESP_CS)
+    esp32_ready = DigitalInOut(board.ESP_BUSY)
+    esp32_reset = DigitalInOut(board.ESP_RESET)
+except AttributeError:
+    esp32_cs = DigitalInOut(board.D13)
+    esp32_ready = DigitalInOut(board.D11)
+    esp32_reset = DigitalInOut(board.D12)
+
+spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
+esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
+
+"""Use below for Most Boards"""
+status_light = neopixel.NeoPixel(
+    board.NEOPIXEL, 1, brightness=0.2
+)  # Uncomment for Most Boards
+"""Uncomment below for ItsyBitsy M4"""
+# status_light = dotstar.DotStar(board.APA102_SCK, board.APA102_MOSI, 1, brightness=0.2)
+# Uncomment below for an externally defined RGB LED
+# import adafruit_rgbled
+# from adafruit_esp32spi import PWMOut
+# RED_LED = PWMOut.PWMOut(esp, 26)
+# GREEN_LED = PWMOut.PWMOut(esp, 27)
+# BLUE_LED = PWMOut.PWMOut(esp, 25)
+# status_light = adafruit_rgbled.RGBLED(RED_LED, BLUE_LED, GREEN_LED)
+wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
+
 print("Connecting to WiFi...")
-wifi.radio.connect(secrets["ssid"], secrets["password"])
+
+wifi.connect()
 
 print("Connected to WiFi!")
 
-if time.localtime().tm_year < 2022:
-    print("Setting System Time in UTC")
-    pool = socketpool.SocketPool(wifi.radio)
-    ntp = adafruit_ntp.NTP(pool, tz_offset=0)
-
-    # NOTE: This changes the system time so make sure you aren't assuming that time
-    # doesn't jump.
-    rtc.RTC().datetime = ntp.datetime
-else:
-    print("Year seems good, skipping set time.")
+print("Getting the time...")
+
+# get_time will raise ValueError if the time isn't available yet so loop until
+# it works.
+now_utc = None
+while now_utc is None:
+    try:
+        now_utc = time.localtime(esp.get_time()[0])
+    except ValueError:
+        pass
+rtc.RTC().datetime = now_utc
+
+print("Time:", str(time.time()))
 
 # You will need an Azure subscription to create an Azure IoT Hub resource
 #
 # If you don't have an Azure subscription:
 #
 # If you are a student, head to https://aka.ms/FreeStudentAzure and sign up, validating with your
 #  student email address. This will give you $100 of Azure credit and free tiers of a load of
 #  service, renewable each year you are a student
 #
 # If you are not a student, head to https://aka.ms/FreeAz and sign up to get $200 of credit for 30
 #  days, as well as free tiers of a load of services
 #
-# Create an Azure IoT Hub and an IoT device in the Azure portal here: https://aka.ms/AzurePortalHome.
+# Create an Azure IoT Hub and an IoT device in the Azure portal here:
+# https://aka.ms/AzurePortalHome.
 # Instructions to create an IoT Hub and device are here: https://aka.ms/CreateIoTHub
 #
 # The free tier of IoT Hub allows up to 8,000 messages a day, so try not to send messages too often
 # if you are using the free tier
 #
 # Once you have a hub and a device, copy the device primary connection string.
 # Add it to the secrets.py file in an entry called device_connection_string
 #
 # The adafruit-circuitpython-azureiot library depends on the following libraries:
 #
-# From the Adafruit CircuitPython Bundle (https://github.com/adafruit/Adafruit_CircuitPython_Bundle):
+# From the Adafruit CircuitPython Bundle https://github.com/adafruit/Adafruit_CircuitPython_Bundle:
 # * adafruit-circuitpython-minimqtt
-# * adafruit-circuitpython-requests
-
+from adafruit_azureiot import IoTHubDevice  # pylint: disable=wrong-import-position
 
-esp = None
-pool = socketpool.SocketPool(wifi.radio)
+pool = adafruit_connection_manager.get_radio_socketpool(esp)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(esp)
 # Create an IoT Hub device client and connect
-device = IoTHubDevice(pool, esp, secrets["device_connection_string"])
+device = IoTHubDevice(pool, ssl_context, secrets["device_connection_string"])
 
-# Subscribe to device twin desired property updates
-# To see these changes, update the desired properties for the device either in code
-# or in the Azure portal by selecting the device in the IoT Hub blade, selecting
-# Device Twin then adding or amending an entry in the 'desired' section
-def device_twin_desired_updated(
-    desired_property_name: str, desired_property_value, desired_version: int
-):
-    print(
-        "Property",
-        desired_property_name,
-        "updated to",
-        str(desired_property_value),
-        "version",
-        desired_version,
-    )
 
+# Subscribe to cloud to device messages
+# To send a message to the device, select it in the Azure Portal, select Message To Device,
+# fill in the message and any properties you want to add, then select Send Message
+def cloud_to_device_message_received(body: str, properties: dict):
+    print("Received message with body", body, "and properties", json.dumps(properties))
 
-# Subscribe to the device twin desired property updated event
-device.on_device_twin_desired_updated = device_twin_desired_updated
+
+# Subscribe to the cloud to device message received events
+device.on_cloud_to_device_message_received = cloud_to_device_message_received
 
 print("Connecting to Azure IoT Hub...")
+
+# Connect to IoT Central
 device.connect()
 
 print("Connected to Azure IoT Hub!")
 
 message_counter = 60
 
 while True:
     try:
+        # Send a device to cloud message every minute
+        # You can see the overview of messages sent from the device in the Overview tab
+        # of the IoT Hub in the Azure Portal
         if message_counter >= 60:
-            # Send a reported property twin update every minute
-            # You can see these in the portal by selecting the device in the IoT Hub blade, selecting
-            # Device Twin then looking for the updates in the 'reported' section
-            patch = {"Temperature": random.randint(0, 50)}
-            device.update_twin(patch)
+            message = {"Temperature": random.randint(0, 50)}
+            device.send_device_to_cloud_message(json.dumps(message))
             message_counter = 0
         else:
             message_counter += 1
 
         # Poll every second for messages from the cloud
         device.loop()
     except (ValueError, RuntimeError) as e:
         print("Connection error, reconnecting\n", str(e))
-        # If we lose connectivity, reset the wifi and reconnect
-        wifi.radio.enabled = False
-        wifi.radio.enabled = True
-        wifi.radio.connect(secrets["ssid"], secrets["password"])
+        wifi.reset()
+        wifi.connect()
         device.reconnect()
         continue
     time.sleep(1)
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/examples/azureiot_secrets_example.py` & `adafruit_circuitpython_azureiot-2.6.0/examples/azureiot_secrets_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 DO NOT CHECK THIS INTO SOURCE CODE CONTROL!!!!11!!!
 """
 
 secrets = {
     # WiFi settings
     "ssid": "",
     "password": "",
-    # Azure IoT Central settings - if you are connecting to Azure IoT Central, fill in these three values
+    # Azure IoT Central settings - if you are connecting to Azure IoT Central, fill in these three
+    # values
     # To get these values, select your device in Azure IoT Central,
     # then select the Connect button
     # A dialog will appear with these three values
     # id_scope comes from the ID scope value
     # device_id comes from the Device ID value
     # key comes from either the Primary key or Secondary key
     "id_scope": "",
     "device_id": "",
     "device_sas_key": "",
     # Azure IoT Hub settings - if you are connecting to Azure IoT Hub, fill in this value
-    # To get this value, from the Azure Portal (https://aka.ms/AzurePortalHome), select your IoT Hub,
-    # then select Explorers -> IoT devices, select your device, then copy the entire primary or secondary
-    # connection string using the copy button next to the value and set this here.
+    # To get this value, from the Azure Portal (https://aka.ms/AzurePortalHome), select your IoT
+    # Hub, then select Explorers -> IoT devices, select your device, then copy the entire primary
+    # or secondary connection string using the copy button next to the value and set this here.
     # It will be in the format:
     #   HostName=<your-hub>.azure-devices.net;DeviceId=<your device id>;SharedAccessKey=<key>
     # Note - you need the primary or secondary connection string, NOT the primary or secondary key
     "device_connection_string": "",
 }
```

### Comparing `adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-button.png` & `adafruit_circuitpython_azureiot-2.6.0/iot-central-connect-button.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/iot-central-connect-dialog.png` & `adafruit_circuitpython_azureiot-2.6.0/iot-central-connect-dialog.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/iot-hub-device-keys.png` & `adafruit_circuitpython_azureiot-2.6.0/iot-hub-device-keys.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/iot-hub-device.png` & `adafruit_circuitpython_azureiot-2.6.0/iot-hub-device.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-azureiot-2.5.9/pyproject.toml` & `adafruit_circuitpython_azureiot-2.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-azureiot"
 description = "Access to Microsoft Azure IoT from CircuitPython"
-version = "2.5.9"
+version = "2.6.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AzureIoT"}
 keywords = [
     "adafruit",
@@ -39,12 +39,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adafruit_azureiot"]
+packages = ["adafruit_azureiot"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

