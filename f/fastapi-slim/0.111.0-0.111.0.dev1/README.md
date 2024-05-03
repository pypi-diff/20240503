# Comparing `tmp/fastapi_slim-0.111.0.tar.gz` & `tmp/fastapi_slim-0.111.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_slim-0.111.0.tar", last modified: Fri May  3 00:21:41 2024, max compression
+gzip compressed data, was "fastapi_slim-0.111.0.dev1.tar", last modified: Tue Apr 30 06:11:53 2024, max compression
```

## Comparing `fastapi_slim-0.111.0.tar` & `fastapi_slim-0.111.0.dev1.tar`

### file list

```diff
@@ -1,1231 +1,1231 @@
--rw-r--r--   0        0        0     1086 2024-05-03 00:21:35.457406 fastapi_slim-0.111.0/LICENSE
--rw-r--r--   0        0        0    23103 2024-05-03 00:21:35.457406 fastapi_slim-0.111.0/README.md
--rw-r--r--   0        0        0     5043 2024-05-03 00:21:35.493406 fastapi_slim-0.111.0/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0      506 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_responses/tutorial001.py
--rw-r--r--   0        0        0      628 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_responses/tutorial002.py
--rw-r--r--   0        0        0      837 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_responses/tutorial003.py
--rw-r--r--   0        0        0      701 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_responses/tutorial004.py
--rw-r--r--   0        0        0      684 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001.py
--rw-r--r--   0        0        0      734 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_an.py
--rw-r--r--   0        0        0      686 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_an_py310.py
--rw-r--r--   0        0        0      705 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_an_py39.py
--rw-r--r--   0        0        0      646 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_py310.py
--rw-r--r--   0        0        0      231 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/advanced_middleware/tutorial001.py
--rw-r--r--   0        0        0      279 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/advanced_middleware/tutorial002.py
--rw-r--r--   0        0        0      213 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/advanced_middleware/tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b/__init__.py
--rw-r--r--   0        0        0     1145 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b/main.py
--rw-r--r--   0        0        0     1866 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an/__init__.py
--rw-r--r--   0        0        0     1205 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an/main.py
--rw-r--r--   0        0        0     1866 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py310/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py310/main.py
--rw-r--r--   0        0        0     1866 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py310/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py39/__init__.py
--rw-r--r--   0        0        0     1176 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py39/main.py
--rw-r--r--   0        0        0     1866 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_py310/__init__.py
--rw-r--r--   0        0        0     1113 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_py310/main.py
--rw-r--r--   0        0        0     1866 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/app_b_py310/test_main.py
--rw-r--r--   0        0        0      118 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/main.py
--rw-r--r--   0        0        0      238 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/test_main.py
--rw-r--r--   0        0        0      334 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/tutorial001.py
--rw-r--r--   0        0        0      757 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/tutorial002.py
--rw-r--r--   0        0        0      528 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/app_testing/tutorial003.py
--rw-r--r--   0        0        0     1415 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/async_sql_databases/tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/async_tests/__init__.py
--rw-r--r--   0        0        0      112 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/async_tests/main.py
--rw-r--r--   0        0        0      306 2024-05-03 00:21:35.577407 fastapi_slim-0.111.0/docs_src/async_tests/test_main.py
--rw-r--r--   0        0        0      519 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/background_tasks/tutorial001.py
--rw-r--r--   0        0        0      675 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002.py
--rw-r--r--   0        0        0      725 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_an.py
--rw-r--r--   0        0        0      683 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_an_py310.py
--rw-r--r--   0        0        0      696 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_an_py39.py
--rw-r--r--   0        0        0      643 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_py310.py
--rw-r--r--   0        0        0      189 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/behind_a_proxy/tutorial001.py
--rw-r--r--   0        0        0      208 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/behind_a_proxy/tutorial002.py
--rw-r--r--   0        0        0      405 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/behind_a_proxy/tutorial003.py
--rw-r--r--   0        0        0      437 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/behind_a_proxy/tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/__init__.py
--rw-r--r--   0        0        0      369 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/internal/__init__.py
--rw-r--r--   0        0        0      147 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/internal/admin.py
--rw-r--r--   0        0        0      552 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/routers/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/routers/items.py
--rw-r--r--   0        0        0      407 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app/routers/users.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/__init__.py
--rw-r--r--   0        0        0      419 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/internal/__init__.py
--rw-r--r--   0        0        0      147 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/internal/admin.py
--rw-r--r--   0        0        0      552 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/routers/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/routers/items.py
--rw-r--r--   0        0        0      407 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/routers/users.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/__init__.py
--rw-r--r--   0        0        0      409 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/dependencies.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/internal/__init__.py
--rw-r--r--   0        0        0      147 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/internal/admin.py
--rw-r--r--   0        0        0      552 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/routers/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/routers/items.py
--rw-r--r--   0        0        0      407 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/routers/users.py
--rw-r--r--   0        0        0      309 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial001.py
--rw-r--r--   0        0        0      271 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial001_py310.py
--rw-r--r--   0        0        0      467 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial002.py
--rw-r--r--   0        0        0      429 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial002_py310.py
--rw-r--r--   0        0        0      362 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial003.py
--rw-r--r--   0        0        0      324 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial003_py310.py
--rw-r--r--   0        0        0      452 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial004.py
--rw-r--r--   0        0        0      408 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body/tutorial004_py310.py
--rw-r--r--   0        0        0      561 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_fields/tutorial001.py
--rw-r--r--   0        0        0      611 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_an.py
--rw-r--r--   0        0        0      563 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_an_py310.py
--rw-r--r--   0        0        0      582 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_an_py39.py
--rw-r--r--   0        0        0      523 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_py310.py
--rw-r--r--   0        0        0      596 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001.py
--rw-r--r--   0        0        0      639 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_an.py
--rw-r--r--   0        0        0      579 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      610 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      546 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_py310.py
--rw-r--r--   0        0        0      490 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial002.py
--rw-r--r--   0        0        0      446 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial002_py310.py
--rw-r--r--   0        0        0      548 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003.py
--rw-r--r--   0        0        0      604 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_an.py
--rw-r--r--   0        0        0      550 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      575 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      504 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_py310.py
--rw-r--r--   0        0        0      653 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004.py
--rw-r--r--   0        0        0      703 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_an.py
--rw-r--r--   0        0        0      643 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_an_py310.py
--rw-r--r--   0        0        0      674 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_an_py39.py
--rw-r--r--   0        0        0      603 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_py310.py
--rw-r--r--   0        0        0      407 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial005.py
--rw-r--r--   0        0        0      457 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial005_an.py
--rw-r--r--   0        0        0      409 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial005_an_py310.py
--rw-r--r--   0        0        0      428 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial005_an_py39.py
--rw-r--r--   0        0        0      369 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial005_py310.py
--rw-r--r--   0        0        0      402 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial001.py
--rw-r--r--   0        0        0      364 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial001_py310.py
--rw-r--r--   0        0        0      413 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial002.py
--rw-r--r--   0        0        0      369 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial002_py310.py
--rw-r--r--   0        0        0      407 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial002_py39.py
--rw-r--r--   0        0        0      414 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial003.py
--rw-r--r--   0        0        0      371 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial003_py310.py
--rw-r--r--   0        0        0      409 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial003_py39.py
--rw-r--r--   0        0        0      504 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial004.py
--rw-r--r--   0        0        0      455 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial004_py310.py
--rw-r--r--   0        0        0      499 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial004_py39.py
--rw-r--r--   0        0        0      517 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial005.py
--rw-r--r--   0        0        0      468 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial005_py310.py
--rw-r--r--   0        0        0      512 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial005_py39.py
--rw-r--r--   0        0        0      530 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial006.py
--rw-r--r--   0        0        0      475 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial006_py310.py
--rw-r--r--   0        0        0      519 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial006_py39.py
--rw-r--r--   0        0        0      581 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial007.py
--rw-r--r--   0        0        0      520 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial007_py310.py
--rw-r--r--   0        0        0      570 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial007_py39.py
--rw-r--r--   0        0        0      273 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial008.py
--rw-r--r--   0        0        0      248 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial008_py39.py
--rw-r--r--   0        0        0      179 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial009.py
--rw-r--r--   0        0        0      154 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial009_py39.py
--rw-r--r--   0        0        0      906 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_updates/tutorial001.py
--rw-r--r--   0        0        0      856 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_updates/tutorial001_py310.py
--rw-r--r--   0        0        0      900 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_updates/tutorial001_py39.py
--rw-r--r--   0        0        0     1060 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_updates/tutorial002.py
--rw-r--r--   0        0        0     1010 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_updates/tutorial002_py310.py
--rw-r--r--   0        0        0     1054 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/body_updates/tutorial002_py39.py
--rw-r--r--   0        0        0      281 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/conditional_openapi/tutorial001.py
--rw-r--r--   0        0        0      205 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/configure_swagger_ui/tutorial001.py
--rw-r--r--   0        0        0      216 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/configure_swagger_ui/tutorial002.py
--rw-r--r--   0        0        0      201 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/configure_swagger_ui/tutorial003.py
--rw-r--r--   0        0        0      202 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/cookie_params/tutorial001.py
--rw-r--r--   0        0        0      247 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/cookie_params/tutorial001_an.py
--rw-r--r--   0        0        0      205 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/cookie_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      218 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/cookie_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      170 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/cookie_params/tutorial001_py310.py
--rw-r--r--   0        0        0      459 2024-05-03 00:21:35.581407 fastapi_slim-0.111.0/docs_src/cors/tutorial001.py
--rw-r--r--   0        0        0     1154 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_docs_ui/tutorial001.py
--rw-r--r--   0        0        0     1175 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_docs_ui/tutorial002.py
--rw-r--r--   0        0        0      973 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_request_and_route/tutorial001.py
--rw-r--r--   0        0        0      932 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_request_and_route/tutorial002.py
--rw-r--r--   0        0        0     1042 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_request_and_route/tutorial003.py
--rw-r--r--   0        0        0      197 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial001.py
--rw-r--r--   0        0        0      215 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial001b.py
--rw-r--r--   0        0        0      352 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial002.py
--rw-r--r--   0        0        0      394 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial003.py
--rw-r--r--   0        0        0      491 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial004.py
--rw-r--r--   0        0        0      186 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial005.py
--rw-r--r--   0        0        0      199 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial006.py
--rw-r--r--   0        0        0      220 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial006b.py
--rw-r--r--   0        0        0      237 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial006c.py
--rw-r--r--   0        0        0      277 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial007.py
--rw-r--r--   0        0        0      360 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial008.py
--rw-r--r--   0        0        0      202 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial009.py
--rw-r--r--   0        0        0      217 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial009b.py
--rw-r--r--   0        0        0      451 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial009c.py
--rw-r--r--   0        0        0      205 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/custom_response/tutorial010.py
--rw-r--r--   0        0        0      312 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dataclasses/tutorial001.py
--rw-r--r--   0        0        0      552 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dataclasses/tutorial002.py
--rw-r--r--   0        0        0     1403 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dataclasses/tutorial003.py
--rw-r--r--   0        0        0      223 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/debugging/tutorial001.py
--rw-r--r--   0        0        0      442 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001.py
--rw-r--r--   0        0        0      495 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_02_an.py
--rw-r--r--   0        0        0      447 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      466 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      502 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_an.py
--rw-r--r--   0        0        0      454 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_an_py310.py
--rw-r--r--   0        0        0      473 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_an_py39.py
--rw-r--r--   0        0        0      404 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial001_py310.py
--rw-r--r--   0        0        0      656 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial002.py
--rw-r--r--   0        0        0      706 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_an.py
--rw-r--r--   0        0        0      664 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_an_py310.py
--rw-r--r--   0        0        0      677 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_an_py39.py
--rw-r--r--   0        0        0      624 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_py310.py
--rw-r--r--   0        0        0      635 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial003.py
--rw-r--r--   0        0        0      697 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_an.py
--rw-r--r--   0        0        0      655 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_an_py310.py
--rw-r--r--   0        0        0      668 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_an_py39.py
--rw-r--r--   0        0        0      603 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_py310.py
--rw-r--r--   0        0        0      639 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial004.py
--rw-r--r--   0        0        0      689 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_an.py
--rw-r--r--   0        0        0      647 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_an_py310.py
--rw-r--r--   0        0        0      660 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_an_py39.py
--rw-r--r--   0        0        0      607 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_py310.py
--rw-r--r--   0        0        0      486 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial005.py
--rw-r--r--   0        0        0      558 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial005_an.py
--rw-r--r--   0        0        0      510 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial005_an_py310.py
--rw-r--r--   0        0        0      529 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial005_an_py39.py
--rw-r--r--   0        0        0      443 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial005_py310.py
--rw-r--r--   0        0        0      583 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial006.py
--rw-r--r--   0        0        0      643 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial006_an.py
--rw-r--r--   0        0        0      633 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial006_an_py39.py
--rw-r--r--   0        0        0       99 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial007.py
--rw-r--r--   0        0        0      455 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008.py
--rw-r--r--   0        0        0      531 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008_an.py
--rw-r--r--   0        0        0      521 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008_an_py39.py
--rw-r--r--   0        0        0      735 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008b.py
--rw-r--r--   0        0        0      785 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008b_an.py
--rw-r--r--   0        0        0      775 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008b_an_py39.py
--rw-r--r--   0        0        0      660 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008c.py
--rw-r--r--   0        0        0      710 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008c_an.py
--rw-r--r--   0        0        0      700 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008c_an_py39.py
--rw-r--r--   0        0        0      694 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008d.py
--rw-r--r--   0        0        0      744 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008d_an.py
--rw-r--r--   0        0        0      734 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial008d_an_py39.py
--rw-r--r--   0        0        0      455 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial009.py
--rw-r--r--   0        0        0      292 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial010.py
--rw-r--r--   0        0        0      504 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial011.py
--rw-r--r--   0        0        0      554 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial011_an.py
--rw-r--r--   0        0        0      544 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial011_an_py39.py
--rw-r--r--   0        0        0      696 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial012.py
--rw-r--r--   0        0        0      756 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial012_an.py
--rw-r--r--   0        0        0      756 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependencies/tutorial012_an_py39.py
--rw-r--r--   0        0        0     1522 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001.py
--rw-r--r--   0        0        0     1582 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_an.py
--rw-r--r--   0        0        0     1528 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_an_py310.py
--rw-r--r--   0        0        0     1553 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_an_py39.py
--rw-r--r--   0        0        0     1478 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_py310.py
--rw-r--r--   0        0        0      461 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/encoder/tutorial001.py
--rw-r--r--   0        0        0      430 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/encoder/tutorial001_py310.py
--rw-r--r--   0        0        0      283 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/events/tutorial001.py
--rw-r--r--   0        0        0      255 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/events/tutorial002.py
--rw-r--r--   0        0        0      569 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/events/tutorial003.py
--rw-r--r--   0        0        0      737 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extending_openapi/tutorial001.py
--rw-r--r--   0        0        0      755 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001.py
--rw-r--r--   0        0        0      830 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_an.py
--rw-r--r--   0        0        0      788 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_an_py310.py
--rw-r--r--   0        0        0      801 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_an_py39.py
--rw-r--r--   0        0        0      724 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_py310.py
--rw-r--r--   0        0        0      943 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial001.py
--rw-r--r--   0        0        0      899 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial001_py310.py
--rw-r--r--   0        0        0      824 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial002.py
--rw-r--r--   0        0        0      792 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial002_py310.py
--rw-r--r--   0        0        0      644 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial003.py
--rw-r--r--   0        0        0      644 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial003_py310.py
--rw-r--r--   0        0        0      381 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial004.py
--rw-r--r--   0        0        0      356 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial004_py39.py
--rw-r--r--   0        0        0      205 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial005.py
--rw-r--r--   0        0        0      180 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/extra_models/tutorial005_py39.py
--rw-r--r--   0        0        0      117 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      139 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      111 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      519 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial001.py
--rw-r--r--   0        0        0      494 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial001_py39.py
--rw-r--r--   0        0        0      755 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial002.py
--rw-r--r--   0        0        0      730 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial002_py39.py
--rw-r--r--   0        0        0      939 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial003.py
--rw-r--r--   0        0        0      914 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial003_py39.py
--rw-r--r--   0        0        0     1066 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial004.js
--rw-r--r--   0        0        0      493 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/generate_clients/tutorial004.py
--rw-r--r--   0        0        0      446 2024-05-03 00:21:35.585407 fastapi_slim-0.111.0/docs_src/graphql/tutorial001.py
--rw-r--r--   0        0        0      299 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/handling_errors/tutorial001.py
--rw-r--r--   0        0        0      404 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/handling_errors/tutorial002.py
--rw-r--r--   0        0        0      626 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/handling_errors/tutorial003.py
--rw-r--r--   0        0        0      762 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/handling_errors/tutorial004.py
--rw-r--r--   0        0        0      667 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/handling_errors/tutorial005.py
--rw-r--r--   0        0        0      928 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/handling_errors/tutorial006.py
--rw-r--r--   0        0        0      214 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial001.py
--rw-r--r--   0        0        0      259 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial001_an.py
--rw-r--r--   0        0        0      217 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      230 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      182 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial001_py310.py
--rw-r--r--   0        0        0      260 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial002.py
--rw-r--r--   0        0        0      317 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial002_an.py
--rw-r--r--   0        0        0      261 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial002_an_py310.py
--rw-r--r--   0        0        0      288 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial002_an_py39.py
--rw-r--r--   0        0        0      228 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial002_py310.py
--rw-r--r--   0        0        0      224 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial003.py
--rw-r--r--   0        0        0      269 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial003_an.py
--rw-r--r--   0        0        0      221 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      240 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      186 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial003_py310.py
--rw-r--r--   0        0        0      218 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/header_params/tutorial003_py39.py
--rw-r--r--   0        0        0      805 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/metadata/tutorial001.py
--rw-r--r--   0        0        0      767 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/metadata/tutorial001_1.py
--rw-r--r--   0        0        0      154 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/metadata/tutorial002.py
--rw-r--r--   0        0        0      161 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/metadata/tutorial003.py
--rw-r--r--   0        0        0      693 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/metadata/tutorial004.py
--rw-r--r--   0        0        0      349 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/middleware/tutorial001.py
--rw-r--r--   0        0        0     1357 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/nosql_databases/tutorial001.py
--rw-r--r--   0        0        0     1371 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/openapi_callbacks/tutorial001.py
--rw-r--r--   0        0        0      550 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/openapi_webhooks/tutorial001.py
--rw-r--r--   0        0        0      167 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial001.py
--rw-r--r--   0        0        0      572 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial002.py
--rw-r--r--   0        0        0      148 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial003.py
--rw-r--r--   0        0        0      717 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial004.py
--rw-r--r--   0        0        0      180 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial005.py
--rw-r--r--   0        0        0     1043 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial006.py
--rw-r--r--   0        0        0      822 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial007.py
--rw-r--r--   0        0        0      789 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py
--rw-r--r--   0        0        0      406 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial001.py
--rw-r--r--   0        0        0      363 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial001_py310.py
--rw-r--r--   0        0        0      401 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial001_py39.py
--rw-r--r--   0        0        0      580 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002.py
--rw-r--r--   0        0        0      537 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002_py310.py
--rw-r--r--   0        0        0      575 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002_py39.py
--rw-r--r--   0        0        0      323 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002b.py
--rw-r--r--   0        0        0      517 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial003.py
--rw-r--r--   0        0        0      474 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial003_py310.py
--rw-r--r--   0        0        0      512 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial003_py39.py
--rw-r--r--   0        0        0      681 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial004.py
--rw-r--r--   0        0        0      638 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial004_py310.py
--rw-r--r--   0        0        0      676 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial004_py39.py
--rw-r--r--   0        0        0      741 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial005.py
--rw-r--r--   0        0        0      698 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial005_py310.py
--rw-r--r--   0        0        0      736 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial005_py39.py
--rw-r--r--   0        0        0      365 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial006.py
--rw-r--r--   0        0        0      138 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params/tutorial001.py
--rw-r--r--   0        0        0      143 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params/tutorial002.py
--rw-r--r--   0        0        0      236 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params/tutorial003.py
--rw-r--r--   0        0        0      193 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params/tutorial003b.py
--rw-r--r--   0        0        0      156 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params/tutorial004.py
--rw-r--r--   0        0        0      546 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params/tutorial005.py
--rw-r--r--   0        0        0      364 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial001.py
--rw-r--r--   0        0        0      417 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial001_an.py
--rw-r--r--   0        0        0      375 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
--rw-r--r--   0        0        0      388 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
--rw-r--r--   0        0        0      332 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      265 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial002.py
--rw-r--r--   0        0        0      321 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial002_an.py
--rw-r--r--   0        0        0      311 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
--rw-r--r--   0        0        0      268 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial003.py
--rw-r--r--   0        0        0      321 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial003_an.py
--rw-r--r--   0        0        0      311 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      280 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial004.py
--rw-r--r--   0        0        0      327 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial004_an.py
--rw-r--r--   0        0        0      317 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      298 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial005.py
--rw-r--r--   0        0        0      341 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial005_an.py
--rw-r--r--   0        0        0      331 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      345 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial006.py
--rw-r--r--   0        0        0      405 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial006_an.py
--rw-r--r--   0        0        0      395 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      162 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial001.py
--rw-r--r--   0        0        0      172 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial002.py
--rw-r--r--   0        0        0      119 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial003.py
--rw-r--r--   0        0        0      124 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial004.py
--rw-r--r--   0        0        0      143 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial005.py
--rw-r--r--   0        0        0      106 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial006.py
--rw-r--r--   0        0        0       80 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial006_py39.py
--rw-r--r--   0        0        0      131 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial007.py
--rw-r--r--   0        0        0       99 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial007_py39.py
--rw-r--r--   0        0        0      171 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial008.py
--rw-r--r--   0        0        0      145 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial008_py39.py
--rw-r--r--   0        0        0       84 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial008b.py
--rw-r--r--   0        0        0       51 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial008b_py310.py
--rw-r--r--   0        0        0      164 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial009.py
--rw-r--r--   0        0        0      131 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial009_py310.py
--rw-r--r--   0        0        0      164 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial009b.py
--rw-r--r--   0        0        0       89 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial009c.py
--rw-r--r--   0        0        0       56 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial009c_py310.py
--rw-r--r--   0        0        0      144 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial010.py
--rw-r--r--   0        0        0      498 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial011.py
--rw-r--r--   0        0        0      461 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial011_py310.py
--rw-r--r--   0        0        0      492 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial011_py39.py
--rw-r--r--   0        0        0      122 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial012.py
--rw-r--r--   0        0        0      138 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial013.py
--rw-r--r--   0        0        0      127 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/python_types/tutorial013_py39.py
--rw-r--r--   0        0        0      250 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial001.py
--rw-r--r--   0        0        0      251 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial002.py
--rw-r--r--   0        0        0      219 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial002_py310.py
--rw-r--r--   0        0        0      406 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial003.py
--rw-r--r--   0        0        0      374 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial003_py310.py
--rw-r--r--   0        0        0      468 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial004.py
--rw-r--r--   0        0        0      436 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial004_py310.py
--rw-r--r--   0        0        0      192 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial005.py
--rw-r--r--   0        0        0      301 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial006.py
--rw-r--r--   0        0        0      269 2024-05-03 00:21:35.589407 fastapi_slim-0.111.0/docs_src/query_params/tutorial006_py310.py
--rw-r--r--   0        0        0      301 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params/tutorial006b.py
--rw-r--r--   0        0        0      271 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial001.py
--rw-r--r--   0        0        0      239 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      308 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial002.py
--rw-r--r--   0        0        0      351 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial002_an.py
--rw-r--r--   0        0        0      309 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial002_an_py310.py
--rw-r--r--   0        0        0      276 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial002_py310.py
--rw-r--r--   0        0        0      329 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial003.py
--rw-r--r--   0        0        0      372 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial003_an.py
--rw-r--r--   0        0        0      330 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial003_an_py310.py
--rw-r--r--   0        0        0      343 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      290 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial003_py310.py
--rw-r--r--   0        0        0      367 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial004.py
--rw-r--r--   0        0        0      410 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial004_an.py
--rw-r--r--   0        0        0      368 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial004_an_py310.py
--rw-r--r--   0        0        0      366 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial004_an_py310_regex.py
--rw-r--r--   0        0        0      381 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      335 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial004_py310.py
--rw-r--r--   0        0        0      276 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial005.py
--rw-r--r--   0        0        0      319 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial005_an.py
--rw-r--r--   0        0        0      309 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      254 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006.py
--rw-r--r--   0        0        0      304 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006_an.py
--rw-r--r--   0        0        0      294 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      267 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006b.py
--rw-r--r--   0        0        0      310 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006b_an.py
--rw-r--r--   0        0        0      300 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006b_an_py39.py
--rw-r--r--   0        0        0      306 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006c.py
--rw-r--r--   0        0        0      349 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006c_an.py
--rw-r--r--   0        0        0      307 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006c_an_py310.py
--rw-r--r--   0        0        0      320 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006c_an_py39.py
--rw-r--r--   0        0        0      274 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006c_py310.py
--rw-r--r--   0        0        0      302 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006d.py
--rw-r--r--   0        0        0      345 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006d_an.py
--rw-r--r--   0        0        0      335 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial006d_an_py39.py
--rw-r--r--   0        0        0      336 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial007.py
--rw-r--r--   0        0        0      379 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial007_an.py
--rw-r--r--   0        0        0      337 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial007_an_py310.py
--rw-r--r--   0        0        0      350 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial007_an_py39.py
--rw-r--r--   0        0        0      304 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial007_py310.py
--rw-r--r--   0        0        0      466 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial008.py
--rw-r--r--   0        0        0      540 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial008_an.py
--rw-r--r--   0        0        0      498 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial008_an_py310.py
--rw-r--r--   0        0        0      511 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial008_an_py39.py
--rw-r--r--   0        0        0      434 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial008_py310.py
--rw-r--r--   0        0        0      313 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial009.py
--rw-r--r--   0        0        0      356 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial009_an.py
--rw-r--r--   0        0        0      314 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial009_an_py310.py
--rw-r--r--   0        0        0      327 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial009_an_py39.py
--rw-r--r--   0        0        0      281 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial009_py310.py
--rw-r--r--   0        0        0      574 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010.py
--rw-r--r--   0        0        0      664 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_an.py
--rw-r--r--   0        0        0      622 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_an_py310.py
--rw-r--r--   0        0        0      635 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_an_py39.py
--rw-r--r--   0        0        0      542 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_py310.py
--rw-r--r--   0        0        0      227 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial011.py
--rw-r--r--   0        0        0      272 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial011_an.py
--rw-r--r--   0        0        0      224 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial011_an_py310.py
--rw-r--r--   0        0        0      237 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial011_an_py39.py
--rw-r--r--   0        0        0      189 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial011_py310.py
--rw-r--r--   0        0        0      221 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial011_py39.py
--rw-r--r--   0        0        0      217 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial012.py
--rw-r--r--   0        0        0      262 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial012_an.py
--rw-r--r--   0        0        0      227 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial012_an_py39.py
--rw-r--r--   0        0        0      192 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial012_py39.py
--rw-r--r--   0        0        0      175 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial013.py
--rw-r--r--   0        0        0      220 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial013_an.py
--rw-r--r--   0        0        0      210 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial013_an_py39.py
--rw-r--r--   0        0        0      330 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial014.py
--rw-r--r--   0        0        0      373 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial014_an.py
--rw-r--r--   0        0        0      331 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial014_an_py310.py
--rw-r--r--   0        0        0      344 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial014_an_py39.py
--rw-r--r--   0        0        0      298 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial014_py310.py
--rw-r--r--   0        0        0      282 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001.py
--rw-r--r--   0        0        0      508 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02.py
--rw-r--r--   0        0        0      553 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02_an.py
--rw-r--r--   0        0        0      505 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      524 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      470 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02_py310.py
--rw-r--r--   0        0        0      371 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_03.py
--rw-r--r--   0        0        0      431 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_03_an.py
--rw-r--r--   0        0        0      421 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_03_an_py39.py
--rw-r--r--   0        0        0      332 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_an.py
--rw-r--r--   0        0        0      322 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      811 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial002.py
--rw-r--r--   0        0        0      861 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial002_an.py
--rw-r--r--   0        0        0      826 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial002_an_py39.py
--rw-r--r--   0        0        0      786 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial002_py39.py
--rw-r--r--   0        0        0      913 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial003.py
--rw-r--r--   0        0        0      987 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial003_an.py
--rw-r--r--   0        0        0      952 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial003_an_py39.py
--rw-r--r--   0        0        0      888 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_files/tutorial003_py39.py
--rw-r--r--   0        0        0      173 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_forms/tutorial001.py
--rw-r--r--   0        0        0      233 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_forms/tutorial001_an.py
--rw-r--r--   0        0        0      223 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_forms/tutorial001_an_py39.py
--rw-r--r--   0        0        0      317 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_forms_and_files/tutorial001.py
--rw-r--r--   0        0        0      396 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_forms_and_files/tutorial001_an.py
--rw-r--r--   0        0        0      386 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/request_forms_and_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      391 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_change_status_code/tutorial001.py
--rw-r--r--   0        0        0      344 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_cookies/tutorial001.py
--rw-r--r--   0        0        0      272 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_cookies/tutorial002.py
--rw-r--r--   0        0        0      505 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_directly/tutorial001.py
--rw-r--r--   0        0        0      354 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_directly/tutorial002.py
--rw-r--r--   0        0        0      309 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_headers/tutorial001.py
--rw-r--r--   0        0        0      222 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_headers/tutorial002.py
--rw-r--r--   0        0        0      562 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial001.py
--rw-r--r--   0        0        0      513 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial001_01.py
--rw-r--r--   0        0        0      469 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial001_01_py310.py
--rw-r--r--   0        0        0      507 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial001_01_py39.py
--rw-r--r--   0        0        0      537 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial001_py310.py
--rw-r--r--   0        0        0      556 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial001_py39.py
--rw-r--r--   0        0        0      350 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial002.py
--rw-r--r--   0        0        0      318 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial002_py310.py
--rw-r--r--   0        0        0      450 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003.py
--rw-r--r--   0        0        0      349 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_01.py
--rw-r--r--   0        0        0      317 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_01_py310.py
--rw-r--r--   0        0        0      381 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_02.py
--rw-r--r--   0        0        0      241 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_03.py
--rw-r--r--   0        0        0      384 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_04.py
--rw-r--r--   0        0        0      352 2024-05-03 00:21:35.593407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_04_py310.py
--rw-r--r--   0        0        0      405 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_05.py
--rw-r--r--   0        0        0      373 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_05_py310.py
--rw-r--r--   0        0        0      431 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial003_py310.py
--rw-r--r--   0        0        0      633 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial004.py
--rw-r--r--   0        0        0      595 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial004_py310.py
--rw-r--r--   0        0        0      627 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial004_py39.py
--rw-r--r--   0        0        0      848 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial005.py
--rw-r--r--   0        0        0      816 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial005_py310.py
--rw-r--r--   0        0        0      848 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial006.py
--rw-r--r--   0        0        0      816 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_model/tutorial006_py310.py
--rw-r--r--   0        0        0      145 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_status_code/tutorial001.py
--rw-r--r--   0        0        0      173 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/response_status_code/tutorial002.py
--rw-r--r--   0        0        0      684 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001.py
--rw-r--r--   0        0        0      669 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001_pv1.py
--rw-r--r--   0        0        0      646 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001_py310.py
--rw-r--r--   0        0        0      631 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001_py310_pv1.py
--rw-r--r--   0        0        0      517 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial002.py
--rw-r--r--   0        0        0      479 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial002_py310.py
--rw-r--r--   0        0        0      612 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003.py
--rw-r--r--   0        0        0      721 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_an.py
--rw-r--r--   0        0        0      673 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_an_py310.py
--rw-r--r--   0        0        0      692 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_an_py39.py
--rw-r--r--   0        0        0      574 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_py310.py
--rw-r--r--   0        0        0      824 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004.py
--rw-r--r--   0        0        0      965 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_an.py
--rw-r--r--   0        0        0      917 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_an_py310.py
--rw-r--r--   0        0        0      936 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_an_py39.py
--rw-r--r--   0        0        0      786 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_py310.py
--rw-r--r--   0        0        0     1386 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005.py
--rw-r--r--   0        0        0     1571 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_an.py
--rw-r--r--   0        0        0     1523 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_an_py310.py
--rw-r--r--   0        0        0     1542 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_an_py39.py
--rw-r--r--   0        0        0     1348 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_py310.py
--rw-r--r--   0        0        0      269 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial001.py
--rw-r--r--   0        0        0      319 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial001_an.py
--rw-r--r--   0        0        0      309 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial001_an_py39.py
--rw-r--r--   0        0        0      755 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial002.py
--rw-r--r--   0        0        0      815 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial002_an.py
--rw-r--r--   0        0        0      761 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial002_an_py310.py
--rw-r--r--   0        0        0      786 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial002_an_py39.py
--rw-r--r--   0        0        0      711 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial002_py310.py
--rw-r--r--   0        0        0     2494 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial003.py
--rw-r--r--   0        0        0     2588 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial003_an.py
--rw-r--r--   0        0        0     2534 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial003_an_py310.py
--rw-r--r--   0        0        0     2559 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial003_an_py39.py
--rw-r--r--   0        0        0     2450 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial003_py310.py
--rw-r--r--   0        0        0     4134 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial004.py
--rw-r--r--   0        0        0     4245 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial004_an.py
--rw-r--r--   0        0        0     4179 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial004_an_py310.py
--rw-r--r--   0        0        0     4216 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial004_an_py39.py
--rw-r--r--   0        0        0     4079 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial004_py310.py
--rw-r--r--   0        0        0     5270 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial005.py
--rw-r--r--   0        0        0     5377 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial005_an.py
--rw-r--r--   0        0        0     5305 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial005_an_py310.py
--rw-r--r--   0        0        0     5348 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial005_an_py39.py
--rw-r--r--   0        0        0     5209 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial005_py310.py
--rw-r--r--   0        0        0     5264 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial005_py39.py
--rw-r--r--   0        0        0      321 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial006.py
--rw-r--r--   0        0        0      371 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial006_an.py
--rw-r--r--   0        0        0      361 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial006_an_py39.py
--rw-r--r--   0        0        0     1116 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial007.py
--rw-r--r--   0        0        0     1183 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial007_an.py
--rw-r--r--   0        0        0     1172 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/security/tutorial007_an_py39.py
--rw-r--r--   0        0        0      489 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial001.py
--rw-r--r--   0        0        0      451 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial001_py310.py
--rw-r--r--   0        0        0      483 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial001_py39.py
--rw-r--r--   0        0        0      524 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial002.py
--rw-r--r--   0        0        0      486 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial002_py310.py
--rw-r--r--   0        0        0      518 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial002_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app01/__init__.py
--rw-r--r--   0        0        0      183 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app01/config.py
--rw-r--r--   0        0        0      267 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app01/main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02/__init__.py
--rw-r--r--   0        0        0      159 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02/config.py
--rw-r--r--   0        0        0      406 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02/main.py
--rw-r--r--   0        0        0      515 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an/__init__.py
--rw-r--r--   0        0        0      159 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an/config.py
--rw-r--r--   0        0        0      456 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an/main.py
--rw-r--r--   0        0        0      515 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an_py39/__init__.py
--rw-r--r--   0        0        0      159 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an_py39/config.py
--rw-r--r--   0        0        0      445 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an_py39/main.py
--rw-r--r--   0        0        0      515 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app02_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03/__init__.py
--rw-r--r--   0        0        0      204 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03/config.py
--rw-r--r--   0        0        0      412 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03/main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an/__init__.py
--rw-r--r--   0        0        0      235 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an/config.py
--rw-r--r--   0        0        0      195 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an/config_pv1.py
--rw-r--r--   0        0        0      451 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an/main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an_py39/__init__.py
--rw-r--r--   0        0        0      204 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an_py39/config.py
--rw-r--r--   0        0        0      462 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/app03_an_py39/main.py
--rw-r--r--   0        0        0      419 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/tutorial001.py
--rw-r--r--   0        0        0      410 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/settings/tutorial001_pv1.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/__init__.py
--rw-r--r--   0        0        0     1928 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/crud.py
--rw-r--r--   0        0        0      461 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/database.py
--rw-r--r--   0        0        0     1632 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/main.py
--rw-r--r--   0        0        0      710 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/models.py
--rw-r--r--   0        0        0      502 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/schemas.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/tests/__init__.py
--rw-r--r--   0        0        0     1260 2024-05-03 00:21:35.597407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/__init__.py
--rw-r--r--   0        0        0     1903 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/crud.py
--rw-r--r--   0        0        0      461 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/database.py
--rw-r--r--   0        0        0     1607 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/main.py
--rw-r--r--   0        0        0      710 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/models.py
--rw-r--r--   0        0        0      464 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/schemas.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/tests/__init__.py
--rw-r--r--   0        0        0     1200 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/__init__.py
--rw-r--r--   0        0        0     1903 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/alt_main.py
--rw-r--r--   0        0        0     1061 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/crud.py
--rw-r--r--   0        0        0      461 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/database.py
--rw-r--r--   0        0        0     1607 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/main.py
--rw-r--r--   0        0        0      710 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/models.py
--rw-r--r--   0        0        0      496 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/schemas.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/tests/__init__.py
--rw-r--r--   0        0        0     1200 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/__init__.py
--rw-r--r--   0        0        0      843 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/crud.py
--rw-r--r--   0        0        0      662 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/database.py
--rw-r--r--   0        0        0     2210 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/main.py
--rw-r--r--   0        0        0      465 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/models.py
--rw-r--r--   0        0        0      868 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/schemas.py
--rw-r--r--   0        0        0      159 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/static_files/tutorial001.py
--rw-r--r--   0        0        0      274 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/sub_applications/tutorial001.py
--rw-r--r--   0        0        0       25 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/templates/static/styles.css
--rw-r--r--   0        0        0      235 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/templates/templates/item.html
--rw-r--r--   0        0        0      521 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/templates/tutorial001.py
--rw-r--r--   0        0        0      230 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/using_request_directly/tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/__init__.py
--rw-r--r--   0        0        0     1432 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial001.py
--rw-r--r--   0        0        0     2842 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial002.py
--rw-r--r--   0        0        0     2909 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial002_an.py
--rw-r--r--   0        0        0     2855 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial002_an_py310.py
--rw-r--r--   0        0        0     2880 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial002_an_py39.py
--rw-r--r--   0        0        0     2798 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial002_py310.py
--rw-r--r--   0        0        0     2574 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial003.py
--rw-r--r--   0        0        0     2549 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/websockets/tutorial003_py39.py
--rw-r--r--   0        0        0      443 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/docs_src/wsgi/tutorial001.py
--rw-r--r--   0        0        0     1081 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/__init__.py
--rw-r--r--   0        0        0    23134 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/_compat.py
--rw-r--r--   0        0        0   176342 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/applications.py
--rw-r--r--   0        0        0     1768 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/background.py
--rw-r--r--   0        0        0     1403 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/concurrency.py
--rw-r--r--   0        0        0     5766 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/datastructures.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/dependencies/__init__.py
--rw-r--r--   0        0        0     2494 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/dependencies/models.py
--rw-r--r--   0        0        0    30241 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/dependencies/utils.py
--rw-r--r--   0        0        0    11068 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/encoders.py
--rw-r--r--   0        0        0     1332 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/exception_handlers.py
--rw-r--r--   0        0        0     4969 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/exceptions.py
--rw-r--r--   0        0        0       54 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/logger.py
--rw-r--r--   0        0        0       58 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/middleware/__init__.py
--rw-r--r--   0        0        0       79 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/middleware/cors.py
--rw-r--r--   0        0        0       79 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/middleware/gzip.py
--rw-r--r--   0        0        0      115 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/middleware/httpsredirect.py
--rw-r--r--   0        0        0      109 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0      153 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/openapi/constants.py
--rw-r--r--   0        0        0    10356 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/openapi/docs.py
--rw-r--r--   0        0        0    15397 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/openapi/models.py
--rw-r--r--   0        0        0    22286 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/openapi/utils.py
--rw-r--r--   0        0        0    64005 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/param_functions.py
--rw-r--r--   0        0        0    28191 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/params.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/py.typed
--rw-r--r--   0        0        0      142 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/requests.py
--rw-r--r--   0        0        0     1761 2024-05-03 00:21:35.601407 fastapi_slim-0.111.0/fastapi/responses.py
--rw-r--r--   0        0        0   174150 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/routing.py
--rw-r--r--   0        0        0      881 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/__init__.py
--rw-r--r--   0        0        0     9368 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/api_key.py
--rw-r--r--   0        0        0      141 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/base.py
--rw-r--r--   0        0        0    13506 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/http.py
--rw-r--r--   0        0        0    21583 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/oauth2.py
--rw-r--r--   0        0        0     2722 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/security/utils.py
--rw-r--r--   0        0        0       69 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/staticfiles.py
--rw-r--r--   0        0        0       76 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/templating.py
--rw-r--r--   0        0        0       66 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/testclient.py
--rw-r--r--   0        0        0      383 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/types.py
--rw-r--r--   0        0        0     8035 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/utils.py
--rw-r--r--   0        0        0      222 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/fastapi/websockets.py
--rw-r--r--   0        0        0     1722 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/pdm_build.py
--rw-r--r--   0        0        0     7355 2024-05-03 00:21:41.933448 fastapi_slim-0.111.0/pyproject.toml
--rw-r--r--   0        0        0       52 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/requirements-docs-tests.txt
--rw-r--r--   0        0        0      465 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/requirements-docs.txt
--rw-r--r--   0        0        0      496 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/requirements-tests.txt
--rw-r--r--   0        0        0      128 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/requirements.txt
--rw-r--r--   0        0        0    11141 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/docs.py
--rwxr-xr-x   0        0        0      112 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/format.sh
--rwxr-xr-x   0        0        0      125 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/lint.sh
--rw-r--r--   0        0        0     5216 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/mkdocs_hooks.py
--rw-r--r--   0        0        0      819 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image01.py
--rw-r--r--   0        0        0      873 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image02.py
--rw-r--r--   0        0        0      892 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image03.py
--rw-r--r--   0        0        0      881 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image04.py
--rw-r--r--   0        0        0      829 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image05.py
--rwxr-xr-x   0        0        0      124 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0       99 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/__init__.py
--rw-r--r--   0        0        0     4452 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/main.py
--rw-r--r--   0        0        0     3688 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_properties.py
--rw-r--r--   0        0        0     4301 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_properties_bool.py
--rw-r--r--   0        0        0     1207 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1117 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     5895 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2974 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2882 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3560 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     5229 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     2148 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0    10493 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_annotated.py
--rw-r--r--   0        0        0    53491 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_application.py
--rw-r--r--   0        0        0      457 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_callable_endpoint.py
--rw-r--r--   0        0        0     2826 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_compat.py
--rw-r--r--   0        0        0     2264 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_computed_fields.py
--rw-r--r--   0        0        0     2892 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_custom_middleware_exception.py
--rw-r--r--   0        0        0     3131 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_custom_route_class.py
--rw-r--r--   0        0        0     1246 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_custom_schema_fields.py
--rw-r--r--   0        0        0     1091 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_custom_swagger_ui_redirect.py
--rw-r--r--   0        0        0     2026 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_datastructures.py
--rw-r--r--   0        0        0     1604 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_datetime_custom_encoder.py
--rw-r--r--   0        0        0     5365 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_default_response_class.py
--rw-r--r--   0        0        0     5117 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_default_response_class_router.py
--rw-r--r--   0        0        0     2787 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_cache.py
--rw-r--r--   0        0        0     3379 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_class.py
--rw-r--r--   0        0        0    11869 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_contextmanager.py
--rw-r--r--   0        0        0     1560 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_contextvars.py
--rw-r--r--   0        0        0     8577 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_duplicates.py
--rw-r--r--   0        0        0     1961 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_normal_exceptions.py
--rw-r--r--   0        0        0    15816 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_overrides.py
--rw-r--r--   0        0        0     1463 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_dependency_security_overrides.py
--rw-r--r--   0        0        0     1193 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_deprecated_openapi_prefix.py
--rw-r--r--   0        0        0     2159 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_duplicate_models_openapi.py
--rw-r--r--   0        0        0      805 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_empty_router.py
--rw-r--r--   0        0        0     3458 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_enforce_once_required_parameter.py
--rw-r--r--   0        0        0     1918 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_exception_handlers.py
--rw-r--r--   0        0        0    14029 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_extra_routes.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model/__init__.py
--rw-r--r--   0        0        0      784 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model/app_pv1.py
--rw-r--r--   0        0        0     4612 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py
--rw-r--r--   0        0        0     6461 2024-05-03 00:21:35.605407 fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model_pv2.py
--rw-r--r--   0        0        0     1202 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0    68299 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_generate_unique_id_function.py
--rw-r--r--   0        0        0     1881 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_generic_parameterless_depends.py
--rw-r--r--   0        0        0     3744 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_get_request_body.py
--rw-r--r--   0        0        0      972 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_http_connection_injection.py
--rw-r--r--   0        0        0      496 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_include_route.py
--rw-r--r--   0        0        0   367192 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_include_router_defaults_overrides.py
--rw-r--r--   0        0        0    13619 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_infer_param_optionality.py
--rw-r--r--   0        0        0     3085 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_inherited_custom_class.py
--rw-r--r--   0        0        0     1704 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_invalid_path_param.py
--rw-r--r--   0        0        0     1248 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     9182 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_jsonable_encoder.py
--rw-r--r--   0        0        0     2506 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_local_docs.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_modules_same_name_body/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_modules_same_name_body/app/__init__.py
--rw-r--r--   0        0        0      160 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_modules_same_name_body/app/a.py
--rw-r--r--   0        0        0      161 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_modules_same_name_body/app/b.py
--rw-r--r--   0        0        0      150 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_modules_same_name_body/app/main.py
--rw-r--r--   0        0        0     5782 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_modules_same_name_body/test_main.py
--rw-r--r--   0        0        0     7821 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_multi_body_errors.py
--rw-r--r--   0        0        0     4610 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_multi_query_errors.py
--rw-r--r--   0        0        0     3777 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_multipart_installation.py
--rw-r--r--   0        0        0      786 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_no_swagger_ui_redirect.py
--rw-r--r--   0        0        0    17438 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_openapi_examples.py
--rw-r--r--   0        0        0     4847 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_openapi_query_parameter_extension.py
--rw-r--r--   0        0        0     1133 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_openapi_route_extensions.py
--rw-r--r--   0        0        0    18887 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_openapi_separate_input_output_schemas.py
--rw-r--r--   0        0        0     2001 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_openapi_servers.py
--rw-r--r--   0        0        0      934 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_operations_signatures.py
--rw-r--r--   0        0        0      562 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_orjson_response_class.py
--rw-r--r--   0        0        0      636 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_param_class.py
--rw-r--r--   0        0        0     3137 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_param_in_path_and_dependency.py
--rw-r--r--   0        0        0     7611 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_param_include_in_schema.py
--rw-r--r--   0        0        0     3414 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_params_repr.py
--rw-r--r--   0        0        0    35209 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_path.py
--rw-r--r--   0        0        0     3362 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_put_no_body.py
--rw-r--r--   0        0        0    11638 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_query.py
--rw-r--r--   0        0        0     2415 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_read_with_orm_mode.py
--rw-r--r--   0        0        0     6344 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_regex_deprecated_body.py
--rw-r--r--   0        0        0     5595 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_regex_deprecated_params.py
--rw-r--r--   0        0        0      792 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_repeated_cookie_headers.py
--rw-r--r--   0        0        0     3248 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_repeated_dependency_schema.py
--rw-r--r--   0        0        0     3745 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_repeated_parameter_alias.py
--rw-r--r--   0        0        0     3208 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_reponse_set_reponse_code_empty.py
--rw-r--r--   0        0        0     6509 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_request_body_parameters_media_type.py
--rw-r--r--   0        0        0     1530 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_required_noneable.py
--rw-r--r--   0        0        0    11379 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_by_alias.py
--rw-r--r--   0        0        0      589 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_change_status_code.py
--rw-r--r--   0        0        0     3415 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_class_no_mediatype.py
--rw-r--r--   0        0        0     3315 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_code_no_body.py
--rw-r--r--   0        0        0    48837 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_model_as_return_annotation.py
--rw-r--r--   0        0        0     1726 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_model_data_filter.py
--rw-r--r--   0        0        0     1746 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_model_data_filter_no_inheritance.py
--rw-r--r--   0        0        0     4118 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_model_include_exclude.py
--rw-r--r--   0        0        0     1124 2024-05-03 00:21:35.609407 fastapi_slim-0.111.0/tests/test_response_model_invalid.py
--rw-r--r--   0        0        0     5379 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_response_model_sub_types.py
--rw-r--r--   0        0        0     1510 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_route_scope.py
--rw-r--r--   0        0        0     3295 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_router_events.py
--rw-r--r--   0        0        0      484 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_router_prefix_with_template.py
--rw-r--r--   0        0        0      974 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_router_redirect_slashes.py
--rw-r--r--   0        0        0    38576 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_schema_extra_examples.py
--rw-r--r--   0        0        0     1944 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_cookie.py
--rw-r--r--   0        0        0     2112 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_cookie_description.py
--rw-r--r--   0        0        0     2146 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1884 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_header.py
--rw-r--r--   0        0        0     2052 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_header_description.py
--rw-r--r--   0        0        0     2082 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_header_optional.py
--rw-r--r--   0        0        0     1863 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_query.py
--rw-r--r--   0        0        0     2023 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_query_description.py
--rw-r--r--   0        0        0     2061 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_api_key_query_optional.py
--rw-r--r--   0        0        0     1787 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_base.py
--rw-r--r--   0        0        0     1973 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_base_description.py
--rw-r--r--   0        0        0     1932 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_base_optional.py
--rw-r--r--   0        0        0     2671 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_basic_optional.py
--rw-r--r--   0        0        0     2654 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_basic_realm.py
--rw-r--r--   0        0        0     2830 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_basic_realm_description.py
--rw-r--r--   0        0        0     2065 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_bearer.py
--rw-r--r--   0        0        0     2255 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_bearer_description.py
--rw-r--r--   0        0        0     2194 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_bearer_optional.py
--rw-r--r--   0        0        0     2090 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_digest.py
--rw-r--r--   0        0        0     2266 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_digest_description.py
--rw-r--r--   0        0        0     2233 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_http_digest_optional.py
--rw-r--r--   0        0        0    11002 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2.py
--rw-r--r--   0        0        0     2338 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2442 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0    11043 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2_optional.py
--rw-r--r--   0        0        0    11183 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2_optional_description.py
--rw-r--r--   0        0        0     2147 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2289 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0     2290 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_openid_connect.py
--rw-r--r--   0        0        0     2409 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_openid_connect_description.py
--rw-r--r--   0        0        0     2488 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_security_openid_connect_optional.py
--rw-r--r--   0        0        0     1414 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_serialize_response.py
--rw-r--r--   0        0        0     4998 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_serialize_response_dataclass.py
--rw-r--r--   0        0        0     4276 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_serialize_response_model.py
--rw-r--r--   0        0        0     2071 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_skip_defaults.py
--rw-r--r--   0        0        0     7550 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_starlette_exception.py
--rw-r--r--   0        0        0     1710 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_starlette_urlconvertors.py
--rw-r--r--   0        0        0    14142 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_sub_callbacks.py
--rw-r--r--   0        0        0      718 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_swagger_ui_init_oauth.py
--rw-r--r--   0        0        0    12068 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tuples.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/__init__.py
--rw-r--r--   0        0        0     4432 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py
--rw-r--r--   0        0        0     4740 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py
--rw-r--r--   0        0        0     4656 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py
--rw-r--r--   0        0        0     4935 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/__init__.py
--rw-r--r--   0        0        0      546 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
--rw-r--r--   0        0        0      549 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
--rw-r--r--   0        0        0      741 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0      737 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0      738 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_advanced_middleware/__init__.py
--rw-r--r--   0        0        0      474 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
--rw-r--r--   0        0        0      570 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
--rw-r--r--   0        0        0      665 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_async_sql_databases/__init__.py
--rw-r--r--   0        0        0     6122 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_async_tests/__init__.py
--rw-r--r--   0        0        0      143 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_async_tests/test_main.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/__init__.py
--rw-r--r--   0        0        0      578 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py
--rw-r--r--   0        0        0      568 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py
--rw-r--r--   0        0        0      571 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
--rw-r--r--   0        0        0      631 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0      628 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0      628 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/__init__.py
--rw-r--r--   0        0        0     1053 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
--rw-r--r--   0        0        0     1032 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
--rw-r--r--   0        0        0     1688 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
--rw-r--r--   0        0        0     1656 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/__init__.py
--rw-r--r--   0        0        0    25140 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/test_main.py
--rw-r--r--   0        0        0    25143 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/test_main_an.py
--rw-r--r--   0        0        0    25481 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_body/__init__.py
--rw-r--r--   0        0        0    15092 2024-05-03 00:21:35.613407 fastapi_slim-0.111.0/tests/test_tutorial/test_body/test_tutorial001.py
--rw-r--r--   0        0        0    15340 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/__init__.py
--rw-r--r--   0        0        0     7341 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001.py
--rw-r--r--   0        0        0     7344 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
--rw-r--r--   0        0        0     7436 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7430 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7433 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/__init__.py
--rw-r--r--   0        0        0     7698 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
--rw-r--r--   0        0        0     7701 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     7806 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7799 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7803 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     9660 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
--rw-r--r--   0        0        0     9663 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     9755 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     9749 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     9752 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_nested_models/__init__.py
--rw-r--r--   0        0        0     4343 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
--rw-r--r--   0        0        0     4417 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/__init__.py
--rw-r--r--   0        0        0    12040 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/test_tutorial001.py
--rw-r--r--   0        0        0    12111 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
--rw-r--r--   0        0        0    12105 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_conditional_openapi/__init__.py
--rw-r--r--   0        0        0     1799 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/__init__.py
--rw-r--r--   0        0        0     1415 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py
--rw-r--r--   0        0        0     1562 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py
--rw-r--r--   0        0        0     1534 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/__init__.py
--rw-r--r--   0        0        0     4017 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py
--rw-r--r--   0        0        0     4020 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     4155 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     4150 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     4149 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cors/__init__.py
--rw-r--r--   0        0        0     1278 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_cors/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_docs_ui/__init__.py
--rw-r--r--   0        0        0     1358 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py
--rw-r--r--   0        0        0     1249 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/__init__.py
--rw-r--r--   0        0        0      886 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
--rw-r--r--   0        0        0     1245 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
--rw-r--r--   0        0        0      526 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/__init__.py
--rw-r--r--   0        0        0     1025 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial001.py
--rw-r--r--   0        0        0     1026 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py
--rw-r--r--   0        0        0     1221 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial004.py
--rw-r--r--   0        0        0      980 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial005.py
--rw-r--r--   0        0        0     1059 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial006.py
--rw-r--r--   0        0        0      899 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py
--rw-r--r--   0        0        0      899 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py
--rw-r--r--   0        0        0      264 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial007.py
--rw-r--r--   0        0        0      487 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial008.py
--rw-r--r--   0        0        0      487 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial009.py
--rw-r--r--   0        0        0      490 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial009b.py
--rw-r--r--   0        0        0      239 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial009c.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/__init__.py
--rw-r--r--   0        0        0     5289 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py
--rw-r--r--   0        0        0     3574 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py
--rw-r--r--   0        0        0    12356 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/__init__.py
--rw-r--r--   0        0        0     7219 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     7222 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     7402 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7398 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7399 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5551 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004.py
--rw-r--r--   0        0        0     5554 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
--rw-r--r--   0        0        0     5734 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5730 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5731 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
--rw-r--r--   0        0        0     5119 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial006.py
--rw-r--r--   0        0        0     5122 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
--rw-r--r--   0        0        0     5400 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0      697 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008b.py
--rw-r--r--   0        0        0      700 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py
--rw-r--r--   0        0        0      918 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py
--rw-r--r--   0        0        0     1166 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008c.py
--rw-r--r--   0        0        0     1172 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py
--rw-r--r--   0        0        0     1263 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py
--rw-r--r--   0        0        0     1226 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008d.py
--rw-r--r--   0        0        0     1235 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py
--rw-r--r--   0        0        0     1331 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py
--rw-r--r--   0        0        0     8638 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial012.py
--rw-r--r--   0        0        0     8641 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
--rw-r--r--   0        0        0     9039 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_events/__init__.py
--rw-r--r--   0        0        0     3638 2024-05-03 00:21:35.617407 fastapi_slim-0.111.0/tests/test_tutorial/test_events/test_tutorial001.py
--rw-r--r--   0        0        0     1414 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_events/test_tutorial002.py
--rw-r--r--   0        0        0     3684 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_events/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extending_openapi/__init__.py
--rw-r--r--   0        0        0     1545 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/__init__.py
--rw-r--r--   0        0        0     6971 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
--rw-r--r--   0        0        0     6974 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     7166 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     7162 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7163 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/__init__.py
--rw-r--r--   0        0        0     5195 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial003.py
--rw-r--r--   0        0        0     5418 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
--rw-r--r--   0        0        0     1981 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial004.py
--rw-r--r--   0        0        0     2169 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
--rw-r--r--   0        0        0     1480 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial005.py
--rw-r--r--   0        0        0     1668 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0     1205 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_generate_clients/__init__.py
--rw-r--r--   0        0        0     7247 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/__init__.py
--rw-r--r--   0        0        0     3298 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py
--rw-r--r--   0        0        0     3371 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py
--rw-r--r--   0        0        0     3294 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py
--rw-r--r--   0        0        0     3800 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py
--rw-r--r--   0        0        0     4429 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py
--rw-r--r--   0        0        0     4072 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/__init__.py
--rw-r--r--   0        0        0     3869 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001.py
--rw-r--r--   0        0        0     3872 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     4052 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     4049 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     4095 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002.py
--rw-r--r--   0        0        0     4098 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py
--rw-r--r--   0        0        0     4278 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     4349 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     4348 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
--rw-r--r--   0        0        0     4240 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003.py
--rw-r--r--   0        0        0     4225 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     4405 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     4401 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     4402 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/__init__.py
--rw-r--r--   0        0        0     1764 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/test_tutorial001.py
--rw-r--r--   0        0        0     1728 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/test_tutorial001_1.py
--rw-r--r--   0        0        0     2077 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_openapi_callbacks/__init__.py
--rw-r--r--   0        0        0     9216 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_openapi_webhooks/__init__.py
--rw-r--r--   0        0        0     4492 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
--rw-r--r--   0        0        0     1020 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
--rw-r--r--   0        0        0      575 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
--rw-r--r--   0        0        0     8915 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
--rw-r--r--   0        0        0     1034 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     1987 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
--rw-r--r--   0        0        0     3419 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
--rw-r--r--   0        0        0     3266 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/__init__.py
--rw-r--r--   0        0        0     1722 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
--rw-r--r--   0        0        0     8900 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     9102 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
--rw-r--r--   0        0        0     9097 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2405 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_params/__init__.py
--rw-r--r--   0        0        0     3369 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_params/test_tutorial004.py
--rw-r--r--   0        0        0     5142 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_path_params/test_tutorial005.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/__init__.py
--rw-r--r--   0        0        0     4072 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/test_tutorial005.py
--rw-r--r--   0        0        0     6285 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/test_tutorial006.py
--rw-r--r--   0        0        0     6364 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/__init__.py
--rw-r--r--   0        0        0     6388 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
--rw-r--r--   0        0        0     6391 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
--rw-r--r--   0        0        0     6496 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
--rw-r--r--   0        0        0     6489 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
--rw-r--r--   0        0        0     6493 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
--rw-r--r--   0        0        0     4017 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
--rw-r--r--   0        0        0     4020 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
--rw-r--r--   0        0        0     4243 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
--rw-r--r--   0        0        0     4238 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
--rw-r--r--   0        0        0     4240 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
--rw-r--r--   0        0        0     4235 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
--rw-r--r--   0        0        0     3485 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
--rw-r--r--   0        0        0     3488 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
--rw-r--r--   0        0        0     3706 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0     3703 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
--rw-r--r--   0        0        0     3434 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
--rw-r--r--   0        0        0     3437 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
--rw-r--r--   0        0        0     3655 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
--rw-r--r--   0        0        0     2937 2024-05-03 00:21:35.621407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
--rw-r--r--   0        0        0     2940 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
--rw-r--r--   0        0        0     3163 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
--rw-r--r--   0        0        0     3162 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
--rw-r--r--   0        0        0     3160 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/__init__.py
--rw-r--r--   0        0        0     7886 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001.py
--rw-r--r--   0        0        0     8388 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py
--rw-r--r--   0        0        0     8391 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
--rw-r--r--   0        0        0     8660 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
--rw-r--r--   0        0        0     8653 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
--rw-r--r--   0        0        0     8657 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
--rw-r--r--   0        0        0     6133 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py
--rw-r--r--   0        0        0     6136 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
--rw-r--r--   0        0        0     6300 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
--rw-r--r--   0        0        0     7708 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     7935 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8679 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002.py
--rw-r--r--   0        0        0     8682 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py
--rw-r--r--   0        0        0     9076 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     9255 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
--rw-r--r--   0        0        0     7311 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003.py
--rw-r--r--   0        0        0     7314 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py
--rw-r--r--   0        0        0     7830 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7827 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/__init__.py
--rw-r--r--   0        0        0     7630 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/test_tutorial001.py
--rw-r--r--   0        0        0     7633 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
--rw-r--r--   0        0        0     7743 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/__init__.py
--rw-r--r--   0        0        0    10042 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
--rw-r--r--   0        0        0    10045 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
--rw-r--r--   0        0        0    10155 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_change_status_code/__init__.py
--rw-r--r--   0        0        0      521 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_cookies/__init__.py
--rw-r--r--   0        0        0      403 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_cookies/test_tutorial001.py
--rw-r--r--   0        0        0      414 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_cookies/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_headers/__init__.py
--rw-r--r--   0        0        0      426 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_headers/test_tutorial001.py
--rw-r--r--   0        0        0      378 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_headers/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/__init__.py
--rw-r--r--   0        0        0     5764 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003.py
--rw-r--r--   0        0        0     5770 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py
--rw-r--r--   0        0        0     5962 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
--rw-r--r--   0        0        0     3476 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py
--rw-r--r--   0        0        0     1090 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py
--rw-r--r--   0        0        0      236 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_04.py
--rw-r--r--   0        0        0      289 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
--rw-r--r--   0        0        0     3476 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py
--rw-r--r--   0        0        0     3699 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
--rw-r--r--   0        0        0     5956 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
--rw-r--r--   0        0        0     5108 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial004.py
--rw-r--r--   0        0        0     5288 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
--rw-r--r--   0        0        0     5284 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
--rw-r--r--   0        0        0     6154 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial005.py
--rw-r--r--   0        0        0     6377 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
--rw-r--r--   0        0        0     6154 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial006.py
--rw-r--r--   0        0        0     6377 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/__init__.py
--rw-r--r--   0        0        0     4779 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py
--rw-r--r--   0        0        0     4555 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py
--rw-r--r--   0        0        0     4824 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py
--rw-r--r--   0        0        0     4600 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py
--rw-r--r--   0        0        0     7060 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
--rw-r--r--   0        0        0     7063 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
--rw-r--r--   0        0        0     7255 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     7251 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     7252 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
--rw-r--r--   0        0        0     6907 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py
--rw-r--r--   0        0        0     6910 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py
--rw-r--r--   0        0        0     6976 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0     6972 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0     6973 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/__init__.py
--rw-r--r--   0        0        0     1905 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial001.py
--rw-r--r--   0        0        0     1908 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial001_an.py
--rw-r--r--   0        0        0     2156 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     8182 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003.py
--rw-r--r--   0        0        0     8185 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_an.py
--rw-r--r--   0        0        0     8594 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     8583 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     8591 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_py310.py
--rw-r--r--   0        0        0    15803 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005.py
--rw-r--r--   0        0        0    15806 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_an.py
--rw-r--r--   0        0        0    16711 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0    16687 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0    16699 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_py310.py
--rw-r--r--   0        0        0    16675 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2318 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial006.py
--rw-r--r--   0        0        0     2321 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial006_an.py
--rw-r--r--   0        0        0     2594 2024-05-03 00:21:35.625407 fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/__init__.py
--rw-r--r--   0        0        0     4958 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py
--rw-r--r--   0        0        0     5016 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5011 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py
--rw-r--r--   0        0        0     4958 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py
--rw-r--r--   0        0        0     5016 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py
--rw-r--r--   0        0        0     5011 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_settings/__init__.py
--rw-r--r--   0        0        0      488 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_settings/test_app02.py
--rw-r--r--   0        0        0      552 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_settings/test_tutorial001.py
--rw-r--r--   0        0        0      556 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_settings/test_tutorial001_pv1.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/__init__.py
--rw-r--r--   0        0        0    16475 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py
--rw-r--r--   0        0        0    16654 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
--rw-r--r--   0        0        0    16924 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
--rw-r--r--   0        0        0    16925 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
--rw-r--r--   0        0        0    16930 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
--rw-r--r--   0        0        0    16921 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
--rw-r--r--   0        0        0      788 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py
--rw-r--r--   0        0        0      825 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
--rw-r--r--   0        0        0      822 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sub_applications/__init__.py
--rw-r--r--   0        0        0     1920 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_templates/__init__.py
--rw-r--r--   0        0        0      910 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_templates/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      819 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main.py
--rw-r--r--   0        0        0      300 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main_b.py
--rw-r--r--   0        0        0      303 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main_b_an.py
--rw-r--r--   0        0        0      360 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main_b_an_py310.py
--rw-r--r--   0        0        0      357 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main_b_an_py39.py
--rw-r--r--   0        0        0      357 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main_b_py310.py
--rw-r--r--   0        0        0      821 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_tutorial001.py
--rw-r--r--   0        0        0      154 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_tutorial002.py
--rw-r--r--   0        0        0      167 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/__init__.py
--rw-r--r--   0        0        0     1527 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     1530 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     2088 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     2073 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     2067 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/__init__.py
--rw-r--r--   0        0        0      822 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial001.py
--rw-r--r--   0        0        0     3683 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002.py
--rw-r--r--   0        0        0     3686 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py
--rw-r--r--   0        0        0     3968 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3960 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3965 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
--rw-r--r--   0        0        0      872 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial003.py
--rw-r--r--   0        0        0     1288 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_wsgi/__init__.py
--rw-r--r--   0        0        0      436 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_tutorial/test_wsgi/test_tutorial001.py
--rw-r--r--   0        0        0      709 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_typing_python39.py
--rw-r--r--   0        0        0     4748 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_union_body.py
--rw-r--r--   0        0        0     5311 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_union_inherited_body.py
--rw-r--r--   0        0        0     2031 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response.py
--rw-r--r--   0        0        0     1208 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response_dataclass.py
--rw-r--r--   0        0        0        0 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response_recursive/__init__.py
--rw-r--r--   0        0        0     1149 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response_recursive/app_pv1.py
--rw-r--r--   0        0        0     1178 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response_recursive/app_pv2.py
--rw-r--r--   0        0        0      900 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py
--rw-r--r--   0        0        0      900 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py
--rw-r--r--   0        0        0     4667 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_webhooks_security.py
--rw-r--r--   0        0        0     2199 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_ws_dependencies.py
--rw-r--r--   0        0        0     7651 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/test_ws_router.py
--rw-r--r--   0        0        0      422 2024-05-03 00:21:35.629407 fastapi_slim-0.111.0/tests/utils.py
--rw-r--r--   0        0        0    26202 1970-01-01 00:00:00.000000 fastapi_slim-0.111.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-30 06:11:45.386818 fastapi_slim-0.111.0.dev1/LICENSE
+-rw-r--r--   0        0        0    22382 2024-04-30 06:11:45.386818 fastapi_slim-0.111.0.dev1/README.md
+-rw-r--r--   0        0        0     5043 2024-04-30 06:11:45.422818 fastapi_slim-0.111.0.dev1/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0      506 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial001.py
+-rw-r--r--   0        0        0      628 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial002.py
+-rw-r--r--   0        0        0      837 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial003.py
+-rw-r--r--   0        0        0      701 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial004.py
+-rw-r--r--   0        0        0      684 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001.py
+-rw-r--r--   0        0        0      734 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an.py
+-rw-r--r--   0        0        0      686 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      705 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      646 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_py310.py
+-rw-r--r--   0        0        0      231 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/advanced_middleware/tutorial001.py
+-rw-r--r--   0        0        0      279 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/advanced_middleware/tutorial002.py
+-rw-r--r--   0        0        0      213 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/advanced_middleware/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b/__init__.py
+-rw-r--r--   0        0        0     1145 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b/main.py
+-rw-r--r--   0        0        0     1866 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an/__init__.py
+-rw-r--r--   0        0        0     1205 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an/main.py
+-rw-r--r--   0        0        0     1866 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/__init__.py
+-rw-r--r--   0        0        0     1163 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/main.py
+-rw-r--r--   0        0        0     1866 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/main.py
+-rw-r--r--   0        0        0     1866 2024-04-30 06:11:45.506818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_py310/__init__.py
+-rw-r--r--   0        0        0     1113 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_py310/main.py
+-rw-r--r--   0        0        0     1866 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_py310/test_main.py
+-rw-r--r--   0        0        0      118 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/main.py
+-rw-r--r--   0        0        0      238 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/test_main.py
+-rw-r--r--   0        0        0      334 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/tutorial001.py
+-rw-r--r--   0        0        0      757 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/tutorial002.py
+-rw-r--r--   0        0        0      528 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/app_testing/tutorial003.py
+-rw-r--r--   0        0        0     1415 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/async_sql_databases/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/async_tests/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/async_tests/main.py
+-rw-r--r--   0        0        0      306 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/async_tests/test_main.py
+-rw-r--r--   0        0        0      519 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial001.py
+-rw-r--r--   0        0        0      675 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002.py
+-rw-r--r--   0        0        0      725 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_an.py
+-rw-r--r--   0        0        0      683 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      696 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      643 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_py310.py
+-rw-r--r--   0        0        0      189 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/behind_a_proxy/tutorial001.py
+-rw-r--r--   0        0        0      208 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/behind_a_proxy/tutorial002.py
+-rw-r--r--   0        0        0      405 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/behind_a_proxy/tutorial003.py
+-rw-r--r--   0        0        0      437 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/behind_a_proxy/tutorial004.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/internal/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/internal/admin.py
+-rw-r--r--   0        0        0      552 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/routers/items.py
+-rw-r--r--   0        0        0      407 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/routers/users.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/internal/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/internal/admin.py
+-rw-r--r--   0        0        0      552 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/items.py
+-rw-r--r--   0        0        0      407 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/users.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/internal/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/internal/admin.py
+-rw-r--r--   0        0        0      552 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/items.py
+-rw-r--r--   0        0        0      407 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/users.py
+-rw-r--r--   0        0        0      309 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial001.py
+-rw-r--r--   0        0        0      271 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial001_py310.py
+-rw-r--r--   0        0        0      467 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial002.py
+-rw-r--r--   0        0        0      429 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial002_py310.py
+-rw-r--r--   0        0        0      362 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial003.py
+-rw-r--r--   0        0        0      324 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial003_py310.py
+-rw-r--r--   0        0        0      452 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial004.py
+-rw-r--r--   0        0        0      408 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body/tutorial004_py310.py
+-rw-r--r--   0        0        0      561 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001.py
+-rw-r--r--   0        0        0      611 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_an.py
+-rw-r--r--   0        0        0      563 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      582 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      523 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_py310.py
+-rw-r--r--   0        0        0      596 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001.py
+-rw-r--r--   0        0        0      639 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an.py
+-rw-r--r--   0        0        0      579 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      610 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      546 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      490 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial002.py
+-rw-r--r--   0        0        0      446 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      548 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003.py
+-rw-r--r--   0        0        0      604 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an.py
+-rw-r--r--   0        0        0      550 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      575 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      504 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      653 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004.py
+-rw-r--r--   0        0        0      703 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an.py
+-rw-r--r--   0        0        0      643 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      674 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      603 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      407 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial005.py
+-rw-r--r--   0        0        0      457 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_an.py
+-rw-r--r--   0        0        0      409 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      428 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      369 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial005_py310.py
+-rw-r--r--   0        0        0      402 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial001.py
+-rw-r--r--   0        0        0      364 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      413 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial002.py
+-rw-r--r--   0        0        0      369 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      407 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial002_py39.py
+-rw-r--r--   0        0        0      414 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial003.py
+-rw-r--r--   0        0        0      371 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      409 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial003_py39.py
+-rw-r--r--   0        0        0      504 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial004.py
+-rw-r--r--   0        0        0      455 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial004_py310.py
+-rw-r--r--   0        0        0      499 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      517 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial005.py
+-rw-r--r--   0        0        0      468 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial005_py310.py
+-rw-r--r--   0        0        0      512 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      530 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial006.py
+-rw-r--r--   0        0        0      475 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial006_py310.py
+-rw-r--r--   0        0        0      519 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial006_py39.py
+-rw-r--r--   0        0        0      581 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial007.py
+-rw-r--r--   0        0        0      520 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py310.py
+-rw-r--r--   0        0        0      570 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py39.py
+-rw-r--r--   0        0        0      273 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial008.py
+-rw-r--r--   0        0        0      248 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial008_py39.py
+-rw-r--r--   0        0        0      179 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial009.py
+-rw-r--r--   0        0        0      154 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial009_py39.py
+-rw-r--r--   0        0        0      906 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial001.py
+-rw-r--r--   0        0        0      856 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial001_py310.py
+-rw-r--r--   0        0        0      900 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial001_py39.py
+-rw-r--r--   0        0        0     1060 2024-04-30 06:11:45.510818 fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial002.py
+-rw-r--r--   0        0        0     1010 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial002_py310.py
+-rw-r--r--   0        0        0     1054 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial002_py39.py
+-rw-r--r--   0        0        0      281 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/conditional_openapi/tutorial001.py
+-rw-r--r--   0        0        0      205 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/configure_swagger_ui/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/configure_swagger_ui/tutorial002.py
+-rw-r--r--   0        0        0      201 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/configure_swagger_ui/tutorial003.py
+-rw-r--r--   0        0        0      202 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/cookie_params/tutorial001.py
+-rw-r--r--   0        0        0      247 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/cookie_params/tutorial001_an.py
+-rw-r--r--   0        0        0      205 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/cookie_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      218 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/cookie_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      170 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/cookie_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      459 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/cors/tutorial001.py
+-rw-r--r--   0        0        0     1154 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_docs_ui/tutorial001.py
+-rw-r--r--   0        0        0     1175 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_docs_ui/tutorial002.py
+-rw-r--r--   0        0        0      973 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_request_and_route/tutorial001.py
+-rw-r--r--   0        0        0      932 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_request_and_route/tutorial002.py
+-rw-r--r--   0        0        0     1042 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_request_and_route/tutorial003.py
+-rw-r--r--   0        0        0      197 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial001.py
+-rw-r--r--   0        0        0      215 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial001b.py
+-rw-r--r--   0        0        0      352 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial002.py
+-rw-r--r--   0        0        0      394 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial003.py
+-rw-r--r--   0        0        0      491 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial004.py
+-rw-r--r--   0        0        0      186 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial005.py
+-rw-r--r--   0        0        0      199 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial006.py
+-rw-r--r--   0        0        0      220 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial006b.py
+-rw-r--r--   0        0        0      237 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial006c.py
+-rw-r--r--   0        0        0      277 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial007.py
+-rw-r--r--   0        0        0      360 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial008.py
+-rw-r--r--   0        0        0      202 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial009.py
+-rw-r--r--   0        0        0      217 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial009b.py
+-rw-r--r--   0        0        0      451 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial009c.py
+-rw-r--r--   0        0        0      205 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/custom_response/tutorial010.py
+-rw-r--r--   0        0        0      312 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dataclasses/tutorial001.py
+-rw-r--r--   0        0        0      552 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dataclasses/tutorial002.py
+-rw-r--r--   0        0        0     1403 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dataclasses/tutorial003.py
+-rw-r--r--   0        0        0      223 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/debugging/tutorial001.py
+-rw-r--r--   0        0        0      442 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001.py
+-rw-r--r--   0        0        0      495 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_02_an.py
+-rw-r--r--   0        0        0      447 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      466 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      502 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_an.py
+-rw-r--r--   0        0        0      454 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      473 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      404 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial001_py310.py
+-rw-r--r--   0        0        0      656 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002.py
+-rw-r--r--   0        0        0      706 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_an.py
+-rw-r--r--   0        0        0      664 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      677 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      624 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_py310.py
+-rw-r--r--   0        0        0      635 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003.py
+-rw-r--r--   0        0        0      697 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_an.py
+-rw-r--r--   0        0        0      655 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      668 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      603 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_py310.py
+-rw-r--r--   0        0        0      639 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004.py
+-rw-r--r--   0        0        0      689 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_an.py
+-rw-r--r--   0        0        0      647 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      660 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      607 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_py310.py
+-rw-r--r--   0        0        0      486 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005.py
+-rw-r--r--   0        0        0      558 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005_an.py
+-rw-r--r--   0        0        0      510 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      529 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      443 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005_py310.py
+-rw-r--r--   0        0        0      583 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial006.py
+-rw-r--r--   0        0        0      643 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial006_an.py
+-rw-r--r--   0        0        0      633 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial006_an_py39.py
+-rw-r--r--   0        0        0       99 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial007.py
+-rw-r--r--   0        0        0      455 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008.py
+-rw-r--r--   0        0        0      531 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008_an.py
+-rw-r--r--   0        0        0      521 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      735 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008b.py
+-rw-r--r--   0        0        0      785 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008b_an.py
+-rw-r--r--   0        0        0      775 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008b_an_py39.py
+-rw-r--r--   0        0        0      660 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008c.py
+-rw-r--r--   0        0        0      710 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008c_an.py
+-rw-r--r--   0        0        0      700 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008c_an_py39.py
+-rw-r--r--   0        0        0      694 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008d.py
+-rw-r--r--   0        0        0      744 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008d_an.py
+-rw-r--r--   0        0        0      734 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008d_an_py39.py
+-rw-r--r--   0        0        0      455 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial009.py
+-rw-r--r--   0        0        0      292 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial010.py
+-rw-r--r--   0        0        0      504 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial011.py
+-rw-r--r--   0        0        0      554 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial011_an.py
+-rw-r--r--   0        0        0      544 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      696 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial012.py
+-rw-r--r--   0        0        0      756 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial012_an.py
+-rw-r--r--   0        0        0      756 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial012_an_py39.py
+-rw-r--r--   0        0        0     1522 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001.py
+-rw-r--r--   0        0        0     1582 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an.py
+-rw-r--r--   0        0        0     1528 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py310.py
+-rw-r--r--   0        0        0     1553 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py39.py
+-rw-r--r--   0        0        0     1478 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_py310.py
+-rw-r--r--   0        0        0      461 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/encoder/tutorial001.py
+-rw-r--r--   0        0        0      430 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/encoder/tutorial001_py310.py
+-rw-r--r--   0        0        0      283 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/events/tutorial001.py
+-rw-r--r--   0        0        0      255 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/events/tutorial002.py
+-rw-r--r--   0        0        0      569 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/events/tutorial003.py
+-rw-r--r--   0        0        0      737 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extending_openapi/tutorial001.py
+-rw-r--r--   0        0        0      755 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001.py
+-rw-r--r--   0        0        0      830 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an.py
+-rw-r--r--   0        0        0      788 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      801 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      724 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_py310.py
+-rw-r--r--   0        0        0      943 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial001.py
+-rw-r--r--   0        0        0      899 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      824 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial002.py
+-rw-r--r--   0        0        0      792 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      644 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial003.py
+-rw-r--r--   0        0        0      644 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      381 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial004.py
+-rw-r--r--   0        0        0      356 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      205 2024-04-30 06:11:45.514819 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial005.py
+-rw-r--r--   0        0        0      180 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      117 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      139 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      111 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      519 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial001.py
+-rw-r--r--   0        0        0      494 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial001_py39.py
+-rw-r--r--   0        0        0      755 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial002.py
+-rw-r--r--   0        0        0      730 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial002_py39.py
+-rw-r--r--   0        0        0      939 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial003.py
+-rw-r--r--   0        0        0      914 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial003_py39.py
+-rw-r--r--   0        0        0     1066 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial004.js
+-rw-r--r--   0        0        0      493 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial004.py
+-rw-r--r--   0        0        0      446 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/graphql/tutorial001.py
+-rw-r--r--   0        0        0      299 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial001.py
+-rw-r--r--   0        0        0      404 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial002.py
+-rw-r--r--   0        0        0      626 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial003.py
+-rw-r--r--   0        0        0      762 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial004.py
+-rw-r--r--   0        0        0      667 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial005.py
+-rw-r--r--   0        0        0      928 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial006.py
+-rw-r--r--   0        0        0      214 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial001.py
+-rw-r--r--   0        0        0      259 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial001_an.py
+-rw-r--r--   0        0        0      217 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      230 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      182 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      260 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial002.py
+-rw-r--r--   0        0        0      317 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial002_an.py
+-rw-r--r--   0        0        0      261 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      288 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      228 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      224 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial003.py
+-rw-r--r--   0        0        0      269 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial003_an.py
+-rw-r--r--   0        0        0      221 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      240 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      186 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      218 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/header_params/tutorial003_py39.py
+-rw-r--r--   0        0        0      805 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial001.py
+-rw-r--r--   0        0        0      767 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial001_1.py
+-rw-r--r--   0        0        0      154 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial002.py
+-rw-r--r--   0        0        0      161 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial003.py
+-rw-r--r--   0        0        0      693 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial004.py
+-rw-r--r--   0        0        0      349 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/middleware/tutorial001.py
+-rw-r--r--   0        0        0     1357 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/nosql_databases/tutorial001.py
+-rw-r--r--   0        0        0     1371 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/openapi_callbacks/tutorial001.py
+-rw-r--r--   0        0        0      550 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/openapi_webhooks/tutorial001.py
+-rw-r--r--   0        0        0      167 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial001.py
+-rw-r--r--   0        0        0      572 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial002.py
+-rw-r--r--   0        0        0      148 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial003.py
+-rw-r--r--   0        0        0      717 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial004.py
+-rw-r--r--   0        0        0      180 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial005.py
+-rw-r--r--   0        0        0     1043 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial006.py
+-rw-r--r--   0        0        0      822 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007.py
+-rw-r--r--   0        0        0      789 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py
+-rw-r--r--   0        0        0      406 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial001.py
+-rw-r--r--   0        0        0      363 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial001_py310.py
+-rw-r--r--   0        0        0      401 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial001_py39.py
+-rw-r--r--   0        0        0      580 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002.py
+-rw-r--r--   0        0        0      537 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py310.py
+-rw-r--r--   0        0        0      575 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py39.py
+-rw-r--r--   0        0        0      323 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002b.py
+-rw-r--r--   0        0        0      517 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003.py
+-rw-r--r--   0        0        0      474 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003_py310.py
+-rw-r--r--   0        0        0      512 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003_py39.py
+-rw-r--r--   0        0        0      681 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004.py
+-rw-r--r--   0        0        0      638 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py310.py
+-rw-r--r--   0        0        0      676 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py39.py
+-rw-r--r--   0        0        0      741 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005.py
+-rw-r--r--   0        0        0      698 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py310.py
+-rw-r--r--   0        0        0      736 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py39.py
+-rw-r--r--   0        0        0      365 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial006.py
+-rw-r--r--   0        0        0      138 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial001.py
+-rw-r--r--   0        0        0      143 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial002.py
+-rw-r--r--   0        0        0      236 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial003.py
+-rw-r--r--   0        0        0      193 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial003b.py
+-rw-r--r--   0        0        0      156 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial004.py
+-rw-r--r--   0        0        0      546 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial005.py
+-rw-r--r--   0        0        0      364 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001.py
+-rw-r--r--   0        0        0      417 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_an.py
+-rw-r--r--   0        0        0      375 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      388 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      332 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      265 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial002.py
+-rw-r--r--   0        0        0      321 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      311 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      268 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial003.py
+-rw-r--r--   0        0        0      321 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      311 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      280 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial004.py
+-rw-r--r--   0        0        0      327 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      317 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      298 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial005.py
+-rw-r--r--   0        0        0      341 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      331 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      345 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial006.py
+-rw-r--r--   0        0        0      405 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      395 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      162 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial001.py
+-rw-r--r--   0        0        0      172 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial002.py
+-rw-r--r--   0        0        0      119 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial003.py
+-rw-r--r--   0        0        0      124 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial004.py
+-rw-r--r--   0        0        0      143 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial005.py
+-rw-r--r--   0        0        0      106 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial006.py
+-rw-r--r--   0        0        0       80 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial006_py39.py
+-rw-r--r--   0        0        0      131 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial007.py
+-rw-r--r--   0        0        0       99 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial007_py39.py
+-rw-r--r--   0        0        0      171 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial008.py
+-rw-r--r--   0        0        0      145 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial008_py39.py
+-rw-r--r--   0        0        0       84 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial008b.py
+-rw-r--r--   0        0        0       51 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial008b_py310.py
+-rw-r--r--   0        0        0      164 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial009.py
+-rw-r--r--   0        0        0      131 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial009_py310.py
+-rw-r--r--   0        0        0      164 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial009b.py
+-rw-r--r--   0        0        0       89 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial009c.py
+-rw-r--r--   0        0        0       56 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial009c_py310.py
+-rw-r--r--   0        0        0      144 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial010.py
+-rw-r--r--   0        0        0      498 2024-04-30 06:11:45.518818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial011.py
+-rw-r--r--   0        0        0      461 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial011_py310.py
+-rw-r--r--   0        0        0      492 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial011_py39.py
+-rw-r--r--   0        0        0      122 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial012.py
+-rw-r--r--   0        0        0      138 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial013.py
+-rw-r--r--   0        0        0      127 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/python_types/tutorial013_py39.py
+-rw-r--r--   0        0        0      250 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial001.py
+-rw-r--r--   0        0        0      251 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial002.py
+-rw-r--r--   0        0        0      219 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      406 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial003.py
+-rw-r--r--   0        0        0      374 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      468 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial004.py
+-rw-r--r--   0        0        0      436 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      192 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial005.py
+-rw-r--r--   0        0        0      301 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial006.py
+-rw-r--r--   0        0        0      269 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial006_py310.py
+-rw-r--r--   0        0        0      301 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params/tutorial006b.py
+-rw-r--r--   0        0        0      271 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial001.py
+-rw-r--r--   0        0        0      239 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      308 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002.py
+-rw-r--r--   0        0        0      351 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      309 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      276 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial002_py310.py
+-rw-r--r--   0        0        0      329 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003.py
+-rw-r--r--   0        0        0      372 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      330 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      343 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      290 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial003_py310.py
+-rw-r--r--   0        0        0      367 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004.py
+-rw-r--r--   0        0        0      410 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      368 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      366 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an_py310_regex.py
+-rw-r--r--   0        0        0      381 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      335 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial004_py310.py
+-rw-r--r--   0        0        0      276 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial005.py
+-rw-r--r--   0        0        0      319 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      309 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      254 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006.py
+-rw-r--r--   0        0        0      304 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      294 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      267 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006b.py
+-rw-r--r--   0        0        0      310 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006b_an.py
+-rw-r--r--   0        0        0      300 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006b_an_py39.py
+-rw-r--r--   0        0        0      306 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c.py
+-rw-r--r--   0        0        0      349 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_an.py
+-rw-r--r--   0        0        0      307 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_an_py310.py
+-rw-r--r--   0        0        0      320 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_an_py39.py
+-rw-r--r--   0        0        0      274 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006c_py310.py
+-rw-r--r--   0        0        0      302 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006d.py
+-rw-r--r--   0        0        0      345 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006d_an.py
+-rw-r--r--   0        0        0      335 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial006d_an_py39.py
+-rw-r--r--   0        0        0      336 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007.py
+-rw-r--r--   0        0        0      379 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_an.py
+-rw-r--r--   0        0        0      337 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_an_py310.py
+-rw-r--r--   0        0        0      350 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      304 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial007_py310.py
+-rw-r--r--   0        0        0      466 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008.py
+-rw-r--r--   0        0        0      540 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an.py
+-rw-r--r--   0        0        0      498 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an_py310.py
+-rw-r--r--   0        0        0      511 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      434 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_py310.py
+-rw-r--r--   0        0        0      313 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009.py
+-rw-r--r--   0        0        0      356 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_an.py
+-rw-r--r--   0        0        0      314 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_an_py310.py
+-rw-r--r--   0        0        0      327 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_an_py39.py
+-rw-r--r--   0        0        0      281 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial009_py310.py
+-rw-r--r--   0        0        0      574 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010.py
+-rw-r--r--   0        0        0      664 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an.py
+-rw-r--r--   0        0        0      622 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py310.py
+-rw-r--r--   0        0        0      635 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py39.py
+-rw-r--r--   0        0        0      542 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_py310.py
+-rw-r--r--   0        0        0      227 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011.py
+-rw-r--r--   0        0        0      272 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_an.py
+-rw-r--r--   0        0        0      224 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_an_py310.py
+-rw-r--r--   0        0        0      237 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      189 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_py310.py
+-rw-r--r--   0        0        0      221 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial011_py39.py
+-rw-r--r--   0        0        0      217 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012.py
+-rw-r--r--   0        0        0      262 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012_an.py
+-rw-r--r--   0        0        0      227 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012_an_py39.py
+-rw-r--r--   0        0        0      192 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial012_py39.py
+-rw-r--r--   0        0        0      175 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial013.py
+-rw-r--r--   0        0        0      220 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial013_an.py
+-rw-r--r--   0        0        0      210 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial013_an_py39.py
+-rw-r--r--   0        0        0      330 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014.py
+-rw-r--r--   0        0        0      373 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_an.py
+-rw-r--r--   0        0        0      331 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_an_py310.py
+-rw-r--r--   0        0        0      344 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_an_py39.py
+-rw-r--r--   0        0        0      298 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial014_py310.py
+-rw-r--r--   0        0        0      282 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001.py
+-rw-r--r--   0        0        0      508 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02.py
+-rw-r--r--   0        0        0      553 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02_an.py
+-rw-r--r--   0        0        0      505 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      524 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      470 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02_py310.py
+-rw-r--r--   0        0        0      371 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_03.py
+-rw-r--r--   0        0        0      431 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_03_an.py
+-rw-r--r--   0        0        0      421 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0      332 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_an.py
+-rw-r--r--   0        0        0      322 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      811 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002.py
+-rw-r--r--   0        0        0      861 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002_an.py
+-rw-r--r--   0        0        0      826 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      786 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002_py39.py
+-rw-r--r--   0        0        0      913 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003.py
+-rw-r--r--   0        0        0      987 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003_an.py
+-rw-r--r--   0        0        0      952 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      888 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003_py39.py
+-rw-r--r--   0        0        0      173 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_forms/tutorial001.py
+-rw-r--r--   0        0        0      233 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_forms/tutorial001_an.py
+-rw-r--r--   0        0        0      223 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_forms/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      317 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_forms_and_files/tutorial001.py
+-rw-r--r--   0        0        0      396 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_forms_and_files/tutorial001_an.py
+-rw-r--r--   0        0        0      386 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/request_forms_and_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      391 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_change_status_code/tutorial001.py
+-rw-r--r--   0        0        0      344 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_cookies/tutorial001.py
+-rw-r--r--   0        0        0      272 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_cookies/tutorial002.py
+-rw-r--r--   0        0        0      505 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_directly/tutorial001.py
+-rw-r--r--   0        0        0      354 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_directly/tutorial002.py
+-rw-r--r--   0        0        0      309 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_headers/tutorial001.py
+-rw-r--r--   0        0        0      222 2024-04-30 06:11:45.522818 fastapi_slim-0.111.0.dev1/docs_src/response_headers/tutorial002.py
+-rw-r--r--   0        0        0      562 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001.py
+-rw-r--r--   0        0        0      513 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_01.py
+-rw-r--r--   0        0        0      469 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_01_py310.py
+-rw-r--r--   0        0        0      507 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_01_py39.py
+-rw-r--r--   0        0        0      537 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0      556 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0      350 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial002.py
+-rw-r--r--   0        0        0      318 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial002_py310.py
+-rw-r--r--   0        0        0      450 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003.py
+-rw-r--r--   0        0        0      349 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_01.py
+-rw-r--r--   0        0        0      317 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_01_py310.py
+-rw-r--r--   0        0        0      381 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_02.py
+-rw-r--r--   0        0        0      241 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_03.py
+-rw-r--r--   0        0        0      384 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_04.py
+-rw-r--r--   0        0        0      352 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_04_py310.py
+-rw-r--r--   0        0        0      405 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_05.py
+-rw-r--r--   0        0        0      373 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_05_py310.py
+-rw-r--r--   0        0        0      431 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial003_py310.py
+-rw-r--r--   0        0        0      633 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial004.py
+-rw-r--r--   0        0        0      595 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial004_py310.py
+-rw-r--r--   0        0        0      627 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial004_py39.py
+-rw-r--r--   0        0        0      848 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial005.py
+-rw-r--r--   0        0        0      816 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial005_py310.py
+-rw-r--r--   0        0        0      848 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial006.py
+-rw-r--r--   0        0        0      816 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial006_py310.py
+-rw-r--r--   0        0        0      145 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_status_code/tutorial001.py
+-rw-r--r--   0        0        0      173 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/response_status_code/tutorial002.py
+-rw-r--r--   0        0        0      684 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001.py
+-rw-r--r--   0        0        0      669 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_pv1.py
+-rw-r--r--   0        0        0      646 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310.py
+-rw-r--r--   0        0        0      631 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310_pv1.py
+-rw-r--r--   0        0        0      517 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial002.py
+-rw-r--r--   0        0        0      479 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial002_py310.py
+-rw-r--r--   0        0        0      612 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003.py
+-rw-r--r--   0        0        0      721 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an.py
+-rw-r--r--   0        0        0      673 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      692 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      574 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_py310.py
+-rw-r--r--   0        0        0      824 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004.py
+-rw-r--r--   0        0        0      965 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an.py
+-rw-r--r--   0        0        0      917 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      936 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      786 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_py310.py
+-rw-r--r--   0        0        0     1386 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005.py
+-rw-r--r--   0        0        0     1571 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an.py
+-rw-r--r--   0        0        0     1523 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     1542 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     1348 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_py310.py
+-rw-r--r--   0        0        0      269 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial001.py
+-rw-r--r--   0        0        0      319 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial001_an.py
+-rw-r--r--   0        0        0      309 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      755 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002.py
+-rw-r--r--   0        0        0      815 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_an.py
+-rw-r--r--   0        0        0      761 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      786 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      711 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_py310.py
+-rw-r--r--   0        0        0     2494 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003.py
+-rw-r--r--   0        0        0     2588 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_an.py
+-rw-r--r--   0        0        0     2534 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_an_py310.py
+-rw-r--r--   0        0        0     2559 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_an_py39.py
+-rw-r--r--   0        0        0     2450 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_py310.py
+-rw-r--r--   0        0        0     4134 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004.py
+-rw-r--r--   0        0        0     4245 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_an.py
+-rw-r--r--   0        0        0     4179 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     4216 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     4079 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_py310.py
+-rw-r--r--   0        0        0     5270 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005.py
+-rw-r--r--   0        0        0     5377 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_an.py
+-rw-r--r--   0        0        0     5305 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     5348 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     5209 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_py310.py
+-rw-r--r--   0        0        0     5264 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_py39.py
+-rw-r--r--   0        0        0      321 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial006.py
+-rw-r--r--   0        0        0      371 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial006_an.py
+-rw-r--r--   0        0        0      361 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial006_an_py39.py
+-rw-r--r--   0        0        0     1116 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial007.py
+-rw-r--r--   0        0        0     1183 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial007_an.py
+-rw-r--r--   0        0        0     1172 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/security/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      489 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial001.py
+-rw-r--r--   0        0        0      451 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial001_py310.py
+-rw-r--r--   0        0        0      483 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial001_py39.py
+-rw-r--r--   0        0        0      524 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002.py
+-rw-r--r--   0        0        0      486 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002_py310.py
+-rw-r--r--   0        0        0      518 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app01/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app01/config.py
+-rw-r--r--   0        0        0      267 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app01/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02/config.py
+-rw-r--r--   0        0        0      406 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02/main.py
+-rw-r--r--   0        0        0      515 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an/config.py
+-rw-r--r--   0        0        0      456 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an/main.py
+-rw-r--r--   0        0        0      515 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an_py39/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an_py39/config.py
+-rw-r--r--   0        0        0      445 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an_py39/main.py
+-rw-r--r--   0        0        0      515 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03/config.py
+-rw-r--r--   0        0        0      412 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an/config.py
+-rw-r--r--   0        0        0      195 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an/config_pv1.py
+-rw-r--r--   0        0        0      451 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an_py39/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an_py39/config.py
+-rw-r--r--   0        0        0      462 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/app03_an_py39/main.py
+-rw-r--r--   0        0        0      419 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/tutorial001.py
+-rw-r--r--   0        0        0      410 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/settings/tutorial001_pv1.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.526818 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/crud.py
+-rw-r--r--   0        0        0      461 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/database.py
+-rw-r--r--   0        0        0     1632 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/main.py
+-rw-r--r--   0        0        0      710 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/models.py
+-rw-r--r--   0        0        0      502 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/tests/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/__init__.py
+-rw-r--r--   0        0        0     1903 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/crud.py
+-rw-r--r--   0        0        0      461 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/database.py
+-rw-r--r--   0        0        0     1607 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/main.py
+-rw-r--r--   0        0        0      710 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/models.py
+-rw-r--r--   0        0        0      464 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/__init__.py
+-rw-r--r--   0        0        0     1903 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/alt_main.py
+-rw-r--r--   0        0        0     1061 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/crud.py
+-rw-r--r--   0        0        0      461 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/database.py
+-rw-r--r--   0        0        0     1607 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/main.py
+-rw-r--r--   0        0        0      710 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/models.py
+-rw-r--r--   0        0        0      496 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/crud.py
+-rw-r--r--   0        0        0      662 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/database.py
+-rw-r--r--   0        0        0     2210 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/main.py
+-rw-r--r--   0        0        0      465 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/models.py
+-rw-r--r--   0        0        0      868 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/schemas.py
+-rw-r--r--   0        0        0      159 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/static_files/tutorial001.py
+-rw-r--r--   0        0        0      274 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/sub_applications/tutorial001.py
+-rw-r--r--   0        0        0       25 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/templates/static/styles.css
+-rw-r--r--   0        0        0      235 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/templates/templates/item.html
+-rw-r--r--   0        0        0      521 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/templates/tutorial001.py
+-rw-r--r--   0        0        0      230 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/using_request_directly/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/__init__.py
+-rw-r--r--   0        0        0     1432 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial001.py
+-rw-r--r--   0        0        0     2842 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002.py
+-rw-r--r--   0        0        0     2909 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_an.py
+-rw-r--r--   0        0        0     2855 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_an_py310.py
+-rw-r--r--   0        0        0     2880 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_an_py39.py
+-rw-r--r--   0        0        0     2798 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_py310.py
+-rw-r--r--   0        0        0     2574 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial003.py
+-rw-r--r--   0        0        0     2549 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial003_py39.py
+-rw-r--r--   0        0        0      443 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/docs_src/wsgi/tutorial001.py
+-rw-r--r--   0        0        0     1086 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/__init__.py
+-rw-r--r--   0        0        0    23134 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/_compat.py
+-rw-r--r--   0        0        0   176342 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/applications.py
+-rw-r--r--   0        0        0     1768 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/background.py
+-rw-r--r--   0        0        0     1403 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/concurrency.py
+-rw-r--r--   0        0        0     5766 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/datastructures.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2494 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/dependencies/models.py
+-rw-r--r--   0        0        0    30241 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/dependencies/utils.py
+-rw-r--r--   0        0        0    11068 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/encoders.py
+-rw-r--r--   0        0        0     1332 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/exception_handlers.py
+-rw-r--r--   0        0        0     4969 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/exceptions.py
+-rw-r--r--   0        0        0       54 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/logger.py
+-rw-r--r--   0        0        0       58 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/openapi/constants.py
+-rw-r--r--   0        0        0    10356 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/openapi/docs.py
+-rw-r--r--   0        0        0    15397 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/openapi/models.py
+-rw-r--r--   0        0        0    22286 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/openapi/utils.py
+-rw-r--r--   0        0        0    64005 2024-04-30 06:11:45.530819 fastapi_slim-0.111.0.dev1/fastapi/param_functions.py
+-rw-r--r--   0        0        0    28191 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/params.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/py.typed
+-rw-r--r--   0        0        0      142 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/requests.py
+-rw-r--r--   0        0        0     1761 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/responses.py
+-rw-r--r--   0        0        0   174150 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/routing.py
+-rw-r--r--   0        0        0      881 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/__init__.py
+-rw-r--r--   0        0        0     9368 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/api_key.py
+-rw-r--r--   0        0        0      141 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/base.py
+-rw-r--r--   0        0        0    13506 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/http.py
+-rw-r--r--   0        0        0    21583 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/oauth2.py
+-rw-r--r--   0        0        0     2722 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/security/utils.py
+-rw-r--r--   0        0        0       69 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/templating.py
+-rw-r--r--   0        0        0       66 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/testclient.py
+-rw-r--r--   0        0        0      383 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/types.py
+-rw-r--r--   0        0        0     8035 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/utils.py
+-rw-r--r--   0        0        0      222 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/fastapi/websockets.py
+-rw-r--r--   0        0        0     1722 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/pdm_build.py
+-rw-r--r--   0        0        0     7306 2024-04-30 06:11:53.758842 fastapi_slim-0.111.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0       52 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/requirements-docs-tests.txt
+-rw-r--r--   0        0        0      465 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/requirements-docs.txt
+-rw-r--r--   0        0        0      496 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/requirements-tests.txt
+-rw-r--r--   0        0        0      128 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/requirements.txt
+-rw-r--r--   0        0        0    11141 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/docs.py
+-rwxr-xr-x   0        0        0      112 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/format.sh
+-rwxr-xr-x   0        0        0      125 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/lint.sh
+-rw-r--r--   0        0        0     5216 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/mkdocs_hooks.py
+-rw-r--r--   0        0        0      819 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image01.py
+-rw-r--r--   0        0        0      873 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image02.py
+-rw-r--r--   0        0        0      892 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image03.py
+-rw-r--r--   0        0        0      881 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image04.py
+-rw-r--r--   0        0        0      829 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image05.py
+-rwxr-xr-x   0        0        0      124 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       99 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0     4452 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/main.py
+-rw-r--r--   0        0        0     3688 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     4301 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_properties_bool.py
+-rw-r--r--   0        0        0     1207 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1117 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     5895 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2974 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2882 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3560 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     5229 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     2148 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0    10493 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_annotated.py
+-rw-r--r--   0        0        0    53491 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_application.py
+-rw-r--r--   0        0        0      457 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_callable_endpoint.py
+-rw-r--r--   0        0        0     2826 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_compat.py
+-rw-r--r--   0        0        0     2264 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_computed_fields.py
+-rw-r--r--   0        0        0     2892 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_custom_middleware_exception.py
+-rw-r--r--   0        0        0     3131 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_custom_route_class.py
+-rw-r--r--   0        0        0     1246 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_custom_schema_fields.py
+-rw-r--r--   0        0        0     1091 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_custom_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     2026 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_datastructures.py
+-rw-r--r--   0        0        0     1604 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_datetime_custom_encoder.py
+-rw-r--r--   0        0        0     5365 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_default_response_class.py
+-rw-r--r--   0        0        0     5117 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_default_response_class_router.py
+-rw-r--r--   0        0        0     2787 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_cache.py
+-rw-r--r--   0        0        0     3379 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_class.py
+-rw-r--r--   0        0        0    11869 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_contextmanager.py
+-rw-r--r--   0        0        0     1560 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_contextvars.py
+-rw-r--r--   0        0        0     8577 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_duplicates.py
+-rw-r--r--   0        0        0     1961 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_normal_exceptions.py
+-rw-r--r--   0        0        0    15816 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_overrides.py
+-rw-r--r--   0        0        0     1463 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_dependency_security_overrides.py
+-rw-r--r--   0        0        0     1193 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_deprecated_openapi_prefix.py
+-rw-r--r--   0        0        0     2159 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_duplicate_models_openapi.py
+-rw-r--r--   0        0        0      805 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_empty_router.py
+-rw-r--r--   0        0        0     3458 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_enforce_once_required_parameter.py
+-rw-r--r--   0        0        0     1918 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_exception_handlers.py
+-rw-r--r--   0        0        0    14029 2024-04-30 06:11:45.534819 fastapi_slim-0.111.0.dev1/tests/test_extra_routes.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model/app_pv1.py
+-rw-r--r--   0        0        0     4612 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py
+-rw-r--r--   0        0        0     6461 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model_pv2.py
+-rw-r--r--   0        0        0     1202 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0    68299 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_generate_unique_id_function.py
+-rw-r--r--   0        0        0     1881 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_generic_parameterless_depends.py
+-rw-r--r--   0        0        0     3744 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_get_request_body.py
+-rw-r--r--   0        0        0      972 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_http_connection_injection.py
+-rw-r--r--   0        0        0      496 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_include_route.py
+-rw-r--r--   0        0        0   367192 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_include_router_defaults_overrides.py
+-rw-r--r--   0        0        0    13619 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_infer_param_optionality.py
+-rw-r--r--   0        0        0     3085 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_inherited_custom_class.py
+-rw-r--r--   0        0        0     1704 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1248 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     9182 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_jsonable_encoder.py
+-rw-r--r--   0        0        0     2506 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_local_docs.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/app/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/app/a.py
+-rw-r--r--   0        0        0      161 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/app/b.py
+-rw-r--r--   0        0        0      150 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/app/main.py
+-rw-r--r--   0        0        0     5782 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/test_main.py
+-rw-r--r--   0        0        0     7821 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_multi_body_errors.py
+-rw-r--r--   0        0        0     4610 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_multi_query_errors.py
+-rw-r--r--   0        0        0     3777 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_multipart_installation.py
+-rw-r--r--   0        0        0      786 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_no_swagger_ui_redirect.py
+-rw-r--r--   0        0        0    17438 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_openapi_examples.py
+-rw-r--r--   0        0        0     4847 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_openapi_query_parameter_extension.py
+-rw-r--r--   0        0        0     1133 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_openapi_route_extensions.py
+-rw-r--r--   0        0        0    18887 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_openapi_separate_input_output_schemas.py
+-rw-r--r--   0        0        0     2001 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_openapi_servers.py
+-rw-r--r--   0        0        0      934 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_operations_signatures.py
+-rw-r--r--   0        0        0      562 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_orjson_response_class.py
+-rw-r--r--   0        0        0      636 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_param_class.py
+-rw-r--r--   0        0        0     3137 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_param_in_path_and_dependency.py
+-rw-r--r--   0        0        0     7611 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_param_include_in_schema.py
+-rw-r--r--   0        0        0     3414 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_params_repr.py
+-rw-r--r--   0        0        0    35209 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_path.py
+-rw-r--r--   0        0        0     3362 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_put_no_body.py
+-rw-r--r--   0        0        0    11638 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_query.py
+-rw-r--r--   0        0        0     2415 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_read_with_orm_mode.py
+-rw-r--r--   0        0        0     6344 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_regex_deprecated_body.py
+-rw-r--r--   0        0        0     5595 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_regex_deprecated_params.py
+-rw-r--r--   0        0        0      792 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_repeated_cookie_headers.py
+-rw-r--r--   0        0        0     3248 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_repeated_dependency_schema.py
+-rw-r--r--   0        0        0     3745 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_repeated_parameter_alias.py
+-rw-r--r--   0        0        0     3208 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_reponse_set_reponse_code_empty.py
+-rw-r--r--   0        0        0     6509 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_request_body_parameters_media_type.py
+-rw-r--r--   0        0        0     1530 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_required_noneable.py
+-rw-r--r--   0        0        0    11379 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_by_alias.py
+-rw-r--r--   0        0        0      589 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_change_status_code.py
+-rw-r--r--   0        0        0     3415 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_class_no_mediatype.py
+-rw-r--r--   0        0        0     3315 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_code_no_body.py
+-rw-r--r--   0        0        0    48837 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_model_as_return_annotation.py
+-rw-r--r--   0        0        0     1726 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_model_data_filter.py
+-rw-r--r--   0        0        0     1746 2024-04-30 06:11:45.538818 fastapi_slim-0.111.0.dev1/tests/test_response_model_data_filter_no_inheritance.py
+-rw-r--r--   0        0        0     4118 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_response_model_include_exclude.py
+-rw-r--r--   0        0        0     1124 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_response_model_invalid.py
+-rw-r--r--   0        0        0     5379 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_response_model_sub_types.py
+-rw-r--r--   0        0        0     1510 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_route_scope.py
+-rw-r--r--   0        0        0     3295 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_router_events.py
+-rw-r--r--   0        0        0      484 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_router_prefix_with_template.py
+-rw-r--r--   0        0        0      974 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_router_redirect_slashes.py
+-rw-r--r--   0        0        0    38576 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_schema_extra_examples.py
+-rw-r--r--   0        0        0     1944 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_cookie.py
+-rw-r--r--   0        0        0     2112 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2146 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1884 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_header.py
+-rw-r--r--   0        0        0     2052 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_header_description.py
+-rw-r--r--   0        0        0     2082 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_header_optional.py
+-rw-r--r--   0        0        0     1863 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_query.py
+-rw-r--r--   0        0        0     2023 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_query_description.py
+-rw-r--r--   0        0        0     2061 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_api_key_query_optional.py
+-rw-r--r--   0        0        0     1787 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_base.py
+-rw-r--r--   0        0        0     1973 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_base_description.py
+-rw-r--r--   0        0        0     1932 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_base_optional.py
+-rw-r--r--   0        0        0     2671 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_basic_optional.py
+-rw-r--r--   0        0        0     2654 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_basic_realm.py
+-rw-r--r--   0        0        0     2830 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2065 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_bearer.py
+-rw-r--r--   0        0        0     2255 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_bearer_description.py
+-rw-r--r--   0        0        0     2194 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_bearer_optional.py
+-rw-r--r--   0        0        0     2090 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_digest.py
+-rw-r--r--   0        0        0     2266 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_digest_description.py
+-rw-r--r--   0        0        0     2233 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_http_digest_optional.py
+-rw-r--r--   0        0        0    11002 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2.py
+-rw-r--r--   0        0        0     2338 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2442 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0    11043 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_optional.py
+-rw-r--r--   0        0        0    11183 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2147 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2289 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0     2290 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_openid_connect.py
+-rw-r--r--   0        0        0     2409 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_openid_connect_description.py
+-rw-r--r--   0        0        0     2488 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_security_openid_connect_optional.py
+-rw-r--r--   0        0        0     1414 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_serialize_response.py
+-rw-r--r--   0        0        0     4998 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_serialize_response_dataclass.py
+-rw-r--r--   0        0        0     4276 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_serialize_response_model.py
+-rw-r--r--   0        0        0     2071 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_skip_defaults.py
+-rw-r--r--   0        0        0     7550 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_starlette_exception.py
+-rw-r--r--   0        0        0     1710 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_starlette_urlconvertors.py
+-rw-r--r--   0        0        0    14142 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_sub_callbacks.py
+-rw-r--r--   0        0        0      718 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_swagger_ui_init_oauth.py
+-rw-r--r--   0        0        0    12068 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tuples.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/__init__.py
+-rw-r--r--   0        0        0     4432 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial001.py
+-rw-r--r--   0        0        0     4740 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial002.py
+-rw-r--r--   0        0        0     4656 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial003.py
+-rw-r--r--   0        0        0     4935 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/__init__.py
+-rw-r--r--   0        0        0      546 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
+-rw-r--r--   0        0        0      549 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
+-rw-r--r--   0        0        0      741 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0      737 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0      738 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/__init__.py
+-rw-r--r--   0        0        0      474 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
+-rw-r--r--   0        0        0      570 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
+-rw-r--r--   0        0        0      665 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_async_sql_databases/__init__.py
+-rw-r--r--   0        0        0     6122 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_async_tests/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_async_tests/test_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/__init__.py
+-rw-r--r--   0        0        0      578 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial001.py
+-rw-r--r--   0        0        0      568 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002.py
+-rw-r--r--   0        0        0      571 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
+-rw-r--r--   0        0        0      631 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0      628 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0      628 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
+-rw-r--r--   0        0        0     1032 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
+-rw-r--r--   0        0        0     1688 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
+-rw-r--r--   0        0        0     1656 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/__init__.py
+-rw-r--r--   0        0        0    25140 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main.py
+-rw-r--r--   0        0        0    25143 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an.py
+-rw-r--r--   0        0        0    25481 2024-04-30 06:11:45.542818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body/__init__.py
+-rw-r--r--   0        0        0    15092 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001.py
+-rw-r--r--   0        0        0    15340 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/__init__.py
+-rw-r--r--   0        0        0     7341 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001.py
+-rw-r--r--   0        0        0     7344 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7436 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7430 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7433 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/__init__.py
+-rw-r--r--   0        0        0     7698 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
+-rw-r--r--   0        0        0     7701 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7806 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7799 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7803 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     9660 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
+-rw-r--r--   0        0        0     9663 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     9755 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     9749 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     9752 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/__init__.py
+-rw-r--r--   0        0        0     4343 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
+-rw-r--r--   0        0        0     4417 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001.py
+-rw-r--r--   0        0        0    12111 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0    12105 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_conditional_openapi/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/__init__.py
+-rw-r--r--   0        0        0     1415 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py
+-rw-r--r--   0        0        0     1562 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py
+-rw-r--r--   0        0        0     1534 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/__init__.py
+-rw-r--r--   0        0        0     4017 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001.py
+-rw-r--r--   0        0        0     4020 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     4155 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     4150 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     4149 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cors/__init__.py
+-rw-r--r--   0        0        0     1278 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cors/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/__init__.py
+-rw-r--r--   0        0        0     1358 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py
+-rw-r--r--   0        0        0     1249 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/__init__.py
+-rw-r--r--   0        0        0      886 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
+-rw-r--r--   0        0        0     1245 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
+-rw-r--r--   0        0        0      526 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/__init__.py
+-rw-r--r--   0        0        0     1025 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001.py
+-rw-r--r--   0        0        0     1026 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001b.py
+-rw-r--r--   0        0        0     1221 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial004.py
+-rw-r--r--   0        0        0      980 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial005.py
+-rw-r--r--   0        0        0     1059 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006.py
+-rw-r--r--   0        0        0      899 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006b.py
+-rw-r--r--   0        0        0      899 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006c.py
+-rw-r--r--   0        0        0      264 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial007.py
+-rw-r--r--   0        0        0      487 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial008.py
+-rw-r--r--   0        0        0      487 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial009.py
+-rw-r--r--   0        0        0      490 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial009b.py
+-rw-r--r--   0        0        0      239 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial009c.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/__init__.py
+-rw-r--r--   0        0        0     5289 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial001.py
+-rw-r--r--   0        0        0     3574 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial002.py
+-rw-r--r--   0        0        0    12356 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     7222 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7402 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7398 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7399 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5551 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004.py
+-rw-r--r--   0        0        0     5554 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5734 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5730 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5731 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     5119 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006.py
+-rw-r--r--   0        0        0     5122 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
+-rw-r--r--   0        0        0     5400 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0      697 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b.py
+-rw-r--r--   0        0        0      700 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py
+-rw-r--r--   0        0        0      918 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py
+-rw-r--r--   0        0        0     1166 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c.py
+-rw-r--r--   0        0        0     1172 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py
+-rw-r--r--   0        0        0     1263 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py
+-rw-r--r--   0        0        0     1226 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d.py
+-rw-r--r--   0        0        0     1235 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py
+-rw-r--r--   0        0        0     1331 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py
+-rw-r--r--   0        0        0     8638 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012.py
+-rw-r--r--   0        0        0     8641 2024-04-30 06:11:45.546818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
+-rw-r--r--   0        0        0     9039 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/__init__.py
+-rw-r--r--   0        0        0     3638 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial001.py
+-rw-r--r--   0        0        0     1414 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial002.py
+-rw-r--r--   0        0        0     3684 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extending_openapi/__init__.py
+-rw-r--r--   0        0        0     1545 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/__init__.py
+-rw-r--r--   0        0        0     6971 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
+-rw-r--r--   0        0        0     6974 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7166 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     7162 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7163 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/__init__.py
+-rw-r--r--   0        0        0     5195 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003.py
+-rw-r--r--   0        0        0     5418 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1981 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004.py
+-rw-r--r--   0        0        0     2169 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     1480 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005.py
+-rw-r--r--   0        0        0     1668 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0     1205 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_generate_clients/__init__.py
+-rw-r--r--   0        0        0     7247 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_generate_clients/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/__init__.py
+-rw-r--r--   0        0        0     3298 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial001.py
+-rw-r--r--   0        0        0     3371 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial002.py
+-rw-r--r--   0        0        0     3294 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial003.py
+-rw-r--r--   0        0        0     3800 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial004.py
+-rw-r--r--   0        0        0     4429 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial005.py
+-rw-r--r--   0        0        0     4072 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/__init__.py
+-rw-r--r--   0        0        0     3869 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3872 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     4052 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     4049 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     4095 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002.py
+-rw-r--r--   0        0        0     4098 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an.py
+-rw-r--r--   0        0        0     4278 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     4349 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     4348 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     4240 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003.py
+-rw-r--r--   0        0        0     4225 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     4405 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     4401 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     4402 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/__init__.py
+-rw-r--r--   0        0        0     1764 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001.py
+-rw-r--r--   0        0        0     1728 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001_1.py
+-rw-r--r--   0        0        0     2077 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_openapi_callbacks/__init__.py
+-rw-r--r--   0        0        0     9216 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_openapi_webhooks/__init__.py
+-rw-r--r--   0        0        0     4492 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
+-rw-r--r--   0        0        0     1020 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
+-rw-r--r--   0        0        0      575 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
+-rw-r--r--   0        0        0     8915 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
+-rw-r--r--   0        0        0     1034 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     1987 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0     3419 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
+-rw-r--r--   0        0        0     3266 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/__init__.py
+-rw-r--r--   0        0        0     1722 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
+-rw-r--r--   0        0        0     8900 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     9102 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     9097 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2405 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_params/__init__.py
+-rw-r--r--   0        0        0     3369 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial004.py
+-rw-r--r--   0        0        0     5142 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/__init__.py
+-rw-r--r--   0        0        0     4072 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial005.py
+-rw-r--r--   0        0        0     6285 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006.py
+-rw-r--r--   0        0        0     6364 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/__init__.py
+-rw-r--r--   0        0        0     6388 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
+-rw-r--r--   0        0        0     6391 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
+-rw-r--r--   0        0        0     6496 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
+-rw-r--r--   0        0        0     6489 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
+-rw-r--r--   0        0        0     6493 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     4017 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
+-rw-r--r--   0        0        0     4020 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
+-rw-r--r--   0        0        0     4243 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
+-rw-r--r--   0        0        0     4238 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
+-rw-r--r--   0        0        0     4240 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     4235 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
+-rw-r--r--   0        0        0     3485 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
+-rw-r--r--   0        0        0     3488 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
+-rw-r--r--   0        0        0     3706 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0     3703 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
+-rw-r--r--   0        0        0     3434 2024-04-30 06:11:45.550819 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
+-rw-r--r--   0        0        0     3437 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
+-rw-r--r--   0        0        0     3655 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
+-rw-r--r--   0        0        0     2937 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
+-rw-r--r--   0        0        0     2940 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
+-rw-r--r--   0        0        0     3163 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
+-rw-r--r--   0        0        0     3162 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
+-rw-r--r--   0        0        0     3160 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/__init__.py
+-rw-r--r--   0        0        0     7886 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001.py
+-rw-r--r--   0        0        0     8388 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02.py
+-rw-r--r--   0        0        0     8391 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
+-rw-r--r--   0        0        0     8660 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0     8653 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0     8657 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
+-rw-r--r--   0        0        0     6133 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03.py
+-rw-r--r--   0        0        0     6136 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
+-rw-r--r--   0        0        0     6300 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0     7708 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7935 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8679 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002.py
+-rw-r--r--   0        0        0     8682 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an.py
+-rw-r--r--   0        0        0     9076 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     9255 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     7311 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003.py
+-rw-r--r--   0        0        0     7314 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7830 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7827 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/__init__.py
+-rw-r--r--   0        0        0     7630 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001.py
+-rw-r--r--   0        0        0     7633 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
+-rw-r--r--   0        0        0     7743 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/__init__.py
+-rw-r--r--   0        0        0    10042 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
+-rw-r--r--   0        0        0    10045 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0    10155 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_change_status_code/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_cookies/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_cookies/test_tutorial001.py
+-rw-r--r--   0        0        0      414 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_cookies/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_headers/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_headers/test_tutorial001.py
+-rw-r--r--   0        0        0      378 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_headers/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/__init__.py
+-rw-r--r--   0        0        0     5764 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003.py
+-rw-r--r--   0        0        0     5770 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01.py
+-rw-r--r--   0        0        0     5962 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
+-rw-r--r--   0        0        0     3476 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_02.py
+-rw-r--r--   0        0        0     1090 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_03.py
+-rw-r--r--   0        0        0      236 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_04.py
+-rw-r--r--   0        0        0      289 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
+-rw-r--r--   0        0        0     3476 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05.py
+-rw-r--r--   0        0        0     3699 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
+-rw-r--r--   0        0        0     5956 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     5108 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004.py
+-rw-r--r--   0        0        0     5288 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     5284 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     6154 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005.py
+-rw-r--r--   0        0        0     6377 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     6154 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006.py
+-rw-r--r--   0        0        0     6377 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/__init__.py
+-rw-r--r--   0        0        0     4779 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py
+-rw-r--r--   0        0        0     4555 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py
+-rw-r--r--   0        0        0     4824 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     4600 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py
+-rw-r--r--   0        0        0     7060 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
+-rw-r--r--   0        0        0     7063 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
+-rw-r--r--   0        0        0     7255 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     7251 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     7252 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     6907 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py
+-rw-r--r--   0        0        0     6910 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py
+-rw-r--r--   0        0        0     6976 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0     6972 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0     6973 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/__init__.py
+-rw-r--r--   0        0        0     1905 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001.py
+-rw-r--r--   0        0        0     1908 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2156 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     8182 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003.py
+-rw-r--r--   0        0        0     8185 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an.py
+-rw-r--r--   0        0        0     8594 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     8583 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     8591 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_py310.py
+-rw-r--r--   0        0        0    15803 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005.py
+-rw-r--r--   0        0        0    15806 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an.py
+-rw-r--r--   0        0        0    16711 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0    16687 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0    16699 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py310.py
+-rw-r--r--   0        0        0    16675 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2318 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006.py
+-rw-r--r--   0        0        0     2321 2024-04-30 06:11:45.554818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an.py
+-rw-r--r--   0        0        0     2594 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py
+-rw-r--r--   0        0        0     5016 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5011 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py
+-rw-r--r--   0        0        0     4958 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py
+-rw-r--r--   0        0        0     5016 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     5011 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_settings/__init__.py
+-rw-r--r--   0        0        0      488 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_settings/test_app02.py
+-rw-r--r--   0        0        0      552 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001.py
+-rw-r--r--   0        0        0      556 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001_pv1.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/__init__.py
+-rw-r--r--   0        0        0    16475 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases.py
+-rw-r--r--   0        0        0    16654 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
+-rw-r--r--   0        0        0    16924 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
+-rw-r--r--   0        0        0    16925 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
+-rw-r--r--   0        0        0    16930 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
+-rw-r--r--   0        0        0    16921 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
+-rw-r--r--   0        0        0      788 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases.py
+-rw-r--r--   0        0        0      825 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
+-rw-r--r--   0        0        0      822 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sub_applications/__init__.py
+-rw-r--r--   0        0        0     1920 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sub_applications/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_templates/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_templates/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main.py
+-rw-r--r--   0        0        0      300 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b.py
+-rw-r--r--   0        0        0      303 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_an.py
+-rw-r--r--   0        0        0      360 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_an_py310.py
+-rw-r--r--   0        0        0      357 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_an_py39.py
+-rw-r--r--   0        0        0      357 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main_b_py310.py
+-rw-r--r--   0        0        0      821 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial001.py
+-rw-r--r--   0        0        0      154 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial002.py
+-rw-r--r--   0        0        0      167 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/__init__.py
+-rw-r--r--   0        0        0     1527 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     1530 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2088 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     2073 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     2067 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/__init__.py
+-rw-r--r--   0        0        0      822 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial001.py
+-rw-r--r--   0        0        0     3683 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002.py
+-rw-r--r--   0        0        0     3686 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3968 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3960 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3965 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      872 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003.py
+-rw-r--r--   0        0        0     1288 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_wsgi/__init__.py
+-rw-r--r--   0        0        0      436 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_wsgi/test_tutorial001.py
+-rw-r--r--   0        0        0      709 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_typing_python39.py
+-rw-r--r--   0        0        0     4748 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_union_body.py
+-rw-r--r--   0        0        0     5311 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_union_inherited_body.py
+-rw-r--r--   0        0        0     2031 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response.py
+-rw-r--r--   0        0        0     1208 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response_dataclass.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/__init__.py
+-rw-r--r--   0        0        0     1149 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/app_pv1.py
+-rw-r--r--   0        0        0     1178 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/app_pv2.py
+-rw-r--r--   0        0        0      900 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py
+-rw-r--r--   0        0        0      900 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py
+-rw-r--r--   0        0        0     4667 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_webhooks_security.py
+-rw-r--r--   0        0        0     2199 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_ws_dependencies.py
+-rw-r--r--   0        0        0     7651 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/test_ws_router.py
+-rw-r--r--   0        0        0      422 2024-04-30 06:11:45.558818 fastapi_slim-0.111.0.dev1/tests/utils.py
+-rw-r--r--   0        0        0    25381 1970-01-01 00:00:00.000000 fastapi_slim-0.111.0.dev1/PKG-INFO
```

### Comparing `fastapi_slim-0.111.0/LICENSE` & `fastapi_slim-0.111.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/README.md` & `fastapi_slim-0.111.0.dev1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -135,14 +135,26 @@
 $ pip install fastapi
 
 ---> 100%
 ```
 
 </div>
 
+You will also need an ASGI server, for production such as <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a> or <a href="https://github.com/pgjones/hypercorn" class="external-link" target="_blank">Hypercorn</a>.
+
+<div class="termy">
+
+```console
+$ pip install "uvicorn[standard]"
+
+---> 100%
+```
+
+</div>
+
 ## Example
 
 ### Create it
 
 * Create a file `main.py` with:
 
 ```Python
