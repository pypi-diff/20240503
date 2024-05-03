# Comparing `tmp/vital-2.1.3.tar.gz` & `tmp/vital-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-2.1.3.tar", max compression
+gzip compressed data, was "vital-2.1.4.tar", max compression
```

## Comparing `vital-2.1.3.tar` & `vital-2.1.4.tar`

### file list

```diff
@@ -1,276 +1,282 @@
--rw-r--r--   0        0        0     3329 2024-04-12 14:15:53.169242 vital-2.1.3/README.md
--rw-r--r--   0        0        0      396 2024-04-12 14:15:53.169242 vital-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    14365 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/__init__.py
--rw-r--r--   0        0        0     5248 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/client.py
--rw-r--r--   0        0        0      519 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/core/api_error.py
--rw-r--r--   0        0        0     1080 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      308 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/environment.py
--rw-r--r--   0        0        0      236 2024-04-12 14:15:53.169242 vital-2.1.3/src/vital/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/errors/bad_request_error.py
--rw-r--r--   0        0        0      313 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/py.typed
--rw-r--r--   0        0        0      532 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/activity/__init__.py
--rw-r--r--   0        0        0     8604 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/activity/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/body/__init__.py
--rw-r--r--   0        0        0     8520 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/body/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/devices/__init__.py
--rw-r--r--   0        0        0     3641 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/devices/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/insurance/__init__.py
--rw-r--r--   0        0        0     6695 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/insurance/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/introspect/__init__.py
--rw-r--r--   0        0        0     8197 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/introspect/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/lab_tests/__init__.py
--rw-r--r--   0        0        0    67299 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/lab_tests/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/link/__init__.py
--rw-r--r--   0        0        0    44285 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/link/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/meal/__init__.py
--rw-r--r--   0        0        0     4703 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/meal/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/profile/__init__.py
--rw-r--r--   0        0        0     5698 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/profile/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/providers/__init__.py
--rw-r--r--   0        0        0     2668 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/providers/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/sleep/__init__.py
--rw-r--r--   0        0        0    15040 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/sleep/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/team/__init__.py
--rw-r--r--   0        0        0    18010 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/team/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/testkit/__init__.py
--rw-r--r--   0        0        0     8435 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/testkit/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/user/__init__.py
--rw-r--r--   0        0        0    36394 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/user/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/vitals/__init__.py
--rw-r--r--   0        0        0   209296 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/vitals/client.py
--rw-r--r--   0        0        0       65 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/workouts/__init__.py
--rw-r--r--   0        0        0    11221 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/resources/workouts/client.py
--rw-r--r--   0        0        0    20943 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/__init__.py
--rw-r--r--   0        0        0     1103 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/activity_v_2_in_db.py
--rw-r--r--   0        0        0      967 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/address.py
--rw-r--r--   0        0        0      971 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/appointment_availability_slots.py
--rw-r--r--   0        0        0     1074 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/appointment_event_status.py
--rw-r--r--   0        0        0      748 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/appointment_provider.py
--rw-r--r--   0        0        0      661 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/appointment_service_type.py
--rw-r--r--   0        0        0     1044 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/appointment_status.py
--rw-r--r--   0        0        0      149 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/appointment_type.py
--rw-r--r--   0        0        0      957 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/area_info.py
--rw-r--r--   0        0        0      510 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/attempt_status.py
--rw-r--r--   0        0        0      649 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/auth_type.py
--rw-r--r--   0        0        0     1468 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/biomarker_result.py
--rw-r--r--   0        0        0     1168 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/body_v_2_in_db.py
--rw-r--r--   0        0        0      970 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_activity_response.py
--rw-r--r--   0        0        0      950 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_body_response.py
--rw-r--r--   0        0        0     3581 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_activity.py
--rw-r--r--   0        0        0     1010 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_api_key.py
--rw-r--r--   0        0        0     1815 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_appointment.py
--rw-r--r--   0        0        0      934 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_appointment_cancellation_reason.py
--rw-r--r--   0        0        0     1051 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_appointment_event.py
--rw-r--r--   0        0        0     1193 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_at_home_phlebotomy_order.py
--rw-r--r--   0        0        0     1030 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_at_home_phlebotomy_order_details.py
--rw-r--r--   0        0        0     1634 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_blood_oxygen_timeseries.py
--rw-r--r--   0        0        0     1632 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_blood_pressure_timeseries.py
--rw-r--r--   0        0        0     1637 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_body.py
--rw-r--r--   0        0        0     1631 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_body_fat_timeseries.py
--rw-r--r--   0        0        0     1630 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_body_weight_timeseries.py
--rw-r--r--   0        0        0     1859 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_caffeine_timeseries.py
--rw-r--r--   0        0        0     1919 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_calories_active_timeseries.py
--rw-r--r--   0        0        0     1658 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_calories_basal_timeseries.py
--rw-r--r--   0        0        0     1623 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_cholesterol_timeseries.py
--rw-r--r--   0        0        0     1071 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_diagnosis_information.py
--rw-r--r--   0        0        0     1874 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_distance_timeseries.py
--rw-r--r--   0        0        0     1540 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py
--rw-r--r--   0        0        0     1656 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_floors_climbed_timeseries.py
--rw-r--r--   0        0        0     1048 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_food.py
--rw-r--r--   0        0        0     1619 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_glucose_timeseries.py
--rw-r--r--   0        0        0     1236 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_heart_rate.py
--rw-r--r--   0        0        0     1606 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_heart_rate_timeseries.py
--rw-r--r--   0        0        0     1624 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_hrv_timeseries.py
--rw-r--r--   0        0        0     1968 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_hypnogram_timeseries.py
--rw-r--r--   0        0        0     1612 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_ige_timeseries.py
--rw-r--r--   0        0        0     1612 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_igg_timeseries.py
--rw-r--r--   0        0        0     1183 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_lab.py
--rw-r--r--   0        0        0     1780 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_lab_test.py
--rw-r--r--   0        0        0      945 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_loinc.py
--rw-r--r--   0        0        0     1147 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_marker.py
--rw-r--r--   0        0        0     1262 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_marker_complete.py
--rw-r--r--   0        0        0     1003 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_meal_response.py
--rw-r--r--   0        0        0     1861 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_mindfulness_minutes_timeseries.py
--rw-r--r--   0        0        0     3286 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_order.py
--rw-r--r--   0        0        0     1311 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_order_details.py
--rw-r--r--   0        0        0      967 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_order_event.py
--rw-r--r--   0        0        0     1060 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_patient_details_compatible.py
--rw-r--r--   0        0        0     1239 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_payor_search_response.py
--rw-r--r--   0        0        0      916 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_physician.py
--rw-r--r--   0        0        0     1210 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_profile.py
--rw-r--r--   0        0        0     1164 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_provider.py
--rw-r--r--   0        0        0     1418 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_provider_detailed.py
--rw-r--r--   0        0        0     1180 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_provider_with_status.py
--rw-r--r--   0        0        0     6046 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_resource.py
--rw-r--r--   0        0        0     1639 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_respiratory_rate_timeseries.py
--rw-r--r--   0        0        0     1088 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_result.py
--rw-r--r--   0        0        0     1862 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_shipment.py
--rw-r--r--   0        0        0     4877 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_sleep.py
--rw-r--r--   0        0        0     1497 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_sleep_stream.py
--rw-r--r--   0        0        0     1898 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_source.py
--rw-r--r--   0        0        0     1003 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_sport.py
--rw-r--r--   0        0        0     1867 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_steps_timeseries.py
--rw-r--r--   0        0        0     1447 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_stream.py
--rw-r--r--   0        0        0     1573 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_stress_level_timeseries.py
--rw-r--r--   0        0        0     1710 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_team.py
--rw-r--r--   0        0        0      992 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_test_kit_order_details.py
--rw-r--r--   0        0        0     1273 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_testkit_order.py
--rw-r--r--   0        0        0     2915 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_user.py
--rw-r--r--   0        0        0     1367 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_user_key.py
--rw-r--r--   0        0        0     1844 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_vo_2_max_timeseries.py
--rw-r--r--   0        0        0     1002 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_walk_in_order_details.py
--rw-r--r--   0        0        0     1129 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_walk_in_test_order.py
--rw-r--r--   0        0        0     1638 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_water_timeseries.py
--rw-r--r--   0        0        0     4268 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_facing_workout.py
--rw-r--r--   0        0        0      955 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_sleep_response.py
--rw-r--r--   0        0        0      951 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_user_id_conflict.py
--rw-r--r--   0        0        0      966 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/client_workout_response.py
--rw-r--r--   0        0        0     1271 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/connected_source_client_facing.py
--rw-r--r--   0        0        0      916 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/connection_status.py
--rw-r--r--   0        0        0     1126 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/consent.py
--rw-r--r--   0        0        0     1519 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/consent_type.py
--rw-r--r--   0        0        0      930 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/day_slots.py
--rw-r--r--   0        0        0     1240 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/delegated_flow_type.py
--rw-r--r--   0        0        0      897 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/demo_connection_status.py
--rw-r--r--   0        0        0      892 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/demo_providers.py
--rw-r--r--   0        0        0     1053 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/device_v_2_in_db.py
--rw-r--r--   0        0        0      153 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/email_providers.py
--rw-r--r--   0        0        0      936 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/energy.py
--rw-r--r--   0        0        0     1172 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/event_destination_preferences.py
--rw-r--r--   0        0        0      762 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/event_destination_preferences_enabled_item.py
--rw-r--r--   0        0        0      754 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/event_destination_preferences_preferred.py
--rw-r--r--   0        0        0     1169 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/fallback_birth_date.py
--rw-r--r--   0        0        0     1376 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/fallback_time_zone.py
--rw-r--r--   0        0        0     1623 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/fats.py
--rw-r--r--   0        0        0      762 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/gender.py
--rw-r--r--   0        0        0     1110 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/get_markers_response.py
--rw-r--r--   0        0        0     1048 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/get_orders_response.py
--rw-r--r--   0        0        0     1087 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/grouped_blood_oxygen.py
--rw-r--r--   0        0        0     1254 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/grouped_blood_oxygen_response.py
--rw-r--r--   0        0        0     1095 2024-04-12 14:15:53.173241 vital-2.1.3/src/vital/types/grouped_blood_pressure.py
--rw-r--r--   0        0        0     1262 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_blood_pressure_response.py
--rw-r--r--   0        0        0     1071 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_body_fat.py
--rw-r--r--   0        0        0     1238 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_body_fat_response.py
--rw-r--r--   0        0        0     1083 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_body_weight.py
--rw-r--r--   0        0        0     1250 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_body_weight_response.py
--rw-r--r--   0        0        0     1074 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_caffeine.py
--rw-r--r--   0        0        0     1241 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_caffeine_response.py
--rw-r--r--   0        0        0     1099 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_calories_active.py
--rw-r--r--   0        0        0     1266 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_calories_active_response.py
--rw-r--r--   0        0        0     1095 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_calories_basal.py
--rw-r--r--   0        0        0     1262 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_calories_basal_response.py
--rw-r--r--   0        0        0     1086 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_cholesterol.py
--rw-r--r--   0        0        0     1253 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_cholesterol_response.py
--rw-r--r--   0        0        0     1074 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_distance.py
--rw-r--r--   0        0        0     1241 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_distance_response.py
--rw-r--r--   0        0        0     1139 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_electrocardiogram_voltage.py
--rw-r--r--   0        0        0     1306 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_electrocardiogram_voltage_response.py
--rw-r--r--   0        0        0     1095 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_floors_climbed.py
--rw-r--r--   0        0        0     1262 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_floors_climbed_response.py
--rw-r--r--   0        0        0     1070 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_glucose.py
--rw-r--r--   0        0        0     1237 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_glucose_response.py
--rw-r--r--   0        0        0     1079 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_heart_rate.py
--rw-r--r--   0        0        0     1246 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_heart_rate_response.py
--rw-r--r--   0        0        0     1054 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_hrv.py
--rw-r--r--   0        0        0     1221 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_hrv_response.py
--rw-r--r--   0        0        0     1078 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_hypnogram.py
--rw-r--r--   0        0        0     1245 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_hypnogram_response.py
--rw-r--r--   0        0        0     1054 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_ige.py
--rw-r--r--   0        0        0     1221 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_ige_response.py
--rw-r--r--   0        0        0     1054 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_igg.py
--rw-r--r--   0        0        0     1221 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_igg_response.py
--rw-r--r--   0        0        0     1115 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_mindfulness_minutes.py
--rw-r--r--   0        0        0     1282 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_mindfulness_minutes_response.py
--rw-r--r--   0        0        0     1103 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_respiratory_rate.py
--rw-r--r--   0        0        0     1270 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_respiratory_rate_response.py
--rw-r--r--   0        0        0     1062 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_steps.py
--rw-r--r--   0        0        0     1229 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_steps_response.py
--rw-r--r--   0        0        0     1087 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_stress_level.py
--rw-r--r--   0        0        0     1254 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_stress_level_response.py
--rw-r--r--   0        0        0     1068 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_vo_2_max.py
--rw-r--r--   0        0        0     1235 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_vo_2_max_response.py
--rw-r--r--   0        0        0     1062 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_water.py
--rw-r--r--   0        0        0     1229 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/grouped_water_response.py
--rw-r--r--   0        0        0     3022 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/health_insurance_create_request.py
--rw-r--r--   0        0        0      811 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/health_insurance_create_request_back_image.py
--rw-r--r--   0        0        0      816 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/health_insurance_create_request_front_image.py
--rw-r--r--   0        0        0      876 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/health_insurance_create_request_patient_signature_image.py
--rw-r--r--   0        0        0      732 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/historical_pull_status.py
--rw-r--r--   0        0        0      966 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/http_validation_error.py
--rw-r--r--   0        0        0      864 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/jpeg.py
--rw-r--r--   0        0        0     1289 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lab_results_metadata.py
--rw-r--r--   0        0        0     1034 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lab_results_raw.py
--rw-r--r--   0        0        0      223 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lab_results_raw_results.py
--rw-r--r--   0        0        0      827 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lab_test_collection_method.py
--rw-r--r--   0        0        0      898 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lab_test_sample_type.py
--rw-r--r--   0        0        0      729 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lab_test_status.py
--rw-r--r--   0        0        0      949 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/last_attempt.py
--rw-r--r--   0        0        0      936 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/libre_config.py
--rw-r--r--   0        0        0      960 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/link_token_exchange_response.py
--rw-r--r--   0        0        0      879 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/lng_lat.py
--rw-r--r--   0        0        0     1553 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/macros.py
--rw-r--r--   0        0        0     1792 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/manual_providers.py
--rw-r--r--   0        0        0      501 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/marker_type.py
--rw-r--r--   0        0        0     1444 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/meal_in_db_base_client_facing_source.py
--rw-r--r--   0        0        0     1233 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/metrics_result.py
--rw-r--r--   0        0        0     1272 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/micros.py
--rw-r--r--   0        0        0     2126 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/o_auth_providers.py
--rw-r--r--   0        0        0     9798 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/order_status.py
--rw-r--r--   0        0        0     1265 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/order_top_level_status.py
--rw-r--r--   0        0        0     1001 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/paginated_users_response.py
--rw-r--r--   0        0        0     1779 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/password_providers.py
--rw-r--r--   0        0        0     1063 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/patient_address_compatible.py
--rw-r--r--   0        0        0     1000 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/patient_details.py
--rw-r--r--   0        0        0     1004 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/person_details.py
--rw-r--r--   0        0        0      993 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/phlebotomy_area_info.py
--rw-r--r--   0        0        0     1065 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/phlebotomy_provider_info.py
--rw-r--r--   0        0        0     1281 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/physician_create_request.py
--rw-r--r--   0        0        0     1008 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/physician_create_request_base.py
--rw-r--r--   0        0        0      806 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/physician_create_request_signature_image.py
--rw-r--r--   0        0        0      863 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/png.py
--rw-r--r--   0        0        0      973 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/post_order_response.py
--rw-r--r--   0        0        0     1106 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/profile_in_db.py
--rw-r--r--   0        0        0     1003 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/provider_link_response.py
--rw-r--r--   0        0        0     5156 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/providers.py
--rw-r--r--   0        0        0      943 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/raw_activity.py
--rw-r--r--   0        0        0      923 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/raw_body.py
--rw-r--r--   0        0        0      935 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/raw_devices.py
--rw-r--r--   0        0        0      917 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/raw_profile.py
--rw-r--r--   0        0        0      928 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/raw_sleep.py
--rw-r--r--   0        0        0      939 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/raw_workout.py
--rw-r--r--   0        0        0     1360 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/region.py
--rw-r--r--   0        0        0      761 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/responsible_relationship.py
--rw-r--r--   0        0        0      662 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/result_type.py
--rw-r--r--   0        0        0     1020 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/shipping_address.py
--rw-r--r--   0        0        0     1146 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/single_historical_pull_statistics.py
--rw-r--r--   0        0        0     1125 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/single_provider_historical_pull_response.py
--rw-r--r--   0        0        0     1081 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/single_resource_statistics.py
--rw-r--r--   0        0        0     1052 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/single_user_historical_pull_response.py
--rw-r--r--   0        0        0     1026 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/single_user_resource_response.py
--rw-r--r--   0        0        0     1152 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/sleep_v_2_in_db.py
--rw-r--r--   0        0        0     1246 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/source.py
--rw-r--r--   0        0        0     1209 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/source_auth_type.py
--rw-r--r--   0        0        0     1123 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/source_link.py
--rw-r--r--   0        0        0      892 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/source_type.py
--rw-r--r--   0        0        0     1248 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/team_config.py
--rw-r--r--   0        0        0     1147 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/time_slot.py
--rw-r--r--   0        0        0      903 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/timeseries_metric_point.py
--rw-r--r--   0        0        0     4865 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/timeseries_resource.py
--rw-r--r--   0        0        0     1138 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/us_address.py
--rw-r--r--   0        0        0     1040 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/user_historical_pulls_response.py
--rw-r--r--   0        0        0     1304 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/user_refresh_error_response.py
--rw-r--r--   0        0        0     1356 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/user_refresh_success_response.py
--rw-r--r--   0        0        0     1015 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/user_resources_response.py
--rw-r--r--   0        0        0      906 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/user_sign_in_token_response.py
--rw-r--r--   0        0        0      952 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/user_success_response.py
--rw-r--r--   0        0        0      992 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      904 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/vital_token_created_response.py
--rw-r--r--   0        0        0     1217 2024-04-12 14:15:53.177241 vital-2.1.3/src/vital/types/workout_v_2_in_db.py
--rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 vital-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3329 2024-05-03 09:41:02.425919 vital-2.1.4/README.md
+-rw-r--r--   0        0        0      396 2024-05-03 09:41:02.425919 vital-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    14691 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/__init__.py
+-rw-r--r--   0        0        0     5404 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/client.py
+-rw-r--r--   0        0        0      519 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/core/api_error.py
+-rw-r--r--   0        0        0     1332 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      308 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/environment.py
+-rw-r--r--   0        0        0      236 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/errors/bad_request_error.py
+-rw-r--r--   0        0        0      313 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/py.typed
+-rw-r--r--   0        0        0      532 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/activity/__init__.py
+-rw-r--r--   0        0        0     8820 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/activity/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/body/__init__.py
+-rw-r--r--   0        0        0     8736 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/body/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/devices/__init__.py
+-rw-r--r--   0        0        0     3749 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/devices/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/insurance/__init__.py
+-rw-r--r--   0        0        0     6803 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/insurance/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/introspect/__init__.py
+-rw-r--r--   0        0        0     8413 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/introspect/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/lab_tests/__init__.py
+-rw-r--r--   0        0        0    67947 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/lab_tests/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/link/__init__.py
+-rw-r--r--   0        0        0    44285 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/link/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/meal/__init__.py
+-rw-r--r--   0        0        0     4811 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/meal/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/profile/__init__.py
+-rw-r--r--   0        0        0     5698 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/profile/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/providers/__init__.py
+-rw-r--r--   0        0        0     2776 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/providers/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/sleep/__init__.py
+-rw-r--r--   0        0        0    15472 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/sleep/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/team/__init__.py
+-rw-r--r--   0        0        0    18216 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/team/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/testkit/__init__.py
+-rw-r--r--   0        0        0     8435 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/testkit/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/user/__init__.py
+-rw-r--r--   0        0        0    36610 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/user/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/vitals/__init__.py
+-rw-r--r--   0        0        0   214696 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/vitals/client.py
+-rw-r--r--   0        0        0       65 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/workouts/__init__.py
+-rw-r--r--   0        0        0    11545 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/resources/workouts/client.py
+-rw-r--r--   0        0        0    21454 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/activity_v_2_in_db.py
+-rw-r--r--   0        0        0      967 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/address.py
+-rw-r--r--   0        0        0      971 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/appointment_availability_slots.py
+-rw-r--r--   0        0        0     1074 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/appointment_event_status.py
+-rw-r--r--   0        0        0      748 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/appointment_provider.py
+-rw-r--r--   0        0        0      661 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/appointment_service_type.py
+-rw-r--r--   0        0        0     1044 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/appointment_status.py
+-rw-r--r--   0        0        0      149 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/appointment_type.py
+-rw-r--r--   0        0        0      957 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/area_info.py
+-rw-r--r--   0        0        0      510 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/attempt_status.py
+-rw-r--r--   0        0        0      649 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/auth_type.py
+-rw-r--r--   0        0        0      537 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/availability.py
+-rw-r--r--   0        0        0     1468 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/biomarker_result.py
+-rw-r--r--   0        0        0     1168 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/body_v_2_in_db.py
+-rw-r--r--   0        0        0      970 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_activity_response.py
+-rw-r--r--   0        0        0      950 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_body_response.py
+-rw-r--r--   0        0        0     3581 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_activity.py
+-rw-r--r--   0        0        0     1010 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_api_key.py
+-rw-r--r--   0        0        0     1815 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_appointment.py
+-rw-r--r--   0        0        0      934 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_appointment_cancellation_reason.py
+-rw-r--r--   0        0        0     1051 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_appointment_event.py
+-rw-r--r--   0        0        0     1193 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_at_home_phlebotomy_order.py
+-rw-r--r--   0        0        0     1030 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_at_home_phlebotomy_order_details.py
+-rw-r--r--   0        0        0     1634 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_blood_oxygen_timeseries.py
+-rw-r--r--   0        0        0     1632 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_blood_pressure_timeseries.py
+-rw-r--r--   0        0        0     1637 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_body.py
+-rw-r--r--   0        0        0     1631 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_body_fat_timeseries.py
+-rw-r--r--   0        0        0     1630 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_body_weight_timeseries.py
+-rw-r--r--   0        0        0     1859 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_caffeine_timeseries.py
+-rw-r--r--   0        0        0     1919 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_calories_active_timeseries.py
+-rw-r--r--   0        0        0     1658 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_calories_basal_timeseries.py
+-rw-r--r--   0        0        0     1623 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_cholesterol_timeseries.py
+-rw-r--r--   0        0        0     1071 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_diagnosis_information.py
+-rw-r--r--   0        0        0     1874 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_distance_timeseries.py
+-rw-r--r--   0        0        0     1540 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py
+-rw-r--r--   0        0        0     1656 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_floors_climbed_timeseries.py
+-rw-r--r--   0        0        0     1048 2024-05-03 09:41:02.425919 vital-2.1.4/src/vital/types/client_facing_food.py
+-rw-r--r--   0        0        0     1619 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_glucose_timeseries.py
+-rw-r--r--   0        0        0     1236 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_heart_rate.py
+-rw-r--r--   0        0        0     1606 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_heart_rate_timeseries.py
+-rw-r--r--   0        0        0     1624 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_hrv_timeseries.py
+-rw-r--r--   0        0        0     1968 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_hypnogram_timeseries.py
+-rw-r--r--   0        0        0     1612 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_ige_timeseries.py
+-rw-r--r--   0        0        0     1612 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_igg_timeseries.py
+-rw-r--r--   0        0        0     1183 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_lab.py
+-rw-r--r--   0        0        0     1780 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_lab_test.py
+-rw-r--r--   0        0        0      945 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_loinc.py
+-rw-r--r--   0        0        0     1147 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_marker.py
+-rw-r--r--   0        0        0     1262 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_marker_complete.py
+-rw-r--r--   0        0        0     1003 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_meal_response.py
+-rw-r--r--   0        0        0     1861 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_mindfulness_minutes_timeseries.py
+-rw-r--r--   0        0        0     3286 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_order.py
+-rw-r--r--   0        0        0     1311 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_order_details.py
+-rw-r--r--   0        0        0      967 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_order_event.py
+-rw-r--r--   0        0        0     1060 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_patient_details_compatible.py
+-rw-r--r--   0        0        0     1239 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_payor_search_response.py
+-rw-r--r--   0        0        0      916 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_physician.py
+-rw-r--r--   0        0        0     1210 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_profile.py
+-rw-r--r--   0        0        0     1164 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_provider.py
+-rw-r--r--   0        0        0     1418 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_provider_detailed.py
+-rw-r--r--   0        0        0     1302 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_provider_with_status.py
+-rw-r--r--   0        0        0     6046 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_resource.py
+-rw-r--r--   0        0        0     1639 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_respiratory_rate_timeseries.py
+-rw-r--r--   0        0        0     1088 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_result.py
+-rw-r--r--   0        0        0     1862 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_shipment.py
+-rw-r--r--   0        0        0     4877 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_sleep.py
+-rw-r--r--   0        0        0     1497 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_sleep_stream.py
+-rw-r--r--   0        0        0     1898 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_source.py
+-rw-r--r--   0        0        0     1003 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_sport.py
+-rw-r--r--   0        0        0     1867 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_steps_timeseries.py
+-rw-r--r--   0        0        0     1447 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_stream.py
+-rw-r--r--   0        0        0     1573 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_stress_level_timeseries.py
+-rw-r--r--   0        0        0     1936 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_team.py
+-rw-r--r--   0        0        0      992 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_test_kit_order_details.py
+-rw-r--r--   0        0        0     1273 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_testkit_order.py
+-rw-r--r--   0        0        0     2915 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_user.py
+-rw-r--r--   0        0        0     1367 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_user_key.py
+-rw-r--r--   0        0        0     1844 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_vo_2_max_timeseries.py
+-rw-r--r--   0        0        0     1002 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_walk_in_order_details.py
+-rw-r--r--   0        0        0     1129 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_walk_in_test_order.py
+-rw-r--r--   0        0        0     1638 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_water_timeseries.py
+-rw-r--r--   0        0        0     4268 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_facing_workout.py
+-rw-r--r--   0        0        0      955 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_sleep_response.py
+-rw-r--r--   0        0        0      951 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_user_id_conflict.py
+-rw-r--r--   0        0        0      966 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/client_workout_response.py
+-rw-r--r--   0        0        0     1271 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/connected_source_client_facing.py
+-rw-r--r--   0        0        0     1077 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/connection_status.py
+-rw-r--r--   0        0        0      487 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/connection_status_state.py
+-rw-r--r--   0        0        0     1126 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/consent.py
+-rw-r--r--   0        0        0     1519 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/consent_type.py
+-rw-r--r--   0        0        0      930 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/day_slots.py
+-rw-r--r--   0        0        0     1240 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/delegated_flow_type.py
+-rw-r--r--   0        0        0      897 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/demo_connection_status.py
+-rw-r--r--   0        0        0      892 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/demo_providers.py
+-rw-r--r--   0        0        0     1053 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/device_v_2_in_db.py
+-rw-r--r--   0        0        0      153 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/email_providers.py
+-rw-r--r--   0        0        0      936 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/energy.py
+-rw-r--r--   0        0        0     1172 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/event_destination_preferences.py
+-rw-r--r--   0        0        0      762 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/event_destination_preferences_enabled_item.py
+-rw-r--r--   0        0        0      754 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/event_destination_preferences_preferred.py
+-rw-r--r--   0        0        0     1169 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/fallback_birth_date.py
+-rw-r--r--   0        0        0     1376 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/fallback_time_zone.py
+-rw-r--r--   0        0        0     1623 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/fats.py
+-rw-r--r--   0        0        0      762 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/gender.py
+-rw-r--r--   0        0        0     1110 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/get_markers_response.py
+-rw-r--r--   0        0        0     1048 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/get_orders_response.py
+-rw-r--r--   0        0        0     1087 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_blood_oxygen.py
+-rw-r--r--   0        0        0     1254 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_blood_oxygen_response.py
+-rw-r--r--   0        0        0     1095 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_blood_pressure.py
+-rw-r--r--   0        0        0     1262 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_blood_pressure_response.py
+-rw-r--r--   0        0        0     1071 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_body_fat.py
+-rw-r--r--   0        0        0     1238 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_body_fat_response.py
+-rw-r--r--   0        0        0     1083 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_body_weight.py
+-rw-r--r--   0        0        0     1250 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_body_weight_response.py
+-rw-r--r--   0        0        0     1074 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_caffeine.py
+-rw-r--r--   0        0        0     1241 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_caffeine_response.py
+-rw-r--r--   0        0        0     1099 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_calories_active.py
+-rw-r--r--   0        0        0     1266 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_calories_active_response.py
+-rw-r--r--   0        0        0     1095 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_calories_basal.py
+-rw-r--r--   0        0        0     1262 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_calories_basal_response.py
+-rw-r--r--   0        0        0     1086 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_cholesterol.py
+-rw-r--r--   0        0        0     1253 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_cholesterol_response.py
+-rw-r--r--   0        0        0     1074 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_distance.py
+-rw-r--r--   0        0        0     1241 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_distance_response.py
+-rw-r--r--   0        0        0     1139 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_electrocardiogram_voltage.py
+-rw-r--r--   0        0        0     1306 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_electrocardiogram_voltage_response.py
+-rw-r--r--   0        0        0     1095 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_floors_climbed.py
+-rw-r--r--   0        0        0     1262 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_floors_climbed_response.py
+-rw-r--r--   0        0        0     1070 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_glucose.py
+-rw-r--r--   0        0        0     1237 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_glucose_response.py
+-rw-r--r--   0        0        0     1079 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_heart_rate.py
+-rw-r--r--   0        0        0     1246 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_heart_rate_response.py
+-rw-r--r--   0        0        0     1054 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_hrv.py
+-rw-r--r--   0        0        0     1221 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_hrv_response.py
+-rw-r--r--   0        0        0     1078 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_hypnogram.py
+-rw-r--r--   0        0        0     1245 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_hypnogram_response.py
+-rw-r--r--   0        0        0     1054 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_ige.py
+-rw-r--r--   0        0        0     1221 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_ige_response.py
+-rw-r--r--   0        0        0     1054 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_igg.py
+-rw-r--r--   0        0        0     1221 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_igg_response.py
+-rw-r--r--   0        0        0     1115 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_mindfulness_minutes.py
+-rw-r--r--   0        0        0     1282 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_mindfulness_minutes_response.py
+-rw-r--r--   0        0        0     1103 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_respiratory_rate.py
+-rw-r--r--   0        0        0     1270 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_respiratory_rate_response.py
+-rw-r--r--   0        0        0     1062 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_steps.py
+-rw-r--r--   0        0        0     1229 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_steps_response.py
+-rw-r--r--   0        0        0     1087 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_stress_level.py
+-rw-r--r--   0        0        0     1254 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_stress_level_response.py
+-rw-r--r--   0        0        0     1068 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_vo_2_max.py
+-rw-r--r--   0        0        0     1235 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_vo_2_max_response.py
+-rw-r--r--   0        0        0     1062 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_water.py
+-rw-r--r--   0        0        0     1229 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/grouped_water_response.py
+-rw-r--r--   0        0        0     3022 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/health_insurance_create_request.py
+-rw-r--r--   0        0        0      811 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/health_insurance_create_request_back_image.py
+-rw-r--r--   0        0        0      816 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/health_insurance_create_request_front_image.py
+-rw-r--r--   0        0        0      876 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/health_insurance_create_request_patient_signature_image.py
+-rw-r--r--   0        0        0      732 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/historical_pull_status.py
+-rw-r--r--   0        0        0      966 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/http_validation_error.py
+-rw-r--r--   0        0        0      864 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/jpeg.py
+-rw-r--r--   0        0        0     1289 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lab_results_metadata.py
+-rw-r--r--   0        0        0     1034 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lab_results_raw.py
+-rw-r--r--   0        0        0      223 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lab_results_raw_results.py
+-rw-r--r--   0        0        0      827 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lab_test_collection_method.py
+-rw-r--r--   0        0        0      898 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lab_test_sample_type.py
+-rw-r--r--   0        0        0      729 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lab_test_status.py
+-rw-r--r--   0        0        0      949 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/last_attempt.py
+-rw-r--r--   0        0        0      936 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/libre_config.py
+-rw-r--r--   0        0        0      960 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/link_token_exchange_response.py
+-rw-r--r--   0        0        0      879 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/lng_lat.py
+-rw-r--r--   0        0        0     1553 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/macros.py
+-rw-r--r--   0        0        0     1792 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/manual_providers.py
+-rw-r--r--   0        0        0      501 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/marker_type.py
+-rw-r--r--   0        0        0     1444 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/meal_in_db_base_client_facing_source.py
+-rw-r--r--   0        0        0     1233 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/metrics_result.py
+-rw-r--r--   0        0        0     1272 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/micros.py
+-rw-r--r--   0        0        0     2126 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/o_auth_providers.py
+-rw-r--r--   0        0        0     9798 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/order_status.py
+-rw-r--r--   0        0        0     1265 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/order_top_level_status.py
+-rw-r--r--   0        0        0     1001 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/paginated_users_response.py
+-rw-r--r--   0        0        0     1779 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/password_providers.py
+-rw-r--r--   0        0        0     1063 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/patient_address_compatible.py
+-rw-r--r--   0        0        0     1000 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/patient_details.py
+-rw-r--r--   0        0        0     1004 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/person_details.py
+-rw-r--r--   0        0        0      993 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/phlebotomy_area_info.py
+-rw-r--r--   0        0        0     1065 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/phlebotomy_provider_info.py
+-rw-r--r--   0        0        0     1281 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/physician_create_request.py
+-rw-r--r--   0        0        0     1008 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/physician_create_request_base.py
+-rw-r--r--   0        0        0      806 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/physician_create_request_signature_image.py
+-rw-r--r--   0        0        0      863 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/png.py
+-rw-r--r--   0        0        0      973 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/post_order_response.py
+-rw-r--r--   0        0        0     1106 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/profile_in_db.py
+-rw-r--r--   0        0        0     1177 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/provider_link_response.py
+-rw-r--r--   0        0        0      499 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/provider_link_response_state.py
+-rw-r--r--   0        0        0     5156 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/providers.py
+-rw-r--r--   0        0        0      943 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/raw_activity.py
+-rw-r--r--   0        0        0      923 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/raw_body.py
+-rw-r--r--   0        0        0      935 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/raw_devices.py
+-rw-r--r--   0        0        0      917 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/raw_profile.py
+-rw-r--r--   0        0        0      928 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/raw_sleep.py
+-rw-r--r--   0        0        0      939 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/raw_workout.py
+-rw-r--r--   0        0        0     1360 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/region.py
+-rw-r--r--   0        0        0     1055 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/resource_availability.py
+-rw-r--r--   0        0        0      761 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/responsible_relationship.py
+-rw-r--r--   0        0        0      662 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/result_type.py
+-rw-r--r--   0        0        0     1000 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/scope_requirements_grants.py
+-rw-r--r--   0        0        0      925 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/scope_requirements_str.py
+-rw-r--r--   0        0        0     1020 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/shipping_address.py
+-rw-r--r--   0        0        0     1146 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/single_historical_pull_statistics.py
+-rw-r--r--   0        0        0     1125 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/single_provider_historical_pull_response.py
+-rw-r--r--   0        0        0     1081 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/single_resource_statistics.py
+-rw-r--r--   0        0        0     1052 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/single_user_historical_pull_response.py
+-rw-r--r--   0        0        0     1026 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/single_user_resource_response.py
+-rw-r--r--   0        0        0     1152 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/sleep_v_2_in_db.py
+-rw-r--r--   0        0        0     1246 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/source.py
+-rw-r--r--   0        0        0     1209 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/source_auth_type.py
+-rw-r--r--   0        0        0     1123 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/source_link.py
+-rw-r--r--   0        0        0      892 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/source_type.py
+-rw-r--r--   0        0        0     1303 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/team_config.py
+-rw-r--r--   0        0        0     1147 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/time_slot.py
+-rw-r--r--   0        0        0      903 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/timeseries_metric_point.py
+-rw-r--r--   0        0        0     4865 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/timeseries_resource.py
+-rw-r--r--   0        0        0     1138 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/us_address.py
+-rw-r--r--   0        0        0     1040 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/user_historical_pulls_response.py
+-rw-r--r--   0        0        0     1304 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/user_refresh_error_response.py
+-rw-r--r--   0        0        0     1356 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/user_refresh_success_response.py
+-rw-r--r--   0        0        0     1015 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/user_resources_response.py
+-rw-r--r--   0        0        0      906 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/user_sign_in_token_response.py
+-rw-r--r--   0        0        0      952 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/user_success_response.py
+-rw-r--r--   0        0        0      992 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      904 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/vital_token_created_response.py
+-rw-r--r--   0        0        0     1217 2024-05-03 09:41:02.429919 vital-2.1.4/src/vital/types/workout_v_2_in_db.py
+-rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 vital-2.1.4/PKG-INFO
```

### Comparing `vital-2.1.3/README.md` & `vital-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/__init__.py` & `vital-2.1.4/src/vital/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     AppointmentProvider,
     AppointmentServiceType,
     AppointmentStatus,
     AppointmentType,
     AreaInfo,
     AttemptStatus,
     AuthType,
