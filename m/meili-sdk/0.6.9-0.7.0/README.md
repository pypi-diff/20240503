# Comparing `tmp/meili-sdk-0.6.9.tar.gz` & `tmp/meili-sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili-sdk-0.6.9.tar", last modified: Tue Apr 23 18:04:07 2024, max compression
+gzip compressed data, was "meili-sdk-0.7.0.tar", last modified: Fri May  3 08:36:08 2024, max compression
```

## Comparing `meili-sdk-0.6.9.tar` & `meili-sdk-0.7.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.329956 meili-sdk-0.6.9/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5025 2024-04-23 18:04:07.329956 meili-sdk-0.6.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4735 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.319956 meili-sdk-0.6.9/meili_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.321956 meili-sdk-0.6.9/meili_sdk/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/apitoken_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/base.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/persistent_token_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/clients/sdk_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.321956 meili-sdk-0.6.9/meili_sdk/config/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/config/type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/config/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.322956 meili-sdk-0.6.9/meili_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/form.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/organization.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/ros_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/team.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.323957 meili-sdk-0.6.9/meili_sdk/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/action_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8530 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.324957 meili-sdk-0.6.9/meili_sdk/mqtt/models/
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/action.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/order.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/models/state.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/mqtt/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.325956 meili-sdk-0.6.9/meili_sdk/resources/
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/maps.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/ros.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/teams.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/users.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/resources/vehicles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.326957 meili-sdk-0.6.9/meili_sdk/schedules/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/schedules/models.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/site.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/token.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.326957 meili-sdk-0.6.9/meili_sdk/websockets/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18613 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.329956 meili-sdk-0.6.9/meili_sdk/websockets/models/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/action_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/cancel_task_message.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/docking_routine_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7135 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/move_message.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/path.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/preset.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/station.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/task_v2.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/topic.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/traffic_control_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/update_map_message.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/meili_sdk/websockets/models/vehicle_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:04:07.320957 meili-sdk-0.6.9/meili_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5025 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2285 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-23 18:04:07.000000 meili-sdk-0.6.9/meili_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-23 18:04:07.330957 meili-sdk-0.6.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-23 18:03:57.000000 meili-sdk-0.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.422376 meili-sdk-0.7.0/meili_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.425376 meili-sdk-0.7.0/meili_sdk/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/apitoken_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/persistent_token_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/sdk_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.426376 meili-sdk-0.7.0/meili_sdk/config/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/config/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/config/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.428376 meili-sdk-0.7.0/meili_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/ros_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/team.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.429376 meili-sdk-0.7.0/meili_sdk/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/action_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9679 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.430376 meili-sdk-0.7.0/meili_sdk/mqtt/models/
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/factsheet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.432376 meili-sdk-0.7.0/meili_sdk/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/ros.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/teams.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/vehicles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.433375 meili-sdk-0.7.0/meili_sdk/schedules/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/token.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.434376 meili-sdk-0.7.0/meili_sdk/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18613 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/meili_sdk/websockets/models/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/action_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/cancel_task_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/docking_routine_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/move_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/preset.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/station.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/task_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/traffic_control_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/update_map_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/vehicle_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.424376 meili-sdk-0.7.0/meili_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/setup.py
```

### Comparing `meili-sdk-0.6.9/LICENSE.txt` & `meili-sdk-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/PKG-INFO` & `meili-sdk-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.9
+Version: 0.7.0
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.9/README.md` & `meili-sdk-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/clients/__init__.py` & `meili-sdk-0.7.0/meili_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/clients/apitoken_client.py` & `meili-sdk-0.7.0/meili_sdk/clients/apitoken_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/clients/base.py` & `meili-sdk-0.7.0/meili_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/clients/sdk_client.py` & `meili-sdk-0.7.0/meili_sdk/clients/sdk_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/exceptions.py` & `meili-sdk-0.7.0/meili_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/models/base.py` & `meili-sdk-0.7.0/meili_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/models/form.py` & `meili-sdk-0.7.0/meili_sdk/models/form.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/models/task.py` & `meili-sdk-0.7.0/meili_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/models/team.py` & `meili-sdk-0.7.0/meili_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/models/trigger.py` & `meili-sdk-0.7.0/meili_sdk/models/trigger.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/models/vehicle.py` & `meili-sdk-0.7.0/meili_sdk/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/mqtt/action_client.py` & `meili-sdk-0.7.0/meili_sdk/mqtt/action_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/mqtt/client.py` & `meili-sdk-0.7.0/meili_sdk/mqtt/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from paho.mqtt.client import Client as _Client
 from paho.mqtt.client import MQTTMessage
 
 from meili_sdk.clients.persistent_token_client import PersistentTokenClient
 from meili_sdk.exceptions import MqttException, UnauthorizedMqttException
 from meili_sdk.mqtt.models.state import VDA5050StateMessage
+from meili_sdk.mqtt.models.factsheet import VDA5050FactsheetMessage
 from meili_sdk.mqtt.site import get_host
 from meili_sdk.token import get_authentication_token
 
 logger = logging.getLogger("meili_sdk")
 
 __all__ = ("MeiliMqttClient",)
 
@@ -84,14 +85,15 @@
         return cls(
             client_id=setup.mqtt_id, token=token, setup_uuid=setup_uuid, *args, *kwargs
         )
 
     def subscribe_default_topics(self, vehicle_serial_number, manufacturer = "meili"):
         self.subscribe_to_orders(vehicle_serial_number, manufacturer=manufacturer)
         self.subscribe_to_actions(vehicle_serial_number, manufacturer=manufacturer)
