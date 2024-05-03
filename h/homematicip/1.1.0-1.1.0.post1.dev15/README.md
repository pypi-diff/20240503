# Comparing `tmp/homematicip-1.1.0.tar.gz` & `tmp/homematicip-1.1.0.post1.dev15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homematicip-1.1.0.tar", last modified: Sun Jan 14 17:42:43 2024, max compression
+gzip compressed data, was "homematicip-1.1.0.post1.dev15.tar", last modified: Fri May  3 15:09:33 2024, max compression
```

## Comparing `homematicip-1.1.0.tar` & `homematicip-1.1.0.post1.dev15.tar`

### file list

```diff
@@ -1,159 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.355631 homematicip-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-14 17:42:34.000000 homematicip-1.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.323631 homematicip-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.331631 homematicip-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-14 17:42:34.000000 homematicip-1.1.0/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-01-14 17:42:34.000000 homematicip-1.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-14 17:42:34.000000 homematicip-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-01-14 17:42:34.000000 homematicip-1.1.0/.github/workflows/test-on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-01-14 17:42:34.000000 homematicip-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-01-14 17:42:34.000000 homematicip-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-01-14 17:42:34.000000 homematicip-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-01-14 17:42:34.000000 homematicip-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-14 17:42:34.000000 homematicip-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    57438 2024-01-14 17:42:43.355631 homematicip-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-01-14 17:42:34.000000 homematicip-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.331631 homematicip-1.1.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-01-14 17:42:34.000000 homematicip-1.1.0/bin/homematicip_cli_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-14 17:42:34.000000 homematicip-1.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.331631 homematicip-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.335631 homematicip-1.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.335631 homematicip-1.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/api_introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/homematicip.aio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/homematicip.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/homematicip.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-14 17:42:34.000000 homematicip-1.1.0/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.335631 homematicip-1.1.0/homematicip_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/fake_cloud_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.335631 homematicip-1.1.0/homematicip_demo/json_data/
--rw-r--r--   0 runner    (1001) docker     (127)   479172 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/json_data/home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/json_data/security_journal.json
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/json_data/unknown_types.json
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_demo/server.key
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.335631 homematicip-1.1.0/homematicip_samples/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.339631 homematicip-1.1.0/homematicip_samples/CheckPresenceOnPing/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/CheckPresenceOnPing/CheckPresenceOnPing.pyproj
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/CheckPresenceOnPing/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/CheckPresenceOnPing/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/CheckPresenceOnPing/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.339631 homematicip-1.1.0/homematicip_samples/ControlDevices/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/ControlDevices/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/ControlDevices/switch_on_off.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.339631 homematicip-1.1.0/homematicip_samples/GetDevicesAndValues/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/GetDevicesAndValues/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/GetDevicesAndValues/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/GetDevicesAndValues/api_with_url.py
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.339631 homematicip-1.1.0/homematicip_samples/QRCodeGenerator/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/QRCodeGenerator/QRCodeGenerator.pyproj
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/QRCodeGenerator/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/QRCodeGenerator/qrcodegenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/QRCodeGenerator/qrcodes_template.html
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/QRCodeGenerator/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/SampleLibrary.sln
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.339631 homematicip-1.1.0/homematicip_samples/SampleTemplate/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/SampleTemplate/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/SampleTemplate/SampleTemplate.pyproj
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/SampleTemplate/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/SampleTemplate/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.339631 homematicip-1.1.0/homematicip_samples/TelegramNotificationBot/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/TelegramNotificationBot/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/TelegramNotificationBot/TelegramNotificationBot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/TelegramNotificationBot/TelegramNotificationBot.pyproj
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-14 17:42:34.000000 homematicip-1.1.0/homematicip_samples/TelegramNotificationBot/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-14 17:42:34.000000 homematicip-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-14 17:42:34.000000 homematicip-1.1.0/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-14 17:42:34.000000 homematicip-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-14 17:42:34.000000 homematicip-1.1.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-14 17:42:34.000000 homematicip-1.1.0/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 17:42:43.355631 homematicip-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-14 17:42:34.000000 homematicip-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.327631 homematicip-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.343631 homematicip-1.1.0/src/homematicip/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/EventHook.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/HomeMaticIPObject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/access_point_update_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.347631 homematicip-1.1.0/src/homematicip/aio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/class_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/home.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/aio/securityEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.347631 homematicip-1.1.0/src/homematicip/base/
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/HomeMaticIPObject.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    82614 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/functionalChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/class_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.351631 homematicip-1.1.0/src/homematicip/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    36059 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/cli/hmip_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/cli/hmip_generate_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    88553 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/functionalHomes.py
--rw-r--r--   0 runner    (1001) docker     (127)    44611 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    29379 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/home.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/oauth_otk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/securityEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-14 17:42:34.000000 homematicip-1.1.0/src/homematicip/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.355631 homematicip-1.1.0/src/homematicip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    57438 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-14 17:42:43.000000 homematicip-1.1.0/src/homematicip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-14 17:42:34.000000 homematicip-1.1.0/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-14 17:42:34.000000 homematicip-1.1.0/test_aio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.351631 homematicip-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 17:42:43.355631 homematicip-1.1.0/tests/aio_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/fake_hmip_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/notest_async_heating_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/notest_connection_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/notest_plugable_switch_measuring_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/test_async_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    42016 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/test_async_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/test_async_functional_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/test_async_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/test_async_home.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/aio_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    76856 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_fake_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_functional_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    21175 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_hmip_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_home.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-01-14 17:42:34.000000 homematicip-1.1.0/tests/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.621180 homematicip-1.1.0.post1.dev15/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/test-on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/api_introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/homematicip.aio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/homematicip.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/homematicip.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.621180 homematicip-1.1.0.post1.dev15/sample_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.633180 homematicip-1.1.0.post1.dev15/sample_data/json_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   524183 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/sample_data/json_data/home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/sample_data/json_data/security_journal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/sample_data/json_data/unknown_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.625180 homematicip-1.1.0.post1.dev15/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.633180 homematicip-1.1.0.post1.dev15/src/homematicip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.633180 homematicip-1.1.0.post1.dev15/src/homematicip/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/action_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/functional_channel_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/group_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44048 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli_debug_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/log_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/client_characteristics_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/client_token_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/rest_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/hmip_event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/exceptions/config_not_found_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/src/homematicip/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/anoymizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52256 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/functional_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/hmip_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/actions/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/actions/test_action_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/actions/test_group_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/connection/test_client_characteristics_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/connection/test_rest_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/events/test_hmip_event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/model/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/model/test_functional_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/test_runner.py
```

### Comparing `homematicip-1.1.0/.github/workflows/build-docs.yml` & `homematicip-1.1.0.post1.dev15/.github/workflows/build-docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 jobs:
   build_docs:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_docs.txt
           pip install -e .
