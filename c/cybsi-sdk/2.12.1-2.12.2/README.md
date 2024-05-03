# Comparing `tmp/cybsi_sdk-2.12.1.tar.gz` & `tmp/cybsi_sdk-2.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybsi_sdk-2.12.1.tar", max compression
+gzip compressed data, was "cybsi_sdk-2.12.2.tar", max compression
```

## Comparing `cybsi_sdk-2.12.1.tar` & `cybsi_sdk-2.12.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    10142 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/LICENSE
--rw-r--r--   0        0        0      777 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/README.md
--rw-r--r--   0        0        0      151 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/__init__.py
--rw-r--r--   0        0        0      217 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/__version__.py
--rw-r--r--   0        0        0      618 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/api.py
--rw-r--r--   0        0        0      365 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/artifact/__init__.py
--rw-r--r--   0        0        0    22150 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/artifact/api.py
--rw-r--r--   0        0        0      663 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/artifact/enums.py
--rw-r--r--   0        0        0      227 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/auth/__init__.py
--rw-r--r--   0        0        0    14437 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/auth/api_key.py
--rw-r--r--   0        0        0      819 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/auth/token.py
--rw-r--r--   0        0        0    10259 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/client.py
--rw-r--r--   0        0        0     4773 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/client_config.py
--rw-r--r--   0        0        0      450 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/data_source/__init__.py
--rw-r--r--   0        0        0    17285 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/data_source/api.py
--rw-r--r--   0        0        0    11497 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/data_source/api_types.py
--rw-r--r--   0        0        0      520 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/data_source/enums.py
--rw-r--r--   0        0        0      630 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/dictionary/__init__.py
--rw-r--r--   0        0        0    13534 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/dictionary/api.py
--rw-r--r--   0        0        0     1320 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/enrichment/__init__.py
--rw-r--r--   0        0        0    10043 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/enrichment/analyzers.py
--rw-r--r--   0        0        0     1407 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/enrichment/api.py
--rw-r--r--   0        0        0    15259 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/enrichment/config_rules.py
--rw-r--r--   0        0        0     2660 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/enrichment/enums.py
--rw-r--r--   0        0        0     9249 2024-04-26 10:35:28.145497 cybsi_sdk-2.12.1/cybsi/api/enrichment/external_dbs.py
--rw-r--r--   0        0        0    12568 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/enrichment/task_queue.py
--rw-r--r--   0        0        0    20436 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/enrichment/tasks.py
--rw-r--r--   0        0        0      823 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/enum.py
--rw-r--r--   0        0        0    11261 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/error.py
--rw-r--r--   0        0        0      237 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/internal/__init__.py
--rw-r--r--   0        0        0     1948 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/internal/base.py
--rw-r--r--   0        0        0     7166 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/internal/connector.py
--rw-r--r--   0        0        0     1707 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/internal/multipart.py
--rw-r--r--   0        0        0      870 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/internal/time.py
--rw-r--r--   0        0        0      125 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/license/__init__.py
--rw-r--r--   0        0        0     2463 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/license/api.py
--rw-r--r--   0        0        0      359 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/license/enums.py
--rw-r--r--   0        0        0     1361 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/__init__.py
--rw-r--r--   0        0        0    10529 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/aggregate_section.py
--rw-r--r--   0        0        0     1188 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/annotations.py
--rw-r--r--   0        0        0     1043 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/api.py
--rw-r--r--   0        0        0    37818 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/entities_api.py
--rw-r--r--   0        0        0     4711 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/entity.py
--rw-r--r--   0        0        0    12621 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/enums.py
--rw-r--r--   0        0        0     3163 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/links.py
--rw-r--r--   0        0        0     5050 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/relationships.py
--rw-r--r--   0        0        0     2397 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observable/view.py
--rw-r--r--   0        0        0      990 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/__init__.py
--rw-r--r--   0        0        0     6009 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/api.py
--rw-r--r--   0        0        0     3648 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/archive.py
--rw-r--r--   0        0        0     3347 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/dns_lookup.py
--rw-r--r--   0        0        0      481 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/enums.py
--rw-r--r--   0        0        0    14423 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/generic.py
--rw-r--r--   0        0        0     3446 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/network_session.py
--rw-r--r--   0        0        0     3336 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/threat.py
--rw-r--r--   0        0        0     1248 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/view.py
--rw-r--r--   0        0        0     3387 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/observation/whois_lookup.py
--rw-r--r--   0        0        0     4179 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/pagination.py
--rw-r--r--   0        0        0      439 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/replist/__init__.py
--rw-r--r--   0        0        0    17391 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/replist/api.py
--rw-r--r--   0        0        0      581 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/replist/enums.py
--rw-r--r--   0        0        0      331 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/report/__init__.py
--rw-r--r--   0        0        0    39720 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/report/api.py
--rw-r--r--   0        0        0      382 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/search/__init__.py
--rw-r--r--   0        0        0      280 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/search/api.py
--rw-r--r--   0        0        0      230 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/search/enums.py
--rw-r--r--   0        0        0     2438 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/search/error.py
--rw-r--r--   0        0        0     8417 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/search/stored_queries.py
--rw-r--r--   0        0        0      232 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/user/__init__.py
--rw-r--r--   0        0        0    15519 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/user/api.py
--rw-r--r--   0        0        0     3777 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/user/enums.py
--rw-r--r--   0        0        0     1160 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/api/view.py
--rw-r--r--   0        0        0        0 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/py.typed
--rw-r--r--   0        0        0       68 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/utils/__init__.py
--rw-r--r--   0        0        0     5078 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/utils/converters.py
--rw-r--r--   0        0        0     3879 2024-04-26 10:35:28.149497 cybsi_sdk-2.12.1/cybsi/utils/views.py
--rw-r--r--   0        0        0     1292 2024-04-26 10:35:28.153497 cybsi_sdk-2.12.1/pyproject.toml
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 cybsi_sdk-2.12.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/LICENSE
+-rw-r--r--   0        0        0      777 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/README.md
+-rw-r--r--   0        0        0      151 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/__version__.py
+-rw-r--r--   0        0        0      618 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/__init__.py
+-rw-r--r--   0        0        0     1360 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/api.py
+-rw-r--r--   0        0        0      365 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/artifact/__init__.py
+-rw-r--r--   0        0        0    22150 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/artifact/api.py
+-rw-r--r--   0        0        0      663 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/artifact/enums.py
+-rw-r--r--   0        0        0      227 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/auth/__init__.py
+-rw-r--r--   0        0        0    14437 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/auth/api_key.py
+-rw-r--r--   0        0        0      819 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/auth/token.py
+-rw-r--r--   0        0        0    10578 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/client.py
+-rw-r--r--   0        0        0     4773 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/client_config.py
+-rw-r--r--   0        0        0      450 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/data_source/__init__.py
+-rw-r--r--   0        0        0    17285 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/data_source/api.py
+-rw-r--r--   0        0        0    11497 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/data_source/api_types.py
+-rw-r--r--   0        0        0      520 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/data_source/enums.py
+-rw-r--r--   0        0        0      630 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/dictionary/__init__.py
+-rw-r--r--   0        0        0    13662 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/dictionary/api.py
+-rw-r--r--   0        0        0     1320 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/__init__.py
+-rw-r--r--   0        0        0    10043 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/analyzers.py
+-rw-r--r--   0        0        0     1407 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/api.py
+-rw-r--r--   0        0        0    15259 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/config_rules.py
+-rw-r--r--   0        0        0     2660 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/enums.py
+-rw-r--r--   0        0        0     9249 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/external_dbs.py
+-rw-r--r--   0        0        0    12568 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/task_queue.py
+-rw-r--r--   0        0        0    20436 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enrichment/tasks.py
+-rw-r--r--   0        0        0      823 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/enum.py
+-rw-r--r--   0        0        0    11261 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/error.py
+-rw-r--r--   0        0        0      237 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/internal/__init__.py
+-rw-r--r--   0        0        0     1948 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/internal/base.py
+-rw-r--r--   0        0        0     7166 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/internal/connector.py
+-rw-r--r--   0        0        0     1707 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/internal/multipart.py
+-rw-r--r--   0        0        0      870 2024-05-03 08:20:24.981925 cybsi_sdk-2.12.2/cybsi/api/internal/time.py
+-rw-r--r--   0        0        0      125 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/license/__init__.py
+-rw-r--r--   0        0        0     2463 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/license/api.py
+-rw-r--r--   0        0        0      359 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/license/enums.py
+-rw-r--r--   0        0        0     1361 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/__init__.py
+-rw-r--r--   0        0        0    10529 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/aggregate_section.py
+-rw-r--r--   0        0        0     1188 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/annotations.py
+-rw-r--r--   0        0        0     1043 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/api.py
+-rw-r--r--   0        0        0    37818 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/entities_api.py
+-rw-r--r--   0        0        0     4711 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/entity.py
+-rw-r--r--   0        0        0    12621 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/enums.py
+-rw-r--r--   0        0        0     3163 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/links.py
+-rw-r--r--   0        0        0     5050 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/relationships.py
+-rw-r--r--   0        0        0     2397 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observable/view.py
+-rw-r--r--   0        0        0      990 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/__init__.py
+-rw-r--r--   0        0        0     6009 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/api.py
+-rw-r--r--   0        0        0     3648 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/archive.py
+-rw-r--r--   0        0        0     3347 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/dns_lookup.py
+-rw-r--r--   0        0        0      481 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/enums.py
+-rw-r--r--   0        0        0    14423 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/generic.py
+-rw-r--r--   0        0        0     3446 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/network_session.py
+-rw-r--r--   0        0        0     3336 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/threat.py
+-rw-r--r--   0        0        0     1248 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/view.py
+-rw-r--r--   0        0        0     3387 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/observation/whois_lookup.py
+-rw-r--r--   0        0        0     4179 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/pagination.py
+-rw-r--r--   0        0        0      439 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/replist/__init__.py
+-rw-r--r--   0        0        0    17391 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/replist/api.py
+-rw-r--r--   0        0        0      581 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/replist/enums.py
+-rw-r--r--   0        0        0      331 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/report/__init__.py
+-rw-r--r--   0        0        0    39720 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/report/api.py
+-rw-r--r--   0        0        0      409 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/search/__init__.py
+-rw-r--r--   0        0        0      280 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/search/api.py
+-rw-r--r--   0        0        0      230 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/search/enums.py
+-rw-r--r--   0        0        0     2438 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/search/error.py
+-rw-r--r--   0        0        0     8577 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/search/stored_queries.py
+-rw-r--r--   0        0        0      232 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/user/__init__.py
+-rw-r--r--   0        0        0    15519 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/user/api.py
+-rw-r--r--   0        0        0     3777 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/user/enums.py
+-rw-r--r--   0        0        0     1160 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/api/view.py
+-rw-r--r--   0        0        0        0 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/py.typed
+-rw-r--r--   0        0        0       68 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/utils/__init__.py
+-rw-r--r--   0        0        0     5078 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/utils/converters.py
+-rw-r--r--   0        0        0     3879 2024-05-03 08:20:24.985925 cybsi_sdk-2.12.2/cybsi/utils/views.py
+-rw-r--r--   0        0        0     1292 2024-05-03 08:20:24.989925 cybsi_sdk-2.12.2/pyproject.toml
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 cybsi_sdk-2.12.2/PKG-INFO
```

### Comparing `cybsi_sdk-2.12.1/LICENSE` & `cybsi_sdk-2.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/README.md` & `cybsi_sdk-2.12.2/README.md`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/__init__.py` & `cybsi_sdk-2.12.2/cybsi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/api.py` & `cybsi_sdk-2.12.2/cybsi/api/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/artifact/api.py` & `cybsi_sdk-2.12.2/cybsi/api/artifact/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/artifact/enums.py` & `cybsi_sdk-2.12.2/cybsi/api/artifact/enums.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/auth/api_key.py` & `cybsi_sdk-2.12.2/cybsi/api/auth/api_key.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/auth/token.py` & `cybsi_sdk-2.12.2/cybsi/api/auth/token.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/client.py` & `cybsi_sdk-2.12.2/cybsi/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,14 +271,27 @@
         return ReplistsAsyncAPI(self._connector)
 
     @property
     def observable(self) -> ObservableAsyncAPI:
         """Observable API handle."""
         return ObservableAsyncAPI(self._connector)
 
+    async def version(self) -> "VersionView":
+        """Get API and server version information.
+
+        Note:
+            Calls `GET /version`.
+        Returns:
+            Version view.
+        """
+
+        path = "/version"
+        resp = await self._connector.do_get(path)
+        return VersionView(resp.json())
+
 
 class VersionView(JsonObjectView):
     """Version view."""
 
     @property
     def api_version(self) -> "Version":
         """API specification version."""
```