+    Availability,
     BiomarkerResult,
     BodyV2InDb,
     ClientActivityResponse,
     ClientBodyResponse,
     ClientFacingActivity,
     ClientFacingApiKey,
     ClientFacingAppointment,
@@ -86,14 +87,15 @@
     ClientFacingWaterTimeseries,
     ClientFacingWorkout,
     ClientSleepResponse,
     ClientUserIdConflict,
     ClientWorkoutResponse,
     ConnectedSourceClientFacing,
     ConnectionStatus,
+    ConnectionStatusState,
     Consent,
     ConsentType,
     DaySlots,
     DelegatedFlowType,
     DemoConnectionStatus,
     DemoProviders,
     DeviceV2InDb,
@@ -198,24 +200,28 @@
     PhysicianCreateRequestSignatureImage,
     PhysicianCreateRequestSignatureImage_ImageJpeg,
     PhysicianCreateRequestSignatureImage_ImagePng,
     Png,
     PostOrderResponse,
     ProfileInDb,
     ProviderLinkResponse,
+    ProviderLinkResponseState,
     Providers,
     RawActivity,
     RawBody,
     RawDevices,
     RawProfile,
     RawSleep,
     RawWorkout,
     Region,
+    ResourceAvailability,
     ResponsibleRelationship,
     ResultType,