@@ -195,46 +207,33 @@
 ### Run it
 
 Run the server with:
 
 <div class="termy">
 
 ```console
-$ fastapi dev main.py
-
- ╭────────── FastAPI CLI - Development mode ───────────╮
- │                                                     │
- │  Serving at: http://127.0.0.1:8000                  │
- │                                                     │
- │  API docs: http://127.0.0.1:8000/docs               │
- │                                                     │
- │  Running in development mode, for production use:   │
- │                                                     │
- │  fastapi run                                        │
- │                                                     │
- ╰─────────────────────────────────────────────────────╯
+$ uvicorn main:app --reload
 
-INFO:     Will watch for changes in these directories: ['/home/user/code/awesomeapp']
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-INFO:     Started reloader process [2248755] using WatchFiles
-INFO:     Started server process [2248757]
+INFO:     Started reloader process [28720]
+INFO:     Started server process [28722]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
 </div>
 
 <details markdown="1">
-<summary>About the command <code>fastapi dev main.py</code>...</summary>
+<summary>About the command <code>uvicorn main:app --reload</code>...</summary>
 
-The command `fastapi dev` reads your `main.py` file, detects the **FastAPI** app in it, and starts a server using <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a>.
+The command `uvicorn main:app` refers to:
 
-By default, `fastapi dev` will start with auto-reload enabled for local development.
-
-You can read more about it in the <a href="https://fastapi.tiangolo.com/fastapi-cli/" target="_blank">FastAPI CLI docs</a>.
+* `main`: the file `main.py` (the Python "module").
+* `app`: the object created inside of `main.py` with the line `app = FastAPI()`.
+* `--reload`: make the server restart after code changes. Only do this for development.
 
 </details>
 
 ### Check it
 
 Open your browser at <a href="http://127.0.0.1:8000/items/5?q=somequery" class="external-link" target="_blank">http://127.0.0.1:8000/items/5?q=somequery</a>.
 
@@ -299,15 +298,15 @@
 
 
 @app.put("/items/{item_id}")
 def update_item(item_id: int, item: Item):
     return {"item_name": item.name, "item_id": item_id}
 ```
 