```

### Comparing `homematicip-1.1.0/.github/workflows/codeql-analysis.yml` & `homematicip-1.1.0.post1.dev15/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/.github/workflows/publish.yml` & `homematicip-1.1.0.post1.dev15/.github/workflows/publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,46 +9,46 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 1
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.12"]
     steps:
       - name: Set Timezone
-        uses: szenius/set-timezone@v1.1
+        uses: szenius/set-timezone@v2.0
         with:
           timezoneLinux: "Europe/Berlin"
           timezoneMacos: "Europe/Berlin"
           timezoneWindows: "Europe/Berlin"
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_dev.txt
           pip install -e .
       - name: Run tests and collect coverage
-        run: pytest --cov tests --asyncio-mode=legacy
+        run: pytest --cov tests --asyncio-mode=auto
   #    - name: Upload coverage to Codecov
   #      uses: codecov/codecov-action@v3
 
   deploy:
     needs: test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
@@ -61,15 +61,15 @@
   build_docs:
     # Publish docs after deployment
     needs: deploy
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_docs.txt
           pip install -e .
```

### Comparing `homematicip-1.1.0/.github/workflows/test-on-push.yml` & `homematicip-1.1.0.post1.dev15/.github/workflows/test-on-push.yml`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,25 @@
   workflow_dispatch:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.11", "3.12"]
+        python-version: ["3.12"]
     steps:
       - name: Set Timezone
-        uses: szenius/set-timezone@v1.1
+        uses: szenius/set-timezone@v2.0
         with:
           timezoneLinux: "Europe/Berlin"
           timezoneMacos: "Europe/Berlin"
           timezoneWindows: "Europe/Berlin"
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements_dev.txt
           pip install -e .
```

### Comparing `homematicip-1.1.0/.gitignore` & `homematicip-1.1.0.post1.dev15/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -109,8 +109,10 @@
 /venv38
 
 #Vscode folder
 .vscode/
 
 #own config file
 homematic.ini
+config.ini
+config.json
 src/homematicip/_version.py
```

### Comparing `homematicip-1.1.0/CHANGELOG.md` & `homematicip-1.1.0.post1.dev15/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/CODE_OF_CONDUCT.md` & `homematicip-1.1.0.post1.dev15/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/LICENSE.txt` & `homematicip-1.1.0.post1.dev15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/README.md` & `homematicip-1.1.0.post1.dev15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 - [x] HMIP-BSM (Brand Switch and Meter Actuator)
 - [ ] HMIP-BSM-I (Brand Switch and Meter Actuator, International)
 - [x] HMIP-BWTH (Wall Thermostat Display with switching output – for brand switches, 230V)
 - [ ] HMIP-BWTH24 (Wall Thermostat Display with switching output – for brand switches, 24V)
 - [x] HMIP-DBB (Doorbell Push-Button)
 - [x] HMIP-DLD (Door Lock Drive)
 - [x] HMIP-DLS (Door Lock Sensor)
+- [x] HmIP-DRG-DALI (Dali Gateway - readonly at the moment)
 - [x] HMIP-DRBLI4 (Blind Actuator for DIN rail mount – 4 channels)
 - [x] HMIP-DRSI1 (Switch Actuator for DIN rail mount – 1x channel)
 - [x] HMIP-DRDI3 (Dimming Actuator Inbound 230V – 3x channels, 200W per channel) electrical DIN rail
 - [x] HMIP-DRSI4 (Switch Actuator for DIN rail mount – 4x channels)
 - [x] HMIP-DSD-PCB (Door Signal Dector PCB)
 - [x] HMIP-eTRV (Heating-Thermostat with Display)
 - [x] HMIP-eTRV-2 (Heating-Thermostat with Display) New Version
@@ -166,14 +167,15 @@
 - [ ] HMIP-PSM-2 (Plugable Switch Measuring, Type F - Standard for Homematic) New Version
 - [x] HMIP-PSM-CH (Plugable Switch Measuring, Type J)
 - [ ] HMIP-PSM-IT (Type L not tested, but it should work)
 - [ ] HMIP-PSM-PE (Type E not tested, but it should work)
 - [ ] HMIP-PSM-UK (Type G not tested, but it should work)
 - [x] HMIP-RC8 (Remote Control - 8x buttons)
 - [ ] HMIP-RCB1 (Remote Control - 1x button)
+- [x] HMIP-RGBW (RGB Led Controller - Readonly at the moment)
 - [x] HMIP-SAM (Acceleration Sensor)
 - [x] HMIP-SCI (Contact Interface Sensor)
 - [x] HMIP-SCTH230 (CO2, Temperature and Humidity Sensor 230V)
 - [ ] HMIP-SFD (Fine Dust Sensor)
 - [x] HMIP-SLO (Light Sensor - outdoor)
 - [x] HMIP-SMI (Motion Detector with Brightness Sensor - indoor)
 - [x] HMIP-SMI55 (Motion Detector with Brightness Sensor and Remote Control - 2x buttons)
