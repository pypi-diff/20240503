# Comparing `tmp/cloudflare_cli4-2.19.4.tar.gz` & `tmp/cloudflare_cli4-2.19.4.post1.tar.gz`

## Comparing `cloudflare_cli4-2.19.4.tar` & `cloudflare_cli4-2.19.4.post1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.coveragerc
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.git
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.mypy.ini
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.python-version
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.readthedocs.yaml
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.travis.yml
--rw-r--r--   0        0        0   116899 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CHANGELOG.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/MANIFEST.in
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/Makefile
--rw-r--r--   0        0        0    54459 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/TABLE-OF-COMMANDS.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/pylintrc
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/requirements-dev.lock
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/requirements.lock
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/requirements.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/setup.cfg
--rwxr-xr-x   0        0        0     2370 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/setup.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/__init__.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/api_decode_from_openapi.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/api_extras.py
--rw-r--r--   0        0        0    60491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/api_v4.py
--rw-r--r--   0        0        0    54686 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/cloudflare.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/exceptions.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/logging_helper.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/network.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/read_configs.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/__init__.py
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/dummy_loa_document.pdf
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_add.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_api_dump.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_certificates.py
--rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_cloudflare.py
--rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_cloudflare_calls.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_dns_import_export.py
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_dns_records.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_find.py
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_graphql.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_images_v2_direct_upload.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_ips.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_issue114.py
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_loa_documents.py
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_load_balancers.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_log_received.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_paging_thru_zones.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_purge_cache.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_radar_returning_csv.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_rulesets.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_urlscanner.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_waiting_room.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/test_workers.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/CloudFlare/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/__init__.py
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/__main__.py
--rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/cli4.1
--rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/cli4.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/converters.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/dump.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/examples.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/myjsonlines.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/cli4/myyaml.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/docs/Makefile
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/docs/conf.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/__init__.py
--rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_account_rules_lists_items.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_ai_images.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_ai_speechrecognition.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_ai_translate.py
--rwxr-xr-x   0        0        0     1988 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_always_use_https.py
--rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_are_zones_ipv6.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_are_zones_ipv6_simple.py
--rwxr-xr-x   0        0        0     1732 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_bot_management.py
--rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_certificates.py
--rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_create_zone_and_populate.py
--rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_custom_hostnames.py
--rwxr-xr-x   0        0        0     2033 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_delete_zone_entry.py
--rwxr-xr-x   0        0        0     1378 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_dns_export.py
--rwxr-xr-x   0        0        0     1463 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_dns_import.py
--rwxr-xr-x   0        0        0     1458 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_dnssec_settings.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_firewall_rules.py
--rwxr-xr-x   0        0        0     2380 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_graphql.py
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_graphql.sh
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_images_v2_direct_upload.py
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_ips.py
--rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_list_api_from_web.py
--rwxr-xr-x   0        0        0     2206 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_page_rules.py
--rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_page_rules.sh
--rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_paging_thru_zones.py
--rwxr-xr-x   0        0        0      782 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_paging_thru_zones.sh
--rwxr-xr-x   0        0        0     3387 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_proxied.py
--rwxr-xr-x   0        0        0     1841 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_settings.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_show_zones_email.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_time_calls.py
--rwxr-xr-x   0        0        0     4320 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_update_dynamic_dns.py
--rwxr-xr-x   0        0        0     5570 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_user.py
--rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_user_tokens.py
--rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_with_usage.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_zone_purge_cache.py
--rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_zone_search.sh
--rwxr-xr-x   0        0        0     2368 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/examples/example_zones.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/.gitignore
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/LICENSE
--rw-r--r--   0        0        0    35977 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/README.md
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/pyproject.toml
--rw-r--r--   0        0        0    37232 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.coveragerc
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.git
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.mypy.ini
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.python-version
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.readthedocs.yaml
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.travis.yml
+-rw-r--r--   0        0        0   116899 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CHANGELOG.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/MANIFEST.in
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/Makefile
+-rw-r--r--   0        0        0    54459 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/TABLE-OF-COMMANDS.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/pylintrc
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/requirements-dev.lock
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/requirements.lock
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/setup.cfg
+-rwxr-xr-x   0        0        0     2370 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/setup.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/__init__.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/api_decode_from_openapi.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/api_extras.py
+-rw-r--r--   0        0        0    60491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/api_v4.py
+-rw-r--r--   0        0        0    54686 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/cloudflare.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/exceptions.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/logging_helper.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/network.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/read_configs.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/__init__.py
+-rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/dummy_loa_document.pdf
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_add.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_api_dump.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_certificates.py
+-rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_cloudflare.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_cloudflare_calls.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_dns_import_export.py
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_dns_records.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_find.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_graphql.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_images_v2_direct_upload.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_ips.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_issue114.py
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_loa_documents.py
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_load_balancers.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_log_received.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_paging_thru_zones.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_purge_cache.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_radar_returning_csv.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_rulesets.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_urlscanner.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_waiting_room.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_workers.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/CloudFlare/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/__init__.py
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/__main__.py
+-rw-r--r--   0        0        0     4610 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/cli4.1
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/cli4.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/converters.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/dump.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/examples.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/myjsonlines.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/cli4/myyaml.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/docs/Makefile
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/docs/conf.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/__init__.py
+-rwxr-xr-x   0        0        0     2779 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_account_rules_lists_items.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_ai_images.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_ai_speechrecognition.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_ai_translate.py
+-rwxr-xr-x   0        0        0     1988 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_always_use_https.py
+-rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_are_zones_ipv6.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_are_zones_ipv6_simple.py
+-rwxr-xr-x   0        0        0     1732 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_bot_management.py
+-rwxr-xr-x   0        0        0     2672 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_certificates.py
+-rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_create_zone_and_populate.py
+-rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_custom_hostnames.py
+-rwxr-xr-x   0        0        0     2033 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_delete_zone_entry.py
+-rwxr-xr-x   0        0        0     1378 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_dns_export.py
+-rwxr-xr-x   0        0        0     1463 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_dns_import.py
+-rwxr-xr-x   0        0        0     1458 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_dnssec_settings.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_firewall_rules.py
+-rwxr-xr-x   0        0        0     2380 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_graphql.py
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_graphql.sh
+-rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_images_v2_direct_upload.py
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_ips.py
+-rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_list_api_from_web.py
+-rwxr-xr-x   0        0        0     2206 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_page_rules.py
+-rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_page_rules.sh
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_paging_thru_zones.py
+-rwxr-xr-x   0        0        0      782 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_paging_thru_zones.sh
+-rwxr-xr-x   0        0        0     3387 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_proxied.py
+-rwxr-xr-x   0        0        0     1841 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_settings.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_show_zones_email.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_time_calls.py
+-rwxr-xr-x   0        0        0     4320 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_update_dynamic_dns.py
+-rwxr-xr-x   0        0        0     5570 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_user.py
+-rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_user_tokens.py
+-rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_with_usage.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_zone_purge_cache.py
+-rwxr-xr-x   0        0        0      421 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_zone_search.sh
+-rwxr-xr-x   0        0        0     2368 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/examples/example_zones.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/.gitignore
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/LICENSE
+-rw-r--r--   0        0        0    35977 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/README.md
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/pyproject.toml
+-rw-r--r--   0        0        0    37201 2020-02-02 00:00:00.000000 cloudflare_cli4-2.19.4.post1/PKG-INFO
```

### Comparing `cloudflare_cli4-2.19.4/.readthedocs.yaml` & `cloudflare_cli4-2.19.4.post1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CHANGELOG.md` & `cloudflare_cli4-2.19.4.post1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/Makefile` & `cloudflare_cli4-2.19.4.post1/Makefile`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/TABLE-OF-COMMANDS.md` & `cloudflare_cli4-2.19.4.post1/TABLE-OF-COMMANDS.md`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/pylintrc` & `cloudflare_cli4-2.19.4.post1/pylintrc`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/requirements-dev.lock` & `cloudflare_cli4-2.19.4.post1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/setup.py` & `cloudflare_cli4-2.19.4.post1/setup.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/api_decode_from_openapi.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/api_decode_from_openapi.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/api_extras.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/api_extras.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/api_v4.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/api_v4.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/cloudflare.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/exceptions.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/logging_helper.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/logging_helper.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/network.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/network.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/read_configs.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/read_configs.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/utils.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/dummy_loa_document.pdf` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/dummy_loa_document.pdf`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_add.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_api_dump.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_api_dump.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_certificates.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_certificates.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_cloudflare.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_cloudflare.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_cloudflare_calls.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_cloudflare_calls.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_dns_import_export.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_dns_import_export.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_dns_records.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_dns_records.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_find.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_graphql.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_images_v2_direct_upload.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_images_v2_direct_upload.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_ips.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_ips.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_issue114.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_issue114.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_loa_documents.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_loa_documents.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_load_balancers.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_load_balancers.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_log_received.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_log_received.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_paging_thru_zones.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_paging_thru_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_purge_cache.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_purge_cache.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_radar_returning_csv.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_radar_returning_csv.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_rulesets.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_rulesets.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_urlscanner.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_urlscanner.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_waiting_room.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_waiting_room.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/test_workers.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/CloudFlare/tests/utils.py` & `cloudflare_cli4-2.19.4.post1/CloudFlare/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/cli4/cli4.1` & `cloudflare_cli4-2.19.4.post1/cli4/cli4.1`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/cli4/cli4.py` & `cloudflare_cli4-2.19.4.post1/cli4/cli4.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/cli4/converters.py` & `cloudflare_cli4-2.19.4.post1/cli4/converters.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/cli4/dump.py` & `cloudflare_cli4-2.19.4.post1/cli4/dump.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/cli4/examples.py` & `cloudflare_cli4-2.19.4.post1/cli4/examples.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/cli4/myyaml.py` & `cloudflare_cli4-2.19.4.post1/cli4/myyaml.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/docs/Makefile` & `cloudflare_cli4-2.19.4.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/docs/conf.py` & `cloudflare_cli4-2.19.4.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_account_rules_lists_items.py` & `cloudflare_cli4-2.19.4.post1/examples/example_account_rules_lists_items.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_ai_images.py` & `cloudflare_cli4-2.19.4.post1/examples/example_ai_images.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_ai_speechrecognition.py` & `cloudflare_cli4-2.19.4.post1/examples/example_ai_speechrecognition.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_ai_translate.py` & `cloudflare_cli4-2.19.4.post1/examples/example_ai_translate.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_always_use_https.py` & `cloudflare_cli4-2.19.4.post1/examples/example_always_use_https.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_are_zones_ipv6.py` & `cloudflare_cli4-2.19.4.post1/examples/example_are_zones_ipv6.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_are_zones_ipv6_simple.py` & `cloudflare_cli4-2.19.4.post1/examples/example_are_zones_ipv6_simple.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_bot_management.py` & `cloudflare_cli4-2.19.4.post1/examples/example_bot_management.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_certificates.py` & `cloudflare_cli4-2.19.4.post1/examples/example_certificates.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_create_zone_and_populate.py` & `cloudflare_cli4-2.19.4.post1/examples/example_create_zone_and_populate.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_custom_hostnames.py` & `cloudflare_cli4-2.19.4.post1/examples/example_custom_hostnames.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_delete_zone_entry.py` & `cloudflare_cli4-2.19.4.post1/examples/example_delete_zone_entry.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_dns_export.py` & `cloudflare_cli4-2.19.4.post1/examples/example_dns_export.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_dns_import.py` & `cloudflare_cli4-2.19.4.post1/examples/example_dns_import.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_dnssec_settings.py` & `cloudflare_cli4-2.19.4.post1/examples/example_dnssec_settings.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_firewall_rules.py` & `cloudflare_cli4-2.19.4.post1/examples/example_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_graphql.py` & `cloudflare_cli4-2.19.4.post1/examples/example_graphql.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_graphql.sh` & `cloudflare_cli4-2.19.4.post1/examples/example_graphql.sh`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_images_v2_direct_upload.py` & `cloudflare_cli4-2.19.4.post1/examples/example_images_v2_direct_upload.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_ips.py` & `cloudflare_cli4-2.19.4.post1/examples/example_ips.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_list_api_from_web.py` & `cloudflare_cli4-2.19.4.post1/examples/example_list_api_from_web.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_page_rules.py` & `cloudflare_cli4-2.19.4.post1/examples/example_page_rules.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_paging_thru_zones.py` & `cloudflare_cli4-2.19.4.post1/examples/example_paging_thru_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_paging_thru_zones.sh` & `cloudflare_cli4-2.19.4.post1/examples/example_paging_thru_zones.sh`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_proxied.py` & `cloudflare_cli4-2.19.4.post1/examples/example_proxied.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_settings.py` & `cloudflare_cli4-2.19.4.post1/examples/example_settings.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_show_zones_email.py` & `cloudflare_cli4-2.19.4.post1/examples/example_show_zones_email.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_time_calls.py` & `cloudflare_cli4-2.19.4.post1/examples/example_time_calls.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_update_dynamic_dns.py` & `cloudflare_cli4-2.19.4.post1/examples/example_update_dynamic_dns.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_user.py` & `cloudflare_cli4-2.19.4.post1/examples/example_user.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_user_tokens.py` & `cloudflare_cli4-2.19.4.post1/examples/example_user_tokens.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_with_usage.py` & `cloudflare_cli4-2.19.4.post1/examples/example_with_usage.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_zone_purge_cache.py` & `cloudflare_cli4-2.19.4.post1/examples/example_zone_purge_cache.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/examples/example_zones.py` & `cloudflare_cli4-2.19.4.post1/examples/example_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/.gitignore` & `cloudflare_cli4-2.19.4.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/LICENSE` & `cloudflare_cli4-2.19.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/README.md` & `cloudflare_cli4-2.19.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `cloudflare_cli4-2.19.4/pyproject.toml` & `cloudflare_cli4-2.19.4.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "cloudflare-cli4"
-version = "2.19.4"
+version = "2.19.4-1"
 readme = "README.md"
-description = "Python wrapper for the Cloudflare v4 API"
+description = "Command line tool to interact with Cloudflare API v4"
 authors = [
     { name = "Martin J. Levy", email = "mahtin@mahtin.com" },
     { name = "Stainless Inc.", email = "support@stainlessapi.com" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -25,17 +25,16 @@
 requires-python = ">3.6.0"
 license = { text = "MIT" }
 
 keywords = ["cloudflare", "API", "wrapper"]
 dependencies = ["requests", "pyyaml", "jsonlines"]
 
 [project.urls]
-documentation = "https://python-cloudflare.readthedocs.io/"
-api-documentation = "https://developers.cloudflare.com/api/"
-source-code = "https://github.com/cloudflare/python-cloudflare"
+documentation = "https://github.com/stainless-api/python-cloudflare-cli4"
+source-code = "https://github.com/stainless-api/python-cloudflare-cli4"
 
 [project.scripts]
 cli4 = "cli4.__main__:main"
 
 [project.data-files]
 "share/man/man1" = ["cli4/cli4.1"]
```

### Comparing `cloudflare_cli4-2.19.4/PKG-INFO` & `cloudflare_cli4-2.19.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.3
 Name: cloudflare-cli4
-Version: 2.19.4
-Summary: Python wrapper for the Cloudflare v4 API
-Project-URL: documentation, https://python-cloudflare.readthedocs.io/
-Project-URL: api-documentation, https://developers.cloudflare.com/api/
-Project-URL: source-code, https://github.com/cloudflare/python-cloudflare
+Version: 2.19.4.post1
+Summary: Command line tool to interact with Cloudflare API v4
+Project-URL: documentation, https://github.com/stainless-api/python-cloudflare-cli4
+Project-URL: source-code, https://github.com/stainless-api/python-cloudflare-cli4
 Author-email: "Martin J. Levy" <mahtin@mahtin.com>, "Stainless Inc." <support@stainlessapi.com>
 License: MIT
 License-File: LICENSE
 Keywords: API,cloudflare,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