-The `fastapi dev` server should reload automatically.
+The server should reload automatically (because you added `--reload` to the `uvicorn` command above).
 
 ### Interactive API docs upgrade
 
 Now go to <a href="http://127.0.0.1:8000/docs" class="external-link" target="_blank">http://127.0.0.1:8000/docs</a>.
 
 * The interactive API documentation will be automatically updated, including the new body:
 
@@ -443,51 +442,34 @@
 
 ## Performance
 
 Independent TechEmpower benchmarks show **FastAPI** applications running under Uvicorn as <a href="https://www.techempower.com/benchmarks/#section=test&runid=7464e520-0dc2-473d-bd34-dbdfd7e85911&hw=ph&test=query&l=zijzen-7" class="external-link" target="_blank">one of the fastest Python frameworks available</a>, only below Starlette and Uvicorn themselves (used internally by FastAPI). (*)
 
 To understand more about it, see the section <a href="https://fastapi.tiangolo.com/benchmarks/" class="internal-link" target="_blank">Benchmarks</a>.
 
-## Dependencies
+## Optional Dependencies
 
 Used by Pydantic:
 
 * <a href="https://github.com/JoshData/python-email-validator" target="_blank"><code>email_validator</code></a> - for email validation.
 * <a href="https://docs.pydantic.dev/latest/usage/pydantic_settings/" target="_blank"><code>pydantic-settings</code></a> - for settings management.
 * <a href="https://docs.pydantic.dev/latest/usage/types/extra_types/extra_types/" target="_blank"><code>pydantic-extra-types</code></a> - for extra types to be used with Pydantic.
 
 Used by Starlette:
 
 * <a href="https://www.python-httpx.org" target="_blank"><code>httpx</code></a> - Required if you want to use the `TestClient`.
 * <a href="https://jinja.palletsprojects.com" target="_blank"><code>jinja2</code></a> - Required if you want to use the default template configuration.
 * <a href="https://github.com/Kludex/python-multipart" target="_blank"><code>python-multipart</code></a> - Required if you want to support form <abbr title="converting the string that comes from an HTTP request into Python data">"parsing"</abbr>, with `request.form()`.
