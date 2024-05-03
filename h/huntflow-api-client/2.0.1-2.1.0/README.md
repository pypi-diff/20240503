# Comparing `tmp/huntflow_api_client-2.0.1.tar.gz` & `tmp/huntflow_api_client-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_api_client-2.0.1.tar", last modified: Tue Jan  9 07:25:06 2024, max compression
+gzip compressed data, was "huntflow_api_client-2.1.0.tar", last modified: Fri May  3 07:48:37 2024, max compression
```

## Comparing `huntflow_api_client-2.0.1.tar` & `huntflow_api_client-2.1.0.tar`

### file list

```diff
@@ -1,139 +1,144 @@
--rw-r--r--   0        0        0     1065 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/LICENSE
--rw-r--r--   0        0        0      488 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/README.md
--rw-r--r--   0        0        0       76 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/__init__.py
--rw-r--r--   0        0        0     5735 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/api.py
--rw-r--r--   0        0        0     2692 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/__init__.py
--rw-r--r--   0        0        0     1251 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/account_offers.py
--rw-r--r--   0        0        0     1770 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/account_vacancy_request.py
--rw-r--r--   0        0        0     1449 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/accounts.py
--rw-r--r--   0        0        0     1631 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/action_logs.py
--rw-r--r--   0        0        0     2595 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_logs.py
--rw-r--r--   0        0        0     2859 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_offers.py
--rw-r--r--   0        0        0     2958 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_on_vacancy.py
--rw-r--r--   0        0        0      735 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0     6966 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/applicants.py
--rw-r--r--   0        0        0      941 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/base.py
--rw-r--r--   0        0        0     2733 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/coworkers.py
--rw-r--r--   0        0        0      748 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/delayed_tasks.py
--rw-r--r--   0        0        0     3022 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/dictionaries.py
--rw-r--r--   0        0        0     2564 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/divisions.py
--rw-r--r--   0        0        0      888 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/email_templates.py
--rw-r--r--   0        0        0     1140 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/file.py
--rw-r--r--   0        0        0     2145 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/multi_vacancies.py
--rw-r--r--   0        0        0     1955 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/organization_settings.py
--rw-r--r--   0        0        0     6797 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/production_calendars.py
--rw-r--r--   0        0        0     2995 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/questionary.py
--rw-r--r--   0        0        0      623 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/regions.py
--rw-r--r--   0        0        0      718 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/rejection_reason.py
--rw-r--r--   0        0        0     3772 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/resume.py
--rw-r--r--   0        0        0     4331 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/survey_type_q.py
--rw-r--r--   0        0        0     4558 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/tags.py
--rw-r--r--   0        0        0      993 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/user_settings.py
--rw-r--r--   0        0        0      690 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/users.py
--rw-r--r--   0        0        0     5763 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/users_management.py
--rw-r--r--   0        0        0    11740 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/vacancies.py
--rw-r--r--   0        0        0     2933 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/vacancy_requests.py
--rw-r--r--   0        0        0     1815 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/entities/webhooks.py
--rw-r--r--   0        0        0      553 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/errors/__init__.py
--rw-r--r--   0        0        0     1128 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/errors/errors.py
--rw-r--r--   0        0        0     3732 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/errors/handlers.py
--rw-r--r--   0        0        0      361 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/errors/response_hooks.py
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/__init__.py
--rw-r--r--   0        0        0     9669 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/common.py
--rw-r--r--   0        0        0     3435 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/consts.py
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/__init__.py
--rw-r--r--   0        0        0     2640 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicant_logs.py
--rw-r--r--   0        0        0      326 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicant_offers.py
--rw-r--r--   0        0        0     3618 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicant_on_vacancy.py
--rw-r--r--   0        0        0     2980 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicants.py
--rw-r--r--   0        0        0     1492 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/dictionaries.py
--rw-r--r--   0        0        0      691 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/divisions.py
--rw-r--r--   0        0        0      957 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/file.py
--rw-r--r--   0        0        0     4553 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/multi_vacancies.py
--rw-r--r--   0        0        0      920 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/production_calendars.py
--rw-r--r--   0        0        0      670 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/resume.py
--rw-r--r--   0        0        0      279 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/survey.py
--rw-r--r--   0        0        0      436 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/tags.py
--rw-r--r--   0        0        0      108 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/users_management.py
--rw-r--r--   0        0        0     3711 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/vacancies.py
--rw-r--r--   0        0        0     1393 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/vacancy_requests.py
--rw-r--r--   0        0        0      482 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/request/webhooks.py
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/__init__.py
--rw-r--r--   0        0        0      602 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/account_offers.py
--rw-r--r--   0        0        0     1909 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/account_vacancy_request.py
--rw-r--r--   0        0        0     1595 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/accounts.py
--rw-r--r--   0        0        0     1187 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/action_logs.py
--rw-r--r--   0        0        0     8554 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_logs.py
--rw-r--r--   0        0        0      622 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_offers.py
--rw-r--r--   0        0        0     1044 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_on_vacancy.py
--rw-r--r--   0        0        0      773 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0     5657 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicants.py
--rw-r--r--   0        0        0     1306 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/coworkers.py
--rw-r--r--   0        0        0     1381 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/delayed_tasks.py
--rw-r--r--   0        0        0     2261 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/dictionaries.py
--rw-r--r--   0        0        0     1507 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/divisions.py
--rw-r--r--   0        0        0     1262 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/email_templates.py
--rw-r--r--   0        0        0     2022 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/file.py
--rw-r--r--   0        0        0      156 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/muilti_vacancies.py
--rw-r--r--   0        0        0     1297 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/organization_settings.py
--rw-r--r--   0        0        0     1525 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/production_calendars.py
--rw-r--r--   0        0        0     1365 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/questionary.py
--rw-r--r--   0        0        0      718 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/regions.py
--rw-r--r--   0        0        0      476 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/rejection_reason.py
--rw-r--r--   0        0        0    13292 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/resume.py
--rw-r--r--   0        0        0     2616 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/survey.py
--rw-r--r--   0        0        0      490 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/tags.py
--rw-r--r--   0        0        0     1509 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/user_settings.py
--rw-r--r--   0        0        0      795 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/users.py
--rw-r--r--   0        0        0     1494 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/users_management.py
--rw-r--r--   0        0        0     6357 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/vacancies.py
--rw-r--r--   0        0        0     2865 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/vacancy_requests.py
--rw-r--r--   0        0        0      719 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/models/response/webhooks.py
--rw-r--r--   0        0        0       53 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/tokens/__init__.py
--rw-r--r--   0        0        0     1871 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/tokens/locker.py
--rw-r--r--   0        0        0     5186 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/tokens/proxy.py
--rw-r--r--   0        0        0      730 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/tokens/storage.py
--rw-r--r--   0        0        0      548 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/huntflow_api_client/tokens/token.py
--rw-r--r--   0        0        0     1646 2024-01-09 07:25:06.759557 huntflow_api_client-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4829 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/api.py
--rw-r--r--   0        0        0       79 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0      176 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/fixtures/server.py
--rw-r--r--   0        0        0      924 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/fixtures/tokens.py
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/__init__.py
--rw-r--r--   0        0        0     3225 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_account_divisions.py
--rw-r--r--   0        0        0     5097 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_account_offers.py
--rw-r--r--   0        0        0     3886 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_account_vacancy_request.py
--rw-r--r--   0        0        0     2329 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_accounts.py
--rw-r--r--   0        0        0     1385 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_action_logs.py
--rw-r--r--   0        0        0     7422 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_applicant_logs.py
--rw-r--r--   0        0        0     3089 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_applicant_offers.py
--rw-r--r--   0        0        0     3664 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_applicant_on_vacancy.py
--rw-r--r--   0        0        0     1244 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_applicant_on_vacancy_statuses.py
--rw-r--r--   0        0        0    11555 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_applicants.py
--rw-r--r--   0        0        0     2909 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_coworkers.py
--rw-r--r--   0        0        0     1358 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_delayed_tasks.py
--rw-r--r--   0        0        0     4497 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_dictionaries.py
--rw-r--r--   0        0        0     2012 2024-01-09 07:24:55.247546 huntflow_api_client-2.0.1/tests/test_entities/test_email_templates.py
--rw-r--r--   0        0        0     1778 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_file.py
--rw-r--r--   0        0        0     2925 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_multi_vacancies.py
--rw-r--r--   0        0        0     2508 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_organization_settings.py
--rw-r--r--   0        0        0     7896 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_production_calendar.py
--rw-r--r--   0        0        0     3445 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_questionary.py
--rw-r--r--   0        0        0     1015 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_regions.py
--rw-r--r--   0        0        0     1069 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_rejection_reasons.py
--rw-r--r--   0        0        0    15232 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_resume.py
--rw-r--r--   0        0        0     8613 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_survey_type_q.py
--rw-r--r--   0        0        0     4638 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_tags.py
--rw-r--r--   0        0        0     2237 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_user_settings.py
--rw-r--r--   0        0        0     1052 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_users.py
--rw-r--r--   0        0        0     6510 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_users_management.py
--rw-r--r--   0        0        0    16866 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_vacancies.py
--rw-r--r--   0        0        0     4406 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_vacancy_request.py
--rw-r--r--   0        0        0     2584 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_entities/test_webhooks.py
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_errors/__init__.py
--rw-r--r--   0        0        0     8107 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_errors/test_error_handlers.py
--rw-r--r--   0        0        0        0 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_tokens/__init__.py
--rw-r--r--   0        0        0     5556 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_tokens/test_access_token.py
--rw-r--r--   0        0        0     2008 2024-01-09 07:24:55.251546 huntflow_api_client-2.0.1/tests/test_tokens/test_huntflow_token_proxy.py
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 huntflow_api_client-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/LICENSE
+-rw-r--r--   0        0        0      488 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/README.md
+-rw-r--r--   0        0        0       76 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/__init__.py
+-rw-r--r--   0        0        0     5735 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/api.py
+-rw-r--r--   0        0        0     2880 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/account_offers.py
+-rw-r--r--   0        0        0     1770 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/account_vacancy_request.py
+-rw-r--r--   0        0        0     1449 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/accounts.py
+-rw-r--r--   0        0        0     1631 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/action_logs.py
+-rw-r--r--   0        0        0     2595 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_logs.py
+-rw-r--r--   0        0        0     2859 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_offers.py
+-rw-r--r--   0        0        0     2958 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      735 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     1238 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_reponse.py
+-rw-r--r--   0        0        0     6966 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicants.py
+-rw-r--r--   0        0        0      941 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/base.py
+-rw-r--r--   0        0        0     2733 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/coworkers.py
+-rw-r--r--   0        0        0      748 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/delayed_tasks.py
+-rw-r--r--   0        0        0     3022 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/dictionaries.py
+-rw-r--r--   0        0        0     2564 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/divisions.py
+-rw-r--r--   0        0        0      888 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/email_templates.py
+-rw-r--r--   0        0        0     1140 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/file.py
+-rw-r--r--   0        0        0     2145 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/multi_vacancies.py
+-rw-r--r--   0        0        0     1955 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/organization_settings.py
+-rw-r--r--   0        0        0     6797 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/production_calendars.py
+-rw-r--r--   0        0        0     2995 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/questionary.py
+-rw-r--r--   0        0        0      623 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/regions.py
+-rw-r--r--   0        0        0      718 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/rejection_reason.py
+-rw-r--r--   0        0        0     3772 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/resume.py
+-rw-r--r--   0        0        0     1575 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_a.py
+-rw-r--r--   0        0        0     4331 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_q.py
+-rw-r--r--   0        0        0     4558 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/tags.py
+-rw-r--r--   0        0        0      993 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/user_settings.py
+-rw-r--r--   0        0        0      690 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/users.py
+-rw-r--r--   0        0        0     5763 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/users_management.py
+-rw-r--r--   0        0        0    11740 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancies.py
+-rw-r--r--   0        0        0     2933 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancy_requests.py
+-rw-r--r--   0        0        0     1815 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/webhooks.py
+-rw-r--r--   0        0        0      553 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/__init__.py
+-rw-r--r--   0        0        0     1128 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/errors.py
+-rw-r--r--   0        0        0     3732 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/handlers.py
+-rw-r--r--   0        0        0      361 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/response_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/__init__.py
+-rw-r--r--   0        0        0     9669 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/common.py
+-rw-r--r--   0        0        0     3435 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/consts.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/__init__.py
+-rw-r--r--   0        0        0     2640 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_logs.py
+-rw-r--r--   0        0        0      326 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_offers.py
+-rw-r--r--   0        0        0     3618 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_on_vacancy.py
+-rw-r--r--   0        0        0     2980 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicants.py
+-rw-r--r--   0        0        0     1492 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/dictionaries.py
+-rw-r--r--   0        0        0      691 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/divisions.py
+-rw-r--r--   0        0        0      957 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/file.py
+-rw-r--r--   0        0        0     4553 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/multi_vacancies.py
+-rw-r--r--   0        0        0      920 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/production_calendars.py
+-rw-r--r--   0        0        0      670 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/resume.py
+-rw-r--r--   0        0        0      279 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/survey.py
+-rw-r--r--   0        0        0      436 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/tags.py
+-rw-r--r--   0        0        0      108 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/users_management.py
+-rw-r--r--   0        0        0     3711 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancies.py
+-rw-r--r--   0        0        0     1393 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancy_requests.py
+-rw-r--r--   0        0        0      482 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/webhooks.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_offers.py
+-rw-r--r--   0        0        0     1909 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_vacancy_request.py
+-rw-r--r--   0        0        0     1595 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/accounts.py
+-rw-r--r--   0        0        0     1187 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/action_logs.py
+-rw-r--r--   0        0        0     8554 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_logs.py
+-rw-r--r--   0        0        0      622 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_offers.py
+-rw-r--r--   0        0        0     1044 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      773 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     1197 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_response.py
+-rw-r--r--   0        0        0     5657 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicants.py
+-rw-r--r--   0        0        0     1306 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/coworkers.py
+-rw-r--r--   0        0        0     1381 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/delayed_tasks.py
+-rw-r--r--   0        0        0     2261 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/dictionaries.py
+-rw-r--r--   0        0        0     1507 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/divisions.py
+-rw-r--r--   0        0        0     1262 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/email_templates.py
+-rw-r--r--   0        0        0     2022 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/file.py
+-rw-r--r--   0        0        0      156 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/muilti_vacancies.py
+-rw-r--r--   0        0        0     1297 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/organization_settings.py
+-rw-r--r--   0        0        0     1525 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/production_calendars.py
+-rw-r--r--   0        0        0     1365 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/questionary.py
+-rw-r--r--   0        0        0      718 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/regions.py
+-rw-r--r--   0        0        0      476 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/rejection_reason.py
+-rw-r--r--   0        0        0    13292 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/resume.py
+-rw-r--r--   0        0        0     2953 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/survey.py
+-rw-r--r--   0        0        0      490 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/tags.py
+-rw-r--r--   0        0        0     1509 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/user_settings.py
+-rw-r--r--   0        0        0      795 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/users.py
+-rw-r--r--   0        0        0     1494 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/users_management.py
+-rw-r--r--   0        0        0     6357 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancies.py
+-rw-r--r--   0        0        0     2865 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancy_requests.py
+-rw-r--r--   0        0        0      719 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/webhooks.py
+-rw-r--r--   0        0        0       53 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/__init__.py
+-rw-r--r--   0        0        0     1871 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/locker.py
+-rw-r--r--   0        0        0     5186 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/proxy.py
+-rw-r--r--   0        0        0      730 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/storage.py
+-rw-r--r--   0        0        0      548 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/token.py
+-rw-r--r--   0        0        0     1649 2024-05-03 07:48:37.511069 huntflow_api_client-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     4829 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/api.py
+-rw-r--r--   0        0        0       79 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      176 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/fixtures/server.py
+-rw-r--r--   0        0        0      924 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/fixtures/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/__init__.py
+-rw-r--r--   0        0        0     3225 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_account_divisions.py
+-rw-r--r--   0        0        0     5097 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_account_offers.py
+-rw-r--r--   0        0        0     3886 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_account_vacancy_request.py
+-rw-r--r--   0        0        0     2329 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_accounts.py
+-rw-r--r--   0        0        0     1385 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_action_logs.py
+-rw-r--r--   0        0        0     7422 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_logs.py
+-rw-r--r--   0        0        0     3089 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_offers.py
+-rw-r--r--   0        0        0     3664 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy.py
+-rw-r--r--   0        0        0     1244 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy_statuses.py
+-rw-r--r--   0        0        0     1574 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_response.py
+-rw-r--r--   0        0        0    11555 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicants.py
+-rw-r--r--   0        0        0     2909 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_coworkers.py
+-rw-r--r--   0        0        0     1358 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_delayed_tasks.py
+-rw-r--r--   0        0        0     4497 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_dictionaries.py
+-rw-r--r--   0        0        0     2012 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_email_templates.py
+-rw-r--r--   0        0        0     1778 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_file.py
+-rw-r--r--   0        0        0     2925 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_multi_vacancies.py
+-rw-r--r--   0        0        0     2508 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_organization_settings.py
+-rw-r--r--   0        0        0     7896 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_production_calendar.py
+-rw-r--r--   0        0        0     3445 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_questionary.py
+-rw-r--r--   0        0        0     1015 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_regions.py
+-rw-r--r--   0        0        0     1069 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_rejection_reasons.py
+-rw-r--r--   0        0        0    15232 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_resume.py
+-rw-r--r--   0        0        0     2058 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_a.py
+-rw-r--r--   0        0        0     8613 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_q.py
+-rw-r--r--   0        0        0     4638 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_tags.py
+-rw-r--r--   0        0        0     2237 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_user_settings.py
+-rw-r--r--   0        0        0     1052 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_users.py
+-rw-r--r--   0        0        0     6510 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_users_management.py
+-rw-r--r--   0        0        0    16866 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_vacancies.py
+-rw-r--r--   0        0        0     4406 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_vacancy_request.py
+-rw-r--r--   0        0        0     2584 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_webhooks.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_errors/__init__.py
+-rw-r--r--   0        0        0     8107 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_errors/test_error_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_tokens/__init__.py
+-rw-r--r--   0        0        0     5556 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_tokens/test_access_token.py
+-rw-r--r--   0        0        0     2008 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_tokens/test_huntflow_token_proxy.py
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 huntflow_api_client-2.1.0/PKG-INFO
```

### Comparing `huntflow_api_client-2.0.1/LICENSE` & `huntflow_api_client-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/api.py` & `huntflow_api_client-2.1.0/huntflow_api_client/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/__init__.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 from huntflow_api_client.entities.account_vacancy_request import AccountVacancyRequest
 from huntflow_api_client.entities.accounts import Account
 from huntflow_api_client.entities.action_logs import ActionLog
 from huntflow_api_client.entities.applicant_logs import ApplicantLog
 from huntflow_api_client.entities.applicant_offers import ApplicantOffer
 from huntflow_api_client.entities.applicant_on_vacancy import ApplicantOnVacancy
 from huntflow_api_client.entities.applicant_on_vacancy_status import ApplicantOnVacancyStatus
