# Comparing `tmp/weconnect-cupra-daern-0.50.8.tar.gz` & `tmp/weconnect-cupra-daern-0.50.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weconnect-cupra-daern-0.50.8.tar", last modified: Thu Jan  4 18:38:13 2024, max compression
+gzip compressed data, was "weconnect-cupra-daern-0.50.9.tar", last modified: Fri May  3 19:05:37 2024, max compression
```

## Comparing `weconnect-cupra-daern-0.50.8.tar` & `weconnect-cupra-daern-0.50.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.589690 weconnect-cupra-daern-0.50.8/
--rw-rw-r--   0 daern     (1000) daern     (1000)     1071 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/LICENSE
--rw-rw-r--   0 daern     (1000) daern     (1000)       51 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/MANIFEST.in
--rw-rw-r--   0 daern     (1000) daern     (1000)     4786 2024-01-04 18:38:13.589690 weconnect-cupra-daern-0.50.8/PKG-INFO
--rw-rw-r--   0 daern     (1000) daern     (1000)     3613 2023-06-07 21:18:32.000000 weconnect-cupra-daern-0.50.8/README.md
--rw-rw-r--   0 daern     (1000) daern     (1000)     3004 2024-01-04 18:38:13.589690 weconnect-cupra-daern-0.50.8/setup.cfg
--rw-rw-r--   0 daern     (1000) daern     (1000)     2053 2023-06-07 19:53:45.000000 weconnect-cupra-daern-0.50.8/setup.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.577689 weconnect-cupra-daern-0.50.8/tests/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/tests/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     8774 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/tests/test_addressable.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    13494 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/tests/test_cupra.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     1002 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/tests/test_elements.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.577689 weconnect-cupra-daern-0.50.8/weconnect_cupra/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)       24 2024-01-04 18:37:01.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/__version.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    25444 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/addressable.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.577689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/__init__.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.577689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3951 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/api.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.577689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/auth/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/auth/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    17254 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/auth/my_cupra_session.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      384 2023-06-12 20:54:47.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/domain.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.581689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    13968 2023-07-31 16:17:24.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/access_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2688 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/battery_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     4507 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/charging_settings.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    14455 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/charging_station.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7754 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/charging_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     8582 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/climatization_settings.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2786 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/climatization_status.py
--rwxr--r--   0 daern     (1000) daern     (1000)     1171 2023-06-12 21:35:19.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/connection_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    12348 2023-10-31 21:16:30.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/controls.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2246 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/engine_state.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      802 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/enums.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3442 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/error.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3399 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/generic_capability.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     5296 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/generic_settings.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.581689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/helpers/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/helpers/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3516 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/helpers/request_tracker.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2253 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/odometer_measurement.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     1518 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/parking_position.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    22925 2024-01-04 18:37:09.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/vehicle.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.581689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7704 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/api.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.581689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/auth/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/auth/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    16467 2023-06-07 19:53:10.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/auth/we_charge_session.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    17807 2023-06-07 19:53:10.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/auth/we_connect_session.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      659 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/domain.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.585689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    10033 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/access_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2461 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/battery_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     1994 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/capability_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3710 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charge_mode.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    11823 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_profiles.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     4319 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_settings.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    19163 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_station.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7719 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     8103 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/climatization_settings.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2886 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/climatization_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2715 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/climatization_timer.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     9456 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/controls.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      568 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/enums.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3403 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/generic_capability.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2101 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/generic_request_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3140 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/generic_settings.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.585689 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/helpers/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/helpers/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3510 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/helpers/request_tracker.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3349 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/lights_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     1657 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/lv_battery_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3778 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/maintenance_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2337 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/odometer_measurement.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     1679 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/parking_position.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     1628 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/range_measurements.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     5096 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/range_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     6720 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/readiness_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7645 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/timer.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    46375 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/vehicle.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7987 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/warning_lights_status.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.585689 weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      142 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/auth_util.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7252 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/openid_session.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3137 2023-06-07 19:46:42.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/session_manager.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      238 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/vw_web_session.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.585689 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/
--rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/__init__.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      880 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/access_control_state.py
--rwxr--r--   0 daern     (1000) daern     (1000)      141 2023-06-12 21:35:26.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/connection_state.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      927 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/control_operation.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3444 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/error.py
--rw-rw-r--   0 daern     (1000) daern     (1000)    10163 2023-07-31 15:03:30.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/generic_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3455 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/plug_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     3836 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/window_heating_status.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     2356 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/errors.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     7417 2023-06-07 19:37:35.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/fetch.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      182 2023-06-07 19:45:56.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/service.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     4330 2023-07-31 14:49:34.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/util.py
--rw-rw-r--   0 daern     (1000) daern     (1000)     9137 2023-06-07 20:09:50.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/weconnect_cupra.py
--rw-rw-r--   0 daern     (1000) daern     (1000)      184 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra/weconnect_errors.py
-drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-01-04 18:38:13.589690 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/
--rw-rw-r--   0 daern     (1000) daern     (1000)     4786 2024-01-04 18:38:13.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/PKG-INFO
--rw-rw-r--   0 daern     (1000) daern     (1000)     4271 2024-01-04 18:38:13.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/SOURCES.txt
--rw-rw-r--   0 daern     (1000) daern     (1000)        1 2024-01-04 18:38:13.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/dependency_links.txt
--rw-rw-r--   0 daern     (1000) daern     (1000)        1 2023-06-07 20:04:08.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/not-zip-safe
--rw-rw-r--   0 daern     (1000) daern     (1000)       77 2024-01-04 18:38:13.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/requires.txt
--rw-rw-r--   0 daern     (1000) daern     (1000)       22 2024-01-04 18:38:13.000000 weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/top_level.txt
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.270229 weconnect-cupra-daern-0.50.9/
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1071 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/LICENSE
+-rw-rw-r--   0 daern     (1000) daern     (1000)       51 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/MANIFEST.in
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4786 2024-05-03 19:05:37.270229 weconnect-cupra-daern-0.50.9/PKG-INFO
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3613 2023-06-07 21:18:32.000000 weconnect-cupra-daern-0.50.9/README.md
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3004 2024-05-03 19:05:37.270229 weconnect-cupra-daern-0.50.9/setup.cfg
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2053 2023-06-07 19:53:45.000000 weconnect-cupra-daern-0.50.9/setup.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.242228 weconnect-cupra-daern-0.50.9/tests/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/tests/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     8774 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/tests/test_addressable.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    13494 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/tests/test_cupra.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1002 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/tests/test_elements.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.246228 weconnect-cupra-daern-0.50.9/weconnect_cupra/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)       24 2024-05-03 19:04:56.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/__version.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    25444 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/addressable.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.246228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/__init__.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.246228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3951 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/api.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.246228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/auth/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/auth/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    17254 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/auth/my_cupra_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      384 2023-06-12 20:54:47.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/domain.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.254228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    13968 2023-07-31 16:17:24.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/access_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2688 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/battery_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4507 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/charging_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    14455 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/charging_station.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7754 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/charging_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     8582 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/climatization_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2786 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/climatization_status.py
+-rwxr--r--   0 daern     (1000) daern     (1000)     1171 2023-06-12 21:35:19.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/connection_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    12325 2024-05-03 19:03:53.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/controls.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2246 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/engine_state.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      802 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/enums.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3442 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/error.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3399 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/generic_capability.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     5296 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/generic_settings.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.254228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/helpers/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/helpers/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3516 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/helpers/request_tracker.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2253 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/odometer_measurement.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1518 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/parking_position.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    22925 2024-01-04 18:37:09.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/vehicle.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.254228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7704 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/api.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.254228 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/auth/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/auth/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    16467 2023-06-07 19:53:10.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/auth/we_charge_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    17807 2023-06-07 19:53:10.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/auth/we_connect_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      659 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/domain.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.262229 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    10033 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/access_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2461 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/battery_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1994 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/capability_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3710 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charge_mode.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    11823 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_profiles.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4319 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    19163 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_station.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7719 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     8103 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/climatization_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2886 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/climatization_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2715 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/climatization_timer.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     9456 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/controls.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      568 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/enums.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3403 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/generic_capability.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2101 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/generic_request_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3140 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/generic_settings.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.266229 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/helpers/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/helpers/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3510 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/helpers/request_tracker.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3349 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/lights_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1657 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/lv_battery_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3778 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/maintenance_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2337 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/odometer_measurement.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1679 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/parking_position.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1628 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/range_measurements.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     5096 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/range_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     6720 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/readiness_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7645 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/timer.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    46375 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/vehicle.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7987 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/warning_lights_status.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.266229 weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      142 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/auth_util.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7252 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/openid_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3137 2023-06-07 19:46:42.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/session_manager.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      238 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/vw_web_session.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.266229 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      880 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/access_control_state.py
+-rwxr--r--   0 daern     (1000) daern     (1000)      141 2023-06-12 21:35:26.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/connection_state.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      927 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/control_operation.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3444 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/error.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    10163 2023-07-31 15:03:30.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/generic_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3455 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/plug_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3836 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/window_heating_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2356 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/errors.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7417 2023-06-07 19:37:35.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/fetch.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      182 2023-06-07 19:45:56.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/service.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4330 2023-07-31 14:49:34.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/util.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     9137 2023-06-07 20:09:50.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/weconnect_cupra.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      184 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra/weconnect_errors.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2024-05-03 19:05:37.270229 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4786 2024-05-03 19:05:37.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/PKG-INFO
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4271 2024-05-03 19:05:37.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/SOURCES.txt
+-rw-rw-r--   0 daern     (1000) daern     (1000)        1 2024-05-03 19:05:37.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/dependency_links.txt
+-rw-rw-r--   0 daern     (1000) daern     (1000)        1 2023-06-07 20:04:08.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/not-zip-safe
+-rw-rw-r--   0 daern     (1000) daern     (1000)       77 2024-05-03 19:05:37.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/requires.txt
+-rw-rw-r--   0 daern     (1000) daern     (1000)       22 2024-05-03 19:05:37.000000 weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/top_level.txt
```

### Comparing `weconnect-cupra-daern-0.50.8/LICENSE` & `weconnect-cupra-daern-0.50.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/PKG-INFO` & `weconnect-cupra-daern-0.50.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-cupra-daern
-Version: 0.50.8
+Version: 0.50.9
 Summary: Python API for the Cupra Born online services
 Home-page: https://github.com/daernsinstantfortress/WeConnect-Cupra-python
 Author: Till Steinbach / Alan Gibson / Stuart Hall
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/tillsteinbach
 Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-Cupra-python
 Project-URL: Bug Tracker, https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues
```

### Comparing `weconnect-cupra-daern-0.50.8/README.md` & `weconnect-cupra-daern-0.50.9/README.md`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/setup.cfg` & `weconnect-cupra-daern-0.50.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/setup.py` & `weconnect-cupra-daern-0.50.9/setup.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/tests/test_addressable.py` & `weconnect-cupra-daern-0.50.9/tests/test_addressable.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/tests/test_cupra.py` & `weconnect-cupra-daern-0.50.9/tests/test_cupra.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/tests/test_elements.py` & `weconnect-cupra-daern-0.50.9/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/addressable.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/addressable.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/api.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/api.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/auth/my_cupra_session.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/auth/my_cupra_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/access_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/access_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/battery_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/battery_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/charging_settings.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/charging_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/charging_station.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/charging_station.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/charging_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/charging_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/climatization_settings.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/climatization_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/climatization_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/climatization_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/connection_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/connection_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/controls.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/controls.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,14 @@
         # Validate inputs
         if value not in [ControlOperation.START, ControlOperation.STOP]:
             return
         
         # Do API request
         controlResponse = self.vehicle.fetcher.post(
             url=f'https://ola.prod.code.seat.cloud.vwgroup.com/vehicles/{self.vehicle.vin.value}/charging/requests/{value.value}',
-            data='{}',
             allow_redirects=True,
             headers={
                 "accept": '*/*',
                 "user-agent": "CUPRAApp%20-%20Store/20220207 CFNetwork/1240.0.4 Darwin/20.6.0",
                 "Content-Type": "application/json",
                 "accept-language": "de-de",
                 "Accept-Encoding": "gzip, deflate"
```

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/engine_state.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/engine_state.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/enums.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/enums.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/error.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/error.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/generic_capability.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/generic_capability.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/generic_settings.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/generic_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/helpers/request_tracker.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/helpers/request_tracker.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/odometer_measurement.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/odometer_measurement.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/parking_position.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/parking_position.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/cupra/elements/vehicle.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/cupra/elements/vehicle.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/api.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/api.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/auth/we_charge_session.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/auth/we_charge_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/auth/we_connect_session.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/auth/we_connect_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/domain.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/domain.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/access_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/access_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/battery_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/battery_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/capability_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/capability_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charge_mode.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charge_mode.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_profiles.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_profiles.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_settings.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_station.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_station.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/charging_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/charging_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/climatization_settings.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/climatization_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/climatization_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/climatization_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/climatization_timer.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/climatization_timer.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/controls.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/controls.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/enums.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/enums.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/generic_capability.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/generic_capability.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/generic_request_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/generic_request_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/generic_settings.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/generic_settings.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/helpers/request_tracker.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/helpers/request_tracker.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/lights_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/lights_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/lv_battery_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/lv_battery_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/maintenance_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/maintenance_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/odometer_measurement.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/odometer_measurement.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/parking_position.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/parking_position.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/range_measurements.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/range_measurements.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/range_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/range_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/readiness_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/readiness_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/timer.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/timer.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/vehicle.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/vehicle.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/api/vw/elements/warning_lights_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/api/vw/elements/warning_lights_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/openid_session.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/openid_session.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/auth/session_manager.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/auth/session_manager.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/access_control_state.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/access_control_state.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/control_operation.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/control_operation.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/error.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/error.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/generic_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/generic_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/plug_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/plug_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/elements/window_heating_status.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/elements/window_heating_status.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/errors.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/errors.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/fetch.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/fetch.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/util.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/util.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra/weconnect_cupra.py` & `weconnect-cupra-daern-0.50.9/weconnect_cupra/weconnect_cupra.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/PKG-INFO` & `weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-cupra-daern
-Version: 0.50.8
+Version: 0.50.9
 Summary: Python API for the Cupra Born online services
 Home-page: https://github.com/daernsinstantfortress/WeConnect-Cupra-python
 Author: Till Steinbach / Alan Gibson / Stuart Hall
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/tillsteinbach
 Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-Cupra-python
 Project-URL: Bug Tracker, https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues
```

### Comparing `weconnect-cupra-daern-0.50.8/weconnect_cupra_daern.egg-info/SOURCES.txt` & `weconnect-cupra-daern-0.50.9/weconnect_cupra_daern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