+        self.subscribe_to_factsheet(vehicle_serial_number, manufacturer=manufacturer)
 
     def run(self, block=False):
         try:
             self.connection_state = MqttConnectionStatus.CONNECTING
             self.client.connect(
                 self.url, port=self.port, keepalive=True, bind_address=""
             )
@@ -134,18 +136,35 @@
         elif not isinstance(message, str):
             try:
                 message = json.dumps(message)
             except (TypeError, ValueError):
                 message = str(message)
 
         self.client.publish(topic=topic, payload=message, qos=qos)
+        
+    def publish_factsheet(self, topic: str, message: any, qos=0):
+        self.__check_connection("Cannot send. Connection is closed")
+
+        if isinstance(message, VDA5050FactsheetMessage):
+            message = json.dumps(dict(message), default=str)
+        elif not isinstance(message, str):
+            try:
+                message = json.dumps(message)
+            except (TypeError, ValueError):
+                message = str(message)
+
+        self.client.publish(topic=topic, payload=message, qos=qos)
 
     def publish_to_state_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=0):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/state"
         return self.publish(topic, message, qos)
+    
+    def publish_to_factsheet_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=0):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/factsheet"
+        return self.publish_factsheet(topic, message, qos)
 
     def wait_for_connection(self, timeout=10):
         """
         Block execution until connection is established
 
         If connection is still closed after timeout provided, it will raise TimeoutError
 
@@ -170,14 +189,18 @@
     def subscribe_to_actions(self, vehicle_serial_number: str, manufacturer: str = "meili"):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/instantActions"
         return self.subscribe(topic)
 
     def subscribe_to_orders(self, vehicle_serial_number: str, manufacturer: str = "meili"):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/order"
         return self.subscribe(topic)
+    
+    def subscribe_to_factsheet(self, vehicle_serial_number: str, manufacturer: str = "meili"):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/factsheet"
+        return self.subscribe(topic)
 
     def __check_connection(self, custom_message=None):
         if not self.client.is_connected():
             raise ConnectionError(custom_message or "Connection is closed")
 
     def __on_connect(self, client: _Client, _: t.Optional[dict], flags: dict, rc: int):
         if rc != 0:
```

### Comparing `meili-sdk-0.6.9/meili_sdk/mqtt/models/action.py` & `meili-sdk-0.7.0/meili_sdk/mqtt/models/action.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/mqtt/models/order.py` & `meili-sdk-0.7.0/meili_sdk/mqtt/models/order.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/mqtt/models/state.py` & `meili-sdk-0.7.0/meili_sdk/mqtt/models/state.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/mqtt/site.py` & `meili-sdk-0.7.0/meili_sdk/mqtt/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/base.py` & `meili-sdk-0.7.0/meili_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/forms.py` & `meili-sdk-0.7.0/meili_sdk/resources/forms.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/organizations.py` & `meili-sdk-0.7.0/meili_sdk/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/tasks.py` & `meili-sdk-0.7.0/meili_sdk/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/teams.py` & `meili-sdk-0.7.0/meili_sdk/resources/teams.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/triggers.py` & `meili-sdk-0.7.0/meili_sdk/resources/triggers.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/resources/vehicles.py` & `meili-sdk-0.7.0/meili_sdk/resources/vehicles.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/schedules/loader.py` & `meili-sdk-0.7.0/meili_sdk/schedules/loader.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/schedules/models.py` & `meili-sdk-0.7.0/meili_sdk/schedules/models.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/site.py` & `meili-sdk-0.7.0/meili_sdk/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/client.py` & `meili-sdk-0.7.0/meili_sdk/websockets/client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/constants.py` & `meili-sdk-0.7.0/meili_sdk/websockets/constants.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/models/__init__.py` & `meili-sdk-0.7.0/meili_sdk/websockets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/models/message.py` & `meili-sdk-0.7.0/meili_sdk/websockets/models/message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/models/task.py` & `meili-sdk-0.7.0/meili_sdk/websockets/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/models/task_v2.py` & `meili-sdk-0.7.0/meili_sdk/websockets/models/task_v2.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/models/traffic_control_action_message.py` & `meili-sdk-0.7.0/meili_sdk/websockets/models/traffic_control_action_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk/websockets/models/update_map_message.py` & `meili-sdk-0.7.0/meili_sdk/websockets/models/update_map_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.6.9/meili_sdk.egg-info/PKG-INFO` & `meili-sdk-0.7.0/meili_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.6.9
+Version: 0.7.0
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.6.9/meili_sdk.egg-info/SOURCES.txt` & `meili-sdk-0.7.0/meili_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 meili_sdk/models/vehicle.py
 meili_sdk/mqtt/__init__.py
 meili_sdk/mqtt/action_client.py
 meili_sdk/mqtt/client.py
 meili_sdk/mqtt/site.py
 meili_sdk/mqtt/models/__init__.py
 meili_sdk/mqtt/models/action.py
+meili_sdk/mqtt/models/factsheet.py
 meili_sdk/mqtt/models/order.py
 meili_sdk/mqtt/models/state.py
 meili_sdk/resources/__init__.py
 meili_sdk/resources/base.py
 meili_sdk/resources/forms.py
 meili_sdk/resources/maps.py
 meili_sdk/resources/organizations.py
```

### Comparing `meili-sdk-0.6.9/setup.cfg` & `meili-sdk-0.7.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = meili-sdk
 description = Meili FMS SDK
-version = 0.6.9
+version = 0.7.0
 license = MIT
 license_files = LICENSE.txt
 description_file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Meili Robots
 author_email = info@meilirobots.com
```