### Comparing `cybsi_sdk-2.12.1/cybsi/api/client_config.py` & `cybsi_sdk-2.12.2/cybsi/api/client_config.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/data_source/api.py` & `cybsi_sdk-2.12.2/cybsi/api/data_source/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/data_source/api_types.py` & `cybsi_sdk-2.12.2/cybsi/api/data_source/api_types.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/data_source/enums.py` & `cybsi_sdk-2.12.2/cybsi/api/data_source/enums.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/dictionary/__init__.py` & `cybsi_sdk-2.12.2/cybsi/api/dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/dictionary/api.py` & `cybsi_sdk-2.12.2/cybsi/api/dictionary/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,16 +356,17 @@
 
 class DictionaryItemForm(JsonObjectForm):
     """Dictionary item form. Use to add dictionary item.
 
     Args:
         dictionary_uuid: Dictionary identifier.
         key: Dictionary item key. The key should consist of characters
-            according to the pattern `[a-zA-Z0-9_ -]` and
-            have length in the range `[1;30]`.
+            according to the pattern `[a-zA-Z0-9_ :.@-]` and
+            have length in the range `[1;50]`.
+            First and last char of key can't be space-symbol
             User-specified key case is preserved.
     """
 
     def __init__(self, *, dictionary_uuid: uuid.UUID, key: str):
         super().__init__()
         self._data["dictionaryUUID"] = str(dictionary_uuid)
         self._data["key"] = key