+from huntflow_api_client.entities.applicant_reponse import ApplicantResponse
 from huntflow_api_client.entities.applicants import Applicant
 from huntflow_api_client.entities.coworkers import Coworker
 from huntflow_api_client.entities.delayed_tasks import DelayedTask
 from huntflow_api_client.entities.dictionaries import Dictionary
 from huntflow_api_client.entities.divisions import AccountDivision
 from huntflow_api_client.entities.email_templates import MailTemplate
 from huntflow_api_client.entities.file import File
 from huntflow_api_client.entities.multi_vacancies import MultiVacancy
 from huntflow_api_client.entities.organization_settings import OrganizationSettings
 from huntflow_api_client.entities.production_calendars import ProductionCalendar
 from huntflow_api_client.entities.questionary import ApplicantsQuestionary
 from huntflow_api_client.entities.regions import Region
 from huntflow_api_client.entities.rejection_reason import RejectionReason
 from huntflow_api_client.entities.resume import Resume
+from huntflow_api_client.entities.survey_type_a import SurveyTypeA
 from huntflow_api_client.entities.survey_type_q import SurveyTypeQ
 from huntflow_api_client.entities.tags import AccountTag, ApplicantTag
 from huntflow_api_client.entities.user_settings import UserSettings
 from huntflow_api_client.entities.users import User
 from huntflow_api_client.entities.users_management import UsersManagement
 from huntflow_api_client.entities.vacancies import Vacancy
 from huntflow_api_client.entities.vacancy_requests import VacancyRequest
