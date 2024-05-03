# Comparing `tmp/patent_client-5.0.2.tar.gz` & `tmp/patent_client-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-5.0.2.tar", max compression
+gzip compressed data, was "patent_client-5.0.3.tar", max compression
```

## Comparing `patent_client-5.0.2.tar` & `patent_client-5.0.3.tar`

### file list

```diff
@@ -1,408 +1,408 @@
--rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.2/LICENSE
--rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.2/README.md
--rw-r--r--   0        0        0     1745 2024-05-02 17:06:23.121142 patent_client-5.0.2/patent_client/__init__.py
--rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.2/patent_client/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.2/patent_client/_async/epo/__init__.py
--rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.2/patent_client/_async/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.2/patent_client/_async/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      384 2024-05-02 17:06:23.121519 patent_client-5.0.2/patent_client/_async/epo/ops/family/api.py
--rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.2/patent_client/_async/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      378 2024-05-01 18:05:47.952110 patent_client-5.0.2/patent_client/_async/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.2/patent_client/_async/epo/ops/family/model.py
--rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.2/patent_client/_async/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1545 2024-05-01 18:05:47.953175 patent_client-5.0.2/patent_client/_async/epo/ops/family/schema.py
--rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.2/patent_client/_async/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.2/patent_client/_async/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.2/patent_client/_async/epo/ops/legal/api.py
--rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.2/patent_client/_async/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      489 2024-05-01 18:05:47.953918 patent_client-5.0.2/patent_client/_async/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.2/patent_client/_async/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5612 2024-05-02 17:06:46.489006 patent_client-5.0.2/patent_client/_async/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.2/patent_client/_async/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4062 2024-05-01 18:05:47.954735 patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.2/patent_client/_async/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.2/patent_client/_async/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.2/patent_client/_async/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5542 2024-05-02 17:06:23.125728 patent_client-5.0.2/patent_client/_async/epo/ops/published/api.py
--rw-r--r--   0        0        0     2743 2024-05-02 17:06:23.130061 patent_client-5.0.2/patent_client/_async/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.2/patent_client/_async/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-02 17:06:56.113096 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-02 17:06:56.116587 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-05-02 17:06:56.126129 patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3226 2024-05-02 17:06:23.135401 patent_client-5.0.2/patent_client/_async/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2433 2024-05-02 17:06:23.135622 patent_client-5.0.2/patent_client/_async/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2108 2024-05-02 17:06:23.135755 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.2/patent_client/_async/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3962 2024-05-01 18:05:47.958633 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1668 2024-05-01 18:05:47.959251 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3193 2024-05-01 18:16:57.840152 patent_client-5.0.2/patent_client/_async/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-02 17:06:56.258594 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-02 17:06:56.262521 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.2/patent_client/_async/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3478 2024-05-02 17:06:23.136036 patent_client-5.0.2/patent_client/_async/epo/ops/session.py
--rw-r--r--   0        0        0     2881 2024-05-02 17:06:23.136269 patent_client-5.0.2/patent_client/_async/epo/ops/util.py
--rw-r--r--   0        0        0     3234 2024-05-02 17:06:23.136731 patent_client-5.0.2/patent_client/_async/http_client.py
--rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.2/patent_client/_async/odp.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.2/patent_client/_async/uspto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.2/patent_client/_async/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2552 2024-05-01 18:05:47.961041 patent_client-5.0.2/patent_client/_async/uspto/assignment/api.py
--rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.2/patent_client/_async/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     3633 2024-05-01 18:05:47.961566 patent_client-5.0.2/patent_client/_async/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.2/patent_client/_async/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3454 2024-05-02 17:06:23.137674 patent_client-5.0.2/patent_client/_async/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4202 2024-05-02 17:06:23.137868 patent_client-5.0.2/patent_client/_async/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5506 2024-05-02 17:06:23.138191 patent_client-5.0.2/patent_client/_async/uspto/assignment/model.py
--rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.2/patent_client/_async/uspto/assignment/model_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3226 2024-05-02 17:06:23.138458 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1567 2024-05-02 17:06:23.138855 patent_client-5.0.2/patent_client/_async/uspto/bulk_data/model.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1902 2024-05-01 18:05:47.969601 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7111 2024-05-02 17:06:23.183391 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6063 2024-05-01 18:05:47.970370 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.2/patent_client/_async/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5502 2024-05-02 17:06:23.183737 patent_client-5.0.2/patent_client/_async/uspto/odp/api.py
--rw-r--r--   0        0        0     2834 2024-05-01 18:05:47.971502 patent_client-5.0.2/patent_client/_async/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     4834 2024-05-02 17:06:23.185321 patent_client-5.0.2/patent_client/_async/uspto/odp/manager.py
--rw-r--r--   0        0        0     1895 2024-05-02 17:06:23.185692 patent_client-5.0.2/patent_client/_async/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16427 2024-05-02 17:06:23.185851 patent_client-5.0.2/patent_client/_async/uspto/odp/model.py
--rw-r--r--   0        0        0    12253 2024-05-01 18:05:47.972423 patent_client-5.0.2/patent_client/_async/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.2/patent_client/_async/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.2/patent_client/_async/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.2/patent_client/_async/uspto/odp/util.py
--rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.2/patent_client/_async/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.2/patent_client/_async/uspto/peds/api.py
--rw-r--r--   0        0        0      711 2024-05-01 18:05:47.973610 patent_client-5.0.2/patent_client/_async/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8585 2024-05-02 17:06:23.208841 patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8495 2024-05-02 17:06:23.209133 patent_client-5.0.2/patent_client/_async/uspto/peds/manager.py
--rw-r--r--   0        0        0     9726 2024-05-02 17:06:23.209568 patent_client-5.0.2/patent_client/_async/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    14987 2024-05-02 17:06:23.209910 patent_client-5.0.2/patent_client/_async/uspto/peds/model.py
--rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.2/patent_client/_async/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.2/patent_client/_async/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.2/patent_client/_async/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10200 2024-05-01 18:05:47.974861 patent_client-5.0.2/patent_client/_async/uspto/ptab/api.py
--rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.2/patent_client/_async/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2085 2024-05-01 18:05:47.975042 patent_client-5.0.2/patent_client/_async/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2311 2024-05-01 18:05:47.975211 patent_client-5.0.2/patent_client/_async/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8358 2024-05-02 17:06:23.210296 patent_client-5.0.2/patent_client/_async/uspto/ptab/model.py
--rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.2/patent_client/_async/uspto/ptab/util.py
--rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.2/patent_client/_async/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6701 2024-05-02 17:06:23.211019 patent_client-5.0.2/patent_client/_async/uspto/public_search/api.py
--rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.2/patent_client/_async/uspto/public_search/api_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6678 2024-05-01 18:05:47.983341 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.2/patent_client/_async/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.2/patent_client/_async/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-02 17:06:58.457561 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4144 2024-05-01 18:05:47.983936 patent_client-5.0.2/patent_client/_async/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7743 2024-05-01 18:05:47.984232 patent_client-5.0.2/patent_client/_async/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      524 2024-05-02 17:06:23.211324 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3144 2024-05-01 18:16:57.840869 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7574 2024-05-01 18:05:47.984820 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2249 2024-05-01 18:05:47.984983 patent_client-5.0.2/patent_client/_async/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.2/patent_client/_async/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4520 2024-05-01 18:05:47.985447 patent_client-5.0.2/patent_client/_async/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.2/patent_client/_async/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4313 2024-05-02 17:06:23.211633 patent_client-5.0.2/patent_client/_async/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.2/patent_client/_async/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.2/patent_client/_async/uspto/public_search/util.py
--rw-r--r--   0        0        0     1249 2024-05-02 17:06:23.211793 patent_client-5.0.2/patent_client/_sync/__init__.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.680949 patent_client-5.0.2/patent_client/_sync/epo/__init__.py
--rw-r--r--   0        0        0      630 2024-05-02 16:54:49.692358 patent_client-5.0.2/patent_client/_sync/epo/ops/__init__.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.706525 patent_client-5.0.2/patent_client/_sync/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      788 2024-05-02 17:06:23.212028 patent_client-5.0.2/patent_client/_sync/epo/ops/family/api.py
--rw-r--r--   0        0        0      855 2024-05-02 16:54:49.710444 patent_client-5.0.2/patent_client/_sync/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714131 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-05-02 16:54:49.714466 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-05-02 16:54:49.714990 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714682 patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      772 2024-05-02 16:54:49.711289 patent_client-5.0.2/patent_client/_sync/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1535 2024-05-02 16:54:49.708518 patent_client-5.0.2/patent_client/_sync/epo/ops/family/model.py
--rw-r--r--   0        0        0      903 2024-05-02 16:54:49.705264 patent_client-5.0.2/patent_client/_sync/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1961 2024-05-02 16:54:49.713729 patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema.py
--rw-r--r--   0        0        0      943 2024-05-02 16:54:49.706394 patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.784538 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      763 2024-05-02 17:06:23.212774 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api.py
--rw-r--r--   0        0        0      704 2024-05-02 16:54:49.799011 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-05-02 16:54:49.811517 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-05-02 16:54:49.808791 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-05-02 16:54:49.811216 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-05-02 16:54:49.810170 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-05-02 16:54:49.810402 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-05-02 16:54:49.810723 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-05-02 16:54:49.808401 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      883 2024-05-02 16:54:49.800072 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2791 2024-05-02 16:54:49.788392 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5908 2024-05-02 17:06:23.223493 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      882 2024-05-02 16:54:49.781664 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4478 2024-05-02 16:54:49.806767 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1632 2024-05-02 16:54:49.783877 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      530 2024-05-02 16:54:49.784387 patent_client-5.0.2/patent_client/_sync/epo/ops/legal/util.py
--rw-r--r--   0        0        0      483 2024-05-02 16:54:49.693120 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1819 2024-05-02 17:06:23.225101 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     2062 2024-05-02 16:54:49.702142 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1533 2024-05-02 16:54:49.699423 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-05-02 16:54:49.692702 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-05-02 16:54:49.697276 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0     1179 2024-05-02 16:54:49.694652 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/model.py
--rw-r--r--   0        0        0     1368 2024-05-02 16:54:49.703985 patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.724238 patent_client-5.0.2/patent_client/_sync/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5746 2024-05-02 17:06:23.227644 patent_client-5.0.2/patent_client/_sync/epo/ops/published/api.py
--rw-r--r--   0        0        0     2878 2024-05-02 17:06:23.227876 patent_client-5.0.2/patent_client/_sync/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1917 2024-05-02 16:54:49.726807 patent_client-5.0.2/patent_client/_sync/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.780449 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-02 17:07:15.825147 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-05-02 16:54:49.779487 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-05-02 16:54:49.779804 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-02 17:07:15.827972 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18448 2024-05-02 17:07:15.837709 patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3516 2024-05-02 17:06:23.236789 patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2383 2024-05-02 17:06:23.237053 patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      737 2024-05-02 16:54:49.766843 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-02 16:54:49.771074 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1466 2024-05-02 16:54:49.778409 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2500 2024-05-02 16:54:49.774783 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/images.py
--rw-r--r--   0        0        0     1259 2024-05-02 16:54:49.776390 patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      701 2024-05-02 16:54:49.753627 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     4378 2024-05-02 16:54:49.760006 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0     1290 2024-05-02 16:54:49.765780 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     2084 2024-05-02 16:54:49.762883 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0     1066 2024-05-02 16:54:49.764083 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3609 2024-05-02 16:54:49.724096 patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-05-02 16:54:49.746815 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-05-02 16:54:49.747751 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-05-02 16:54:49.747456 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-05-02 16:54:49.747138 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-02 17:07:16.001415 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-05-02 16:54:49.749328 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-02 17:07:16.005271 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-05-02 16:54:49.748436 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-05-02 16:54:49.746102 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-05-02 16:54:49.750694 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-05-02 16:54:49.750054 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-05-02 16:54:49.751835 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.752720 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-05-02 16:54:49.751111 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-05-02 16:54:49.751285 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-05-02 16:54:49.751611 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-05-02 16:54:49.750350 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-05-02 16:54:49.749720 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-05-02 16:54:49.752544 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-05-02 16:54:49.745766 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-05-02 16:54:49.748069 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-05-02 16:54:49.749004 patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3872 2024-05-02 17:06:23.237251 patent_client-5.0.2/patent_client/_sync/epo/ops/session.py
--rw-r--r--   0        0        0     3129 2024-05-02 17:06:23.237454 patent_client-5.0.2/patent_client/_sync/epo/ops/util.py
--rw-r--r--   0        0        0     3611 2024-05-02 17:06:23.237646 patent_client-5.0.2/patent_client/_sync/http_client.py
--rw-r--r--   0        0        0      616 2024-05-02 17:06:23.238055 patent_client-5.0.2/patent_client/_sync/odp.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.274313 patent_client-5.0.2/patent_client/_sync/uspto/__init__.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.422160 patent_client-5.0.2/patent_client/_sync/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2936 2024-05-02 16:54:49.435281 patent_client-5.0.2/patent_client/_sync/uspto/assignment/api.py
--rw-r--r--   0        0        0     1273 2024-05-02 17:06:23.238245 patent_client-5.0.2/patent_client/_sync/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     4049 2024-05-02 16:54:49.422016 patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1565 2024-05-02 16:54:49.439130 patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-05-02 16:54:49.448163 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-05-02 16:54:49.448757 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-05-02 16:54:49.445263 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-05-02 16:54:49.446731 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-05-02 16:54:49.446163 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-05-02 16:54:49.447858 patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3826 2024-05-02 17:06:23.250231 patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4308 2024-05-02 17:06:23.251951 patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5910 2024-05-02 17:06:23.253634 patent_client-5.0.2/patent_client/_sync/uspto/assignment/model.py
--rw-r--r--   0        0        0     2348 2024-05-02 16:54:49.416385 patent_client-5.0.2/patent_client/_sync/uspto/assignment/model_test.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.277934 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3593 2024-05-02 17:06:23.253879 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1382 2024-05-02 16:54:49.288731 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     3113 2024-05-02 16:54:49.293522 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1963 2024-05-02 16:54:49.277782 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1971 2024-05-02 17:06:23.256609 patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/model.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.620966 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2446 2024-05-02 16:54:49.635557 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1463 2024-05-02 16:54:49.637862 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-05-02 16:54:49.620829 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     2272 2024-05-02 16:54:49.641199 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7354 2024-05-02 17:06:23.295181 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3853 2024-05-02 16:54:49.602482 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6479 2024-05-02 16:54:49.620511 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5668 2024-05-02 16:54:49.611314 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-05-02 16:54:49.641637 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-05-02 16:54:49.642377 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-05-02 16:54:49.642679 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-05-02 16:54:49.642129 patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      417 2024-05-02 16:54:49.474650 patent_client-5.0.2/patent_client/_sync/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5786 2024-05-02 17:06:23.296817 patent_client-5.0.2/patent_client/_sync/uspto/odp/api.py
--rw-r--r--   0        0        0     2898 2024-05-02 16:54:49.512417 patent_client-5.0.2/patent_client/_sync/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-05-02 16:54:49.523098 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-05-02 16:54:49.524963 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-05-02 16:54:49.522829 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-05-02 16:54:49.524478 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-05-02 16:54:49.522678 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-05-02 16:54:49.520625 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-05-02 16:54:49.523412 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-05-02 16:54:49.525169 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-05-02 16:54:49.520959 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-05-02 16:54:49.522498 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-05-02 16:54:49.523715 patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     5053 2024-05-02 17:06:23.306387 patent_client-5.0.2/patent_client/_sync/uspto/odp/manager.py
--rw-r--r--   0        0        0     2025 2024-05-02 17:06:23.306557 patent_client-5.0.2/patent_client/_sync/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16610 2024-05-02 17:06:23.306733 patent_client-5.0.2/patent_client/_sync/uspto/odp/model.py
--rw-r--r--   0        0        0    12669 2024-05-02 16:54:49.469166 patent_client-5.0.2/patent_client/_sync/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2812 2024-05-02 16:54:49.473108 patent_client-5.0.2/patent_client/_sync/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-05-02 16:54:49.474462 patent_client-5.0.2/patent_client/_sync/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      891 2024-05-02 16:54:49.474154 patent_client-5.0.2/patent_client/_sync/uspto/odp/util.py
--rw-r--r--   0        0        0      548 2024-05-02 16:54:49.549313 patent_client-5.0.2/patent_client/_sync/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4838 2024-05-02 16:54:49.579007 patent_client-5.0.2/patent_client/_sync/uspto/peds/api.py
--rw-r--r--   0        0        0     1031 2024-05-02 16:54:49.580486 patent_client-5.0.2/patent_client/_sync/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-05-02 16:54:49.595544 patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8585 2024-05-02 17:06:23.327094 patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8814 2024-05-02 17:06:23.328428 patent_client-5.0.2/patent_client/_sync/uspto/peds/manager.py
--rw-r--r--   0        0        0     9448 2024-05-02 17:06:23.330140 patent_client-5.0.2/patent_client/_sync/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    15332 2024-05-02 17:06:23.330325 patent_client-5.0.2/patent_client/_sync/uspto/peds/model.py
--rw-r--r--   0        0        0     6532 2024-05-02 16:54:49.548772 patent_client-5.0.2/patent_client/_sync/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-05-02 16:54:49.540007 patent_client-5.0.2/patent_client/_sync/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      604 2024-05-02 17:06:23.330644 patent_client-5.0.2/patent_client/_sync/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10579 2024-05-02 16:54:49.674786 patent_client-5.0.2/patent_client/_sync/uspto/ptab/api.py
--rw-r--r--   0        0        0     1021 2024-05-02 16:54:49.676210 patent_client-5.0.2/patent_client/_sync/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-05-02 16:54:49.680173 patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-05-02 16:54:49.680705 patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2467 2024-05-02 16:54:49.679688 patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2415 2024-05-02 16:54:49.646348 patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8762 2024-05-02 17:06:23.333231 patent_client-5.0.2/patent_client/_sync/uspto/ptab/model.py
--rw-r--r--   0        0        0      658 2024-05-02 16:54:49.647071 patent_client-5.0.2/patent_client/_sync/uspto/ptab/util.py
--rw-r--r--   0        0        0      742 2024-05-02 17:06:23.333548 patent_client-5.0.2/patent_client/_sync/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6952 2024-05-02 17:06:23.333795 patent_client-5.0.2/patent_client/_sync/uspto/public_search/api.py
--rw-r--r--   0        0        0      682 2024-05-02 16:54:49.335976 patent_client-5.0.2/patent_client/_sync/uspto/public_search/api_test.py
--rw-r--r--   0        0        0      416 2024-05-02 16:54:49.389789 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2482 2024-05-02 16:54:49.394364 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     7094 2024-05-02 16:54:49.407282 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     2010 2024-05-02 16:54:49.396701 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1451 2024-05-02 17:06:23.352623 patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-05-02 16:54:49.324277 patent_client-5.0.2/patent_client/_sync/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-05-02 16:54:49.379455 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-05-02 16:54:49.385172 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-05-02 16:54:49.389523 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-05-02 16:54:49.387433 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-02 17:07:18.152251 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-05-02 16:54:49.370527 patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4487 2024-05-02 16:54:49.344979 patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7339 2024-05-02 16:54:49.306132 patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      940 2024-05-02 17:06:23.354093 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3548 2024-05-02 16:54:49.351720 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7978 2024-05-02 16:54:49.367308 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2665 2024-05-02 16:54:49.355383 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1951 2024-05-02 17:06:23.355657 patent_client-5.0.2/patent_client/_sync/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4936 2024-05-02 16:54:49.323048 patent_client-5.0.2/patent_client/_sync/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-05-02 16:54:49.293946 patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4729 2024-05-02 17:06:23.355939 patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-05-02 16:54:49.345205 patent_client-5.0.2/patent_client/_sync/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      689 2024-05-02 16:54:49.323888 patent_client-5.0.2/patent_client/_sync/uspto/public_search/util.py
--rw-r--r--   0        0        0     6043 2024-05-01 18:05:48.009638 patent_client-5.0.2/patent_client/parser.py
--rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.2/patent_client/patches.py
--rw-r--r--   0        0        0     3276 2024-05-02 17:06:23.356172 patent_client-5.0.2/patent_client/session.py
--rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.2/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.2/patent_client/test_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.2/patent_client/util/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.2/patent_client/util/asyncio_util.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.2/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4313 2024-05-02 17:07:19.017614 patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6924 2024-05-02 17:07:19.020230 patent_client-5.0.2/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.2/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.2/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3554 2024-05-02 17:06:23.356557 patent_client-5.0.2/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.2/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.2/patent_client/util/format.py
--rw-r--r--   0        0        0     9728 2024-05-02 17:06:23.356944 patent_client-5.0.2/patent_client/util/manager.py
--rw-r--r--   0        0        0     3035 2024-05-02 17:06:23.357203 patent_client-5.0.2/patent_client/util/pydantic_util.py
--rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.2/patent_client/util/request_util.py
--rw-r--r--   0        0        0     1255 2024-05-02 17:06:23.357370 patent_client-5.0.2/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2024-05-02 17:10:12.308623 patent_client-5.0.2/patent_client/version.py
--rw-r--r--   0        0        0     3376 2024-05-02 17:10:12.308856 patent_client-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.3/LICENSE
+-rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.3/README.md
+-rw-r--r--   0        0        0     1739 2024-05-03 14:36:15.835984 patent_client-5.0.3/patent_client/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.3/patent_client/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.3/patent_client/_async/epo/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.3/patent_client/_async/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.3/patent_client/_async/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-03 14:36:15.831422 patent_client-5.0.3/patent_client/_async/epo/ops/family/api.py
+-rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.3/patent_client/_async/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      356 2024-05-03 14:36:15.835205 patent_client-5.0.3/patent_client/_async/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.3/patent_client/_async/epo/ops/family/model.py
+-rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.3/patent_client/_async/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1503 2024-05-03 14:36:15.835904 patent_client-5.0.3/patent_client/_async/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.3/patent_client/_async/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.3/patent_client/_async/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.3/patent_client/_async/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.3/patent_client/_async/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      467 2024-05-03 14:36:15.837797 patent_client-5.0.3/patent_client/_async/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.3/patent_client/_async/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5434 2024-05-03 14:36:15.837457 patent_client-5.0.3/patent_client/_async/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.3/patent_client/_async/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4018 2024-05-03 14:36:15.834188 patent_client-5.0.3/patent_client/_async/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.3/patent_client/_async/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.3/patent_client/_async/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.3/patent_client/_async/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.3/patent_client/_async/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5472 2024-05-03 14:36:15.841611 patent_client-5.0.3/patent_client/_async/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2699 2024-05-03 14:36:15.838896 patent_client-5.0.3/patent_client/_async/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.3/patent_client/_async/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-03 14:39:02.936670 patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-03 14:39:02.939584 patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-03 14:39:02.949056 patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3204 2024-05-03 14:36:15.837911 patent_client-5.0.3/patent_client/_async/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2411 2024-05-03 14:36:15.836960 patent_client-5.0.3/patent_client/_async/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.3/patent_client/_async/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.3/patent_client/_async/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.3/patent_client/_async/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2078 2024-05-03 14:36:15.832663 patent_client-5.0.3/patent_client/_async/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.3/patent_client/_async/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3934 2024-05-03 14:36:15.837433 patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1640 2024-05-03 14:36:15.839189 patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3160 2024-05-03 14:36:15.830965 patent_client-5.0.3/patent_client/_async/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-03 14:39:03.080244 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-03 14:39:03.084101 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.3/patent_client/_async/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3478 2024-05-03 14:36:15.830707 patent_client-5.0.3/patent_client/_async/epo/ops/session.py
+-rw-r--r--   0        0        0     2881 2024-05-03 14:36:15.835538 patent_client-5.0.3/patent_client/_async/epo/ops/util.py
+-rw-r--r--   0        0        0     3220 2024-05-03 14:36:15.832110 patent_client-5.0.3/patent_client/_async/http_client.py
+-rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.3/patent_client/_async/odp.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.3/patent_client/_async/uspto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.3/patent_client/_async/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-03 14:36:15.830107 patent_client-5.0.3/patent_client/_async/uspto/assignment/api.py
+-rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.3/patent_client/_async/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     3595 2024-05-03 14:36:15.834092 patent_client-5.0.3/patent_client/_async/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.3/patent_client/_async/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3424 2024-05-03 14:36:15.833024 patent_client-5.0.3/patent_client/_async/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4158 2024-05-03 14:36:15.836364 patent_client-5.0.3/patent_client/_async/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5500 2024-05-03 14:36:15.831536 patent_client-5.0.3/patent_client/_async/uspto/assignment/model.py
+-rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.3/patent_client/_async/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.3/patent_client/_async/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3182 2024-05-03 14:36:15.834395 patent_client-5.0.3/patent_client/_async/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.3/patent_client/_async/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.3/patent_client/_async/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.3/patent_client/_async/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1553 2024-05-03 14:36:15.838261 patent_client-5.0.3/patent_client/_async/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1762 2024-05-03 14:36:15.840608 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     6897 2024-05-03 14:36:15.840603 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6031 2024-05-03 14:36:15.838927 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.3/patent_client/_async/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5284 2024-05-03 14:36:15.831119 patent_client-5.0.3/patent_client/_async/uspto/odp/api.py
+-rw-r--r--   0        0        0     2818 2024-05-03 14:36:15.833277 patent_client-5.0.3/patent_client/_async/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     4782 2024-05-03 14:36:15.831130 patent_client-5.0.3/patent_client/_async/uspto/odp/manager.py
+-rw-r--r--   0        0        0     1895 2024-05-02 17:06:23.185692 patent_client-5.0.3/patent_client/_async/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16091 2024-05-03 14:36:15.834907 patent_client-5.0.3/patent_client/_async/uspto/odp/model.py
+-rw-r--r--   0        0        0    12133 2024-05-03 14:36:15.835762 patent_client-5.0.3/patent_client/_async/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.3/patent_client/_async/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.3/patent_client/_async/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.3/patent_client/_async/uspto/odp/util.py
+-rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.3/patent_client/_async/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.3/patent_client/_async/uspto/peds/api.py
+-rw-r--r--   0        0        0      683 2024-05-03 14:36:15.835682 patent_client-5.0.3/patent_client/_async/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.3/patent_client/_async/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8619 2024-05-03 14:09:11.635614 patent_client-5.0.3/patent_client/_async/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8191 2024-05-03 14:36:15.831868 patent_client-5.0.3/patent_client/_async/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9623 2024-05-03 14:36:15.832507 patent_client-5.0.3/patent_client/_async/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    14958 2024-05-03 14:36:15.833958 patent_client-5.0.3/patent_client/_async/uspto/peds/model.py
+-rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.3/patent_client/_async/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.3/patent_client/_async/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.3/patent_client/_async/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10134 2024-05-03 14:36:15.834845 patent_client-5.0.3/patent_client/_async/uspto/ptab/api.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.3/patent_client/_async/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.3/patent_client/_async/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.3/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2025 2024-05-03 14:36:15.830109 patent_client-5.0.3/patent_client/_async/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2249 2024-05-03 14:36:15.836119 patent_client-5.0.3/patent_client/_async/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8382 2024-05-03 14:36:15.838732 patent_client-5.0.3/patent_client/_async/uspto/ptab/model.py
+-rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.3/patent_client/_async/uspto/ptab/util.py
+-rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.3/patent_client/_async/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6921 2024-05-03 14:36:15.830325 patent_client-5.0.3/patent_client/_async/uspto/public_search/api.py
+-rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.3/patent_client/_async/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6548 2024-05-03 14:36:15.833022 patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.3/patent_client/_async/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.3/patent_client/_async/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-03 14:39:05.314306 patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4132 2024-05-03 14:36:15.836491 patent_client-5.0.3/patent_client/_async/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7627 2024-05-03 14:36:15.841430 patent_client-5.0.3/patent_client/_async/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      554 2024-05-03 14:37:46.655035 patent_client-5.0.3/patent_client/_async/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3091 2024-05-03 14:36:15.839357 patent_client-5.0.3/patent_client/_async/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7574 2024-05-03 14:36:15.834971 patent_client-5.0.3/patent_client/_async/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2243 2024-05-03 14:36:15.838431 patent_client-5.0.3/patent_client/_async/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.3/patent_client/_async/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4498 2024-05-03 14:36:15.832881 patent_client-5.0.3/patent_client/_async/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.3/patent_client/_async/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4056 2024-05-03 14:36:15.834101 patent_client-5.0.3/patent_client/_async/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.3/patent_client/_async/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.3/patent_client/_async/uspto/public_search/util.py
+-rw-r--r--   0        0        0     1249 2024-05-03 14:37:59.408803 patent_client-5.0.3/patent_client/_sync/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.946323 patent_client-5.0.3/patent_client/_sync/epo/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-03 14:37:59.957541 patent_client-5.0.3/patent_client/_sync/epo/ops/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.973334 patent_client-5.0.3/patent_client/_sync/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-03 14:37:59.975927 patent_client-5.0.3/patent_client/_sync/epo/ops/family/api.py
+-rw-r--r--   0        0        0      839 2024-05-03 14:38:49.876504 patent_client-5.0.3/patent_client/_sync/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-05-03 14:37:59.982146 patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-05-03 14:37:59.982491 patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-05-03 14:37:59.983472 patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-05-03 14:37:59.982936 patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      750 2024-05-03 14:37:59.977628 patent_client-5.0.3/patent_client/_sync/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1535 2024-05-03 14:37:59.975224 patent_client-5.0.3/patent_client/_sync/epo/ops/family/model.py
+-rw-r--r--   0        0        0      887 2024-05-03 14:38:49.886728 patent_client-5.0.3/patent_client/_sync/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1919 2024-05-03 14:37:59.979931 patent_client-5.0.3/patent_client/_sync/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      943 2024-05-03 14:37:59.973183 patent_client-5.0.3/patent_client/_sync/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:38:00.071771 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-03 14:38:00.076639 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      688 2024-05-03 14:38:49.870707 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-05-03 14:38:00.108475 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-05-03 14:38:00.106613 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-05-03 14:38:00.108158 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-05-03 14:38:00.107017 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-05-03 14:38:00.107316 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-05-03 14:38:00.107797 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-05-03 14:38:00.105336 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      847 2024-05-03 14:38:49.483639 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2791 2024-05-03 14:38:00.075813 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5767 2024-05-03 14:38:49.462011 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      866 2024-05-03 14:38:49.881641 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4434 2024-05-03 14:38:00.093797 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1632 2024-05-03 14:38:00.071240 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      530 2024-05-03 14:38:00.071623 patent_client-5.0.3/patent_client/_sync/epo/ops/legal/util.py
+-rw-r--r--   0        0        0      483 2024-05-03 14:37:59.958442 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1819 2024-05-03 14:37:59.962155 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     2023 2024-05-03 14:38:49.483460 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1533 2024-05-03 14:37:59.964464 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-05-03 14:37:59.958165 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-05-03 14:37:59.962327 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0     1179 2024-05-03 14:37:59.959877 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0     1368 2024-05-03 14:37:59.969102 patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.992497 patent_client-5.0.3/patent_client/_sync/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5742 2024-05-03 14:38:49.482645 patent_client-5.0.3/patent_client/_sync/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2878 2024-05-03 14:38:49.865496 patent_client-5.0.3/patent_client/_sync/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1917 2024-05-03 14:37:59.994962 patent_client-5.0.3/patent_client/_sync/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-05-03 14:38:00.067428 patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-03 14:39:22.596510 patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-05-03 14:38:00.065518 patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-05-03 14:38:00.066050 patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-03 14:39:22.599463 patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-03 14:39:22.609014 patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3494 2024-05-03 14:38:00.013599 patent_client-5.0.3/patent_client/_sync/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2383 2024-05-03 14:38:49.482564 patent_client-5.0.3/patent_client/_sync/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      737 2024-05-03 14:38:00.052292 patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-03 14:38:00.056955 patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1466 2024-05-03 14:38:00.064527 patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2470 2024-05-03 14:38:00.060644 patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0     1259 2024-05-03 14:38:00.062374 patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      701 2024-05-03 14:38:00.038716 patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     4350 2024-05-03 14:38:00.045206 patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0     1290 2024-05-03 14:38:00.051413 patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     2056 2024-05-03 14:38:00.048218 patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0     1066 2024-05-03 14:38:00.049481 patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3576 2024-05-03 14:37:59.992330 patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-05-03 14:38:00.015294 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-05-03 14:38:00.016283 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-05-03 14:38:00.015986 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-05-03 14:38:00.015636 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-03 14:39:22.736261 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-05-03 14:38:00.018038 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-03 14:39:22.739802 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-05-03 14:38:00.017010 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-05-03 14:38:00.014576 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-05-03 14:38:00.019341 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-05-03 14:38:00.018683 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-05-03 14:38:00.020342 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-05-03 14:38:00.020802 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-05-03 14:38:00.019616 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-05-03 14:38:00.019820 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-05-03 14:38:00.020084 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-05-03 14:38:00.019037 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-05-03 14:38:00.018326 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-05-03 14:38:00.020596 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-05-03 14:38:00.014020 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-05-03 14:38:00.016662 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-05-03 14:38:00.017639 patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3872 2024-05-03 14:37:59.957025 patent_client-5.0.3/patent_client/_sync/epo/ops/session.py
+-rw-r--r--   0        0        0     3129 2024-05-03 14:38:49.877746 patent_client-5.0.3/patent_client/_sync/epo/ops/util.py
+-rw-r--r--   0        0        0     3597 2024-05-03 14:37:59.406711 patent_client-5.0.3/patent_client/_sync/http_client.py
+-rw-r--r--   0        0        0      616 2024-05-03 14:37:59.409428 patent_client-5.0.3/patent_client/_sync/odp.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.409653 patent_client-5.0.3/patent_client/_sync/uspto/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.581935 patent_client-5.0.3/patent_client/_sync/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2922 2024-05-03 14:37:59.595069 patent_client-5.0.3/patent_client/_sync/uspto/assignment/api.py
+-rw-r--r--   0        0        0     1256 2024-05-03 14:38:49.879205 patent_client-5.0.3/patent_client/_sync/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     4011 2024-05-03 14:37:59.581745 patent_client-5.0.3/patent_client/_sync/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1565 2024-05-03 14:37:59.598773 patent_client-5.0.3/patent_client/_sync/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-05-03 14:37:59.624868 patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-05-03 14:37:59.625166 patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-05-03 14:37:59.619332 patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-05-03 14:37:59.623839 patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-05-03 14:37:59.620365 patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-05-03 14:37:59.624583 patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3766 2024-05-03 14:38:49.482752 patent_client-5.0.3/patent_client/_sync/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4209 2024-05-03 14:38:49.863041 patent_client-5.0.3/patent_client/_sync/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5904 2024-05-03 14:37:59.590868 patent_client-5.0.3/patent_client/_sync/uspto/assignment/model.py
+-rw-r--r--   0        0        0     2348 2024-05-03 14:37:59.576141 patent_client-5.0.3/patent_client/_sync/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.413829 patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-03 14:37:59.422782 patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1364 2024-05-03 14:38:49.484327 patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     3099 2024-05-03 14:38:49.483153 patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1923 2024-05-03 14:38:49.890648 patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1957 2024-05-03 14:37:59.416922 patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.824146 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2470 2024-05-03 14:38:49.483353 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1445 2024-05-03 14:38:49.866060 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-05-03 14:37:59.824012 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     2132 2024-05-03 14:37:59.842850 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7139 2024-05-03 14:38:49.893850 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3741 2024-05-03 14:38:49.483285 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6447 2024-05-03 14:37:59.823779 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5668 2024-05-03 14:37:59.814658 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-05-03 14:37:59.843238 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-05-03 14:37:59.843827 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-05-03 14:37:59.844147 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-05-03 14:37:59.843618 patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      417 2024-05-03 14:37:59.650663 patent_client-5.0.3/patent_client/_sync/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5546 2024-05-03 14:38:49.483162 patent_client-5.0.3/patent_client/_sync/uspto/odp/api.py
+-rw-r--r--   0        0        0     2871 2024-05-03 14:38:49.483546 patent_client-5.0.3/patent_client/_sync/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-05-03 14:37:59.705978 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-05-03 14:37:59.707466 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-05-03 14:37:59.705680 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-05-03 14:37:59.706997 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-05-03 14:37:59.705491 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-05-03 14:37:59.704809 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-05-03 14:37:59.706290 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-05-03 14:37:59.707699 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-05-03 14:37:59.704983 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-05-03 14:37:59.705315 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-05-03 14:37:59.706607 patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     4979 2024-05-03 14:38:49.482805 patent_client-5.0.3/patent_client/_sync/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2003 2024-05-03 14:38:49.482899 patent_client-5.0.3/patent_client/_sync/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16273 2024-05-03 14:38:49.884466 patent_client-5.0.3/patent_client/_sync/uspto/odp/model.py
+-rw-r--r--   0        0        0    12549 2024-05-03 14:37:59.645134 patent_client-5.0.3/patent_client/_sync/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2812 2024-05-03 14:37:59.649159 patent_client-5.0.3/patent_client/_sync/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-05-03 14:37:59.650478 patent_client-5.0.3/patent_client/_sync/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      891 2024-05-03 14:37:59.650234 patent_client-5.0.3/patent_client/_sync/uspto/odp/util.py
+-rw-r--r--   0        0        0      548 2024-05-03 14:37:59.731670 patent_client-5.0.3/patent_client/_sync/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4838 2024-05-03 14:37:59.761494 patent_client-5.0.3/patent_client/_sync/uspto/peds/api.py
+-rw-r--r--   0        0        0      986 2024-05-03 14:38:49.482412 patent_client-5.0.3/patent_client/_sync/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-05-03 14:37:59.800574 patent_client-5.0.3/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8619 2024-05-03 14:37:59.800135 patent_client-5.0.3/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8510 2024-05-03 14:37:59.775474 patent_client-5.0.3/patent_client/_sync/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9245 2024-05-03 14:38:49.484513 patent_client-5.0.3/patent_client/_sync/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    15280 2024-05-03 14:38:49.873839 patent_client-5.0.3/patent_client/_sync/uspto/peds/model.py
+-rw-r--r--   0        0        0     6532 2024-05-03 14:37:59.731254 patent_client-5.0.3/patent_client/_sync/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-05-03 14:37:59.722594 patent_client-5.0.3/patent_client/_sync/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      604 2024-05-03 14:37:59.905537 patent_client-5.0.3/patent_client/_sync/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10513 2024-05-03 14:37:59.932278 patent_client-5.0.3/patent_client/_sync/uspto/ptab/api.py
+-rw-r--r--   0        0        0      992 2024-05-03 14:38:49.482407 patent_client-5.0.3/patent_client/_sync/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-05-03 14:37:59.945524 patent_client-5.0.3/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-05-03 14:37:59.946098 patent_client-5.0.3/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2407 2024-05-03 14:37:59.936957 patent_client-5.0.3/patent_client/_sync/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2270 2024-05-03 14:38:49.483857 patent_client-5.0.3/patent_client/_sync/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8786 2024-05-03 14:37:59.918088 patent_client-5.0.3/patent_client/_sync/uspto/ptab/model.py
+-rw-r--r--   0        0        0      658 2024-05-03 14:37:59.905006 patent_client-5.0.3/patent_client/_sync/uspto/ptab/util.py
+-rw-r--r--   0        0        0      742 2024-05-03 14:37:59.464708 patent_client-5.0.3/patent_client/_sync/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     7172 2024-05-03 14:37:59.475169 patent_client-5.0.3/patent_client/_sync/uspto/public_search/api.py
+-rw-r--r--   0        0        0      667 2024-05-03 14:38:49.483013 patent_client-5.0.3/patent_client/_sync/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 14:37:59.551065 patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-03 14:37:59.554323 patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6964 2024-05-03 14:37:59.567019 patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     2010 2024-05-03 14:37:59.556752 patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1451 2024-05-03 14:37:59.477738 patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-05-03 14:37:59.463915 patent_client-5.0.3/patent_client/_sync/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-05-03 14:37:59.548153 patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-05-03 14:37:59.548647 patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-05-03 14:37:59.550751 patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-05-03 14:37:59.550202 patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-03 14:39:24.949529 patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-05-03 14:37:59.532547 patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4475 2024-05-03 14:38:49.889662 patent_client-5.0.3/patent_client/_sync/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7113 2024-05-03 14:38:49.483580 patent_client-5.0.3/patent_client/_sync/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      970 2024-05-03 14:37:59.508737 patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3495 2024-05-03 14:37:59.513808 patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7978 2024-05-03 14:37:59.529290 patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2659 2024-05-03 14:37:59.517537 patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1951 2024-05-03 14:37:59.449288 patent_client-5.0.3/patent_client/_sync/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4914 2024-05-03 14:37:59.462820 patent_client-5.0.3/patent_client/_sync/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-05-03 14:37:59.434686 patent_client-5.0.3/patent_client/_sync/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4472 2024-05-03 14:37:59.455910 patent_client-5.0.3/patent_client/_sync/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-05-03 14:37:59.484812 patent_client-5.0.3/patent_client/_sync/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      689 2024-05-03 14:37:59.463571 patent_client-5.0.3/patent_client/_sync/uspto/public_search/util.py
+-rw-r--r--   0        0        0     6027 2024-05-03 14:36:15.830608 patent_client-5.0.3/patent_client/parser.py
+-rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.3/patent_client/patches.py
+-rw-r--r--   0        0        0     3262 2024-05-03 14:36:15.835349 patent_client-5.0.3/patent_client/session.py
+-rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.3/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.3/patent_client/test_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.3/patent_client/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.3/patent_client/util/asyncio_util.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.3/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4313 2024-05-03 14:39:25.849554 patent_client-5.0.3/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.3/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6924 2024-05-03 14:39:25.852213 patent_client-5.0.3/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.3/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.3/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3522 2024-05-03 14:36:15.832764 patent_client-5.0.3/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.3/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.3/patent_client/util/format.py
+-rw-r--r--   0        0        0     9700 2024-05-03 14:36:15.831113 patent_client-5.0.3/patent_client/util/manager.py
+-rw-r--r--   0        0        0     3062 2024-05-03 14:23:08.076198 patent_client-5.0.3/patent_client/util/pydantic_util.py
+-rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.3/patent_client/util/request_util.py
+-rw-r--r--   0        0        0     1233 2024-05-03 14:36:15.837976 patent_client-5.0.3/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2024-05-03 14:39:34.356039 patent_client-5.0.3/patent_client/version.py
+-rw-r--r--   0        0        0     3407 2024-05-03 14:39:34.356309 patent_client-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.3/PKG-INFO
```

### Comparing `patent_client-5.0.2/LICENSE` & `patent_client-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/README.md` & `patent_client-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/__init__.py` & `patent_client-5.0.3/patent_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 # Set up a specific logger with our desired output level
 logger = logging.getLogger(__name__)
 logger.setLevel(SETTINGS.log_level)
 
 
 # Add the log message handler to the logger
 handler = logging.FileHandler(LOG_FILENAME)