+    ScopeRequirementsGrants,
+    ScopeRequirementsStr,
     ShippingAddress,
     SingleHistoricalPullStatistics,
     SingleProviderHistoricalPullResponse,
     SingleResourceStatistics,
     SingleUserHistoricalPullResponse,
     SingleUserResourceResponse,
     SleepV2InDb,
@@ -268,14 +274,15 @@
     "AppointmentProvider",
     "AppointmentServiceType",
     "AppointmentStatus",
     "AppointmentType",
     "AreaInfo",
     "AttemptStatus",
     "AuthType",
+    "Availability",
     "BadRequestError",
     "BiomarkerResult",
     "BodyV2InDb",
     "ClientActivityResponse",
     "ClientBodyResponse",
     "ClientFacingActivity",
     "ClientFacingApiKey",
@@ -347,14 +354,15 @@
     "ClientFacingWaterTimeseries",
     "ClientFacingWorkout",
     "ClientSleepResponse",
     "ClientUserIdConflict",
     "ClientWorkoutResponse",
     "ConnectedSourceClientFacing",
     "ConnectionStatus",
+    "ConnectionStatusState",
     "Consent",
     "ConsentType",
     "DaySlots",
     "DelegatedFlowType",
     "DemoConnectionStatus",
     "DemoProviders",
     "DeviceV2InDb",