@@ -37,28 +39,30 @@
     "AccountVacancyRequest",
     "ActionLog",
     "Applicant",
     "ApplicantLog",
     "ApplicantOffer",
     "ApplicantOnVacancy",
     "ApplicantOnVacancyStatus",
+    "ApplicantResponse",
     "ApplicantTag",
     "ApplicantsQuestionary",
     "Coworker",
     "DelayedTask",
     "Dictionary",
     "File",
     "MailTemplate",
     "MultiVacancy",
     "OrganizationSettings",
     "ProductionCalendar",
     "Region",
     "RejectionReason",
     "Resume",
+    "SurveyTypeA",
+    "SurveyTypeQ",
     "User",
     "UsersManagement",
     "UserSettings",
     "Vacancy",
     "VacancyRequest",
     "Webhook",
-    "SurveyTypeQ",
 )
```

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/account_offers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/account_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/account_vacancy_request.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/accounts.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/action_logs.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/action_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_logs.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_offers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_on_vacancy.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/applicant_on_vacancy_status.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/applicants.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/base.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/coworkers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/delayed_tasks.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/dictionaries.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/divisions.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/email_templates.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/email_templates.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/file.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/multi_vacancies.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/multi_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/organization_settings.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/organization_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/production_calendars.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/questionary.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/regions.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/regions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/rejection_reason.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/rejection_reason.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/resume.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/survey_type_q.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_q.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/tags.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/user_settings.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/user_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/users.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/users.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/users_management.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/users_management.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/vacancies.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/vacancy_requests.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/entities/webhooks.py` & `huntflow_api_client-2.1.0/huntflow_api_client/entities/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/errors/__init__.py` & `huntflow_api_client-2.1.0/huntflow_api_client/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/errors/errors.py` & `huntflow_api_client-2.1.0/huntflow_api_client/errors/errors.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/errors/handlers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/common.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/common.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/consts.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/consts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicant_logs.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicant_on_vacancy.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/applicants.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/dictionaries.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/divisions.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/file.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/multi_vacancies.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/multi_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/production_calendars.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/resume.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/vacancies.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/request/vacancy_requests.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/account_offers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/account_vacancy_request.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/accounts.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/action_logs.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/action_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_logs.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_offers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_on_vacancy.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicant_on_vacancy_status.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/applicants.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/coworkers.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/delayed_tasks.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/dictionaries.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/divisions.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/email_templates.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/email_templates.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/file.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/organization_settings.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/organization_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/production_calendars.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/questionary.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/regions.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/regions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/resume.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/survey.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/survey.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,7 +61,19 @@
 class SurveyQuestionaryAnswerResponse(BaseModel):
     id: int = Field(..., description="Survey questionary answer ID")
     created: datetime.datetime = Field(..., description="Date and time of creating an answer")
     survey: SurveySchemaTypeQResponse = Field(..., description="Survey questionary schema")
     respondent: SurveyQuestionaryRespondentWithName
     survey_questionary: SurveyQuestionaryCreatedInfo
     data: dict = Field(..., description="Answer data")
+
+
+class SurveySchemasTypeAListResponse(BaseModel):
+    items: List[BaseSurveySchemaType] = Field(..., description="List of type a survey schemas")
+
+
+class SurveySchemaTypeAResponse(BaseSurveySchemaTypeWithSchemas):
+    type: SurveyType = Field(
+        SurveyType.TYPE_A,
+        description="Type of survey",
+        frozen=True,
+    )
```

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/user_settings.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/user_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/users.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/users.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/users_management.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/users_management.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/vacancies.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/vacancy_requests.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/models/response/webhooks.py` & `huntflow_api_client-2.1.0/huntflow_api_client/models/response/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/tokens/locker.py` & `huntflow_api_client-2.1.0/huntflow_api_client/tokens/locker.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/tokens/proxy.py` & `huntflow_api_client-2.1.0/huntflow_api_client/tokens/proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/tokens/storage.py` & `huntflow_api_client-2.1.0/huntflow_api_client/tokens/storage.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/huntflow_api_client/tokens/token.py` & `huntflow_api_client-2.1.0/huntflow_api_client/tokens/token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/pyproject.toml` & `huntflow_api_client-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "huntflow-api-client"
-version = "2.0.1"
+version = "2.1.0"
 description = "Huntflow API Client for Python"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "email-validator>=1.3.1",
     "pydantic>=2.3.0",
 ]