@@ -373,15 +374,16 @@
 
 class DictItemAttributeValue(JsonObjectForm):
     """Dictionary item. Used as attribute value to create a general observation.
     See :meth:`~cybsi.api.observation.generic.GenericObservationForm.add_attribute_fact`
 
     Args:
        key: Dictionary item key. The key should consist of characters
-            according to the pattern `[a-zA-Z0-9_ -]` and
-            have length in the range `[1;30]`.
+            according to the pattern `[a-zA-Z0-9_ :.@-]` and
+            have length in the range `[1;50]`.
+            First and last char of key can't be space-symbol
             User-specified key case is preserved.
     """
 
     def __init__(self, *, key: str):
         super().__init__()
         self._data["key"] = key
```

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/__init__.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/analyzers.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/analyzers.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/api.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/config_rules.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/config_rules.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/enums.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/enums.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/external_dbs.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/external_dbs.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/task_queue.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/task_queue.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enrichment/tasks.py` & `cybsi_sdk-2.12.2/cybsi/api/enrichment/tasks.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/enum.py` & `cybsi_sdk-2.12.2/cybsi/api/enum.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/error.py` & `cybsi_sdk-2.12.2/cybsi/api/error.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/internal/base.py` & `cybsi_sdk-2.12.2/cybsi/api/internal/base.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/internal/connector.py` & `cybsi_sdk-2.12.2/cybsi/api/internal/connector.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/internal/multipart.py` & `cybsi_sdk-2.12.2/cybsi/api/internal/multipart.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/internal/time.py` & `cybsi_sdk-2.12.2/cybsi/api/internal/time.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/license/api.py` & `cybsi_sdk-2.12.2/cybsi/api/license/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/__init__.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/aggregate_section.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/aggregate_section.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/annotations.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/annotations.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/api.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/entities_api.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/entities_api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/entity.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/entity.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/enums.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/enums.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/links.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/links.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/relationships.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/relationships.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observable/view.py` & `cybsi_sdk-2.12.2/cybsi/api/observable/view.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/__init__.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/api.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/archive.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/archive.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/dns_lookup.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/dns_lookup.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/generic.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/generic.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/network_session.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/network_session.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/threat.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/threat.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/view.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/view.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/observation/whois_lookup.py` & `cybsi_sdk-2.12.2/cybsi/api/observation/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/pagination.py` & `cybsi_sdk-2.12.2/cybsi/api/pagination.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/replist/api.py` & `cybsi_sdk-2.12.2/cybsi/api/replist/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/replist/enums.py` & `cybsi_sdk-2.12.2/cybsi/api/replist/enums.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/report/api.py` & `cybsi_sdk-2.12.2/cybsi/api/report/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/search/error.py` & `cybsi_sdk-2.12.2/cybsi/api/search/error.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/search/stored_queries.py` & `cybsi_sdk-2.12.2/cybsi/api/search/stored_queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
     def filter(
         self,
         *,
         user_uuid: Optional[uuid.UUID] = None,
         cursor: Optional[Cursor] = None,
         limit: Optional[int] = None,
-    ) -> Page["StoredQueryView"]:
+    ) -> Page["StoredQueryFilterView"]:
         """Get page of filtered stored queries list.
 
         Note:
             Calls `GET /search/stored-queries`
         Args:
             user_uuid: User's identifier.
                 Filter stored queries by author's id.
@@ -134,15 +134,15 @@
             params["userUUID"] = str(user_uuid)
         if cursor:
             params["cursor"] = str(cursor)
         if limit:
             params["limit"] = str(limit)
 
         resp = self._connector.do_get(self._path, params=params)
-        page = Page(self._connector.do_get, resp, StoredQueryView)
+        page = Page(self._connector.do_get, resp, StoredQueryFilterView)
         return page
 
 
 class StoredQueryForm(JsonObjectForm):
     """Stored query form.
 
     This is the form you need to fill to register stored query.
@@ -260,22 +260,27 @@
 
     @property
     def name(self) -> str:
         """Query name."""
         return self._get("name")
 
 
-class StoredQueryView(_TaggedRefView, StoredQueryCommonView):
-    """View of a stored query,
-    as retrieved by :meth:`StoredQueriesAPI.view`."""
+class StoredQueryFilterView(StoredQueryCommonView):
+    """Filter view of a stored query,
+    as retrieved by :meth:`StoredQueriesAPI.filter`."""
 
     @property
     def text(self) -> str:
         """Query text."""
 
         return self._get("text")
 
     @property
     def author(self) -> RefView:
         """User, author of the query."""
 
         return RefView(self._get("author"))
+
+
+class StoredQueryView(_TaggedRefView, StoredQueryFilterView):
+    """View of a stored query,
+    as retrieved by :meth:`StoredQueriesAPI.view`."""
```