+* <a href="https://pythonhosted.org/itsdangerous/" target="_blank"><code>itsdangerous</code></a> - Required for `SessionMiddleware` support.
+* <a href="https://pyyaml.org/wiki/PyYAMLDocumentation" target="_blank"><code>pyyaml</code></a> - Required for Starlette's `SchemaGenerator` support (you probably don't need it with FastAPI).
 
 Used by FastAPI / Starlette:
 
 * <a href="https://www.uvicorn.org" target="_blank"><code>uvicorn</code></a> - for the server that loads and serves your application.
 * <a href="https://github.com/ijl/orjson" target="_blank"><code>orjson</code></a> - Required if you want to use `ORJSONResponse`.
 * <a href="https://github.com/esnme/ultrajson" target="_blank"><code>ujson</code></a> - Required if you want to use `UJSONResponse`.
-* `fastapi-cli` - to provide the `fastapi` command.
-
-When you install `fastapi` it comes these standard dependencies.
-
-## `fastapi-slim`
-
-If you don't want the extra standard optional dependencies, install `fastapi-slim` instead.
-
-When you install with:
-
-```bash
-pip install fastapi
-```
-
-...it includes the same code and dependencies as:
-
-```bash
-pip install "fastapi-slim[standard]"
-```
 
-The standard extra dependencies are the ones mentioned above.
+You can install all of these with `pip install "fastapi[all]"`.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -62,63 +62,59 @@
 --- ## **Typer**, the FastAPI of CLIs _[_h_t_t_p_s_:_/_/_t_y_p_e_r_._t_i_a_n_g_o_l_o_._c_o_m_/_i_m_g_/_l_o_g_o_-
 _m_a_r_g_i_n_/_l_o_g_o_-_m_a_r_g_i_n_-_v_e_c_t_o_r_._s_v_g_]If you are building a CLI app to be used in the
 terminal instead of a web API, check out _*_*_T_y_p_e_r_*_*. **Typer** is FastAPI's
 little sibling. And it's intended to be the **FastAPI of CLIs**. â¨ï¸ ð ##
 Requirements FastAPI stands on the shoulders of giants: * _S_t_a_r_l_e_t_t_e for the web
 parts. * _P_y_d_a_n_t_i_c for the data parts. ## Installation
 ```console $ pip install fastapi ---> 100% ```