-requires-python = ">3.8"
+requires-python = ">=3.8.1"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `huntflow_api_client-2.0.1/tests/api.py` & `huntflow_api_client-2.1.0/tests/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/fixtures/tokens.py` & `huntflow_api_client-2.1.0/tests/fixtures/tokens.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_account_divisions.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_account_divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_account_offers.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_account_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_account_vacancy_request.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_accounts.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_action_logs.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_action_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_applicant_logs.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_applicant_offers.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_applicant_on_vacancy.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_applicant_on_vacancy_statuses.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy_statuses.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_applicants.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_coworkers.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_delayed_tasks.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_dictionaries.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_email_templates.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_email_templates.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_file.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_multi_vacancies.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_multi_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_organization_settings.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_organization_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_production_calendar.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_production_calendar.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_questionary.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_regions.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_regions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_rejection_reasons.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_rejection_reasons.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_resume.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_survey_type_q.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_q.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_tags.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_user_settings.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_users.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_users.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_users_management.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_users_management.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_vacancies.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_vacancy_request.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_entities/test_webhooks.py` & `huntflow_api_client-2.1.0/tests/test_entities/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_errors/test_error_handlers.py` & `huntflow_api_client-2.1.0/tests/test_errors/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_tokens/test_access_token.py` & `huntflow_api_client-2.1.0/tests/test_tokens/test_access_token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/tests/test_tokens/test_huntflow_token_proxy.py` & `huntflow_api_client-2.1.0/tests/test_tokens/test_huntflow_token_proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.0.1/PKG-INFO` & `huntflow_api_client-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: huntflow-api-client
-Version: 2.0.1
+Version: 2.1.0
 Summary: Huntflow API Client for Python
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >3.8
+Requires-Python: >=3.8.1
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: email-validator>=1.3.1
 Requires-Dist: pydantic>=2.3.0
 Description-Content-Type: text/markdown
 
 [![](https://img.shields.io/pypi/pyversions/huntflow-api-client.svg)](https://pypi.org/project/huntflow-api-client/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

