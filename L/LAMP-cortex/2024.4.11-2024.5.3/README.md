# Comparing `tmp/lamp_cortex-2024.4.11.tar.gz` & `tmp/lamp_cortex-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamp_cortex-2024.4.11.tar", max compression
+gzip compressed data, was "lamp_cortex-2024.5.3.tar", max compression
```

## Comparing `lamp_cortex-2024.4.11.tar` & `lamp_cortex-2024.5.3.tar`

### file list

```diff
@@ -1,76 +1,79 @@
--rw-r--r--   0        0        0     1544 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/LICENSE.md
--rw-r--r--   0        0        0     6652 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/README.md
--rw-r--r--   0        0        0      495 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/__init__.py
--rw-r--r--   0        0        0       71 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/__main__.py
--rw-r--r--   0        0        0    47767 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/feature_types.py
--rw-r--r--   0        0        0    17384 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/participant_ext.py
--rw-r--r--   0        0        0        0 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/__init__.py
--rw-r--r--   0        0        0     3313 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/acc_jerk.py
--rw-r--r--   0        0        0     5200 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/game_level_scores.py
--rw-r--r--   0        0        0     5357 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/screen_active.py
--rw-r--r--   0        0        0    16154 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/significant_locations.py
--rw-r--r--   0        0        0     5447 2024-04-11 15:37:38.286816 lamp_cortex-2024.4.11/cortex/primary/survey_scores.py
--rw-r--r--   0        0        0     3846 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/primary/trips.py
--rw-r--r--   0        0        0        0 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/__init__.py
--rw-r--r--   0        0        0     1408 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/accelerometer.py
--rw-r--r--   0        0        0     2092 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/ambient_light.py
--rw-r--r--   0        0        0     1188 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/analytics.py
--rw-r--r--   0        0        0      983 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/balloon_risk.py
--rw-r--r--   0        0        0     1286 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/bluetooth.py
--rw-r--r--   0        0        0     1216 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/calls.py
--rw-r--r--   0        0        0     1036 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/cats_and_dogs.py
--rw-r--r--   0        0        0     3537 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/device_motion.py
--rw-r--r--   0        0        0     1632 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/device_state.py
--rw-r--r--   0        0        0     1617 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/device_usage.py
--rw-r--r--   0        0        0     1304 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/gps.py
--rw-r--r--   0        0        0     1238 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/gyroscope.py
--rw-r--r--   0        0        0     1854 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/jewels_a.py
--rw-r--r--   0        0        0     1854 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/jewels_b.py
--rw-r--r--   0        0        0     1724 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/messages_usage.py
--rw-r--r--   0        0        0     1300 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/nearby_device.py
--rw-r--r--   0        0        0     1929 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/phone_usage.py
--rw-r--r--   0        0        0     1062 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/pop_the_bubbles.py
--rw-r--r--   0        0        0     1606 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/screen_state.py
--rw-r--r--   0        0        0     1338 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/sleep.py
--rw-r--r--   0        0        0      686 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/sms.py
--rw-r--r--   0        0        0     1044 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/spatial_span.py
--rw-r--r--   0        0        0     1021 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/steps.py
--rw-r--r--   0        0        0     4512 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/survey.py
--rw-r--r--   0        0        0      710 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/telephony.py
--rw-r--r--   0        0        0     2022 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/raw/visits.py
--rw-r--r--   0        0        0    10252 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/run.py
--rw-r--r--   0        0        0        0 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/__init__.py
--rw-r--r--   0        0        0     4016 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/app_time.py
--rw-r--r--   0        0        0     1674 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/call_degree.py
--rw-r--r--   0        0        0     2732 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/call_duration.py
--rw-r--r--   0        0        0     2197 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/call_number.py
--rw-r--r--   0        0        0     4076 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/data_quality.py
--rw-r--r--   0        0        0     1690 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/entropy.py
--rw-r--r--   0        0        0     1792 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/game_results.py
--rw-r--r--   0        0        0     1703 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/healthkit_sleep_duration.py
--rw-r--r--   0        0        0     1594 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/hometime.py
--rw-r--r--   0        0        0     7666 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/inactive_duration.py
--rw-r--r--   0        0        0     1473 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/nearby_device_count.py
--rw-r--r--   0        0        0     1916 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/screen_duration.py
--rw-r--r--   0        0        0     5794 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/step_count.py
--rw-r--r--   0        0        0     1360 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/survey_results.py
--rw-r--r--   0        0        0     1619 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/trip_distance.py
--rw-r--r--   0        0        0     1411 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/secondary/trip_duration.py
--rw-r--r--   0        0        0    10120 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/study_ext.py
--rw-r--r--   0        0        0        0 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/__init__.py
--rw-r--r--   0        0        0    12534 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/db.py
--rw-r--r--   0        0        0     1575 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/example_module_specs.json
--rw-r--r--   0        0        0    10467 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/example_modules.json
--rw-r--r--   0        0        0     1527 2024-04-11 15:37:38.290816 lamp_cortex-2024.4.11/cortex/utils/misc_functions.py
--rw-r--r--   0        0        0     8234 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/utils/module_scheduler.py
--rw-r--r--   0        0        0     5758 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/utils/notifications.py
--rw-r--r--   0        0        0     9435 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/utils/useful_functions.py
--rw-r--r--   0        0        0        0 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/visualizations/__init__.py
--rw-r--r--   0        0        0    13510 2024-04-11 15:37:38.294816 lamp_cortex-2024.4.11/cortex/visualizations/correlation_functions.py
--rw-r--r--   0        0        0  2385556 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/correlation_plots.ipynb
--rw-r--r--   0        0        0    19820 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/data_quality.py
--rw-r--r--   0        0        0     4137 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/example_scoring.json
--rw-r--r--   0        0        0    36829 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/participant.py
--rwxr-xr-x   0        0        0      280 2024-04-11 15:37:38.310816 lamp_cortex-2024.4.11/cortex/visualizations/run_data_quality.sh
--rw-r--r--   0        0        0     1198 2024-04-11 15:37:47.822866 lamp_cortex-2024.4.11/pyproject.toml
--rw-r--r--   0        0        0     8359 1970-01-01 00:00:00.000000 lamp_cortex-2024.4.11/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-05-03 18:05:49.511170 lamp_cortex-2024.5.3/LICENSE.md
+-rw-r--r--   0        0        0     6652 2024-05-03 18:05:49.511170 lamp_cortex-2024.5.3/README.md
+-rw-r--r--   0        0        0      495 2024-05-03 18:05:49.511170 lamp_cortex-2024.5.3/cortex/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-03 18:05:49.511170 lamp_cortex-2024.5.3/cortex/__main__.py
+-rw-r--r--   0        0        0    47767 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/feature_types.py
+-rw-r--r--   0        0        0    17384 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/participant_ext.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/__init__.py
+-rw-r--r--   0        0        0     3313 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/acc_jerk.py
+-rw-r--r--   0        0        0     5200 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/game_level_scores.py
+-rw-r--r--   0        0        0     5357 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/screen_active.py
+-rw-r--r--   0        0        0    16154 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/significant_locations.py
+-rw-r--r--   0        0        0     5447 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/survey_scores.py
+-rw-r--r--   0        0        0     3846 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/primary/trips.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/__init__.py
+-rw-r--r--   0        0        0     1408 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/accelerometer.py
+-rw-r--r--   0        0        0     2092 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/ambient_light.py
+-rw-r--r--   0        0        0     1188 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/analytics.py
+-rw-r--r--   0        0        0      983 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/balloon_risk.py
+-rw-r--r--   0        0        0     1286 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/bluetooth.py
+-rw-r--r--   0        0        0     1216 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/calls.py
+-rw-r--r--   0        0        0     1036 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/cats_and_dogs.py
+-rw-r--r--   0        0        0     3537 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/device_motion.py
+-rw-r--r--   0        0        0     1632 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/device_state.py
+-rw-r--r--   0        0        0     1617 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/device_usage.py
+-rw-r--r--   0        0        0     1304 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/gps.py
+-rw-r--r--   0        0        0     1238 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/gyroscope.py
+-rw-r--r--   0        0        0     1854 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/jewels_a.py
+-rw-r--r--   0        0        0     1854 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/jewels_b.py
+-rw-r--r--   0        0        0     1724 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/messages_usage.py
+-rw-r--r--   0        0        0     1300 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/nearby_device.py
+-rw-r--r--   0        0        0     1929 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/phone_usage.py
+-rw-r--r--   0        0        0     1062 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/pop_the_bubbles.py
+-rw-r--r--   0        0        0     1606 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/screen_state.py
+-rw-r--r--   0        0        0     1338 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/sleep.py
+-rw-r--r--   0        0        0      686 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/sms.py
+-rw-r--r--   0        0        0     1044 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/spatial_span.py
+-rw-r--r--   0        0        0     1021 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/steps.py
+-rw-r--r--   0        0        0     4512 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/survey.py
+-rw-r--r--   0        0        0      710 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/telephony.py
+-rw-r--r--   0        0        0     2022 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/raw/visits.py
+-rw-r--r--   0        0        0    10252 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/run.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/__init__.py
+-rw-r--r--   0        0        0     4081 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/app_time.py
+-rw-r--r--   0        0        0     1674 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/call_degree.py
+-rw-r--r--   0        0        0     2732 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/call_duration.py
+-rw-r--r--   0        0        0     2154 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/call_number.py
+-rw-r--r--   0        0        0     4076 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/data_quality.py
+-rw-r--r--   0        0        0     1690 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/entropy.py
+-rw-r--r--   0        0        0     1792 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/game_results.py
+-rw-r--r--   0        0        0     1703 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/healthkit_sleep_duration.py
+-rw-r--r--   0        0        0     1594 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/hometime.py
+-rw-r--r--   0        0        0     7666 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/inactive_duration.py
+-rw-r--r--   0        0        0     1473 2024-05-03 18:05:49.515170 lamp_cortex-2024.5.3/cortex/secondary/nearby_device_count.py
+-rw-r--r--   0        0        0     1916 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/screen_duration.py
+-rw-r--r--   0        0        0     5794 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/step_count.py
+-rw-r--r--   0        0        0     1360 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/survey_results.py
+-rw-r--r--   0        0        0     1318 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/text_degree.py
+-rw-r--r--   0        0        0     1910 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/text_number.py
+-rw-r--r--   0        0        0     1619 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/trip_distance.py
+-rw-r--r--   0        0        0     1411 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/trip_duration.py
+-rw-r--r--   0        0        0     1904 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/secondary/visit_time.py
+-rw-r--r--   0        0        0    10120 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/study_ext.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/__init__.py
+-rw-r--r--   0        0        0    12534 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/db.py
+-rw-r--r--   0        0        0     1575 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/example_module_specs.json
+-rw-r--r--   0        0        0    10467 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/example_modules.json
+-rw-r--r--   0        0        0     1527 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/misc_functions.py
+-rw-r--r--   0        0        0     8234 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/module_scheduler.py
+-rw-r--r--   0        0        0     5758 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/notifications.py
+-rw-r--r--   0        0        0     9435 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/utils/useful_functions.py
+-rw-r--r--   0        0        0        0 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/visualizations/__init__.py
+-rw-r--r--   0        0        0    13510 2024-05-03 18:05:49.519170 lamp_cortex-2024.5.3/cortex/visualizations/correlation_functions.py
+-rw-r--r--   0        0        0  2385556 2024-05-03 18:05:49.535170 lamp_cortex-2024.5.3/cortex/visualizations/correlation_plots.ipynb
+-rw-r--r--   0        0        0    19820 2024-05-03 18:05:49.535170 lamp_cortex-2024.5.3/cortex/visualizations/data_quality.py
+-rw-r--r--   0        0        0     4137 2024-05-03 18:05:49.535170 lamp_cortex-2024.5.3/cortex/visualizations/example_scoring.json
+-rw-r--r--   0        0        0    36829 2024-05-03 18:05:49.535170 lamp_cortex-2024.5.3/cortex/visualizations/participant.py
+-rwxr-xr-x   0        0        0      280 2024-05-03 18:05:49.535170 lamp_cortex-2024.5.3/cortex/visualizations/run_data_quality.sh
+-rw-r--r--   0        0        0     1197 2024-05-03 18:06:03.711366 lamp_cortex-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0     8358 1970-01-01 00:00:00.000000 lamp_cortex-2024.5.3/PKG-INFO
```

### Comparing `lamp_cortex-2024.4.11/LICENSE.md` & `lamp_cortex-2024.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/README.md` & `lamp_cortex-2024.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/feature_types.py` & `lamp_cortex-2024.5.3/cortex/feature_types.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/participant_ext.py` & `lamp_cortex-2024.5.3/cortex/participant_ext.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/primary/acc_jerk.py` & `lamp_cortex-2024.5.3/cortex/primary/acc_jerk.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/primary/game_level_scores.py` & `lamp_cortex-2024.5.3/cortex/primary/game_level_scores.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/primary/screen_active.py` & `lamp_cortex-2024.5.3/cortex/primary/screen_active.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/primary/significant_locations.py` & `lamp_cortex-2024.5.3/cortex/primary/significant_locations.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/primary/survey_scores.py` & `lamp_cortex-2024.5.3/cortex/primary/survey_scores.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/primary/trips.py` & `lamp_cortex-2024.5.3/cortex/primary/trips.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/accelerometer.py` & `lamp_cortex-2024.5.3/cortex/raw/accelerometer.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/ambient_light.py` & `lamp_cortex-2024.5.3/cortex/raw/ambient_light.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/analytics.py` & `lamp_cortex-2024.5.3/cortex/raw/analytics.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/balloon_risk.py` & `lamp_cortex-2024.5.3/cortex/raw/balloon_risk.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/bluetooth.py` & `lamp_cortex-2024.5.3/cortex/raw/bluetooth.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/calls.py` & `lamp_cortex-2024.5.3/cortex/raw/calls.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/cats_and_dogs.py` & `lamp_cortex-2024.5.3/cortex/raw/cats_and_dogs.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/device_motion.py` & `lamp_cortex-2024.5.3/cortex/raw/device_motion.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/device_state.py` & `lamp_cortex-2024.5.3/cortex/raw/device_state.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/device_usage.py` & `lamp_cortex-2024.5.3/cortex/raw/device_usage.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/gps.py` & `lamp_cortex-2024.5.3/cortex/raw/gps.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/gyroscope.py` & `lamp_cortex-2024.5.3/cortex/raw/gyroscope.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/jewels_a.py` & `lamp_cortex-2024.5.3/cortex/raw/jewels_a.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/jewels_b.py` & `lamp_cortex-2024.5.3/cortex/raw/jewels_b.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/messages_usage.py` & `lamp_cortex-2024.5.3/cortex/raw/messages_usage.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/nearby_device.py` & `lamp_cortex-2024.5.3/cortex/raw/nearby_device.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/phone_usage.py` & `lamp_cortex-2024.5.3/cortex/raw/phone_usage.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/pop_the_bubbles.py` & `lamp_cortex-2024.5.3/cortex/raw/pop_the_bubbles.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/screen_state.py` & `lamp_cortex-2024.5.3/cortex/raw/screen_state.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/sleep.py` & `lamp_cortex-2024.5.3/cortex/raw/sleep.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/sms.py` & `lamp_cortex-2024.5.3/cortex/raw/sms.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/spatial_span.py` & `lamp_cortex-2024.5.3/cortex/raw/spatial_span.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/steps.py` & `lamp_cortex-2024.5.3/cortex/raw/steps.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/survey.py` & `lamp_cortex-2024.5.3/cortex/raw/survey.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/telephony.py` & `lamp_cortex-2024.5.3/cortex/raw/telephony.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/raw/visits.py` & `lamp_cortex-2024.5.3/cortex/raw/visits.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/run.py` & `lamp_cortex-2024.5.3/cortex/run.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/app_time.py` & `lamp_cortex-2024.5.3/cortex/secondary/app_time.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..raw.device_usage import device_usage
 from .. import raw
 
 @secondary_feature(
     name="cortex.app_time",
     dependencies=[device_usage]
 )