### Comparing `cybsi_sdk-2.12.1/cybsi/api/user/api.py` & `cybsi_sdk-2.12.2/cybsi/api/user/api.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/user/enums.py` & `cybsi_sdk-2.12.2/cybsi/api/user/enums.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/api/view.py` & `cybsi_sdk-2.12.2/cybsi/api/view.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/utils/converters.py` & `cybsi_sdk-2.12.2/cybsi/utils/converters.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/cybsi/utils/views.py` & `cybsi_sdk-2.12.2/cybsi/utils/views.py`

 * *Files identical despite different names*

### Comparing `cybsi_sdk-2.12.1/pyproject.toml` & `cybsi_sdk-2.12.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cybsi-sdk"
-version = "2.12.1"
+version = "2.12.2"
 description = "Cybsi development kit"
 authors = ["Cybsi SDK developers"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "cybsi" },
 ]
@@ -38,15 +38,15 @@
 [tool.isort]
 profile = "black"
 extend_skip = ["__init__.py"]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "2.12.1"
+current = "2.12.2"
 
 regex = '''
   ^
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
```

### Comparing `cybsi_sdk-2.12.1/PKG-INFO` & `cybsi_sdk-2.12.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybsi-sdk
-Version: 2.12.1
+Version: 2.12.2
 Summary: Cybsi development kit
 License: Apache-2.0
 Author: Cybsi SDK developers
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