+You will also need an ASGI server, for production such as _U_v_i_c_o_r_n or _H_y_p_e_r_c_o_r_n.
+```console $ pip install "uvicorn[standard]" ---> 100% ```
 ## Example ### Create it * Create a file `main.py` with: ```Python from typing
 import Union from fastapi import FastAPI app = FastAPI() @app.get("/") def
 read_root(): return {"Hello": "World"} @app.get("/items/{item_id}") def
 read_item(item_id: int, q: Union[str, None] = None): return {"item_id":
 item_id, "q": q} ``` Or use async def... If your code uses `async` / `await`,
 use `async def`: ```Python hl_lines="9 14" from typing import Union from
 fastapi import FastAPI app = FastAPI() @app.get("/") async def read_root():
 return {"Hello": "World"} @app.get("/items/{item_id}") async def read_item
 (item_id: int, q: Union[str, None] = None): return {"item_id": item_id, "q": q}
 ``` **Note**: If you don't know, check the _"In a hurry?"_ section about
 _`_a_s_y_n_c_`_ _a_n_d_ _`_a_w_a_i_t_`_ _i_n_ _t_h_e_ _d_o_c_s. ### Run it Run the server with:
-```console $ fastapi dev main.py â­ââââââââââ FastAPI CLI
-- Development mode ââââââââââââ® â â â Serving at:
-http://127.0.0.1:8000 â â â â API docs: http://127.0.0.1:8000/docs â
-â â â Running in development mode, for production use: â â â â
-fastapi run â â â
-â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
-INFO: Will watch for changes in these directories: ['/home/user/code/
-awesomeapp'] INFO: Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to
-quit) INFO: Started reloader process [2248755] using WatchFiles INFO: Started
-server process [2248757] INFO: Waiting for application startup. INFO:
-Application startup complete. ```
-About the command fastapi dev main.py... The command `fastapi dev` reads your
-`main.py` file, detects the **FastAPI** app in it, and starts a server using
-_U_v_i_c_o_r_n. By default, `fastapi dev` will start with auto-reload enabled for
-local development. You can read more about it in the _F_a_s_t_A_P_I_ _C_L_I_ _d_o_c_s. ###
-Check it Open your browser at _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_i_t_e_m_s_/_5_?_q_=_s_o_m_e_q_u_e_r_y. You
-will see the JSON response as: ```JSON {"item_id": 5, "q": "somequery"} ``` You
-already created an API that: * Receives HTTP requests in the _paths_ `/` and `/
-items/{item_id}`. * Both _paths_ take `GET` ooppeerraattiioonnss (also known as HTTP
-_methods_). * The _path_ `/items/{item_id}` has a _path parameter_ `item_id`
-that should be an `int`. * The _path_ `/items/{item_id}` has an optional `str`
-_query parameter_ `q`. ### Interactive API docs Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:
-_8_0_0_0_/_d_o_c_s. You will see the automatic interactive API documentation (provided
-by _S_w_a_g_g_e_r_ _U_I): ![Swagger UI](https://fastapi.tiangolo.com/img/index/index-01-
-swagger-ui-simple.png) ### Alternative API docs And now, go to _h_t_t_p_:_/_/
-_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. You will see the alternative automatic documentation
-(provided by _R_e_D_o_c): ![ReDoc](https://fastapi.tiangolo.com/img/index/index-02-
-redoc-simple.png) ## Example upgrade Now modify the file `main.py` to receive a
-body from a `PUT` request. Declare the body using standard Python types, thanks
-to Pydantic. ```Python hl_lines="4 9-12 25-27" from typing import Union from
-fastapi import FastAPI from pydantic import BaseModel app = FastAPI() class
-Item(BaseModel): name: str price: float is_offer: Union[bool, None] = None
-@app.get("/") def read_root(): return {"Hello": "World"} @app.get("/items/
-{item_id}") def read_item(item_id: int, q: Union[str, None] = None): return
-{"item_id": item_id, "q": q} @app.put("/items/{item_id}") def update_item
-(item_id: int, item: Item): return {"item_name": item.name, "item_id": item_id}
-``` The `fastapi dev` server should reload automatically. ### Interactive API
-docs upgrade Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. * The interactive API
+```console $ uvicorn main:app --reload INFO: Uvicorn running on http://
+127.0.0.1:8000 (Press CTRL+C to quit) INFO: Started reloader process [28720]
+INFO: Started server process [28722] INFO: Waiting for application startup.
+INFO: Application startup complete. ```
+About the command uvicorn main:app --reload... The command `uvicorn main:app`
+refers to: * `main`: the file `main.py` (the Python "module"). * `app`: the
+object created inside of `main.py` with the line `app = FastAPI()`. * `--
+reload`: make the server restart after code changes. Only do this for
+development. ### Check it Open your browser at _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_i_t_e_m_s_/
+_5_?_q_=_s_o_m_e_q_u_e_r_y. You will see the JSON response as: ```JSON {"item_id": 5, "q":
+"somequery"} ``` You already created an API that: * Receives HTTP requests in
+the _paths_ `/` and `/items/{item_id}`. * Both _paths_ take `GET` ooppeerraattiioonnss
+(also known as HTTP _methods_). * The _path_ `/items/{item_id}` has a _path
+parameter_ `item_id` that should be an `int`. * The _path_ `/items/{item_id}`
+has an optional `str` _query parameter_ `q`. ### Interactive API docs Now go to
+_h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. You will see the automatic interactive API
+documentation (provided by _S_w_a_g_g_e_r_ _U_I): ![Swagger UI](https://
+fastapi.tiangolo.com/img/index/index-01-swagger-ui-simple.png) ### Alternative
+API docs And now, go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. You will see the
+alternative automatic documentation (provided by _R_e_D_o_c): ![ReDoc](https://
+fastapi.tiangolo.com/img/index/index-02-redoc-simple.png) ## Example upgrade
+Now modify the file `main.py` to receive a body from a `PUT` request. Declare
+the body using standard Python types, thanks to Pydantic. ```Python hl_lines="4
+9-12 25-27" from typing import Union from fastapi import FastAPI from pydantic
+import BaseModel app = FastAPI() class Item(BaseModel): name: str price: float
+is_offer: Union[bool, None] = None @app.get("/") def read_root(): return
+{"Hello": "World"} @app.get("/items/{item_id}") def read_item(item_id: int, q:
+Union[str, None] = None): return {"item_id": item_id, "q": q} @app.put("/items/
+{item_id}") def update_item(item_id: int, item: Item): return {"item_name":
+item.name, "item_id": item_id} ``` The server should reload automatically
+(because you added `--reload` to the `uvicorn` command above). ### Interactive
+API docs upgrade Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. * The interactive API
 documentation will be automatically updated, including the new body: ![Swagger
 UI](https://fastapi.tiangolo.com/img/index/index-03-swagger-02.png) * Click on
 the button "Try it out", it allows you to fill the parameters and directly
 interact with the API: ![Swagger UI interaction](https://fastapi.tiangolo.com/
 img/index/index-04-swagger-03.png) * Then click on the "Execute" button, the
 user interface will communicate with your API, send the parameters, get the
 results and show them on the screen: ![Swagger UI interaction](https://
@@ -173,22 +169,20 @@
 Pydantic). * **GraphQL** integration with _S_t_r_a_w_b_e_r_r_y and other libraries. *
 Many extra features (thanks to Starlette) as: * **WebSockets** * extremely easy
 tests based on HTTPX and `pytest` * **CORS** * **Cookie Sessions** * ...and
 more. ## Performance Independent TechEmpower benchmarks show **FastAPI**
 applications running under Uvicorn as _o_n_e_ _o_f_ _t_h_e_ _f_a_s_t_e_s_t_ _P_y_t_h_o_n_ _f_r_a_m_e_w_o_r_k_s
 _a_v_a_i_l_a_b_l_e, only below Starlette and Uvicorn themselves (used internally by
 FastAPI). (*) To understand more about it, see the section _B_e_n_c_h_m_a_r_k_s. ##
-Dependencies Used by Pydantic: * _e_m_a_i_l___v_a_l_i_d_a_t_o_r - for email validation. *
-_p_y_d_a_n_t_i_c_-_s_e_t_t_i_n_g_s - for settings management. * _p_y_d_a_n_t_i_c_-_e_x_t_r_a_-_t_y_p_e_s - for extra
-types to be used with Pydantic. Used by Starlette: * _h_t_t_p_x - Required if you
-want to use the `TestClient`. * _j_i_n_j_a_2 - Required if you want to use the
-default template configuration. * _p_y_t_h_o_n_-_m_u_l_t_i_p_a_r_t - Required if you want to
-support form "parsing", with `request.form()`. Used by FastAPI / Starlette: *
-_u_v_i_c_o_r_n - for the server that loads and serves your application. * _o_r_j_s_o_n -
-Required if you want to use `ORJSONResponse`. * _u_j_s_o_n - Required if you want to
-use `UJSONResponse`. * `fastapi-cli` - to provide the `fastapi` command. When
-you install `fastapi` it comes these standard dependencies. ## `fastapi-slim`
-If you don't want the extra standard optional dependencies, install `fastapi-
-slim` instead. When you install with: ```bash pip install fastapi ``` ...it
-includes the same code and dependencies as: ```bash pip install "fastapi-slim
-[standard]" ``` The standard extra dependencies are the ones mentioned above.
-## License This project is licensed under the terms of the MIT license.
+Optional Dependencies Used by Pydantic: * _e_m_a_i_l___v_a_l_i_d_a_t_o_r - for email
+validation. * _p_y_d_a_n_t_i_c_-_s_e_t_t_i_n_g_s - for settings management. * _p_y_d_a_n_t_i_c_-_e_x_t_r_a_-
+_t_y_p_e_s - for extra types to be used with Pydantic. Used by Starlette: * _h_t_t_p_x -
+Required if you want to use the `TestClient`. * _j_i_n_j_a_2 - Required if you want
+to use the default template configuration. * _p_y_t_h_o_n_-_m_u_l_t_i_p_a_r_t - Required if you
+want to support form "parsing", with `request.form()`. * _i_t_s_d_a_n_g_e_r_o_u_s -
+Required for `SessionMiddleware` support. * _p_y_y_a_m_l - Required for Starlette's
+`SchemaGenerator` support (you probably don't need it with FastAPI). Used by
+FastAPI / Starlette: * _u_v_i_c_o_r_n - for the server that loads and serves your
+application. * _o_r_j_s_o_n - Required if you want to use `ORJSONResponse`. * _u_j_s_o_n -
+Required if you want to use `UJSONResponse`. You can install all of these with
+`pip install "fastapi[all]"`. ## License This project is licensed under the
+terms of the MIT license.
```

### Comparing `fastapi_slim-0.111.0/docs/en/docs/img/favicon.png` & `fastapi_slim-0.111.0.dev1/docs/en/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_responses/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_responses/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_responses/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_responses/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/additional_status_codes/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/additional_status_codes/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_an/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_an/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py310/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py310/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py39/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_an_py39/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_py310/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/app_b_py310/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/app_b_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/app_testing/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/app_testing/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/async_sql_databases/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/async_sql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/background_tasks/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/background_tasks/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/background_tasks/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/bigger_applications/app/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/bigger_applications/app/routers/items.py` & `fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/bigger_applications/app_an/routers/items.py` & `fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/bigger_applications/app_an_py39/routers/items.py` & `fastapi_slim-0.111.0.dev1/docs_src/bigger_applications/app_an_py39/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_fields/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_fields/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_fields/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_multiple_params/tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_multiple_params/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial005_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial006.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial006_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial006_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial007.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial007_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_nested_models/tutorial007_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_nested_models/tutorial007_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_updates/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_updates/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_updates/tutorial001_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_updates/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_updates/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/body_updates/tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/body_updates/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/custom_docs_ui/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/custom_docs_ui/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/custom_docs_ui/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/custom_docs_ui/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/custom_request_and_route/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/custom_request_and_route/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/custom_request_and_route/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/custom_request_and_route/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/custom_request_and_route/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/custom_request_and_route/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dataclasses/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/dataclasses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dataclasses/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/dataclasses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial005_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial005_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial006.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial006_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial006_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008b.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008b.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008b_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008b_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008b_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008b_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008c.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008c.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008c_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008c_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008c_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008c_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008d.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008d.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008d_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008d_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial008d_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial008d_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial011_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial011_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial012.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial012_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependencies/tutorial012_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependencies/tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/dependency_testing/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/dependency_testing/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/events/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/events/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extending_openapi/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/extending_openapi/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_data_types/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_data_types/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_models/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_models/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_models/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_models/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_models/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/extra_models/tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/extra_models/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/generate_clients/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/generate_clients/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/generate_clients/tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/generate_clients/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/generate_clients/tutorial003_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/generate_clients/tutorial004.js` & `fastapi_slim-0.111.0.dev1/docs_src/generate_clients/tutorial004.js`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/handling_errors/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/handling_errors/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/handling_errors/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/handling_errors/tutorial006.py` & `fastapi_slim-0.111.0.dev1/docs_src/handling_errors/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/metadata/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/metadata/tutorial001_1.py` & `fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/metadata/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/metadata/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/nosql_databases/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/nosql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/openapi_callbacks/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/openapi_callbacks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/openapi_webhooks/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/openapi_webhooks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial006.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial007.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_advanced_configuration/tutorial007_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial003_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial004_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_operation_configuration/tutorial005_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_operation_configuration/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/path_params/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/path_params/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial008_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010.py` & `fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/query_params_str_validations/tutorial010_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/query_params_str_validations/tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial001_02_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/request_files/tutorial003_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/request_files/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial001_01.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_01.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial001_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial004_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial006.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/response_model/tutorial006_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/response_model/tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001_pv1.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial001_py310_pv1.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial001_py310_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/schema_extra_example/tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/schema_extra_example/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial004.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial004_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial004_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial004_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial005.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial005_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial005_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial005_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial005_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial007.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial007_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/security/tutorial007_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/security/tutorial007_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/separate_openapi_schemas/tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/separate_openapi_schemas/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/settings/app02/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/settings/app02/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/settings/app02_an/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/settings/app02_an_py39/test_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/settings/app02_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/alt_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/crud.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/models.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/alt_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/crud.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/models.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/alt_main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/crud.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/models.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/crud.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/database.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/database.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/main.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/sql_databases_peewee/sql_app/schemas.py` & `fastapi_slim-0.111.0.dev1/docs_src/sql_databases_peewee/sql_app/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/templates/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/templates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial001.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial002.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial003.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/docs_src/websockets/tutorial003_py39.py` & `fastapi_slim-0.111.0.dev1/docs_src/websockets/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/__init__.py` & `fastapi_slim-0.111.0.dev1/fastapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """FastAPI framework, high performance, easy to learn, fast to code, ready for production"""
 
-__version__ = "0.111.0"
+__version__ = "0.111.0.dev1"
 
 from starlette import status as status
 
 from .applications import FastAPI as FastAPI
 from .background import BackgroundTasks as BackgroundTasks
 from .datastructures import UploadFile as UploadFile
 from .exceptions import HTTPException as HTTPException
```

### Comparing `fastapi_slim-0.111.0/fastapi/_compat.py` & `fastapi_slim-0.111.0.dev1/fastapi/_compat.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/applications.py` & `fastapi_slim-0.111.0.dev1/fastapi/applications.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/background.py` & `fastapi_slim-0.111.0.dev1/fastapi/background.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/concurrency.py` & `fastapi_slim-0.111.0.dev1/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/datastructures.py` & `fastapi_slim-0.111.0.dev1/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/dependencies/models.py` & `fastapi_slim-0.111.0.dev1/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/dependencies/utils.py` & `fastapi_slim-0.111.0.dev1/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/encoders.py` & `fastapi_slim-0.111.0.dev1/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/exception_handlers.py` & `fastapi_slim-0.111.0.dev1/fastapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/exceptions.py` & `fastapi_slim-0.111.0.dev1/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/openapi/docs.py` & `fastapi_slim-0.111.0.dev1/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/openapi/models.py` & `fastapi_slim-0.111.0.dev1/fastapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/openapi/utils.py` & `fastapi_slim-0.111.0.dev1/fastapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/param_functions.py` & `fastapi_slim-0.111.0.dev1/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/params.py` & `fastapi_slim-0.111.0.dev1/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/responses.py` & `fastapi_slim-0.111.0.dev1/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/routing.py` & `fastapi_slim-0.111.0.dev1/fastapi/routing.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/security/__init__.py` & `fastapi_slim-0.111.0.dev1/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/security/api_key.py` & `fastapi_slim-0.111.0.dev1/fastapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/security/http.py` & `fastapi_slim-0.111.0.dev1/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/security/oauth2.py` & `fastapi_slim-0.111.0.dev1/fastapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/security/open_id_connect_url.py` & `fastapi_slim-0.111.0.dev1/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/fastapi/utils.py` & `fastapi_slim-0.111.0.dev1/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/pdm_build.py` & `fastapi_slim-0.111.0.dev1/pdm_build.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/pyproject.toml` & `fastapi_slim-0.111.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,34 +43,32 @@
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "starlette>=0.37.2,<0.38.0",
     "pydantic>=1.7.4,!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0",
     "typing-extensions>=4.8.0",
 ]
-version = "0.111.0"
+version = "0.111.0.dev1"
 
 [project.urls]
 Homepage = "https://github.com/tiangolo/fastapi"
 Documentation = "https://fastapi.tiangolo.com/"
 Repository = "https://github.com/tiangolo/fastapi"
 
 [project.optional-dependencies]
 standard = [
-    "fastapi-cli >=0.0.2",
     "httpx >=0.23.0",
     "jinja2 >=2.11.2",
     "python-multipart >=0.0.7",
     "ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0",
     "orjson >=3.2.1",
     "email_validator >=2.0.0",
     "uvicorn[standard] >=0.12.0",
 ]
 all = [
-    "fastapi-cli >=0.0.2",
     "httpx >=0.23.0",
     "jinja2 >=2.11.2",
     "python-multipart >=0.0.7",
     "itsdangerous >=1.1.0",
     "pyyaml >=5.3.1",
     "ujson >=4.0.1,!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0",
     "orjson >=3.2.1",
```

### Comparing `fastapi_slim-0.111.0/scripts/docs.py` & `fastapi_slim-0.111.0.dev1/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/scripts/mkdocs_hooks.py` & `fastapi_slim-0.111.0.dev1/scripts/mkdocs_hooks.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image01.py` & `fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image01.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image02.py` & `fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image02.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image03.py` & `fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image03.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image04.py` & `fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image04.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/scripts/playwright/separate_openapi_schemas/image05.py` & `fastapi_slim-0.111.0.dev1/scripts/playwright/separate_openapi_schemas/image05.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/main.py` & `fastapi_slim-0.111.0.dev1/tests/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_properties.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_properties_bool.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_properties_bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_response_extra.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_responses_bad.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_responses_custom_model_in_callback.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_responses_custom_validationerror.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_responses_default_validationerror.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_responses_response_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_additional_responses_router.py` & `fastapi_slim-0.111.0.dev1/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_ambiguous_params.py` & `fastapi_slim-0.111.0.dev1/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_annotated.py` & `fastapi_slim-0.111.0.dev1/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_application.py` & `fastapi_slim-0.111.0.dev1/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_compat.py` & `fastapi_slim-0.111.0.dev1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_computed_fields.py` & `fastapi_slim-0.111.0.dev1/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_custom_middleware_exception.py` & `fastapi_slim-0.111.0.dev1/tests/test_custom_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_custom_route_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_custom_route_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_custom_schema_fields.py` & `fastapi_slim-0.111.0.dev1/tests/test_custom_schema_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_custom_swagger_ui_redirect.py` & `fastapi_slim-0.111.0.dev1/tests/test_custom_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_datastructures.py` & `fastapi_slim-0.111.0.dev1/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_datetime_custom_encoder.py` & `fastapi_slim-0.111.0.dev1/tests/test_datetime_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_default_response_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_default_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_default_response_class_router.py` & `fastapi_slim-0.111.0.dev1/tests/test_default_response_class_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_cache.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_contextmanager.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_contextmanager.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_contextvars.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_contextvars.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_duplicates.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_duplicates.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_normal_exceptions.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_normal_exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_overrides.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_dependency_security_overrides.py` & `fastapi_slim-0.111.0.dev1/tests/test_dependency_security_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_deprecated_openapi_prefix.py` & `fastapi_slim-0.111.0.dev1/tests/test_deprecated_openapi_prefix.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_duplicate_models_openapi.py` & `fastapi_slim-0.111.0.dev1/tests/test_duplicate_models_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_empty_router.py` & `fastapi_slim-0.111.0.dev1/tests/test_empty_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_enforce_once_required_parameter.py` & `fastapi_slim-0.111.0.dev1/tests/test_enforce_once_required_parameter.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_exception_handlers.py` & `fastapi_slim-0.111.0.dev1/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_extra_routes.py` & `fastapi_slim-0.111.0.dev1/tests/test_extra_routes.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model/app_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model/app_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model/test_filter_pydantic_sub_model_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_filter_pydantic_sub_model_pv2.py` & `fastapi_slim-0.111.0.dev1/tests/test_filter_pydantic_sub_model_pv2.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_forms_from_non_typing_sequences.py` & `fastapi_slim-0.111.0.dev1/tests/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_generate_unique_id_function.py` & `fastapi_slim-0.111.0.dev1/tests/test_generate_unique_id_function.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_generic_parameterless_depends.py` & `fastapi_slim-0.111.0.dev1/tests/test_generic_parameterless_depends.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_get_request_body.py` & `fastapi_slim-0.111.0.dev1/tests/test_get_request_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_http_connection_injection.py` & `fastapi_slim-0.111.0.dev1/tests/test_http_connection_injection.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_include_router_defaults_overrides.py` & `fastapi_slim-0.111.0.dev1/tests/test_include_router_defaults_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_infer_param_optionality.py` & `fastapi_slim-0.111.0.dev1/tests/test_infer_param_optionality.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_inherited_custom_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_inherited_custom_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_invalid_path_param.py` & `fastapi_slim-0.111.0.dev1/tests/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_invalid_sequence_param.py` & `fastapi_slim-0.111.0.dev1/tests/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_jsonable_encoder.py` & `fastapi_slim-0.111.0.dev1/tests/test_jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_local_docs.py` & `fastapi_slim-0.111.0.dev1/tests/test_local_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_modules_same_name_body/test_main.py` & `fastapi_slim-0.111.0.dev1/tests/test_modules_same_name_body/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_multi_body_errors.py` & `fastapi_slim-0.111.0.dev1/tests/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_multi_query_errors.py` & `fastapi_slim-0.111.0.dev1/tests/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_multipart_installation.py` & `fastapi_slim-0.111.0.dev1/tests/test_multipart_installation.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_no_swagger_ui_redirect.py` & `fastapi_slim-0.111.0.dev1/tests/test_no_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_openapi_examples.py` & `fastapi_slim-0.111.0.dev1/tests/test_openapi_examples.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_openapi_query_parameter_extension.py` & `fastapi_slim-0.111.0.dev1/tests/test_openapi_query_parameter_extension.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_openapi_route_extensions.py` & `fastapi_slim-0.111.0.dev1/tests/test_openapi_route_extensions.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_openapi_separate_input_output_schemas.py` & `fastapi_slim-0.111.0.dev1/tests/test_openapi_separate_input_output_schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_openapi_servers.py` & `fastapi_slim-0.111.0.dev1/tests/test_openapi_servers.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_operations_signatures.py` & `fastapi_slim-0.111.0.dev1/tests/test_operations_signatures.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_orjson_response_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_orjson_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_param_class.py` & `fastapi_slim-0.111.0.dev1/tests/test_param_class.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_param_in_path_and_dependency.py` & `fastapi_slim-0.111.0.dev1/tests/test_param_in_path_and_dependency.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_param_include_in_schema.py` & `fastapi_slim-0.111.0.dev1/tests/test_param_include_in_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_params_repr.py` & `fastapi_slim-0.111.0.dev1/tests/test_params_repr.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_path.py` & `fastapi_slim-0.111.0.dev1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_put_no_body.py` & `fastapi_slim-0.111.0.dev1/tests/test_put_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_query.py` & `fastapi_slim-0.111.0.dev1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_read_with_orm_mode.py` & `fastapi_slim-0.111.0.dev1/tests/test_read_with_orm_mode.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_regex_deprecated_body.py` & `fastapi_slim-0.111.0.dev1/tests/test_regex_deprecated_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_regex_deprecated_params.py` & `fastapi_slim-0.111.0.dev1/tests/test_regex_deprecated_params.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_repeated_cookie_headers.py` & `fastapi_slim-0.111.0.dev1/tests/test_repeated_cookie_headers.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_repeated_dependency_schema.py` & `fastapi_slim-0.111.0.dev1/tests/test_repeated_dependency_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_repeated_parameter_alias.py` & `fastapi_slim-0.111.0.dev1/tests/test_repeated_parameter_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_reponse_set_reponse_code_empty.py` & `fastapi_slim-0.111.0.dev1/tests/test_reponse_set_reponse_code_empty.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_request_body_parameters_media_type.py` & `fastapi_slim-0.111.0.dev1/tests/test_request_body_parameters_media_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_required_noneable.py` & `fastapi_slim-0.111.0.dev1/tests/test_required_noneable.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_by_alias.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_by_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_change_status_code.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_change_status_code.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_class_no_mediatype.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_class_no_mediatype.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_code_no_body.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_code_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_model_as_return_annotation.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_model_as_return_annotation.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_model_data_filter.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_model_data_filter.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_model_data_filter_no_inheritance.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_model_data_filter_no_inheritance.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_model_include_exclude.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_model_include_exclude.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_model_invalid.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_model_invalid.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_response_model_sub_types.py` & `fastapi_slim-0.111.0.dev1/tests/test_response_model_sub_types.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_route_scope.py` & `fastapi_slim-0.111.0.dev1/tests/test_route_scope.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_router_events.py` & `fastapi_slim-0.111.0.dev1/tests/test_router_events.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_router_redirect_slashes.py` & `fastapi_slim-0.111.0.dev1/tests/test_router_redirect_slashes.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_schema_extra_examples.py` & `fastapi_slim-0.111.0.dev1/tests/test_schema_extra_examples.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_cookie.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_cookie_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_cookie_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_header.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_header.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_header_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_header_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_query.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_query.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_query_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_api_key_query_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_base.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_base_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_base_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_base_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_basic_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_basic_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_basic_realm.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_basic_realm_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_bearer.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_bearer_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_bearer_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_digest.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_digest.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_digest_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_http_digest_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2_authorization_code_bearer.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2_authorization_code_bearer_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2_optional_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2_password_bearer_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_oauth2_password_bearer_optional_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_openid_connect.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_openid_connect.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_openid_connect_description.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_security_openid_connect_optional.py` & `fastapi_slim-0.111.0.dev1/tests/test_security_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_serialize_response.py` & `fastapi_slim-0.111.0.dev1/tests/test_serialize_response.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_serialize_response_dataclass.py` & `fastapi_slim-0.111.0.dev1/tests/test_serialize_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_serialize_response_model.py` & `fastapi_slim-0.111.0.dev1/tests/test_serialize_response_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_skip_defaults.py` & `fastapi_slim-0.111.0.dev1/tests/test_skip_defaults.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_starlette_exception.py` & `fastapi_slim-0.111.0.dev1/tests/test_starlette_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_starlette_urlconvertors.py` & `fastapi_slim-0.111.0.dev1/tests/test_starlette_urlconvertors.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_sub_callbacks.py` & `fastapi_slim-0.111.0.dev1/tests/test_sub_callbacks.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_swagger_ui_init_oauth.py` & `fastapi_slim-0.111.0.dev1/tests/test_swagger_ui_init_oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tuples.py` & `fastapi_slim-0.111.0.dev1/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_responses/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/test_main.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/test_main_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_configure_swagger_ui/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_cors/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_cors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_docs_ui/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial001b.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006b.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_custom_response/test_tutorial006c.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dataclasses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008b.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008b_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008c.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008c_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008d.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial008d_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial012.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_events/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_events/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_events/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_events/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_generate_clients/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_handling_errors/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/test_tutorial001_1.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_metadata/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_metadata/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_params/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_path_params/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_path_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_02.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_03.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial001_py310_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_schema_extra_example/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial003_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial005_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial006.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial006_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_separate_openapi_schemas/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_settings/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_settings/test_tutorial001_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_settings/test_tutorial001_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_sub_applications/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_templates/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_templates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_main.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial001.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial003.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py` & `fastapi_slim-0.111.0.dev1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_typing_python39.py` & `fastapi_slim-0.111.0.dev1/tests/test_typing_python39.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_union_body.py` & `fastapi_slim-0.111.0.dev1/tests/test_union_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_union_inherited_body.py` & `fastapi_slim-0.111.0.dev1/tests/test_union_inherited_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_validate_response.py` & `fastapi_slim-0.111.0.dev1/tests/test_validate_response.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_validate_response_dataclass.py` & `fastapi_slim-0.111.0.dev1/tests/test_validate_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_validate_response_recursive/app_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/app_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_validate_response_recursive/app_pv2.py` & `fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/app_pv2.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py` & `fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv1.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py` & `fastapi_slim-0.111.0.dev1/tests/test_validate_response_recursive/test_validate_response_recursive_pv2.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_webhooks_security.py` & `fastapi_slim-0.111.0.dev1/tests/test_webhooks_security.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_ws_dependencies.py` & `fastapi_slim-0.111.0.dev1/tests/test_ws_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/tests/test_ws_router.py` & `fastapi_slim-0.111.0.dev1/tests/test_ws_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_slim-0.111.0/PKG-INFO` & `fastapi_slim-0.111.0.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-slim
-Version: 0.111.0
+Version: 0.111.0.dev1
 Summary: FastAPI framework, high performance, easy to learn, fast to code, ready for production
 Author-Email: =?utf-8?q?Sebasti=C3=A1n_Ram=C3=ADrez?= <tiangolo@gmail.com>
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -33,23 +33,21 @@
 Project-URL: Homepage, https://github.com/tiangolo/fastapi
 Project-URL: Documentation, https://fastapi.tiangolo.com/
 Project-URL: Repository, https://github.com/tiangolo/fastapi
 Requires-Python: >=3.8
 Requires-Dist: starlette<0.38.0,>=0.37.2
 Requires-Dist: pydantic!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0,>=1.7.4
 Requires-Dist: typing-extensions>=4.8.0
-Requires-Dist: fastapi-cli>=0.0.2; extra == "standard"
 Requires-Dist: httpx>=0.23.0; extra == "standard"
 Requires-Dist: jinja2>=2.11.2; extra == "standard"
 Requires-Dist: python-multipart>=0.0.7; extra == "standard"
 Requires-Dist: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1; extra == "standard"
 Requires-Dist: orjson>=3.2.1; extra == "standard"
 Requires-Dist: email_validator>=2.0.0; extra == "standard"
 Requires-Dist: uvicorn[standard]>=0.12.0; extra == "standard"
-Requires-Dist: fastapi-cli>=0.0.2; extra == "all"
 Requires-Dist: httpx>=0.23.0; extra == "all"
 Requires-Dist: jinja2>=2.11.2; extra == "all"
 Requires-Dist: python-multipart>=0.0.7; extra == "all"
 Requires-Dist: itsdangerous>=1.1.0; extra == "all"
 Requires-Dist: pyyaml>=5.3.1; extra == "all"
 Requires-Dist: ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1; extra == "all"
 Requires-Dist: orjson>=3.2.1; extra == "all"
@@ -198,14 +196,26 @@
 $ pip install fastapi
 
 ---> 100%
 ```
 
 </div>
 
+You will also need an ASGI server, for production such as <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a> or <a href="https://github.com/pgjones/hypercorn" class="external-link" target="_blank">Hypercorn</a>.
+
+<div class="termy">
+
+```console
+$ pip install "uvicorn[standard]"
+
+---> 100%
+```
+
+</div>
+
 ## Example
 
 ### Create it
 
 * Create a file `main.py` with:
 
 ```Python
@@ -258,46 +268,33 @@
 ### Run it
 
 Run the server with:
 
 <div class="termy">
 
 ```console
-$ fastapi dev main.py
-
- ╭────────── FastAPI CLI - Development mode ───────────╮
- │                                                     │
- │  Serving at: http://127.0.0.1:8000                  │
- │                                                     │
- │  API docs: http://127.0.0.1:8000/docs               │
- │                                                     │
- │  Running in development mode, for production use:   │
- │                                                     │
- │  fastapi run                                        │
- │                                                     │
- ╰─────────────────────────────────────────────────────╯
+$ uvicorn main:app --reload
 
-INFO:     Will watch for changes in these directories: ['/home/user/code/awesomeapp']
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-INFO:     Started reloader process [2248755] using WatchFiles
-INFO:     Started server process [2248757]
+INFO:     Started reloader process [28720]
+INFO:     Started server process [28722]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 ```
 
 </div>
 
 <details markdown="1">
-<summary>About the command <code>fastapi dev main.py</code>...</summary>
+<summary>About the command <code>uvicorn main:app --reload</code>...</summary>
 
-The command `fastapi dev` reads your `main.py` file, detects the **FastAPI** app in it, and starts a server using <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a>.
+The command `uvicorn main:app` refers to:
 
-By default, `fastapi dev` will start with auto-reload enabled for local development.
-
-You can read more about it in the <a href="https://fastapi.tiangolo.com/fastapi-cli/" target="_blank">FastAPI CLI docs</a>.
+* `main`: the file `main.py` (the Python "module").
+* `app`: the object created inside of `main.py` with the line `app = FastAPI()`.
+* `--reload`: make the server restart after code changes. Only do this for development.
 
 </details>
 
 ### Check it
 
 Open your browser at <a href="http://127.0.0.1:8000/items/5?q=somequery" class="external-link" target="_blank">http://127.0.0.1:8000/items/5?q=somequery</a>.
 
@@ -362,15 +359,15 @@
 
 
 @app.put("/items/{item_id}")
 def update_item(item_id: int, item: Item):
     return {"item_name": item.name, "item_id": item_id}
 ```
 
-The `fastapi dev` server should reload automatically.
+The server should reload automatically (because you added `--reload` to the `uvicorn` command above).
 
 ### Interactive API docs upgrade
 
 Now go to <a href="http://127.0.0.1:8000/docs" class="external-link" target="_blank">http://127.0.0.1:8000/docs</a>.
 
 * The interactive API documentation will be automatically updated, including the new body:
 
@@ -506,51 +503,34 @@
 
 ## Performance
 
 Independent TechEmpower benchmarks show **FastAPI** applications running under Uvicorn as <a href="https://www.techempower.com/benchmarks/#section=test&runid=7464e520-0dc2-473d-bd34-dbdfd7e85911&hw=ph&test=query&l=zijzen-7" class="external-link" target="_blank">one of the fastest Python frameworks available</a>, only below Starlette and Uvicorn themselves (used internally by FastAPI). (*)
 
 To understand more about it, see the section <a href="https://fastapi.tiangolo.com/benchmarks/" class="internal-link" target="_blank">Benchmarks</a>.
 
-## Dependencies
+## Optional Dependencies
 
 Used by Pydantic:
 
 * <a href="https://github.com/JoshData/python-email-validator" target="_blank"><code>email_validator</code></a> - for email validation.
 * <a href="https://docs.pydantic.dev/latest/usage/pydantic_settings/" target="_blank"><code>pydantic-settings</code></a> - for settings management.
 * <a href="https://docs.pydantic.dev/latest/usage/types/extra_types/extra_types/" target="_blank"><code>pydantic-extra-types</code></a> - for extra types to be used with Pydantic.
 
 Used by Starlette:
 
 * <a href="https://www.python-httpx.org" target="_blank"><code>httpx</code></a> - Required if you want to use the `TestClient`.
 * <a href="https://jinja.palletsprojects.com" target="_blank"><code>jinja2</code></a> - Required if you want to use the default template configuration.
 * <a href="https://github.com/Kludex/python-multipart" target="_blank"><code>python-multipart</code></a> - Required if you want to support form <abbr title="converting the string that comes from an HTTP request into Python data">"parsing"</abbr>, with `request.form()`.
+* <a href="https://pythonhosted.org/itsdangerous/" target="_blank"><code>itsdangerous</code></a> - Required for `SessionMiddleware` support.
+* <a href="https://pyyaml.org/wiki/PyYAMLDocumentation" target="_blank"><code>pyyaml</code></a> - Required for Starlette's `SchemaGenerator` support (you probably don't need it with FastAPI).
 
 Used by FastAPI / Starlette:
 
 * <a href="https://www.uvicorn.org" target="_blank"><code>uvicorn</code></a> - for the server that loads and serves your application.
 * <a href="https://github.com/ijl/orjson" target="_blank"><code>orjson</code></a> - Required if you want to use `ORJSONResponse`.
 * <a href="https://github.com/esnme/ultrajson" target="_blank"><code>ujson</code></a> - Required if you want to use `UJSONResponse`.
-* `fastapi-cli` - to provide the `fastapi` command.
-
-When you install `fastapi` it comes these standard dependencies.
-
-## `fastapi-slim`
-
-If you don't want the extra standard optional dependencies, install `fastapi-slim` instead.
-
-When you install with:
-
-```bash
-pip install fastapi
-```
-
-...it includes the same code and dependencies as:
-
-```bash
-pip install "fastapi-slim[standard]"
-```
 
-The standard extra dependencies are the ones mentioned above.
+You can install all of these with `pip install "fastapi[all]"`.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-slim Version: 0.111.0 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-slim Version: 0.111.0.dev1 Summary: FastAPI
 framework, high performance, easy to learn, fast to code, ready for production
 Author-Email: =?utf-8?q?Sebasti=C3=A1n_Ram=C3=ADrez?=
 gmail.com> Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Internet Classifier: Topic
 :: Software Development :: Libraries :: Application Frameworks Classifier:
@@ -19,26 +19,24 @@
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Internet :: WWW/HTTP
 Project-URL: Homepage, https://github.com/tiangolo/fastapi Project-URL:
 Documentation, https://fastapi.tiangolo.com/ Project-URL: Repository, https://
 github.com/tiangolo/fastapi Requires-Python: >=3.8 Requires-Dist:
 starlette<0.38.0,>=0.37.2 Requires-Dist:
 pydantic!=1.8,!=1.8.1,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0,>=1.7.4 Requires-Dist:
-typing-extensions>=4.8.0 Requires-Dist: fastapi-cli>=0.0.2; extra == "standard"
-Requires-Dist: httpx>=0.23.0; extra == "standard" Requires-Dist:
-jinja2>=2.11.2; extra == "standard" Requires-Dist: python-multipart>=0.0.7;
-extra == "standard" Requires-Dist:
+typing-extensions>=4.8.0 Requires-Dist: httpx>=0.23.0; extra == "standard"
+Requires-Dist: jinja2>=2.11.2; extra == "standard" Requires-Dist: python-
+multipart>=0.0.7; extra == "standard" Requires-Dist:
 ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1; extra ==
 "standard" Requires-Dist: orjson>=3.2.1; extra == "standard" Requires-Dist:
 email_validator>=2.0.0; extra == "standard" Requires-Dist: uvicorn
-[standard]>=0.12.0; extra == "standard" Requires-Dist: fastapi-cli>=0.0.2;
-extra == "all" Requires-Dist: httpx>=0.23.0; extra == "all" Requires-Dist:
-jinja2>=2.11.2; extra == "all" Requires-Dist: python-multipart>=0.0.7; extra ==
-"all" Requires-Dist: itsdangerous>=1.1.0; extra == "all" Requires-Dist:
-pyyaml>=5.3.1; extra == "all" Requires-Dist:
+[standard]>=0.12.0; extra == "standard" Requires-Dist: httpx>=0.23.0; extra ==
+"all" Requires-Dist: jinja2>=2.11.2; extra == "all" Requires-Dist: python-
+multipart>=0.0.7; extra == "all" Requires-Dist: itsdangerous>=1.1.0; extra ==
+"all" Requires-Dist: pyyaml>=5.3.1; extra == "all" Requires-Dist:
 ujson!=4.0.2,!=4.1.0,!=4.2.0,!=4.3.0,!=5.0.0,!=5.1.0,>=4.0.1; extra == "all"
 Requires-Dist: orjson>=3.2.1; extra == "all" Requires-Dist:
 email_validator>=2.0.0; extra == "all" Requires-Dist: uvicorn
 [standard]>=0.12.0; extra == "all" Requires-Dist: pydantic-settings>=2.0.0;
 extra == "all" Requires-Dist: pydantic-extra-types>=2.0.0; extra == "all"
 Provides-Extra: standard Provides-Extra: all Description-Content-Type: text/
 markdown
@@ -106,63 +104,59 @@
 --- ## **Typer**, the FastAPI of CLIs _[_h_t_t_p_s_:_/_/_t_y_p_e_r_._t_i_a_n_g_o_l_o_._c_o_m_/_i_m_g_/_l_o_g_o_-
 _m_a_r_g_i_n_/_l_o_g_o_-_m_a_r_g_i_n_-_v_e_c_t_o_r_._s_v_g_]If you are building a CLI app to be used in the
 terminal instead of a web API, check out _*_*_T_y_p_e_r_*_*. **Typer** is FastAPI's
 little sibling. And it's intended to be the **FastAPI of CLIs**. â¨ï¸ ð ##
 Requirements FastAPI stands on the shoulders of giants: * _S_t_a_r_l_e_t_t_e for the web
 parts. * _P_y_d_a_n_t_i_c for the data parts. ## Installation
 ```console $ pip install fastapi ---> 100% ```
+You will also need an ASGI server, for production such as _U_v_i_c_o_r_n or _H_y_p_e_r_c_o_r_n.
+```console $ pip install "uvicorn[standard]" ---> 100% ```
 ## Example ### Create it * Create a file `main.py` with: ```Python from typing
 import Union from fastapi import FastAPI app = FastAPI() @app.get("/") def
 read_root(): return {"Hello": "World"} @app.get("/items/{item_id}") def
 read_item(item_id: int, q: Union[str, None] = None): return {"item_id":
 item_id, "q": q} ``` Or use async def... If your code uses `async` / `await`,
 use `async def`: ```Python hl_lines="9 14" from typing import Union from
 fastapi import FastAPI app = FastAPI() @app.get("/") async def read_root():
 return {"Hello": "World"} @app.get("/items/{item_id}") async def read_item
 (item_id: int, q: Union[str, None] = None): return {"item_id": item_id, "q": q}
 ``` **Note**: If you don't know, check the _"In a hurry?"_ section about
 _`_a_s_y_n_c_`_ _a_n_d_ _`_a_w_a_i_t_`_ _i_n_ _t_h_e_ _d_o_c_s. ### Run it Run the server with:
-```console $ fastapi dev main.py â­ââââââââââ FastAPI CLI
-- Development mode ââââââââââââ® â â â Serving at:
-http://127.0.0.1:8000 â â â â API docs: http://127.0.0.1:8000/docs â
-â â â Running in development mode, for production use: â â â â
-fastapi run â â â
-â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
-INFO: Will watch for changes in these directories: ['/home/user/code/
-awesomeapp'] INFO: Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to
-quit) INFO: Started reloader process [2248755] using WatchFiles INFO: Started
-server process [2248757] INFO: Waiting for application startup. INFO:
-Application startup complete. ```
-About the command fastapi dev main.py... The command `fastapi dev` reads your
-`main.py` file, detects the **FastAPI** app in it, and starts a server using
-_U_v_i_c_o_r_n. By default, `fastapi dev` will start with auto-reload enabled for
-local development. You can read more about it in the _F_a_s_t_A_P_I_ _C_L_I_ _d_o_c_s. ###
-Check it Open your browser at _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_i_t_e_m_s_/_5_?_q_=_s_o_m_e_q_u_e_r_y. You
-will see the JSON response as: ```JSON {"item_id": 5, "q": "somequery"} ``` You
-already created an API that: * Receives HTTP requests in the _paths_ `/` and `/
-items/{item_id}`. * Both _paths_ take `GET` ooppeerraattiioonnss (also known as HTTP
-_methods_). * The _path_ `/items/{item_id}` has a _path parameter_ `item_id`
-that should be an `int`. * The _path_ `/items/{item_id}` has an optional `str`
-_query parameter_ `q`. ### Interactive API docs Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:
-_8_0_0_0_/_d_o_c_s. You will see the automatic interactive API documentation (provided
-by _S_w_a_g_g_e_r_ _U_I): ![Swagger UI](https://fastapi.tiangolo.com/img/index/index-01-
-swagger-ui-simple.png) ### Alternative API docs And now, go to _h_t_t_p_:_/_/
-_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. You will see the alternative automatic documentation
-(provided by _R_e_D_o_c): ![ReDoc](https://fastapi.tiangolo.com/img/index/index-02-
-redoc-simple.png) ## Example upgrade Now modify the file `main.py` to receive a
-body from a `PUT` request. Declare the body using standard Python types, thanks
-to Pydantic. ```Python hl_lines="4 9-12 25-27" from typing import Union from
-fastapi import FastAPI from pydantic import BaseModel app = FastAPI() class
-Item(BaseModel): name: str price: float is_offer: Union[bool, None] = None
-@app.get("/") def read_root(): return {"Hello": "World"} @app.get("/items/
-{item_id}") def read_item(item_id: int, q: Union[str, None] = None): return
-{"item_id": item_id, "q": q} @app.put("/items/{item_id}") def update_item
-(item_id: int, item: Item): return {"item_name": item.name, "item_id": item_id}
-``` The `fastapi dev` server should reload automatically. ### Interactive API
-docs upgrade Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. * The interactive API
+```console $ uvicorn main:app --reload INFO: Uvicorn running on http://
+127.0.0.1:8000 (Press CTRL+C to quit) INFO: Started reloader process [28720]
+INFO: Started server process [28722] INFO: Waiting for application startup.
+INFO: Application startup complete. ```
+About the command uvicorn main:app --reload... The command `uvicorn main:app`
+refers to: * `main`: the file `main.py` (the Python "module"). * `app`: the
+object created inside of `main.py` with the line `app = FastAPI()`. * `--
+reload`: make the server restart after code changes. Only do this for
+development. ### Check it Open your browser at _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_i_t_e_m_s_/
+_5_?_q_=_s_o_m_e_q_u_e_r_y. You will see the JSON response as: ```JSON {"item_id": 5, "q":
+"somequery"} ``` You already created an API that: * Receives HTTP requests in
+the _paths_ `/` and `/items/{item_id}`. * Both _paths_ take `GET` ooppeerraattiioonnss
+(also known as HTTP _methods_). * The _path_ `/items/{item_id}` has a _path
+parameter_ `item_id` that should be an `int`. * The _path_ `/items/{item_id}`
+has an optional `str` _query parameter_ `q`. ### Interactive API docs Now go to
+_h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. You will see the automatic interactive API
+documentation (provided by _S_w_a_g_g_e_r_ _U_I): ![Swagger UI](https://
+fastapi.tiangolo.com/img/index/index-01-swagger-ui-simple.png) ### Alternative
+API docs And now, go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_r_e_d_o_c. You will see the
+alternative automatic documentation (provided by _R_e_D_o_c): ![ReDoc](https://
+fastapi.tiangolo.com/img/index/index-02-redoc-simple.png) ## Example upgrade
+Now modify the file `main.py` to receive a body from a `PUT` request. Declare
+the body using standard Python types, thanks to Pydantic. ```Python hl_lines="4
+9-12 25-27" from typing import Union from fastapi import FastAPI from pydantic
+import BaseModel app = FastAPI() class Item(BaseModel): name: str price: float
+is_offer: Union[bool, None] = None @app.get("/") def read_root(): return
+{"Hello": "World"} @app.get("/items/{item_id}") def read_item(item_id: int, q:
+Union[str, None] = None): return {"item_id": item_id, "q": q} @app.put("/items/
+{item_id}") def update_item(item_id: int, item: Item): return {"item_name":
+item.name, "item_id": item_id} ``` The server should reload automatically
+(because you added `--reload` to the `uvicorn` command above). ### Interactive
+API docs upgrade Now go to _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_/_d_o_c_s. * The interactive API
 documentation will be automatically updated, including the new body: ![Swagger
 UI](https://fastapi.tiangolo.com/img/index/index-03-swagger-02.png) * Click on
 the button "Try it out", it allows you to fill the parameters and directly
 interact with the API: ![Swagger UI interaction](https://fastapi.tiangolo.com/
 img/index/index-04-swagger-03.png) * Then click on the "Execute" button, the
 user interface will communicate with your API, send the parameters, get the
 results and show them on the screen: ![Swagger UI interaction](https://
@@ -217,22 +211,20 @@
 Pydantic). * **GraphQL** integration with _S_t_r_a_w_b_e_r_r_y and other libraries. *
 Many extra features (thanks to Starlette) as: * **WebSockets** * extremely easy
 tests based on HTTPX and `pytest` * **CORS** * **Cookie Sessions** * ...and
 more. ## Performance Independent TechEmpower benchmarks show **FastAPI**
 applications running under Uvicorn as _o_n_e_ _o_f_ _t_h_e_ _f_a_s_t_e_s_t_ _P_y_t_h_o_n_ _f_r_a_m_e_w_o_r_k_s
 _a_v_a_i_l_a_b_l_e, only below Starlette and Uvicorn themselves (used internally by
 FastAPI). (*) To understand more about it, see the section _B_e_n_c_h_m_a_r_k_s. ##
-Dependencies Used by Pydantic: * _e_m_a_i_l___v_a_l_i_d_a_t_o_r - for email validation. *
-_p_y_d_a_n_t_i_c_-_s_e_t_t_i_n_g_s - for settings management. * _p_y_d_a_n_t_i_c_-_e_x_t_r_a_-_t_y_p_e_s - for extra
-types to be used with Pydantic. Used by Starlette: * _h_t_t_p_x - Required if you
-want to use the `TestClient`. * _j_i_n_j_a_2 - Required if you want to use the
-default template configuration. * _p_y_t_h_o_n_-_m_u_l_t_i_p_a_r_t - Required if you want to
-support form "parsing", with `request.form()`. Used by FastAPI / Starlette: *
-_u_v_i_c_o_r_n - for the server that loads and serves your application. * _o_r_j_s_o_n -
-Required if you want to use `ORJSONResponse`. * _u_j_s_o_n - Required if you want to
-use `UJSONResponse`. * `fastapi-cli` - to provide the `fastapi` command. When
-you install `fastapi` it comes these standard dependencies. ## `fastapi-slim`
-If you don't want the extra standard optional dependencies, install `fastapi-
-slim` instead. When you install with: ```bash pip install fastapi ``` ...it
-includes the same code and dependencies as: ```bash pip install "fastapi-slim
-[standard]" ``` The standard extra dependencies are the ones mentioned above.
-## License This project is licensed under the terms of the MIT license.
+Optional Dependencies Used by Pydantic: * _e_m_a_i_l___v_a_l_i_d_a_t_o_r - for email
+validation. * _p_y_d_a_n_t_i_c_-_s_e_t_t_i_n_g_s - for settings management. * _p_y_d_a_n_t_i_c_-_e_x_t_r_a_-
+_t_y_p_e_s - for extra types to be used with Pydantic. Used by Starlette: * _h_t_t_p_x -
+Required if you want to use the `TestClient`. * _j_i_n_j_a_2 - Required if you want
+to use the default template configuration. * _p_y_t_h_o_n_-_m_u_l_t_i_p_a_r_t - Required if you
+want to support form "parsing", with `request.form()`. * _i_t_s_d_a_n_g_e_r_o_u_s -
+Required for `SessionMiddleware` support. * _p_y_y_a_m_l - Required for Starlette's
+`SchemaGenerator` support (you probably don't need it with FastAPI). Used by
+FastAPI / Starlette: * _u_v_i_c_o_r_n - for the server that loads and serves your
+application. * _o_r_j_s_o_n - Required if you want to use `ORJSONResponse`. * _u_j_s_o_n -
+Required if you want to use `UJSONResponse`. You can install all of these with
+`pip install "fastapi[all]"`. ## License This project is licensed under the
+terms of the MIT license.
```