-def app_time(category=None, attach=False, **kwargs):
+def app_time(category="all", attach=False, **kwargs):
     """ Get app usage data from raw device_usage.
 
     Args:
         **kwargs:
             id (string): The participant's LAMP id. Required.
             start (int): The initial UNIX timestamp (in ms) of the window for which the feature
                 is being generated. Required.
@@ -52,34 +52,32 @@
                     "social": "SRDeviceUsageCategorySocialNetworking",
                     "sports": "SRDeviceUsageCategorySports",
                     "stickers": "SRDeviceUsageCategoryStickers",
                     "travel": "SRDeviceUsageCategoryTravel",
                     "utilities": "SRDeviceUsageCategoryUtilities",
                     "weather": "SRDeviceUsageCategoryWeather"}
     
-    if (category is None) or category not in category_map.keys():
-        raise Exception("Please specify the argument 'category' as one of: %s" % list(category_map.keys()))
+    if category != "all" and category not in category_map.keys():
+        raise Exception("Please specify the argument 'category' as either 'all' or one of: %s" % list(category_map.keys()))
     
     _device_usage = device_usage(**kwargs)['data']
     
     if len(_device_usage) == 0:
         return {'timestamp': kwargs['start'], 'value': None}
-    
-    category_id = category_map[category]
         
     app_usage = [f['applicationUsageByCategory'] for f in _device_usage
                  if len(f['applicationUsageByCategory']) > 0]
     
-    type_usage = [f[category_id] for f in app_usage if category_id in f.keys()]
-    
-    usage_list = []
-    for element in type_usage:
-        usage_list += [f for f in element]
+    if category == 'all':
+        type_usage = [f[j] for f in app_usage for j in category_map.values() if j in f.keys()]
+    else:
+        category_id = category_map[category]
+        type_usage = [f[category_id] for f in app_usage if category_id in f.keys()]
     
-    value = np.sum([f['usageTime'] for f in usage_list])
+    value = np.sum(dur['usageTime'] for f in type_usage for dur in f)
     
     # After this time, data was reported in ms, not s. Change the unit from s to ms if data was collected before this time.
     cutoff_time = 1677088485*1000
     if kwargs['end'] <= cutoff_time:
         value *= 1000
     
     return {'timestamp': kwargs['start'], 'value': value}
```

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/call_degree.py` & `lamp_cortex-2024.5.3/cortex/secondary/call_degree.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/call_duration.py` & `lamp_cortex-2024.5.3/cortex/secondary/call_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/call_number.py` & `lamp_cortex-2024.5.3/cortex/secondary/call_number.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,12 +52,11 @@
     elif call_direction in ("incoming", "outgoing"):
 
         group = [calls for calls in _calls if calls['type'] == call_direction]
         number = len(group)
 
     else:
         number = None
-        log.info(""" %s was passed but is not an acceptable argument.
-        Acceptable arguments include 'all','incoming', or 'outgoing'" """,
-                 call_direction)
+        raise Exception(f"{call_direction} is not a proper argument. "
+                        + "Must be incoming, outgoing, or all")
 
     return {'timestamp': kwargs['start'], 'value': number}