@@ -459,24 +467,28 @@
     "PhysicianCreateRequestSignatureImage",
     "PhysicianCreateRequestSignatureImage_ImageJpeg",
     "PhysicianCreateRequestSignatureImage_ImagePng",
     "Png",
     "PostOrderResponse",
     "ProfileInDb",
     "ProviderLinkResponse",
+    "ProviderLinkResponseState",
     "Providers",
     "RawActivity",
     "RawBody",
     "RawDevices",
     "RawProfile",
     "RawSleep",
     "RawWorkout",
     "Region",
+    "ResourceAvailability",
     "ResponsibleRelationship",
     "ResultType",
+    "ScopeRequirementsGrants",
+    "ScopeRequirementsStr",
     "ShippingAddress",
     "SingleHistoricalPullStatistics",
     "SingleProviderHistoricalPullResponse",
     "SingleResourceStatistics",
     "SingleUserHistoricalPullResponse",
     "SingleUserResourceResponse",
     "SleepV2InDb",
```

### Comparing `vital-2.1.3/src/vital/client.py` & `vital-2.1.4/src/vital/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 
 class Vital:
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: VitalEnvironment = VitalEnvironment.PRODUCTION,
+        vital_link_token: str,
         api_key: str,
         timeout: typing.Optional[float] = 60,
         httpx_client: typing.Optional[httpx.Client] = None
     ):
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
+            vital_link_token=vital_link_token,
             api_key=api_key,
             httpx_client=httpx.Client(timeout=timeout) if httpx_client is None else httpx_client,
         )
         self.link = LinkClient(client_wrapper=self._client_wrapper)
         self.profile = ProfileClient(client_wrapper=self._client_wrapper)
         self.devices = DevicesClient(client_wrapper=self._client_wrapper)
         self.activity = ActivityClient(client_wrapper=self._client_wrapper)