-handler.setFormatter(
-    logging.Formatter("%(asctime)s:%(levelname)s:%(name)s:%(message)s")
-)
+handler.setFormatter(logging.Formatter("%(asctime)s:%(levelname)s:%(name)s:%(message)s"))
 logger.addHandler(handler)
 
 logger.info(f"Starting Patent Client with log level {SETTINGS.log_level}")
 
 try:
     from ._sync import *
 except ImportError:
```

### Comparing `patent_client-5.0.2/patent_client/_async/__init__.py` & `patent_client-5.0.3/patent_client/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/model.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/model_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/schema.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,19 @@
     publication_number = DocDbNumberField(
         './/epo:publication-reference/epo:document-id[@document-id-type="docdb"]'
     )
     application_number = DocDbNumberField(
         './/epo:application-reference/epo:document-id[@document-id-type="docdb"]'
     )
     family_id = f.Str("./@family-id")
-    publication_reference = f.List(
-        DocumentIdSchema, ".//epo:publication-reference/epo:document-id"
-    )
-    application_reference = f.List(
-        DocumentIdSchema, ".//epo:application-reference/epo:document-id"
-    )
+    publication_reference = f.List(DocumentIdSchema, ".//epo:publication-reference/epo:document-id")
+    application_reference = f.List(DocumentIdSchema, ".//epo:application-reference/epo:document-id")
     priority_claims = f.List(PriorityClaimSchema, ".//epo:priority-claim")
 
 
 class FamilySchema(Schema):
-    publication_reference = DocumentIdSchema(
-        ".//ops:patent-family/ops:publication-reference"
-    )
+    publication_reference = DocumentIdSchema(".//ops:patent-family/ops:publication-reference")
     num_records = f.Int(".//ops:patent-family/@total-result-count")
     publication_number = DocDbNumberField(
         './/ops:patent-family/ops:publication-reference/epo:document-id[@document-id-type="docdb"]'
     )
     family_members = f.List(FamilyMemberSchema, ".//ops:family-member")
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/family/schema_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/model.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/national_codes.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/national_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,71 +31,59 @@
 async def generate_legal_code_db():
     current = await has_current_spreadsheet()
     if current:
         logger.info("Legal Code Database is Current - skipping database creation")
         return
     else:
         try:
-            logger.info(
-                "Legal Code Database is out of date - creating legal code database"
-            )
+            logger.info("Legal Code Database is out of date - creating legal code database")
             path = await get_spreadsheet()
         except Exception:
             logger.exception(
                 "Could not find live code file - falling back to default dated 2023-11-05"
             )
-            path = (
-                Path(__file__).parent
-                / "fixtures"
-                / "legal_code_descriptions_202417.xlsx"
-            )
+            path = Path(__file__).parent / "fixtures" / "legal_code_descriptions_202417.xlsx"
         create_code_database(path)
 
 
 async def has_current_spreadsheet():
     con = sqlite3.connect(db_location, timeout=30)
     cur = con.cursor()
     try:
         fname = cur.execute("SELECT * FROM meta").fetchone()[0]
-        date_string = re.search(r"legal_code_descriptions_([\d-]+)\.xlsx", fname).group(
-            1
-        )
+        date_string = re.search(r"legal_code_descriptions_([\d-]+)\.xlsx", fname).group(1)
         try:
             date = datetime.datetime.strptime(date_string, "%Y-%W-%w").date()
-        except (
-            ValueError
-        ):  # Indicates using an older format and database needs to be updated
+        except ValueError:  # Indicates using an older format and database needs to be updated
             return False
         age = datetime.datetime.now().date() - date
         logger.debug(f"Legal Code Database is {age} days old")
         return age.days < 7
     except (sqlite3.OperationalError, TypeError):
         return False
 
 
 async def get_spreadsheet_from_epo_website() -> tuple[datetime.date, str]:
     url = "https://www.epo.org/searching-for-patents/data/coverage/weekly.html"
     response = await session.get(url)
     response.raise_for_status()
     tree = ET.HTML(response.text)
-    date_string = tree.xpath(
-        ".//tr/td[contains(text(), 'Legal event codes')]/../td[4]"
-    )[0].text.strip()
+    date_string = tree.xpath(".//tr/td[contains(text(), 'Legal event codes')]/../td[4]")[
+        0
+    ].text.strip()
     week, year = date_string.split()[1].split("/")
     date = datetime.datetime.strptime(f"{year}-{week}-0", "%Y-%W-%w").date()
     excel_url = tree.xpath('.//a[contains(@href, "Legal-event-codes")][1]/@href')[0]
     logger.info(f"Found new spreadsheet for {date.isoformat()}: {excel_url}")
     return (date, excel_url)
 
 
 async def get_spreadsheet() -> tuple[datetime.date, Path]:
     date, excel_url = await get_spreadsheet_from_epo_website()
-    out_path = (
-        legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
-    )
+    out_path = legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
     if out_path.exists():
         logger.info(f"File already downloaded! Current as of {date.isoformat()}")
         return out_path
     out_path = await session.download(excel_url, path=out_path)
     logger.info(f"Downloaded new live code file for date {date.isoformat()}")
     return out_path
 
@@ -111,16 +99,15 @@
     except (sqlite3.OperationalError, TypeError):
         pass
 
     cur.execute("CREATE TABLE IF NOT EXISTS meta (file_name text)")
     cur.execute("INSERT INTO meta values (?)", (excel_path.name,))
     wb = load_workbook(excel_path)
     data = list(
-        tuple(i.strip() for i in r)
-        for r in wb[wb.sheetnames[0]].iter_rows(values_only=True)
+        tuple(i.strip() for i in r) for r in wb[wb.sheetnames[0]].iter_rows(values_only=True)
     )
     rows = data[1:]
     cur.execute("DROP TABLE IF EXISTS legal_codes")
     cur.execute(
         """CREATE TABLE IF NOT EXISTS legal_codes (
     country_code text,
     event_code text,
@@ -132,17 +119,15 @@
     last_update_orig text,
     event_class text,
     event_class_description text)"""
     )
     cur.execute(
         """CREATE INDEX IF NOT EXISTS country_event_code ON legal_codes (country_code, event_code)"""
     )
-    cur.executemany(
-        "INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows
-    )
+    cur.executemany("INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows)
     con.commit()
 
 
 class LegalCodes:
     def __init__(self):
         self.initialized = False
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,23 +99,19 @@
     extension_states = f.Str(".//ops:L524EP", formatter=lambda x: x.split(" "))
     effective_date = f.Date(".//ops:L525EP")
     date_of_withdrawal = f.Str(".//ops:L526EP")
 
     def deserialize(self, obj) -> "Dict":
         obj = super().deserialize(obj)
         if obj.event_code == "REG":
-            code_data = code_db.get_code_data(
-                obj.event_country, obj.regional_event_code
-            )
+            code_data = code_db.get_code_data(obj.event_country, obj.regional_event_code)
             obj["event_code"] = obj.event_country + "." + obj.regional_event_code
         else:
             code_data = code_db.get_code_data(obj.country_code, obj.event_code)
             obj["event_code"] = obj.country_code + "." + obj.event_code
         obj["event_description"] = code_data["description"]
         return obj
 
 
 class LegalSchema(Schema):
-    publication_reference = DocumentIdSchema(
-        ".//ops:patent-family/ops:publication-reference"
-    )
+    publication_reference = DocumentIdSchema(".//ops:patent-family/ops:publication-reference")
     events = f.List(LegalEventSchema, ".//ops:legal")
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/legal/schema_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/api_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/errors.txt` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/messages.txt` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/model.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/number_service/schema.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/api.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,41 +20,35 @@
         """Published Data Constituents API
         number: document number to search
         doc_type: document type (application / publication)
         format: document number format (original / docdb / epodoc)
         constituents: what data to retrieve. Can be combined. (biblio / abstract / full-cycle)
 
         """
-        base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/"
+        base_url = (
+            f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/"
+        )
         if isinstance(constituents, str):
             constituents = (constituents,)
         url = base_url + ",".join(constituents)
         response = await session.get(url)
         return response.text
 
     @classmethod
-    async def get_biblio(
-        cls, number, doc_type="publication", format="docdb"
-    ) -> "BiblioResult":
-        text = await cls.get_constituents(
-            number, doc_type, format, constituents="biblio"
-        )
+    async def get_biblio(cls, number, doc_type="publication", format="docdb") -> "BiblioResult":
+        text = await cls.get_constituents(number, doc_type, format, constituents="biblio")
         return BiblioResult.model_validate(text)
 
     @classmethod
     async def get_abstract(cls, number, doc_type="publication", format="docdb"):
-        return await cls.get_constituents(
-            number, doc_type, format, constituents="abstract"
-        )
+        return await cls.get_constituents(number, doc_type, format, constituents="abstract")
 
     @classmethod
     async def get_full_cycle(cls, number, doc_type="publication", format="docdb"):
-        return await cls.get_constituents(
-            number, doc_type, format, constituents="full-cycle"
-        )
+        return await cls.get_constituents(number, doc_type, format, constituents="full-cycle")
 
 
 class PublishedFulltextApi:
     fulltext_jurisdictions = "EP, WO, AT, BE, BG, CA, CH, CY, CZ, DK, EE, ES, FR, GB, GR, HR, IE, IT, LT, LU, MC, MD, ME, NO, PL, PT, RO, RS, SE, SK".split(
         ", "
     )
 
@@ -82,17 +76,15 @@
     async def get_description(cls, number, doc_type="publication", format="docdb"):
         text = await cls.get_fulltext_result(
             number, doc_type="publication", format="docdb", inquiry="description"
         )
         return Description.model_validate(text)
 
     @classmethod
-    async def get_claims(
-        cls, number, doc_type="publication", format="docdb"
-    ) -> "Claims":
+    async def get_claims(cls, number, doc_type="publication", format="docdb") -> "Claims":
         text = await cls.get_fulltext_result(
             number, doc_type="publication", format="docdb", inquiry="claims"
         )
         return Claims.model_validate(text)
 
 
 class PublishedSearchApi:
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/api_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
     @pytest.mark.asyncio
     async def test_doc_example_full_cycle(self):
-        result = await PublishedApi.biblio.get_full_cycle(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = await PublishedApi.biblio.get_full_cycle("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_full_cycle_result.xml"
         expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
     @pytest.mark.asyncio
     async def test_doc_example_abstract(self):
@@ -47,17 +45,15 @@
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
 
 class TestFullTextAsyncApi:
     @pytest.mark.asyncio
     async def test_description(self):
-        result = await PublishedApi.fulltext.get_description(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = await PublishedApi.fulltext.get_description("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_description_result.xml"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
     @pytest.mark.asyncio
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/cql.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/manager.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         limit = self.config.limit or page.num_results - offset
         num_results = page.num_results
         num_results -= offset
         num_results = min(limit, num_results)
         return num_results
 
     async def _get_results(self):
-        for start, end in get_ranges(
-            self.config.limit, self.config.offset, self.result_size
-        ):
+        for start, end in get_ranges(self.config.limit, self.config.offset, self.result_size):
             page = await self._get_search_results_range(start, end)
             for result in page.results:
                 yield result
             if len(page.results) < self.result_size:
                 break
 
     async def get(self, number, doc_type="publication", format="docdb") -> BiblioResult:
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/manager_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/manager_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 
 class TestPublished:
     @pytest.mark.asyncio
     async def test_inpadoc_manager(self):
         result = Inpadoc.objects.filter(applicant="Microsoft")
         assert await result.count() > 20
-        countries = [
-            c async for c in result.limit(20).values_list("country", flat=True)
-        ]
+        countries = [c async for c in result.limit(20).values_list("country", flat=True)]
         assert sum(1 for c in countries if c == "US") >= 1
 
     @pytest.mark.asyncio
     async def test_get_biblio_from_result(self):
         doc = await Inpadoc.objects.filter(applicant="Google").first()
         result = await doc.biblio
         assert len(result.titles) > 0
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/biblio.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/fulltext.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/images.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/model/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 
     async def download(self, path="."):
         from ..api import PublishedImagesApi
 
         out_file = Path(path) / f"{self.doc_number}.pdf"
         writer = PdfWriter()
         for i in range(1, self.num_pages + 1):
-            page_data = await PublishedImagesApi.get_page_image_from_link(
-                self.link, page_number=i
-            )
+            page_data = await PublishedImagesApi.get_page_image_from_link(self.link, page_number=i)
             page = PdfReader(page_data).pages[0]
             if page["/Rotate"] == 90:
                 page.rotate_clockwise(-90)
             writer.add_page(page)
 
         for section in self.sections:
             writer.add_outline_item(section.name.capitalize(), section.start_page)
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/model/search.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/biblio.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/biblio.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,15 @@
         './/epo:classification-scheme[@scheme="UC"]/following-sibling::epo:classification-symbol',
     )
     priority_claims = f.List(DocumentIdSchema, ".//epo:priority-claim/epo:document-id")
     title = f.Str('.//epo:invention-title[@lang="en"]')
     titles = f.List(TitleSchema, ".//epo:invention-title")
     abstract = f.Str('.//epo:abstract[@lang="en"]')
     citations = f.List(CitationSchema, ".//epo:citation")
-    applicants_epodoc = f.List(
-        f.Str(), './/epo:applicant[@data-format="epodoc"]//epo:name'
-    )
-    applicants_original = f.List(
-        f.Str(), './/epo:applicant[@data-format="original"]//epo:name'
-    )
+    applicants_epodoc = f.List(f.Str(), './/epo:applicant[@data-format="epodoc"]//epo:name')
+    applicants_original = f.List(f.Str(), './/epo:applicant[@data-format="original"]//epo:name')
     inventors_epodoc = f.List(f.Str(), './/epo:inventor[@data-format="epodoc"]')
     inventors_original = f.List(f.Str(), './/epo:inventor[@data-format="original"]')
 
 
 class BiblioResultSchema(Schema):
     documents = f.List(InpadocBiblioSchema, ".//epo:exchange-document")
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/images.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,10 @@
     sections = f.List(SectionSchema, "./ops:document-section")
     doc_number = f.Str("./@link", formatter=get_doc_number)
 
 
 class ImagesSchema(Schema):
     # search_reference = DocumentIdSchema(".//ops:document-inquiry/ops:publication-reference")
     publication_number = DocDbSchema(".//ops:inquiry-result/epo:publication-reference")
-    full_document = ImageDocumentSchema(
-        './/ops:document-instance[@desc="FullDocument"]'
-    )
+    full_document = ImageDocumentSchema('.//ops:document-instance[@desc="FullDocument"]')
     drawing = ImageDocumentSchema('.//ops:document-instance[@desc="Drawing"]')
-    first_page = ImageDocumentSchema(
-        './/ops:document-instance[@desc="FirstPageClipping"]'
-    )
+    first_page = ImageDocumentSchema('.//ops:document-instance[@desc="FirstPageClipping"]')
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema/search.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/schema_test.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/schema_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 from pathlib import Path
 
 import lxml.etree as ET
 import pytest
 
 from patent_client.util.test import compare_dicts
 
-from .schema import (
-    BiblioResultSchema,
-    ClaimsSchema,
-    DescriptionSchema,
-    ImagesSchema,
-    SearchSchema,
-)
+from .schema import BiblioResultSchema, ClaimsSchema, DescriptionSchema, ImagesSchema, SearchSchema
 
 test_dir = Path(__file__).parent / "test"
 expected_dir = Path(__file__).parent / "test" / "expected"
 
 
 def test_biblio():
     tree = ET.parse(test_dir / "biblio_example.xml")
@@ -83,16 +77,15 @@
 
 def test_full_cycle():
     tree = ET.parse(test_dir / "full_cycle_example.xml")
     result = BiblioResultSchema().load(tree)
     assert len(result.documents) == 2
     d = result.documents[0]
     assert (
-        d.title
-        == "Apparatus for manufacturing green bricks for the brick manufacturing industry"
+        d.title == "Apparatus for manufacturing green bricks for the brick manufacturing industry"
     )
 
 
 def test_biblio_2():
     filename = "biblio_example_4"
     input = test_dir / f"{filename}.xml"
     tree = ET.parse(input)
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/description_example.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/image_example.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/published/test/search_example.xml` & `patent_client-5.0.3/patent_client/_async/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/session.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,17 +70,17 @@
             response = yield self.build_refresh_request()
             if response.status_code != 200:
                 logger.debug(f"EPO Authentication Error!\n{response.text}")
                 raise OpsAuthenticationError(
                     "Failed to authenticate with EPO OPS! Please check your credentials. See the setup instructions at https://patent-client.readthedocs.io/en/stable/getting_started.html"
                 )
             data = response.json()
-            self.expires = dt.datetime.fromtimestamp(
-                int(data["issued_at"]) / 1000
-            ) + dt.timedelta(seconds=int(data["expires_in"]))
+            self.expires = dt.datetime.fromtimestamp(int(data["issued_at"]) / 1000) + dt.timedelta(
+                seconds=int(data["expires_in"])
+            )
             self.authorization_header = f"Bearer {data['access_token']}"
             request.headers["Authorization"] = self.authorization_header
             yield request
 
     def build_refresh_request(self):
         token = base64.b64encode(f"{self.key}:{self.secret}".encode())
         return httpx.Request(
```

### Comparing `patent_client-5.0.2/patent_client/_async/epo/ops/util.py` & `patent_client-5.0.3/patent_client/_async/epo/ops/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,25 +68,25 @@
         return await self._get_model(
             ".published.model.Claims", base_class=InpadocModel
         ).objects.get(self.docdb_number)
 
     @async_property
     async def legal(self) -> List["LegalEvent"]:
         return (
-            await self._get_model(
-                ".legal.model.Legal", base_class=InpadocModel
-            ).objects.get(self.docdb_number)
+            await self._get_model(".legal.model.Legal", base_class=InpadocModel).objects.get(
+                self.docdb_number
+            )
         ).events
 
     @async_property
     async def family(
         self,
     ) -> List["FamilyMember"]:
         return (
-            await self._get_model(
-                ".family.model.Family", base_class=InpadocModel
-            ).objects.get(self.docdb_number)
+            await self._get_model(".family.model.Family", base_class=InpadocModel).objects.get(
+                self.docdb_number
+            )
         ).family_members
 
     async def download(self, path: str = "."):
         images = await self.images
         return await images.full_document.download(path)
```

### Comparing `patent_client-5.0.2/patent_client/_async/http_client.py` & `patent_client-5.0.3/patent_client/_async/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
+import typing as tp
 import warnings
 from hashlib import blake2b
 from pathlib import Path
-import typing as tp
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
@@ -32,17 +32,15 @@
 patent_client_transport = hishel.AsyncCacheTransport(
     transport=httpx.AsyncHTTPTransport(
         verify=False,
         http2=True,
         retries=3,
     ),
     storage=hishel.AsyncFileStorage(base_path=CACHE_DIR),
-    controller=hishel.Controller(
-        allow_heuristics=True, key_generator=cache_key_generator
-    ),
+    controller=hishel.Controller(allow_heuristics=True, key_generator=cache_key_generator),
 )
 
 
 class PatentClientSession(httpx.AsyncClient):
     _default_user_agent = f"Mozilla/5.0 Python Patent Clientbot/{__version__} (parkerhancock@users.noreply.github.com)"
 
     def __init__(self, **kwargs):
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,15 @@
             },
             headers={"Accept": "application/xml"},
         )
         response.raise_for_status()
         return AssignmentPage.model_validate(convert_xml_to_json(response.content))
 
     @classmethod
-    async def download_pdf(
-        cls, reel: str, frame: str, path: Optional[Path] = None
-    ) -> Path:
+    async def download_pdf(cls, reel: str, frame: str, path: Optional[Path] = None) -> Path:
         url = cls.get_download_url(reel, frame)
 
         if path is None:
             path = Path.cwd()
             output_path = output_path = path / f"assignment-pat-{reel}-{frame}.pdf"
         elif path.is_dir():
             output_path = path / f"assignment-pat-{reel}-{frame}.pdf"
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/api_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/convert.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,15 @@
     ]
     output["properties"] = zip_lists(output, property_fields, "property")
     # Delete the original fields
     for key in assignor_fields + assignee_fields + property_fields:
         del output[key]
     # Collect the correspondent into a dict
     corr_address_fields = ["corrAddress1", "corrAddress2", "corrAddress3"]
-    correspondent_address = "\n".join(
-        output[k] for k in corr_address_fields if k in output
-    )
+    correspondent_address = "\n".join(output[k] for k in corr_address_fields if k in output)
     if correspondent_address:
         output["corr_address"] = correspondent_address
     for key in corr_address_fields:
         if key in output:
             del output[key]
     output["correspondent"] = {
         "name": output["corrName"],
@@ -59,17 +57,15 @@
     }
     del output["corrName"]
     del output["corr_address"]
 
     # Collect the address for each assignee into a single string
     for assignee in output["assignees"]:
         address_lines = "\n".join(
-            assignee[k]
-            for k in ["patAssigneeAddress1", "patAssigneeAddress2"]
-            if assignee[k]
+            assignee[k] for k in ["patAssigneeAddress1", "patAssigneeAddress2"] if assignee[k]
         )
         last_line = f"{assignee['patAssigneeCity']}, {assignee['patAssigneeState']} {assignee['patAssigneePostcode']}"
         if assignee["patAssigneeCountryName"]:
             last_line += f" ({assignee['patAssigneeCountryName']})"
         assignee_address = "\n".join([address_lines, last_line])
         if assignee_address:
             assignee["patAssigneeAddress"] = assignee_address
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/convert_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
             query = clean_number(query)
         # Handle Ordering
         order_map = {
             "execution_date": "ExecutionDate+asc",
             "-execution_date": "ExecutionDate+desc",
         }
         if len(self.config.order_by) > 1:
-            raise ValueError(
-                "Assignment API does not support multiple sort parameters!"
-            )
+            raise ValueError("Assignment API does not support multiple sort parameters!")
         elif len(self.config.order_by) == 1:
             sort = order_map[self.config.order_by[0]]
         else:
             sort = "ExecutionDate+desc"
 
         # if isinstance(query, list):
         #    query = [f'"{q}"' for q in query]
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/manager_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/manager_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,25 +73,21 @@
             assignment.image_url
             == "http://legacy-assignments.uspto.gov/assignments/assignment-pat-038505-0128.pdf"
         )
 
     @pytest.mark.asyncio
     async def test_slice_assignments(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
-        assignment_list1 = [
-            assignment.id async for assignment in await assignments[0:5]
-        ]
+        assignment_list1 = [assignment.id async for assignment in await assignments[0:5]]
         assert len(assignment_list1) == 5
 
         assignment_list2 = [assignment.id async for assignment in await assignments[:5]]
         assert len(assignment_list2) == 5
 
-        assignment_list3 = [
-            assignment.id async for assignment in await assignments[-5:]
-        ]
+        assignment_list3 = [assignment.id async for assignment in await assignments[-5:]]
         assert len(assignment_list3) == 5
 
     @pytest.mark.asyncio
     async def test_iterate_assignments(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
         assignment_list = [assignment.id async for assignment in assignments]
         assert len(assignment_list) == await assignments.count()
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/model.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
+import typing as tp
 import warnings
 from pathlib import Path
-import typing as tp
 
 from dateutil.parser import isoparse
 from pydantic import BeforeValidator, ConfigDict, Field, field_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
@@ -31,17 +31,15 @@
 def parse_date(string):
     dt = parse_datetime(string)
     if dt is None:
         return None
     return dt.date()
 
 
-DatetimeAsDate = Annotated[
-    tp.Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
-]
+DatetimeAsDate = Annotated[tp.Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))]
 
 
 class AbstractAssignmentModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
@@ -74,43 +72,43 @@
 
     @property
     def application(self) -> tp.Optional["USApplication"]:
         """The related US Application"""
         try:
             appl_id = getattr(self, "appl_id", None)
             if appl_id is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(appl_id=appl_id)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    appl_id=appl_id
+                )
             appl_id = getattr(self, "pct_num", None)
             if appl_id is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(appl_id=appl_id)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    appl_id=appl_id
+                )
             pub_num = getattr(self, "publ_num", None)
             if pub_num is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(app_early_pub_number=pub_num)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    app_early_pub_number=pub_num
+                )
             pat_num = getattr(self, "pat_num", None)
             if pat_num is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(patent_number=pat_num)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    patent_number=pat_num
+                )
         except Exception:
             pass
         warnings.warn(f"Unable to find application for {self}")
         return None
 
     @property
     def patent(self) -> "Patent":
         """The related US Patent, if any"""
