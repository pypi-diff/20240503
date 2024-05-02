# Comparing `tmp/morebs2-0.0.8.tar.gz` & `tmp/morebs2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morebs2-0.0.8.tar", last modified: Sat Apr  6 19:41:32 2024, max compression
+gzip compressed data, was "morebs2-0.0.9.tar", last modified: Sat Apr 27 20:53:36 2024, max compression
```

## Comparing `morebs2-0.0.8.tar` & `morebs2-0.0.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 19:41:32.219823 morebs2-0.0.8/
--rw-rw-rw-   0        0        0     7169 2023-09-12 01:51:38.000000 morebs2-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      911 2024-04-06 19:41:32.219823 morebs2-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-06 19:27:55.000000 morebs2-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 19:41:31.676580 morebs2-0.0.8/morebs2/
--rw-rw-rw-   0        0        0       53 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/__init__.py
--rw-rw-rw-   0        0        0     7620 2024-04-06 19:32:58.000000 morebs2-0.0.8/morebs2/aprng_gauge.py
--rw-rw-rw-   0        0        0     9609 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_clump_data_generator.py
--rw-rw-rw-   0        0        0     1849 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_clump_data_generator_test.py
--rw-rw-rw-   0        0        0    17948 2024-02-06 01:45:03.000000 morebs2-0.0.8/morebs2/ball_comp.py
--rw-rw-rw-   0        0        0     9508 2024-02-19 04:29:04.000000 morebs2-0.0.8/morebs2/ball_comp_components.py
--rw-rw-rw-   0        0        0     2195 2024-02-06 01:45:05.000000 morebs2-0.0.8/morebs2/ball_comp_test.py
--rw-rw-rw-   0        0        0     3616 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_comp_test_cases.py
--rw-rw-rw-   0        0        0     9384 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_operator.py
--rw-rw-rw-   0        0        0     2172 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_operator_navigation_test.py
--rw-rw-rw-   0        0        0     1346 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_operator_split_test.py
--rw-rw-rw-   0        0        0     1583 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_operator_test_cases.py
--rw-rw-rw-   0        0        0     6030 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/ball_volume_estimators.py
--rw-rw-rw-   0        0        0     3409 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/chained_poly_interpolation.py
--rw-rw-rw-   0        0        0    22003 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/deline.py
--rw-rw-rw-   0        0        0     7064 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/deline_helpers.py
--rw-rw-rw-   0        0        0     4611 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/deline_mc.py
--rw-rw-rw-   0        0        0     4223 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/distributions.py
--rw-rw-rw-   0        0        0     6744 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/fit_2n2.py
--rw-rw-rw-   0        0        0     1211 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/globalls.py
--rw-rw-rw-   0        0        0     6461 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/hop_pattern.py
--rw-rw-rw-   0        0        0    20982 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/line.py
--rw-rw-rw-   0        0        0    30620 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/matrix_methods.py
--rw-rw-rw-   0        0        0     7251 2024-03-08 20:06:07.000000 morebs2-0.0.8/morebs2/measures.py
--rw-rw-rw-   0        0        0     4386 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/message_streamer.py
--rw-rw-rw-   0        0        0     1573 2024-03-06 06:26:15.000000 morebs2-0.0.8/morebs2/modular_labeller.py
--rw-rw-rw-   0        0        0     1991 2023-12-28 08:50:26.000000 morebs2-0.0.8/morebs2/numerical_extras.py
--rw-rw-rw-   0        0        0     9847 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/numerical_generator.py
--rw-rw-rw-   0        0        0     6520 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/numerical_space_data_generator.py
--rw-rw-rw-   0        0        0    13713 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/point_sorter.py
--rw-rw-rw-   0        0        0     4774 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/point_weight_function.py
--rw-rw-rw-   0        0        0    12158 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/poly_factor.py
--rw-rw-rw-   0        0        0    26397 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/poly_interpolation.py
--rw-rw-rw-   0        0        0    12702 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/poly_struct.py
--rw-rw-rw-   0        0        0     4466 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/random_generators.py
--rw-rw-rw-   0        0        0    28986 2024-04-03 21:33:23.000000 morebs2-0.0.8/morebs2/relevance_functions.py
--rw-rw-rw-   0        0        0     1073 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/relevance_functions_extended.py
--rw-rw-rw-   0        0        0    14223 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/rssi.py
--rw-rw-rw-   0        0        0     4015 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/rssi_components.py
--rw-rw-rw-   0        0        0    16342 2024-04-06 11:44:14.000000 morebs2-0.0.8/morebs2/search_space_iterator.py
--rw-rw-rw-   0        0        0     4968 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/set_merger.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:41:32.204203 morebs2-0.0.8/morebs2/tests/
--rw-rw-rw-   0        0        0        0 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/__init__.py
--rw-rw-rw-   0        0        0     3332 2024-04-06 15:37:56.000000 morebs2-0.0.8/morebs2/tests/aprng_gauge_test.py
--rw-rw-rw-   0        0        0     2969 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/ball_comp_components_test.py
--rw-rw-rw-   0        0        0     1117 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/ball_comp_components_test_cases.py
--rw-rw-rw-   0        0        0     2837 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/chained_poly_interpolation_test.py
--rw-rw-rw-   0        0        0     5692 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/deline_test.py
--rw-rw-rw-   0        0        0     1139 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/fit_2n2_test.py
--rw-rw-rw-   0        0        0     6014 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/hop_pattern_test.py
--rw-rw-rw-   0        0        0     4693 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/matrix_methods__bounds__test.py
--rw-rw-rw-   0        0        0     1986 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/message_streamer_test.py
--rw-rw-rw-   0        0        0     2743 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/numerical_generator_test.py
--rw-rw-rw-   0        0        0     5554 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/numerical_space_data_generator_test.py
--rw-rw-rw-   0        0        0     4351 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/point_sorter_test.py
--rw-rw-rw-   0        0        0     8302 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/point_weight_function_test.py
--rw-rw-rw-   0        0        0     2125 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/poly_factor_test.py
--rw-rw-rw-   0        0        0     9908 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/poly_interpolation_test.py
--rw-rw-rw-   0        0        0     1276 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/poly_struct_test.py
--rw-rw-rw-   0        0        0     6627 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/relevance_functions_test.py
--rw-rw-rw-   0        0        0     1590 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/relevance_functions_test2.py
--rw-rw-rw-   0        0        0     2169 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/rssi_test.py
--rw-rw-rw-   0        0        0     1101 2023-09-12 01:51:38.000000 morebs2-0.0.8/morebs2/tests/rssi_test_cases.py
--rw-rw-rw-   0        0        0     9224 2023-09-12 01:51:39.000000 morebs2-0.0.8/morebs2/tests/search_space_iterator_test.py
--rw-rw-rw-   0        0        0     4336 2023-09-12 01:51:39.000000 morebs2-0.0.8/morebs2/tests/search_space_iterator_test_cases.py
--rw-rw-rw-   0        0        0      958 2023-09-12 01:51:39.000000 morebs2-0.0.8/morebs2/tests/set_merger_test_cases.py
--rw-rw-rw-   0        0        0     3246 2023-09-12 01:51:39.000000 morebs2-0.0.8/morebs2/tests/set_merger_tests.py
--rw-rw-rw-   0        0        0     4925 2023-09-12 01:51:39.000000 morebs2-0.0.8/morebs2/travel_data.py
--rw-rw-rw-   0        0        0      665 2023-09-12 01:51:39.000000 morebs2-0.0.8/morebs2/variance_works.py
--rw-rw-rw-   0        0        0     1773 2023-09-16 02:49:08.000000 morebs2-0.0.8/morebs2/violation_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:41:32.219823 morebs2-0.0.8/morebs2.egg-info/
--rw-rw-rw-   0        0        0      911 2024-04-06 19:41:31.000000 morebs2-0.0.8/morebs2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2362 2024-04-06 19:41:31.000000 morebs2-0.0.8/morebs2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 19:41:31.000000 morebs2-0.0.8/morebs2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 19:41:31.000000 morebs2-0.0.8/morebs2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      606 2024-04-06 19:40:49.000000 morebs2-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 19:41:32.219823 morebs2-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      472 2024-04-06 19:37:10.000000 morebs2-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:53:36.913799 morebs2-0.0.9/
+-rw-rw-rw-   0        0        0     7169 2023-09-12 01:51:38.000000 morebs2-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      911 2024-04-27 20:53:36.896887 morebs2-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-06 19:27:55.000000 morebs2-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-27 20:53:36.630955 morebs2-0.0.9/morebs2/
+-rw-rw-rw-   0        0        0       53 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/__init__.py
+-rw-rw-rw-   0        0        0     7480 2024-04-09 14:44:46.000000 morebs2-0.0.9/morebs2/aprng_gauge.py
+-rw-rw-rw-   0        0        0     9609 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_clump_data_generator.py
+-rw-rw-rw-   0        0        0     1849 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_clump_data_generator_test.py
+-rw-rw-rw-   0        0        0    17948 2024-02-06 01:45:03.000000 morebs2-0.0.9/morebs2/ball_comp.py
+-rw-rw-rw-   0        0        0     9508 2024-02-19 04:29:04.000000 morebs2-0.0.9/morebs2/ball_comp_components.py
+-rw-rw-rw-   0        0        0     2195 2024-02-06 01:45:05.000000 morebs2-0.0.9/morebs2/ball_comp_test.py
+-rw-rw-rw-   0        0        0     3616 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_comp_test_cases.py
+-rw-rw-rw-   0        0        0     9384 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_operator.py
+-rw-rw-rw-   0        0        0     2172 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_operator_navigation_test.py
+-rw-rw-rw-   0        0        0     1346 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_operator_split_test.py
+-rw-rw-rw-   0        0        0     1583 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_operator_test_cases.py
+-rw-rw-rw-   0        0        0     6030 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/ball_volume_estimators.py
+-rw-rw-rw-   0        0        0     3409 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/chained_poly_interpolation.py
+-rw-rw-rw-   0        0        0    22003 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/deline.py
+-rw-rw-rw-   0        0        0     7064 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/deline_helpers.py
+-rw-rw-rw-   0        0        0     4611 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/deline_mc.py
+-rw-rw-rw-   0        0        0     4223 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/distributions.py
+-rw-rw-rw-   0        0        0     6744 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/fit_2n2.py
+-rw-rw-rw-   0        0        0     1211 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/globalls.py
+-rw-rw-rw-   0        0        0     6461 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/hop_pattern.py
+-rw-rw-rw-   0        0        0    20982 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/line.py
+-rw-rw-rw-   0        0        0    30410 2024-04-10 17:56:16.000000 morebs2-0.0.9/morebs2/matrix_methods.py
+-rw-rw-rw-   0        0        0     7251 2024-03-08 20:06:07.000000 morebs2-0.0.9/morebs2/measures.py
+-rw-rw-rw-   0        0        0     4386 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/message_streamer.py
+-rw-rw-rw-   0        0        0     1573 2024-03-06 06:26:15.000000 morebs2-0.0.9/morebs2/modular_labeller.py
+-rw-rw-rw-   0        0        0     1991 2023-12-28 08:50:26.000000 morebs2-0.0.9/morebs2/numerical_extras.py
+-rw-rw-rw-   0        0        0     9876 2024-04-27 20:32:09.000000 morebs2-0.0.9/morebs2/numerical_generator.py
+-rw-rw-rw-   0        0        0     6520 2024-04-26 15:22:06.000000 morebs2-0.0.9/morebs2/numerical_space_data_generator.py
+-rw-rw-rw-   0        0        0    13713 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/point_sorter.py
+-rw-rw-rw-   0        0        0     4774 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/point_weight_function.py
+-rw-rw-rw-   0        0        0    12158 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/poly_factor.py
+-rw-rw-rw-   0        0        0    26397 2024-04-09 00:15:05.000000 morebs2-0.0.9/morebs2/poly_interpolation.py
+-rw-rw-rw-   0        0        0    12702 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/poly_struct.py
+-rw-rw-rw-   0        0        0     4466 2024-04-09 11:41:41.000000 morebs2-0.0.9/morebs2/random_generators.py
+-rw-rw-rw-   0        0        0    28986 2024-04-03 21:33:23.000000 morebs2-0.0.9/morebs2/relevance_functions.py
+-rw-rw-rw-   0        0        0     1073 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/relevance_functions_extended.py
+-rw-rw-rw-   0        0        0    14215 2024-04-26 15:29:54.000000 morebs2-0.0.9/morebs2/rssi.py
+-rw-rw-rw-   0        0        0     4015 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/rssi_components.py
+-rw-rw-rw-   0        0        0    16342 2024-04-06 11:44:14.000000 morebs2-0.0.9/morebs2/search_space_iterator.py
+-rw-rw-rw-   0        0        0     4968 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/set_merger.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:53:36.896887 morebs2-0.0.9/morebs2/tests/
+-rw-rw-rw-   0        0        0        0 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3542 2024-04-07 14:27:30.000000 morebs2-0.0.9/morebs2/tests/aprng_gauge_test.py
+-rw-rw-rw-   0        0        0     2969 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/ball_comp_components_test.py
+-rw-rw-rw-   0        0        0     1117 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/ball_comp_components_test_cases.py
+-rw-rw-rw-   0        0        0     2837 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/chained_poly_interpolation_test.py
+-rw-rw-rw-   0        0        0     5692 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/deline_test.py
+-rw-rw-rw-   0        0        0     1139 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/fit_2n2_test.py
+-rw-rw-rw-   0        0        0     6014 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/hop_pattern_test.py
+-rw-rw-rw-   0        0        0     4693 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/matrix_methods__bounds__test.py
+-rw-rw-rw-   0        0        0     1986 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/message_streamer_test.py
+-rw-rw-rw-   0        0        0     2743 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/numerical_generator_test.py
+-rw-rw-rw-   0        0        0     5554 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/numerical_space_data_generator_test.py
+-rw-rw-rw-   0        0        0     4351 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/point_sorter_test.py
+-rw-rw-rw-   0        0        0     8302 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/point_weight_function_test.py
+-rw-rw-rw-   0        0        0     2125 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/poly_factor_test.py
+-rw-rw-rw-   0        0        0     9908 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/poly_interpolation_test.py
+-rw-rw-rw-   0        0        0     1276 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/poly_struct_test.py
+-rw-rw-rw-   0        0        0     6627 2024-04-16 20:20:15.000000 morebs2-0.0.9/morebs2/tests/relevance_functions_test.py
+-rw-rw-rw-   0        0        0     1590 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/relevance_functions_test2.py
+-rw-rw-rw-   0        0        0     2169 2023-09-12 01:51:38.000000 morebs2-0.0.9/morebs2/tests/rssi_test.py
+-rw-rw-rw-   0        0        0     1101 2024-04-16 20:14:56.000000 morebs2-0.0.9/morebs2/tests/rssi_test_cases.py
+-rw-rw-rw-   0        0        0     9224 2023-09-12 01:51:39.000000 morebs2-0.0.9/morebs2/tests/search_space_iterator_test.py
+-rw-rw-rw-   0        0        0     4336 2023-09-12 01:51:39.000000 morebs2-0.0.9/morebs2/tests/search_space_iterator_test_cases.py
+-rw-rw-rw-   0        0        0      958 2023-09-12 01:51:39.000000 morebs2-0.0.9/morebs2/tests/set_merger_test_cases.py
+-rw-rw-rw-   0        0        0     3246 2023-09-12 01:51:39.000000 morebs2-0.0.9/morebs2/tests/set_merger_tests.py
+-rw-rw-rw-   0        0        0     4925 2023-09-12 01:51:39.000000 morebs2-0.0.9/morebs2/travel_data.py
+-rw-rw-rw-   0        0        0      665 2023-09-12 01:51:39.000000 morebs2-0.0.9/morebs2/variance_works.py
+-rw-rw-rw-   0        0        0     1773 2023-09-16 02:49:08.000000 morebs2-0.0.9/morebs2/violation_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-27 20:53:36.896887 morebs2-0.0.9/morebs2.egg-info/
+-rw-rw-rw-   0        0        0      911 2024-04-27 20:53:36.000000 morebs2-0.0.9/morebs2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2362 2024-04-27 20:53:36.000000 morebs2-0.0.9/morebs2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 20:53:36.000000 morebs2-0.0.9/morebs2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-27 20:53:36.000000 morebs2-0.0.9/morebs2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      606 2024-04-27 20:52:21.000000 morebs2-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-27 20:53:36.913799 morebs2-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-04-27 20:41:58.000000 morebs2-0.0.9/setup.py
```

### Comparing `morebs2-0.0.8/LICENSE` & `morebs2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/PKG-INFO` & `morebs2-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morebs2
-Version: 0.0.8
+Version: 0.0.9
 Summary: data structures to aid in numerical data generation and clustering
 Home-page: https://github.com/Changissnz/morebs
 Author: Richard Pham
 Author-email: Richard Pham <phamrichard45@gmail.com>
 Project-URL: Homepage, https://www.github.com/changissnz/morebs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `morebs2-0.0.8/morebs2/aprng_gauge.py` & `morebs2-0.0.9/morebs2/aprng_gauge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-"""