@@ -59,20 +61,22 @@
 
 class AsyncVital:
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: VitalEnvironment = VitalEnvironment.PRODUCTION,
+        vital_link_token: str,
         api_key: str,
         timeout: typing.Optional[float] = 60,
         httpx_client: typing.Optional[httpx.AsyncClient] = None
     ):
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
+            vital_link_token=vital_link_token,
             api_key=api_key,
             httpx_client=httpx.AsyncClient(timeout=timeout) if httpx_client is None else httpx_client,
         )
         self.link = AsyncLinkClient(client_wrapper=self._client_wrapper)
         self.profile = AsyncProfileClient(client_wrapper=self._client_wrapper)
         self.devices = AsyncDevicesClient(client_wrapper=self._client_wrapper)
         self.activity = AsyncActivityClient(client_wrapper=self._client_wrapper)
```

### Comparing `vital-2.1.3/src/vital/core/__init__.py` & `vital-2.1.4/src/vital/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/core/datetime_utils.py` & `vital-2.1.4/src/vital/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/core/jsonable_encoder.py` & `vital-2.1.4/src/vital/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/resources/__init__.py` & `vital-2.1.4/src/vital/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/resources/activity/client.py` & `vital-2.1.4/src/vital/resources/activity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.activity.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -88,14 +89,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.activity.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -140,14 +142,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.activity.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -187,14 +190,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.activity.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
```

### Comparing `vital-2.1.3/src/vital/resources/body/client.py` & `vital-2.1.4/src/vital/resources/body/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.body.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -88,14 +89,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.body.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -140,14 +142,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.body.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -187,14 +190,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.body.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
```

### Comparing `vital-2.1.3/src/vital/resources/devices/client.py` & `vital-2.1.4/src/vital/resources/devices/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             - user_id: str.
 
             - provider: typing.Optional[str]. Provider oura/strava etc
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.devices.get_raw(
             user_id="user-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -69,14 +70,15 @@
             - user_id: str.
 
             - provider: typing.Optional[str]. Provider oura/strava etc
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.devices.get_raw(
             user_id="user-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `vital-2.1.3/src/vital/resources/insurance/client.py` & `vital-2.1.4/src/vital/resources/insurance/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         """
         Parameters:
             - diagnosis_query: str.
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.insurance.search_diagnosis(
             diagnosis_query="diagnosis-query",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -124,14 +125,15 @@
         """
         Parameters:
             - diagnosis_query: str.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.insurance.search_diagnosis(
             diagnosis_query="diagnosis-query",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `vital-2.1.3/src/vital/resources/introspect/client.py` & `vital-2.1.4/src/vital/resources/introspect/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
             - cursor: typing.Optional[str].
         ---
         from vital import Providers
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.introspect.get_user_resources(
             provider=Providers.OURA,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -88,14 +89,15 @@
 
             - cursor: typing.Optional[str].
         ---
         from vital import Providers
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.introspect.get_user_historical_pulls(
             provider=Providers.OURA,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -140,14 +142,15 @@
 
             - cursor: typing.Optional[str].
         ---
         from vital import Providers
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.introspect.get_user_resources(
             provider=Providers.OURA,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -187,14 +190,15 @@
 
             - cursor: typing.Optional[str].
         ---
         from vital import Providers
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.introspect.get_user_historical_pulls(
             provider=Providers.OURA,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `vital-2.1.3/src/vital/resources/lab_tests/client.py` & `vital-2.1.4/src/vital/resources/lab_tests/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         """
         GET all the lab tests the team has access to.
 
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/lab_tests"),
@@ -148,14 +149,15 @@
             - page: typing.Optional[int].
 
             - size: typing.Optional[int].
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get_markers()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/lab_tests/markers"),
@@ -183,14 +185,15 @@
             - page: typing.Optional[int].
 
             - size: typing.Optional[int].
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get_markers_for_lab_test(
             lab_test_id="lab-test-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -241,14 +244,15 @@
         """
         GET all the labs.
 
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get_labs()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/lab_tests/labs"),
@@ -440,14 +444,15 @@
         """
         Get the list of reasons for cancelling an at-home phlebotomy appointment.
 
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get_phlebotomy_appointment_cancellation_reason()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
@@ -784,14 +789,15 @@
             - page: typing.Optional[int].
 
             - size: typing.Optional[int].
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get_orders()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/orders"),
@@ -828,14 +834,15 @@
         """
         GET all the lab tests the team has access to.
 
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/lab_tests"),
@@ -923,14 +930,15 @@
             - page: typing.Optional[int].
 
             - size: typing.Optional[int].
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get_markers()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/lab_tests/markers"),
@@ -958,14 +966,15 @@
             - page: typing.Optional[int].
 
             - size: typing.Optional[int].
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get_markers_for_lab_test(
             lab_test_id="lab-test-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -1016,14 +1025,15 @@
         """
         GET all the labs.
 
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get_labs()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/lab_tests/labs"),
@@ -1217,14 +1227,15 @@
         """
         Get the list of reasons for cancelling an at-home phlebotomy appointment.
 
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get_phlebotomy_appointment_cancellation_reason()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
@@ -1561,14 +1572,15 @@
             - page: typing.Optional[int].
 
             - size: typing.Optional[int].
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get_orders()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/orders"),
```

### Comparing `vital-2.1.3/src/vital/resources/link/client.py` & `vital-2.1.4/src/vital/resources/link/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/resources/meal/client.py` & `vital-2.1.4/src/vital/resources/meal/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.meal.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -92,14 +93,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.meal.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
```

### Comparing `vital-2.1.3/src/vital/resources/profile/client.py` & `vital-2.1.4/src/vital/resources/profile/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/resources/providers/client.py` & `vital-2.1.4/src/vital/resources/providers/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         """
         Get Provider list
 
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.providers.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/providers"),
@@ -53,14 +54,15 @@
         """
         Get Provider list
 
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.providers.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/providers"),
```

### Comparing `vital-2.1.3/src/vital/resources/sleep/client.py` & `vital-2.1.4/src/vital/resources/sleep/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.sleep.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -89,14 +90,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.sleep.get_stream(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -136,14 +138,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.sleep.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -170,14 +173,15 @@
 
         Parameters:
             - sleep_id: str. The Vital Sleep ID
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.sleep.get_stream_by_sleep_id(
             sleep_id="sleep-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -220,14 +224,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -267,14 +272,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get_stream(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -314,14 +320,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -348,14 +355,15 @@
 
         Parameters:
             - sleep_id: str. The Vital Sleep ID
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get_stream_by_sleep_id(
             sleep_id="sleep-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `vital-2.1.3/src/vital/resources/team/client.py` & `vital-2.1.4/src/vital/resources/team/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,34 +19,31 @@
     import pydantic  # type: ignore
 
 
 class TeamClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_link_config(self, *, vital_link_token: typing.Optional[str] = None) -> typing.Dict[str, typing.Any]:
+    def get_link_config(self) -> typing.Dict[str, typing.Any]:
         """
         Post teams.
 
-        Parameters:
-            - vital_link_token: typing.Optional[str].
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.team.get_link_config()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/link/config"),
-            headers=remove_none_from_dict(
-                {**self._client_wrapper.get_headers(), "x-vital-link-token": vital_link_token}
-            ),
+            headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Dict[str, typing.Any], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -84,14 +81,15 @@
 
         Parameters:
             - query_id: typing.Optional[str].
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.team.get_user_by_id()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/users/search"),
@@ -110,14 +108,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_svix_url(self) -> typing.Dict[str, typing.Any]:
         """
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.team.get_svix_url()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/svix/url"),
@@ -140,14 +139,15 @@
 
         Parameters:
             - data_type: typing.Optional[str].
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.team.get_source_priorities()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/source/priorities"),
@@ -171,14 +171,15 @@
 
         Parameters:
             - team_id: str.
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.team.update_source_priorities(
             team_id="team-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -202,14 +203,15 @@
         """
         Parameters:
             - team_id: str.
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.team.get_physicians(
             team_id="team-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -229,34 +231,31 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTeamClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_link_config(self, *, vital_link_token: typing.Optional[str] = None) -> typing.Dict[str, typing.Any]:
+    async def get_link_config(self) -> typing.Dict[str, typing.Any]:
         """
         Post teams.
 
-        Parameters:
-            - vital_link_token: typing.Optional[str].
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.team.get_link_config()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/link/config"),
-            headers=remove_none_from_dict(
-                {**self._client_wrapper.get_headers(), "x-vital-link-token": vital_link_token}
-            ),
+            headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Dict[str, typing.Any], _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -294,14 +293,15 @@
 
         Parameters:
             - query_id: typing.Optional[str].
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.team.get_user_by_id()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/users/search"),
@@ -320,14 +320,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_svix_url(self) -> typing.Dict[str, typing.Any]:
         """
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.team.get_svix_url()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/svix/url"),
@@ -350,14 +351,15 @@
 
         Parameters:
             - data_type: typing.Optional[str].
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.team.get_source_priorities()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/source/priorities"),
@@ -381,14 +383,15 @@
 
         Parameters:
             - team_id: str.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.team.update_source_priorities(
             team_id="team-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -412,14 +415,15 @@
         """
         Parameters:
             - team_id: str.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.team.get_physicians(
             team_id="team-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `vital-2.1.3/src/vital/resources/testkit/client.py` & `vital-2.1.4/src/vital/resources/testkit/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/resources/user/client.py` & `vital-2.1.4/src/vital/resources/user/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 
         Parameters:
             - user_id: str.
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.user.get_connected_providers(
             user_id="user-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -252,14 +253,15 @@
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
             - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.user.patch(
             user_id="user-id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
@@ -521,14 +523,15 @@
 
         Parameters:
             - user_id: str.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.user.get_connected_providers(
             user_id="user-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -613,14 +616,15 @@
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
             - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.user.patch(
             user_id="user-id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
```

### Comparing `vital-2.1.3/src/vital/resources/vitals/client.py` & `vital-2.1.4/src/vital/resources/vitals/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.vo_2_max_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -136,14 +137,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.stress_level_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -188,14 +190,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.mindfulness_minutes_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -240,14 +243,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.caffeine_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -292,14 +296,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.water_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -342,14 +347,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.steps_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -392,14 +398,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.floors_climbed_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -444,14 +451,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.distance_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -496,14 +504,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_basal_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -548,14 +557,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_active_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -600,14 +610,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.respiratory_rate_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -652,14 +663,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.ige_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -702,14 +714,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.igg_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -752,14 +765,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.hypnogram_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -804,14 +818,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.hrv_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -854,14 +869,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.heartrate_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -906,14 +922,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.glucose_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -956,14 +973,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1008,14 +1026,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_weight_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1060,14 +1079,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_fat_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1112,14 +1132,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_oxygen_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1164,14 +1185,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.electrocardiogram_voltage_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1216,14 +1238,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_pressure_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1265,14 +1288,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.vo_2_max(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1310,14 +1334,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.stress_level(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1355,14 +1380,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.mindfulness_minutes(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1402,14 +1428,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.caffeine(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1447,14 +1474,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.water(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1492,14 +1520,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.steps(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1537,14 +1566,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.floors_climbed(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1582,14 +1612,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.distance(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1627,14 +1658,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_basal(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1672,14 +1704,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_active(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1717,14 +1750,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.respiratory_rate(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1764,14 +1798,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.ige(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1809,14 +1844,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.igg(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1854,14 +1890,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.hypnogram(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1899,14 +1936,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.hrv(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1944,14 +1982,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.heartrate(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -1989,14 +2028,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.glucose(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2034,14 +2074,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_triglycerides(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2081,14 +2122,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_total(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2128,14 +2170,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_ldl(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2173,14 +2216,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_hdl(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2218,14 +2262,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2263,14 +2308,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_weight(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2308,14 +2354,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_fat(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2353,14 +2400,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_oxygen(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2398,14 +2446,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.electrocardiogram_voltage(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2445,14 +2494,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_pressure(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2498,14 +2548,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.vo_2_max_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2548,14 +2599,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.stress_level_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2600,14 +2652,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.mindfulness_minutes_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2652,14 +2705,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.caffeine_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2704,14 +2758,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.water_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2754,14 +2809,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.steps_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2804,14 +2860,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.floors_climbed_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2856,14 +2913,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.distance_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2908,14 +2966,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_basal_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -2960,14 +3019,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_active_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3012,14 +3072,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.respiratory_rate_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3064,14 +3125,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.ige_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3114,14 +3176,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.igg_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3164,14 +3227,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hypnogram_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3216,14 +3280,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hrv_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3266,14 +3331,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.heartrate_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3318,14 +3384,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.glucose_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3368,14 +3435,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3420,14 +3488,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_weight_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3472,14 +3541,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_fat_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3524,14 +3594,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_oxygen_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3576,14 +3647,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.electrocardiogram_voltage_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3628,14 +3700,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_pressure_grouped(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3677,14 +3750,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.vo_2_max(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3722,14 +3796,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.stress_level(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3767,14 +3842,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.mindfulness_minutes(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3814,14 +3890,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.caffeine(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3859,14 +3936,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.water(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3904,14 +3982,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.steps(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3949,14 +4028,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.floors_climbed(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -3994,14 +4074,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.distance(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4039,14 +4120,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_basal(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4084,14 +4166,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_active(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4129,14 +4212,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.respiratory_rate(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4176,14 +4260,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.ige(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4221,14 +4306,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.igg(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4266,14 +4352,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hypnogram(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4311,14 +4398,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hrv(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4356,14 +4444,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.heartrate(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4401,14 +4490,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.glucose(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4446,14 +4536,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_triglycerides(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4493,14 +4584,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_total(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4540,14 +4632,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_ldl(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4585,14 +4678,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_hdl(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4630,14 +4724,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4675,14 +4770,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_weight(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4720,14 +4816,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_fat(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4765,14 +4862,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_oxygen(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4810,14 +4908,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.electrocardiogram_voltage(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -4857,14 +4956,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_pressure(
             user_id="user-id",
             start_date="start-date",
         )
         """
```

### Comparing `vital-2.1.3/src/vital/resources/workouts/client.py` & `vital-2.1.4/src/vital/resources/workouts/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.workouts.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -89,14 +90,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.workouts.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -121,14 +123,15 @@
         """
         Parameters:
             - workout_id: str. The Vital ID for the workout
         ---
         from vital.client import Vital
 
         client = Vital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         client.workouts.get_by_workout_id(
             workout_id="workout-id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -173,14 +176,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.workouts.get(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -220,14 +224,15 @@
             - start_date: str. Date from in YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 00:00:00
 
             - end_date: typing.Optional[str]. Date to YYYY-MM-DD or ISO formatted date time. If a date is provided without a time, the time will be set to 23:59:59
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.workouts.get_raw(
             user_id="user-id",
             start_date="start-date",
         )
         """
@@ -252,14 +257,15 @@
         """
         Parameters:
             - workout_id: str. The Vital ID for the workout
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
+            vital_link_token="YOUR_VITAL_LINK_TOKEN",
             api_key="YOUR_API_KEY",
         )
         await client.workouts.get_by_workout_id(
             workout_id="workout-id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `vital-2.1.3/src/vital/types/__init__.py` & `vital-2.1.4/src/vital/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .appointment_provider import AppointmentProvider
 from .appointment_service_type import AppointmentServiceType
 from .appointment_status import AppointmentStatus
 from .appointment_type import AppointmentType
 from .area_info import AreaInfo
 from .attempt_status import AttemptStatus
 from .auth_type import AuthType
+from .availability import Availability
 from .biomarker_result import BiomarkerResult
 from .body_v_2_in_db import BodyV2InDb
 from .client_activity_response import ClientActivityResponse
 from .client_body_response import ClientBodyResponse
 from .client_facing_activity import ClientFacingActivity
 from .client_facing_api_key import ClientFacingApiKey
 from .client_facing_appointment import ClientFacingAppointment
@@ -87,14 +88,15 @@
 from .client_facing_water_timeseries import ClientFacingWaterTimeseries
 from .client_facing_workout import ClientFacingWorkout
 from .client_sleep_response import ClientSleepResponse
 from .client_user_id_conflict import ClientUserIdConflict
 from .client_workout_response import ClientWorkoutResponse
 from .connected_source_client_facing import ConnectedSourceClientFacing
 from .connection_status import ConnectionStatus
+from .connection_status_state import ConnectionStatusState
 from .consent import Consent
 from .consent_type import ConsentType
 from .day_slots import DaySlots
 from .delegated_flow_type import DelegatedFlowType
 from .demo_connection_status import DemoConnectionStatus
 from .demo_providers import DemoProviders
 from .device_v_2_in_db import DeviceV2InDb
@@ -207,24 +209,28 @@
     PhysicianCreateRequestSignatureImage_ImageJpeg,
     PhysicianCreateRequestSignatureImage_ImagePng,
 )
 from .png import Png
 from .post_order_response import PostOrderResponse
 from .profile_in_db import ProfileInDb
 from .provider_link_response import ProviderLinkResponse
+from .provider_link_response_state import ProviderLinkResponseState
 from .providers import Providers
 from .raw_activity import RawActivity
 from .raw_body import RawBody
 from .raw_devices import RawDevices
 from .raw_profile import RawProfile
 from .raw_sleep import RawSleep
 from .raw_workout import RawWorkout
 from .region import Region
+from .resource_availability import ResourceAvailability
 from .responsible_relationship import ResponsibleRelationship
 from .result_type import ResultType
+from .scope_requirements_grants import ScopeRequirementsGrants
+from .scope_requirements_str import ScopeRequirementsStr
 from .shipping_address import ShippingAddress
 from .single_historical_pull_statistics import SingleHistoricalPullStatistics
 from .single_provider_historical_pull_response import SingleProviderHistoricalPullResponse
 from .single_resource_statistics import SingleResourceStatistics
 from .single_user_historical_pull_response import SingleUserHistoricalPullResponse
 from .single_user_resource_response import SingleUserResourceResponse
 from .sleep_v_2_in_db import SleepV2InDb
@@ -256,14 +262,15 @@
     "AppointmentProvider",
     "AppointmentServiceType",
     "AppointmentStatus",
     "AppointmentType",
     "AreaInfo",
     "AttemptStatus",
     "AuthType",
+    "Availability",
     "BiomarkerResult",
     "BodyV2InDb",
     "ClientActivityResponse",
     "ClientBodyResponse",
     "ClientFacingActivity",
     "ClientFacingApiKey",
     "ClientFacingAppointment",
@@ -334,14 +341,15 @@
     "ClientFacingWaterTimeseries",
     "ClientFacingWorkout",
     "ClientSleepResponse",
     "ClientUserIdConflict",
     "ClientWorkoutResponse",
     "ConnectedSourceClientFacing",
     "ConnectionStatus",
+    "ConnectionStatusState",
     "Consent",
     "ConsentType",
     "DaySlots",
     "DelegatedFlowType",
     "DemoConnectionStatus",
     "DemoProviders",
     "DeviceV2InDb",
@@ -446,24 +454,28 @@
     "PhysicianCreateRequestSignatureImage",
     "PhysicianCreateRequestSignatureImage_ImageJpeg",
     "PhysicianCreateRequestSignatureImage_ImagePng",
     "Png",
     "PostOrderResponse",
     "ProfileInDb",
     "ProviderLinkResponse",
+    "ProviderLinkResponseState",
     "Providers",
     "RawActivity",
     "RawBody",
     "RawDevices",
     "RawProfile",
     "RawSleep",
     "RawWorkout",
     "Region",
+    "ResourceAvailability",
     "ResponsibleRelationship",
     "ResultType",
+    "ScopeRequirementsGrants",
+    "ScopeRequirementsStr",
     "ShippingAddress",
     "SingleHistoricalPullStatistics",
     "SingleProviderHistoricalPullResponse",
     "SingleResourceStatistics",
     "SingleUserHistoricalPullResponse",
     "SingleUserResourceResponse",
     "SleepV2InDb",
```

### Comparing `vital-2.1.3/src/vital/types/activity_v_2_in_db.py` & `vital-2.1.4/src/vital/types/activity_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/address.py` & `vital-2.1.4/src/vital/types/address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/appointment_availability_slots.py` & `vital-2.1.4/src/vital/types/appointment_availability_slots.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/appointment_event_status.py` & `vital-2.1.4/src/vital/types/appointment_event_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/appointment_provider.py` & `vital-2.1.4/src/vital/types/appointment_provider.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/appointment_service_type.py` & `vital-2.1.4/src/vital/types/appointment_service_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/appointment_status.py` & `vital-2.1.4/src/vital/types/appointment_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/area_info.py` & `vital-2.1.4/src/vital/types/area_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/auth_type.py` & `vital-2.1.4/src/vital/types/auth_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/biomarker_result.py` & `vital-2.1.4/src/vital/types/biomarker_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/body_v_2_in_db.py` & `vital-2.1.4/src/vital/types/body_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_activity_response.py` & `vital-2.1.4/src/vital/types/client_activity_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_body_response.py` & `vital-2.1.4/src/vital/types/client_body_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_activity.py` & `vital-2.1.4/src/vital/types/client_facing_activity.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_api_key.py` & `vital-2.1.4/src/vital/types/client_facing_api_key.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_appointment.py` & `vital-2.1.4/src/vital/types/client_facing_appointment.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_appointment_cancellation_reason.py` & `vital-2.1.4/src/vital/types/client_facing_appointment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_appointment_event.py` & `vital-2.1.4/src/vital/types/client_facing_appointment_event.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_at_home_phlebotomy_order.py` & `vital-2.1.4/src/vital/types/client_facing_at_home_phlebotomy_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_at_home_phlebotomy_order_details.py` & `vital-2.1.4/src/vital/types/client_facing_at_home_phlebotomy_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_blood_oxygen_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_blood_oxygen_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_blood_pressure_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_blood_pressure_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_body.py` & `vital-2.1.4/src/vital/types/client_facing_body.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_body_fat_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_body_fat_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_body_weight_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_body_weight_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_caffeine_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_caffeine_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_calories_active_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_calories_active_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_calories_basal_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_calories_basal_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_cholesterol_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_cholesterol_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_diagnosis_information.py` & `vital-2.1.4/src/vital/types/client_facing_diagnosis_information.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_distance_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_distance_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_floors_climbed_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_floors_climbed_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_food.py` & `vital-2.1.4/src/vital/types/client_facing_food.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_glucose_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_glucose_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_heart_rate.py` & `vital-2.1.4/src/vital/types/client_facing_heart_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_heart_rate_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_heart_rate_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_hrv_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_hrv_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_hypnogram_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_hypnogram_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_ige_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_ige_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_igg_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_igg_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_lab.py` & `vital-2.1.4/src/vital/types/client_facing_lab.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_lab_test.py` & `vital-2.1.4/src/vital/types/client_facing_lab_test.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_loinc.py` & `vital-2.1.4/src/vital/types/client_facing_loinc.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_marker.py` & `vital-2.1.4/src/vital/types/client_facing_marker.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_marker_complete.py` & `vital-2.1.4/src/vital/types/client_facing_marker_complete.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_meal_response.py` & `vital-2.1.4/src/vital/types/client_facing_meal_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_mindfulness_minutes_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_mindfulness_minutes_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_order.py` & `vital-2.1.4/src/vital/types/client_facing_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_order_details.py` & `vital-2.1.4/src/vital/types/client_facing_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_order_event.py` & `vital-2.1.4/src/vital/types/client_facing_order_event.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_patient_details_compatible.py` & `vital-2.1.4/src/vital/types/client_facing_patient_details_compatible.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_payor_search_response.py` & `vital-2.1.4/src/vital/types/client_facing_payor_search_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_physician.py` & `vital-2.1.4/src/vital/types/client_facing_physician.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_profile.py` & `vital-2.1.4/src/vital/types/client_facing_profile.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_provider.py` & `vital-2.1.4/src/vital/types/client_facing_provider.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_provider_detailed.py` & `vital-2.1.4/src/vital/types/client_facing_provider_detailed.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_provider_with_status.py` & `vital-2.1.4/src/vital/types/client_facing_provider_with_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .resource_availability import ResourceAvailability
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ClientFacingProviderWithStatus(pydantic.BaseModel):
     name: str = pydantic.Field(description="Name of source of information")
     slug: str = pydantic.Field(description="Slug for designated source")
     logo: str = pydantic.Field(description="URL for source logo")
     status: str = pydantic.Field(description="Status of source, either error or connected")
+    resource_availability: typing.Dict[str, ResourceAvailability]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.3/src/vital/types/client_facing_resource.py` & `vital-2.1.4/src/vital/types/client_facing_resource.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_respiratory_rate_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_respiratory_rate_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_result.py` & `vital-2.1.4/src/vital/types/client_facing_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_shipment.py` & `vital-2.1.4/src/vital/types/client_facing_shipment.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_sleep.py` & `vital-2.1.4/src/vital/types/client_facing_sleep.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_sleep_stream.py` & `vital-2.1.4/src/vital/types/client_facing_sleep_stream.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_source.py` & `vital-2.1.4/src/vital/types/client_facing_source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_sport.py` & `vital-2.1.4/src/vital/types/client_facing_sport.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_steps_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_steps_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_stream.py` & `vital-2.1.4/src/vital/types/client_facing_stream.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_stress_level_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_stress_level_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_team.py` & `vital-2.1.4/src/vital/types/client_facing_team.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,23 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ClientFacingTeam(pydantic.BaseModel):
+    """
+    [Deprecated] GET /v2/team is in the process of being removed.
+    Neither customers nor Dashboard should retrieve team settings and metadata directly.
+
+    All must migrate to the Team endpoints of the Org Management API.
+    """
+
     id: str
-    org_id: typing.Optional[str]
+    org_id: str
     name: str
     svix_app_id: typing.Optional[str]
     client_id: typing.Optional[str]
     client_secret: typing.Optional[str]
     airtable_api_key: typing.Optional[str]
     airtable_base_id: typing.Optional[str]
     webhook_secret: typing.Optional[str]
```

### Comparing `vital-2.1.3/src/vital/types/client_facing_test_kit_order_details.py` & `vital-2.1.4/src/vital/types/client_facing_test_kit_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_testkit_order.py` & `vital-2.1.4/src/vital/types/client_facing_testkit_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_user.py` & `vital-2.1.4/src/vital/types/client_facing_user.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_user_key.py` & `vital-2.1.4/src/vital/types/client_facing_user_key.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_vo_2_max_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_vo_2_max_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_walk_in_order_details.py` & `vital-2.1.4/src/vital/types/client_facing_walk_in_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_walk_in_test_order.py` & `vital-2.1.4/src/vital/types/client_facing_walk_in_test_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_water_timeseries.py` & `vital-2.1.4/src/vital/types/client_facing_water_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_facing_workout.py` & `vital-2.1.4/src/vital/types/client_facing_workout.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_sleep_response.py` & `vital-2.1.4/src/vital/types/client_sleep_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_user_id_conflict.py` & `vital-2.1.4/src/vital/types/client_user_id_conflict.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/client_workout_response.py` & `vital-2.1.4/src/vital/types/client_workout_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/connected_source_client_facing.py` & `vital-2.1.4/src/vital/types/connected_source_client_facing.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/connection_status.py` & `vital-2.1.4/src/vital/types/scope_requirements_str.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ConnectionStatus(pydantic.BaseModel):
-    success: bool
-    redirect_url: typing.Optional[str]
+class ScopeRequirementsStr(pydantic.BaseModel):
+    required: typing.List[str]
+    optional: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.3/src/vital/types/consent.py` & `vital-2.1.4/src/vital/types/consent.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/consent_type.py` & `vital-2.1.4/src/vital/types/consent_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/day_slots.py` & `vital-2.1.4/src/vital/types/day_slots.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/delegated_flow_type.py` & `vital-2.1.4/src/vital/types/delegated_flow_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/demo_connection_status.py` & `vital-2.1.4/src/vital/types/demo_connection_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/demo_providers.py` & `vital-2.1.4/src/vital/types/demo_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/device_v_2_in_db.py` & `vital-2.1.4/src/vital/types/device_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/energy.py` & `vital-2.1.4/src/vital/types/energy.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/event_destination_preferences.py` & `vital-2.1.4/src/vital/types/event_destination_preferences.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/event_destination_preferences_enabled_item.py` & `vital-2.1.4/src/vital/types/event_destination_preferences_enabled_item.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/event_destination_preferences_preferred.py` & `vital-2.1.4/src/vital/types/event_destination_preferences_preferred.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/fallback_birth_date.py` & `vital-2.1.4/src/vital/types/fallback_birth_date.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/fallback_time_zone.py` & `vital-2.1.4/src/vital/types/fallback_time_zone.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/fats.py` & `vital-2.1.4/src/vital/types/fats.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/gender.py` & `vital-2.1.4/src/vital/types/gender.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/get_markers_response.py` & `vital-2.1.4/src/vital/types/get_markers_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/get_orders_response.py` & `vital-2.1.4/src/vital/types/get_orders_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_blood_oxygen.py` & `vital-2.1.4/src/vital/types/grouped_blood_oxygen.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_blood_oxygen_response.py` & `vital-2.1.4/src/vital/types/grouped_blood_oxygen_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_blood_pressure.py` & `vital-2.1.4/src/vital/types/grouped_blood_pressure.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_blood_pressure_response.py` & `vital-2.1.4/src/vital/types/grouped_blood_pressure_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_body_fat.py` & `vital-2.1.4/src/vital/types/grouped_body_fat.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_body_fat_response.py` & `vital-2.1.4/src/vital/types/grouped_body_fat_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_body_weight.py` & `vital-2.1.4/src/vital/types/grouped_body_weight.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_body_weight_response.py` & `vital-2.1.4/src/vital/types/grouped_body_weight_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_caffeine.py` & `vital-2.1.4/src/vital/types/grouped_caffeine.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_caffeine_response.py` & `vital-2.1.4/src/vital/types/grouped_caffeine_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_calories_active.py` & `vital-2.1.4/src/vital/types/grouped_calories_active.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_calories_active_response.py` & `vital-2.1.4/src/vital/types/grouped_calories_active_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_calories_basal.py` & `vital-2.1.4/src/vital/types/grouped_calories_basal.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_calories_basal_response.py` & `vital-2.1.4/src/vital/types/grouped_calories_basal_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_cholesterol.py` & `vital-2.1.4/src/vital/types/grouped_cholesterol.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_cholesterol_response.py` & `vital-2.1.4/src/vital/types/grouped_cholesterol_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_distance.py` & `vital-2.1.4/src/vital/types/grouped_distance.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_distance_response.py` & `vital-2.1.4/src/vital/types/grouped_distance_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_electrocardiogram_voltage.py` & `vital-2.1.4/src/vital/types/grouped_electrocardiogram_voltage.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_electrocardiogram_voltage_response.py` & `vital-2.1.4/src/vital/types/grouped_electrocardiogram_voltage_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_floors_climbed.py` & `vital-2.1.4/src/vital/types/grouped_floors_climbed.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_floors_climbed_response.py` & `vital-2.1.4/src/vital/types/grouped_floors_climbed_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_glucose.py` & `vital-2.1.4/src/vital/types/grouped_glucose.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_glucose_response.py` & `vital-2.1.4/src/vital/types/grouped_glucose_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_heart_rate.py` & `vital-2.1.4/src/vital/types/grouped_heart_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_heart_rate_response.py` & `vital-2.1.4/src/vital/types/grouped_heart_rate_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_hrv.py` & `vital-2.1.4/src/vital/types/grouped_hrv.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_hrv_response.py` & `vital-2.1.4/src/vital/types/grouped_hrv_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_hypnogram.py` & `vital-2.1.4/src/vital/types/grouped_hypnogram.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_hypnogram_response.py` & `vital-2.1.4/src/vital/types/grouped_hypnogram_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_ige.py` & `vital-2.1.4/src/vital/types/grouped_ige.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_ige_response.py` & `vital-2.1.4/src/vital/types/grouped_ige_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_igg.py` & `vital-2.1.4/src/vital/types/grouped_igg.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_igg_response.py` & `vital-2.1.4/src/vital/types/grouped_igg_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_mindfulness_minutes.py` & `vital-2.1.4/src/vital/types/grouped_mindfulness_minutes.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_mindfulness_minutes_response.py` & `vital-2.1.4/src/vital/types/grouped_mindfulness_minutes_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_respiratory_rate.py` & `vital-2.1.4/src/vital/types/grouped_respiratory_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_respiratory_rate_response.py` & `vital-2.1.4/src/vital/types/grouped_respiratory_rate_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_steps.py` & `vital-2.1.4/src/vital/types/grouped_steps.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_steps_response.py` & `vital-2.1.4/src/vital/types/grouped_steps_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_stress_level.py` & `vital-2.1.4/src/vital/types/grouped_stress_level.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_stress_level_response.py` & `vital-2.1.4/src/vital/types/grouped_stress_level_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_vo_2_max.py` & `vital-2.1.4/src/vital/types/grouped_vo_2_max.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_vo_2_max_response.py` & `vital-2.1.4/src/vital/types/grouped_vo_2_max_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_water.py` & `vital-2.1.4/src/vital/types/grouped_water.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/grouped_water_response.py` & `vital-2.1.4/src/vital/types/grouped_water_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/health_insurance_create_request.py` & `vital-2.1.4/src/vital/types/health_insurance_create_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/health_insurance_create_request_back_image.py` & `vital-2.1.4/src/vital/types/health_insurance_create_request_back_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/health_insurance_create_request_front_image.py` & `vital-2.1.4/src/vital/types/health_insurance_create_request_front_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/health_insurance_create_request_patient_signature_image.py` & `vital-2.1.4/src/vital/types/health_insurance_create_request_patient_signature_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/historical_pull_status.py` & `vital-2.1.4/src/vital/types/historical_pull_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/http_validation_error.py` & `vital-2.1.4/src/vital/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/jpeg.py` & `vital-2.1.4/src/vital/types/jpeg.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/lab_results_metadata.py` & `vital-2.1.4/src/vital/types/lab_results_metadata.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/lab_results_raw.py` & `vital-2.1.4/src/vital/types/lab_results_raw.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/lab_test_collection_method.py` & `vital-2.1.4/src/vital/types/lab_test_collection_method.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/lab_test_sample_type.py` & `vital-2.1.4/src/vital/types/lab_test_sample_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/lab_test_status.py` & `vital-2.1.4/src/vital/types/lab_test_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/last_attempt.py` & `vital-2.1.4/src/vital/types/last_attempt.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/libre_config.py` & `vital-2.1.4/src/vital/types/libre_config.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/link_token_exchange_response.py` & `vital-2.1.4/src/vital/types/link_token_exchange_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/lng_lat.py` & `vital-2.1.4/src/vital/types/lng_lat.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/macros.py` & `vital-2.1.4/src/vital/types/macros.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/manual_providers.py` & `vital-2.1.4/src/vital/types/manual_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/meal_in_db_base_client_facing_source.py` & `vital-2.1.4/src/vital/types/meal_in_db_base_client_facing_source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/metrics_result.py` & `vital-2.1.4/src/vital/types/metrics_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/micros.py` & `vital-2.1.4/src/vital/types/micros.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/o_auth_providers.py` & `vital-2.1.4/src/vital/types/o_auth_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/order_status.py` & `vital-2.1.4/src/vital/types/order_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/order_top_level_status.py` & `vital-2.1.4/src/vital/types/order_top_level_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/paginated_users_response.py` & `vital-2.1.4/src/vital/types/paginated_users_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/password_providers.py` & `vital-2.1.4/src/vital/types/password_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/patient_address_compatible.py` & `vital-2.1.4/src/vital/types/patient_address_compatible.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/patient_details.py` & `vital-2.1.4/src/vital/types/patient_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/person_details.py` & `vital-2.1.4/src/vital/types/person_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/phlebotomy_area_info.py` & `vital-2.1.4/src/vital/types/phlebotomy_area_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/phlebotomy_provider_info.py` & `vital-2.1.4/src/vital/types/phlebotomy_provider_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/physician_create_request.py` & `vital-2.1.4/src/vital/types/physician_create_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/physician_create_request_base.py` & `vital-2.1.4/src/vital/types/physician_create_request_base.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/physician_create_request_signature_image.py` & `vital-2.1.4/src/vital/types/physician_create_request_signature_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/png.py` & `vital-2.1.4/src/vital/types/png.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/post_order_response.py` & `vital-2.1.4/src/vital/types/post_order_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/profile_in_db.py` & `vital-2.1.4/src/vital/types/profile_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/provider_link_response.py` & `vital-2.1.4/src/vital/types/user_sign_in_token_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .password_providers import PasswordProviders
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ProviderLinkResponse(pydantic.BaseModel):
-    provider: PasswordProviders
-    connected: bool
-    provider_id: typing.Optional[str]
+class UserSignInTokenResponse(pydantic.BaseModel):
+    user_id: str
+    sign_in_token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.3/src/vital/types/providers.py` & `vital-2.1.4/src/vital/types/providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/raw_activity.py` & `vital-2.1.4/src/vital/types/raw_activity.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/raw_body.py` & `vital-2.1.4/src/vital/types/raw_body.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/raw_devices.py` & `vital-2.1.4/src/vital/types/raw_devices.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/raw_profile.py` & `vital-2.1.4/src/vital/types/raw_profile.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/raw_sleep.py` & `vital-2.1.4/src/vital/types/raw_sleep.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/raw_workout.py` & `vital-2.1.4/src/vital/types/raw_workout.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/region.py` & `vital-2.1.4/src/vital/types/region.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/responsible_relationship.py` & `vital-2.1.4/src/vital/types/responsible_relationship.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/result_type.py` & `vital-2.1.4/src/vital/types/result_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/shipping_address.py` & `vital-2.1.4/src/vital/types/shipping_address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/single_historical_pull_statistics.py` & `vital-2.1.4/src/vital/types/single_historical_pull_statistics.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/single_provider_historical_pull_response.py` & `vital-2.1.4/src/vital/types/single_provider_historical_pull_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/single_resource_statistics.py` & `vital-2.1.4/src/vital/types/single_resource_statistics.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/single_user_historical_pull_response.py` & `vital-2.1.4/src/vital/types/single_user_historical_pull_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/single_user_resource_response.py` & `vital-2.1.4/src/vital/types/single_user_resource_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/sleep_v_2_in_db.py` & `vital-2.1.4/src/vital/types/sleep_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/source.py` & `vital-2.1.4/src/vital/types/source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/source_auth_type.py` & `vital-2.1.4/src/vital/types/source_auth_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/source_link.py` & `vital-2.1.4/src/vital/types/source_link.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/source_type.py` & `vital-2.1.4/src/vital/types/source_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/team_config.py` & `vital-2.1.4/src/vital/types/team_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 class TeamConfig(pydantic.BaseModel):
     libreview: LibreConfig
     texts_enabled: typing.Optional[bool]
     push_historical_data: typing.Optional[bool]
     provider_raw_data: typing.Optional[bool]
+    reject_duplicate_connection: typing.Optional[bool]
     eds_preferences: typing.Optional[EventDestinationPreferences]
     event_type_prefixes: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vital-2.1.3/src/vital/types/time_slot.py` & `vital-2.1.4/src/vital/types/time_slot.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/timeseries_metric_point.py` & `vital-2.1.4/src/vital/types/timeseries_metric_point.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/timeseries_resource.py` & `vital-2.1.4/src/vital/types/timeseries_resource.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/us_address.py` & `vital-2.1.4/src/vital/types/us_address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/user_historical_pulls_response.py` & `vital-2.1.4/src/vital/types/user_historical_pulls_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/user_refresh_error_response.py` & `vital-2.1.4/src/vital/types/user_refresh_error_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/user_refresh_success_response.py` & `vital-2.1.4/src/vital/types/user_refresh_success_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/user_resources_response.py` & `vital-2.1.4/src/vital/types/user_resources_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/user_sign_in_token_response.py` & `vital-2.1.4/src/vital/types/vital_token_created_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UserSignInTokenResponse(pydantic.BaseModel):
-    user_id: str
-    sign_in_token: str
+class VitalTokenCreatedResponse(pydantic.BaseModel):
+    code: str
+    exchange_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.3/src/vital/types/user_success_response.py` & `vital-2.1.4/src/vital/types/user_success_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/validation_error.py` & `vital-2.1.4/src/vital/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/src/vital/types/vital_token_created_response.py` & `vital-2.1.4/src/vital/types/scope_requirements_grants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .scope_requirements_str import ScopeRequirementsStr
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class VitalTokenCreatedResponse(pydantic.BaseModel):
-    code: str
-    exchange_url: str
+class ScopeRequirementsGrants(pydantic.BaseModel):
+    user_granted: ScopeRequirementsStr
+    user_denied: ScopeRequirementsStr
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.3/src/vital/types/workout_v_2_in_db.py` & `vital-2.1.4/src/vital/types/workout_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.3/PKG-INFO` & `vital-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 2.1.3
+Version: 2.1.4
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