-        return self._get_model(
-            "patent_client.uspto.public_search.model.Patent"
-        ).objects.get(publication_number=self.pat_num)
+        return self._get_model("patent_client.uspto.public_search.model.Patent").objects.get(
+            publication_number=self.pat_num
+        )
 
     @property
     def publication(
         self,
     ) -> "PublishedApplication":
         """The related US Publication, if any"""
         return self._get_model(
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/assignment/model_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/bulk_data/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 client = PatentClientSession()
 
 
 class BulkDataApi:
     @classmethod
     async def get_latest(cls) -> tp.List[Product]:
         """Returns all products with Latest Files"""
-        response = await client.get(
-            "https://bulkdata.uspto.gov:443/BDSS-API/products/all/latest"
-        )
+        response = await client.get("https://bulkdata.uspto.gov:443/BDSS-API/products/all/latest")
         return [Product(**product) for product in response.json()]
 
     @classmethod
     async def get_by_name(
         cls,
         product_name: str,
         from_date: tp.Optional[datetime.date] = None,
@@ -46,17 +44,15 @@
         )
         response.raise_for_status()
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     async def get_popular(cls) -> tp.List[Product]:
         """Returns popular products along with latest files."""
-        response = await client.get(
-            "https://bulkdata.uspto.gov:443/BDSS-API/products/popular"
-        )
+        response = await client.get("https://bulkdata.uspto.gov:443/BDSS-API/products/popular")
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     async def get_by_short_name(
         cls,
         product_name: str,
         from_date: tp.Optional[tp.Union[datetime.date, str]] = None,
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/api_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/manager_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/bulk_data/model.py` & `patent_client-5.0.3/patent_client/_async/uspto/bulk_data/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,10 +32,8 @@
     title: str = Field(alias="productTitle")
     frequency: tp.Optional[str] = Field(alias="productFrequency", default=None)
     level: str = Field(alias="productLevel")
     from_date: datetime.date = Field(alias="productFromDate")
     to_date: datetime.date = Field(alias="productToDate")
     number_of_files: int = Field(alias="numberOfFiles")
     parent_product: tp.Optional[str] = Field(alias="parentProduct", default=None)
-    files: tp.Optional[tp.List[File]] = Field(
-        alias="productFiles", default_factory=list
-    )
+    files: tp.Optional[tp.List[File]] = Field(alias="productFiles", default_factory=list)
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/api_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,49 +6,37 @@
 query_builder = QueryBuilder()
 
 global_dossier_api = GlobalDossierApi()
 
 
 class GlobalDossierBaseManager(AsyncManager):
     def filter(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
     def order_by(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
     def limit(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
     def offset(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
 
 class GlobalDossierManager(GlobalDossierBaseManager):
     async def get(self, *args, **kwargs):
-        return await global_dossier_api.get_file(
-            **query_builder.build_query(*args, **kwargs)
-        )
+        return await global_dossier_api.get_file(**query_builder.build_query(*args, **kwargs))
 
 
 class GlobalDossierApplicationManager(GlobalDossierBaseManager):
     async def get(self, *args, **kwargs):
         query = query_builder.build_query(*args, **kwargs)
         gd_file = await global_dossier_api.get_file(**query)
         if query["type_code"] == "application":
-            return next(
-                a for a in gd_file.applications if a.app_num in query["doc_number"]
-            )
+            return next(a for a in gd_file.applications if a.app_num in query["doc_number"])
         elif query["type_code"] == "publication":
             return next(
                 a
                 for a in gd_file.applications
                 if any(p.pub_num in query["doc_number"] for p in a.pub_list)
             )
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,17 +56,15 @@
     app_date: tp.Optional[MDYDate] = Field(alias="appDateStr")
     country_code: tp.Optional[str] = None
     kind_code: tp.Optional[str] = None
     doc_num: tp.Optional["GlobalDossierDocumentNumber"] = None
     title: tp.Optional[str] = None
     applicant_names: OptionalStrList = Field(default_factory=list)
     ip_5: tp.Optional[bool] = Field(alias="ip5")
-    priority_claim_list: "tp.List[GlobalDossierPriorityClaim]" = Field(
-        default_factory=list
-    )
+    priority_claim_list: "tp.List[GlobalDossierPriorityClaim]" = Field(default_factory=list)
     pub_list: "tp.List[GlobalDossierPublication]" = Field(default_factory=list)
 
     def __repr__(self):
         return f"GlobalDossierApplication(app_num={self.app_num}, country_code={self.country_code})"
 
     @async_property
     async def document_list(self) -> "DocumentList":
@@ -89,70 +87,54 @@
                 self.country_code, self.app_num, self.kind_code
             )
         ).office_action_docs
 
     @async_property
     async def us_application(self) -> "USApplication":
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
-        return await self._get_model("..peds.model.USApplication").objects.get(
-            self.app_num
-        )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
+        return await self._get_model("..peds.model.USApplication").objects.get(self.app_num)
 
     @async_property
     async def us_publication(self) -> "PublishedApplication":
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
         pub = list(p for p in self.pub_list if p.kind_code == "A1")
         if len(pub) > 1:
             raise ValueError("More than one US publication for application!")
-        return await self._get_model(
-            "..public_search.model.PublishedApplication"
-        ).objects.get(pub[0].pub_num)
+        return await self._get_model("..public_search.model.PublishedApplication").objects.get(
+            pub[0].pub_num
+        )
 
     @async_property
     async def us_patent(self) -> "Patent":
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
         pat = list(p for p in self.pub_list if p.kind_code in ("A", "B1", "B2"))
         if len(pat) > 1:
             raise ValueError("More than one US patent for application!")
-        return await self._get_model("..public_search.model.Patent").objects.get(
-            pat[0].pub_num
-        )
+        return await self._get_model("..public_search.model.Patent").objects.get(pat[0].pub_num)
 
     @async_property
     async def us_assignments(self) -> list["Assignment"]:
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
-        return self._get_model("..assignment.model.Assignment").objects.filter(
-            appl_id=self.app_num
-        )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
+        return self._get_model("..assignment.model.Assignment").objects.filter(appl_id=self.app_num)
 
 
 TextBool = Annotated[bool, BeforeValidator(lambda x: x == "true")]
 
 
 class GlobalDossier(GlobalDossierBaseModel):
     country: tp.Optional[str] = None
     internal: tp.Optional[TextBool] = None
     corr_app_num: tp.Optional[str] = None
     id: tp.Optional[str] = None
     type: tp.Optional[str] = None
-    applications: tp.List[GlobalDossierApplication] = Field(
-        default_factory=list, alias="list"
-    )
+    applications: tp.List[GlobalDossierApplication] = Field(default_factory=list, alias="list")
 
     def __repr__(self):
         return f"GlobalDossier(id={self.id}, type={self.type}, country={self.country})"
 
 
 class Document(GlobalDossierBaseModel):
     doc_number: tp.Optional[str] = None
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/model_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,17 +115,15 @@
                     "office_code": office_code,
                     "doc_number": arg,
                     "type_code": candidates[0]["type_code"],
                 }
 
         elif kwargs:
             numbers = {
-                k: v
-                for k, v in kwargs.items()
-                if k in ("publication", "application", "patent")
+                k: v for k, v in kwargs.items() if k in ("publication", "application", "patent")
             }
             if len(numbers) > 1:
                 raise QueryException(
                     "You may only pass one keyword from the set of (application, publication, patent)"
                 )
             elif not numbers:
                 raise QueryException("No number passed! Please pass a valid number")
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/query_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app.json` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.3/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,24 @@
 
 class ODPApi:
     base_url = "https://beta-api.uspto.gov"
 
     def __init__(self):
         self.client = PatentClientSession(headers={"X-API-KEY": SETTINGS.odp_api_key})
 
-    async def post_search(
-        self, search_request: SearchRequest = SearchRequest()
-    ) -> tp.Dict:
+    async def post_search(self, search_request: SearchRequest = SearchRequest()) -> tp.Dict:
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = await self.client.post(
             url, json=search_data, headers={"accept": "application/json"}
         )
         response.raise_for_status()
         return response.json()
 
-    async def get_search(
-        self, search_request: SearchGetRequest = SearchGetRequest()
-    ) -> tp.Dict:
+    async def get_search(self, search_request: SearchGetRequest = SearchGetRequest()) -> tp.Dict:
         """Patent application search by supplying query parameters
         Query parameters are optional. When no query parameters supplied, top 25 applications are returned"""
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = await self.client.get(url, params=search_data)
         response.raise_for_status()
         return response.json()
@@ -52,36 +48,27 @@
     async def get_application_data(self, application_id: str) -> USApplication:
         """Patent application data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}"
         response = await self.client.get(url)
         response.raise_for_status()
         return USApplication(**response.json()["patentBag"][0])
 
-    async def get_application_biblio_data(
-        self, application_id: str
-    ) -> USApplicationBiblio:
+    async def get_application_biblio_data(self, application_id: str) -> USApplicationBiblio:
         """Patent application basic data by application id"""
-        url = (
-            self.base_url
-            + f"/api/v1/patent/applications/{application_id}/application-data"
-        )
+        url = self.base_url + f"/api/v1/patent/applications/{application_id}/application-data"
         response = await self.client.get(url)
         response.raise_for_status()
         return USApplicationBiblio(**response.json()["patentBag"][0])
 
-    async def get_patent_term_adjustment_data(
-        self, application_id: str
-    ) -> TermAdjustment:
+    async def get_patent_term_adjustment_data(self, application_id: str) -> TermAdjustment:
         """Patent application term adjustment data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}/adjustment"
         response = await self.client.get(url)
         response.raise_for_status()
-        return TermAdjustment(
-            **response.json()["patentBag"][0]["patentTermAdjustmentData"]
-        )
+        return TermAdjustment(**response.json()["patentBag"][0]["patentTermAdjustmentData"])
 
     async def get_assignments(self, application_id: str) -> tp.List[Assignment]:
         """Patent application term adjustment data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}/assignment"
         response = await self.client.get(url)
         response.raise_for_status()
         data = response.json()["patentBag"][0]["assignmentBag"]
@@ -97,36 +84,27 @@
     async def get_continuity_data(self, application_id: str) -> Continuity:
         """Patent application continuity data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}/continuity"
         response = await self.client.get(url)
         response.raise_for_status()
         return Continuity(**response.json())
 
-    async def get_foreign_priority_data(
-        self, application_id: str
-    ) -> tp.List[ForeignPriority]:
+    async def get_foreign_priority_data(self, application_id: str) -> tp.List[ForeignPriority]:
         """Patent application foreign priority data by application id"""
-        url = (
-            self.base_url
-            + f"/api/v1/patent/applications/{application_id}/foreign-priority"
-        )
+        url = self.base_url + f"/api/v1/patent/applications/{application_id}/foreign-priority"
         response = await self.client.get(url)
         response.raise_for_status()
         return [
             ForeignPriority(**foreign_priority)
-            for foreign_priority in response.json()["patentBag"][0][
-                "foreignPriorityBag"
-            ]
+            for foreign_priority in response.json()["patentBag"][0]["foreignPriorityBag"]
         ]
 
     async def get_transactions(self, application_id: str) -> tp.List[Transaction]:
         """Patent application transactions by application id"""
-        url = (
-            self.base_url + f"/api/v1/patent/applications/{application_id}/transactions"
-        )
+        url = self.base_url + f"/api/v1/patent/applications/{application_id}/transactions"
         response = await self.client.get(url)
         response.raise_for_status()
         return [
             Transaction(**transaction)
             for transaction in response.json()["patentBag"][0]["transactionContentBag"]
         ]
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/api_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,15 @@
     assert application.appl_id is not None, "Expected basic patent data"
 
 
 @pytest.mark.asyncio
 async def test_get_patent_term_adjustment_data(odp_api):
     application_id = "16123456"
     response = await odp_api.get_patent_term_adjustment_data(application_id)
-    assert (
-        response.adjustment_total_quantity is not None
-    ), "Expected patent term adjustment data"
+    assert response.adjustment_total_quantity is not None, "Expected patent term adjustment data"
 
 
 @pytest.mark.asyncio
 async def test_get_assignments(odp_api):
     application_id = "15123456"
     response = await odp_api.get_assignments(application_id)
     assert len(response) > 0, "Expected at least one assignment"
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/application.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/documents.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/search.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.3/patent_client/_async/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,17 @@
 
 class USApplicationManager(AsyncManager):
     default_filter = "appl_id"
     default_fields = []
     response_model = USApplication
 
     async def count(self):
-        return (
-            await api.post_search(
-                self._create_search_obj(fields=["applicationNumberText"])
-            )
-        )["count"]
+        return (await api.post_search(self._create_search_obj(fields=["applicationNumberText"])))[
+            "count"
+        ]
 
     async def _get_results(self) -> tp.AsyncIterator["SearchResult"]:
         query_obj = self._create_search_obj()
         for start, rows in get_start_and_row_count(self.config.limit):
             page_query = query_obj.model_dump()
             page_query["pagination"] = {"offset": start, "limit": rows}
             page_query_obj = SearchRequest(**page_query)
@@ -134,17 +132,15 @@
         return await api.get_customer_numbers(self.config.filter["appl_id"][0])
 
 
 class ForeignPriorityManager(AsyncManager):
     default_filter = "appl_id"
 
     async def _get_results(self) -> "ForeignPriority":
-        for doc in await api.get_foreign_priority_data(
-            self.config.filter["appl_id"][0]
-        ):
+        for doc in await api.get_foreign_priority_data(self.config.filter["appl_id"][0]):
             yield doc
 
 
 class TransactionManager(AsyncManager):
     default_filter = "appl_id"
 
     async def _get_results(self) -> tp.AsyncIterator["Transaction"]:
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/manager_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/model.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,55 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *             Source File: patent_client/_async/uspto/odp/model.py             *
+# ********************************************************************************
+
 import datetime
 from enum import Enum
 from typing import Any, List, Optional
 
-from async_property import async_property
 from async_property.base import AsyncPropertyDescriptor
 from pydantic import AliasPath, BeforeValidator, ConfigDict, Field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
 
 class BaseODPModel(BaseModel):
-    model_config = ConfigDict(
-        alias_generator=to_camel, ignored_types=(AsyncPropertyDescriptor,)
-    )
+    model_config = ConfigDict(alias_generator=to_camel, ignored_types=(AsyncPropertyDescriptor,))
 
 
 # Common
 
 
 class Address(BaseODPModel):
     city_name: Optional[str] = Field(alias="cityName", default=None)
-    geographic_region_name: Optional[str] = Field(
-        alias="geographicRegionName", default=None
-    )
-    geographic_region_code: Optional[str] = Field(
-        alias="geographicRegionCode", default=None
-    )
+    geographic_region_name: Optional[str] = Field(alias="geographicRegionName", default=None)
+    geographic_region_code: Optional[str] = Field(alias="geographicRegionCode", default=None)
     country_code: Optional[str] = Field(alias="countryCode", default=None)
     postal_code: Optional[str] = Field(alias="postalCode", default=None)
     country_name: Optional[str] = Field(alias="countryName", default=None)
-    address_line_one_text: Optional[str] = Field(
-        alias="addressLineOneText", default=None
-    )
-    address_line_two_text: Optional[str] = Field(
-        alias="addressLineTwoText", default=None
-    )
+    address_line_one_text: Optional[str] = Field(alias="addressLineOneText", default=None)
+    address_line_two_text: Optional[str] = Field(alias="addressLineTwoText", default=None)
     name_line_one_text: Optional[str] = Field(alias="nameLineOneText", default=None)
     name_line_two_text: Optional[str] = Field(alias="nameLineTwoText", default=None)
-    postal_address_category: Optional[str] = Field(
-        alias="postalAddressCategory", default=None
-    )
-    correspondent_name_text: Optional[str] = Field(
-        alias="correspondentNameText", default=None
-    )
+    postal_address_category: Optional[str] = Field(alias="postalAddressCategory", default=None)
+    correspondent_name_text: Optional[str] = Field(alias="correspondentNameText", default=None)
 
 
 # Continuity
 
 
 class Relationship(BaseODPModel):
     application_status_code: int = Field()
     claim_type_code: str = Field(alias="claimParentageTypeCode")
     filing_date: datetime.date
-    application_status_description: str = Field(
-        alias="applicationStatusDescriptionText"
-    )
+    application_status_description: str = Field(alias="applicationStatusDescriptionText")
     claim_type_description: str = Field(alias="claimParentageTypeCodeDescription")
     parent_application_id: str = Field(alias="parentApplicationNumberText")
     child_application_id: str = Field(alias="childApplicationNumberText")
 
 
 class Continuity(BaseODPModel):
     count: int
@@ -89,28 +78,28 @@
     mail_date: datetime.datetime = Field(alias="officialDate")
     document_identifier: str = Field(alias="documentIdentifier")
     document_code: str = Field(alias="documentCode")
     document_code_description: str = Field(alias="documentCodeDescriptionText")
     direction_category: str = Field(alias="directionCategory")
     download_option_bag: list[dict] = Field(alias="downloadOptionBag")
 
-    async def download(self, type="PDF", out_path=None):
+    def download(self, type="PDF", out_path=None):
         from .manager import api
 
         try:
-            url = next(
-                u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type
-            )["downloadUrl"]
+            url = next(u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type)[
+                "downloadUrl"
+            ]
         except StopIteration:
             raise ValueError(f"No download URL found for this document type: {type}")
         if out_path is None:
             out_path = f"{self.appl_id} - {self.mail_date.date()} - {self.document_code} - {self.document_code_description}.{type.lower()}".replace(
                 "/", "-"
             )
-        return await api.client.download(url, "GET", path=out_path)
+        return api.client.download(url, "GET", path=out_path)
 
 
 # Assignment
 
 
 class Assignor(BaseODPModel):
     execution_date: datetime.date = Field(alias="executionDate")
@@ -165,25 +154,21 @@
     first_name: Optional[str] = Field(alias="firstName", default=None)
     last_name: Optional[str] = Field(alias="lastName", default=None)
     registration_number: str = Field(alias="registrationNumber")
     attorney_address_bag: list[Address] = Field(alias="attorneyAddressBag")
     telecommunication_address_bag: list[TelecommunicationAddress] = Field(
         alias="telecommunicationAddressBag"
     )
-    registered_practitioner_category: str = Field(
-        alias="registeredPractitionerCategory"
-    )
+    registered_practitioner_category: str = Field(alias="registeredPractitionerCategory")
     name_suffix: Optional[str] = Field(alias="nameSuffix", default=None)
 
 
 class CustomerNumber(BaseODPModel):
     attorneys: list[Attorney] = Field(alias="attorneyBag")
-    customer_number: Optional[str] = Field(
-        alias=AliasPath("customerNumber", "patronIdentifier")
-    )
+    customer_number: Optional[str] = Field(alias=AliasPath("customerNumber", "patronIdentifier"))
     address: Optional[Address] = Field(
         alias=AliasPath("customerNumber", "powerOfAttorneyAddressBag", 0)
     )
 
 
 # Transactions
 
@@ -203,22 +188,18 @@
     action_date: datetime.date = Field(alias="actionDate")
 
 
 class TermAdjustment(BaseODPModel):
     applicant_day_delay_quantity: Optional[int] = Field(
         alias="applicantDayDelayQuantity", default=None
     )
-    overlapping_day_quantity: Optional[int] = Field(
-        alias="overlappingDayQuantity", default=None
-    )
+    overlapping_day_quantity: Optional[int] = Field(alias="overlappingDayQuantity", default=None)
     filing_date: Optional[datetime.date] = Field(alias="filingDate", default=None)
     c_delay_quantity: Optional[int] = Field(alias="cDelayQuantity", default=None)
-    adjustment_total_quantity: Optional[int] = Field(
-        alias="adjustmentTotalQuantity", default=None
-    )
+    adjustment_total_quantity: Optional[int] = Field(alias="adjustmentTotalQuantity", default=None)
     b_delay_quantity: Optional[int] = Field(alias="bDelayQuantity", default=None)
     grant_date: Optional[datetime.date] = Field(alias="grantDate", default=None)
     a_delay_quantity: Optional[int] = Field(alias="aDelayQuantity", default=None)
     non_overlapping_day_quantity: Optional[int] = Field(
         alias="nonOverlappingDayQuantity", default=None
     )
     ip_office_day_delay_quantity: Optional[int] = Field(
@@ -261,77 +242,63 @@
     appl_id: str = Field(alias="applicationNumberText")
     first_inventor_name: str = Field(alias="firstInventorName")
     first_applicant_name: str = Field(alias="firstApplicantName")
     cpc_classifications: list[str] = Field(alias="cpcClassificationBag")
     entity_status: str = Field(alias="businessEntityStatusCategory")
     app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber")
 
-    @async_property
-    async def bibliographic_data(self) -> "USApplicationBiblio":
-        return await self._get_model(".model.USApplicationBiblio").objects.get(
-            appl_id=self.appl_id
-        )
-
-    @async_property
-    async def application(self) -> "USApplication":
-        return await self._get_model(".model.USApplication").objects.get(
-            appl_id=self.appl_id
-        )
-
-    @async_property
-    async def continuity(self) -> Continuity:
-        return await self._get_model(".model.Continuity").objects.get(
-            appl_id=self.appl_id
-        )
+    @property
+    def bibliographic_data(self) -> "USApplicationBiblio":
+        return self._get_model(".model.USApplicationBiblio").objects.get(appl_id=self.appl_id)
+
+    @property
+    def application(self) -> "USApplication":
+        return self._get_model(".model.USApplication").objects.get(appl_id=self.appl_id)
+
+    @property
+    def continuity(self) -> Continuity:
+        return self._get_model(".model.Continuity").objects.get(appl_id=self.appl_id)
 
-    @async_property
-    async def documents(self) -> list[Document]:
+    @property
+    def documents(self) -> list[Document]:
         return self._get_model(".model.Document").objects.filter(appl_id=self.appl_id)
 
-    @async_property
-    async def term_adjustment(self) -> TermAdjustment:
-        return self._get_model(".model.TermAdjustment").objects.filter(
-            appl_id=self.appl_id
-        )
+    @property
+    def term_adjustment(self) -> TermAdjustment:
+        return self._get_model(".model.TermAdjustment").objects.filter(appl_id=self.appl_id)
 
-    @async_property
-    async def assignments(self) -> list[Assignment]:
+    @property
+    def assignments(self) -> list[Assignment]:
         return self._get_model(".model.Assignment").objects.filter(appl_id=self.appl_id)
 
-    @async_property
-    async def customer_number(self) -> CustomerNumber:
-        return self._get_model(".model.CustomerNumber").objects.filter(
-            appl_id=self.appl_id
-        )
-
-    @async_property
-    async def foreign_priority(self) -> ForeignPriority:
-        return self._get_model(".model.ForeignPriority").objects.filter(
-            appl_id=self.appl_id
-        )
-
-    @async_property
-    async def transactions(self) -> list[Transaction]:
-        return self._get_model(".model.Transaction").objects.filter(
-            appl_id=self.appl_id
-        )
+    @property
+    def customer_number(self) -> CustomerNumber:
+        return self._get_model(".model.CustomerNumber").objects.filter(appl_id=self.appl_id)
+
+    @property
+    def foreign_priority(self) -> ForeignPriority:
+        return self._get_model(".model.ForeignPriority").objects.filter(appl_id=self.appl_id)
+
+    @property
+    def transactions(self) -> list[Transaction]:
+        return self._get_model(".model.Transaction").objects.filter(appl_id=self.appl_id)
 
     # Aliases
 
-    @async_property
-    async def biblio(self) -> "USApplicationBiblio":
-        return await self.bibliographic_data
-
-    @async_property
-    async def app(self) -> "USApplication":
-        return await self.application
-
-    @async_property
-    async def docs(self) -> list[Document]:
-        return await self.documents
+    @property
+    def biblio(self) -> "USApplicationBiblio":
+        return self.bibliographic_data
+
+    @property
+    def app(self) -> "USApplication":
+        return self.application
+
+    @property
+    def docs(self) -> list[Document]:
+        return self.documents
 
 
 class USApplication(BaseODPModel):
     aia_indicator: YNBool = Field(alias="firstInventorToFileIndicator")
     app_filing_date: datetime.date = Field(alias="filingDate")
     inventors: list[Inventor] = Field(alias="inventorBag")
     customer_number: int = Field(alias="customerNumber")
@@ -357,17 +324,15 @@
     transactions: list[Transaction] = Field(alias="transactionContentBag")
     parent_applications: Optional[list[Relationship]] = Field(
         alias=AliasPath("continuityBag", "parentContinuityBag"), default=None
     )
     child_applications: Optional[list[Relationship]] = Field(
         alias=AliasPath("continuityBag", "childContinuityBag"), default=None
     )
-    patent_term_adjustment: Optional[TermAdjustment] = Field(
-        alias="patentTermAdjustmentData"
-    )
+    patent_term_adjustment: Optional[TermAdjustment] = Field(alias="patentTermAdjustmentData")
 
     @model_validator(mode="before")
     @classmethod
     def _validate_patent_term_adjustment(cls, v):
         if v["patentTermAdjustmentData"] == dict():
             v["patentTermAdjustmentData"] = None
         return v
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/model_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/model_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,31 +34,26 @@
     assert continuity.parent_continuity[0].application_status_code == 161
     assert continuity.parent_continuity[0].claim_type_code == "NST"
     assert continuity.parent_continuity[0].filing_date == datetime.date(2015, 4, 22)
     assert (
         continuity.parent_continuity[0].application_status_description
         == "Abandoned  --  Failure to Respond to an Office Action"
     )
-    assert (
-        continuity.parent_continuity[0].claim_type_description
-        == "is a National Stage Entry of"
-    )
+    assert continuity.parent_continuity[0].claim_type_description == "is a National Stage Entry of"
     assert continuity.parent_continuity[0].parent_application_id == "PCT/US15/27322"
     assert continuity.parent_continuity[0].child_application_id == "15123456"
     assert len(continuity.child_continuity) == 1
     assert continuity.child_continuity[0].application_status_code == 160
     assert continuity.child_continuity[0].claim_type_code == "CON"
     assert continuity.child_continuity[0].filing_date == datetime.date(2018, 9, 13)
     assert (
         continuity.child_continuity[0].application_status_description
         == "Abandoned  --  Incomplete Application (Pre-examination)"
     )
-    assert (
-        continuity.child_continuity[0].claim_type_description == "is a Continuation of"
-    )
+    assert continuity.child_continuity[0].claim_type_description == "is a Continuation of"
     assert continuity.child_continuity[0].parent_application_id == "15123456"
     assert continuity.child_continuity[0].child_application_id == "16132008"
 
 
 def test_document(fixture_dir):
     data = json.loads((fixture_dir / "documents.json").read_text())
     for doc_data in data["documentBag"]:
@@ -159,36 +154,29 @@
     assert transactions[3].transaction_code == "SMAL"
     assert (
         transactions[3].transaction_description
         == "Applicant Has Filed a Verified Statement of Small Entity Status in Compliance with 37 CFR 1.27"
     )
     assert transactions[-1].recorded_date == datetime.date.fromisoformat("2020-10-21")
     assert transactions[-1].transaction_code == "IDSC"
-    assert (
-        transactions[-1].transaction_description
-        == "Information Disclosure Statement considered"
-    )
+    assert transactions[-1].transaction_description == "Information Disclosure Statement considered"
 
 
 def test_patent_term_adjustment(fixture_dir):
     data = json.loads((fixture_dir / "adjustment.json").read_text())
     patent_term_adjustment_data = data["patentBag"][0]["patentTermAdjustmentData"]
     patent_term_adjustment = TermAdjustment(**patent_term_adjustment_data)
 
     assert patent_term_adjustment.applicant_day_delay_quantity == 15
     assert patent_term_adjustment.overlapping_day_quantity == 0
-    assert patent_term_adjustment.filing_date == datetime.date.fromisoformat(
-        "2018-09-06"
-    )
+    assert patent_term_adjustment.filing_date == datetime.date.fromisoformat("2018-09-06")
     assert patent_term_adjustment.c_delay_quantity == 0
     assert patent_term_adjustment.adjustment_total_quantity == 0
     assert patent_term_adjustment.b_delay_quantity == 0
-    assert patent_term_adjustment.grant_date == datetime.date.fromisoformat(
-        "2021-01-26"
-    )
+    assert patent_term_adjustment.grant_date == datetime.date.fromisoformat("2021-01-26")
     assert patent_term_adjustment.a_delay_quantity == 142
     assert patent_term_adjustment.non_overlapping_day_quantity == 127
     assert patent_term_adjustment.ip_office_day_delay_quantity == 142
 
     assert len(patent_term_adjustment.history) > 0
     for history_item in patent_term_adjustment.history:
         assert isinstance(history_item, TermAdjustmentHistory)
@@ -201,17 +189,15 @@
 
 def test_application_biblio(fixture_dir):
     data = json.loads((fixture_dir / "biblio.json").read_text())
     application_biblio_data = data["patentBag"][0]
     application_biblio = USApplicationBiblio(**application_biblio_data)
 
     assert application_biblio.aia_indicator is True
-    assert application_biblio.app_filing_date == datetime.date.fromisoformat(
-        "2016-09-02"
-    )
+    assert application_biblio.app_filing_date == datetime.date.fromisoformat("2016-09-02")
     assert len(application_biblio.inventors) > 0
     assert application_biblio.customer_number == 26161
     assert application_biblio.group_art_unit == "3775"
     assert application_biblio.invention_title == "TONGUE RETRACTORS FOR FRENOTOMIES"
     assert len(application_biblio.correspondence_address) > 0
     assert application_biblio.app_conf_num == 7229
     assert application_biblio.atty_docket_num == "29539-0122US1"
@@ -239,17 +225,15 @@
     assert application.appl_id == "15123456"
     assert application.first_inventor_name == "Marvin Wang"
     assert application.first_applicant_name == "The General Hospital Corporation"
     assert len(application.cpc_classifications) > 0
     assert application.entity_status == "Small"
     assert application.app_type_code == "UTL"
     assert application.national_stage_indicator is False
-    assert application.effective_filing_date == datetime.date.fromisoformat(
-        "2016-09-02"
-    )
+    assert application.effective_filing_date == datetime.date.fromisoformat("2016-09-02")
     assert len(application.assignments) > 0
     assert len(application.attorneys.attorneys) > 0
     assert len(application.transactions) > 0
     assert len(application.parent_applications) > 0
     assert len(application.child_applications) > 0
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/query.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/odp/query_fields.csv` & `patent_client-5.0.3/patent_client/_async/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/api_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/peds/api_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,19 +8,15 @@
     result = await PatentExaminationDataSystemApi().create_query("applId:(16123456)")
     assert result.num_found == 1
     assert result.applications[0].appl_id == "16123456"
 
 
 @pytest.mark.asyncio
 async def test_can_search_by_customer_number():
-    result = await PatentExaminationDataSystemApi().create_query(
-        "appCustNumber:(70155)"
-    )
+    result = await PatentExaminationDataSystemApi().create_query("appCustNumber:(70155)")
     assert result.num_found > 10
 
 
 @pytest.mark.asyncio
 async def test_can_limit_by_rows():
-    result = await PatentExaminationDataSystemApi().create_query(
-        "appCustNumber:(70155)", rows=5
-    )
+    result = await PatentExaminationDataSystemApi().create_query("appCustNumber:(70155)", rows=5)
     assert len(result.applications) == 5
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.3/patent_client/_async/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.3/patent_client/_async/uspto/peds/fixtures/app_1_output.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'applications'": "{0: {'app_confr_number': '1659'}}"}*

```diff
@@ -1,12 +1,13 @@
 {
     "applications": [
         {
             "app_attr_dock_number": "Suntulit_02",
             "app_cls_sub_cls": "700/276000",
+            "app_confr_number": "1659",
             "app_early_pub_date": "2010-09-16",
             "app_early_pub_number": "US20100235004A1",
             "app_exam_name": "BAHTA, KIDEST",
             "app_filing_date": "2010-03-11",
             "app_grp_art_number": "2127",
             "app_location": "ELECTRONIC",
             "app_status": "Patented Case",
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/peds/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
+import typing as tp
 from collections.abc import Sequence
 from pathlib import Path
 from tempfile import TemporaryDirectory
-import typing as tp
 
 from dateutil.parser import parse as dt_parse
 from pypdf import PdfMerger
 
 from patent_client.util.manager import AsyncManager
 from patent_client.util.request_util import get_start_and_row_count
 
@@ -57,17 +57,15 @@
     async def _get_results(self) -> tp.AsyncIterator["USApplication"]:
         query_params = self.get_query_params()
         api = PatentExaminationDataSystemApi()
         counter = 0
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, page_size=20
         ):
-            page = await api.create_query(
-                **{**query_params, "start": start, "rows": rows}
-            )
+            page = await api.create_query(**{**query_params, "start": start, "rows": rows})
             for app in page.applications:
                 yield app
                 counter += 1
                 if self.config.limit and counter >= self.config.limit:
                     break
             if len(page.applications) < rows:
                 break
@@ -95,17 +93,15 @@
                 if "__" in k:
                     f, *op = k.split("__")
                     if len(op) > 1:
                         raise ValueError(
                             f"Invalid date filter: {k}={v}; Cannot have more than one operator"
                         )
                     if op[0] not in ("gte", "lte"):
-                        raise ValueError(
-                            f"Invalid date filter: {k}={v}; Invalid operator: {op[0]}"
-                        )
+                        raise ValueError(f"Invalid date filter: {k}={v}; Invalid operator: {op[0]}")
                     if isinstance(v, (list, tuple)):
                         raise ValueError(
                             f"Invalid date filter: {k}={v}; Cannot have multiple values with operator {op[0]}"
                         )
                     date_filter_tuples.append((f, op[0], cast_as_datetime(v)))
                 else:
                     if isinstance(v, (list, tuple)):
@@ -118,29 +114,21 @@
                     else:
                         date_filter_tuples.append((k, "exact", cast_as_datetime(v)))
             # Create pairs of gte/lte filters
             query_date_filter_tuples = set()
             for k, op, v in date_filter_tuples:
                 if op == "gte":
                     lte_query = next(
-                        (
-                            v
-                            for k, op, v in date_filter_tuples
-                            if k == k and op == "lte"
-                        ),
+                        (v for k, op, v in date_filter_tuples if k == k and op == "lte"),
                         "*",
                     )
                     query_date_filter_tuples.add((k, (v, lte_query)))
                 elif op == "lte":
                     gte_query = next(
-                        (
-                            v
-                            for k, op, v in date_filter_tuples
-                            if k == k and op == "gte"
-                        ),
+                        (v for k, op, v in date_filter_tuples if k == k and op == "gte"),
                         "*",
                     )
                     query_date_filter_tuples.add((k, (gte_query, v)))
                 elif op == "exact":
                     query_date_filter_tuples.add((k, (v, v)))
 
             # Create the query string
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/manager_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/peds/manager_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import datetime
 import json
 from collections import OrderedDict
 from pathlib import Path
 
 import pytest
-from pypdf import PdfReader
 
-from .model import PedsPage, USApplication, RemovedDataException
+from .model import PedsPage, RemovedDataException, USApplication
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
 class TestPatentExaminationDataDeserialization:
     def test_application(self):
         input_file = fixtures / "app_1_input.json"
@@ -49,16 +48,15 @@
         assert app.patent_title == "METHOD AND APPARATUS FOR AN L.E.D. FLASHLIGHT"
 
     @pytest.mark.asyncio
     async def test_get_by_application_number(self):
         app_no = "15145443"
         app = await USApplication.objects.get(app_no)
         assert (
-            app.patent_title
-            == "Suction and Discharge Lines for a Dual Hydraulic Fracturing Unit"
+            app.patent_title == "Suction and Discharge Lines for a Dual Hydraulic Fracturing Unit"
         )
 
     @pytest.mark.asyncio
     async def test_get_many_by_application_number(self):
         app_nos = ["14971450", "15332765", "13441334", "15332709", "14542000"]
         data = USApplication.objects.filter(*app_nos)
         assert await data.count() == 5
@@ -225,46 +223,43 @@
         fp = app.foreign_priority
         assert isinstance(fp, list)
         app = fp[0]
         assert app.country_name == "NORWAY"
         assert app.filing_date == datetime.date(2017, 2, 15)
         assert app.priority_claim == "20170229"
 
-
     @pytest.mark.asyncio
     async def test_raises_warning_on_missing_information(self):
         app = await USApplication.objects.get(patent_number=10000000)
         with pytest.raises(RemovedDataException):
             _ = app.expiration
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.attorneys
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.pta_pte_summary
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.pta_pte_tran_history
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.parent_continuity
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.child_continuity
 
+
 class TestDocuments:
     @pytest.mark.vcr
     async def test_can_get_document_listing(self):
         app = await USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         assert await docs.count() > 50
 
     @pytest.mark.vcr
     async def test_can_get_application_from_document(self):
         app = await USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         doc = await docs[5]
         backref_app = await doc.application
         assert app.appl_id == backref_app.appl_id
-
-
-
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/model.py` & `patent_client-5.0.3/patent_client/_async/uspto/peds/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 import datetime
-from pathlib import Path
 import typing as tp
+from pathlib import Path
 
 from async_property import async_property
-from dateutil.relativedelta import relativedelta
-from pydantic import (
-    AliasPath,
-    BeforeValidator,
-    ConfigDict,
-    Field,
-    computed_field,
-    model_validator,
-)
+from pydantic import AliasPath, BeforeValidator, ConfigDict, Field, computed_field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated, Self
 
 from patent_client.util.pydantic_util import BaseModel, Date, DateTime
 
 if tp.TYPE_CHECKING:
     from ...epo.ops.published.model import InpadocBiblio
@@ -111,14 +103,15 @@
 
 
 class USApplication(PEDSBaseModel):
     appl_id: str
     app_filing_date: Date
     app_exam_name: tp.Optional[str] = None
     public_ind: YNBool
+    app_confr_number: tp.Optional[str] = None
     inventor_name: tp.Optional[str] = None
     app_early_pub_number: tp.Optional[str] = None
     app_early_pub_date: tp.Optional[Date] = None
     patent_number: tp.Optional[str] = None
     patent_issue_date: tp.Optional[Date] = None
     app_location: tp.Optional[str] = None
     app_grp_art_number: tp.Optional[str] = None
@@ -142,36 +135,47 @@
     def __repr__(self):
         return f"USApplication(appl_id='{self.appl_id}', patent_title='{self.patent_title}', app_status='{self.app_status}')"
 
     # Data removed by USPTO
 
     @property
     def attorneys(self):
-        raise RemovedDataException("Attorney information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+        raise RemovedDataException(
+            "Attorney information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
 
     @property
     def expiration(self):
-        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def pta_pte_summary(self):
-        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def pta_pte_tran_history(self):
-        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def parent_continuity(self):
-        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def child_continuity(self):
-        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-
+        raise RemovedDataException(
+            "Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
 
     @property
     def patent_center_link(self) -> str:
         return f"https://patentcenter.uspto.gov/applications/{self.appl_id}"
 
     @property
     def google_patents_link(self) -> tp.Optional[str]:
@@ -224,42 +228,36 @@
         return self._get_model(".Document").objects.filter(appl_id=self.appl_id)
 
     @property
     def related_assignments(
         self,
     ) -> tp.Iterable["Assignment"]:
         """Related Assignments from the Assignments API"""
-        return self._get_model("..assignment.model.Assignment").objects.filter(
-            appl_id=self.appl_id
-        )
+        return self._get_model("..assignment.model.Assignment").objects.filter(appl_id=self.appl_id)
 
     @property
     def ptab_proceedings(
         self,
     ) -> tp.Iterable["PtabProceeding"]:
         """Related PtabProceedings for this application"""
-        return self._get_model("..ptab.model.PtabProceeding").objects.filter(
-            appl_id=self.appl_id
-        )
+        return self._get_model("..ptab.model.PtabProceeding").objects.filter(appl_id=self.appl_id)
 
     @property
     def patent(self) -> tp.Optional["Patent"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("..public_search.model.Patent").objects.get(
             publication_number=self.patent_number
         )
 
     @property
     def publication(
         self,
     ) -> tp.Optional["PublishedApplication"]:
         """Fulltext version of the Publication - If Available"""
-        return self._get_model(
-            "..public_search.model.PublishedApplication"
-        ).objects.get(
+        return self._get_model("..public_search.model.PublishedApplication").objects.get(
             publication_number=self.publication_number,
         )
 
     @property
     def inpadoc_patent(
         self,
     ) -> tp.Optional["InpadocBiblio"]:
@@ -286,17 +284,15 @@
             "corrAddrNameLineTwo",
             "corrAddrNameLineThree",
         ]
         values["corrName"] = " ".join(
             [values[field] for field in correspondent_name_fields if field in values]
         )
         correspondent_adddress_lines = "\n".join(
-            values[f]
-            for f in ("corrAddrStreetLineOne", "corrAddrStreetLineTwo")
-            if f in values
+            values[f] for f in ("corrAddrStreetLineOne", "corrAddrStreetLineTwo") if f in values
         )
         correspondent_address_last_line = f"{values.get('corrAddrCity', '')}, {values.get('corrAddrGeoRegionCode', '')} {values.get('corrAddrPostalCode', '')}"
         if "corrAddrCountryName" in values:
             correspondent_address_last_line += f" ({values['corrAddrCountryName']})"
         values["corrAddress"] = "\n".join(
             [correspondent_adddress_lines, correspondent_address_last_line]
         )
@@ -393,14 +389,12 @@
         return await self._get_model(".USApplication").objects.get(
             appl_id=self.application_number_text
         )
 
 
 class PedsPage(PEDSBaseModel):
     num_found: int = Field(
-        validation_alias=AliasPath(
-            "queryResults", "searchResponse", "response", "numFound"
-        )
+        validation_alias=AliasPath("queryResults", "searchResponse", "response", "numFound")
     )
     applications: tp.List[USApplication] = Field(
         validation_alias=AliasPath("queryResults", "searchResponse", "response", "docs")
     )
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/query.py` & `patent_client-5.0.3/patent_client/_async/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/peds/search_index.csv` & `patent_client-5.0.3/patent_client/_async/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,15 @@
             "applicationNumberText": application_number,
             "recordStartNumber": start,
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
 
-        query_dict = update_query_with_date(
-            document_filing_date, "documentFiling", query_dict
-        )
+        query_dict = update_query_with_date(document_filing_date, "documentFiling", query_dict)
 
         response = await client.get(
             url="https://developer.uspto.gov/ptab-api/documents", params=query_dict
         )
         response.raise_for_status()
         return PtabDocumentPage.model_validate_json(response.content)
 
@@ -161,20 +159,16 @@
             "recordStartNumber": start,
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
         query_dict = update_query_with_date(declaration_date, "declaration", query_dict)
         query_dict = update_query_with_date(institution_date, "institution", query_dict)
-        query_dict = update_query_with_date(
-            proceeding_filing_date, "proceedingFiling", query_dict
-        )
-        query_dict = update_query_with_date(
-            accorded_filing_date, "accordedFiling", query_dict
-        )
+        query_dict = update_query_with_date(proceeding_filing_date, "proceedingFiling", query_dict)
+        query_dict = update_query_with_date(accorded_filing_date, "accordedFiling", query_dict)
         query_dict = update_query_with_date(
             proceeding_last_modified_date, "proceedingLastModified", query_dict
         )
         query_dict = update_query_with_date(grant_date, "grant", query_dict)
 
         response = await client.get(
             url="https://developer.uspto.gov/ptab-api/proceedings", params=query_dict
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/api_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,35 +17,30 @@
     instance_schema = None
     api_method: Optional[Callable] = None
 
     async def _get_results(self):
         query = deepcopy(self.config.filter)
         query = peds_to_ptab(query)
         query["sort"] = " ".join(
-            inflection.camelize(o, uppercase_first_letter=False)
-            for o in self.config.order_by
+            inflection.camelize(o, uppercase_first_letter=False) for o in self.config.order_by
         )
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, self.page_size
         ):
             query["start"] = start
             query["rows"] = rows
             page = await self.api_method(**query)
             for doc in page.docs:
                 yield doc
             if len(page.docs) < rows:
                 break
 
     async def count(self):
         page = await self.api_method(**peds_to_ptab(self.config.filter))
-        return (
-            min(self.config.limit, page.num_found)
-            if self.config.limit
-            else page.num_found
-        )
+        return min(self.config.limit, page.num_found) if self.config.limit else page.num_found
 
     # def allowed_filters(self):
     #    params = schema_doc["paths"][self.path]["get"]["parameters"]
     #    return {inflection.underscore(p["name"]): p["description"] for p in params}
 
 
 class PtabProceedingManager(PtabManager[PtabProceeding]):
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/manager_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/manager_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,22 +45,17 @@
     async def test_filter_by_proceeding(self):
         result = PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
         assert await result.count() == 77
 
     @pytest.mark.asyncio
     async def test_sort_by_document_number(self):
         result = (
-            await PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
-            .limit(3)
-            .count()
+            await PtabDocument.objects.filter(proceeding_number="IPR2016-00831").limit(3).count()
         )
         assert result == 3
 
 
 class TestPtabDecision:
     @pytest.mark.asyncio
     async def test_get_by_proceeding(self):
         result = await PtabDecision.objects.get(proceeding_number="IPR2016-00831")
-        assert (
-            result.identifier
-            == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
-        )
+        assert result.identifier == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/ptab/model.py` & `patent_client-5.0.3/patent_client/_async/uspto/ptab/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import re
-from pathlib import Path
 import typing as tp
+from pathlib import Path
 
 from pydantic import BeforeValidator, ConfigDict, Field
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel, DateTime
 
@@ -167,15 +167,17 @@
         filename = filename.encode(encoding="ascii", errors="ignore").decode("ascii")
         filename = fname_re.sub("", filename)
         out_path = Path(path) if path else Path.cwd()
         if out_path.is_dir():
             out_path = Path(path) / filename
         else:
             out_path = out_path
-        download_url = f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
+        download_url = (
+            f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
+        )
         return await client.download(download_url, path=out_path)
 
 
 class PtabDecision(PtabBaseModel):
     proceeding_number: str
     board_rulings: tp.List[str] = Field(default_factory=list)
     decision_type_category: tp.Optional[str] = None
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/api.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,27 @@
 
 class PublicSearchApi:
     def __init__(self):
         self.client = PatentClientSession(
             headers={
                 "X-Requested-With": "XMLHttpRequest",
                 "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+                "Origin": "https://ppubs.uspto.gov",
+                "Referer": "https://ppubs.uspto.gov/pubwebapp/",
+                "Pragma": "no-cache",
+                "Cache-Control": "no-cache",
+                "Priority": "u=1, i",
             },
             http2=True,
             follow_redirects=True,
         )
         self.session = dict()
         self.case_id = None
         self.queries = dict()
-        self.search_query = json.loads(
-            (Path(__file__).parent / "search_query.json").read_text()
-        )
+        self.search_query = json.loads((Path(__file__).parent / "search_query.json").read_text())
 
     async def run_query(
         self,
         query,
         start=0,
         limit=500,
         sort="date_publ desc",
@@ -70,17 +73,15 @@
 
         counts = await self.make_request(
             "POST",
             "https://ppubs.uspto.gov/dirsearch-public/searches/counts",
             json=data["query"],
         )
         counts.raise_for_status()
-        search_url = (
-            "https://ppubs.uspto.gov/dirsearch-public/searches/searchWithBeFamily"
-        )
+        search_url = "https://ppubs.uspto.gov/dirsearch-public/searches/searchWithBeFamily"
         query_response = await self.make_request("POST", search_url, json=data)
         query_response.raise_for_status()
         result = query_response.json()
         if result.get("error", None) is not None:
             raise UsptoException(
                 f"Error #{result['error']['errorCode']}\n{result['error']['errorMessage']}"
             )
@@ -129,15 +130,15 @@
 
     async def _request_save(self, obj):
         page_keys = [
             f"{obj.image_location}/{i:0>8}.tif"
             for i in range(1, obj.document_structure.page_count + 1)
         ]
         response = await self.client.post(
-            "https://ppubs.uspto.gov/dirsearch-public/print/imageviewer",
+            "https://ppubs.uspto.gov/dirsearch-public/internal/print/imageviewer",
             json={
                 "caseId": self.case_id,
                 "pageKeys": page_keys,
                 "patentGuid": obj.guid,
                 "saveOrPrint": "save",
                 "source": obj.type,
             },
@@ -155,30 +156,30 @@
         try:
             print_job_id = await self._request_save(obj)
         except httpx.HTTPStatusError:
             await self.get_session()
             print_job_id = await self._request_save(obj)
         while True:
             response = await self.client.post(
-                "https://ppubs.uspto.gov/dirsearch-public/print/print-process",
+                "https://ppubs.uspto.gov/dirsearch-public/internal/print/print-process",
                 json=[
                     print_job_id,
                 ],
             )
             response.raise_for_status()
             print_data = response.json()
             if print_data[0]["printStatus"] == "COMPLETED":
                 break
             await asyncio.sleep(1)
         pdf_name = print_data[0]["pdfName"]
         with out_path.open("wb") as f:
             try:
                 request = self.client.build_request(
                     "GET",
-                    f"https://ppubs.uspto.gov/dirsearch-public/print/save/{pdf_name}",
+                    f"https://ppubs.uspto.gov/dirsearch-public/internal/print/save/{pdf_name}",
                 )
                 response = await self.client.send(request, stream=True)
                 response.raise_for_status()
                 async for chunk in response.aiter_bytes():
                     if chunk:
                         f.write(chunk)
             except httpx.HTTPStatusError as e:
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/biblio.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/document.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,43 +33,35 @@
 class UsReferenceSchema(ZipSchema):
     publication_number = f.String("urpn")
     # us_class = f.String("usRefClassification")
     # cpc_class = f.String("usRefCpcClassification")
     # group = f.String("usRefGroup")
     pub_month = f.Date(
         "usRefIssueDate",
-        dt_converter=lambda s: datetime.datetime(
-            year=int(s[:4]), month=int(s[4:6]), day=1
-        ),
+        dt_converter=lambda s: datetime.datetime(year=int(s[:4]), month=int(s[4:6]), day=1),
     )
     patentee_name = f.String("usRefPatenteeName")
     cited_by_examiner = f.Boolean("usRefGroup", true_func=lambda s: "examiner" in s)
 
 
 class ForeignReferenceSchema(ZipSchema):
     citation_classification = f.String("foreignRefCitationClassification")
     citation_cpc = f.String("foreignRefCitationCpc")
     country_code = f.String("foreignRefCountryCode")
     # group = f.String("foreignRefGroup")
     patent_number = f.String("foreignRefPatentNumber")
     pub_month = f.Date(
         "foreignRefPubDate",
-        dt_converter=lambda s: datetime.datetime(
-            year=int(s[:4]), month=int(s[4:6]), day=1
-        ),
-    )
-    cited_by_examiner = f.Boolean(
-        "foreignRefGroup", true_func=lambda s: "examiner" in s
+        dt_converter=lambda s: datetime.datetime(year=int(s[:4]), month=int(s[4:6]), day=1),
     )
+    cited_by_examiner = f.Boolean("foreignRefGroup", true_func=lambda s: "examiner" in s)
 
 
 class NplReferenceSchema(RegexSchema):
-    __regex__ = (
-        r"(?P<citation>.*)(?P<cited_by_examiner>cited by (applicant|examiner).?$)"
-    )
+    __regex__ = r"(?P<citation>.*)(?P<cited_by_examiner>cited by (applicant|examiner).?$)"
     citation = f.String()
     cited_by_examiner = f.Bool(true_func=lambda s: "examiner" in s)
 
 
 class RelatedApplicationSchema(ZipSchema):
     child_patent_country = f.String("relatedApplChildPatentCountry")
     child_patent_number = f.String("relatedApplChildPatentNumber")
@@ -166,30 +158,22 @@
     composite_id = f.String("compositeId")
     database_name = f.String("databaseName")
     derwent_week_int = f.Integer("derwentWeekInt")
 
     # References Cited
     us_references = UsReferenceSchema(data_key=False)
     foreign_references = ForeignReferenceSchema(data_key=False)
-    npl_references = f.DelimitedString(
-        NplReferenceSchema, "otherRefPub.0", delimeter="<br />"
-    )
+    npl_references = f.DelimitedString(NplReferenceSchema, "otherRefPub.0", delimeter="<br />")
 
     # Classifications
     cpc_inventive = f.List(CpcCodeSchema)
     cpc_additional = f.List(CpcCodeSchema)
 
     intl_class_issued = f.DelimitedString(f.String, "ipcCodeFlattened", delimeter=";")
-    intl_class_current_primary = f.List(
-        IntlCodeSchema, "curIntlPatentClassificationPrimary"
-    )
-    intl_class_currrent_secondary = f.List(
-        IntlCodeSchema, "curIntlPatentClassificationSecondary"
-    )
+    intl_class_current_primary = f.List(IntlCodeSchema, "curIntlPatentClassificationPrimary")
+    intl_class_currrent_secondary = f.List(IntlCodeSchema, "curIntlPatentClassificationSecondary")
 
-    us_class_current = f.DelimitedString(
-        f.Str(), "uspcFullClassificationFlattened", delimeter=";"
-    )
+    us_class_current = f.DelimitedString(f.Str(), "uspcFullClassificationFlattened", delimeter=";")
     us_class_issued = f.List(f.Str, "issuedUsClassificationFull")
 
     field_of_search_us = f.List(f.Str(), "fieldOfSearchClassSubclassHighlights")
     field_of_search_cpc = f.List(f.Str(), "fieldOfSearchCpcClassification")
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert/shared.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/convert_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/count_query.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/manager.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,15 @@
             yield doc
 
 
 class PublicSearchBiblioManager(GenericPublicSearchBiblioManager[PublicSearchBiblio]):
     pass
 
 
-class PublicSearchDocumentManager(
-    GenericPublicSearchDocumentManager[PublicSearchDocument]
-):
+class PublicSearchDocumentManager(GenericPublicSearchDocumentManager[PublicSearchDocument]):
     pass
 
 
 class PatentBiblioManager(GenericPublicSearchBiblioManager[PatentBiblio]):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
@@ -128,15 +126,13 @@
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "US-PGPUB",
         ]
 
 
-class PublishedApplicationManager(
-    GenericPublicSearchDocumentManager[PublishedApplication]
-):
+class PublishedApplicationManager(GenericPublicSearchDocumentManager[PublishedApplication]):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "US-PGPUB",
         ]
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/manager_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,15 @@
         pat = await Patent.objects.get(6460631)
         for claim in pat.claims:
             pass
         assert True
 
     @pytest.mark.asyncio
     async def test_handles_search_without_results(self):
-        query = Patent.objects.filter(
-            query='"379/56".CCLS. AND @APD>=19700101<=19950928'
-        )
+        query = Patent.objects.filter(query='"379/56".CCLS. AND @APD>=19700101<=19950928')
         assert await query.count() == 0
 
     @pytest.mark.asyncio
     async def test_can_get_forward_references(self):
         pat = await Patent.objects.get(6103599)
         forward_refs = pat.forward_citations
         assert await forward_refs.count() >= 100
@@ -121,28 +119,24 @@
     async def test_can_get_design_patents(self):
         pat = await Patent.objects.get("D645062")
         assert pat.patent_title == "Gripping arm"
         assert pat.appl_id == "29380046"
 
     @pytest.mark.asyncio
     async def test_search_that_has_single_patent(self):
-        result = Patent.objects.filter(
-            title="tennis", issue_date="2010-01-01->2010-02-27"
-        )
+        result = Patent.objects.filter(title="tennis", issue_date="2010-01-01->2010-02-27")
         assert await result.count() == 1
         obj = await result.first()
         assert obj.publication_number == "7658211"
         assert obj.patent_title == "Tennis ball recharging apparatus method"
 
-    @pytest.mark.skip("This test is too slow")
-    @pytest.mark.no_vcr
     @pytest.mark.asyncio
     async def test_can_get_images(self, tmp_path):
         pat = await Patent.objects.get("6103599")
-        path = await pat.adownload_images(path=tmp_path)
+        path = await pat.download_images(path=tmp_path)
         assert path == tmp_path / "US-6103599-A.pdf"
         assert path.exists()
 
 
 class TestPublishedApplicationFullTextAsync:
     @pytest.mark.asyncio
     async def test_fetch_publication(self):
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/__init__.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/model/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 
 __all__ = [
     "PatentBiblio",
     "Patent",
     "PublishedApplicationBiblio",
     "PublishedApplication",
     "PublicSearchBiblio",
+    "PublicSearchBiblioPage",
     "PublicSearchDocument",
     "PublicSearchDocument",
 ]
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/biblio.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/model/biblio.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,26 @@
 from typing import Optional
 
 from pydantic import AliasPath, Field, model_validator
 
 from patent_client.util.pydantic_util import BaseModel
 
 from ..convert.biblio import PublicSearchBiblioPageSchema
-from .shared import (
-    ApplicationNumber,
-    DateTimeAsDate,
-    DocumentStructure,
-    HtmlString,
-    OptionalList,
-)
+from .shared import ApplicationNumber, DateTimeAsDate, DocumentStructure, HtmlString, OptionalList
 
 
 class PublicSearchBiblio(BaseModel):
     guid: Optional[str] = None
     publication_number: Optional[str] = None
     publication_date: Optional[datetime.date] = None
     patent_title: Optional[HtmlString] = None
     type: Optional[str] = None
     main_classification_code: Optional[str] = None
-    applicant_names: OptionalList[str] = Field(
-        alias="applicant_name", default_factory=list
-    )
-    assignee_names: OptionalList[str] = Field(
-        alias="assignee_name", default_factory=list
-    )
+    applicant_names: OptionalList[str] = Field(alias="applicant_name", default_factory=list)
+    assignee_names: OptionalList[str] = Field(alias="assignee_name", default_factory=list)
     uspc_full_classification: OptionalList[str] = Field(default_factory=list)
     ipc_code: OptionalList[str] = Field(default_factory=list)
     cpc_additional: OptionalList[str] = Field(default_factory=list)
     app_filing_date: Optional[datetime.date] = None
     related_appl_filing_date: OptionalList[DateTimeAsDate] = Field(
         alias="relatedApplFilingDate", default_factory=list
     )
@@ -57,17 +47,17 @@
 
     @property
     def application(self):
         return self._get_model("...peds.model.USApplication").objects.get(self.appl_id)
 
     @property
     def global_dossier(self):
-        return self._get_model(
-            "...global_dossier.model.GlobalDossierApplication"
-        ).objects.get(self.appl_id)
+        return self._get_model("...global_dossier.model.GlobalDossierApplication").objects.get(
+            self.appl_id
+        )
 
     @property
     def assignments(self):
         return self._get_model("...assignment.model.Assignment").objects.filter(
             appl_id=self.appl_id
         )
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/document.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/model/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,17 +200,17 @@
 
     @property
     def application(self):
         return self._get_model("...peds.model.USApplication").objects.get(self.appl_id)
 
     @property
     def global_dossier(self):
-        return self._get_model(
-            "...global_dossier.model.GlobalDossierApplication"
-        ).objects.get(self.appl_id)
+        return self._get_model("...global_dossier.model.GlobalDossierApplication").objects.get(
+            self.appl_id
+        )
 
     @property
     def assignments(self):
         return self._get_model("...assignment.model.Assignment").objects.filter(
             appl_id=self.appl_id
         )
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/model/shared.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/model/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         str_strip_whitespace=True,
     )
 
 
 T = TypeVar("T")
 
 
-OptionalList = Annotated[
-    List[T], BeforeValidator(lambda x: x if isinstance(x, list) else list())
-]
+OptionalList = Annotated[List[T], BeforeValidator(lambda x: x if isinstance(x, list) else list())]
 DateTimeAsDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: x.date() if isinstance(x, datetime.datetime) else x),
 ]
 HtmlString = Annotated[str, BeforeValidator(html_to_text)]
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/model_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/query.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 
 class QueryBuilder:
     def __init__(self):
         config_file = Path(__file__).parent / "query_config.csv"
         with config_file.open(encoding="utf-8-sig") as csvfile:
             reader = csv.DictReader(csvfile)
             config = list(reader)
-        self.search_keywords = {
-            r["keyword"]: r["query_field"] for r in config if r["query_field"]
-        }
+        self.search_keywords = {r["keyword"]: r["query_field"] for r in config if r["query_field"]}
         self.order_by_keywords = {
             r["keyword"]: r["order_by_field"] for r in config if r["order_by_field"]
         }
         self.date_fields = [r["keyword"] for r in config if r["is_date"] == "X"]
 
     def convert_date(self, date):
         if isinstance(date, str):
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/query_config.csv` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/query_test.py` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/query_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,63 +7,51 @@
 
 class QueryTest:
     def test_default_query(self):
         assert PatentBiblioManager().filter("6103599")._query == '"6103599".PN.'
 
     def test_plural_default_query(self):
         assert (
-            PatentBiblioManager().filter("6103599", "6103600")._query
-            == '("6103599" "6103600").PN.'
+            PatentBiblioManager().filter("6103599", "6103600")._query == '("6103599" "6103600").PN.'
         )
 
     def test_keyword_query(self):
-        assert (
-            PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
-        )
+        assert PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
 
     def test_plural_keyword_query(self):
         assert (
             PatentBiblioManager().filter(appl_id=("11111111", "11222222"))._query
             == '("11111111" "11222222").APNR.'
         )
 
     def test_keyword_date_query(self):
         assert (
-            PatentBiblioManager().filter(app_filing_date="2021-01-01")._query
-            == '@APD="20210101"'
+            PatentBiblioManager().filter(app_filing_date="2021-01-01")._query == '@APD="20210101"'
         )
         assert (
             PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01"))._query
             == '@APD="20210101"'
         )
         assert (
-            PatentBiblioManager()
-            .filter(app_filing_date=parse_dt("2021-01-01").date())
-            ._query
+            PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01").date())._query
             == '@APD="20210101"'
         )
 
     def test_keyword_date_range_query(self):
         assert (
-            PatentBiblioManager()
-            .filter(app_filing_date="2021-01-01->2021-02-01")
-            ._query
+            PatentBiblioManager().filter(app_filing_date="2021-01-01->2021-02-01")._query
             == "@APD>=20210101<=20210201"
         )
         assert (
-            PatentBiblioManager()
-            .filter(app_filing_date__range=("2021-01-01", "2021-02-01"))
-            ._query
+            PatentBiblioManager().filter(app_filing_date__range=("2021-01-01", "2021-02-01"))._query
             == "@APD>=20210101<=20210201"
         )
         assert (
             PatentBiblioManager()
-            .filter(
-                app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01"))
-            )
+            .filter(app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01")))
             ._query
             == "@APD>=20210101<=20210201"
         )
 
     def test_date_operator_queries(self):
         assert (
             PatentBiblioManager().filter(app_filing_date__gt="2021-01-01")._query
@@ -94,38 +82,30 @@
 
     def test_multiple_fields(self):
         assert (
             PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
             == '@APD="20210101" AND "6103599".PN.'
         )
         assert (
-            PatentBiblioManager()
-            .filter("6103599")
-            .filter(app_filing_date="2021-01-01")
-            ._query
+            PatentBiblioManager().filter("6103599").filter(app_filing_date="2021-01-01")._query
             == '"6103599".PN. AND @APD="20210101"'
         )
         assert (
             PatentBiblioManager()
             .filter(patent_number="6103599", app_filing_date="2021-01-01")
             ._query
             == '@APD="20210101" AND "6103599".PN.'
         )
 
     def test_raw_query(self):
-        assert (
-            PatentBiblioManager().filter(query="example query")._query
-            == "example query"
-        )
+        assert PatentBiblioManager().filter(query="example query")._query == "example query"
 
     def test_raw_query_with_keywords(self):
         assert (
-            PatentBiblioManager()
-            .filter(query="some text", patent_number="6103599")
-            ._query
+            PatentBiblioManager().filter(query="some text", patent_number="6103599")._query
             == '"6103599".PN. AND some text'
         )
 
     def test_default_or(self):
         assert (
             PatentBiblioManager()
             .option(default_operator="OR")
```

### Comparing `patent_client-5.0.2/patent_client/_async/uspto/public_search/search_query.json` & `patent_client-5.0.3/patent_client/_async/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/__init__.py` & `patent_client-5.0.3/patent_client/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/__init__.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/api.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,12 +7,10 @@
 from ..session import session
 from .model import Family
 
 
 class FamilyAsyncApi:
     @classmethod
     def get_family(cls, number, doc_type="publication", format="docdb"):
-        url = (
-            f"http://ops.epo.org/3.2/rest-services/family/{doc_type}/{format}/{number}"
-        )
+        url = f"http://ops.epo.org/3.2/rest-services/family/{doc_type}/{format}/{number}"
         response = session.get(url)
         return Family.model_validate(response.text)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/api_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/api_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/epo/ops/family/api_test.py         *
 # ********************************************************************************
 
 import json
 from pathlib import Path
 
-import pytest
-
 from .api import FamilyAsyncApi
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
-
 def test_api():
     result = FamilyAsyncApi.get_family("EP1000000A1")
     expected_file = fixtures / "family_api_output.json"
     # expected_file.write_text(result.model_dump_json(indent=2))
     expected = expected_file.read_text()
     assert json.loads(expected) == json.loads(result.model_dump_json())
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/manager.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,10 +11,8 @@
 from .schema import FamilySchema
 
 
 class FamilyManager(Manager[Family]):
     __schema__ = FamilySchema
 
     def get(self, doc_number):
-        return FamilyAsyncApi.get_family(
-            doc_number, doc_type="publication", format="docdb"
-        )
+        return FamilyAsyncApi.get_family(doc_number, doc_type="publication", format="docdb")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/model.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/model_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/model_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 # *                             DO NOT MANUALLY EDIT                             *
 # *        Source File: patent_client/_async/epo/ops/family/model_test.py        *
 # ********************************************************************************
 
 import json
 from pathlib import Path
 
-import pytest
-
 from patent_client.util.test import compare_dicts
 
 from .model import Family
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
-
 def test_model():
     result = Family.objects.get("EP1000000A1")
     expected_file = fixtures / "family_model_output.json"
     # expected_file.write_text(result.model_dump_json(indent=2))
     expected = json.loads(expected_file.read_text())
     compare_dicts(json.loads(result.model_dump_json()), expected)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,19 @@
     publication_number = DocDbNumberField(
         './/epo:publication-reference/epo:document-id[@document-id-type="docdb"]'
     )
     application_number = DocDbNumberField(
         './/epo:application-reference/epo:document-id[@document-id-type="docdb"]'
     )
     family_id = f.Str("./@family-id")
-    publication_reference = f.List(
-        DocumentIdSchema, ".//epo:publication-reference/epo:document-id"
-    )
-    application_reference = f.List(
-        DocumentIdSchema, ".//epo:application-reference/epo:document-id"
-    )
+    publication_reference = f.List(DocumentIdSchema, ".//epo:publication-reference/epo:document-id")
+    application_reference = f.List(DocumentIdSchema, ".//epo:application-reference/epo:document-id")
     priority_claims = f.List(PriorityClaimSchema, ".//epo:priority-claim")
 
 
 class FamilySchema(Schema):
-    publication_reference = DocumentIdSchema(
-        ".//ops:patent-family/ops:publication-reference"
-    )
+    publication_reference = DocumentIdSchema(".//ops:patent-family/ops:publication-reference")
     num_records = f.Int(".//ops:patent-family/@total-result-count")
     publication_number = DocDbNumberField(
         './/ops:patent-family/ops:publication-reference/epo:document-id[@document-id-type="docdb"]'
     )
     family_members = f.List(FamilyMemberSchema, ".//ops:family-member")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/family/schema_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/api_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/api_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/epo/ops/legal/api_test.py          *
 # ********************************************************************************
 
 from pathlib import Path
 
-import pytest
-
 from .api import LegalApi
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
-
 def test_async_example():
     result = LegalApi.get_legal("EP1000000A1")
     assert str(result.publication_reference) == "EP1000000A1"
     assert len(result.events) >= 50
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/manager.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,13 +12,9 @@
 from .model import LegalEvent
 from .schema import LegalSchema
 
 
 class LegalManager(Manager):
     __schema__ = LegalSchema
 
-    def get(
-        self, doc_number, doc_type="publication", format="docdb"
-    ) -> ListCollection[LegalEvent]:
-        return self.__schema__.load(
-            LegalApi.get_legal(doc_number, doc_type, format)
-        ).events
+    def get(self, doc_number, doc_type="publication", format="docdb") -> ListCollection[LegalEvent]:
+        return self.__schema__.load(LegalApi.get_legal(doc_number, doc_type, format)).events
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/model.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/national_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *      Source File: patent_client/_async/epo/ops/legal/national_codes.py       *
 # ********************************************************************************
 
-import asyncio
 import datetime
 import logging
 import re
 import sqlite3
 from pathlib import Path
 
 import lxml.etree as ET
@@ -37,71 +36,59 @@
 def generate_legal_code_db():
     current = has_current_spreadsheet()
     if current:
         logger.info("Legal Code Database is Current - skipping database creation")
         return
     else:
         try:
-            logger.info(
-                "Legal Code Database is out of date - creating legal code database"
-            )
+            logger.info("Legal Code Database is out of date - creating legal code database")
             path = get_spreadsheet()
         except Exception:
             logger.exception(
                 "Could not find live code file - falling back to default dated 2023-11-05"
             )
-            path = (
-                Path(__file__).parent
-                / "fixtures"
-                / "legal_code_descriptions_202417.xlsx"
-            )
+            path = Path(__file__).parent / "fixtures" / "legal_code_descriptions_202417.xlsx"
         create_code_database(path)
 
 
 def has_current_spreadsheet():
     con = sqlite3.connect(db_location, timeout=30)
     cur = con.cursor()
     try:
         fname = cur.execute("SELECT * FROM meta").fetchone()[0]
-        date_string = re.search(r"legal_code_descriptions_([\d-]+)\.xlsx", fname).group(
-            1
-        )
+        date_string = re.search(r"legal_code_descriptions_([\d-]+)\.xlsx", fname).group(1)
         try:
             date = datetime.datetime.strptime(date_string, "%Y-%W-%w").date()
-        except (
-            ValueError
-        ):  # Indicates using an older format and database needs to be updated
+        except ValueError:  # Indicates using an older format and database needs to be updated
             return False
         age = datetime.datetime.now().date() - date
         logger.debug(f"Legal Code Database is {age} days old")
         return age.days < 7
     except (sqlite3.OperationalError, TypeError):
         return False
 
 
 def get_spreadsheet_from_epo_website() -> tuple[datetime.date, str]:
     url = "https://www.epo.org/searching-for-patents/data/coverage/weekly.html"
     response = session.get(url)
     response.raise_for_status()
     tree = ET.HTML(response.text)
-    date_string = tree.xpath(
-        ".//tr/td[contains(text(), 'Legal event codes')]/../td[4]"
-    )[0].text.strip()
+    date_string = tree.xpath(".//tr/td[contains(text(), 'Legal event codes')]/../td[4]")[
+        0
+    ].text.strip()
     week, year = date_string.split()[1].split("/")
     date = datetime.datetime.strptime(f"{year}-{week}-0", "%Y-%W-%w").date()
     excel_url = tree.xpath('.//a[contains(@href, "Legal-event-codes")][1]/@href')[0]
     logger.info(f"Found new spreadsheet for {date.isoformat()}: {excel_url}")
     return (date, excel_url)
 
 
 def get_spreadsheet() -> tuple[datetime.date, Path]:
     date, excel_url = get_spreadsheet_from_epo_website()
-    out_path = (
-        legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
-    )
+    out_path = legal_code_dir / f"legal_code_descriptions_{date.strftime('%Y-%W-%w')}.xlsx"
     if out_path.exists():
         logger.info(f"File already downloaded! Current as of {date.isoformat()}")
         return out_path
     out_path = session.download(excel_url, path=out_path)
     logger.info(f"Downloaded new live code file for date {date.isoformat()}")
     return out_path
 
@@ -117,18 +104,18 @@
     except (sqlite3.OperationalError, TypeError):
         pass
 
     cur.execute("CREATE TABLE IF NOT EXISTS meta (file_name text)")
     cur.execute("INSERT INTO meta values (?)", (excel_path.name,))
     wb = load_workbook(excel_path)
     data = list(
-        tuple(i.strip() for i in r)
-        for r in wb[wb.sheetnames[0]].iter_rows(values_only=True)
+        tuple(i.strip() for i in r) for r in wb[wb.sheetnames[0]].iter_rows(values_only=True)
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
@@ -137,17 +124,15 @@
     last_update_orig text,
     event_class text,
     event_class_description text)"""
     )
     cur.execute(
         """CREATE INDEX IF NOT EXISTS country_event_code ON legal_codes (country_code, event_code)"""
     )
-    cur.executemany(
-        "INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows
-    )
+    cur.executemany("INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows)
     con.commit()
 
 
 class LegalCodes:
     def __init__(self):
         self.initialized = False
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/national_codes_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/national_codes_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *    Source File: patent_client/_async/epo/ops/legal/national_codes_test.py    *
 # ********************************************************************************
 
 import datetime
 
-import pytest
-
 from ..legal import national_codes
 
 
 def stub_date():
     return datetime.datetime(2022, 8, 1).date()
 
 
 def test_legal_codes():
     dt = national_codes.current_date
     national_codes.current_date = stub_date
     national_codes.current_date = dt
 
 
-
 def test_epo_website_parsing():
     sp_date, sp_url = national_codes.get_spreadsheet_from_epo_website()
     assert isinstance(sp_date, datetime.date)
     assert isinstance(sp_url, str)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,23 +105,19 @@
     extension_states = f.Str(".//ops:L524EP", formatter=lambda x: x.split(" "))
     effective_date = f.Date(".//ops:L525EP")
     date_of_withdrawal = f.Str(".//ops:L526EP")
 
     def deserialize(self, obj) -> "Dict":
         obj = super().deserialize(obj)
         if obj.event_code == "REG":
-            code_data = code_db.get_code_data(
-                obj.event_country, obj.regional_event_code
-            )
+            code_data = code_db.get_code_data(obj.event_country, obj.regional_event_code)
             obj["event_code"] = obj.event_country + "." + obj.regional_event_code
         else:
             code_data = code_db.get_code_data(obj.country_code, obj.event_code)
             obj["event_code"] = obj.country_code + "." + obj.event_code
         obj["event_description"] = code_data["description"]
         return obj
 
 
 class LegalSchema(Schema):
-    publication_reference = DocumentIdSchema(
-        ".//ops:patent-family/ops:publication-reference"
-    )
+    publication_reference = DocumentIdSchema(".//ops:patent-family/ops:publication-reference")
     events = f.List(LegalEventSchema, ".//ops:legal")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/schema_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/legal/util.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/legal/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/api_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/api_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *     Source File: patent_client/_async/epo/ops/number_service/api_test.py     *
 # ********************************************************************************
 
-import pytest
 
 from .api import NumberServiceApi
 
 
 class TestNumberServiceApi:
-    
     def test_docdb_to_epodoc(self):
         actual = NumberServiceApi.convert_number(
             "MD.20050130.A.20050130", "application", "docdb", "epodoc"
         )
         assert not actual.messages
         assert actual.input_doc.id_type == "docdb"
         assert actual.output_doc.id_type == "epodoc"
 
-    
     def test_original_to_docdb(self):
         actual = NumberServiceApi.convert_number(
             "JP.(2006-147056).A.20060526", "application", "original", "docdb"
         )
         assert not actual.messages
         assert actual.input_doc.id_type == "original"
         assert actual.output_doc.id_type == "docdb"
 
-    
     def test_docdb_to_original(self):
         actual = NumberServiceApi.convert_number(
             "JP.2006147056.A.20060526", "application", "docdb", "original"
         )
         assert not actual.messages
         assert actual.input_doc.id_type == "docdb"
         assert actual.output_doc.id_type == "original"
 
-    
     def test_original_to_epodoc(self):
         actual = NumberServiceApi.convert_number(
             "US.(08/921,321).A.19970829", "application", "original", "epodoc"
         )
         assert not actual.messages
         assert actual.input_doc.id_type == "original"
         assert actual.output_doc.id_type == "epodoc"
 
-    
     def test_original_to_docdb_pct(self):
         actual = NumberServiceApi.convert_number(
             "PCT/GB02/04635.20021011", "application", "original", "docdb"
         )
         assert actual.input_doc.id_type == "original"
         assert actual.output_doc.id_type == "docdb"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/errors.txt` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/messages.txt` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/model.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/number_service/schema.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/api.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,25 @@
         """Published Data Constituents API
         number: document number to search
         doc_type: document type (application / publication)
         format: document number format (original / docdb / epodoc)
         constituents: what data to retrieve. Can be combined. (biblio / abstract / full-cycle)
 
         """
-        base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/"
+        base_url = (
+            f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/"
+        )
         if isinstance(constituents, str):
             constituents = (constituents,)
         url = base_url + ",".join(constituents)
         response = session.get(url)
         return response.text
 
     @classmethod
-    def get_biblio(
-        cls, number, doc_type="publication", format="docdb"
-    ) -> "BiblioResult":
+    def get_biblio(cls, number, doc_type="publication", format="docdb") -> "BiblioResult":
         text = cls.get_constituents(number, doc_type, format, constituents="biblio")
         return BiblioResult.model_validate(text)
 
     @classmethod
     def get_abstract(cls, number, doc_type="publication", format="docdb"):
         return cls.get_constituents(number, doc_type, format, constituents="abstract")
 
@@ -118,17 +118,15 @@
     @classmethod
     def get_images(cls, number, doc_type="publication", format="docdb"):
         base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/images"
         response = session.get(base_url)
         return Images.model_validate(response.text)
 
     @classmethod
-    def get_page_image(
-        cls, country, number, kind, image_type, page_number, image_format="pdf"
-    ):
+    def get_page_image(cls, country, number, kind, image_type, page_number, image_format="pdf"):
         response = session.get(
             f"https://ops.epo.org/3.2/rest-services/published-data/images/{country}/{number}/{kind}/{image_type}.{image_format}",
             params={"Range": page_number},
             extensions={"force_cache": True},
         )
         return BytesIO(response.content)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/api_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/cql.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/fixtures/search_result.xml`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9621666666666666%*

 * *Differences: {"'results'": "{0: {'family_id': '89026819', 'country': 'WO', 'doc_number': '2023231455', 'kind': "*

 * *              "'A1', 'docdb_number': 'WO2023231455A1'}, 1: {'family_id': '89026515', 'country': "*

 * *              "'WO', 'doc_number': '2023230759', 'kind': 'A1', 'docdb_number': 'WO2023230759A1'}, "*

 * *              "2: {'family_id': '88978082', 'country': 'WO', 'doc_number': '2023235868', 'kind': "*

 * *              "'A1', 'docdb_number': 'WO2023235868A1'}, 3: {'family_id': '89025146', 'country': "*

 * *              "'W […]*

```diff
@@ -1,808 +1,808 @@
 {
     "begin": 1,
     "end": 100,
     "num_results": 10000,
     "query": "ti = plastic",
     "results": [
         {
-            "country": "TW",
-            "doc_number": "I833656",
-            "docdb_number": "TWI833656B",
-            "family_id": "90825108",
+            "country": "WO",
+            "doc_number": "2023231455",
+            "docdb_number": "WO2023231455A1",
+            "family_id": "89026819",
             "id_type": "docdb",
-            "kind": "B"
+            "kind": "A1"
         },
         {
-            "country": "TW",
-            "doc_number": "I833389",
-            "docdb_number": "TWI833389B",
-            "family_id": "90627870",
+            "country": "WO",
+            "doc_number": "2023230759",
+            "docdb_number": "WO2023230759A1",
+            "family_id": "89026515",
             "id_type": "docdb",
-            "kind": "B"
+            "kind": "A1"
         },
         {
-            "country": "TW",
-            "doc_number": "M651695",
-            "docdb_number": "TWM651695U",
-            "family_id": "90823799",
+            "country": "WO",
+            "doc_number": "2023235868",
+            "docdb_number": "WO2023235868A1",
+            "family_id": "88978082",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "A1"
         },
         {
-            "country": "TW",
-            "doc_number": "M651049",
-            "docdb_number": "TWM651049U",
-            "family_id": "88753474",
+            "country": "WO",
+            "doc_number": "2023234696",
+            "docdb_number": "WO2023234696A1",
+            "family_id": "89025146",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "A1"
         },
         {
             "country": "TW",
-            "doc_number": "M651104",
-            "docdb_number": "TWM651104U",
-            "family_id": "90823348",
+            "doc_number": "D208131",
+            "docdb_number": "TWD208131S",
+            "family_id": "89023924",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "S"
         },
         {
-            "country": "TW",
-            "doc_number": "M651078",
-            "docdb_number": "TWM651078U",
-            "family_id": "90823290",
+            "country": "KR",
+            "doc_number": "20230158686",
+            "docdb_number": "KR20230158686A",
+            "family_id": "88982250",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "A"
         },
         {
-            "country": "TW",
-            "doc_number": "M651068",
-            "docdb_number": "TWM651068U",
-            "family_id": "90823284",
+            "country": "KR",
+            "doc_number": "20230158820",
+            "docdb_number": "KR20230158820A",
+            "family_id": "88982191",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "A"
         },
         {
-            "country": "CA",
-            "doc_number": "3235790",
-            "docdb_number": "CA3235790A1",
-            "family_id": "84363069",
+            "country": "KR",
+            "doc_number": "20230159050",
+            "docdb_number": "KR20230159050A",
+            "family_id": "88982153",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "CA",
-            "doc_number": "3236276",
-            "docdb_number": "CA3236276A1",
-            "family_id": "80446795",
+            "country": "HR",
+            "doc_number": "P20231011",
+            "docdb_number": "HRP20231011T1",
+            "family_id": "88980069",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "T1"
         },
         {
-            "country": "TW",
-            "doc_number": "202405064",
-            "docdb_number": "TW202405064A",
-            "family_id": "90822854",
+            "country": "US",
+            "doc_number": "11837525",
+            "docdb_number": "US11837525B1",
+            "family_id": "88979950",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "B1"
         },
         {
-            "country": "TW",
-            "doc_number": "202404853",
-            "docdb_number": "TW202404853A",
-            "family_id": "86732062",
+            "country": "AU",
+            "doc_number": "2022270981",
+            "docdb_number": "AU2022270981A1",
+            "family_id": "81654922",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "TW",
-            "doc_number": "202404813",
-            "docdb_number": "TW202404813A",
-            "family_id": "90822810",
+            "country": "US",
+            "doc_number": "2023391491",
+            "docdb_number": "US2023391491A1",
+            "family_id": "88978082",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "PL",
-            "doc_number": "4103490",
-            "docdb_number": "PL4103490T3",
-            "family_id": "74550685",
+            "country": "US",
+            "doc_number": "2023391030",
+            "docdb_number": "US2023391030A1",
+            "family_id": "81207908",
             "id_type": "docdb",
-            "kind": "T3"
+            "kind": "A1"
         },
         {
-            "country": "PL",
-            "doc_number": "131036",
-            "docdb_number": "PL131036U1",
-            "family_id": "90790628",
+            "country": "US",
+            "doc_number": "2023390974",
+            "docdb_number": "US2023390974A1",
+            "family_id": "83354964",
             "id_type": "docdb",
-            "kind": "U1"
+            "kind": "A1"
         },
         {
-            "country": "PL",
-            "doc_number": "442543",
-            "docdb_number": "PL442543A1",
-            "family_id": "90790589",
+            "country": "US",
+            "doc_number": "2023392648",
+            "docdb_number": "US2023392648A1",
+            "family_id": "77821550",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024086147",
-            "docdb_number": "WO2024086147A1",
-            "family_id": "90738205",
+            "country": "US",
+            "doc_number": "2023391702",
+            "docdb_number": "US2023391702A1",
+            "family_id": "85506628",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024085310",
-            "docdb_number": "WO2024085310A1",
-            "family_id": "90737986",
+            "country": "US",
+            "doc_number": "2023391979",
+            "docdb_number": "US2023391979A1",
+            "family_id": "75989882",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024085218",
-            "docdb_number": "WO2024085218A1",
-            "family_id": "90737902",
+            "country": "US",
+            "doc_number": "2023391532",
+            "docdb_number": "US2023391532A1",
+            "family_id": "83510132",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024085131",
-            "docdb_number": "WO2024085131A1",
-            "family_id": "90737893",
+            "country": "US",
+            "doc_number": "2023391531",
+            "docdb_number": "US2023391531A1",
+            "family_id": "88977223",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024085217",
-            "docdb_number": "WO2024085217A1",
-            "family_id": "90737625",
+            "country": "US",
+            "doc_number": "2023395478",
+            "docdb_number": "US2023395478A1",
+            "family_id": "88975952",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024085001",
-            "docdb_number": "WO2024085001A1",
-            "family_id": "90737463",
+            "country": "KR",
+            "doc_number": "20230160071",
+            "docdb_number": "KR20230160071A",
+            "family_id": "88974637",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "MX",
-            "doc_number": "2023008483",
-            "docdb_number": "MX2023008483A",
-            "family_id": "76525546",
+            "country": "KR",
+            "doc_number": "20230159907",
+            "docdb_number": "KR20230159907A",
+            "family_id": "88974607",
             "id_type": "docdb",
             "kind": "A"
         },
         {
-            "country": "MX",
-            "doc_number": "2023008484",
-            "docdb_number": "MX2023008484A",
-            "family_id": "77076147",
+            "country": "KR",
+            "doc_number": "20230160072",
+            "docdb_number": "KR20230160072A",
+            "family_id": "88974484",
             "id_type": "docdb",
             "kind": "A"
         },
         {
-            "country": "MX",
-            "doc_number": "2023006430",
-            "docdb_number": "MX2023006430A",
-            "family_id": "74003695",
+            "country": "KR",
+            "doc_number": "20230158401",
+            "docdb_number": "KR20230158401A",
+            "family_id": "81603573",
             "id_type": "docdb",
             "kind": "A"
         },
         {
-            "country": "MX",
-            "doc_number": "2023007539",
-            "docdb_number": "MX2023007539A",
-            "family_id": "60663297",
+            "country": "KR",
+            "doc_number": "20230158355",
+            "docdb_number": "KR20230158355A",
+            "family_id": "88974316",
             "id_type": "docdb",
             "kind": "A"
         },
         {
-            "country": "CZ",
-            "doc_number": "37828",
-            "docdb_number": "CZ37828U1",
-            "family_id": "90730538",
+            "country": "TW",
+            "doc_number": "D215827",
+            "docdb_number": "TWD215827S",
+            "family_id": "80213908",
             "id_type": "docdb",
-            "kind": "U1"
+            "kind": "S"
         },
         {
-            "country": "CA",
-            "doc_number": "3234950",
-            "docdb_number": "CA3234950A1",
-            "family_id": "78516473",
+            "country": "KR",
+            "doc_number": "20230160548",
+            "docdb_number": "KR20230160548A",
+            "family_id": "88972504",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "CA",
-            "doc_number": "3235168",
-            "docdb_number": "CA3235168A1",
-            "family_id": "84488522",
+            "country": "KR",
+            "doc_number": "102606021",
+            "docdb_number": "KR102606021B1",
+            "family_id": "88972218",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "B1"
         },
         {
-            "country": "PL",
-            "doc_number": "4037981",
-            "docdb_number": "PL4037981T3",
-            "family_id": "68158839",
+            "country": "KR",
+            "doc_number": "102605080",
+            "docdb_number": "KR102605080B1",
+            "family_id": "88972211",
             "id_type": "docdb",
-            "kind": "T3"
+            "kind": "B1"
         },
         {
-            "country": "PL",
-            "doc_number": "4146552",
-            "docdb_number": "PL4146552T3",
-            "family_id": "75787169",
+            "country": "TW",
+            "doc_number": "D213705",
+            "docdb_number": "TWD213705S",
+            "family_id": "83887328",
             "id_type": "docdb",
-            "kind": "T3"
+            "kind": "S"
         },
         {
-            "country": "PL",
-            "doc_number": "3401116",
-            "docdb_number": "PL3401116T3",
-            "family_id": "46598567",
+            "country": "MX",
+            "doc_number": "2022014441",
+            "docdb_number": "MX2022014441A",
+            "family_id": "88970339",
             "id_type": "docdb",
-            "kind": "T3"
+            "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "102657428",
-            "docdb_number": "KR102657428B1",
-            "family_id": "90715742",
+            "doc_number": "20230157558",
+            "docdb_number": "KR20230157558A",
+            "family_id": "88968999",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "102657898",
-            "docdb_number": "KR102657898B1",
-            "family_id": "90715644",
+            "doc_number": "20230157579",
+            "docdb_number": "KR20230157579A",
+            "family_id": "88968995",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "102657430",
-            "docdb_number": "KR102657430B1",
-            "family_id": "90715608",
+            "doc_number": "20230157569",
+            "docdb_number": "KR20230157569A",
+            "family_id": "88968868",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "20240042873",
-            "docdb_number": "KR20240042873A",
-            "family_id": "90714746",
+            "doc_number": "20230157580",
+            "docdb_number": "KR20230157580A",
+            "family_id": "88968785",
             "id_type": "docdb",
             "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "20240046656",
-            "docdb_number": "KR20240046656A",
-            "family_id": "90707720",
+            "doc_number": "20230163168",
+            "docdb_number": "KR20230163168A",
+            "family_id": "88968624",
             "id_type": "docdb",
             "kind": "A"
         },
         {
-            "country": "WO",
-            "doc_number": "2024080444",
-            "docdb_number": "WO2024080444A1",
-            "family_id": "90669705",
+            "country": "KR",
+            "doc_number": "20230163049",
+            "docdb_number": "KR20230163049A",
+            "family_id": "86386898",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "WO",
-            "doc_number": "2024078463",
-            "docdb_number": "WO2024078463A1",
-            "family_id": "90668794",
+            "country": "KR",
+            "doc_number": "20230163169",
+            "docdb_number": "KR20230163169A",
+            "family_id": "88968536",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "WO",
-            "doc_number": "2024077378",
-            "docdb_number": "WO2024077378A1",
-            "family_id": "90668384",
+            "country": "KR",
+            "doc_number": "102607706",
+            "docdb_number": "KR102607706B1",
+            "family_id": "88968322",
+            "id_type": "docdb",
+            "kind": "B1"
+        },
+        {
+            "country": "CA",
+            "doc_number": "3220140",
+            "docdb_number": "CA3220140A1",
+            "family_id": "84323562",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024077341",
-            "docdb_number": "WO2024077341A1",
-            "family_id": "90668376",
+            "country": "CA",
+            "doc_number": "3145627",
+            "docdb_number": "CA3145627A1",
+            "family_id": "80845708",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "102653061",
-            "docdb_number": "KR102653061B1",
-            "family_id": "90666970",
+            "country": "US",
+            "doc_number": "D1006621",
+            "docdb_number": "USD1006621S",
+            "family_id": "87103626",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "S"
         },
         {
-            "country": "KR",
-            "doc_number": "102653566",
-            "docdb_number": "KR102653566B1",
-            "family_id": "90666872",
+            "country": "TW",
+            "doc_number": "I816624",
+            "docdb_number": "TWI816624B",
+            "family_id": "88966242",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "B"
         },
         {
-            "country": "KR",
-            "doc_number": "20240043203",
-            "docdb_number": "KR20240043203A",
-            "family_id": "90662639",
+            "country": "TW",
+            "doc_number": "I815727",
+            "docdb_number": "TWI815727B",
+            "family_id": "88966135",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "B"
         },
         {
             "country": "KR",
-            "doc_number": "20240043548",
-            "docdb_number": "KR20240043548A",
-            "family_id": "90139969",
+            "doc_number": "20230157142",
+            "docdb_number": "KR20230157142A",
+            "family_id": "88964805",
             "id_type": "docdb",
             "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "20240043202",
-            "docdb_number": "KR20240043202A",
-            "family_id": "90662430",
+            "doc_number": "20230157195",
+            "docdb_number": "KR20230157195A",
+            "family_id": "88964710",
             "id_type": "docdb",
             "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "20240000586",
-            "docdb_number": "KR20240000586U",
-            "family_id": "90652216",
+            "doc_number": "102601709",
+            "docdb_number": "KR102601709B1",
+            "family_id": "88964631",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "B1"
         },
         {
             "country": "KR",
-            "doc_number": "20240000585",
-            "docdb_number": "KR20240000585U",
-            "family_id": "90652208",
+            "doc_number": "20230162352",
+            "docdb_number": "KR20230162352A",
+            "family_id": "88957449",
             "id_type": "docdb",
-            "kind": "U"
+            "kind": "A"
         },
         {
             "country": "KR",
-            "doc_number": "20240044024",
-            "docdb_number": "KR20240044024A",
-            "family_id": "90637935",
+            "doc_number": "20230162439",
+            "docdb_number": "KR20230162439A",
+            "family_id": "88957352",
             "id_type": "docdb",
             "kind": "A"
         },
         {
-            "country": "US",
-            "doc_number": "11958035",
-            "docdb_number": "US11958035B1",
-            "family_id": "90628143",
+            "country": "TW",
+            "doc_number": "202334301",
+            "docdb_number": "TW202334301A",
+            "family_id": "73597840",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "A"
         },
         {
             "country": "TW",
-            "doc_number": "D168181",
-            "docdb_number": "TWD168181S",
-            "family_id": "58017128",
+            "doc_number": "202334447",
+            "docdb_number": "TW202334447A",
+            "family_id": "85988655",
             "id_type": "docdb",
-            "kind": "S"
+            "kind": "A"
         },
         {
-            "country": "US",
-            "doc_number": "2024123713",
-            "docdb_number": "US2024123713A1",
-            "family_id": "90627870",
+            "country": "TW",
+            "doc_number": "202336243",
+            "docdb_number": "TW202336243A",
+            "family_id": "86999064",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "US",
-            "doc_number": "2024123703",
-            "docdb_number": "US2024123703A1",
-            "family_id": "82838722",
+            "country": "TW",
+            "doc_number": "202335849",
+            "docdb_number": "TW202335849A",
+            "family_id": "88927282",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
         },
         {
-            "country": "US",
-            "doc_number": "2024123645",
-            "docdb_number": "US2024123645A1",
-            "family_id": "72895926",
+            "country": "TW",
+            "doc_number": "M646076",
+            "docdb_number": "TWM646076U",
+            "family_id": "88926760",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "U"
         },
         {
-            "country": "US",
-            "doc_number": "2024125712",
-            "docdb_number": "US2024125712A1",
-            "family_id": "84393933",
+            "country": "TW",
+            "doc_number": "M645830",
+            "docdb_number": "TWM645830U",
+            "family_id": "88926690",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "U"
         },
         {
-            "country": "US",
-            "doc_number": "2024124777",
-            "docdb_number": "US2024124777A1",
-            "family_id": "74844690",
+            "country": "TW",
+            "doc_number": "M645929",
+            "docdb_number": "TWM645929U",
+            "family_id": "88926588",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "U"
         },
         {
-            "country": "US",
-            "doc_number": "2024124695",
-            "docdb_number": "US2024124695A1",
-            "family_id": "75625462",
+            "country": "ZA",
+            "doc_number": "202106100",
+            "docdb_number": "ZA202106100B",
+            "family_id": "66091823",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "B"
         },
         {
-            "country": "US",
-            "doc_number": "2024124723",
-            "docdb_number": "US2024124723A1",
-            "family_id": "83227752",
+            "country": "ZA",
+            "doc_number": "202204391",
+            "docdb_number": "ZA202204391B",
+            "family_id": "76522858",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "B"
         },
         {
-            "country": "US",
-            "doc_number": "2024124688",
-            "docdb_number": "US2024124688A1",
-            "family_id": "84271945",
+            "country": "ZA",
+            "doc_number": "202213098",
+            "docdb_number": "ZA202213098B",
+            "family_id": "72178808",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "B"
         },
         {
-            "country": "US",
-            "doc_number": "2024124197",
-            "docdb_number": "US2024124197A1",
-            "family_id": "83458920",
+            "country": "RS",
+            "doc_number": "64758",
+            "docdb_number": "RS64758B1",
+            "family_id": "73598767",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "B1"
         },
         {
-            "country": "US",
-            "doc_number": "2024124195",
-            "docdb_number": "US2024124195A1",
-            "family_id": "48944722",
+            "country": "ZA",
+            "doc_number": "202106098",
+            "docdb_number": "ZA202106098B",
+            "family_id": "66091823",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "B"
         },
         {
-            "country": "US",
-            "doc_number": "2024128558",
-            "docdb_number": "US2024128558A1",
-            "family_id": "89573406",
+            "country": "WO",
+            "doc_number": "2023228476",
+            "docdb_number": "WO2023228476A1",
+            "family_id": "85111670",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "CA",
-            "doc_number": "3234486",
-            "docdb_number": "CA3234486A1",
-            "family_id": "86539181",
+            "country": "WO",
+            "doc_number": "2023227805",
+            "docdb_number": "WO2023227805A1",
+            "family_id": "81940880",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "US",
-            "doc_number": "D1022517",
-            "docdb_number": "USD1022517S",
-            "family_id": "90624115",
-            "id_type": "docdb",
-            "kind": "S"
-        },
-        {
-            "country": "CA",
-            "doc_number": "3234581",
-            "docdb_number": "CA3234581A1",
-            "family_id": "84331663",
+            "country": "WO",
+            "doc_number": "2023226291",
+            "docdb_number": "WO2023226291A1",
+            "family_id": "82727028",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "CA",
-            "doc_number": "3204464",
-            "docdb_number": "CA3204464A1",
-            "family_id": "90623930",
+            "country": "WO",
+            "doc_number": "2023225844",
+            "docdb_number": "WO2023225844A1",
+            "family_id": "88918196",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "CA",
-            "doc_number": "3215901",
-            "docdb_number": "CA3215901A1",
-            "family_id": "87973336",
+            "country": "US",
+            "doc_number": "2023380656",
+            "docdb_number": "US2023380656A1",
+            "family_id": "88878034",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "UA",
-            "doc_number": "155739",
-            "docdb_number": "UA155739U",
-            "family_id": "90623846",
-            "id_type": "docdb",
-            "kind": "U"
-        },
-        {
-            "country": "AU",
-            "doc_number": "2022347406",
-            "docdb_number": "AU2022347406A1",
-            "family_id": "85602511",
+            "country": "US",
+            "doc_number": "2023383077",
+            "docdb_number": "US2023383077A1",
+            "family_id": "83320415",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "PL",
-            "doc_number": "4043356",
-            "docdb_number": "PL4043356T3",
-            "family_id": "75108586",
+            "country": "US",
+            "doc_number": "2023383089",
+            "docdb_number": "US2023383089A1",
+            "family_id": "85506628",
             "id_type": "docdb",
-            "kind": "T3"
+            "kind": "A1"
         },
         {
-            "country": "CR",
-            "doc_number": "20230593",
-            "docdb_number": "CR20230593A",
-            "family_id": "84425163",
+            "country": "US",
+            "doc_number": "2023383090",
+            "docdb_number": "US2023383090A1",
+            "family_id": "85506628",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024117259",
-            "docdb_number": "US2024117259A1",
-            "family_id": "74875212",
+            "doc_number": "2023382818",
+            "docdb_number": "US2023382818A1",
+            "family_id": "78212136",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024117245",
-            "docdb_number": "US2024117245A1",
-            "family_id": "90574969",
+            "doc_number": "2023383052",
+            "docdb_number": "US2023383052A1",
+            "family_id": "84979460",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024117254",
-            "docdb_number": "US2024117254A1",
-            "family_id": "88778432",
+            "doc_number": "2023382837",
+            "docdb_number": "US2023382837A1",
+            "family_id": "85506628",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024117139",
-            "docdb_number": "US2024117139A1",
-            "family_id": "88517542",
+            "doc_number": "2023384546",
+            "docdb_number": "US2023384546A1",
+            "family_id": "88877112",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024117179",
-            "docdb_number": "US2024117179A1",
-            "family_id": "90459142",
+            "doc_number": "2023384466",
+            "docdb_number": "US2023384466A1",
+            "family_id": "81207914",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024116665",
-            "docdb_number": "US2024116665A1",
-            "family_id": "87973336",
+            "doc_number": "2023383889",
+            "docdb_number": "US2023383889A1",
+            "family_id": "81974236",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
             "country": "US",
-            "doc_number": "2024116244",
-            "docdb_number": "US2024116244A1",
-            "family_id": "90574599",
+            "doc_number": "2023383546",
+            "docdb_number": "US2023383546A1",
+            "family_id": "88876890",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "US",
-            "doc_number": "2024118485",
-            "docdb_number": "US2024118485A1",
-            "family_id": "82448166",
+            "country": "AU",
+            "doc_number": "2022277645",
+            "docdb_number": "AU2022277645A1",
+            "family_id": "76137890",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "US",
-            "doc_number": "2024120532",
-            "docdb_number": "US2024120532A1",
-            "family_id": "64999236",
+            "country": "AU",
+            "doc_number": "2022277812",
+            "docdb_number": "AU2022277812A1",
+            "family_id": "76137891",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "MX",
-            "doc_number": "2023006084",
-            "docdb_number": "MX2023006084A",
-            "family_id": "74592130",
+            "country": "HU",
+            "doc_number": "2200172",
+            "docdb_number": "HU2200172A1",
+            "family_id": "88875085",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "MX",
-            "doc_number": "2023005974",
-            "docdb_number": "MX2023005974A",
-            "family_id": "78819781",
+            "country": "HU",
+            "doc_number": "2200166",
+            "docdb_number": "HU2200166A1",
+            "family_id": "87519893",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "MX",
-            "doc_number": "2023006468",
-            "docdb_number": "MX2023006468A",
-            "family_id": "73856726",
+            "country": "FI",
+            "doc_number": "3875387",
+            "docdb_number": "FI3875387T3",
+            "family_id": "69770772",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "T3"
         },
         {
             "country": "CA",
-            "doc_number": "3233886",
-            "docdb_number": "CA3233886A1",
-            "family_id": "83121436",
+            "doc_number": "3219909",
+            "docdb_number": "CA3219909A1",
+            "family_id": "84229144",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "MX",
-            "doc_number": "2023002849",
-            "docdb_number": "MX2023002849A",
-            "family_id": "72670467",
-            "id_type": "docdb",
-            "kind": "A"
-        },
-        {
             "country": "PL",
-            "doc_number": "4047156",
-            "docdb_number": "PL4047156T3",
-            "family_id": "80446574",
+            "doc_number": "3733373",
+            "docdb_number": "PL3733373T3",
+            "family_id": "66793748",
             "id_type": "docdb",
             "kind": "T3"
         },
         {
-            "country": "PL",
-            "doc_number": "3894516",
-            "docdb_number": "PL3894516T3",
-            "family_id": "70554000",
+            "country": "US",
+            "doc_number": "11820887",
+            "docdb_number": "US11820887B1",
+            "family_id": "88836477",
             "id_type": "docdb",
-            "kind": "T3"
+            "kind": "B1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240040960",
-            "docdb_number": "KR20240040960A",
-            "family_id": "90483891",
+            "country": "US",
+            "doc_number": "11820888",
+            "docdb_number": "US11820888B1",
+            "family_id": "88836477",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "B1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240036170",
-            "docdb_number": "KR20240036170A",
-            "family_id": "90483457",
+            "country": "WO",
+            "doc_number": "2023224269",
+            "docdb_number": "WO2023224269A1",
+            "family_id": "88835511",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240036252",
-            "docdb_number": "KR20240036252A",
-            "family_id": "90483435",
+            "country": "WO",
+            "doc_number": "2023223909",
+            "docdb_number": "WO2023223909A1",
+            "family_id": "88835391",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240036207",
-            "docdb_number": "KR20240036207A",
-            "family_id": "90483352",
+            "country": "WO",
+            "doc_number": "2023221910",
+            "docdb_number": "WO2023221910A1",
+            "family_id": "88834582",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "102649436",
-            "docdb_number": "KR102649436B1",
-            "family_id": "90483165",
+            "country": "WO",
+            "doc_number": "2023221748",
+            "docdb_number": "WO2023221748A1",
+            "family_id": "82983517",
             "id_type": "docdb",
-            "kind": "B1"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240040566",
-            "docdb_number": "KR20240040566A",
-            "family_id": "90482952",
+            "country": "US",
+            "doc_number": "2023375092",
+            "docdb_number": "US2023375092A1",
+            "family_id": "80632146",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240040472",
-            "docdb_number": "KR20240040472A",
-            "family_id": "90482814",
+            "country": "US",
+            "doc_number": "2023374771",
+            "docdb_number": "US2023374771A1",
+            "family_id": "88792245",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240040296",
-            "docdb_number": "KR20240040296A",
-            "family_id": "90482718",
+            "country": "US",
+            "doc_number": "2023374251",
+            "docdb_number": "US2023374251A1",
+            "family_id": "85506628",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240037778",
-            "docdb_number": "KR20240037778A",
-            "family_id": "90481218",
+            "country": "US",
+            "doc_number": "2023374250",
+            "docdb_number": "US2023374250A1",
+            "family_id": "84979460",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240037446",
-            "docdb_number": "KR20240037446A",
-            "family_id": "90481134",
+            "country": "US",
+            "doc_number": "2023374248",
+            "docdb_number": "US2023374248A1",
+            "family_id": "84539738",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "KR",
-            "doc_number": "20240039757",
-            "docdb_number": "KR20240039757A",
-            "family_id": "90480577",
+            "country": "US",
+            "doc_number": "2023374247",
+            "docdb_number": "US2023374247A1",
+            "family_id": "84979460",
             "id_type": "docdb",
-            "kind": "A"
+            "kind": "A1"
         },
         {
-            "country": "AU",
-            "doc_number": "2022351419",
-            "docdb_number": "AU2022351419A1",
-            "family_id": "78179129",
+            "country": "US",
+            "doc_number": "2023373565",
+            "docdb_number": "US2023373565A1",
+            "family_id": "82116719",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024071294",
-            "docdb_number": "WO2024071294A1",
-            "family_id": "90478098",
+            "country": "US",
+            "doc_number": "2023376701",
+            "docdb_number": "US2023376701A1",
+            "family_id": "72670467",
             "id_type": "docdb",
             "kind": "A1"
         },
         {
-            "country": "WO",
-            "doc_number": "2024071139",
-            "docdb_number": "WO2024071139A1",
-            "family_id": "90478038",
+            "country": "MX",
+            "doc_number": "2022013555",
+            "docdb_number": "MX2022013555A",
+            "family_id": "71096473",
             "id_type": "docdb",
-            "kind": "A1"
+            "kind": "A"
+        },
+        {
+            "country": "MX",
+            "doc_number": "2022013073",
+            "docdb_number": "MX2022013073A",
+            "family_id": "60267871",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "MX",
+            "doc_number": "2022012745",
+            "docdb_number": "MX2022012745A",
+            "family_id": "78221835",
+            "id_type": "docdb",
+            "kind": "A"
         }
     ]
 }
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
         limit = self.config.limit or page.num_results - offset
         num_results = page.num_results
         num_results -= offset
         num_results = min(limit, num_results)
         return num_results
 
     def _get_results(self):
-        for start, end in get_ranges(
-            self.config.limit, self.config.offset, self.result_size
-        ):
+        for start, end in get_ranges(self.config.limit, self.config.offset, self.result_size):
             page = self._get_search_results_range(start, end)
             for result in page.results:
                 yield result
             if len(page.results) < self.result_size:
                 break
 
     def get(self, number, doc_type="publication", format="docdb") -> BiblioResult:
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/__init__.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/biblio.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/fulltext.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/images.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 
     def download(self, path="."):
         from ..api import PublishedImagesApi
 
         out_file = Path(path) / f"{self.doc_number}.pdf"
         writer = PdfWriter()
         for i in range(1, self.num_pages + 1):
-            page_data = PublishedImagesApi.get_page_image_from_link(
-                self.link, page_number=i
-            )
+            page_data = PublishedImagesApi.get_page_image_from_link(self.link, page_number=i)
             page = PdfReader(page_data).pages[0]
             if page["/Rotate"] == 90:
                 page.rotate_clockwise(-90)
             writer.add_page(page)
 
         for section in self.sections:
             writer.add_outline_item(section.name.capitalize(), section.start_page)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/model/search.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/__init__.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/biblio.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/biblio.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,19 +90,15 @@
         './/epo:classification-scheme[@scheme="UC"]/following-sibling::epo:classification-symbol',
     )
     priority_claims = f.List(DocumentIdSchema, ".//epo:priority-claim/epo:document-id")
     title = f.Str('.//epo:invention-title[@lang="en"]')
     titles = f.List(TitleSchema, ".//epo:invention-title")
     abstract = f.Str('.//epo:abstract[@lang="en"]')
     citations = f.List(CitationSchema, ".//epo:citation")
-    applicants_epodoc = f.List(
-        f.Str(), './/epo:applicant[@data-format="epodoc"]//epo:name'
-    )
-    applicants_original = f.List(
-        f.Str(), './/epo:applicant[@data-format="original"]//epo:name'
-    )
+    applicants_epodoc = f.List(f.Str(), './/epo:applicant[@data-format="epodoc"]//epo:name')
+    applicants_original = f.List(f.Str(), './/epo:applicant[@data-format="original"]//epo:name')
     inventors_epodoc = f.List(f.Str(), './/epo:inventor[@data-format="epodoc"]')
     inventors_original = f.List(f.Str(), './/epo:inventor[@data-format="original"]')
 
 
 class BiblioResultSchema(Schema):
     documents = f.List(InpadocBiblioSchema, ".//epo:exchange-document")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/images.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,10 @@
     sections = f.List(SectionSchema, "./ops:document-section")
     doc_number = f.Str("./@link", formatter=get_doc_number)
 
 
 class ImagesSchema(Schema):
     # search_reference = DocumentIdSchema(".//ops:document-inquiry/ops:publication-reference")
     publication_number = DocDbSchema(".//ops:inquiry-result/epo:publication-reference")
-    full_document = ImageDocumentSchema(
-        './/ops:document-instance[@desc="FullDocument"]'
-    )
+    full_document = ImageDocumentSchema('.//ops:document-instance[@desc="FullDocument"]')
     drawing = ImageDocumentSchema('.//ops:document-instance[@desc="Drawing"]')
-    first_page = ImageDocumentSchema(
-        './/ops:document-instance[@desc="FirstPageClipping"]'
-    )
+    first_page = ImageDocumentSchema('.//ops:document-instance[@desc="FirstPageClipping"]')
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema/search.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/schema_test.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/schema_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,15 @@
 from pathlib import Path
 
 import lxml.etree as ET
 import pytest
 
 from patent_client.util.test import compare_dicts
 
-from .schema import (
-    BiblioResultSchema,
-    ClaimsSchema,
-    DescriptionSchema,
-    ImagesSchema,
-    SearchSchema,
-)
+from .schema import BiblioResultSchema, ClaimsSchema, DescriptionSchema, ImagesSchema, SearchSchema
 
 test_dir = Path(__file__).parent / "test"
 expected_dir = Path(__file__).parent / "test" / "expected"
 
 
 def test_biblio():
     tree = ET.parse(test_dir / "biblio_example.xml")
@@ -89,16 +83,15 @@
 
 def test_full_cycle():
     tree = ET.parse(test_dir / "full_cycle_example.xml")
     result = BiblioResultSchema().load(tree)
     assert len(result.documents) == 2
     d = result.documents[0]
     assert (
-        d.title
-        == "Apparatus for manufacturing green bricks for the brick manufacturing industry"
+        d.title == "Apparatus for manufacturing green bricks for the brick manufacturing industry"
     )
 
 
 def test_biblio_2():
     filename = "biblio_example_4"
     input = test_dir / f"{filename}.xml"
     tree = ET.parse(input)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/description_example.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/image_example.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/published/test/search_example.xml` & `patent_client-5.0.3/patent_client/_sync/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/session.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,17 @@
             response = yield self.build_refresh_request()
             if response.status_code != 200:
                 logger.debug(f"EPO Authentication Error!\n{response.text}")
                 raise OpsAuthenticationError(
                     "Failed to authenticate with EPO OPS! Please check your credentials. See the setup instructions at https://patent-client.readthedocs.io/en/stable/getting_started.html"
                 )
             data = response.json()
-            self.expires = dt.datetime.fromtimestamp(
-                int(data["issued_at"]) / 1000
-            ) + dt.timedelta(seconds=int(data["expires_in"]))
+            self.expires = dt.datetime.fromtimestamp(int(data["issued_at"]) / 1000) + dt.timedelta(
+                seconds=int(data["expires_in"])
+            )
             self.authorization_header = f"Bearer {data['access_token']}"
             request.headers["Authorization"] = self.authorization_header
             yield request
 
     def build_refresh_request(self):
         token = base64.b64encode(f"{self.key}:{self.secret}".encode())
         return httpx.Request(
```

### Comparing `patent_client-5.0.2/patent_client/_sync/epo/ops/util.py` & `patent_client-5.0.3/patent_client/_sync/epo/ops/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,46 +52,46 @@
     def biblio(self) -> "InpadocBiblio":
         return self._get_model(
             ".published.model.InpadocBiblio", base_class=InpadocModel
         ).objects.get(self.docdb_number)
 
     @property
     def images(self) -> "Images":
-        return self._get_model(
-            ".published.model.Images", base_class=InpadocModel
-        ).objects.get(self.docdb_number)
+        return self._get_model(".published.model.Images", base_class=InpadocModel).objects.get(
+            self.docdb_number
+        )
 
     @property
     def description(self) -> Optional[str]:
         return (
-            self._get_model(
-                ".published.model.Description", base_class=InpadocModel
-            ).objects.get(self.docdb_number)
+            self._get_model(".published.model.Description", base_class=InpadocModel).objects.get(
+                self.docdb_number
+            )
         ).description
 
     @property
     def claims(self) -> "Claims":
-        return self._get_model(
-            ".published.model.Claims", base_class=InpadocModel
-        ).objects.get(self.docdb_number)
+        return self._get_model(".published.model.Claims", base_class=InpadocModel).objects.get(
+            self.docdb_number
+        )
 
     @property
     def legal(self) -> List["LegalEvent"]:
         return (
             self._get_model(".legal.model.Legal", base_class=InpadocModel).objects.get(
                 self.docdb_number
             )
         ).events
 
     @property
     def family(
         self,
     ) -> List["FamilyMember"]:
         return (
-            self._get_model(
-                ".family.model.Family", base_class=InpadocModel
-            ).objects.get(self.docdb_number)
+            self._get_model(".family.model.Family", base_class=InpadocModel).objects.get(
+                self.docdb_number
+            )
         ).family_members
 
     def download(self, path: str = "."):
         images = self.images
         return images.full_document.download(path)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/http_client.py` & `patent_client-5.0.3/patent_client/_sync/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *               Source File: patent_client/_async/http_client.py               *
 # ********************************************************************************
 
 import re
+import typing as tp
 import warnings
 from hashlib import blake2b
 from pathlib import Path
-import typing as tp
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
@@ -38,17 +38,15 @@
 patent_client_transport = hishel.CacheTransport(
     transport=httpx.HTTPTransport(
         verify=False,
         http2=True,
         retries=3,
     ),
     storage=hishel.FileStorage(base_path=CACHE_DIR),
-    controller=hishel.Controller(
-        allow_heuristics=True, key_generator=cache_key_generator
-    ),
+    controller=hishel.Controller(allow_heuristics=True, key_generator=cache_key_generator),
 )
 
 
 class PatentClientSession(httpx.Client):
     _default_user_agent = f"Mozilla/5.0 Python Patent Clientbot/{__version__} (parkerhancock@users.noreply.github.com)"
 
     def __init__(self, **kwargs):
```

### Comparing `patent_client-5.0.2/patent_client/_sync/odp.py` & `patent_client-5.0.3/patent_client/_sync/odp.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,15 @@
             },
             headers={"Accept": "application/xml"},
         )
         response.raise_for_status()
         return AssignmentPage.model_validate(convert_xml_to_json(response.content))
 
     @classmethod
-    def download_pdf(
-        cls, reel: str, frame: str, path: Optional[Path] = None
-    ) -> Path:
+    def download_pdf(cls, reel: str, frame: str, path: Optional[Path] = None) -> Path:
         url = cls.get_download_url(reel, frame)
 
         if path is None:
             path = Path.cwd()
             output_path = output_path = path / f"assignment-pat-{reel}-{frame}.pdf"
         elif path.is_dir():
             output_path = path / f"assignment-pat-{reel}-{frame}.pdf"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/api_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *        Source File: patent_client/_async/uspto/assignment/api_test.py        *
 # ********************************************************************************
 
 from pathlib import Path
 
-import pytest
-
 from .api import AssignmentApi
 
 
-
 def test_alookup():
     query = "test_query"
     filter = "OwnerName"
     sort = "ExecutionDate+desc"
     rows = 5
     start = 0
     assignments = AssignmentApi.lookup(
@@ -23,15 +20,14 @@
     )
     assert assignments is not None, "Expected to get a response"
     assert (
         len(assignments) <= rows
     ), "Expected number of assignments to be less than or equal to requested rows"
 
 
-
 def test_download_pdf(tmp_path: Path):
     reel = "12345"
     frame = "67890"
     path = AssignmentApi.download_pdf(reel=reel, frame=frame, path=tmp_path)
     assert path.exists(), "Expected the PDF file to exist"
     assert path.is_file(), "Expected the path to be a file"
     assert path.suffix == ".pdf", "Expected the file to be a PDF"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,15 @@
     ]
     output["properties"] = zip_lists(output, property_fields, "property")
     # Delete the original fields
     for key in assignor_fields + assignee_fields + property_fields:
         del output[key]
     # Collect the correspondent into a dict
     corr_address_fields = ["corrAddress1", "corrAddress2", "corrAddress3"]
-    correspondent_address = "\n".join(
-        output[k] for k in corr_address_fields if k in output
-    )
+    correspondent_address = "\n".join(output[k] for k in corr_address_fields if k in output)
     if correspondent_address:
         output["corr_address"] = correspondent_address
     for key in corr_address_fields:
         if key in output:
             del output[key]
     output["correspondent"] = {
         "name": output["corrName"],
@@ -65,17 +63,15 @@
     }
     del output["corrName"]
     del output["corr_address"]
 
     # Collect the address for each assignee into a single string
     for assignee in output["assignees"]:
         address_lines = "\n".join(
-            assignee[k]
-            for k in ["patAssigneeAddress1", "patAssigneeAddress2"]
-            if assignee[k]
+            assignee[k] for k in ["patAssigneeAddress1", "patAssigneeAddress2"] if assignee[k]
         )
         last_line = f"{assignee['patAssigneeCity']}, {assignee['patAssigneeState']} {assignee['patAssigneePostcode']}"
         if assignee["patAssigneeCountryName"]:
             last_line += f" ({assignee['patAssigneeCountryName']})"
         assignee_address = "\n".join([address_lines, last_line])
         if assignee_address:
             assignee["patAssigneeAddress"] = assignee_address
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/convert_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,15 @@
     def allowed_filters(self):
         return list(self.fields.keys())
 
     def _get_results(self) -> Iterator["Assignment"]:
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, self.page_size
         ):
-            response = AssignmentApi.lookup(
-                **{**self.get_query(), "start": start, "rows": rows}
-            )
+            response = AssignmentApi.lookup(**{**self.get_query(), "start": start, "rows": rows})
             for doc in response.docs:
                 yield doc
             if len(response.docs) < rows:
                 break
 
     def get_query(self):
         """Get assignments.
@@ -82,17 +80,15 @@
             query = clean_number(query)
         # Handle Ordering
         order_map = {
             "execution_date": "ExecutionDate+asc",
             "-execution_date": "ExecutionDate+desc",
         }
         if len(self.config.order_by) > 1:
-            raise ValueError(
-                "Assignment API does not support multiple sort parameters!"
-            )
+            raise ValueError("Assignment API does not support multiple sort parameters!")
         elif len(self.config.order_by) == 1:
             sort = order_map[self.config.order_by[0]]
         else:
             sort = "ExecutionDate+desc"
 
         # if isinstance(query, list):
         #    query = [f'"{q}"' for q in query]
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/manager_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *      Source File: patent_client/_async/uspto/assignment/manager_test.py      *
 # ********************************************************************************
 
 import datetime
 
-import pytest
-
 from .model import Assignment
 
 
 class TestAssignment:
-    
     def test_get_assignment(self):
         a = Assignment.objects.get("18247-405")
         assert a.id == "18247-405"
         assert a.conveyance_text == "NUNC PRO TUNC ASSIGNMENT"
         assert a.last_update_date <= datetime.date.fromisoformat("2008-01-22")
         assert a.transaction_date.isoformat() == "2019-07-11"
         assert a.recorded_date.isoformat() == "2006-09-14"
@@ -43,61 +40,50 @@
         assert a.properties[0].inventors == "James J. Fallon"
         assert a.properties[0].issue_date.isoformat() == "2006-10-31"
         assert a.properties[0].pat_num == "7130913"
         assert a.properties[0].pct_num is None
         assert a.properties[0].publ_date.isoformat() == "2004-04-15"
         assert a.properties[0].publ_num == "20040073746"
 
-    
     def test_fetch_assignments_by_assignee(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
         assert assignments.count() >= 22
         assert (assignments[5]).assignors[0].name == "OEHRING, JARED"
         assignments = Assignment.objects.filter(assignee="LogicBlox")
         assert assignments.count() >= 9
 
-    
     def test_fetch_assignments_by_patent(self):
         assignments = Assignment.objects.filter(patent_number="8,789,601")
         assert assignments.count() >= 1
         assert "48041-605" in [a.id for a in assignments]
 
-    
     def test_fetch_assignments_by_application(self):
         assignments = Assignment.objects.filter(appl_id="14/190,982")
         assert assignments.count() >= 1
 
-    
     def test_fetch_assignee_with_greater_than_500_assignments(self):
         assignments = Assignment.objects.filter(assignee="Borealis")
         assert assignments.count() >= 1268
 
-    
     def test_get_assignment_image(self):
         assignments = Assignment.objects.filter(patent_number=6095661)
         assignment = assignments.first()
         assert (
             assignment.image_url
             == "http://legacy-assignments.uspto.gov/assignments/assignment-pat-038505-0128.pdf"
         )
 
-    
     def test_slice_assignments(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
-        assignment_list1 = [
-            assignment.id for assignment in assignments[0:5]
-        ]
+        assignment_list1 = [assignment.id for assignment in assignments[0:5]]
         assert len(assignment_list1) == 5
 
         assignment_list2 = [assignment.id for assignment in assignments[:5]]
         assert len(assignment_list2) == 5
 
-        assignment_list3 = [
-            assignment.id for assignment in assignments[-5:]
-        ]
+        assignment_list3 = [assignment.id for assignment in assignments[-5:]]
         assert len(assignment_list3) == 5
 
-    
     def test_iterate_assignments(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
         assignment_list = [assignment.id for assignment in assignments]
         assert len(assignment_list) == assignments.count()
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/model.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/uspto/assignment/model.py          *
 # ********************************************************************************
 
 import datetime
+import typing as tp
 import warnings
 from pathlib import Path
-import typing as tp
 
 from dateutil.parser import isoparse
 from pydantic import BeforeValidator, ConfigDict, Field, field_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
@@ -37,17 +37,15 @@
 def parse_date(string):
     dt = parse_datetime(string)
     if dt is None:
         return None
     return dt.date()
 
 
-DatetimeAsDate = Annotated[
-    tp.Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
-]
+DatetimeAsDate = Annotated[tp.Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))]
 
 
 class AbstractAssignmentModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
@@ -80,43 +78,43 @@
 
     @property
     def application(self) -> tp.Optional["USApplication"]:
         """The related US Application"""
         try:
             appl_id = getattr(self, "appl_id", None)
             if appl_id is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(appl_id=appl_id)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    appl_id=appl_id
+                )
             appl_id = getattr(self, "pct_num", None)
             if appl_id is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(appl_id=appl_id)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    appl_id=appl_id
+                )
             pub_num = getattr(self, "publ_num", None)
             if pub_num is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(app_early_pub_number=pub_num)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    app_early_pub_number=pub_num
+                )
             pat_num = getattr(self, "pat_num", None)
             if pat_num is not None:
-                return self._get_model(
-                    "patent_client.uspto.peds.model.USApplication"
-                ).objects.get(patent_number=pat_num)
+                return self._get_model("patent_client.uspto.peds.model.USApplication").objects.get(
+                    patent_number=pat_num
+                )
         except Exception:
             pass
         warnings.warn(f"Unable to find application for {self}")
         return None
 
     @property
     def patent(self) -> "Patent":
         """The related US Patent, if any"""
-        return self._get_model(
-            "patent_client.uspto.public_search.model.Patent"
-        ).objects.get(publication_number=self.pat_num)
+        return self._get_model("patent_client.uspto.public_search.model.Patent").objects.get(
+            publication_number=self.pat_num
+        )
 
     @property
     def publication(
         self,
     ) -> "PublishedApplication":
         """The related US Publication, if any"""
         return self._get_model(
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/assignment/model_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 client = PatentClientSession()
 
 
 class BulkDataApi:
     @classmethod
     def get_latest(cls) -> tp.List[Product]:
         """Returns all products with Latest Files"""
-        response = client.get(
-            "https://bulkdata.uspto.gov:443/BDSS-API/products/all/latest"
-        )
+        response = client.get("https://bulkdata.uspto.gov:443/BDSS-API/products/all/latest")
         return [Product(**product) for product in response.json()]
 
     @classmethod
     def get_by_name(
         cls,
         product_name: str,
         from_date: tp.Optional[datetime.date] = None,
@@ -52,17 +50,15 @@
         )
         response.raise_for_status()
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     def get_popular(cls) -> tp.List[Product]:
         """Returns popular products along with latest files."""
-        response = client.get(
-            "https://bulkdata.uspto.gov:443/BDSS-API/products/popular"
-        )
+        response = client.get("https://bulkdata.uspto.gov:443/BDSS-API/products/popular")
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     def get_by_short_name(
         cls,
         product_name: str,
         from_date: tp.Optional[tp.Union[datetime.date, str]] = None,
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/api_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/api_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,40 +6,34 @@
 
 import pytest
 
 from .api import BulkDataApi
 from .model import File, Product
 
 
-
 def test_can_get_latest():
     latest = BulkDataApi.get_latest()
     first = latest[0]
     assert isinstance(first, Product)
     assert isinstance(first.files[0], File)
 
 
-
 def test_can_get_by_short_name():
     first = BulkDataApi.get_by_short_name("PTGRXML")
     assert isinstance(first, Product)
     assert isinstance(first.files[0], File)
 
 
-
 def test_can_get_by_short_name_with_date_range():
-    first = BulkDataApi.get_by_short_name(
-        "PTGRXML", from_date="2023-06-01", to_date="2023-08-01"
-    )
+    first = BulkDataApi.get_by_short_name("PTGRXML", from_date="2023-06-01", to_date="2023-08-01")
     assert isinstance(first, Product)
     assert isinstance(first.files[0], File)
     assert len(first.files) == 10
 
 
-
 @pytest.mark.no_vcr
 @pytest.mark.skip(reason="This test is too slow")
 def test_can_download_file(tmpdir):
     product = BulkDataApi.get_by_short_name("PTGRXML")
     file = product.files[0]
     file.adownload(tmpdir)
     assert len(list(tmpdir.listdir())) == 1
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,15 @@
     def filter_by_name(self, short_name) -> tp.Iterator["Product"]:
         result = BulkDataApi.get_by_name(short_name)
         for product in result:
             yield product
 
 
 class FileManager(Manager):
-    def filter_by_short_name(
-        self, short_name, from_date=None, to_date=None
-    ) -> tp.Iterator["File"]:
+    def filter_by_short_name(self, short_name, from_date=None, to_date=None) -> tp.Iterator["File"]:
         if from_date is not None:
             from_date = (
                 from_date
                 if isinstance(from_date, datetime.date)
                 else datetime.date.fromisoformat(from_date)
             )
         if to_date is not None:
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/manager_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,53 +2,46 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *      Source File: patent_client/_async/uspto/bulk_data/manager_test.py       *
 # ********************************************************************************
 
 import datetime
 
-import pytest
-
 from .manager import date_ranges
 from .model import File, Product
 
 
 class TestProduct:
-    
     def test_can_get_latest(self):
         latest = [p for p in Product.objects.filter_by_latest()]
         assert isinstance(latest[0], Product)
 
-    
     def test_can_get_by_short_name(self):
         first = Product.objects.get_by_short_name("PTGRXML")
         assert isinstance(first, Product)
         assert isinstance(first.files[0], File)
 
-    
     def test_can_filter_by_name(self):
         first = [p for p in Product.objects.filter_by_name("Assignment")]
         first = list(first)[0]
         assert isinstance(first, Product)
         assert isinstance(first.files[0], File)
 
 
 class TestFile:
-    
     def test_can_filter_by_short_name(self):
         results = [
             f
             for f in File.objects.filter_by_short_name(
                 "PTGRXML", from_date="2023-06-15", to_date="2023-08-15"
             )
         ]
         assert len(results) == 10
         assert isinstance(results[0], File)
 
-    
     def test_can_get_daily_assignments(self):
         results = [f for f in File.objects.filter_by_short_name("PASDL")]
         assert len(results) > 1
         assert isinstance(results[0], File)
 
 
 def test_date_ranges():
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/bulk_data/model.py` & `patent_client-5.0.3/patent_client/_sync/uspto/bulk_data/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,10 +38,8 @@
     title: str = Field(alias="productTitle")
     frequency: tp.Optional[str] = Field(alias="productFrequency", default=None)
     level: str = Field(alias="productLevel")
     from_date: datetime.date = Field(alias="productFromDate")
     to_date: datetime.date = Field(alias="productToDate")
     number_of_files: int = Field(alias="numberOfFiles")
     parent_product: tp.Optional[str] = Field(alias="parentProduct", default=None)
-    files: tp.Optional[tp.List[File]] = Field(
-        alias="productFiles", default_factory=list
-    )
+    files: tp.Optional[tp.List[File]] = Field(alias="productFiles", default_factory=list)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
         response = client.get(main_script)
         api_url_re = re.compile(r'apiURL:\s*"([^"]+)"')
         match = api_url_re.search(response.text)
         self.api_base_url = match.group(1) if match else None
         return self.api_base_url
 
     def get_file(self, doc_number, type_code="application", office_code="US"):
-        url = f"{self.get_base_url()}/patent-family/svc/family/{type_code}/{office_code}/{doc_number}"
+        url = (
+            f"{self.get_base_url()}/patent-family/svc/family/{type_code}/{office_code}/{doc_number}"
+        )
         _ = client.options(url)
         response = client.get(url)
         response.raise_for_status()
         return GlobalDossier.model_validate_json(response.content)
 
     def get_doc_list(self, country, doc_number, kind_code):
         url = f"{self.get_base_url()}/doc-list/svc/doclist/{country}/{doc_number}/{kind_code}"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/api_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/api_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,44 +2,39 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *      Source File: patent_client/_async/uspto/global_dossier/api_test.py      *
 # ********************************************************************************
 
 from pathlib import Path
 
-import pytest
-
 from .api import GlobalDossierApi
 from .model import DocumentList, GlobalDossier
 
 
-
 def test_get_file():
     api = GlobalDossierApi()
     doc_number = "16740760"
     type_code = "application"
     office_code = "US"
     response = api.get_file(doc_number, type_code, office_code)
     assert isinstance(response, GlobalDossier)
     assert response.country == "US"
     assert response.id == "16740760"
 
 
-
 def test_get_doc_list():
     api = GlobalDossierApi()
     country = "US"
     doc_number = "16740760"
     kind_code = "A"
     response = api.get_doc_list(country, doc_number, kind_code)
     assert isinstance(response, DocumentList)
     assert len(response.docs) > 0
 
 
-
 def test_get_document(tmp_path: Path):
     api = GlobalDossierApi()
     country = "US"
     doc_number = "201816123456.A"
     document_id = "KJM2MWIEDFLYX10"
     out_path = tmp_path / "test_document.pdf"
     api.get_document(country, doc_number, document_id, out_path)
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,49 +12,37 @@
 query_builder = QueryBuilder()
 
 global_dossier_api = GlobalDossierApi()
 
 
 class GlobalDossierBaseManager(Manager):
     def filter(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
     def order_by(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
     def limit(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
     def offset(self, *args, **kwargs):
-        raise NotImplementedError(
-            "GlobalDossier can only retrieve using the GET interface"
-        )
+        raise NotImplementedError("GlobalDossier can only retrieve using the GET interface")
 
 
 class GlobalDossierManager(GlobalDossierBaseManager):
     def get(self, *args, **kwargs):
-        return global_dossier_api.get_file(
-            **query_builder.build_query(*args, **kwargs)
-        )
+        return global_dossier_api.get_file(**query_builder.build_query(*args, **kwargs))
 
 
 class GlobalDossierApplicationManager(GlobalDossierBaseManager):
     def get(self, *args, **kwargs):
         query = query_builder.build_query(*args, **kwargs)
         gd_file = global_dossier_api.get_file(**query)
         if query["type_code"] == "application":
-            return next(
-                a for a in gd_file.applications if a.app_num in query["doc_number"]
-            )
+            return next(a for a in gd_file.applications if a.app_num in query["doc_number"])
         elif query["type_code"] == "publication":
             return next(
                 a
                 for a in gd_file.applications
                 if any(p.pub_num in query["doc_number"] for p in a.pub_list)
             )
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # *       Source File: patent_client/_async/uspto/global_dossier/model.py        *
 # ********************************************************************************
 
 import datetime
 import typing as tp
 from pathlib import Path
 
-
 from pydantic import BeforeValidator, ConfigDict, Field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
 if tp.TYPE_CHECKING:
@@ -62,17 +61,15 @@
     app_date: tp.Optional[MDYDate] = Field(alias="appDateStr")
     country_code: tp.Optional[str] = None
     kind_code: tp.Optional[str] = None
     doc_num: tp.Optional["GlobalDossierDocumentNumber"] = None
     title: tp.Optional[str] = None
     applicant_names: OptionalStrList = Field(default_factory=list)
     ip_5: tp.Optional[bool] = Field(alias="ip5")
-    priority_claim_list: "tp.List[GlobalDossierPriorityClaim]" = Field(
-        default_factory=list
-    )
+    priority_claim_list: "tp.List[GlobalDossierPriorityClaim]" = Field(default_factory=list)
     pub_list: "tp.List[GlobalDossierPublication]" = Field(default_factory=list)
 
     def __repr__(self):
         return f"GlobalDossierApplication(app_num={self.app_num}, country_code={self.country_code})"
 
     @property
     def document_list(self) -> "DocumentList":
@@ -95,70 +92,54 @@
                 self.country_code, self.app_num, self.kind_code
             )
         ).office_action_docs
 
     @property
     def us_application(self) -> "USApplication":
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
-        return self._get_model("..peds.model.USApplication").objects.get(
-            self.app_num
-        )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
+        return self._get_model("..peds.model.USApplication").objects.get(self.app_num)
 
     @property
     def us_publication(self) -> "PublishedApplication":
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
         pub = list(p for p in self.pub_list if p.kind_code == "A1")
         if len(pub) > 1:
             raise ValueError("More than one US publication for application!")
-        return self._get_model(
-            "..public_search.model.PublishedApplication"
-        ).objects.get(pub[0].pub_num)
+        return self._get_model("..public_search.model.PublishedApplication").objects.get(
+            pub[0].pub_num
+        )
 
     @property
     def us_patent(self) -> "Patent":
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
         pat = list(p for p in self.pub_list if p.kind_code in ("A", "B1", "B2"))
         if len(pat) > 1:
             raise ValueError("More than one US patent for application!")
-        return self._get_model("..public_search.model.Patent").objects.get(
-            pat[0].pub_num
-        )
+        return self._get_model("..public_search.model.Patent").objects.get(pat[0].pub_num)
 
     @property
     def us_assignments(self) -> list["Assignment"]:
         if self.country_code != "US":
-            raise ValueError(
-                f"Global Dossier Application is not a US Application! {self}"
-            )
-        return self._get_model("..assignment.model.Assignment").objects.filter(
-            appl_id=self.app_num
-        )
+            raise ValueError(f"Global Dossier Application is not a US Application! {self}")
+        return self._get_model("..assignment.model.Assignment").objects.filter(appl_id=self.app_num)
 
 
 TextBool = Annotated[bool, BeforeValidator(lambda x: x == "true")]
 
 
 class GlobalDossier(GlobalDossierBaseModel):
     country: tp.Optional[str] = None
     internal: tp.Optional[TextBool] = None
     corr_app_num: tp.Optional[str] = None
     id: tp.Optional[str] = None
     type: tp.Optional[str] = None
-    applications: tp.List[GlobalDossierApplication] = Field(
-        default_factory=list, alias="list"
-    )
+    applications: tp.List[GlobalDossierApplication] = Field(default_factory=list, alias="list")
 
     def __repr__(self):
         return f"GlobalDossier(id={self.id}, type={self.type}, country={self.country})"
 
 
 class Document(GlobalDossierBaseModel):
     doc_number: tp.Optional[str] = None
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/model_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/model_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,50 +6,45 @@
 
 import pytest
 
 from .model import Document, DocumentList, GlobalDossier, GlobalDossierApplication
 
 
 class TestGlobalDossier:
-    
     def test_us_lookup(self):
         result = GlobalDossier.objects.get("16123456")
         assert result.id == "16123456"
 
-    
     def test_us_lookup_docs(self):
         dossier = GlobalDossier.objects.get("16123456")
         result = dossier.applications[0].document_list
         assert len(result.office_action_docs) >= 2
 
     @pytest.mark.skip("issue in pytest-recording")
     def test_us_download_docs(self, tmpdir):
         dossier = GlobalDossier.objects.get("16123456")
         result = dossier.applications[0].documents[0].download(tmpdir)
         assert result.exists()
 
-    
     def test_us_app_lookup(self):
         result = GlobalDossierApplication.objects.get("16123456")
         assert result.app_num == "16123456"
         assert isinstance(result, GlobalDossierApplication)
 
-    
     def test_us_app_lookup_docs(self):
         result = GlobalDossierApplication.objects.get("16123456")
         document_list = result.document_list
         documents = result.documents
         office_actions = result.office_actions
         assert isinstance(document_list, DocumentList)
         assert isinstance(documents, list)
         assert isinstance(documents[0], Document)
         assert isinstance(office_actions, list)
         assert isinstance(office_actions[0], Document)
 
-    
     def test_links(self):
         app = GlobalDossierApplication.objects.get("16123456")
         us_application = app.us_application
         assert (
             us_application.patent_title
             == "LEARNING ASSISTANCE DEVICE, METHOD OF OPERATING LEARNING ASSISTANCE DEVICE, LEARNING ASSISTANCE PROGRAM, LEARNING ASSISTANCE SYSTEM, AND TERMINAL DEVICE"
         )
@@ -61,28 +56,21 @@
         # assert (
         #    GlobalDossierApplication.objects.get("16123456").us_patent.patent_title
         #    == "Learning assistance device, method of operating learning assistance device, learning assistance program, learning assistance system, and terminal device"
         # )
         assignments = app.us_assignments
         assert (assignments.first()).id == "46816-108"
         with pytest.raises(ValueError):
-            (
-                GlobalDossierApplication.objects.get(publication="EP1000000")
-            ).us_application
+            (GlobalDossierApplication.objects.get(publication="EP1000000")).us_application
         # Broken links to Public Patent Search
         # with pytest.raises(ValueError):
         #    GlobalDossierApplication.objects.get(publication="EP1000000").us_publication
         # with pytest.raises(ValueError):
         #    GlobalDossierApplication.objects.get(publication="EP1000000").us_patent
         with pytest.raises(ValueError):
-            (
-                GlobalDossierApplication.objects.get(publication="EP1000000")
-            ).us_assignments
+            (GlobalDossierApplication.objects.get(publication="EP1000000")).us_assignments
 
-    
     def test_issue_99(self):
-        app = GlobalDossierApplication.objects.get(
-            "16740760", type="application", office="US"
-        )
+        app = GlobalDossierApplication.objects.get("16740760", type="application", office="US")
         assert app.app_num == "16740760"
         app = GlobalDossierApplication.objects.get("17193105")
         assert app.app_num == "17193105"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,15 @@
                     "office_code": office_code,
                     "doc_number": arg,
                     "type_code": candidates[0]["type_code"],
                 }
 
         elif kwargs:
             numbers = {
-                k: v
-                for k, v in kwargs.items()
-                if k in ("publication", "application", "patent")
+                k: v for k, v in kwargs.items() if k in ("publication", "application", "patent")
             }
             if len(numbers) > 1:
                 raise QueryException(
                     "You may only pass one keyword from the set of (application, publication, patent)"
                 )
             elif not numbers:
                 raise QueryException("No number passed! Please pass a valid number")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/query_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app.json` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.3/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,28 +27,22 @@
 
 class ODPApi:
     base_url = "https://beta-api.uspto.gov"
 
     def __init__(self):
         self.client = PatentClientSession(headers={"X-API-KEY": SETTINGS.odp_api_key})
 
-    def post_search(
-        self, search_request: SearchRequest = SearchRequest()
-    ) -> tp.Dict:
+    def post_search(self, search_request: SearchRequest = SearchRequest()) -> tp.Dict:
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
-        response = self.client.post(
-            url, json=search_data, headers={"accept": "application/json"}
-        )
+        response = self.client.post(url, json=search_data, headers={"accept": "application/json"})
         response.raise_for_status()
         return response.json()
 
-    def get_search(
-        self, search_request: SearchGetRequest = SearchGetRequest()
-    ) -> tp.Dict:
+    def get_search(self, search_request: SearchGetRequest = SearchGetRequest()) -> tp.Dict:
         """Patent application search by supplying query parameters
         Query parameters are optional. When no query parameters supplied, top 25 applications are returned"""
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = self.client.get(url, params=search_data)
         response.raise_for_status()
         return response.json()
@@ -58,36 +52,27 @@
     def get_application_data(self, application_id: str) -> USApplication:
         """Patent application data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}"
         response = self.client.get(url)
         response.raise_for_status()
         return USApplication(**response.json()["patentBag"][0])
 
-    def get_application_biblio_data(
-        self, application_id: str
-    ) -> USApplicationBiblio:
+    def get_application_biblio_data(self, application_id: str) -> USApplicationBiblio:
         """Patent application basic data by application id"""
-        url = (
-            self.base_url
-            + f"/api/v1/patent/applications/{application_id}/application-data"
-        )
+        url = self.base_url + f"/api/v1/patent/applications/{application_id}/application-data"
         response = self.client.get(url)
         response.raise_for_status()
         return USApplicationBiblio(**response.json()["patentBag"][0])
 
-    def get_patent_term_adjustment_data(
-        self, application_id: str
-    ) -> TermAdjustment:
+    def get_patent_term_adjustment_data(self, application_id: str) -> TermAdjustment:
         """Patent application term adjustment data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}/adjustment"
         response = self.client.get(url)
         response.raise_for_status()
-        return TermAdjustment(
-            **response.json()["patentBag"][0]["patentTermAdjustmentData"]
-        )
+        return TermAdjustment(**response.json()["patentBag"][0]["patentTermAdjustmentData"])
 
     def get_assignments(self, application_id: str) -> tp.List[Assignment]:
         """Patent application term adjustment data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}/assignment"
         response = self.client.get(url)
         response.raise_for_status()
         data = response.json()["patentBag"][0]["assignmentBag"]
@@ -103,36 +88,27 @@
     def get_continuity_data(self, application_id: str) -> Continuity:
         """Patent application continuity data by application id"""
         url = self.base_url + f"/api/v1/patent/applications/{application_id}/continuity"
         response = self.client.get(url)
         response.raise_for_status()
         return Continuity(**response.json())
 
-    def get_foreign_priority_data(
-        self, application_id: str
-    ) -> tp.List[ForeignPriority]:
+    def get_foreign_priority_data(self, application_id: str) -> tp.List[ForeignPriority]:
         """Patent application foreign priority data by application id"""
-        url = (
-            self.base_url
-            + f"/api/v1/patent/applications/{application_id}/foreign-priority"
-        )
+        url = self.base_url + f"/api/v1/patent/applications/{application_id}/foreign-priority"
         response = self.client.get(url)
         response.raise_for_status()
         return [
             ForeignPriority(**foreign_priority)
-            for foreign_priority in response.json()["patentBag"][0][
-                "foreignPriorityBag"
-            ]
+            for foreign_priority in response.json()["patentBag"][0]["foreignPriorityBag"]
         ]
 
     def get_transactions(self, application_id: str) -> tp.List[Transaction]:
         """Patent application transactions by application id"""
-        url = (
-            self.base_url + f"/api/v1/patent/applications/{application_id}/transactions"
-        )
+        url = self.base_url + f"/api/v1/patent/applications/{application_id}/transactions"
         response = self.client.get(url)
         response.raise_for_status()
         return [
             Transaction(**transaction)
             for transaction in response.json()["patentBag"][0]["transactionContentBag"]
         ]
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/api_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/api_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,84 +11,71 @@
 
 
 @pytest.fixture
 def odp_api():
     return ODPApi()
 
 
-
 def test_post_search(odp_api):
     search_request = SearchRequest(q="firstNamedApplicant:STMicroelectronics S.A.")
     response = odp_api.post_search(search_request)
     assert response["count"] > 0, "Expected at least one result"
 
 
-
 def test_get_search(odp_api):
     search_request = SearchRequest(q="firstNamedApplicant:STMicroelectronics S.A.")
     response = odp_api.get_search(search_request)
     assert response["count"] > 0, "Expected at least one result"
 
 
-
 def test_get_application_data(odp_api):
     application_id = "15123456"
     application = odp_api.get_application_data(application_id)
     assert application.appl_id is not None, "Expected patent data"
 
 
-
 def test_get_application_basic_data(odp_api):
     application_id = "15123456"
     application = odp_api.get_application_biblio_data(application_id)
     assert application.appl_id is not None, "Expected basic patent data"
 
 
-
 def test_get_patent_term_adjustment_data(odp_api):
     application_id = "16123456"
     response = odp_api.get_patent_term_adjustment_data(application_id)
-    assert (
-        response.adjustment_total_quantity is not None
-    ), "Expected patent term adjustment data"
-
+    assert response.adjustment_total_quantity is not None, "Expected patent term adjustment data"
 
 
 def test_get_assignments(odp_api):
     application_id = "15123456"
     response = odp_api.get_assignments(application_id)
     assert len(response) > 0, "Expected at least one assignment"
 
 
-
 def test_get_attorney_data(odp_api):
     application_id = "15123456"
     response = odp_api.get_attorney_data(application_id)
     assert response.attorneys is not None, "Expected attorney data"
 
 
-
 def test_get_continuity_data(odp_api):
     application_id = "15123456"
     response = odp_api.get_continuity_data(application_id)
     assert response.parent_continuity is not None, "Expected continuity data"
 
 
-
 def test_get_foreign_priority_data(odp_api):
     application_id = "16123456"
     response = odp_api.get_foreign_priority_data(application_id)
     assert len(response) > 0, "Expected at least one foreign priority"
 
 
-
 def test_get_transactions(odp_api):
     application_id = "15123456"
     response = odp_api.get_transactions(application_id)
     assert len(response) > 0, "Expected at least one transaction"
 
 
-
 def test_get_documents(odp_api):
     application_id = "15123456"
     response = odp_api.get_documents(application_id)
     assert len(response) > 0, "Expected at least one document"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/application.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/documents.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/search.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,15 @@
 
 class USApplicationManager(Manager):
     default_filter = "appl_id"
     default_fields = []
     response_model = USApplication
 
     def count(self):
-        return (
-            api.post_search(
-                self._create_search_obj(fields=["applicationNumberText"])
-            )
-        )["count"]
+        return (api.post_search(self._create_search_obj(fields=["applicationNumberText"])))["count"]
 
     def _get_results(self) -> tp.Iterator["SearchResult"]:
         query_obj = self._create_search_obj()
         for start, rows in get_start_and_row_count(self.config.limit):
             page_query = query_obj.model_dump()
             page_query["pagination"] = {"offset": start, "limit": rows}
             page_query_obj = SearchRequest(**page_query)
@@ -140,17 +136,15 @@
         return api.get_customer_numbers(self.config.filter["appl_id"][0])
 
 
 class ForeignPriorityManager(Manager):
     default_filter = "appl_id"
 
     def _get_results(self) -> "ForeignPriority":
-        for doc in api.get_foreign_priority_data(
-            self.config.filter["appl_id"][0]
-        ):
+        for doc in api.get_foreign_priority_data(self.config.filter["appl_id"][0]):
             yield doc
 
 
 class TransactionManager(Manager):
     default_filter = "appl_id"
 
     def _get_results(self) -> tp.Iterator["Transaction"]:
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,59 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/uspto/odp/manager_test.py          *
 # ********************************************************************************
 
-import pytest
 
 from .manager import USApplicationBiblioManager, USApplicationManager
 
 
-
 def test_all_apps():
     manager = USApplicationManager().filter(query=dict())
     assert manager.count() > 1000
 
 
-
 def test_get_one_app():
     app = USApplicationManager().get(q="applicationNumberText:16123456")
     assert app is not None
     assert app.appl_id == "16123456"
 
 
-
 def test_get_app_from_search_result():
     manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     application = result.application
     assert application.appl_id == "16123456"
 
 
-
 def test_get_app_biblio_from_search_result():
     manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     biblio = result.biblio
     assert biblio.appl_id == "16123456"
 
 
-
 def test_get_continuity_from_search_result():
     manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     continuity = result.continuity
     assert len(continuity.child_continuity) > 0
 
 
-
 def test_get_documents_from_search_result():
     manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     documents = result.documents
     assert documents.count() > 0
 
 
-
 def test_simple_keyword_searches():
     manager = USApplicationManager()
     result = manager.get("16123456")
     assert result.appl_id == "16123456"
 
 
-
 def test_combination_search():
     manager = USApplicationManager()
     result = manager.filter(invention_title="Hair Dryer", filing_date_gte="2020-01-01")
     assert result.count() > 5
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/model.py` & `patent_client-5.0.3/patent_client/_async/uspto/odp/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,50 @@
-# ********************************************************************************
-# *         WARNING: This file is automatically generated by unasync.py.         *
-# *                             DO NOT MANUALLY EDIT                             *
-# *             Source File: patent_client/_async/uspto/odp/model.py             *
-# ********************************************************************************
-
 import datetime
 from enum import Enum
 from typing import Any, List, Optional
 
-
+from async_property import async_property
 from async_property.base import AsyncPropertyDescriptor
 from pydantic import AliasPath, BeforeValidator, ConfigDict, Field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
 
 class BaseODPModel(BaseModel):
-    model_config = ConfigDict(
-        alias_generator=to_camel, ignored_types=(AsyncPropertyDescriptor,)
-    )
+    model_config = ConfigDict(alias_generator=to_camel, ignored_types=(AsyncPropertyDescriptor,))
 
 
 # Common
 
 
 class Address(BaseODPModel):
     city_name: Optional[str] = Field(alias="cityName", default=None)
-    geographic_region_name: Optional[str] = Field(
-        alias="geographicRegionName", default=None
-    )
-    geographic_region_code: Optional[str] = Field(
-        alias="geographicRegionCode", default=None
-    )
+    geographic_region_name: Optional[str] = Field(alias="geographicRegionName", default=None)
+    geographic_region_code: Optional[str] = Field(alias="geographicRegionCode", default=None)
     country_code: Optional[str] = Field(alias="countryCode", default=None)
     postal_code: Optional[str] = Field(alias="postalCode", default=None)
     country_name: Optional[str] = Field(alias="countryName", default=None)
-    address_line_one_text: Optional[str] = Field(
-        alias="addressLineOneText", default=None
-    )
-    address_line_two_text: Optional[str] = Field(
-        alias="addressLineTwoText", default=None
-    )
+    address_line_one_text: Optional[str] = Field(alias="addressLineOneText", default=None)
+    address_line_two_text: Optional[str] = Field(alias="addressLineTwoText", default=None)
     name_line_one_text: Optional[str] = Field(alias="nameLineOneText", default=None)
     name_line_two_text: Optional[str] = Field(alias="nameLineTwoText", default=None)
-    postal_address_category: Optional[str] = Field(
-        alias="postalAddressCategory", default=None
-    )
-    correspondent_name_text: Optional[str] = Field(
-        alias="correspondentNameText", default=None
-    )
+    postal_address_category: Optional[str] = Field(alias="postalAddressCategory", default=None)
+    correspondent_name_text: Optional[str] = Field(alias="correspondentNameText", default=None)
 
 
 # Continuity
 
 
 class Relationship(BaseODPModel):
     application_status_code: int = Field()
     claim_type_code: str = Field(alias="claimParentageTypeCode")
     filing_date: datetime.date
-    application_status_description: str = Field(
-        alias="applicationStatusDescriptionText"
-    )
+    application_status_description: str = Field(alias="applicationStatusDescriptionText")
     claim_type_description: str = Field(alias="claimParentageTypeCodeDescription")
     parent_application_id: str = Field(alias="parentApplicationNumberText")
     child_application_id: str = Field(alias="childApplicationNumberText")
 
 
 class Continuity(BaseODPModel):
     count: int
@@ -95,28 +73,28 @@
     mail_date: datetime.datetime = Field(alias="officialDate")
     document_identifier: str = Field(alias="documentIdentifier")
     document_code: str = Field(alias="documentCode")
     document_code_description: str = Field(alias="documentCodeDescriptionText")
     direction_category: str = Field(alias="directionCategory")
     download_option_bag: list[dict] = Field(alias="downloadOptionBag")
 
-    def download(self, type="PDF", out_path=None):
+    async def download(self, type="PDF", out_path=None):
         from .manager import api
 
         try:
-            url = next(
-                u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type
-            )["downloadUrl"]
+            url = next(u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type)[
+                "downloadUrl"
+            ]
         except StopIteration:
             raise ValueError(f"No download URL found for this document type: {type}")
         if out_path is None:
             out_path = f"{self.appl_id} - {self.mail_date.date()} - {self.document_code} - {self.document_code_description}.{type.lower()}".replace(
                 "/", "-"
             )
-        return api.client.download(url, "GET", path=out_path)
+        return await api.client.download(url, "GET", path=out_path)
 
 
 # Assignment
 
 
 class Assignor(BaseODPModel):
     execution_date: datetime.date = Field(alias="executionDate")
@@ -171,25 +149,21 @@
     first_name: Optional[str] = Field(alias="firstName", default=None)
     last_name: Optional[str] = Field(alias="lastName", default=None)
     registration_number: str = Field(alias="registrationNumber")
     attorney_address_bag: list[Address] = Field(alias="attorneyAddressBag")
     telecommunication_address_bag: list[TelecommunicationAddress] = Field(
         alias="telecommunicationAddressBag"
     )
-    registered_practitioner_category: str = Field(
-        alias="registeredPractitionerCategory"
-    )
+    registered_practitioner_category: str = Field(alias="registeredPractitionerCategory")
     name_suffix: Optional[str] = Field(alias="nameSuffix", default=None)
 
 
 class CustomerNumber(BaseODPModel):
     attorneys: list[Attorney] = Field(alias="attorneyBag")
-    customer_number: Optional[str] = Field(
-        alias=AliasPath("customerNumber", "patronIdentifier")
-    )
+    customer_number: Optional[str] = Field(alias=AliasPath("customerNumber", "patronIdentifier"))
     address: Optional[Address] = Field(
         alias=AliasPath("customerNumber", "powerOfAttorneyAddressBag", 0)
     )
 
 
 # Transactions
 
@@ -209,22 +183,18 @@
     action_date: datetime.date = Field(alias="actionDate")
 
 
 class TermAdjustment(BaseODPModel):
     applicant_day_delay_quantity: Optional[int] = Field(
         alias="applicantDayDelayQuantity", default=None
     )
-    overlapping_day_quantity: Optional[int] = Field(
-        alias="overlappingDayQuantity", default=None
-    )
+    overlapping_day_quantity: Optional[int] = Field(alias="overlappingDayQuantity", default=None)
     filing_date: Optional[datetime.date] = Field(alias="filingDate", default=None)
     c_delay_quantity: Optional[int] = Field(alias="cDelayQuantity", default=None)
-    adjustment_total_quantity: Optional[int] = Field(
-        alias="adjustmentTotalQuantity", default=None
-    )
+    adjustment_total_quantity: Optional[int] = Field(alias="adjustmentTotalQuantity", default=None)
     b_delay_quantity: Optional[int] = Field(alias="bDelayQuantity", default=None)
     grant_date: Optional[datetime.date] = Field(alias="grantDate", default=None)
     a_delay_quantity: Optional[int] = Field(alias="aDelayQuantity", default=None)
     non_overlapping_day_quantity: Optional[int] = Field(
         alias="nonOverlappingDayQuantity", default=None
     )
     ip_office_day_delay_quantity: Optional[int] = Field(
@@ -267,77 +237,63 @@
     appl_id: str = Field(alias="applicationNumberText")
     first_inventor_name: str = Field(alias="firstInventorName")
     first_applicant_name: str = Field(alias="firstApplicantName")
     cpc_classifications: list[str] = Field(alias="cpcClassificationBag")
     entity_status: str = Field(alias="businessEntityStatusCategory")
     app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber")
 
-    @property
-    def bibliographic_data(self) -> "USApplicationBiblio":
-        return self._get_model(".model.USApplicationBiblio").objects.get(
-            appl_id=self.appl_id
-        )
-
-    @property
-    def application(self) -> "USApplication":
-        return self._get_model(".model.USApplication").objects.get(
-            appl_id=self.appl_id
-        )
-
-    @property
-    def continuity(self) -> Continuity:
-        return self._get_model(".model.Continuity").objects.get(
-            appl_id=self.appl_id
-        )
+    @async_property
+    async def bibliographic_data(self) -> "USApplicationBiblio":
+        return await self._get_model(".model.USApplicationBiblio").objects.get(appl_id=self.appl_id)
+
+    @async_property
+    async def application(self) -> "USApplication":
+        return await self._get_model(".model.USApplication").objects.get(appl_id=self.appl_id)
+
+    @async_property
+    async def continuity(self) -> Continuity:
+        return await self._get_model(".model.Continuity").objects.get(appl_id=self.appl_id)
 
-    @property
-    def documents(self) -> list[Document]:
+    @async_property
+    async def documents(self) -> list[Document]:
         return self._get_model(".model.Document").objects.filter(appl_id=self.appl_id)
 
-    @property
-    def term_adjustment(self) -> TermAdjustment:
-        return self._get_model(".model.TermAdjustment").objects.filter(
-            appl_id=self.appl_id
-        )
+    @async_property
+    async def term_adjustment(self) -> TermAdjustment:
+        return self._get_model(".model.TermAdjustment").objects.filter(appl_id=self.appl_id)
 
-    @property
-    def assignments(self) -> list[Assignment]:
+    @async_property
+    async def assignments(self) -> list[Assignment]:
         return self._get_model(".model.Assignment").objects.filter(appl_id=self.appl_id)
 
-    @property
-    def customer_number(self) -> CustomerNumber:
-        return self._get_model(".model.CustomerNumber").objects.filter(
-            appl_id=self.appl_id
-        )
-
-    @property
-    def foreign_priority(self) -> ForeignPriority:
-        return self._get_model(".model.ForeignPriority").objects.filter(
-            appl_id=self.appl_id
-        )
-
-    @property
-    def transactions(self) -> list[Transaction]:
-        return self._get_model(".model.Transaction").objects.filter(
-            appl_id=self.appl_id
-        )
+    @async_property
+    async def customer_number(self) -> CustomerNumber:
+        return self._get_model(".model.CustomerNumber").objects.filter(appl_id=self.appl_id)
+
+    @async_property
+    async def foreign_priority(self) -> ForeignPriority:
+        return self._get_model(".model.ForeignPriority").objects.filter(appl_id=self.appl_id)
+
+    @async_property
+    async def transactions(self) -> list[Transaction]:
+        return self._get_model(".model.Transaction").objects.filter(appl_id=self.appl_id)
 
     # Aliases
 
-    @property
-    def biblio(self) -> "USApplicationBiblio":
-        return self.bibliographic_data
-
-    @property
-    def app(self) -> "USApplication":
-        return self.application
-
-    @property
-    def docs(self) -> list[Document]:
-        return self.documents
+    @async_property
+    async def biblio(self) -> "USApplicationBiblio":
+        return await self.bibliographic_data
+
+    @async_property
+    async def app(self) -> "USApplication":
+        return await self.application
+
+    @async_property
+    async def docs(self) -> list[Document]:
+        return await self.documents
 
 
 class USApplication(BaseODPModel):
     aia_indicator: YNBool = Field(alias="firstInventorToFileIndicator")
     app_filing_date: datetime.date = Field(alias="filingDate")
     inventors: list[Inventor] = Field(alias="inventorBag")
     customer_number: int = Field(alias="customerNumber")
@@ -363,17 +319,15 @@
     transactions: list[Transaction] = Field(alias="transactionContentBag")
     parent_applications: Optional[list[Relationship]] = Field(
         alias=AliasPath("continuityBag", "parentContinuityBag"), default=None
     )
     child_applications: Optional[list[Relationship]] = Field(
         alias=AliasPath("continuityBag", "childContinuityBag"), default=None
     )
-    patent_term_adjustment: Optional[TermAdjustment] = Field(
-        alias="patentTermAdjustmentData"
-    )
+    patent_term_adjustment: Optional[TermAdjustment] = Field(alias="patentTermAdjustmentData")
 
     @model_validator(mode="before")
     @classmethod
     def _validate_patent_term_adjustment(cls, v):
         if v["patentTermAdjustmentData"] == dict():
             v["patentTermAdjustmentData"] = None
         return v
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/model_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,31 +40,26 @@
     assert continuity.parent_continuity[0].application_status_code == 161
     assert continuity.parent_continuity[0].claim_type_code == "NST"
     assert continuity.parent_continuity[0].filing_date == datetime.date(2015, 4, 22)
     assert (
         continuity.parent_continuity[0].application_status_description
         == "Abandoned  --  Failure to Respond to an Office Action"
     )
-    assert (
-        continuity.parent_continuity[0].claim_type_description
-        == "is a National Stage Entry of"
-    )
+    assert continuity.parent_continuity[0].claim_type_description == "is a National Stage Entry of"
     assert continuity.parent_continuity[0].parent_application_id == "PCT/US15/27322"
     assert continuity.parent_continuity[0].child_application_id == "15123456"
     assert len(continuity.child_continuity) == 1
     assert continuity.child_continuity[0].application_status_code == 160
     assert continuity.child_continuity[0].claim_type_code == "CON"
     assert continuity.child_continuity[0].filing_date == datetime.date(2018, 9, 13)
     assert (
         continuity.child_continuity[0].application_status_description
         == "Abandoned  --  Incomplete Application (Pre-examination)"
     )
-    assert (
-        continuity.child_continuity[0].claim_type_description == "is a Continuation of"
-    )
+    assert continuity.child_continuity[0].claim_type_description == "is a Continuation of"
     assert continuity.child_continuity[0].parent_application_id == "15123456"
     assert continuity.child_continuity[0].child_application_id == "16132008"
 
 
 def test_document(fixture_dir):
     data = json.loads((fixture_dir / "documents.json").read_text())
     for doc_data in data["documentBag"]:
@@ -165,36 +160,29 @@
     assert transactions[3].transaction_code == "SMAL"
     assert (
         transactions[3].transaction_description
         == "Applicant Has Filed a Verified Statement of Small Entity Status in Compliance with 37 CFR 1.27"
     )
     assert transactions[-1].recorded_date == datetime.date.fromisoformat("2020-10-21")
     assert transactions[-1].transaction_code == "IDSC"
-    assert (
-        transactions[-1].transaction_description
-        == "Information Disclosure Statement considered"
-    )
+    assert transactions[-1].transaction_description == "Information Disclosure Statement considered"
 
 
 def test_patent_term_adjustment(fixture_dir):
     data = json.loads((fixture_dir / "adjustment.json").read_text())
     patent_term_adjustment_data = data["patentBag"][0]["patentTermAdjustmentData"]
     patent_term_adjustment = TermAdjustment(**patent_term_adjustment_data)
 
     assert patent_term_adjustment.applicant_day_delay_quantity == 15
     assert patent_term_adjustment.overlapping_day_quantity == 0
-    assert patent_term_adjustment.filing_date == datetime.date.fromisoformat(
-        "2018-09-06"
-    )
+    assert patent_term_adjustment.filing_date == datetime.date.fromisoformat("2018-09-06")
     assert patent_term_adjustment.c_delay_quantity == 0
     assert patent_term_adjustment.adjustment_total_quantity == 0
     assert patent_term_adjustment.b_delay_quantity == 0
-    assert patent_term_adjustment.grant_date == datetime.date.fromisoformat(
-        "2021-01-26"
-    )
+    assert patent_term_adjustment.grant_date == datetime.date.fromisoformat("2021-01-26")
     assert patent_term_adjustment.a_delay_quantity == 142
     assert patent_term_adjustment.non_overlapping_day_quantity == 127
     assert patent_term_adjustment.ip_office_day_delay_quantity == 142
 
     assert len(patent_term_adjustment.history) > 0
     for history_item in patent_term_adjustment.history:
         assert isinstance(history_item, TermAdjustmentHistory)
@@ -207,17 +195,15 @@
 
 def test_application_biblio(fixture_dir):
     data = json.loads((fixture_dir / "biblio.json").read_text())
     application_biblio_data = data["patentBag"][0]
     application_biblio = USApplicationBiblio(**application_biblio_data)
 
     assert application_biblio.aia_indicator is True
-    assert application_biblio.app_filing_date == datetime.date.fromisoformat(
-        "2016-09-02"
-    )
+    assert application_biblio.app_filing_date == datetime.date.fromisoformat("2016-09-02")
     assert len(application_biblio.inventors) > 0
     assert application_biblio.customer_number == 26161
     assert application_biblio.group_art_unit == "3775"
     assert application_biblio.invention_title == "TONGUE RETRACTORS FOR FRENOTOMIES"
     assert len(application_biblio.correspondence_address) > 0
     assert application_biblio.app_conf_num == 7229
     assert application_biblio.atty_docket_num == "29539-0122US1"
@@ -245,17 +231,15 @@
     assert application.appl_id == "15123456"
     assert application.first_inventor_name == "Marvin Wang"
     assert application.first_applicant_name == "The General Hospital Corporation"
     assert len(application.cpc_classifications) > 0
     assert application.entity_status == "Small"
     assert application.app_type_code == "UTL"
     assert application.national_stage_indicator is False
-    assert application.effective_filing_date == datetime.date.fromisoformat(
-        "2016-09-02"
-    )
+    assert application.effective_filing_date == datetime.date.fromisoformat("2016-09-02")
     assert len(application.assignments) > 0
     assert len(application.attorneys.attorneys) > 0
     assert len(application.transactions) > 0
     assert len(application.parent_applications) > 0
     assert len(application.child_applications) > 0
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/query.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/query_fields.csv` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/odp/util.py` & `patent_client-5.0.3/patent_client/_sync/uspto/odp/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/__init__.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/api_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/api_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *           Source File: patent_client/_async/uspto/peds/api_test.py           *
 # ********************************************************************************
 
-import pytest
 
 from .api import PatentExaminationDataSystemApi
 
 
-
 def test_can_get_app():
     result = PatentExaminationDataSystemApi().create_query("applId:(16123456)")
     assert result.num_found == 1
     assert result.applications[0].appl_id == "16123456"
 
 
-
 def test_can_search_by_customer_number():
-    result = PatentExaminationDataSystemApi().create_query(
-        "appCustNumber:(70155)"
-    )
+    result = PatentExaminationDataSystemApi().create_query("appCustNumber:(70155)")
     assert result.num_found > 10
 
 
-
 def test_can_limit_by_rows():
-    result = PatentExaminationDataSystemApi().create_query(
-        "appCustNumber:(70155)", rows=5
-    )
+    result = PatentExaminationDataSystemApi().create_query("appCustNumber:(70155)", rows=5)
     assert len(result.applications) == 5
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/fixtures/app_1_output.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'applications'": "{0: {'app_confr_number': '1659'}}"}*

```diff
@@ -1,12 +1,13 @@
 {
     "applications": [
         {
             "app_attr_dock_number": "Suntulit_02",
             "app_cls_sub_cls": "700/276000",
+            "app_confr_number": "1659",
             "app_early_pub_date": "2010-09-16",
             "app_early_pub_number": "US20100235004A1",
             "app_exam_name": "BAHTA, KIDEST",
             "app_filing_date": "2010-03-11",
             "app_grp_art_number": "2127",
             "app_location": "ELECTRONIC",
             "app_status": "Patented Case",
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *           Source File: patent_client/_async/uspto/peds/manager.py            *
 # ********************************************************************************
 
 import datetime
 import logging
+import typing as tp
 from collections.abc import Sequence
 from pathlib import Path
 from tempfile import TemporaryDirectory
-import typing as tp
 
 from dateutil.parser import parse as dt_parse
 from pypdf import PdfMerger
 
 from patent_client.util.manager import Manager
 from patent_client.util.request_util import get_start_and_row_count
 
@@ -63,17 +63,15 @@
     def _get_results(self) -> tp.Iterator["USApplication"]:
         query_params = self.get_query_params()
         api = PatentExaminationDataSystemApi()
         counter = 0
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, page_size=20
         ):
-            page = api.create_query(
-                **{**query_params, "start": start, "rows": rows}
-            )
+            page = api.create_query(**{**query_params, "start": start, "rows": rows})
             for app in page.applications:
                 yield app
                 counter += 1
                 if self.config.limit and counter >= self.config.limit:
                     break
             if len(page.applications) < rows:
                 break
@@ -101,17 +99,15 @@
                 if "__" in k:
                     f, *op = k.split("__")
                     if len(op) > 1:
                         raise ValueError(
                             f"Invalid date filter: {k}={v}; Cannot have more than one operator"
                         )
                     if op[0] not in ("gte", "lte"):
-                        raise ValueError(
-                            f"Invalid date filter: {k}={v}; Invalid operator: {op[0]}"
-                        )
+                        raise ValueError(f"Invalid date filter: {k}={v}; Invalid operator: {op[0]}")
                     if isinstance(v, (list, tuple)):
                         raise ValueError(
                             f"Invalid date filter: {k}={v}; Cannot have multiple values with operator {op[0]}"
                         )
                     date_filter_tuples.append((f, op[0], cast_as_datetime(v)))
                 else:
                     if isinstance(v, (list, tuple)):
@@ -124,29 +120,21 @@
                     else:
                         date_filter_tuples.append((k, "exact", cast_as_datetime(v)))
             # Create pairs of gte/lte filters
             query_date_filter_tuples = set()
             for k, op, v in date_filter_tuples:
                 if op == "gte":
                     lte_query = next(
-                        (
-                            v
-                            for k, op, v in date_filter_tuples
-                            if k == k and op == "lte"
-                        ),
+                        (v for k, op, v in date_filter_tuples if k == k and op == "lte"),
                         "*",
                     )
                     query_date_filter_tuples.add((k, (v, lte_query)))
                 elif op == "lte":
                     gte_query = next(
-                        (
-                            v
-                            for k, op, v in date_filter_tuples
-                            if k == k and op == "gte"
-                        ),
+                        (v for k, op, v in date_filter_tuples if k == k and op == "gte"),
                         "*",
                     )
                     query_date_filter_tuples.add((k, (gte_query, v)))
                 elif op == "exact":
                     query_date_filter_tuples.add((k, (v, v)))
 
             # Create the query string
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/manager_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 import datetime
 import json
 from collections import OrderedDict
 from pathlib import Path
 
 import pytest
-from pypdf import PdfReader
 
-from .model import PedsPage, USApplication, RemovedDataException
+from .model import PedsPage, RemovedDataException, USApplication
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
 class TestPatentExaminationDataDeserialization:
     def test_application(self):
         input_file = fixtures / "app_1_input.json"
@@ -24,56 +23,48 @@
         app = PedsPage.model_validate_json(input_file.read_text())
         # output_file.write_text(app.model_dump_json(indent=2))
         expected_data = json.loads(output_file.read_text())
         assert json.loads(app.model_dump_json()) == expected_data
 
 
 class TestPatentExaminationData:
-    
     def test_get_inventors(self):
         app = USApplication.objects.get(12721698)
         inventors = app.inventors
         assert len(inventors) == 1
         inventor = inventors[0]
         assert inventor.name == "Thind; Deepinder Singh"
         assert inventor.address == "Mankato, MN (US)"
 
-    
     def test_search_by_customer_number(self):
         result = USApplication.objects.filter(app_cust_number="70155")
         assert result.count() > 1
 
-    
     def test_get_by_pub_number(self):
         pub_no = "US20060127129A1"
         app = USApplication.objects.get(app_early_pub_number=pub_no)
         assert app.patent_title == "ELECTROPHOTOGRAPHIC IMAGE FORMING APPARATUS"
 
-    
     def test_get_by_pat_number(self):
         pat_no = 6095661
         app = USApplication.objects.get(patent_number=pat_no)
         assert app.patent_title == "METHOD AND APPARATUS FOR AN L.E.D. FLASHLIGHT"
 
-    
     def test_get_by_application_number(self):
         app_no = "15145443"
         app = USApplication.objects.get(app_no)
         assert (
-            app.patent_title
-            == "Suction and Discharge Lines for a Dual Hydraulic Fracturing Unit"
+            app.patent_title == "Suction and Discharge Lines for a Dual Hydraulic Fracturing Unit"
         )
 
-    
     def test_get_many_by_application_number(self):
         app_nos = ["14971450", "15332765", "13441334", "15332709", "14542000"]
         data = USApplication.objects.filter(*app_nos)
         assert data.count() == 5
 
-    
     def test_search_pat_by_assignee(self):
         data = (
             USApplication.objects.filter(first_named_applicant="LogicBlox")
             .order_by("appl_id")
             .limit(4)
         )
         expected_titles = [
@@ -83,53 +74,48 @@
             "LEAPFROG TREE-JOIN",
         ]
         apps = [a for a in data]
         app_titles = [a.patent_title.upper() for a in apps]
         for t in expected_titles:
             assert t in app_titles
 
-    
     def test_get_many_by_publication_number(self):
         nos = [
             "US20080034424A1",
             "US20100020700A1",
             "US20110225644A1",
             "US20050120054A1",
             "US20050188423A1",
         ]
         data = USApplication.objects.filter(app_early_pub_number=nos)
         assert data.count() == 5
 
-    
     @pytest.mark.skip("Continuity information has been removed from PEDS")
     def test_get_child_data(self):
         parent = USApplication.objects.get("14018930")
         child = parent.child_continuity[0]
         assert child.child_appl_id == "14919159"
         assert child.relationship == "claims the benefit of"
         # assert child.child.patent_title == "LEAPFROG TREE-JOIN"
 
-    
     @pytest.mark.skip("Continuity information has been removed from PEDS")
     def test_get_parent_data(self):
         child = USApplication.objects.get("14018930")
         parent = child.parent_continuity[0]
         assert parent.parent_appl_id == "61706484"
         assert parent.relationship == "Claims Priority from Provisional Application"
         assert parent.parent_app_filing_date is not None
         # assert parent.parent.patent_title == "Leapfrog Tree-Join"
 
-    
     @pytest.mark.skip("PTA information has been removed from PEDS")
     def test_pta_history(self):
         app = USApplication.objects.get("14095073")
         pta_history = app.pta_pte_tran_history
         assert len(pta_history) > 10
 
-    
     @pytest.mark.skip("PTA information has been removed from PEDS")
     def test_pta_summary(self):
         app = USApplication.objects.get("14095073")
         expected = OrderedDict(
             [
                 ("kind", "PTA"),
                 ("a_delay", 169),
@@ -138,32 +124,29 @@
                 ("total_days", 159),
             ]
         )
         actual = app.pta_pte_summary.model_dump()
         for k, v in expected.items():
             assert actual[k] == v
 
-    
     def test_transactions(self):
         app = USApplication.objects.get("14095073")
         assert len(app.transactions) > 70
 
-    
     def test_correspondent(self):
         app = USApplication.objects.get("14095073")
         expected_keys = [
             "corr_name",
             "corr_cust_no",
             "corr_address",
         ]
 
         for k in expected_keys:
             assert getattr(app, k, None) is not None
 
-    
     @pytest.mark.skip("Attorney information has been removed from PEDS")
     def test_attorneys(self):
         app = USApplication.objects.get("14095073")
         assert len(app.attorneys) > 1
         actual = app.attorneys[0].model_dump()
         assert int(actual["registration_no"]) > 1000
         expected_keys = [
@@ -171,26 +154,24 @@
             "full_name",
             "phone_num",
             "reg_status",
         ]
         for k in expected_keys:
             assert k in actual
 
-    
     def test_iterator(self):
         apps = USApplication.objects.filter(first_named_applicant="Tesla").limit(68)
         counter = 0
         try:
             for a in apps:
                 counter += 1
         except KeyError as e:
             raise e
         assert apps.count() == counter
 
-    
     @pytest.mark.skip("PTA information has been removed from PEDS")
     def test_expiration_date(self):
         app = USApplication.objects.get("15384723")
         expected = {
             "parent_appl_id": "12322218",
             "parent_app_filing_date": datetime.date(2009, 1, 29),
             "parent_relationship": "is a Continuation in part of",
@@ -213,64 +194,58 @@
             "extended_term": datetime.date(2037, 10, 16),
             "terminal_disclaimer_filed": False,
         }
         actual = dict(app.expiration)
         for k in expected.keys():
             assert expected[k] == actual[k]
 
-    
     @pytest.mark.skip("Expiration date is not supported for PCT applications")
     def test_expiration_date_for_pct_apps(self):
         app = USApplication.objects.get("PCT/US2014/020588")
         with pytest.raises(Exception) as exc:
             _ = app.expiration
         assert exc.match("Expiration date not supported for PCT Applications")
 
-    
     def test_foreign_priority(self):
         app = USApplication.objects.get(patent_number=10544653)
         fp = app.foreign_priority
         assert isinstance(fp, list)
         app = fp[0]
         assert app.country_name == "NORWAY"
         assert app.filing_date == datetime.date(2017, 2, 15)
         assert app.priority_claim == "20170229"
 
-
-    
     def test_raises_warning_on_missing_information(self):
         app = USApplication.objects.get(patent_number=10000000)
         with pytest.raises(RemovedDataException):
             _ = app.expiration
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.attorneys
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.pta_pte_summary
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.pta_pte_tran_history
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.parent_continuity
-            
+
         with pytest.raises(RemovedDataException):
             _ = app.child_continuity
 
+
 class TestDocuments:
     @pytest.mark.vcr
     def test_can_get_document_listing(self):
         app = USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         assert docs.count() > 50
 
     @pytest.mark.vcr
     def test_can_get_application_from_document(self):
         app = USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         doc = docs[5]
         backref_app = doc.application
         assert app.appl_id == backref_app.appl_id
-
-
-
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/model.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *            Source File: patent_client/_async/uspto/peds/model.py             *
 # ********************************************************************************
 
 import datetime
-from pathlib import Path
 import typing as tp
+from pathlib import Path
 
-
-from dateutil.relativedelta import relativedelta
-from pydantic import (
-    AliasPath,
-    BeforeValidator,
-    ConfigDict,
-    Field,
-    computed_field,
-    model_validator,
-)
+from pydantic import AliasPath, BeforeValidator, ConfigDict, Field, computed_field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated, Self
 
 from patent_client.util.pydantic_util import BaseModel, Date, DateTime
 
 if tp.TYPE_CHECKING:
     from ...epo.ops.published.model import InpadocBiblio
@@ -117,14 +108,15 @@
 
 
 class USApplication(PEDSBaseModel):
     appl_id: str
     app_filing_date: Date
     app_exam_name: tp.Optional[str] = None
     public_ind: YNBool
+    app_confr_number: tp.Optional[str] = None
     inventor_name: tp.Optional[str] = None
     app_early_pub_number: tp.Optional[str] = None
     app_early_pub_date: tp.Optional[Date] = None
     patent_number: tp.Optional[str] = None
     patent_issue_date: tp.Optional[Date] = None
     app_location: tp.Optional[str] = None
     app_grp_art_number: tp.Optional[str] = None
@@ -148,36 +140,47 @@
     def __repr__(self):
         return f"USApplication(appl_id='{self.appl_id}', patent_title='{self.patent_title}', app_status='{self.app_status}')"
 
     # Data removed by USPTO
 
     @property
     def attorneys(self):
-        raise RemovedDataException("Attorney information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+        raise RemovedDataException(
+            "Attorney information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
 
     @property
     def expiration(self):
-        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def pta_pte_summary(self):
-        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def pta_pte_tran_history(self):
-        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def parent_continuity(self):
-        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-    
+        raise RemovedDataException(
+            "Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
+
     @property
     def child_continuity(self):
-        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
-
+        raise RemovedDataException(
+            "Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html"
+        )
 
     @property
     def patent_center_link(self) -> str:
         return f"https://patentcenter.uspto.gov/applications/{self.appl_id}"
 
     @property
     def google_patents_link(self) -> tp.Optional[str]:
@@ -230,42 +233,36 @@
         return self._get_model(".Document").objects.filter(appl_id=self.appl_id)
 
     @property
     def related_assignments(
         self,
     ) -> tp.Iterable["Assignment"]:
         """Related Assignments from the Assignments API"""
-        return self._get_model("..assignment.model.Assignment").objects.filter(
-            appl_id=self.appl_id
-        )
+        return self._get_model("..assignment.model.Assignment").objects.filter(appl_id=self.appl_id)
 
     @property
     def ptab_proceedings(
         self,
     ) -> tp.Iterable["PtabProceeding"]:
         """Related PtabProceedings for this application"""
-        return self._get_model("..ptab.model.PtabProceeding").objects.filter(
-            appl_id=self.appl_id
-        )
+        return self._get_model("..ptab.model.PtabProceeding").objects.filter(appl_id=self.appl_id)
 
     @property
     def patent(self) -> tp.Optional["Patent"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("..public_search.model.Patent").objects.get(
             publication_number=self.patent_number
         )
 
     @property
     def publication(
         self,
     ) -> tp.Optional["PublishedApplication"]:
         """Fulltext version of the Publication - If Available"""
-        return self._get_model(
-            "..public_search.model.PublishedApplication"
-        ).objects.get(
+        return self._get_model("..public_search.model.PublishedApplication").objects.get(
             publication_number=self.publication_number,
         )
 
     @property
     def inpadoc_patent(
         self,
     ) -> tp.Optional["InpadocBiblio"]:
@@ -292,17 +289,15 @@
             "corrAddrNameLineTwo",
             "corrAddrNameLineThree",
         ]
         values["corrName"] = " ".join(
             [values[field] for field in correspondent_name_fields if field in values]
         )
         correspondent_adddress_lines = "\n".join(
-            values[f]
-            for f in ("corrAddrStreetLineOne", "corrAddrStreetLineTwo")
-            if f in values
+            values[f] for f in ("corrAddrStreetLineOne", "corrAddrStreetLineTwo") if f in values
         )
         correspondent_address_last_line = f"{values.get('corrAddrCity', '')}, {values.get('corrAddrGeoRegionCode', '')} {values.get('corrAddrPostalCode', '')}"
         if "corrAddrCountryName" in values:
             correspondent_address_last_line += f" ({values['corrAddrCountryName']})"
         values["corrAddress"] = "\n".join(
             [correspondent_adddress_lines, correspondent_address_last_line]
         )
@@ -392,21 +387,17 @@
         full_url = f"https://ped.uspto.gov/api/queries/cms/{self.pdf_url}"
         out_path = client.download(full_url, path=path)
         return out_path
 
     @computed_field
     @property
     def application(self) -> USApplication:
-        return self._get_model(".USApplication").objects.get(
-            appl_id=self.application_number_text
-        )
+        return self._get_model(".USApplication").objects.get(appl_id=self.application_number_text)
 
 
 class PedsPage(PEDSBaseModel):
     num_found: int = Field(
-        validation_alias=AliasPath(
-            "queryResults", "searchResponse", "response", "numFound"
-        )
+        validation_alias=AliasPath("queryResults", "searchResponse", "response", "numFound")
     )
     applications: tp.List[USApplication] = Field(
         validation_alias=AliasPath("queryResults", "searchResponse", "response", "docs")
     )
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/query.py` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/peds/search_index.csv` & `patent_client-5.0.3/patent_client/_sync/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/__init__.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,15 @@
             "applicationNumberText": application_number,
             "recordStartNumber": start,
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
 
-        query_dict = update_query_with_date(
-            document_filing_date, "documentFiling", query_dict
-        )
+        query_dict = update_query_with_date(document_filing_date, "documentFiling", query_dict)
 
         response = client.get(
             url="https://developer.uspto.gov/ptab-api/documents", params=query_dict
         )
         response.raise_for_status()
         return PtabDocumentPage.model_validate_json(response.content)
 
@@ -167,20 +165,16 @@
             "recordStartNumber": start,
             "recordTotalQuantity": rows,
             "sortOrderCategory": sort,
         }
         query_dict = {k: v for k, v in query_dict.items() if v is not None}
         query_dict = update_query_with_date(declaration_date, "declaration", query_dict)
         query_dict = update_query_with_date(institution_date, "institution", query_dict)
-        query_dict = update_query_with_date(
-            proceeding_filing_date, "proceedingFiling", query_dict
-        )
-        query_dict = update_query_with_date(
-            accorded_filing_date, "accordedFiling", query_dict
-        )
+        query_dict = update_query_with_date(proceeding_filing_date, "proceedingFiling", query_dict)
+        query_dict = update_query_with_date(accorded_filing_date, "accordedFiling", query_dict)
         query_dict = update_query_with_date(
             proceeding_last_modified_date, "proceedingLastModified", query_dict
         )
         query_dict = update_query_with_date(grant_date, "grant", query_dict)
 
         response = client.get(
             url="https://developer.uspto.gov/ptab-api/proceedings", params=query_dict
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/api_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *           Source File: patent_client/_async/uspto/ptab/api_test.py           *
 # ********************************************************************************
 
-import pytest
 
 from .api import PtabApi
 
 
 class TestPtabApi:
-    
     def test_can_get_document(self):
         page = PtabApi.get_documents(document_identifier="170680401")
         assert len(page.docs) == 1
 
-    
     def test_can_get_document_range(self):
         page = PtabApi.get_documents(
             proceeding_number="IPR2022-00037",
             document_filing_date=("2023-01-01", "2023-09-15"),
         )
         assert len(page.docs) == 25
 
-    
     def test_can_get_proceeding(self):
         page = PtabApi.get_proceedings(proceeding_number="IPR2022-00037")
         assert len(page.docs) == 1
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,35 +23,30 @@
     instance_schema = None
     api_method: Optional[Callable] = None
 
     def _get_results(self):
         query = deepcopy(self.config.filter)
         query = peds_to_ptab(query)
         query["sort"] = " ".join(
-            inflection.camelize(o, uppercase_first_letter=False)
-            for o in self.config.order_by
+            inflection.camelize(o, uppercase_first_letter=False) for o in self.config.order_by
         )
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, self.page_size
         ):
             query["start"] = start
             query["rows"] = rows
             page = self.api_method(**query)
             for doc in page.docs:
                 yield doc
             if len(page.docs) < rows:
                 break
 
     def count(self):
         page = self.api_method(**peds_to_ptab(self.config.filter))
-        return (
-            min(self.config.limit, page.num_found)
-            if self.config.limit
-            else page.num_found
-        )
+        return min(self.config.limit, page.num_found) if self.config.limit else page.num_found
 
     # def allowed_filters(self):
     #    params = schema_doc["paths"][self.path]["get"]["parameters"]
     #    return {inflection.underscore(p["name"]): p["description"] for p in params}
 
 
 class PtabProceedingManager(PtabManager[PtabProceeding]):
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/manager_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,55 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/uspto/ptab/manager_test.py         *
 # ********************************************************************************
 
-import pytest
 
 from .model import PtabDecision, PtabDocument, PtabProceeding
 
 
 class TestPtabProceeding:
-    
     def test_get_by_proceeding_number(self):
         result = PtabProceeding.objects.get("IPR2016-00831")
         assert result.respondent_patent_number == "6162705"
 
-    
     def test_get_by_patent_number(self):
         result = PtabProceeding.objects.get(patent_number="6103599")
         assert result.proceeding_number == "IPR2016-00833"
 
-    
     def test_get_by_application_number(self):
         result = PtabProceeding.objects.get(appl_id="09089931")
         assert result.proceeding_number == "IPR2016-00833"
 
-    
     def test_filter_by_party(self):
         result = PtabProceeding.objects.filter(party_name="Apple")
         assert result.count() >= 400
 
-    
     def test_filter_with_limit(self):
         result = PtabProceeding.objects.filter(party_name="Apple").limit(26)
         assert result.count() == 26
         objects = [a for a in result]
         assert len(objects) == 26
 
-    
     def test_offset(self):
         result = PtabProceeding.objects.filter(party_name="Apple").limit(3)
         objects = [a for a in result]
         assert result.first() == objects[0]
         assert result.offset(1).first() == objects[1]
         assert result.offset(1).offset(1).first() == objects[2]
 
 
 class TestPtabDocument:
-    
     def test_filter_by_proceeding(self):
         result = PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
         assert result.count() == 77
 
-    
     def test_sort_by_document_number(self):
-        result = (
-            PtabDocument.objects.filter(proceeding_number="IPR2016-00831")
-            .limit(3)
-            .count()
-        )
+        result = PtabDocument.objects.filter(proceeding_number="IPR2016-00831").limit(3).count()
         assert result == 3
 
 
 class TestPtabDecision:
-    
     def test_get_by_proceeding(self):
         result = PtabDecision.objects.get(proceeding_number="IPR2016-00831")
-        assert (
-            result.identifier
-            == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
-        )
+        assert result.identifier == "a44c5f1557b7b60d00e66604d3668ce442d53f964aa597011cc476b4"
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/model.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *            Source File: patent_client/_async/uspto/ptab/model.py             *
 # ********************************************************************************
 
 import datetime
 import re
-from pathlib import Path
 import typing as tp
+from pathlib import Path
 
 from pydantic import BeforeValidator, ConfigDict, Field
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel, DateTime
 
@@ -173,15 +173,17 @@
         filename = filename.encode(encoding="ascii", errors="ignore").decode("ascii")
         filename = fname_re.sub("", filename)
         out_path = Path(path) if path else Path.cwd()
         if out_path.is_dir():
             out_path = Path(path) / filename
         else:
             out_path = out_path
-        download_url = f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
+        download_url = (
+            f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
+        )
         return client.download(download_url, path=out_path)
 
 
 class PtabDecision(PtabBaseModel):
     proceeding_number: str
     board_rulings: tp.List[str] = Field(default_factory=list)
     decision_type_category: tp.Optional[str] = None
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/ptab/util.py` & `patent_client-5.0.3/patent_client/_sync/uspto/ptab/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/__init__.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/api.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,24 +30,27 @@
 
 class PublicSearchApi:
     def __init__(self):
         self.client = PatentClientSession(
             headers={
                 "X-Requested-With": "XMLHttpRequest",
                 "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+                "Origin": "https://ppubs.uspto.gov",
+                "Referer": "https://ppubs.uspto.gov/pubwebapp/",
+                "Pragma": "no-cache",
+                "Cache-Control": "no-cache",
+                "Priority": "u=1, i",
             },
             http2=True,
             follow_redirects=True,
         )
         self.session = dict()
         self.case_id = None
         self.queries = dict()
-        self.search_query = json.loads(
-            (Path(__file__).parent / "search_query.json").read_text()
-        )
+        self.search_query = json.loads((Path(__file__).parent / "search_query.json").read_text())
 
     def run_query(
         self,
         query,
         start=0,
         limit=500,
         sort="date_publ desc",
@@ -76,17 +79,15 @@
 
         counts = self.make_request(
             "POST",
             "https://ppubs.uspto.gov/dirsearch-public/searches/counts",
             json=data["query"],
         )
         counts.raise_for_status()
-        search_url = (
-            "https://ppubs.uspto.gov/dirsearch-public/searches/searchWithBeFamily"
-        )
+        search_url = "https://ppubs.uspto.gov/dirsearch-public/searches/searchWithBeFamily"
         query_response = self.make_request("POST", search_url, json=data)
         query_response.raise_for_status()
         result = query_response.json()
         if result.get("error", None) is not None:
             raise UsptoException(
                 f"Error #{result['error']['errorCode']}\n{result['error']['errorMessage']}"
             )
@@ -135,15 +136,15 @@
 
     def _request_save(self, obj):
         page_keys = [
             f"{obj.image_location}/{i:0>8}.tif"
             for i in range(1, obj.document_structure.page_count + 1)
         ]
         response = self.client.post(
-            "https://ppubs.uspto.gov/dirsearch-public/print/imageviewer",
+            "https://ppubs.uspto.gov/dirsearch-public/internal/print/imageviewer",
             json={
                 "caseId": self.case_id,
                 "pageKeys": page_keys,
                 "patentGuid": obj.guid,
                 "saveOrPrint": "save",
                 "source": obj.type,
             },
@@ -161,30 +162,30 @@
         try:
             print_job_id = self._request_save(obj)
         except httpx.HTTPStatusError:
             self.get_session()
             print_job_id = self._request_save(obj)
         while True:
             response = self.client.post(
-                "https://ppubs.uspto.gov/dirsearch-public/print/print-process",
+                "https://ppubs.uspto.gov/dirsearch-public/internal/print/print-process",
                 json=[
                     print_job_id,
                 ],
             )
             response.raise_for_status()
             print_data = response.json()
             if print_data[0]["printStatus"] == "COMPLETED":
                 break
             asyncio.sleep(1)
         pdf_name = print_data[0]["pdfName"]
         with out_path.open("wb") as f:
             try:
                 request = self.client.build_request(
                     "GET",
-                    f"https://ppubs.uspto.gov/dirsearch-public/print/save/{pdf_name}",
+                    f"https://ppubs.uspto.gov/dirsearch-public/internal/print/save/{pdf_name}",
                 )
                 response = self.client.send(request, stream=True)
                 response.raise_for_status()
                 for chunk in response.iter_bytes():
                     if chunk:
                         f.write(chunk)
             except httpx.HTTPStatusError as e:
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/biblio.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/document.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/document.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,43 +39,35 @@
 class UsReferenceSchema(ZipSchema):
     publication_number = f.String("urpn")
     # us_class = f.String("usRefClassification")
     # cpc_class = f.String("usRefCpcClassification")
     # group = f.String("usRefGroup")
     pub_month = f.Date(
         "usRefIssueDate",
-        dt_converter=lambda s: datetime.datetime(
-            year=int(s[:4]), month=int(s[4:6]), day=1
-        ),
+        dt_converter=lambda s: datetime.datetime(year=int(s[:4]), month=int(s[4:6]), day=1),
     )
     patentee_name = f.String("usRefPatenteeName")
     cited_by_examiner = f.Boolean("usRefGroup", true_func=lambda s: "examiner" in s)
 
 
 class ForeignReferenceSchema(ZipSchema):
     citation_classification = f.String("foreignRefCitationClassification")
     citation_cpc = f.String("foreignRefCitationCpc")
     country_code = f.String("foreignRefCountryCode")
     # group = f.String("foreignRefGroup")
     patent_number = f.String("foreignRefPatentNumber")
     pub_month = f.Date(
         "foreignRefPubDate",
-        dt_converter=lambda s: datetime.datetime(
-            year=int(s[:4]), month=int(s[4:6]), day=1
-        ),
-    )
-    cited_by_examiner = f.Boolean(
-        "foreignRefGroup", true_func=lambda s: "examiner" in s
+        dt_converter=lambda s: datetime.datetime(year=int(s[:4]), month=int(s[4:6]), day=1),
     )
+    cited_by_examiner = f.Boolean("foreignRefGroup", true_func=lambda s: "examiner" in s)
 
 
 class NplReferenceSchema(RegexSchema):
-    __regex__ = (
-        r"(?P<citation>.*)(?P<cited_by_examiner>cited by (applicant|examiner).?$)"
-    )
+    __regex__ = r"(?P<citation>.*)(?P<cited_by_examiner>cited by (applicant|examiner).?$)"
     citation = f.String()
     cited_by_examiner = f.Bool(true_func=lambda s: "examiner" in s)
 
 
 class RelatedApplicationSchema(ZipSchema):
     child_patent_country = f.String("relatedApplChildPatentCountry")
     child_patent_number = f.String("relatedApplChildPatentNumber")
@@ -172,30 +164,22 @@
     composite_id = f.String("compositeId")
     database_name = f.String("databaseName")
     derwent_week_int = f.Integer("derwentWeekInt")
 
     # References Cited
     us_references = UsReferenceSchema(data_key=False)
     foreign_references = ForeignReferenceSchema(data_key=False)
-    npl_references = f.DelimitedString(
-        NplReferenceSchema, "otherRefPub.0", delimeter="<br />"
-    )
+    npl_references = f.DelimitedString(NplReferenceSchema, "otherRefPub.0", delimeter="<br />")
 
     # Classifications
     cpc_inventive = f.List(CpcCodeSchema)
     cpc_additional = f.List(CpcCodeSchema)
 
     intl_class_issued = f.DelimitedString(f.String, "ipcCodeFlattened", delimeter=";")
-    intl_class_current_primary = f.List(
-        IntlCodeSchema, "curIntlPatentClassificationPrimary"
-    )
-    intl_class_currrent_secondary = f.List(
-        IntlCodeSchema, "curIntlPatentClassificationSecondary"
-    )
+    intl_class_current_primary = f.List(IntlCodeSchema, "curIntlPatentClassificationPrimary")
+    intl_class_currrent_secondary = f.List(IntlCodeSchema, "curIntlPatentClassificationSecondary")
 
-    us_class_current = f.DelimitedString(
-        f.Str(), "uspcFullClassificationFlattened", delimeter=";"
-    )
+    us_class_current = f.DelimitedString(f.Str(), "uspcFullClassificationFlattened", delimeter=";")
     us_class_issued = f.List(f.Str, "issuedUsClassificationFull")
 
     field_of_search_us = f.List(f.Str(), "fieldOfSearchClassSubclassHighlights")
     field_of_search_cpc = f.List(f.Str(), "fieldOfSearchCpcClassification")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert/shared.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/convert_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/count_query.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *       Source File: patent_client/_async/uspto/public_search/manager.py       *
 # ********************************************************************************
 
-from typing import Iterator, Generic, TypeVar
+from typing import Generic, Iterator, TypeVar
 
 from patent_client.util.manager import Manager
 from patent_client.util.request_util import get_start_and_row_count
 
 from .api import PublicSearchApi
 from .model import (
     Patent,
@@ -102,17 +102,15 @@
             yield doc
 
 
 class PublicSearchBiblioManager(GenericPublicSearchBiblioManager[PublicSearchBiblio]):
     pass
 
 
-class PublicSearchDocumentManager(
-    GenericPublicSearchDocumentManager[PublicSearchDocument]
-):
+class PublicSearchDocumentManager(GenericPublicSearchDocumentManager[PublicSearchDocument]):
     pass
 
 
 class PatentBiblioManager(GenericPublicSearchBiblioManager[PatentBiblio]):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
@@ -134,15 +132,13 @@
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "US-PGPUB",
         ]
 
 
-class PublishedApplicationManager(
-    GenericPublicSearchDocumentManager[PublishedApplication]
-):
+class PublishedApplicationManager(GenericPublicSearchDocumentManager[PublishedApplication]):
     def __init__(self, config=None):
         super().__init__(config=config)
         self.config.options["sources"] = [
             "US-PGPUB",
         ]
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/manager_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/manager_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,38 +12,33 @@
     PublicSearchDocument,
     PublishedApplication,
     PublishedApplicationBiblio,
 )
 
 
 class TestPatents:
-    
     def test_simple_lookup(self):
         app = PublicSearchDocument.objects.get(patent_number="6103599")
         assert app.appl_id == "09089931"
         assert app.guid == "US-6103599-A"
         assert app.patent_title == "Planarizing technique for multilayered substrates"
 
-    
     def test_tennis_patents(self):
         tennis_patents = Patent.objects.filter(title="tennis", assignee_name="wilson")
         assert tennis_patents.count() > 10
 
-    
     def test_fetch_patent(self):
         pat = Patent.objects.get(6095661)
         assert pat.patent_title == "Method and apparatus for an L.E.D. flashlight"
         assert len(pat.abstract) == 1543
 
-    
     def test_government_interest(self):
         pat = Patent.objects.get(11555621)
         assert pat.document.government_interest is not None
 
-    
     def test_claims(self):
         pat = Patent.objects.get(6095661)
         assert len(pat.claims) == 52
         assert pat.claims[0].number == 1
         assert len(pat.claims[0].text) == 1269
         assert len(pat.claims[0].limitations) == 5
         assert pat.claims[30].number == 31
@@ -54,116 +49,97 @@
         assert pat.claims[30].depends_on == list()
         assert pat.claims[31].dependent
         assert not pat.claims[31].independent
         assert pat.claims[31].depends_on == [
             31,
         ]
 
-    
     def test_us8645300(self):
         pat_no = 8645300
         pat = Patent.objects.get(pat_no)
         assert pat.patent_title == "System and method for intent data processing"
 
-    
     def test_search_classification(self):
         query = '"B60N2/5628".CPC. AND @APD>="20210101"<=20210107'
         results = Patent.objects.filter(query=query)
         assert results.count() >= 1
         app = results.first()
         assert app.publication_number == "11554698"
 
-    
     def test_can_fetch_reissue_applications(self):
         pat_no = "RE43633"
         pat = Patent.objects.get(pat_no)
         assert (
             pat.patent_title
             == "System and method for linking streams of multimedia data to reference material for display"
         )
         assert pat.claims[0].text[:25] == "1. .[.A system for linkin"
 
-    
     def test_can_get_field_of_search(self):
         pat_no = "9140110"
         pat = Patent.objects.get(pat_no)
         assert len(pat.field_of_search_us) >= 6
         pat_no = "8832265"
         pat = Patent.objects.get(pat_no)
         assert len(pat.field_of_search_us) == 7
 
-    
     def test_handles_disclaimers(self):
         """Some patents have notice markers on the issue date regarding statutory disclaimers"""
         pat = Patent.objects.get("5439055")
         assert pat.publication_date.isoformat() == "1995-08-08"
 
-    
     def test_handles_claims_for_US6460631(self):
         pat = Patent.objects.get(6460631)
         for claim in pat.claims:
             pass
         assert True
 
-    
     def test_handles_search_without_results(self):
-        query = Patent.objects.filter(
-            query='"379/56".CCLS. AND @APD>=19700101<=19950928'
-        )
+        query = Patent.objects.filter(query='"379/56".CCLS. AND @APD>=19700101<=19950928')
         assert query.count() == 0
 
-    
     def test_can_get_forward_references(self):
         pat = Patent.objects.get(6103599)
         forward_refs = pat.forward_citations
         assert forward_refs.count() >= 100
 
-    
     def test_classifications_with_foreign_priority_data(self):
         pat = Patent.objects.get(7752445)
         assert len(pat.us_class_issued) == 6
         assert pat.foreign_priority[0].app_number == "2004-052835"
 
-    
     def test_can_get_design_patents(self):
         pat = Patent.objects.get("D645062")
         assert pat.patent_title == "Gripping arm"
         assert pat.appl_id == "29380046"
 
-    
     def test_search_that_has_single_patent(self):
-        result = Patent.objects.filter(
-            title="tennis", issue_date="2010-01-01->2010-02-27"
-        )
+        result = Patent.objects.filter(title="tennis", issue_date="2010-01-01->2010-02-27")
         assert result.count() == 1
         obj = result.first()
         assert obj.publication_number == "7658211"
         assert obj.patent_title == "Tennis ball recharging apparatus method"
 
-    @pytest.mark.skip("This test is too slow")
-    @pytest.mark.no_vcr
     def test_can_get_images(self, tmp_path):
         pat = Patent.objects.get("6103599")
-        path = pat.adownload_images(path=tmp_path)
+        path = pat.download_images(path=tmp_path)
         assert path == tmp_path / "US-6103599-A.pdf"
         assert path.exists()
 
 
 class TestPublishedApplicationFullTextAsync:
-    
     def test_fetch_publication(self):
         pub_no = 20_160_009_839
         pub = PublishedApplication.objects.get(pub_no)
         assert (
             pub.patent_title
             == "POLYMER PRODUCTS AND MULTI-STAGE POLYMERIZATION PROCESSES FOR THE PRODUCTION THEREOF"
         )
         assert len(pub.abstract) == 651
 
-    
     def test_publication_claims(self):
         pub_no = 20_160_009_839
         pub = PublishedApplication.objects.get(pub_no)
         assert len(pub.claims) == 25
         # Test Claim 1
         claim_1 = pub.claims[0]
         assert claim_1.number == 1
@@ -171,47 +147,43 @@
         assert len(claim_1.limitations) == 3
         assert claim_1.independent
         # Test Dependent Claim 2
         claim_2 = pub.claims[1]
         assert claim_2.number == 2
         assert claim_2.dependent
 
-    
     def test_us_pub_20170370151(self):
         pub_no = 20_170_370_151
         pub = PublishedApplication.objects.get(pub_no)
         for i in range(6):
             assert pub.claims[i].text == f"{i + 1}. (canceled)"
         assert (
             "A system to control directional drilling in borehole drilling for"
             in pub.claims[6].text
         )
 
-    
     def test_search_classification(self):
         query = '"166/308.1".CCLS. AND @APD>=20150101<=20210101'
         results = PublishedApplicationBiblio.objects.filter(query=query)
         assert results.count() == 41
         counter = 0
         for _ in results:
             counter += 1
         assert counter == 41
 
-    
     def test_nonstandard_claim_format(self):
         obj = PublishedApplication.objects.get("20170260839")
         assert obj.claims[0].text[:39] == "1. A method of well ranging comprising:"
 
     @pytest.mark.skip("This test is too slow")
     def test_can_get_images(self, tmp_path):
         pat = PublishedApplication.objects.get("20090150362")
         pat.adownload_images(path=tmp_path)
         assert (tmp_path / "US-20090150362-A1.pdf").exists()
 
-    
     def test_pages(self):
         pats = PatentBiblio.objects.filter(title="system").limit(525)
         old_p = None
         counter = 0
         for p in pats:
             counter += 1
             assert p != old_p
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/__init__.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 
 __all__ = [
     "PatentBiblio",
     "Patent",
     "PublishedApplicationBiblio",
     "PublishedApplication",
     "PublicSearchBiblio",
+    "PublicSearchBiblioPage",
     "PublicSearchDocument",
     "PublicSearchDocument",
 ]
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/biblio.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/biblio.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,26 @@
 from typing import Optional
 
 from pydantic import AliasPath, Field, model_validator
 
 from patent_client.util.pydantic_util import BaseModel
 
 from ..convert.biblio import PublicSearchBiblioPageSchema
-from .shared import (
-    ApplicationNumber,
-    DateTimeAsDate,
-    DocumentStructure,
-    HtmlString,
-    OptionalList,
-)
+from .shared import ApplicationNumber, DateTimeAsDate, DocumentStructure, HtmlString, OptionalList
 
 
 class PublicSearchBiblio(BaseModel):
     guid: Optional[str] = None
     publication_number: Optional[str] = None
     publication_date: Optional[datetime.date] = None
     patent_title: Optional[HtmlString] = None
     type: Optional[str] = None
     main_classification_code: Optional[str] = None
-    applicant_names: OptionalList[str] = Field(
-        alias="applicant_name", default_factory=list
-    )
-    assignee_names: OptionalList[str] = Field(
-        alias="assignee_name", default_factory=list
-    )
+    applicant_names: OptionalList[str] = Field(alias="applicant_name", default_factory=list)
+    assignee_names: OptionalList[str] = Field(alias="assignee_name", default_factory=list)
     uspc_full_classification: OptionalList[str] = Field(default_factory=list)
     ipc_code: OptionalList[str] = Field(default_factory=list)
     cpc_additional: OptionalList[str] = Field(default_factory=list)
     app_filing_date: Optional[datetime.date] = None
     related_appl_filing_date: OptionalList[DateTimeAsDate] = Field(
         alias="relatedApplFilingDate", default_factory=list
     )
@@ -63,17 +53,17 @@
 
     @property
     def application(self):
         return self._get_model("...peds.model.USApplication").objects.get(self.appl_id)
 
     @property
     def global_dossier(self):
-        return self._get_model(
-            "...global_dossier.model.GlobalDossierApplication"
-        ).objects.get(self.appl_id)
+        return self._get_model("...global_dossier.model.GlobalDossierApplication").objects.get(
+            self.appl_id
+        )
 
     @property
     def assignments(self):
         return self._get_model("...assignment.model.Assignment").objects.filter(
             appl_id=self.appl_id
         )
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/document.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,17 +206,17 @@
 
     @property
     def application(self):
         return self._get_model("...peds.model.USApplication").objects.get(self.appl_id)
 
     @property
     def global_dossier(self):
-        return self._get_model(
-            "...global_dossier.model.GlobalDossierApplication"
-        ).objects.get(self.appl_id)
+        return self._get_model("...global_dossier.model.GlobalDossierApplication").objects.get(
+            self.appl_id
+        )
 
     @property
     def assignments(self):
         return self._get_model("...assignment.model.Assignment").objects.filter(
             appl_id=self.appl_id
         )
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model/shared.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/model/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,15 @@
         str_strip_whitespace=True,
     )
 
 
 T = TypeVar("T")
 
 
-OptionalList = Annotated[
-    List[T], BeforeValidator(lambda x: x if isinstance(x, list) else list())
-]
+OptionalList = Annotated[List[T], BeforeValidator(lambda x: x if isinstance(x, list) else list())]
 DateTimeAsDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: x.date() if isinstance(x, datetime.datetime) else x),
 ]
 HtmlString = Annotated[str, BeforeValidator(html_to_text)]
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/model_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/query.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 
 class QueryBuilder:
     def __init__(self):
         config_file = Path(__file__).parent / "query_config.csv"
         with config_file.open(encoding="utf-8-sig") as csvfile:
             reader = csv.DictReader(csvfile)
             config = list(reader)
-        self.search_keywords = {
-            r["keyword"]: r["query_field"] for r in config if r["query_field"]
-        }
+        self.search_keywords = {r["keyword"]: r["query_field"] for r in config if r["query_field"]}
         self.order_by_keywords = {
             r["keyword"]: r["order_by_field"] for r in config if r["order_by_field"]
         }
         self.date_fields = [r["keyword"] for r in config if r["is_date"] == "X"]
 
     def convert_date(self, date):
         if isinstance(date, str):
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_config.csv` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/query_test.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/query_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,63 +13,51 @@
 
 class QueryTest:
     def test_default_query(self):
         assert PatentBiblioManager().filter("6103599")._query == '"6103599".PN.'
 
     def test_plural_default_query(self):
         assert (
-            PatentBiblioManager().filter("6103599", "6103600")._query
-            == '("6103599" "6103600").PN.'
+            PatentBiblioManager().filter("6103599", "6103600")._query == '("6103599" "6103600").PN.'
         )
 
     def test_keyword_query(self):
-        assert (
-            PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
-        )
+        assert PatentBiblioManager().filter(appl_id="6103599")._query == '"6103599".APNR.'
 
     def test_plural_keyword_query(self):
         assert (
             PatentBiblioManager().filter(appl_id=("11111111", "11222222"))._query
             == '("11111111" "11222222").APNR.'
         )
 
     def test_keyword_date_query(self):
         assert (
-            PatentBiblioManager().filter(app_filing_date="2021-01-01")._query
-            == '@APD="20210101"'
+            PatentBiblioManager().filter(app_filing_date="2021-01-01")._query == '@APD="20210101"'
         )
         assert (
             PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01"))._query
             == '@APD="20210101"'
         )
         assert (
-            PatentBiblioManager()
-            .filter(app_filing_date=parse_dt("2021-01-01").date())
-            ._query
+            PatentBiblioManager().filter(app_filing_date=parse_dt("2021-01-01").date())._query
             == '@APD="20210101"'
         )
 
     def test_keyword_date_range_query(self):
         assert (
-            PatentBiblioManager()
-            .filter(app_filing_date="2021-01-01->2021-02-01")
-            ._query
+            PatentBiblioManager().filter(app_filing_date="2021-01-01->2021-02-01")._query
             == "@APD>=20210101<=20210201"
         )
         assert (
-            PatentBiblioManager()
-            .filter(app_filing_date__range=("2021-01-01", "2021-02-01"))
-            ._query
+            PatentBiblioManager().filter(app_filing_date__range=("2021-01-01", "2021-02-01"))._query
             == "@APD>=20210101<=20210201"
         )
         assert (
             PatentBiblioManager()
-            .filter(
-                app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01"))
-            )
+            .filter(app_filing_date__range=(parse_dt("2021-01-01"), parse_dt("2021-02-01")))
             ._query
             == "@APD>=20210101<=20210201"
         )
 
     def test_date_operator_queries(self):
         assert (
             PatentBiblioManager().filter(app_filing_date__gt="2021-01-01")._query
@@ -100,38 +88,30 @@
 
     def test_multiple_fields(self):
         assert (
             PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
             == '@APD="20210101" AND "6103599".PN.'
         )
         assert (
-            PatentBiblioManager()
-            .filter("6103599")
-            .filter(app_filing_date="2021-01-01")
-            ._query
+            PatentBiblioManager().filter("6103599").filter(app_filing_date="2021-01-01")._query
             == '"6103599".PN. AND @APD="20210101"'
         )
         assert (
             PatentBiblioManager()
             .filter(patent_number="6103599", app_filing_date="2021-01-01")
             ._query
             == '@APD="20210101" AND "6103599".PN.'
         )
 
     def test_raw_query(self):
-        assert (
-            PatentBiblioManager().filter(query="example query")._query
-            == "example query"
-        )
+        assert PatentBiblioManager().filter(query="example query")._query == "example query"
 
     def test_raw_query_with_keywords(self):
         assert (
-            PatentBiblioManager()
-            .filter(query="some text", patent_number="6103599")
-            ._query
+            PatentBiblioManager().filter(query="some text", patent_number="6103599")._query
             == '"6103599".PN. AND some text'
         )
 
     def test_default_or(self):
         assert (
             PatentBiblioManager()
             .option(default_operator="OR")
```

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/search_query.json` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/_sync/uspto/public_search/util.py` & `patent_client-5.0.3/patent_client/_sync/uspto/public_search/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/parser.py` & `patent_client-5.0.3/patent_client/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,15 @@
             elif self.type == "patent" and self.number.isdigit():
                 formatted_number = "{:,}".format(int(self.number))
             elif self.type == "design patent":
                 formatted_number = self.number
             elif self.type == "patent":
                 formatted_number = self.number
             elif self.type == "application":
-                formatted_number = (
-                    self.number[:2] + "/" + self.number[2:5] + "," + self.number[5:]
-                )
+                formatted_number = self.number[:2] + "/" + self.number[2:5] + "," + self.number[5:]
             return f"US {formatted_number} {self.kind_code}".strip()
         elif self.country == "CA":
             return f"CA {self.number} {self.kind_code}"
         else:
             return f"{self.country} {self.number}"
 
     def abbreviation(self):
@@ -165,8 +163,10 @@
         else:
             raise ValueError()
 
     def __str__(self):
         return f"PCT{self.country}{self.year}{self.number}"
 
     def __repr__(self):
-        return f"<PCTApplication(country_code={self.country}, year={self.year}, number={self.number})>"
+        return (
+            f"<PCTApplication(country_code={self.country}, year={self.year}, number={self.number})>"
+        )
```

### Comparing `patent_client-5.0.2/patent_client/session.py` & `patent_client-5.0.3/patent_client/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
+import typing as tp
 import warnings
 from hashlib import blake2b
 from pathlib import Path
-import typing as tp
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
@@ -32,17 +32,15 @@
 patent_client_transport = hishel.AsyncCacheTransport(
     transport=httpx.AsyncHTTPTransport(
         verify=False,
         http2=True,
         retries=3,
     ),
     storage=hishel.AsyncFileStorage(base_path=CACHE_DIR),
-    controller=hishel.Controller(
-        allow_heuristics=True, key_generator=cache_key_generator
-    ),
+    controller=hishel.Controller(allow_heuristics=True, key_generator=cache_key_generator),
 )
 
 
 class PatentClientAsyncSession(httpx.AsyncClient):
     _default_user_agent = f"Mozilla/5.0 Python Patent Clientbot/{__version__} (parkerhancock@users.noreply.github.com)"
 
     def __init__(self, **kwargs):
```

### Comparing `patent_client-5.0.2/patent_client/settings.py` & `patent_client-5.0.3/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/test_parser.py` & `patent_client-5.0.3/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/asyncio_util.py` & `patent_client-5.0.3/patent_client/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-5.0.3/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-5.0.3/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/claims/examples/published_claims.json` & `patent_client-5.0.3/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/claims/examples/published_claims.txt` & `patent_client-5.0.3/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/claims/model.py` & `patent_client-5.0.3/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/claims/parser.py` & `patent_client-5.0.3/patent_client/util/claims/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,25 @@
     def parse_claim_string(self, text):
         number = int(NUMBER_RE.search(text).group("number"))
         text = NUMBER_RE.sub("", text)
         return {
             "number": number,
             # "text": NUMBER_RE.sub("", text),
             "limitations": [
-                clean_text("".join(lim))
-                for lim in list(grouper(LIMITATION_RE.split(text), 2, ""))
+                clean_text("".join(lim)) for lim in list(grouper(LIMITATION_RE.split(text), 2, ""))
             ],
             "depends_on": self.parse_dependency(text, number),
             "dependent_claims": list(),
         }
 
     def parse_dependency(self, text, number):
         dependency = DEPENDENCY_RE.search(text)
         if dependency is not None:
             claims = dependency.groupdict()["number"]
             claim_numbers = [
-                int(m.groupdict()["number"])
-                for m in DEPENDENT_CLAIMS_RE.finditer(claims)
+                int(m.groupdict()["number"]) for m in DEPENDENT_CLAIMS_RE.finditer(claims)
             ]
             return claim_numbers
         elif DEPEND_ALL_RE.search(text):
             return list(range(1, number))
         else:
             return list()
```

### Comparing `patent_client-5.0.2/patent_client/util/claims/parser_test.py` & `patent_client-5.0.3/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/format.py` & `patent_client-5.0.3/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/manager.py` & `patent_client-5.0.3/patent_client/util/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,15 @@
         self.config = config or ManagerConfig()
 
     # Manager Iteration / Slicing
 
     def __iter__(self) -> Iterator[ModelType]:
         return self._get_results()
 
-    def __getitem__(
-        self, key: Union[slice, int]
-    ) -> Union[Manager[ModelType], ModelType]:
+    def __getitem__(self, key: Union[slice, int]) -> Union[Manager[ModelType], ModelType]:
         if isinstance(key, slice):
             if key.step is not None:
                 raise AttributeError("Step is not supported")
             start = key.start if key.start else 0
             start = len(self) + start if start < 0 else start
             stop = key.stop if key.stop else len(self)
             stop = len(self) + stop if stop < 0 else stop
@@ -209,17 +207,15 @@
         return self._get_results()
 
     async def _get_results(self) -> AsyncIterator[ModelType]:
         raise NotImplementedError(
             f"This method must be defined in a subclass of {self.__class__.__name__}"
         )
 
-    async def __getitem__(
-        self, key: Union[slice, int]
-    ) -> Union[Manager[ModelType], ModelType]:
+    async def __getitem__(self, key: Union[slice, int]) -> Union[Manager[ModelType], ModelType]:
         if isinstance(key, slice):
             if key.step is not None:
                 raise AttributeError("Step is not supported")
             count = await self.count()
             start = key.start if key.start else 0
             start = count + start if start < 0 else start
             stop = key.stop if key.stop else count
```

### Comparing `patent_client-5.0.2/patent_client/util/pydantic_util.py` & `patent_client-5.0.3/patent_client/util/pydantic_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 import importlib
 import re
 import typing as tp
 
 from async_property.base import AsyncPropertyDescriptor
 from dateutil.parser import isoparse
 from dateutil.parser import parse as parse_dt
-from pydantic import BaseModel as PydanticBaseModel, BeforeValidator, ConfigDict
+from pydantic import BaseModel as PydanticBaseModel
+from pydantic import BeforeValidator, ConfigDict
 from typing_extensions import Annotated
 
 from patent_client.util.manager import Manager
 
 
 def parse_datetime(date_obj: tp.Union[str, datetime.datetime]) -> datetime.datetime:
     if isinstance(date_obj, datetime.datetime):
         return date_obj
     try:
         return isoparse(date_obj)
     except ValueError:
         return parse_dt(date_obj)
 
 
-def parse_date(date_obj: tp.Union[str, datetime.datetime, datetime.date]) -> datetime.date:
+def parse_date(
+    date_obj: tp.Union[str, datetime.datetime, datetime.date],
+) -> datetime.date:
     if isinstance(date_obj, datetime.date):
         return date_obj
     elif isinstance(date_obj, datetime.datetime):
         return date_obj.date()
     try:
         return isoparse(date_obj).date()
     except ValueError:
```

### Comparing `patent_client-5.0.2/patent_client/util/request_util.py` & `patent_client-5.0.3/patent_client/util/request_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.2/patent_client/util/test.py` & `patent_client-5.0.3/patent_client/util/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     dict_1_keys = set(dict_1.keys())
     dict_2_keys = set(dict_2.keys())
     in_1_not_2 = dict_1_keys - dict_2_keys
     in_2_not_1 = dict_2_keys - dict_1_keys
     if len(in_1_not_2) > 0:
         raise ValueError(f"At {key}, Keys {in_1_not_2} are in Dict 1, but not Dict 2")
     if len(in_2_not_1) > 0:
-        raise ValueError(
-            f"At {key}, Keys {in_2_not_1} are not in Dict 1, but are in Dict 2"
-        )
+        raise ValueError(f"At {key}, Keys {in_2_not_1} are not in Dict 1, but are in Dict 2")
 
     for k, v in dict_1.items():
         if isinstance(v, list) and not isinstance(v, str):
             return compare_lists(v, dict_2[k], key=f"{key}.{k}")
         elif isinstance(v, dict):
             return compare_dicts(v, dict_2[k], key=f"{key}.{k}")
         else:
```

### Comparing `patent_client-5.0.2/pyproject.toml` & `patent_client-5.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "5.0.2"
+version = "5.0.3"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
@@ -101,14 +101,17 @@
 [scripts]
 test = "pytest --basetemp=tmp"
 render_docs = "make -f docs/Makefile html"
 
 [tool.pycln]
 all = true
 
+[tool.ruff]
+line-length = 100
+
 [tool.isort]
 profile = 'black'
 line_length = 100
 skip_gitignore = true
 
 [tool.pytest.ini_options]
 python_files = [
```

### Comparing `patent_client-5.0.2/PKG-INFO` & `patent_client-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 5.0.2
+Version: 5.0.3
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
```