-- required methods (from previous model): 
-
-
-"""
-############################################
-"""
-    APRNGGauge(AbstractPRNG* aprng, std::pair<float,float> fr, float point_radius = 0.) {
-        assert(fr.second > fr.first);
-        this->aprng = aprng; 
-        this->fr = fr;
-        this->point_radius = point_radius;
-        cycle_scores = mat(0,0,fill::zeros);
-    }
-
-    void MeasureCycle(bool floatgen);
-    void DefaultSetRadius(vec v);
-    std::vector<float> CycleOne(bool floatgen);
-    void GaugePROutput();
-    void GauagePROutputReferential(vec r);
-"""
-############################################
-
 from .search_space_iterator import *
 
 def range_op(rangez,default_value=0.,f_inner=np.subtract,f_outer=np.add):
     rangez_ = to_noncontiguous_ranges(rangez)
     l = len(rangez_)
     s = default_value
     for i in range(0,l):
@@ -53,18 +30,34 @@
         stat = v[i] <= v[i+1]
         if not stat: break 
     return stat 
 
 def is_reflective_condition(v):
     return len(v) == len(np.unique(v))
 
+"""
+Generates numbers in an n-dimensional square
+structure according to variables such as 
+`is_perm`, `is_reflective`. The variable 
+`subset_size` indicates the dimension of the 
+output from `__next__`. 
+
+The value `length` is the length of the vector
+that the output of this class is supposed to 
+accomodate. 
+"""
 class BatchIncrStruct:
 
     def __init__(self,length:int,is_perm=False,\
         is_reflective=False,subset_size=2):
+        """
+        length := int or float, specifies the max 
+                for each bound
+        subset_size := int, otherwise known as the n in n-dim.
+        """
 
         assert type(length) == type(subset_size)
         assert type(length) == int
             
         assert type(is_reflective) == type(is_perm)
         assert type(is_reflective) == bool
```

### Comparing `morebs2-0.0.8/morebs2/ball_clump_data_generator.py` & `morebs2-0.0.9/morebs2/ball_clump_data_generator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_clump_data_generator_test.py` & `morebs2-0.0.9/morebs2/ball_clump_data_generator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_comp.py` & `morebs2-0.0.9/morebs2/ball_comp.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_comp_components.py` & `morebs2-0.0.9/morebs2/ball_comp_components.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_comp_test.py` & `morebs2-0.0.9/morebs2/ball_comp_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_comp_test_cases.py` & `morebs2-0.0.9/morebs2/ball_comp_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_operator.py` & `morebs2-0.0.9/morebs2/ball_operator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_operator_navigation_test.py` & `morebs2-0.0.9/morebs2/ball_operator_navigation_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_operator_split_test.py` & `morebs2-0.0.9/morebs2/ball_operator_split_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_operator_test_cases.py` & `morebs2-0.0.9/morebs2/ball_operator_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/ball_volume_estimators.py` & `morebs2-0.0.9/morebs2/ball_volume_estimators.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/chained_poly_interpolation.py` & `morebs2-0.0.9/morebs2/chained_poly_interpolation.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/deline.py` & `morebs2-0.0.9/morebs2/deline.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/deline_helpers.py` & `morebs2-0.0.9/morebs2/deline_helpers.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/deline_mc.py` & `morebs2-0.0.9/morebs2/deline_mc.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/distributions.py` & `morebs2-0.0.9/morebs2/distributions.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/fit_2n2.py` & `morebs2-0.0.9/morebs2/fit_2n2.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/globalls.py` & `morebs2-0.0.9/morebs2/globalls.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/hop_pattern.py` & `morebs2-0.0.9/morebs2/hop_pattern.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/line.py` & `morebs2-0.0.9/morebs2/line.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/matrix_methods.py` & `morebs2-0.0.9/morebs2/matrix_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,31 +193,24 @@
 
 def is_point_qualified(unqualifiedAreas, point):
 
     for x in unqualifiedAreas:
         if point_in_area(point, x): return False
     return True
 
-# UPDATE:
 """
 if degree in [0,90,180,270],
 
 0: 0
 90: 1
 180: 2
 270: 3
 """
 def quadrant_of_corner_point_in_area(cp, area):
-
-    #deg = degree
-    #def angle_between_two_points_clockwise(startX, endX):
-    ##print("AREA ", area)
-
     corners = area_to_corners(area)
-
     indices = indices_of_vector_in_matrix(corners, cp)
     if len(indices) != 1: raise ValueError("quadrant for corner point {} could not be obtained for\n{}".format(cp, corners))
     return indices[0]
 
 ############################################ END: area
 
 ############################################ START: qualifying area search
@@ -311,18 +304,14 @@
     elif areaWanted == "ymax":
         maxXGivenY = greatest_qualifying_fourway_point_at_point(pointY, unqualifiedAreas, area, id1)
         mp2 = missing_area_point_for_three_points(np.array([maxXGivenY, pointY, point]))
         area2 = trim_area(area, corners_to_area(np.array([maxXGivenY, pointY, point, mp2])))
         return area2
     raise ValueError("invalid wanted area arg.")
 
-# TODO: problem: what if want x > y or y < x ?
-
-# TODO: code this. delete above.
-
 """
 iterate from .min x (point) in `incrementDirections` at in
 
 incrementDirections: increment|axis
 """
 def greatest_qualifying_fourway_point_at_point(point, unqualifiedAreas, area, incrementDirections):
```

### Comparing `morebs2-0.0.8/morebs2/measures.py` & `morebs2-0.0.9/morebs2/measures.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/message_streamer.py` & `morebs2-0.0.9/morebs2/message_streamer.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/modular_labeller.py` & `morebs2-0.0.9/morebs2/modular_labeller.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/numerical_extras.py` & `morebs2-0.0.9/morebs2/numerical_extras.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/numerical_generator.py` & `morebs2-0.0.9/morebs2/numerical_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,24 +173,24 @@
     return np.random.randint(0, 2, (vecOrder,))
 
 ####---------------------------------------------------------------------
 #### uniform dist. numerical generators
 
 """
 """
-def generate_uniform_sequence_in_bounds(vecOrder, bounds):
+def generate_uniform_sequence_in_bounds(vecOrder, bounds,rnd_struct=rng):
     assert is_2dmatrix(bounds), "invalid bounds {}".format(bounds)
     assert vecOrder == len(bounds) or len(bounds) == 1, "invalid bounds"
 
     if len(bounds) == 1:
-        return rng.uniform(bounds[0,0], bounds[0,1], (vecOrder,))
+        return rnd_struct.uniform(bounds[0,0], bounds[0,1], (vecOrder,))
     else:
         q = np.zeros((vecOrder,))
         for i in range(vecOrder):
-            q[i] = rng.uniform(bounds[i,0], bounds[i,1])#, (vecOrder,))
+            q[i] = rnd_struct.uniform(bounds[i,0], bounds[i,1])#, (vecOrder,))
         return q
 
 def random_bounds_edge(bounds):
     assert is_bounds_vector(bounds), "invalid bounds"
     bs = generate_random_binary_sequence(bounds.shape[0])
     r = [i for i in range(bounds.shape[0])]
     return bounds[r,bs]
```

### Comparing `morebs2-0.0.8/morebs2/numerical_space_data_generator.py` & `morebs2-0.0.9/morebs2/numerical_space_data_generator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/point_sorter.py` & `morebs2-0.0.9/morebs2/point_sorter.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/point_weight_function.py` & `morebs2-0.0.9/morebs2/point_weight_function.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/poly_factor.py` & `morebs2-0.0.9/morebs2/poly_factor.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/poly_interpolation.py` & `morebs2-0.0.9/morebs2/poly_interpolation.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/poly_struct.py` & `morebs2-0.0.9/morebs2/poly_struct.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/random_generators.py` & `morebs2-0.0.9/morebs2/random_generators.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/relevance_functions.py` & `morebs2-0.0.9/morebs2/relevance_functions.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/relevance_functions_extended.py` & `morebs2-0.0.9/morebs2/relevance_functions_extended.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/rssi.py` & `morebs2-0.0.9/morebs2/rssi.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,18 +207,14 @@
 
         # TODO: optional, add update func. for png here
         return False
 
     def update_vars_for_rch(self): 
         return [np.copy(self.bounds),self.ssi.de_bounds(),deepcopy(self.SSIHop)] + list(deepcopy(self.aua))
 
-
-
-
-
     def check_duplicate_range(self,d):
         '''
         checks if range `d` is already present in `self.rangeHistory`.
 
         :rtype: bool
         '''
         for d_ in self.rangeHistory:
```

### Comparing `morebs2-0.0.8/morebs2/rssi_components.py` & `morebs2-0.0.9/morebs2/rssi_components.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/search_space_iterator.py` & `morebs2-0.0.9/morebs2/search_space_iterator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/set_merger.py` & `morebs2-0.0.9/morebs2/set_merger.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/aprng_gauge_test.py` & `morebs2-0.0.9/morebs2/tests/aprng_gauge_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,14 +83,19 @@
         assert q0 == ans
 
         q1 = aprng_gauge.max_float_uwpd(5,rv)
         nuwpd = aprng_gauge.normalized_float_uwpd(v,rv)
         assert np.round(ans / q1,5) == \
             nuwpd, "got {} wanted {}".format(nuwpd,ans/q1) 
 
+    def test__to_noncontiguous_ranges(self):
+        ranges = [[0,1],[0.7,1.5],[1.6,2.0],[1.65,2.3]]
+        tnr = aprng_gauge.to_noncontiguous_ranges(ranges)
+        assert tnr == [[0, 1.5], [1.6, 2.3]]
+
     def test_APRNGGauge__measure_cycle(self):
 
         bounds = np.array([[0,5],\
                         [0,5],\
                         [0,5]])
 
         start_point = np.zeros((3,))
```

### Comparing `morebs2-0.0.8/morebs2/tests/ball_comp_components_test.py` & `morebs2-0.0.9/morebs2/tests/ball_comp_components_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/ball_comp_components_test_cases.py` & `morebs2-0.0.9/morebs2/tests/ball_comp_components_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/chained_poly_interpolation_test.py` & `morebs2-0.0.9/morebs2/tests/chained_poly_interpolation_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/deline_test.py` & `morebs2-0.0.9/morebs2/tests/deline_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/fit_2n2_test.py` & `morebs2-0.0.9/morebs2/tests/fit_2n2_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/hop_pattern_test.py` & `morebs2-0.0.9/morebs2/tests/hop_pattern_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/matrix_methods__bounds__test.py` & `morebs2-0.0.9/morebs2/tests/matrix_methods__bounds__test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/message_streamer_test.py` & `morebs2-0.0.9/morebs2/tests/message_streamer_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/numerical_generator_test.py` & `morebs2-0.0.9/morebs2/tests/numerical_generator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/numerical_space_data_generator_test.py` & `morebs2-0.0.9/morebs2/tests/numerical_space_data_generator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/point_sorter_test.py` & `morebs2-0.0.9/morebs2/tests/point_sorter_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/point_weight_function_test.py` & `morebs2-0.0.9/morebs2/tests/point_weight_function_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/poly_factor_test.py` & `morebs2-0.0.9/morebs2/tests/poly_factor_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/poly_interpolation_test.py` & `morebs2-0.0.9/morebs2/tests/poly_interpolation_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/poly_struct_test.py` & `morebs2-0.0.9/morebs2/tests/poly_struct_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/relevance_functions_test.py` & `morebs2-0.0.9/morebs2/tests/relevance_functions_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/relevance_functions_test2.py` & `morebs2-0.0.9/morebs2/tests/relevance_functions_test2.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/rssi_test.py` & `morebs2-0.0.9/morebs2/tests/rssi_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/rssi_test_cases.py` & `morebs2-0.0.9/morebs2/tests/rssi_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/search_space_iterator_test.py` & `morebs2-0.0.9/morebs2/tests/search_space_iterator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/search_space_iterator_test_cases.py` & `morebs2-0.0.9/morebs2/tests/search_space_iterator_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/set_merger_test_cases.py` & `morebs2-0.0.9/morebs2/tests/set_merger_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/tests/set_merger_tests.py` & `morebs2-0.0.9/morebs2/tests/set_merger_tests.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/travel_data.py` & `morebs2-0.0.9/morebs2/travel_data.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/variance_works.py` & `morebs2-0.0.9/morebs2/variance_works.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2/violation_handler.py` & `morebs2-0.0.9/morebs2/violation_handler.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/morebs2.egg-info/PKG-INFO` & `morebs2-0.0.9/morebs2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morebs2
-Version: 0.0.8
+Version: 0.0.9
 Summary: data structures to aid in numerical data generation and clustering
 Home-page: https://github.com/Changissnz/morebs
 Author: Richard Pham
 Author-email: Richard Pham <phamrichard45@gmail.com>
 Project-URL: Homepage, https://www.github.com/changissnz/morebs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `morebs2-0.0.8/morebs2.egg-info/SOURCES.txt` & `morebs2-0.0.9/morebs2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.8/pyproject.toml` & `morebs2-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "morebs2"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Richard Pham", email="phamrichard45@gmail.com" },
 ]
 description = "data structures to aid in numerical data generation and clustering"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

