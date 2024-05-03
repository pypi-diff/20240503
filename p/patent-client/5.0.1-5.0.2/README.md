# Comparing `tmp/patent_client-5.0.1.tar.gz` & `tmp/patent_client-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-5.0.1.tar", max compression
+gzip compressed data, was "patent_client-5.0.2.tar", max compression
```

## Comparing `patent_client-5.0.1.tar` & `patent_client-5.0.2.tar`

### file list

```diff
@@ -1,408 +1,408 @@
--rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.1/LICENSE
--rw-r--r--   0        0        0     6283 2024-05-02 16:19:13.662029 patent_client-5.0.1/README.md
--rw-r--r--   0        0        0     1745 2024-05-01 18:31:51.839413 patent_client-5.0.1/patent_client/__init__.py
--rw-r--r--   0        0        0      833 2024-05-01 18:11:58.854819 patent_client-5.0.1/patent_client/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.1/patent_client/_async/epo/__init__.py
--rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.1/patent_client/_async/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.1/patent_client/_async/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      384 2024-05-02 16:38:02.138419 patent_client-5.0.1/patent_client/_async/epo/ops/family/api.py
--rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.1/patent_client/_async/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      378 2024-05-01 18:05:47.952110 patent_client-5.0.1/patent_client/_async/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.1/patent_client/_async/epo/ops/family/model.py
--rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.1/patent_client/_async/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1545 2024-05-01 18:05:47.953175 patent_client-5.0.1/patent_client/_async/epo/ops/family/schema.py
--rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.1/patent_client/_async/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.1/patent_client/_async/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      359 2024-05-02 16:38:02.129547 patent_client-5.0.1/patent_client/_async/epo/ops/legal/api.py
--rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.1/patent_client/_async/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      489 2024-05-01 18:05:47.953918 patent_client-5.0.1/patent_client/_async/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.1/patent_client/_async/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5554 2024-05-01 18:49:55.209500 patent_client-5.0.1/patent_client/_async/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.1/patent_client/_async/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4062 2024-05-01 18:05:47.954735 patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.1/patent_client/_async/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1415 2024-05-02 16:38:02.133836 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.1/patent_client/_async/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5542 2024-05-02 16:38:45.106304 patent_client-5.0.1/patent_client/_async/epo/ops/published/api.py
--rw-r--r--   0        0        0     2743 2024-05-02 16:55:55.950023 patent_client-5.0.1/patent_client/_async/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.1/patent_client/_async/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-02 16:54:56.798037 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-02 16:54:56.801597 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-05-02 16:54:56.812017 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3226 2024-05-02 16:37:07.255945 patent_client-5.0.1/patent_client/_async/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2433 2024-05-02 16:55:55.950077 patent_client-5.0.1/patent_client/_async/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2108 2024-05-02 16:32:37.841594 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3962 2024-05-01 18:05:47.958633 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1668 2024-05-01 18:05:47.959251 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3193 2024-05-01 18:16:57.840152 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-02 16:54:56.944056 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-02 16:54:56.947909 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3478 2024-05-02 16:38:02.129285 patent_client-5.0.1/patent_client/_async/epo/ops/session.py
--rw-r--r--   0        0        0     2881 2024-05-02 16:55:55.950107 patent_client-5.0.1/patent_client/_async/epo/ops/util.py
--rw-r--r--   0        0        0     3234 2024-05-01 18:32:10.993912 patent_client-5.0.1/patent_client/_async/http_client.py
--rw-r--r--   0        0        0      201 2024-05-01 18:11:58.854920 patent_client-5.0.1/patent_client/_async/odp.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.1/patent_client/_async/uspto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.1/patent_client/_async/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2552 2024-05-01 18:05:47.961041 patent_client-5.0.1/patent_client/_async/uspto/assignment/api.py
--rw-r--r--   0        0        0      921 2024-05-01 18:11:58.854972 patent_client-5.0.1/patent_client/_async/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     3633 2024-05-01 18:05:47.961566 patent_client-5.0.1/patent_client/_async/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.1/patent_client/_async/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3454 2024-05-01 18:15:07.226884 patent_client-5.0.1/patent_client/_async/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4202 2024-05-01 18:14:52.417225 patent_client-5.0.1/patent_client/_async/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5506 2024-05-01 18:33:09.323130 patent_client-5.0.1/patent_client/_async/uspto/assignment/model.py
--rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.1/patent_client/_async/uspto/assignment/model_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3226 2024-05-01 18:37:44.350189 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1567 2024-05-01 18:37:29.912372 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/model.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1902 2024-05-01 18:05:47.969601 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7111 2024-05-01 18:11:58.855043 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6063 2024-05-01 18:05:47.970370 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.1/patent_client/_async/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5502 2024-05-01 18:11:58.855103 patent_client-5.0.1/patent_client/_async/uspto/odp/api.py
--rw-r--r--   0        0        0     2834 2024-05-01 18:05:47.971502 patent_client-5.0.1/patent_client/_async/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     4834 2024-05-01 18:11:58.855157 patent_client-5.0.1/patent_client/_async/uspto/odp/manager.py
--rw-r--r--   0        0        0     1895 2024-05-01 18:11:58.855213 patent_client-5.0.1/patent_client/_async/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16427 2024-05-01 18:11:58.855271 patent_client-5.0.1/patent_client/_async/uspto/odp/model.py
--rw-r--r--   0        0        0    12253 2024-05-01 18:05:47.972423 patent_client-5.0.1/patent_client/_async/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.1/patent_client/_async/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.1/patent_client/_async/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.1/patent_client/_async/uspto/odp/util.py
--rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.1/patent_client/_async/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.1/patent_client/_async/uspto/peds/api.py
--rw-r--r--   0        0        0      711 2024-05-01 18:05:47.973610 patent_client-5.0.1/patent_client/_async/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8585 2024-05-02 16:13:03.406844 patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8495 2024-05-02 16:01:44.826324 patent_client-5.0.1/patent_client/_async/uspto/peds/manager.py
--rw-r--r--   0        0        0     9726 2024-05-02 16:13:06.160175 patent_client-5.0.1/patent_client/_async/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    14987 2024-05-02 16:10:44.102210 patent_client-5.0.1/patent_client/_async/uspto/peds/model.py
--rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.1/patent_client/_async/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.1/patent_client/_async/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      188 2024-05-01 18:14:39.938865 patent_client-5.0.1/patent_client/_async/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10200 2024-05-01 18:05:47.974861 patent_client-5.0.1/patent_client/_async/uspto/ptab/api.py
--rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.1/patent_client/_async/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2085 2024-05-01 18:05:47.975042 patent_client-5.0.1/patent_client/_async/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2311 2024-05-01 18:05:47.975211 patent_client-5.0.1/patent_client/_async/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8358 2024-05-01 18:37:03.633749 patent_client-5.0.1/patent_client/_async/uspto/ptab/model.py
--rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.1/patent_client/_async/uspto/ptab/util.py
--rw-r--r--   0        0        0      326 2024-05-01 18:14:14.991401 patent_client-5.0.1/patent_client/_async/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6701 2024-05-01 18:38:39.241032 patent_client-5.0.1/patent_client/_async/uspto/public_search/api.py
--rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.1/patent_client/_async/uspto/public_search/api_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6678 2024-05-01 18:05:47.983341 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1035 2024-05-01 18:13:57.304685 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.1/patent_client/_async/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-02 16:54:59.151394 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4144 2024-05-01 18:05:47.983936 patent_client-5.0.1/patent_client/_async/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7743 2024-05-01 18:05:47.984232 patent_client-5.0.1/patent_client/_async/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      524 2024-05-01 18:40:07.745391 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3144 2024-05-01 18:16:57.840869 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7574 2024-05-01 18:05:47.984820 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2249 2024-05-01 18:05:47.984983 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1535 2024-05-01 18:13:46.898757 patent_client-5.0.1/patent_client/_async/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4520 2024-05-01 18:05:47.985447 patent_client-5.0.1/patent_client/_async/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.1/patent_client/_async/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4313 2024-05-01 18:12:45.762919 patent_client-5.0.1/patent_client/_async/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.1/patent_client/_async/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.1/patent_client/_async/uspto/public_search/util.py
--rw-r--r--   0        0        0     1249 2024-05-02 16:54:49.273351 patent_client-5.0.1/patent_client/_sync/__init__.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.680949 patent_client-5.0.1/patent_client/_sync/epo/__init__.py
--rw-r--r--   0        0        0      630 2024-05-02 16:54:49.692358 patent_client-5.0.1/patent_client/_sync/epo/ops/__init__.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.706525 patent_client-5.0.1/patent_client/_sync/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      788 2024-05-02 16:54:49.709397 patent_client-5.0.1/patent_client/_sync/epo/ops/family/api.py
--rw-r--r--   0        0        0      855 2024-05-02 16:54:49.710444 patent_client-5.0.1/patent_client/_sync/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714131 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-05-02 16:54:49.714466 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-05-02 16:54:49.714990 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714682 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      772 2024-05-02 16:54:49.711289 patent_client-5.0.1/patent_client/_sync/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1535 2024-05-02 16:54:49.708518 patent_client-5.0.1/patent_client/_sync/epo/ops/family/model.py
--rw-r--r--   0        0        0      903 2024-05-02 16:54:49.705264 patent_client-5.0.1/patent_client/_sync/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1961 2024-05-02 16:54:49.713729 patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema.py
--rw-r--r--   0        0        0      943 2024-05-02 16:54:49.706394 patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.784538 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      763 2024-05-02 16:54:49.789201 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api.py
--rw-r--r--   0        0        0      704 2024-05-02 16:54:49.799011 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-05-02 16:54:49.811517 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-05-02 16:54:49.808791 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-05-02 16:54:49.811216 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-05-02 16:54:49.810170 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-05-02 16:54:49.810402 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-05-02 16:54:49.810723 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-05-02 16:54:49.808401 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      883 2024-05-02 16:54:49.800072 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2791 2024-05-02 16:54:49.788392 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5908 2024-05-02 16:54:49.798143 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      882 2024-05-02 16:54:49.781664 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4478 2024-05-02 16:54:49.806767 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1632 2024-05-02 16:54:49.783877 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      530 2024-05-02 16:54:49.784387 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/util.py
--rw-r--r--   0        0        0      483 2024-05-02 16:54:49.693120 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1819 2024-05-02 16:54:49.696999 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     2062 2024-05-02 16:54:49.702142 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1533 2024-05-02 16:54:49.699423 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-05-02 16:54:49.692702 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-05-02 16:54:49.697276 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0     1179 2024-05-02 16:54:49.694652 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/model.py
--rw-r--r--   0        0        0     1368 2024-05-02 16:54:49.703985 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.724238 patent_client-5.0.1/patent_client/_sync/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5746 2024-05-02 16:55:55.949498 patent_client-5.0.1/patent_client/_sync/epo/ops/published/api.py
--rw-r--r--   0        0        0     2878 2024-05-02 16:55:55.949751 patent_client-5.0.1/patent_client/_sync/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1917 2024-05-02 16:54:49.726807 patent_client-5.0.1/patent_client/_sync/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.780449 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-02 16:55:18.406245 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-05-02 16:54:49.779487 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-05-02 16:54:49.779804 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-02 16:55:18.590618 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18448 2024-05-02 16:55:18.792704 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3516 2024-05-02 16:54:49.745375 patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2383 2024-05-02 16:55:55.949242 patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      737 2024-05-02 16:54:49.766843 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-02 16:54:49.771074 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1466 2024-05-02 16:54:49.778409 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2500 2024-05-02 16:54:49.774783 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/images.py
--rw-r--r--   0        0        0     1259 2024-05-02 16:54:49.776390 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      701 2024-05-02 16:54:49.753627 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     4378 2024-05-02 16:54:49.760006 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0     1290 2024-05-02 16:54:49.765780 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     2084 2024-05-02 16:54:49.762883 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0     1066 2024-05-02 16:54:49.764083 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3609 2024-05-02 16:54:49.724096 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-05-02 16:54:49.746815 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-05-02 16:54:49.747751 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-05-02 16:54:49.747456 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-05-02 16:54:49.747138 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-02 16:55:22.225396 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-05-02 16:54:49.749328 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-02 16:55:22.229990 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-05-02 16:54:49.748436 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-05-02 16:54:49.746102 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-05-02 16:54:49.750694 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-05-02 16:54:49.750054 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-05-02 16:54:49.751835 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.752720 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-05-02 16:54:49.751111 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-05-02 16:54:49.751285 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-05-02 16:54:49.751611 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-05-02 16:54:49.750350 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-05-02 16:54:49.749720 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-05-02 16:54:49.752544 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-05-02 16:54:49.745766 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-05-02 16:54:49.748069 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-05-02 16:54:49.749004 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3872 2024-05-02 16:54:49.691686 patent_client-5.0.1/patent_client/_sync/epo/ops/session.py
--rw-r--r--   0        0        0     3129 2024-05-02 16:55:55.949894 patent_client-5.0.1/patent_client/_sync/epo/ops/util.py
--rw-r--r--   0        0        0     3611 2024-05-02 16:54:49.271384 patent_client-5.0.1/patent_client/_sync/http_client.py
--rw-r--r--   0        0        0      616 2024-05-02 16:54:49.274025 patent_client-5.0.1/patent_client/_sync/odp.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.274313 patent_client-5.0.1/patent_client/_sync/uspto/__init__.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.422160 patent_client-5.0.1/patent_client/_sync/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2936 2024-05-02 16:54:49.435281 patent_client-5.0.1/patent_client/_sync/uspto/assignment/api.py
--rw-r--r--   0        0        0     1273 2024-05-02 16:54:49.436962 patent_client-5.0.1/patent_client/_sync/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     4049 2024-05-02 16:54:49.422016 patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1565 2024-05-02 16:54:49.439130 patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-05-02 16:54:49.448163 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-05-02 16:54:49.448757 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-05-02 16:54:49.445263 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-05-02 16:54:49.446731 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-05-02 16:54:49.446163 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-05-02 16:54:49.447858 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3826 2024-05-02 16:54:49.444752 patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4308 2024-05-02 16:54:49.413378 patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5910 2024-05-02 16:54:49.431060 patent_client-5.0.1/patent_client/_sync/uspto/assignment/model.py
--rw-r--r--   0        0        0     2348 2024-05-02 16:54:49.416385 patent_client-5.0.1/patent_client/_sync/uspto/assignment/model_test.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.277934 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3593 2024-05-02 16:54:49.286527 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1382 2024-05-02 16:54:49.288731 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     3113 2024-05-02 16:54:49.293522 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1963 2024-05-02 16:54:49.277782 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1971 2024-05-02 16:54:49.280906 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/model.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.620966 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2446 2024-05-02 16:54:49.635557 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1463 2024-05-02 16:54:49.637862 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-05-02 16:54:49.620829 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     2272 2024-05-02 16:54:49.641199 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7354 2024-05-02 16:54:49.632107 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3853 2024-05-02 16:54:49.602482 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6479 2024-05-02 16:54:49.620511 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5668 2024-05-02 16:54:49.611314 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-05-02 16:54:49.641637 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-05-02 16:54:49.642377 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-05-02 16:54:49.642679 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-05-02 16:54:49.642129 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      417 2024-05-02 16:54:49.474650 patent_client-5.0.1/patent_client/_sync/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5786 2024-05-02 16:54:49.507980 patent_client-5.0.1/patent_client/_sync/uspto/odp/api.py
--rw-r--r--   0        0        0     2898 2024-05-02 16:54:49.512417 patent_client-5.0.1/patent_client/_sync/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-05-02 16:54:49.523098 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-05-02 16:54:49.524963 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-05-02 16:54:49.522829 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-05-02 16:54:49.524478 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-05-02 16:54:49.522678 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-05-02 16:54:49.520625 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-05-02 16:54:49.523412 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-05-02 16:54:49.525169 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-05-02 16:54:49.520959 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-05-02 16:54:49.522498 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-05-02 16:54:49.523715 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     5053 2024-05-02 16:54:49.520104 patent_client-5.0.1/patent_client/_sync/uspto/odp/manager.py
--rw-r--r--   0        0        0     2025 2024-05-02 16:54:49.451871 patent_client-5.0.1/patent_client/_sync/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16610 2024-05-02 16:54:49.499830 patent_client-5.0.1/patent_client/_sync/uspto/odp/model.py
--rw-r--r--   0        0        0    12669 2024-05-02 16:54:49.469166 patent_client-5.0.1/patent_client/_sync/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2812 2024-05-02 16:54:49.473108 patent_client-5.0.1/patent_client/_sync/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-05-02 16:54:49.474462 patent_client-5.0.1/patent_client/_sync/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      891 2024-05-02 16:54:49.474154 patent_client-5.0.1/patent_client/_sync/uspto/odp/util.py
--rw-r--r--   0        0        0      548 2024-05-02 16:54:49.549313 patent_client-5.0.1/patent_client/_sync/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4838 2024-05-02 16:54:49.579007 patent_client-5.0.1/patent_client/_sync/uspto/peds/api.py
--rw-r--r--   0        0        0     1031 2024-05-02 16:54:49.580486 patent_client-5.0.1/patent_client/_sync/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-05-02 16:54:49.595544 patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8585 2024-05-02 16:54:49.594371 patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8814 2024-05-02 16:54:49.593537 patent_client-5.0.1/patent_client/_sync/uspto/peds/manager.py
--rw-r--r--   0        0        0     9448 2024-05-02 16:54:49.539641 patent_client-5.0.1/patent_client/_sync/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    15332 2024-05-02 16:54:49.571891 patent_client-5.0.1/patent_client/_sync/uspto/peds/model.py
--rw-r--r--   0        0        0     6532 2024-05-02 16:54:49.548772 patent_client-5.0.1/patent_client/_sync/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-05-02 16:54:49.540007 patent_client-5.0.1/patent_client/_sync/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      604 2024-05-02 16:54:49.647690 patent_client-5.0.1/patent_client/_sync/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10579 2024-05-02 16:54:49.674786 patent_client-5.0.1/patent_client/_sync/uspto/ptab/api.py
--rw-r--r--   0        0        0     1021 2024-05-02 16:54:49.676210 patent_client-5.0.1/patent_client/_sync/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-05-02 16:54:49.680173 patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-05-02 16:54:49.680705 patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2467 2024-05-02 16:54:49.679688 patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2415 2024-05-02 16:54:49.646348 patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8762 2024-05-02 16:54:49.660127 patent_client-5.0.1/patent_client/_sync/uspto/ptab/model.py
--rw-r--r--   0        0        0      658 2024-05-02 16:54:49.647071 patent_client-5.0.1/patent_client/_sync/uspto/ptab/util.py
--rw-r--r--   0        0        0      742 2024-05-02 16:54:49.325197 patent_client-5.0.1/patent_client/_sync/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6952 2024-05-02 16:54:49.335229 patent_client-5.0.1/patent_client/_sync/uspto/public_search/api.py
--rw-r--r--   0        0        0      682 2024-05-02 16:54:49.335976 patent_client-5.0.1/patent_client/_sync/uspto/public_search/api_test.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.389789 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2482 2024-05-02 16:54:49.394364 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     7094 2024-05-02 16:54:49.407282 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     2010 2024-05-02 16:54:49.396701 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1451 2024-05-02 16:54:49.337751 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-05-02 16:54:49.324277 patent_client-5.0.1/patent_client/_sync/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-05-02 16:54:49.379455 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-05-02 16:54:49.385172 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-05-02 16:54:49.389523 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-05-02 16:54:49.387433 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-02 16:55:24.352861 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-05-02 16:54:49.370527 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4487 2024-05-02 16:54:49.344979 patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7339 2024-05-02 16:54:49.306132 patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      940 2024-05-02 16:54:49.346685 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3548 2024-05-02 16:54:49.351720 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7978 2024-05-02 16:54:49.367308 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2665 2024-05-02 16:54:49.355383 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1951 2024-05-02 16:54:49.308937 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4936 2024-05-02 16:54:49.323048 patent_client-5.0.1/patent_client/_sync/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-05-02 16:54:49.293946 patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4729 2024-05-02 16:54:49.316153 patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-05-02 16:54:49.345205 patent_client-5.0.1/patent_client/_sync/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      689 2024-05-02 16:54:49.323888 patent_client-5.0.1/patent_client/_sync/uspto/public_search/util.py
--rw-r--r--   0        0        0     6043 2024-05-01 18:05:48.009638 patent_client-5.0.1/patent_client/parser.py
--rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.1/patent_client/patches.py
--rw-r--r--   0        0        0     3276 2024-05-01 18:37:20.358790 patent_client-5.0.1/patent_client/session.py
--rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.1/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.1/patent_client/test_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.1/patent_client/util/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.1/patent_client/util/asyncio_util.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.1/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4313 2024-05-02 16:55:25.224279 patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6924 2024-05-02 16:55:25.227038 patent_client-5.0.1/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.1/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      735 2024-05-01 18:11:58.857909 patent_client-5.0.1/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3554 2024-05-01 18:11:58.857956 patent_client-5.0.1/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.1/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.1/patent_client/util/format.py
--rw-r--r--   0        0        0     9728 2024-05-02 16:55:55.950403 patent_client-5.0.1/patent_client/util/manager.py
--rw-r--r--   0        0        0     3035 2024-05-01 18:29:51.038167 patent_client-5.0.1/patent_client/util/pydantic_util.py
--rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.1/patent_client/util/request_util.py
--rw-r--r--   0        0        0     1255 2024-05-01 18:11:58.858129 patent_client-5.0.1/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2024-05-02 16:56:44.518693 patent_client-5.0.1/patent_client/version.py
--rw-r--r--   0        0        0     3376 2024-05-02 16:56:44.518941 patent_client-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.2/LICENSE
+-rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.2/README.md
+-rw-r--r--   0        0        0     1745 2024-05-02 17:06:23.121142 patent_client-5.0.2/patent_client/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.2/patent_client/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.2/patent_client/_async/epo/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.2/patent_client/_async/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.2/patent_client/_async/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      384 2024-05-02 17:06:23.121519 patent_client-5.0.2/patent_client/_async/epo/ops/family/api.py
+-rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.2/patent_client/_async/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      378 2024-05-01 18:05:47.952110 patent_client-5.0.2/patent_client/_async/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.2/patent_client/_async/epo/ops/family/model.py
+-rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.2/patent_client/_async/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1545 2024-05-01 18:05:47.953175 patent_client-5.0.2/patent_client/_async/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.2/patent_client/_async/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.2/patent_client/_async/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.2/patent_client/_async/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.2/patent_client/_async/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      489 2024-05-01 18:05:47.953918 patent_client-5.0.2/patent_client/_async/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.2/patent_client/_async/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5612 2024-05-02 17:06:46.489006 patent_client-5.0.2/patent_client/_async/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.2/patent_client/_async/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4062 2024-05-01 18:05:47.954735 patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.2/patent_client/_async/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.2/patent_client/_async/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5542 2024-05-02 17:06:23.125728 patent_client-5.0.2/patent_client/_async/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2743 2024-05-02 17:06:23.130061 patent_client-5.0.2/patent_client/_async/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.2/patent_client/_async/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-02 17:06:56.113096 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-02 17:06:56.116587 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-02 17:06:56.126129 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3226 2024-05-02 17:06:23.135401 patent_client-5.0.2/patent_client/_async/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2433 2024-05-02 17:06:23.135622 patent_client-5.0.2/patent_client/_async/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2108 2024-05-02 17:06:23.135755 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3962 2024-05-01 18:05:47.958633 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1668 2024-05-01 18:05:47.959251 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3193 2024-05-01 18:16:57.840152 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-02 17:06:56.258594 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-02 17:06:56.262521 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3478 2024-05-02 17:06:23.136036 patent_client-5.0.2/patent_client/_async/epo/ops/session.py
+-rw-r--r--   0        0        0     2881 2024-05-02 17:06:23.136269 patent_client-5.0.2/patent_client/_async/epo/ops/util.py
+-rw-r--r--   0        0        0     3234 2024-05-02 17:06:23.136731 patent_client-5.0.2/patent_client/_async/http_client.py
+-rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.2/patent_client/_async/odp.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.2/patent_client/_async/uspto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.2/patent_client/_async/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-01 18:05:47.961041 patent_client-5.0.2/patent_client/_async/uspto/assignment/api.py
+-rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.2/patent_client/_async/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     3633 2024-05-01 18:05:47.961566 patent_client-5.0.2/patent_client/_async/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.2/patent_client/_async/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3454 2024-05-02 17:06:23.137674 patent_client-5.0.2/patent_client/_async/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4202 2024-05-02 17:06:23.137868 patent_client-5.0.2/patent_client/_async/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5506 2024-05-02 17:06:23.138191 patent_client-5.0.2/patent_client/_async/uspto/assignment/model.py
+-rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.2/patent_client/_async/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3226 2024-05-02 17:06:23.138458 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1567 2024-05-02 17:06:23.138855 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1902 2024-05-01 18:05:47.969601 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7111 2024-05-02 17:06:23.183391 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6063 2024-05-01 18:05:47.970370 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.2/patent_client/_async/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5502 2024-05-02 17:06:23.183737 patent_client-5.0.2/patent_client/_async/uspto/odp/api.py
+-rw-r--r--   0        0        0     2834 2024-05-01 18:05:47.971502 patent_client-5.0.2/patent_client/_async/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     4834 2024-05-02 17:06:23.185321 patent_client-5.0.2/patent_client/_async/uspto/odp/manager.py
+-rw-r--r--   0        0        0     1895 2024-05-02 17:06:23.185692 patent_client-5.0.2/patent_client/_async/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16427 2024-05-02 17:06:23.185851 patent_client-5.0.2/patent_client/_async/uspto/odp/model.py
+-rw-r--r--   0        0        0    12253 2024-05-01 18:05:47.972423 patent_client-5.0.2/patent_client/_async/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.2/patent_client/_async/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.2/patent_client/_async/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.2/patent_client/_async/uspto/odp/util.py
+-rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.2/patent_client/_async/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.2/patent_client/_async/uspto/peds/api.py
+-rw-r--r--   0        0        0      711 2024-05-01 18:05:47.973610 patent_client-5.0.2/patent_client/_async/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8585 2024-05-02 17:06:23.208841 patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8495 2024-05-02 17:06:23.209133 patent_client-5.0.2/patent_client/_async/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9726 2024-05-02 17:06:23.209568 patent_client-5.0.2/patent_client/_async/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    14987 2024-05-02 17:06:23.209910 patent_client-5.0.2/patent_client/_async/uspto/peds/model.py
+-rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.2/patent_client/_async/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.2/patent_client/_async/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.2/patent_client/_async/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10200 2024-05-01 18:05:47.974861 patent_client-5.0.2/patent_client/_async/uspto/ptab/api.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.2/patent_client/_async/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2085 2024-05-01 18:05:47.975042 patent_client-5.0.2/patent_client/_async/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2311 2024-05-01 18:05:47.975211 patent_client-5.0.2/patent_client/_async/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8358 2024-05-02 17:06:23.210296 patent_client-5.0.2/patent_client/_async/uspto/ptab/model.py
+-rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.2/patent_client/_async/uspto/ptab/util.py
+-rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.2/patent_client/_async/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6701 2024-05-02 17:06:23.211019 patent_client-5.0.2/patent_client/_async/uspto/public_search/api.py
+-rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.2/patent_client/_async/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6678 2024-05-01 18:05:47.983341 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.2/patent_client/_async/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-02 17:06:58.457561 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4144 2024-05-01 18:05:47.983936 patent_client-5.0.2/patent_client/_async/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7743 2024-05-01 18:05:47.984232 patent_client-5.0.2/patent_client/_async/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      524 2024-05-02 17:06:23.211324 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3144 2024-05-01 18:16:57.840869 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7574 2024-05-01 18:05:47.984820 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2249 2024-05-01 18:05:47.984983 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.2/patent_client/_async/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4520 2024-05-01 18:05:47.985447 patent_client-5.0.2/patent_client/_async/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.2/patent_client/_async/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4313 2024-05-02 17:06:23.211633 patent_client-5.0.2/patent_client/_async/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.2/patent_client/_async/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.2/patent_client/_async/uspto/public_search/util.py
+-rw-r--r--   0        0        0     1249 2024-05-02 17:06:23.211793 patent_client-5.0.2/patent_client/_sync/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.680949 patent_client-5.0.2/patent_client/_sync/epo/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-02 16:54:49.692358 patent_client-5.0.2/patent_client/_sync/epo/ops/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.706525 patent_client-5.0.2/patent_client/_sync/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-02 17:06:23.212028 patent_client-5.0.2/patent_client/_sync/epo/ops/family/api.py
+-rw-r--r--   0        0        0      855 2024-05-02 16:54:49.710444 patent_client-5.0.2/patent_client/_sync/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714131 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-05-02 16:54:49.714466 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-05-02 16:54:49.714990 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714682 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      772 2024-05-02 16:54:49.711289 patent_client-5.0.2/patent_client/_sync/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1535 2024-05-02 16:54:49.708518 patent_client-5.0.2/patent_client/_sync/epo/ops/family/model.py
+-rw-r--r--   0        0        0      903 2024-05-02 16:54:49.705264 patent_client-5.0.2/patent_client/_sync/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1961 2024-05-02 16:54:49.713729 patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      943 2024-05-02 16:54:49.706394 patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.784538 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-02 17:06:23.212774 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      704 2024-05-02 16:54:49.799011 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-05-02 16:54:49.811517 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-05-02 16:54:49.808791 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-05-02 16:54:49.811216 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-05-02 16:54:49.810170 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-05-02 16:54:49.810402 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-05-02 16:54:49.810723 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-05-02 16:54:49.808401 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      883 2024-05-02 16:54:49.800072 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2791 2024-05-02 16:54:49.788392 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5908 2024-05-02 17:06:23.223493 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      882 2024-05-02 16:54:49.781664 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4478 2024-05-02 16:54:49.806767 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1632 2024-05-02 16:54:49.783877 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      530 2024-05-02 16:54:49.784387 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/util.py
+-rw-r--r--   0        0        0      483 2024-05-02 16:54:49.693120 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1819 2024-05-02 17:06:23.225101 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     2062 2024-05-02 16:54:49.702142 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1533 2024-05-02 16:54:49.699423 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-05-02 16:54:49.692702 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-05-02 16:54:49.697276 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0     1179 2024-05-02 16:54:49.694652 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0     1368 2024-05-02 16:54:49.703985 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.724238 patent_client-5.0.2/patent_client/_sync/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5746 2024-05-02 17:06:23.227644 patent_client-5.0.2/patent_client/_sync/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2878 2024-05-02 17:06:23.227876 patent_client-5.0.2/patent_client/_sync/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1917 2024-05-02 16:54:49.726807 patent_client-5.0.2/patent_client/_sync/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.780449 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-02 17:07:15.825147 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-05-02 16:54:49.779487 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-05-02 16:54:49.779804 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-02 17:07:15.827972 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18448 2024-05-02 17:07:15.837709 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3516 2024-05-02 17:06:23.236789 patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2383 2024-05-02 17:06:23.237053 patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      737 2024-05-02 16:54:49.766843 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-02 16:54:49.771074 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1466 2024-05-02 16:54:49.778409 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2500 2024-05-02 16:54:49.774783 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0     1259 2024-05-02 16:54:49.776390 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      701 2024-05-02 16:54:49.753627 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     4378 2024-05-02 16:54:49.760006 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0     1290 2024-05-02 16:54:49.765780 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     2084 2024-05-02 16:54:49.762883 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0     1066 2024-05-02 16:54:49.764083 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3609 2024-05-02 16:54:49.724096 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-05-02 16:54:49.746815 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-05-02 16:54:49.747751 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-05-02 16:54:49.747456 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-05-02 16:54:49.747138 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-02 17:07:16.001415 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-05-02 16:54:49.749328 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-02 17:07:16.005271 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-05-02 16:54:49.748436 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-05-02 16:54:49.746102 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-05-02 16:54:49.750694 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-05-02 16:54:49.750054 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-05-02 16:54:49.751835 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.752720 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-05-02 16:54:49.751111 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-05-02 16:54:49.751285 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-05-02 16:54:49.751611 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-05-02 16:54:49.750350 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-05-02 16:54:49.749720 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-05-02 16:54:49.752544 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-05-02 16:54:49.745766 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-05-02 16:54:49.748069 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-05-02 16:54:49.749004 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3872 2024-05-02 17:06:23.237251 patent_client-5.0.2/patent_client/_sync/epo/ops/session.py
+-rw-r--r--   0        0        0     3129 2024-05-02 17:06:23.237454 patent_client-5.0.2/patent_client/_sync/epo/ops/util.py
+-rw-r--r--   0        0        0     3611 2024-05-02 17:06:23.237646 patent_client-5.0.2/patent_client/_sync/http_client.py
+-rw-r--r--   0        0        0      616 2024-05-02 17:06:23.238055 patent_client-5.0.2/patent_client/_sync/odp.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.274313 patent_client-5.0.2/patent_client/_sync/uspto/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.422160 patent_client-5.0.2/patent_client/_sync/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2936 2024-05-02 16:54:49.435281 patent_client-5.0.2/patent_client/_sync/uspto/assignment/api.py
+-rw-r--r--   0        0        0     1273 2024-05-02 17:06:23.238245 patent_client-5.0.2/patent_client/_sync/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     4049 2024-05-02 16:54:49.422016 patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1565 2024-05-02 16:54:49.439130 patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-05-02 16:54:49.448163 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-05-02 16:54:49.448757 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-05-02 16:54:49.445263 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-05-02 16:54:49.446731 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-05-02 16:54:49.446163 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-05-02 16:54:49.447858 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3826 2024-05-02 17:06:23.250231 patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4308 2024-05-02 17:06:23.251951 patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5910 2024-05-02 17:06:23.253634 patent_client-5.0.2/patent_client/_sync/uspto/assignment/model.py
+-rw-r--r--   0        0        0     2348 2024-05-02 16:54:49.416385 patent_client-5.0.2/patent_client/_sync/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.277934 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3593 2024-05-02 17:06:23.253879 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1382 2024-05-02 16:54:49.288731 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     3113 2024-05-02 16:54:49.293522 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1963 2024-05-02 16:54:49.277782 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1971 2024-05-02 17:06:23.256609 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.620966 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2446 2024-05-02 16:54:49.635557 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1463 2024-05-02 16:54:49.637862 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-05-02 16:54:49.620829 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     2272 2024-05-02 16:54:49.641199 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7354 2024-05-02 17:06:23.295181 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3853 2024-05-02 16:54:49.602482 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6479 2024-05-02 16:54:49.620511 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5668 2024-05-02 16:54:49.611314 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-05-02 16:54:49.641637 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-05-02 16:54:49.642377 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-05-02 16:54:49.642679 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-05-02 16:54:49.642129 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      417 2024-05-02 16:54:49.474650 patent_client-5.0.2/patent_client/_sync/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5786 2024-05-02 17:06:23.296817 patent_client-5.0.2/patent_client/_sync/uspto/odp/api.py
+-rw-r--r--   0        0        0     2898 2024-05-02 16:54:49.512417 patent_client-5.0.2/patent_client/_sync/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-05-02 16:54:49.523098 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-05-02 16:54:49.524963 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-05-02 16:54:49.522829 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-05-02 16:54:49.524478 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-05-02 16:54:49.522678 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-05-02 16:54:49.520625 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-05-02 16:54:49.523412 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-05-02 16:54:49.525169 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-05-02 16:54:49.520959 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-05-02 16:54:49.522498 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-05-02 16:54:49.523715 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5053 2024-05-02 17:06:23.306387 patent_client-5.0.2/patent_client/_sync/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2025 2024-05-02 17:06:23.306557 patent_client-5.0.2/patent_client/_sync/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16610 2024-05-02 17:06:23.306733 patent_client-5.0.2/patent_client/_sync/uspto/odp/model.py
+-rw-r--r--   0        0        0    12669 2024-05-02 16:54:49.469166 patent_client-5.0.2/patent_client/_sync/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2812 2024-05-02 16:54:49.473108 patent_client-5.0.2/patent_client/_sync/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-05-02 16:54:49.474462 patent_client-5.0.2/patent_client/_sync/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      891 2024-05-02 16:54:49.474154 patent_client-5.0.2/patent_client/_sync/uspto/odp/util.py
+-rw-r--r--   0        0        0      548 2024-05-02 16:54:49.549313 patent_client-5.0.2/patent_client/_sync/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4838 2024-05-02 16:54:49.579007 patent_client-5.0.2/patent_client/_sync/uspto/peds/api.py
+-rw-r--r--   0        0        0     1031 2024-05-02 16:54:49.580486 patent_client-5.0.2/patent_client/_sync/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-05-02 16:54:49.595544 patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8585 2024-05-02 17:06:23.327094 patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8814 2024-05-02 17:06:23.328428 patent_client-5.0.2/patent_client/_sync/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9448 2024-05-02 17:06:23.330140 patent_client-5.0.2/patent_client/_sync/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    15332 2024-05-02 17:06:23.330325 patent_client-5.0.2/patent_client/_sync/uspto/peds/model.py
+-rw-r--r--   0        0        0     6532 2024-05-02 16:54:49.548772 patent_client-5.0.2/patent_client/_sync/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-05-02 16:54:49.540007 patent_client-5.0.2/patent_client/_sync/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      604 2024-05-02 17:06:23.330644 patent_client-5.0.2/patent_client/_sync/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10579 2024-05-02 16:54:49.674786 patent_client-5.0.2/patent_client/_sync/uspto/ptab/api.py
+-rw-r--r--   0        0        0     1021 2024-05-02 16:54:49.676210 patent_client-5.0.2/patent_client/_sync/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-05-02 16:54:49.680173 patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-05-02 16:54:49.680705 patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2467 2024-05-02 16:54:49.679688 patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2415 2024-05-02 16:54:49.646348 patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8762 2024-05-02 17:06:23.333231 patent_client-5.0.2/patent_client/_sync/uspto/ptab/model.py
+-rw-r--r--   0        0        0      658 2024-05-02 16:54:49.647071 patent_client-5.0.2/patent_client/_sync/uspto/ptab/util.py
+-rw-r--r--   0        0        0      742 2024-05-02 17:06:23.333548 patent_client-5.0.2/patent_client/_sync/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6952 2024-05-02 17:06:23.333795 patent_client-5.0.2/patent_client/_sync/uspto/public_search/api.py
+-rw-r--r--   0        0        0      682 2024-05-02 16:54:49.335976 patent_client-5.0.2/patent_client/_sync/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.389789 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-02 16:54:49.394364 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     7094 2024-05-02 16:54:49.407282 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     2010 2024-05-02 16:54:49.396701 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1451 2024-05-02 17:06:23.352623 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-05-02 16:54:49.324277 patent_client-5.0.2/patent_client/_sync/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-05-02 16:54:49.379455 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-05-02 16:54:49.385172 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-05-02 16:54:49.389523 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-05-02 16:54:49.387433 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-02 17:07:18.152251 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-05-02 16:54:49.370527 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4487 2024-05-02 16:54:49.344979 patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7339 2024-05-02 16:54:49.306132 patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      940 2024-05-02 17:06:23.354093 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3548 2024-05-02 16:54:49.351720 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7978 2024-05-02 16:54:49.367308 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2665 2024-05-02 16:54:49.355383 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1951 2024-05-02 17:06:23.355657 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4936 2024-05-02 16:54:49.323048 patent_client-5.0.2/patent_client/_sync/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-05-02 16:54:49.293946 patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4729 2024-05-02 17:06:23.355939 patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-05-02 16:54:49.345205 patent_client-5.0.2/patent_client/_sync/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      689 2024-05-02 16:54:49.323888 patent_client-5.0.2/patent_client/_sync/uspto/public_search/util.py
+-rw-r--r--   0        0        0     6043 2024-05-01 18:05:48.009638 patent_client-5.0.2/patent_client/parser.py
+-rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.2/patent_client/patches.py
+-rw-r--r--   0        0        0     3276 2024-05-02 17:06:23.356172 patent_client-5.0.2/patent_client/session.py
+-rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.2/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.2/patent_client/test_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.2/patent_client/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.2/patent_client/util/asyncio_util.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.2/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4313 2024-05-02 17:07:19.017614 patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6924 2024-05-02 17:07:19.020230 patent_client-5.0.2/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.2/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.2/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3554 2024-05-02 17:06:23.356557 patent_client-5.0.2/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.2/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.2/patent_client/util/format.py
+-rw-r--r--   0        0        0     9728 2024-05-02 17:06:23.356944 patent_client-5.0.2/patent_client/util/manager.py
+-rw-r--r--   0        0        0     3035 2024-05-02 17:06:23.357203 patent_client-5.0.2/patent_client/util/pydantic_util.py
+-rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.2/patent_client/util/request_util.py
+-rw-r--r--   0        0        0     1255 2024-05-02 17:06:23.357370 patent_client-5.0.2/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2024-05-02 17:10:12.308623 patent_client-5.0.2/patent_client/version.py
+-rw-r--r--   0        0        0     3376 2024-05-02 17:10:12.308856 patent_client-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.2/PKG-INFO
```

### Comparing `patent_client-5.0.1/LICENSE` & `patent_client-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/README.md` & `patent_client-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/__init__.py` & `patent_client-5.0.2/patent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/__init__.py` & `patent_client-5.0.2/patent_client/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/model.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/model_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/schema.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/family/schema_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/model.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/national_codes.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/national_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     date, excel_url = await get_spreadsheet_from_epo_website()
     out_path = (
         legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
     )
     if out_path.exists():
         logger.info(f"File already downloaded! Current as of {date.isoformat()}")
         return out_path