```

### Comparing `homematicip-1.1.0/docs/Makefile` & `homematicip-1.1.0.post1.dev15/docs/Makefile`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/make.bat` & `homematicip-1.1.0.post1.dev15/docs/make.bat`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/api_introduction.rst` & `homematicip-1.1.0.post1.dev15/docs/source/api_introduction.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/conf.py` & `homematicip-1.1.0.post1.dev15/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/gettingstarted.rst` & `homematicip-1.1.0.post1.dev15/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/homematicip.aio.rst` & `homematicip-1.1.0.post1.dev15/docs/source/homematicip.aio.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/homematicip.base.rst` & `homematicip-1.1.0.post1.dev15/docs/source/homematicip.base.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/homematicip.rst` & `homematicip-1.1.0.post1.dev15/docs/source/homematicip.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/docs/source/index.rst` & `homematicip-1.1.0.post1.dev15/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/homematicip_demo/json_data/home.json` & `homematicip-1.1.0.post1.dev15/sample_data/json_data/home.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948487124664211%*

 * *Differences: {"'devices'": "{'3014F7110000000000000023': {'availableFirmwareVersion': '1.0.62', "*

 * *              "'firmwareVersion': '1.0.62', 'firmwareVersionInteger': 65598, 'functionalChannels': "*

 * *              "{'0': {'functionalChannelType': 'DEVICE_BASE', 'lowBat': None, 'rssiDeviceValue': "*

 * *              "-44, 'rssiPeerValue': None, 'supportedOptionalFeatures': {replace: "*

 * *              "OrderedDict([('IFeatureBusConfigMismatch', False), ('IFeatureDeviceCoProError', "*

 * *              "False), ('IFeatureDeviceCoProRe […]*

```diff
@@ -1360,69 +1360,319 @@
             "oem": "eQ-3",
             "permanentlyReachable": true,
             "serializedGlobalTradeItemNumber": "3014F7110000000000000022",
             "type": "WALL_MOUNTED_THERMOSTAT_PRO",
             "updateState": "UP_TO_DATE"
         },
         "3014F7110000000000000023": {
-            "availableFirmwareVersion": "0.0.0",
+            "availableFirmwareVersion": "1.0.62",
             "connectionType": "HMIP_RF",
-            "firmwareVersion": "1.8.0",
-            "firmwareVersionInteger": 67584,
+            "deviceArchetype": "HMIP",
+            "fastColorChangeSupported": true,
+            "firmwareVersion": "1.0.62",
+            "firmwareVersionInteger": 65598,
             "functionalChannels": {
                 "0": {
+                    "busConfigMismatch": null,
+                    "coProFaulty": false,
+                    "coProRestartNeeded": false,
+                    "coProUpdateFailure": false,
                     "configPending": false,
+                    "controlsMountingOrientation": null,
+                    "daliBusState": null,
+                    "defaultLinkedGroup": [],
+                    "deviceCommunicationError": null,
+                    "deviceDriveError": null,
+                    "deviceDriveModeError": null,
                     "deviceId": "3014F7110000000000000023",
+                    "deviceOperationMode": "UNIVERSAL_LIGHT_2_TUNABLE_WHITE",
+                    "deviceOverheated": false,
+                    "deviceOverloaded": false,
+                    "devicePowerFailureDetected": false,
+                    "deviceUndervoltage": false,
+                    "displayContrast": null,
                     "dutyCycle": false,
-                    "functionalChannelType": "DEVICE_OPERATIONLOCK",
+                    "functionalChannelType": "DEVICE_BASE",
                     "groupIndex": 0,
                     "groups": [
                         "00000000-0000-0000-0000-000000000008"
                     ],
                     "index": 0,
                     "label": "",
-                    "lowBat": false,
-                    "operationLockActive": false,
+                    "lockJammed": null,
+                    "lowBat": null,
+                    "mountingOrientation": null,
+                    "multicastRoutingEnabled": false,
+                    "particulateMatterSensorCommunicationError": null,
+                    "particulateMatterSensorError": null,
+                    "powerShortCircuit": null,
+                    "profilePeriodLimitReached": null,
                     "routerModuleEnabled": false,
                     "routerModuleSupported": false,
-                    "rssiDeviceValue": -61,
-                    "rssiPeerValue": -58,
-                    "supportedOptionalFeatures": {},
+                    "rssiDeviceValue": -44,
+                    "rssiPeerValue": null,
+                    "sensorCommunicationError": null,
+                    "sensorError": null,
+                    "shortCircuitDataLine": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureBusConfigMismatch": false,
+                        "IFeatureDeviceCoProError": false,
+                        "IFeatureDeviceCoProRestart": false,
+                        "IFeatureDeviceCoProUpdate": false,
+                        "IFeatureDeviceCommunicationError": false,
+                        "IFeatureDeviceDaliBusError": false,
+                        "IFeatureDeviceDriveError": false,
+                        "IFeatureDeviceDriveModeError": false,
+                        "IFeatureDeviceIdentify": false,
+                        "IFeatureDeviceOverheated": true,
+                        "IFeatureDeviceOverloaded": false,
+                        "IFeatureDeviceParticulateMatterSensorCommunicationError": false,
+                        "IFeatureDeviceParticulateMatterSensorError": false,
+                        "IFeatureDevicePowerFailure": false,
+                        "IFeatureDeviceSensorCommunicationError": false,
+                        "IFeatureDeviceSensorError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorCommunicationError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorError": false,
+                        "IFeatureDeviceTemperatureOutOfRange": false,
+                        "IFeatureDeviceUndervoltage": false,
+                        "IFeatureMulticastRouter": false,
+                        "IFeaturePowerShortCircuit": false,
+                        "IFeatureProfilePeriodLimit": false,
+                        "IFeatureRssiValue": true,
+                        "IFeatureShortCircuitDataLine": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDefaultLinkedGroup": false,
+                        "IOptionalFeatureDeviceErrorLockJammed": false,
+                        "IOptionalFeatureDeviceOperationMode": true,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureDisplayContrast": false,
+                        "IOptionalFeatureDutyCycle": true,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureLowBat": false,
+                        "IOptionalFeatureMountingOrientation": false
+                    },
+                    "temperatureHumiditySensorCommunicationError": null,
+                    "temperatureHumiditySensorError": null,
+                    "temperatureOutOfRange": false,
                     "unreach": false
                 },
                 "1": {
-                    "actualTemperature": 24.5,
+                    "channelActive": false,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 4100,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
                     "deviceId": "3014F7110000000000000023",
-                    "display": "ACTUAL_HUMIDITY",
-                    "functionalChannelType": "WALL_MOUNTED_THERMOSTAT_PRO_CHANNEL",
+                    "dim2WarmActive": false,
+                    "dimLevel": 0.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
                     "groupIndex": 1,
                     "groups": [
-                        "00000000-0000-0000-0000-000000000010"
+                        "00000000-0000-0000-0000-000000000014",
+                        "00000000-0000-0000-0000-000000000017",
+                        "00000000-0000-0000-0000-000000000023"
                     ],
-                    "humidity": 46,
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
                     "index": 1,
+                    "label": "Decke Fernseher",
+                    "lampFailure": null,
+                    "lightSceneId": 0,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": false,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": 0.0,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "2": {
+                    "channelActive": false,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 3050,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F7110000000000000023",
+                    "dim2WarmActive": false,
+                    "dimLevel": 0.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 2,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000014"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 2,
+                    "label": "LED TV",
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": false,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "3": {
+                    "channelActive": false,
+                    "channelRole": null,
+                    "colorTemperature": null,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F7110000000000000023",
+                    "dim2WarmActive": null,
+                    "dimLevel": null,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 0,
+                    "groups": [],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": null,
+                    "index": 3,
                     "label": "",
-                    "setPointTemperature": 19.0,
-                    "temperatureOffset": 0.0,
-                    "valveActualTemperature": 20.0,
-                    "vaporAmount": 6.177718198711658
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": null,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": false,
+                        "IFeatureLightProfileActuatorChannel": false,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "4": {
+                    "channelActive": false,
+                    "channelRole": null,
+                    "colorTemperature": null,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F7110000000000000023",
+                    "dim2WarmActive": null,
+                    "dimLevel": null,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 0,
+                    "groups": [],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": null,
+                    "index": 4,
+                    "label": "",
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": null,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": false,
+                        "IFeatureLightProfileActuatorChannel": false,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
                 }
             },
             "homeId": "00000000-0000-0000-0000-000000000001",
             "id": "3014F7110000000000000023",
-            "label": "Wandthermostat4",
-            "lastStatusUpdate": 1524516454116,
+            "label": "LED 2",
+            "lastStatusUpdate": 1707896379040,
             "liveUpdateState": "LIVE_UPDATE_NOT_SUPPORTED",
+            "manuallyUpdateForced": false,
             "manufacturerCode": 1,
-            "modelId": 297,
-            "modelType": "HmIP-WTH-2",
+            "measuredAttributes": {},
+            "modelId": 462,
+            "modelType": "HmIP-RGBW",
             "oem": "eQ-3",
             "permanentlyReachable": true,
             "serializedGlobalTradeItemNumber": "3014F7110000000000000023",
-            "type": "WALL_MOUNTED_THERMOSTAT_PRO",
+            "type": "RGBW_DIMMER",
             "updateState": "UP_TO_DATE"
         },
         "3014F7110000000000000024": {
             "availableFirmwareVersion": "0.0.0",
             "connectionType": "HMIP_RF",
             "firmwareVersion": "1.8.0",
             "firmwareVersionInteger": 67584,
@@ -4179,14 +4429,369 @@
             "modelType": "HmIP-SMI",
             "oem": "eQ-3",
             "permanentlyReachable": true,
             "serializedGlobalTradeItemNumber": "3014F711000000000000BB11",
             "type": "MOTION_DETECTOR_INDOOR",
             "updateState": "UP_TO_DATE"
         },
+        "3014F711000000000000DALI": {
+            "availableFirmwareVersion": "1.4.8",
+            "connectionType": "HMIP_LAN",
+            "deviceArchetype": "HMIP",
+            "fastColorChangeSupported": false,
+            "firmwareVersion": "1.4.8",
+            "firmwareVersionInteger": 66568,
+            "functionalChannels": {
+                "0": {
+                    "busConfigMismatch": null,
+                    "coProFaulty": false,
+                    "coProRestartNeeded": false,
+                    "coProUpdateFailure": false,
+                    "configPending": false,
+                    "controlsMountingOrientation": null,
+                    "daliBusState": "BUS_OK",
+                    "defaultLinkedGroup": [],
+                    "deviceCommunicationError": null,
+                    "deviceDriveError": null,
+                    "deviceDriveModeError": null,
+                    "deviceId": "3014F711000000000000DALI",
+                    "deviceOperationMode": null,
+                    "deviceOverheated": false,
+                    "deviceOverloaded": false,
+                    "devicePowerFailureDetected": false,
+                    "deviceUndervoltage": false,
+                    "displayContrast": null,
+                    "dutyCycle": null,
+                    "functionalChannelType": "DEVICE_BASE",
+                    "groupIndex": 0,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000008"
+                    ],
+                    "index": 0,
+                    "label": "",
+                    "lockJammed": null,
+                    "lowBat": null,
+                    "mountingOrientation": null,
+                    "multicastRoutingEnabled": false,
+                    "particulateMatterSensorCommunicationError": null,
+                    "particulateMatterSensorError": null,
+                    "powerShortCircuit": null,
+                    "profilePeriodLimitReached": null,
+                    "routerModuleEnabled": false,
+                    "routerModuleSupported": false,
+                    "rssiDeviceValue": null,
+                    "rssiPeerValue": null,
+                    "sensorCommunicationError": null,
+                    "sensorError": null,
+                    "shortCircuitDataLine": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureBusConfigMismatch": false,
+                        "IFeatureDeviceCoProError": true,
+                        "IFeatureDeviceCoProRestart": false,
+                        "IFeatureDeviceCoProUpdate": false,
+                        "IFeatureDeviceCommunicationError": false,
+                        "IFeatureDeviceDaliBusError": true,
+                        "IFeatureDeviceDriveError": false,
+                        "IFeatureDeviceDriveModeError": false,
+                        "IFeatureDeviceIdentify": true,
+                        "IFeatureDeviceOverheated": false,
+                        "IFeatureDeviceOverloaded": false,
+                        "IFeatureDeviceParticulateMatterSensorCommunicationError": false,
+                        "IFeatureDeviceParticulateMatterSensorError": false,
+                        "IFeatureDevicePowerFailure": false,
+                        "IFeatureDeviceSensorCommunicationError": false,
+                        "IFeatureDeviceSensorError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorCommunicationError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorError": false,
+                        "IFeatureDeviceTemperatureOutOfRange": false,
+                        "IFeatureDeviceUndervoltage": false,
+                        "IFeatureMulticastRouter": false,
+                        "IFeaturePowerShortCircuit": false,
+                        "IFeatureProfilePeriodLimit": false,
+                        "IFeatureRssiValue": false,
+                        "IFeatureShortCircuitDataLine": false,
+                        "IOptionalFeatureDefaultLinkedGroup": false,
+                        "IOptionalFeatureDeviceErrorLockJammed": false,
+                        "IOptionalFeatureDeviceOperationMode": false,
+                        "IOptionalFeatureDisplayContrast": false,
+                        "IOptionalFeatureDutyCycle": false,
+                        "IOptionalFeatureLowBat": false,
+                        "IOptionalFeatureMountingOrientation": false
+                    },
+                    "temperatureHumiditySensorCommunicationError": null,
+                    "temperatureHumiditySensorError": null,
+                    "temperatureOutOfRange": false,
+                    "unreach": false
+                },
+                "1": {
+                    "channelActive": true,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 3000,
+                    "connectedDeviceUnreach": false,
+                    "controlGearFailure": false,
+                    "deviceId": "3014F711000000000000DALI",
+                    "dim2WarmActive": false,
+                    "dimLevel": 1.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 1,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000009"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 1,
+                    "label": "Spot R4",
+                    "lampFailure": false,
+                    "lightSceneId": 0,
+                    "limitFailure": false,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": true,
+                    "onMinLevel": 0.0,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": 0.0,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": true,
+                        "IFeatureControlGearFailure": true,
+                        "IFeatureLampFailure": true,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": true,
+                        "IOptionalFeatureChannelActive": true,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "2": {
+                    "channelActive": true,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 3000,
+                    "connectedDeviceUnreach": false,
+                    "controlGearFailure": false,
+                    "deviceId": "3014F711000000000000DALI",
+                    "dim2WarmActive": false,
+                    "dimLevel": 1.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 2,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000009"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 2,
+                    "label": "Spot R5",
+                    "lampFailure": false,
+                    "lightSceneId": 0,
+                    "limitFailure": false,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": true,
+                    "onMinLevel": 0.0,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": 0.0,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": true,
+                        "IFeatureControlGearFailure": true,
+                        "IFeatureLampFailure": true,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": true,
+                        "IOptionalFeatureChannelActive": true,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "3": {
+                    "channelActive": true,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 3000,
+                    "connectedDeviceUnreach": false,
+                    "controlGearFailure": false,
+                    "deviceId": "3014F711000000000000DALI",
+                    "dim2WarmActive": false,
+                    "dimLevel": 1.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 3,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000009"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 3,
+                    "label": "Spot L5",
+                    "lampFailure": false,
+                    "lightSceneId": 0,
+                    "limitFailure": false,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": true,
+                    "onMinLevel": 0.0,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": 0.0,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": true,
+                        "IFeatureControlGearFailure": true,
+                        "IFeatureLampFailure": true,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": true,
+                        "IOptionalFeatureChannelActive": true,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "4": {
+                    "channelActive": false,
+                    "channelRole": null,
+                    "channelSelections": [],
+                    "colorTemperature": null,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F711000000000000DALI",
+                    "dim2WarmActive": null,
+                    "dimLevel": null,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_GROUP_CHANNEL",
+                    "groupIndex": 33,
+                    "groups": [],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": null,
+                    "index": 4,
+                    "label": "",
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": null,
+                    "onMinLevel": 0.0,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": false,
+                        "IFeatureLightProfileActuatorChannel": false,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "5": {
+                    "channelActive": false,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "channelSelections": [
+                        1,
+                        2,
+                        3
+                    ],
+                    "colorTemperature": 3000,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F711000000000000DALI",
+                    "dim2WarmActive": false,
+                    "dimLevel": 1.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_GROUP_CHANNEL",
+                    "groupIndex": 35,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000009"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 5,
+                    "label": "ALL",
+                    "lampFailure": null,
+                    "lightSceneId": 0,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": true,
+                    "onMinLevel": 0.0,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": 0.0,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                }
+            },
+            "homeId": "00000000-0000-0000-0000-000000000001",
+            "id": "3014F711000000000000DALI",
+            "label": "DALI Gateway",
+            "lastStatusUpdate": 1713127484921,
+            "liveUpdateState": "LIVE_UPDATE_NOT_SUPPORTED",
+            "manuallyUpdateForced": false,
+            "manufacturerCode": 1,
+            "measuredAttributes": {},
+            "modelId": 461,
+            "modelType": "HmIP-DRG-DALI",
+            "oem": "eQ-3",
+            "permanentlyReachable": true,
+            "serializedGlobalTradeItemNumber": "3014F711000000000000DALI",
+            "type": "DALI_GATEWAY",
+            "updateState": "UP_TO_DATE"
+        },
         "3014F711000000000000DLD2": {
             "availableFirmwareVersion": "1.4.12",
             "connectionType": "HMIP_RF",
             "deviceArchetype": "HMIP",
             "firmwareVersion": "1.4.10",
             "firmwareVersionInteger": 66570,
             "functionalChannels": {
@@ -5223,14 +5828,324 @@
             "modelType": "HmIPW-FIO6",
             "oem": "eQ-3",
             "permanentlyReachable": true,
             "serializedGlobalTradeItemNumber": "3014F711000000000000FIO6",
             "type": "WIRED_INPUT_SWITCH_6",
             "updateState": "UP_TO_DATE"
         },
+        "3014F711000000000000RGBW": {
+            "availableFirmwareVersion": "1.0.62",
+            "connectionType": "HMIP_RF",
+            "deviceArchetype": "HMIP",
+            "fastColorChangeSupported": true,
+            "firmwareVersion": "1.0.62",
+            "firmwareVersionInteger": 65598,
+            "functionalChannels": {
+                "0": {
+                    "busConfigMismatch": null,
+                    "coProFaulty": false,
+                    "coProRestartNeeded": false,
+                    "coProUpdateFailure": false,
+                    "configPending": false,
+                    "controlsMountingOrientation": null,
+                    "daliBusState": null,
+                    "defaultLinkedGroup": [],
+                    "deviceCommunicationError": null,
+                    "deviceDriveError": null,
+                    "deviceDriveModeError": null,
+                    "deviceId": "3014F711000000000000RGBW",
+                    "deviceOperationMode": "UNIVERSAL_LIGHT_2_TUNABLE_WHITE",
+                    "deviceOverheated": false,
+                    "deviceOverloaded": false,
+                    "devicePowerFailureDetected": false,
+                    "deviceUndervoltage": false,
+                    "displayContrast": null,
+                    "dutyCycle": false,
+                    "functionalChannelType": "DEVICE_BASE",
+                    "groupIndex": 0,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000008"
+                    ],
+                    "index": 0,
+                    "label": "",
+                    "lockJammed": null,
+                    "lowBat": null,
+                    "mountingOrientation": null,
+                    "multicastRoutingEnabled": false,
+                    "particulateMatterSensorCommunicationError": null,
+                    "particulateMatterSensorError": null,
+                    "powerShortCircuit": null,
+                    "profilePeriodLimitReached": null,
+                    "routerModuleEnabled": false,
+                    "routerModuleSupported": false,
+                    "rssiDeviceValue": -48,
+                    "rssiPeerValue": null,
+                    "sensorCommunicationError": null,
+                    "sensorError": null,
+                    "shortCircuitDataLine": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureBusConfigMismatch": false,
+                        "IFeatureDeviceCoProError": false,
+                        "IFeatureDeviceCoProRestart": false,
+                        "IFeatureDeviceCoProUpdate": false,
+                        "IFeatureDeviceCommunicationError": false,
+                        "IFeatureDeviceDaliBusError": false,
+                        "IFeatureDeviceDriveError": false,
+                        "IFeatureDeviceDriveModeError": false,
+                        "IFeatureDeviceIdentify": false,
+                        "IFeatureDeviceOverheated": true,
+                        "IFeatureDeviceOverloaded": false,
+                        "IFeatureDeviceParticulateMatterSensorCommunicationError": false,
+                        "IFeatureDeviceParticulateMatterSensorError": false,
+                        "IFeatureDevicePowerFailure": false,
+                        "IFeatureDeviceSensorCommunicationError": false,
+                        "IFeatureDeviceSensorError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorCommunicationError": false,
+                        "IFeatureDeviceTemperatureHumiditySensorError": false,
+                        "IFeatureDeviceTemperatureOutOfRange": false,
+                        "IFeatureDeviceUndervoltage": false,
+                        "IFeatureMulticastRouter": false,
+                        "IFeaturePowerShortCircuit": false,
+                        "IFeatureProfilePeriodLimit": false,
+                        "IFeatureRssiValue": true,
+                        "IFeatureShortCircuitDataLine": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDefaultLinkedGroup": false,
+                        "IOptionalFeatureDeviceErrorLockJammed": false,
+                        "IOptionalFeatureDeviceOperationMode": true,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureDisplayContrast": false,
+                        "IOptionalFeatureDutyCycle": true,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureLowBat": false,
+                        "IOptionalFeatureMountingOrientation": false
+                    },
+                    "temperatureHumiditySensorCommunicationError": null,
+                    "temperatureHumiditySensorError": null,
+                    "temperatureOutOfRange": false,
+                    "unreach": false
+                },
+                "1": {
+                    "channelActive": false,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 4100,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F711000000000000RGBW",
+                    "dim2WarmActive": false,
+                    "dimLevel": 0.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 1,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000014",
+                        "00000000-0000-0000-0000-000000000017",
+                        "00000000-0000-0000-0000-000000000023"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 1,
+                    "label": "Decke Sofa",
+                    "lampFailure": null,
+                    "lightSceneId": 0,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": false,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": 0.0,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "2": {
+                    "channelActive": false,
+                    "channelRole": "UNIVERSAL_LIGHT_ACTUATOR",
+                    "colorTemperature": 4100,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F711000000000000RGBW",
+                    "dim2WarmActive": false,
+                    "dimLevel": 0.0,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 2,
+                    "groups": [
+                        "00000000-0000-0000-0000-000000000014",
+                        "00000000-0000-0000-0000-000000000017",
+                        "00000000-0000-0000-0000-000000000023"
+                    ],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": false,
+                    "index": 2,
+                    "label": "Decke Fenster",
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": false,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": true,
+                        "IFeatureLightProfileActuatorChannel": true,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": true,
+                        "IOptionalFeatureColorTemperatureDim2Warm": true,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": true,
+                        "IOptionalFeatureDimmerState": true,
+                        "IOptionalFeatureHardwareColorTemperature": true,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "3": {
+                    "channelActive": false,
+                    "channelRole": null,
+                    "colorTemperature": null,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F711000000000000RGBW",
+                    "dim2WarmActive": null,
+                    "dimLevel": null,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 0,
+                    "groups": [],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": null,
+                    "index": 3,
+                    "label": "",
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": null,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": false,
+                        "IFeatureLightProfileActuatorChannel": false,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                },
+                "4": {
+                    "channelActive": false,
+                    "channelRole": null,
+                    "colorTemperature": null,
+                    "connectedDeviceUnreach": null,
+                    "controlGearFailure": null,
+                    "deviceId": "3014F711000000000000RGBW",
+                    "dim2WarmActive": null,
+                    "dimLevel": null,
+                    "functionalChannelType": "UNIVERSAL_LIGHT_CHANNEL",
+                    "groupIndex": 0,
+                    "groups": [],
+                    "hardwareColorTemperatureColdWhite": 6500,
+                    "hardwareColorTemperatureWarmWhite": 2000,
+                    "hue": null,
+                    "humanCentricLightActive": null,
+                    "index": 4,
+                    "label": "",
+                    "lampFailure": null,
+                    "lightSceneId": null,
+                    "limitFailure": null,
+                    "maximumColorTemperature": 6500,
+                    "minimalColorTemperature": 2000,
+                    "on": null,
+                    "onMinLevel": 0.05,
+                    "profileMode": "AUTOMATIC",
+                    "saturationLevel": null,
+                    "supportedOptionalFeatures": {
+                        "IFeatureConnectedDeviceUnreach": false,
+                        "IFeatureControlGearFailure": false,
+                        "IFeatureLampFailure": false,
+                        "IFeatureLightGroupActuatorChannel": false,
+                        "IFeatureLightProfileActuatorChannel": false,
+                        "IFeatureLimitFailure": false,
+                        "IOptionalFeatureChannelActive": false,
+                        "IOptionalFeatureColorTemperature": false,
+                        "IOptionalFeatureColorTemperatureDim2Warm": false,
+                        "IOptionalFeatureColorTemperatureDynamicDaylight": false,
+                        "IOptionalFeatureDimmerState": false,
+                        "IOptionalFeatureHardwareColorTemperature": false,
+                        "IOptionalFeatureHueSaturationValue": false,
+                        "IOptionalFeatureLightScene": false,
+                        "IOptionalFeatureLightSceneWithShortTimes": false,
+                        "IOptionalFeatureOnMinLevel": true
+                    },
+                    "userDesiredProfileMode": "AUTOMATIC"
+                }
+            },
+            "homeId": "00000000-0000-0000-0000-000000000001",
+            "id": "3014F711000000000000RGBW",
+            "label": "LED 1",
+            "lastStatusUpdate": 1707895310349,
+            "liveUpdateState": "LIVE_UPDATE_NOT_SUPPORTED",
+            "manuallyUpdateForced": false,
+            "manufacturerCode": 1,
+            "measuredAttributes": {},
+            "modelId": 462,
+            "modelType": "HmIP-RGBW",
+            "oem": "eQ-3",
+            "permanentlyReachable": true,
+            "serializedGlobalTradeItemNumber": "3014F711000000000000RGBW",
+            "type": "RGBW_DIMMER",
+            "updateState": "UP_TO_DATE"
+        },
         "3014F711000000000000WSPI": {
             "availableFirmwareVersion": "1.0.30",
             "connectionType": "HMIP_WIRED",
             "deviceArchetype": "HMIP",
             "firmwareVersion": "1.0.30",
             "firmwareVersionInteger": 65566,
             "functionalChannels": {
@@ -13268,14 +14183,31 @@
             "secondaryShadingLevel": null,
             "secondaryShadingStateType": "NOT_EXISTENT",
             "shutterLevel": 0.97,
             "slatsLevel": null,
             "type": "SHUTTER_PROFILE",
             "unreach": false
         },
+        "00000000-0000-0000-0000-0000000000EN": {
+            "channels": [
+                {
+                    "channelIndex": 1,
+                    "deviceId": "3014F7110000000000000019"
+                }
+            ],
+            "dutyCycle": false,
+            "homeId": "00000000-0000-0000-0000-000000000001",
+            "id": "00000000-0000-0000-0000-0000000000EN",
+            "label": "EnergyGroupHWR",
+            "lastStatusUpdate": 1713711529425,
+            "lowBat": false,
+            "metaGroupId": "00000000-0000-0000-0000-000000000023",
+            "type": "ENERGY",
+            "unreach": false
+        },
         "00000000-0000-0000-0000-0000000000IC": {
             "channels": [
                 {
                     "channelIndex": 1,
                     "deviceId": "3014F7110000000000000005"
                 },
                 {
```

### Comparing `homematicip-1.1.0/homematicip_demo/json_data/security_journal.json` & `homematicip-1.1.0.post1.dev15/sample_data/json_data/security_journal.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/homematicip_demo/json_data/unknown_types.json` & `homematicip-1.1.0.post1.dev15/sample_data/json_data/unknown_types.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0/pyproject.toml` & `homematicip-1.1.0.post1.dev15/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,48 +4,47 @@
     "setuptools-scm>=8.0"]
 
 [project]
 name = "homematicip"
 description = "An API for the homematicip cloud"
 readme = "README.md"
 dependencies = [
-    "requests>=2.24.0",
-    "websocket-client>=1.0.0",
-    "async_timeout>=3.0.1",
-    "websockets>=8.1",
-    "aiohttp>=3.9"
+  "pydantic",
+  "websockets",
+  "httpx",
+  "click",
+  "alive-progress"
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.12"
 authors = [
   {name = "Thomas Hahn", email = "homematicip-rest-api@outlook.com"},
 ]
 classifiers=[
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 keywords = ["homematicip cloud","homematicip"]
 dynamic = [
     "version"
 ]
-license = {file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://github.com/hahn-th/homematicip-rest-api"
 Repository = "https://github.com/hahn-th/homematicip-rest-api.git"
 Issues = "https://github.com/hahn-th/homematicip-rest-api/issues"
 Changelog = "https://github.com/hahn-th/homematicip-rest-api/blob/master/CHANGELOG.md"
 
 [tool.setuptools_scm]
 version_file = "src/homematicip/_version.py"
 version_scheme = "no-guess-dev"
 local_scheme = "no-local-version"
 
+
+[project.scripts]
+hmip = "homematicip.cli.hmip_cli:cli"
+
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+#addopts = "--cov=src --cov-report term-missing"
 
-
-[project.scripts]
-hmip_cli = "homematicip.cli.hmip_cli:main"
-hmip_generate_auth_token = "homematicip.cli.hmip_generate_auth_token:main"
+[tool.coverage.run]
+source = ["src"]
```

### Comparing `homematicip-1.1.0/src/homematicip/__init__.py` & `homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config_io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,89 @@
-# coding=utf-8
-import configparser
+import json
+import logging
 import os
 import platform
-from collections import namedtuple
+from configparser import ConfigParser
+from dataclasses import asdict
 
-# from ._version import get_versions
+from homematicip.configuration.config import PersistentConfig
+from homematicip.configuration.log_helper import get_home_path
 
-# __version__ = get_versions()["version"]
-# del get_versions
 
-HmipConfig = namedtuple(
-    "HmipConfig", ["auth_token", "access_point", "log_level", "log_file", "raw_config"]
-)
-
-
-def find_and_load_config_file() -> HmipConfig:
-    for f in get_config_file_locations():
-        try:
-            return load_config_file(f)
-        except FileNotFoundError:
-            pass
-    return None
-
-
-def load_config_file(config_file: str) -> HmipConfig:
-    """Loads the config ini file.
-    :raises a FileNotFoundError when the config file does not exist."""
-    expanded_config_file = os.path.expanduser(config_file)
-    _config = configparser.ConfigParser()
-    with open(expanded_config_file, "r") as fl:
-        _config.read_file(fl)
-        logging_filename = _config.get("LOGGING", "FileName", fallback="hmip.log")
-        if logging_filename == "None":
-            logging_filename = None
-
-        _hmip_config = HmipConfig(
-            _config["AUTH"]["AuthToken"],
-            _config["AUTH"]["AccessPoint"],
-            int(_config.get("LOGGING", "Level", fallback=30)),
-            logging_filename,
-            _config._sections,
-        )
-        return _hmip_config
-
-
-def get_config_file_locations() -> []:
-    search_locations = ["./config.ini"]
-
-    os_name = platform.system()
-
-    if os_name == "Windows":
-        appdata = os.getenv("appdata")
-        programdata = os.getenv("programdata")
-        search_locations.append(
-            os.path.join(appdata, "homematicip-rest-api\\config.ini")
-        )
-        search_locations.append(
-            os.path.join(programdata, "homematicip-rest-api\\config.ini")
-        )
-    elif os_name == "Linux":
-        search_locations.append("~/.homematicip-rest-api/config.ini")
-        search_locations.append("/etc/homematicip-rest-api/config.ini")
-    elif os_name == "Darwin":  # MAC
-        # are these folders right?
-        search_locations.append("~/Library/Preferences/homematicip-rest-api/config.ini")
-        search_locations.append(
-            "/Library/Application Support/homematicip-rest-api/config.ini"
-        )
-    return search_locations
+class ConfigIO:
+
+    @classmethod
+    def find_config_in_well_known_locations(cls) -> PersistentConfig | None:
+        """Find the configuration file in the well known locations.
+        @return the configuration if found, None otherwise."""
+        for location in cls._get_well_known_locations():
+            if os.path.exists(location):
+                return cls.from_file(location)
+
+        return None
+
+    @classmethod
+    def _get_well_known_locations(cls) -> list[str]:
+        """Get the well known locations for the configuration file."""
+        config_filename = "config.json"
+        search_locations = [os.path.join("./", config_filename)]
+
+        os_name = platform.system()
+
+        if os_name == "Windows":
+            appdata = os.getenv("appdata")
+            programdata = os.getenv("programdata")
+            search_locations.append(
+                os.path.join(appdata, "homematicip-rest-api", config_filename)
+            )
+            search_locations.append(
+                os.path.join(programdata, "homematicip-rest-api", config_filename)
+            )
+        elif os_name == "Linux":
+            search_locations.append(f"~/.homematicip-rest-api/{config_filename}")
+            search_locations.append(f"/etc/homematicip-rest-api/{config_filename}")
+        elif os_name == "Darwin":  # MAC
+            # are these folders right?
+            search_locations.append(f"~/Library/Preferences/homematicip-rest-api/{config_filename}")
+            search_locations.append(
+                f"/Library/Application Support/homematicip-rest-api/{config_filename}"
+            )
+        return search_locations
+
+    @classmethod
+    def from_file(cls, file_path) -> PersistentConfig:
+        """Open a file and load the configuration from it."""
+        with open(file_path,"r") as f:
+            json_config = json.load(f)
+            config = PersistentConfig(**json_config)
+
+        # config_parser = ConfigParser()
+        # config_parser.read(file_path)
+        #
+        # config = PersistentConfig()
+        # config.auth_token = config_parser.get('AUTH', 'authtoken', fallback=None)
+        # config.accesspoint_id = config_parser.get('AUTH', 'accesspoint', fallback=None)
+        # config.level = int(config_parser.get('LOGGING', 'level', fallback=logging.INFO))
+        # config.log_file = config_parser.get('LOGGING', 'log_file', fallback=None)
+
+        return config
+
+    @classmethod
+    def to_file(cls, config: PersistentConfig) -> str:
+        """Write the configuration to a file.
+        @return the file path of the written file."""
+        # config_parser = ConfigParser()
+        # config_parser['AUTH'] = {
+        #     'authtoken': config.auth_token,
+        #     'accesspoint': config.accesspoint_id
+        # }
+        # config_parser['LOGGING'] = {
+        #     'level': config.level,
+        #     'log_file': config.log_file
+        # }
+        #
+        filename = os.path.join(get_home_path(), "config.json")
+
+        with open(filename, 'w') as file:
+            json.dump(asdict(config), file)
+
+        return filename
```

### Comparing `homematicip-1.1.0/src/homematicip/auth.py` & `homematicip-1.1.0.post1.dev15/src/homematicip/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,72 @@
-# coding=utf-8
-import json
+import logging
 import uuid
+from dataclasses import dataclass
 
-import requests
+from homematicip.connection.rest_connection import ConnectionContext, RestResult, RestConnection
 
-import homematicip
-from homematicip.home import Home
+LOGGER = logging.getLogger(__name__)
 
 
-class Auth(object):
-    def __init__(self, home: Home):
-        self.uuid = str(uuid.uuid4())
+@dataclass
+class Auth:
+
+    client_id: str = str(uuid.uuid4())
+    header: dict = None
+    pin: str = None
+    connection: RestConnection = None
+
+    def __init__(self, context: ConnectionContext):
+        LOGGER.debug("Initialize new Auth")
+        self.connection = RestConnection(context)
         self.headers = {
             "content-type": "application/json",
             "accept": "application/json",
-            "VERSION": "12",
-            "CLIENTAUTH": home._connection.clientauth_token,
+            "VERSION": "12"
         }
-        self.url_rest = home._connection.urlREST
-        self.pin = None
 
-    def connectionRequest(
-        self, access_point, devicename="homematicip-python"
-    ) -> requests.Response:
-        data = {"deviceId": self.uuid, "deviceName": devicename, "sgtin": access_point}
+    async def connection_request(self, access_point: str, device_name="homematicip-python", pin=None) -> RestResult:
+        LOGGER.debug(f"Requesting connection for access point {access_point}")
         headers = self.headers
-        if self.pin != None:
-            headers["PIN"] = self.pin
-        response = requests.post(
-            "{}/hmip/auth/connectionRequest".format(self.url_rest),
-            json=data,
-            headers=headers,
-        )
-        return response
-
-    def isRequestAcknowledged(self):
-        data = {"deviceId": self.uuid}
-        response = requests.post(
-            "{}/hmip/auth/isRequestAcknowledged".format(self.url_rest),
-            json=data,
-            headers=self.headers,
-        )
-        return response.status_code == 200
-
-    def requestAuthToken(self):
-        data = {"deviceId": self.uuid}
-        response = requests.post(
-            "{}/hmip/auth/requestAuthToken".format(self.url_rest),
-            json=data,
-            headers=self.headers,
-        )
-        return json.loads(response.text)["authToken"]
-
-    def confirmAuthToken(self, authToken):
-        data = {"deviceId": self.uuid, "authToken": authToken}
-        response = requests.post(
-            "{}/hmip/auth/confirmAuthToken".format(self.url_rest),
-            json=data,
-            headers=self.headers,
-        )
-        return json.loads(response.text)["clientId"]
+        if pin is not None:
+            headers["PIN"] = pin
+
+        data = {
+            "deviceId": self.client_id,
+            "deviceName": device_name,
+            "sgtin": access_point
+        }
+
+        return await self.connection.async_post("auth/connectionRequest", data, headers)
+
+    async def is_request_acknowledged(self) -> bool:
+        LOGGER.debug("Checking if request is acknowledged")
+        data = {
+            "deviceId": self.client_id
+        }
+
+        result = await self.connection.async_post("auth/isRequestAcknowledged", data, self.headers)
+
+        LOGGER.debug(f"Request acknowledged result: {result}")
+        return result.status == 200
+
+    async def request_auth_token(self) -> str:
+        """Request an auth token from the access point.
+        @return: The auth token"""
+        LOGGER.debug("Requesting auth token")
+        data = {"deviceId": self.client_id}
+        result = await self.connection.async_post("auth/requestAuthToken", data, self.headers)
+        LOGGER.debug(f"Request auth token result: {result}")
+
+        return result.json["authToken"]
+
+    async def confirm_auth_token(self, auth_token: str) -> str:
+        """Confirm the auth token and get the client id.
+        @param auth_token: The auth token
+        @return: The client id"""
+
+        LOGGER.debug("Confirming auth token")
+        data = {"deviceId": self.client_id, "authToken": auth_token}
+        result = await self.connection.async_post("auth/confirmAuthToken", data, self.headers)
+        LOGGER.debug(f"Confirm auth token result: {result}")
+
+        return result.json["clientId"]
```