```

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/data_quality.py` & `lamp_cortex-2024.5.3/cortex/secondary/data_quality.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/entropy.py` & `lamp_cortex-2024.5.3/cortex/secondary/entropy.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/game_results.py` & `lamp_cortex-2024.5.3/cortex/secondary/game_results.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/healthkit_sleep_duration.py` & `lamp_cortex-2024.5.3/cortex/secondary/healthkit_sleep_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/hometime.py` & `lamp_cortex-2024.5.3/cortex/secondary/hometime.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/inactive_duration.py` & `lamp_cortex-2024.5.3/cortex/secondary/inactive_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/nearby_device_count.py` & `lamp_cortex-2024.5.3/cortex/secondary/nearby_device_count.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/screen_duration.py` & `lamp_cortex-2024.5.3/cortex/secondary/screen_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/step_count.py` & `lamp_cortex-2024.5.3/cortex/secondary/step_count.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/survey_results.py` & `lamp_cortex-2024.5.3/cortex/secondary/survey_results.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/trip_distance.py` & `lamp_cortex-2024.5.3/cortex/secondary/trip_distance.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/secondary/trip_duration.py` & `lamp_cortex-2024.5.3/cortex/secondary/trip_duration.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/study_ext.py` & `lamp_cortex-2024.5.3/cortex/study_ext.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/db.py` & `lamp_cortex-2024.5.3/cortex/utils/db.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/example_module_specs.json` & `lamp_cortex-2024.5.3/cortex/utils/example_module_specs.json`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/example_modules.json` & `lamp_cortex-2024.5.3/cortex/utils/example_modules.json`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/misc_functions.py` & `lamp_cortex-2024.5.3/cortex/utils/misc_functions.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/module_scheduler.py` & `lamp_cortex-2024.5.3/cortex/utils/module_scheduler.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/notifications.py` & `lamp_cortex-2024.5.3/cortex/utils/notifications.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/utils/useful_functions.py` & `lamp_cortex-2024.5.3/cortex/utils/useful_functions.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/visualizations/correlation_functions.py` & `lamp_cortex-2024.5.3/cortex/visualizations/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/visualizations/correlation_plots.ipynb` & `lamp_cortex-2024.5.3/cortex/visualizations/correlation_plots.ipynb`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/visualizations/data_quality.py` & `lamp_cortex-2024.5.3/cortex/visualizations/data_quality.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/visualizations/example_scoring.json` & `lamp_cortex-2024.5.3/cortex/visualizations/example_scoring.json`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/cortex/visualizations/participant.py` & `lamp_cortex-2024.5.3/cortex/visualizations/participant.py`

 * *Files identical despite different names*

### Comparing `lamp_cortex-2024.4.11/pyproject.toml` & `lamp_cortex-2024.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LAMP-cortex"
-version = "2024.4.11"
+version = "2024.5.3"
 license = "BSD-3-Clause"
 description = "The Cortex data analysis toolkit for the LAMP Platform."
 authors = ["Division of Digital Psychiatry at Beth Israel Deaconess Medical Center <team@digitalpsych.org>"]
 readme = "README.md"
 homepage = "https://docs.lamp.digital"
 documentation = "https://docs.lamp.digital"
 repository = "https://github.com/BIDMCDigitalPsychiatry/LAMP-cortex"
```

### Comparing `lamp_cortex-2024.4.11/PKG-INFO` & `lamp_cortex-2024.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LAMP-cortex
-Version: 2024.4.11
+Version: 2024.5.3
 Summary: The Cortex data analysis toolkit for the LAMP Platform.
 Home-page: https://docs.lamp.digital
 License: BSD-3-Clause
 Keywords: LAMP Cortex
 Author: Division of Digital Psychiatry at Beth Israel Deaconess Medical Center
 Author-email: team@digitalpsych.org
 Requires-Python: >=3.8,<4.0
```