-    out_path = session.download(excel_url, path=out_path)
+    out_path = await session.download(excel_url, path=out_path)
     logger.info(f"Downloaded new live code file for date {date.isoformat()}")
     return out_path
 
 
 def create_code_database(excel_path):
     con = sqlite3.connect(db_location, timeout=30)
     cur = con.cursor()
@@ -115,14 +115,15 @@
     cur.execute("INSERT INTO meta values (?)", (excel_path.name,))
     wb = load_workbook(excel_path)
     data = list(
         tuple(i.strip() for i in r)
         for r in wb[wb.sheetnames[0]].iter_rows(values_only=True)
     )
     rows = data[1:]
+    cur.execute("DROP TABLE IF EXISTS legal_codes")
     cur.execute(
         """CREATE TABLE IF NOT EXISTS legal_codes (
     country_code text,
     event_code text,
     date_created text,
     influence text,
     description text,
```

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.txt` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/messages.txt` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/model.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/schema.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/api.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/api_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/cql.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/manager.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/manager_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/biblio.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/fulltext.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/images.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/search.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/biblio.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/images.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/search.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema_test.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/description_example.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/image_example.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/search_example.xml` & `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/session.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/epo/ops/util.py` & `patent_client-5.0.2/patent_client/_async/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/http_client.py` & `patent_client-5.0.2/patent_client/_async/http_client.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/api_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/convert.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/convert_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/manager_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/model.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/assignment/model_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/model.py` & `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app.json` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/api_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/application.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/documents.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/search.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/manager_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/model.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/model_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/query.py` & `patent_client-5.0.2/patent_client/_async/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/odp/query_fields.csv` & `patent_client-5.0.2/patent_client/_async/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/api_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/manager_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/model.py` & `patent_client-5.0.2/patent_client/_async/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/query.py` & `patent_client-5.0.2/patent_client/_async/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/peds/search_index.csv` & `patent_client-5.0.2/patent_client/_async/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/api_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/manager_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/ptab/model.py` & `patent_client-5.0.2/patent_client/_async/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/api.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/biblio.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/document.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/shared.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/count_query.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/manager.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/manager_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/__init__.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/biblio.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/document.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/shared.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/model_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/query.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/query_config.csv` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/query_test.py` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_async/uspto/public_search/search_query.json` & `patent_client-5.0.2/patent_client/_async/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/__init__.py` & `patent_client-5.0.2/patent_client/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/__init__.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/api.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/api_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/manager.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/model.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/model_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/manager.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/model.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/util.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.txt` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/messages.txt` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/model.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/schema.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/api.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/api_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/cql.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/__init__.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/biblio.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/fulltext.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/images.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/search.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/__init__.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/biblio.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/images.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/search.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema_test.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/description_example.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/image_example.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/search_example.xml` & `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/session.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/epo/ops/util.py` & `patent_client-5.0.2/patent_client/_sync/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/http_client.py` & `patent_client-5.0.2/patent_client/_sync/http_client.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/odp.py` & `patent_client-5.0.2/patent_client/_sync/odp.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/model.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/assignment/model_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/model.py` & `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app.json` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/application.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/documents.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/search.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/model.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/model_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/query.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/query_fields.csv` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/odp/util.py` & `patent_client-5.0.2/patent_client/_sync/uspto/odp/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/__init__.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/model.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/query.py` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/peds/search_index.csv` & `patent_client-5.0.2/patent_client/_sync/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/__init__.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/model.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/ptab/util.py` & `patent_client-5.0.2/patent_client/_sync/uspto/ptab/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/__init__.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/api.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/api_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/biblio.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/document.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/shared.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/count_query.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/__init__.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/biblio.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/document.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/shared.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/query.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_config.csv` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_test.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/search_query.json` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/_sync/uspto/public_search/util.py` & `patent_client-5.0.2/patent_client/_sync/uspto/public_search/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/parser.py` & `patent_client-5.0.2/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/session.py` & `patent_client-5.0.2/patent_client/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/settings.py` & `patent_client-5.0.2/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/test_parser.py` & `patent_client-5.0.2/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/asyncio_util.py` & `patent_client-5.0.2/patent_client/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/examples/published_claims.json` & `patent_client-5.0.2/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/examples/published_claims.txt` & `patent_client-5.0.2/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/model.py` & `patent_client-5.0.2/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/parser.py` & `patent_client-5.0.2/patent_client/util/claims/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/claims/parser_test.py` & `patent_client-5.0.2/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/format.py` & `patent_client-5.0.2/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/manager.py` & `patent_client-5.0.2/patent_client/util/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/pydantic_util.py` & `patent_client-5.0.2/patent_client/util/pydantic_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/request_util.py` & `patent_client-5.0.2/patent_client/util/request_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/patent_client/util/test.py` & `patent_client-5.0.2/patent_client/util/test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.1/pyproject.toml` & `patent_client-5.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "5.0.1"
+version = "5.0.2"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
```

### Comparing `patent_client-5.0.1/PKG-INFO` & `patent_client-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 5.0.1
+Version: 5.0.2
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
```

