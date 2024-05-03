# Comparing `tmp/patent_client-5.0.6.tar.gz` & `tmp/patent_client-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-5.0.6.tar", max compression
+gzip compressed data, was "patent_client-5.0.7.tar", max compression
```

## Comparing `patent_client-5.0.6.tar` & `patent_client-5.0.7.tar`

### file list

```diff
@@ -1,409 +1,409 @@
--rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.6/LICENSE
--rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.6/README.md
--rw-r--r--   0        0        0     1739 2024-05-03 17:25:00.646245 patent_client-5.0.6/patent_client/__init__.py
--rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.6/patent_client/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.6/patent_client/_async/epo/__init__.py
--rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.6/patent_client/_async/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.6/patent_client/_async/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      360 2024-05-03 17:25:00.646675 patent_client-5.0.6/patent_client/_async/epo/ops/family/api.py
--rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.6/patent_client/_async/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      356 2024-05-03 17:25:00.646963 patent_client-5.0.6/patent_client/_async/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.6/patent_client/_async/epo/ops/family/model.py
--rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.6/patent_client/_async/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1503 2024-05-03 17:25:00.647248 patent_client-5.0.6/patent_client/_async/epo/ops/family/schema.py
--rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.6/patent_client/_async/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.6/patent_client/_async/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.6/patent_client/_async/epo/ops/legal/api.py
--rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.6/patent_client/_async/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      467 2024-05-03 17:25:00.653744 patent_client-5.0.6/patent_client/_async/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.6/patent_client/_async/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5434 2024-05-03 17:25:00.657228 patent_client-5.0.6/patent_client/_async/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.6/patent_client/_async/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4018 2024-05-03 17:25:00.661652 patent_client-5.0.6/patent_client/_async/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.6/patent_client/_async/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.6/patent_client/_async/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.6/patent_client/_async/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.6/patent_client/_async/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5472 2024-05-03 17:25:00.661893 patent_client-5.0.6/patent_client/_async/epo/ops/published/api.py
--rw-r--r--   0        0        0     2699 2024-05-03 17:25:00.662175 patent_client-5.0.6/patent_client/_async/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.6/patent_client/_async/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-03 18:14:56.983992 patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-03 18:14:56.987365 patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-05-03 18:14:56.997023 patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3204 2024-05-03 17:25:00.662696 patent_client-5.0.6/patent_client/_async/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2411 2024-05-03 17:25:00.662959 patent_client-5.0.6/patent_client/_async/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.6/patent_client/_async/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.6/patent_client/_async/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.6/patent_client/_async/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2078 2024-05-03 17:25:00.663177 patent_client-5.0.6/patent_client/_async/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.6/patent_client/_async/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3934 2024-05-03 17:25:00.663421 patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1640 2024-05-03 17:25:00.664113 patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3160 2024-05-03 17:25:00.664661 patent_client-5.0.6/patent_client/_async/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-03 18:14:57.128503 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-03 18:14:57.132594 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.6/patent_client/_async/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3478 2024-05-03 17:25:00.664935 patent_client-5.0.6/patent_client/_async/epo/ops/session.py
--rw-r--r--   0        0        0     2881 2024-05-03 17:25:00.665195 patent_client-5.0.6/patent_client/_async/epo/ops/util.py
--rw-r--r--   0        0        0     3220 2024-05-03 17:25:00.665599 patent_client-5.0.6/patent_client/_async/http_client.py
--rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.6/patent_client/_async/odp.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.6/patent_client/_async/uspto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.6/patent_client/_async/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2538 2024-05-03 17:25:00.665812 patent_client-5.0.6/patent_client/_async/uspto/assignment/api.py
--rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.6/patent_client/_async/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     3595 2024-05-03 17:25:00.666143 patent_client-5.0.6/patent_client/_async/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.6/patent_client/_async/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3424 2024-05-03 17:25:00.666449 patent_client-5.0.6/patent_client/_async/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4158 2024-05-03 17:25:00.666715 patent_client-5.0.6/patent_client/_async/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5500 2024-05-03 17:25:00.666971 patent_client-5.0.6/patent_client/_async/uspto/assignment/model.py
--rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.6/patent_client/_async/uspto/assignment/model_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.6/patent_client/_async/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3182 2024-05-03 17:25:00.667431 patent_client-5.0.6/patent_client/_async/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.6/patent_client/_async/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.6/patent_client/_async/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.6/patent_client/_async/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1553 2024-05-03 17:25:00.667735 patent_client-5.0.6/patent_client/_async/uspto/bulk_data/model.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1762 2024-05-03 17:25:00.667994 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     6897 2024-05-03 17:25:00.668558 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6031 2024-05-03 17:25:00.668826 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.6/patent_client/_async/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5900 2024-05-03 17:59:27.275145 patent_client-5.0.6/patent_client/_async/uspto/odp/api.py
--rw-r--r--   0        0        0     2818 2024-05-03 17:25:00.669417 patent_client-5.0.6/patent_client/_async/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     5420 2024-05-03 18:16:50.562485 patent_client-5.0.6/patent_client/_async/uspto/odp/manager.py
--rw-r--r--   0        0        0     1953 2024-05-03 18:17:11.242859 patent_client-5.0.6/patent_client/_async/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16223 2024-05-03 18:15:54.884428 patent_client-5.0.6/patent_client/_async/uspto/odp/model.py
--rw-r--r--   0        0        0    12133 2024-05-03 17:25:00.670224 patent_client-5.0.6/patent_client/_async/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.6/patent_client/_async/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.6/patent_client/_async/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.6/patent_client/_async/uspto/odp/util.py
--rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.6/patent_client/_async/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.6/patent_client/_async/uspto/peds/api.py
--rw-r--r--   0        0        0      683 2024-05-03 17:25:00.670577 patent_client-5.0.6/patent_client/_async/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.6/patent_client/_async/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8619 2024-05-03 17:25:00.673086 patent_client-5.0.6/patent_client/_async/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8191 2024-05-03 17:25:00.673373 patent_client-5.0.6/patent_client/_async/uspto/peds/manager.py
--rw-r--r--   0        0        0     9623 2024-05-03 17:25:00.673653 patent_client-5.0.6/patent_client/_async/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    14958 2024-05-03 17:25:00.673984 patent_client-5.0.6/patent_client/_async/uspto/peds/model.py
--rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.6/patent_client/_async/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.6/patent_client/_async/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.6/patent_client/_async/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10134 2024-05-03 17:25:00.674181 patent_client-5.0.6/patent_client/_async/uspto/ptab/api.py
--rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.6/patent_client/_async/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.6/patent_client/_async/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.6/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2025 2024-05-03 17:25:00.674454 patent_client-5.0.6/patent_client/_async/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2249 2024-05-03 17:25:00.674630 patent_client-5.0.6/patent_client/_async/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8382 2024-05-03 17:25:00.674990 patent_client-5.0.6/patent_client/_async/uspto/ptab/model.py
--rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.6/patent_client/_async/uspto/ptab/util.py
--rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.6/patent_client/_async/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6921 2024-05-03 17:25:00.675209 patent_client-5.0.6/patent_client/_async/uspto/public_search/api.py
--rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.6/patent_client/_async/uspto/public_search/api_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6548 2024-05-03 17:25:00.680068 patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.6/patent_client/_async/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.6/patent_client/_async/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-03 18:14:59.917298 patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4132 2024-05-03 17:25:00.680395 patent_client-5.0.6/patent_client/_async/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7627 2024-05-03 17:25:00.680977 patent_client-5.0.6/patent_client/_async/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      554 2024-05-03 17:25:00.681546 patent_client-5.0.6/patent_client/_async/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3091 2024-05-03 17:25:00.681713 patent_client-5.0.6/patent_client/_async/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7574 2024-05-03 17:25:00.681893 patent_client-5.0.6/patent_client/_async/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2243 2024-05-03 17:25:00.682051 patent_client-5.0.6/patent_client/_async/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.6/patent_client/_async/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4498 2024-05-03 17:25:00.682225 patent_client-5.0.6/patent_client/_async/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.6/patent_client/_async/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4056 2024-05-03 17:25:00.682391 patent_client-5.0.6/patent_client/_async/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.6/patent_client/_async/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.6/patent_client/_async/uspto/public_search/util.py
--rw-r--r--   0        0        0     1249 2024-05-03 14:37:59.408803 patent_client-5.0.6/patent_client/_sync/__init__.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.946323 patent_client-5.0.6/patent_client/_sync/epo/__init__.py
--rw-r--r--   0        0        0      630 2024-05-03 14:37:59.957541 patent_client-5.0.6/patent_client/_sync/epo/ops/__init__.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.973334 patent_client-5.0.6/patent_client/_sync/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      764 2024-05-03 17:25:00.682574 patent_client-5.0.6/patent_client/_sync/epo/ops/family/api.py
--rw-r--r--   0        0        0      839 2024-05-03 17:25:00.682830 patent_client-5.0.6/patent_client/_sync/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-05-03 14:37:59.982146 patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-05-03 14:37:59.982491 patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-05-03 14:37:59.983472 patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-05-03 14:37:59.982936 patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      750 2024-05-03 17:25:00.684037 patent_client-5.0.6/patent_client/_sync/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1535 2024-05-03 14:37:59.975224 patent_client-5.0.6/patent_client/_sync/epo/ops/family/model.py
--rw-r--r--   0        0        0      887 2024-05-03 17:25:00.684290 patent_client-5.0.6/patent_client/_sync/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1919 2024-05-03 17:25:00.684469 patent_client-5.0.6/patent_client/_sync/epo/ops/family/schema.py
--rw-r--r--   0        0        0      943 2024-05-03 14:37:59.973183 patent_client-5.0.6/patent_client/_sync/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0      416 2024-05-03 14:38:00.071771 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      763 2024-05-03 14:38:00.076639 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/api.py
--rw-r--r--   0        0        0      688 2024-05-03 17:25:00.684808 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-05-03 14:38:00.108475 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-05-03 14:38:00.106613 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-05-03 14:38:00.108158 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-05-03 14:38:00.107017 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-05-03 14:38:00.107316 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-05-03 14:38:00.107797 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-05-03 14:38:00.105336 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      847 2024-05-03 17:25:00.693194 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2791 2024-05-03 14:38:00.075813 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5767 2024-05-03 17:25:00.694359 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      866 2024-05-03 17:25:00.695959 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4434 2024-05-03 17:25:00.697554 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1632 2024-05-03 14:38:00.071240 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      530 2024-05-03 14:38:00.071623 patent_client-5.0.6/patent_client/_sync/epo/ops/legal/util.py
--rw-r--r--   0        0        0      483 2024-05-03 14:37:59.958442 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1819 2024-05-03 14:37:59.962155 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     2023 2024-05-03 17:25:00.697813 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1533 2024-05-03 14:37:59.964464 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-05-03 14:37:59.958165 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-05-03 14:37:59.962327 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0     1179 2024-05-03 14:37:59.959877 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/model.py
--rw-r--r--   0        0        0     1368 2024-05-03 14:37:59.969102 patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.992497 patent_client-5.0.6/patent_client/_sync/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5742 2024-05-03 17:25:00.698709 patent_client-5.0.6/patent_client/_sync/epo/ops/published/api.py
--rw-r--r--   0        0        0     2878 2024-05-03 14:38:49.865496 patent_client-5.0.6/patent_client/_sync/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1917 2024-05-03 14:37:59.994962 patent_client-5.0.6/patent_client/_sync/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-05-03 14:38:00.067428 patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-05-03 18:09:35.996425 patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-05-03 14:38:00.065518 patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-05-03 14:38:00.066050 patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-05-03 18:09:35.999837 patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-05-03 18:09:36.013031 patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3494 2024-05-03 17:25:00.708409 patent_client-5.0.6/patent_client/_sync/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2383 2024-05-03 14:38:49.482564 patent_client-5.0.6/patent_client/_sync/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      737 2024-05-03 14:38:00.052292 patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-03 14:38:00.056955 patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1466 2024-05-03 14:38:00.064527 patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2470 2024-05-03 17:25:00.709798 patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/images.py
--rw-r--r--   0        0        0     1259 2024-05-03 14:38:00.062374 patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      701 2024-05-03 14:38:00.038716 patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     4350 2024-05-03 17:25:00.710088 patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0     1290 2024-05-03 14:38:00.051413 patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     2056 2024-05-03 17:25:00.710680 patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0     1066 2024-05-03 14:38:00.049481 patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3576 2024-05-03 17:25:00.710850 patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-05-03 14:38:00.015294 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-05-03 14:38:00.016283 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-05-03 14:38:00.015986 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-05-03 14:38:00.015636 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-05-03 18:09:36.184901 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-05-03 14:38:00.018038 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-05-03 18:09:36.189101 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-05-03 14:38:00.017010 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-05-03 14:38:00.014576 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-05-03 14:38:00.019341 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-05-03 14:38:00.018683 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-05-03 14:38:00.020342 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-05-03 14:38:00.020802 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-05-03 14:38:00.019616 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-05-03 14:38:00.019820 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-05-03 14:38:00.020084 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-05-03 14:38:00.019037 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-05-03 14:38:00.018326 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-05-03 14:38:00.020596 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-05-03 14:38:00.014020 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-05-03 14:38:00.016662 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-05-03 14:38:00.017639 patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3872 2024-05-03 17:25:00.711131 patent_client-5.0.6/patent_client/_sync/epo/ops/session.py
--rw-r--r--   0        0        0     3129 2024-05-03 17:25:00.711297 patent_client-5.0.6/patent_client/_sync/epo/ops/util.py
--rw-r--r--   0        0        0     3597 2024-05-03 17:25:00.711477 patent_client-5.0.6/patent_client/_sync/http_client.py
--rw-r--r--   0        0        0      616 2024-05-03 14:37:59.409428 patent_client-5.0.6/patent_client/_sync/odp.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.409653 patent_client-5.0.6/patent_client/_sync/uspto/__init__.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.581935 patent_client-5.0.6/patent_client/_sync/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2922 2024-05-03 17:25:00.711743 patent_client-5.0.6/patent_client/_sync/uspto/assignment/api.py
--rw-r--r--   0        0        0     1256 2024-05-03 17:25:00.711980 patent_client-5.0.6/patent_client/_sync/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     4011 2024-05-03 17:25:00.727612 patent_client-5.0.6/patent_client/_sync/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1565 2024-05-03 14:37:59.598773 patent_client-5.0.6/patent_client/_sync/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-05-03 14:37:59.624868 patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-05-03 14:37:59.625166 patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-05-03 14:37:59.619332 patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-05-03 14:37:59.623839 patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-05-03 14:37:59.620365 patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-05-03 14:37:59.624583 patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3766 2024-05-03 17:25:00.727803 patent_client-5.0.6/patent_client/_sync/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4209 2024-05-03 17:25:00.728069 patent_client-5.0.6/patent_client/_sync/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5904 2024-05-03 17:25:00.728286 patent_client-5.0.6/patent_client/_sync/uspto/assignment/model.py
--rw-r--r--   0        0        0     2348 2024-05-03 14:37:59.576141 patent_client-5.0.6/patent_client/_sync/uspto/assignment/model_test.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.413829 patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3549 2024-05-03 17:25:00.728508 patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1364 2024-05-03 17:25:00.729050 patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     3099 2024-05-03 17:25:00.733117 patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1923 2024-05-03 17:25:00.734640 patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1957 2024-05-03 17:25:00.734845 patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/model.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.824146 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2470 2024-05-03 17:25:00.735127 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1445 2024-05-03 17:25:00.735465 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-05-03 14:37:59.824012 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     2132 2024-05-03 17:25:00.811902 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7139 2024-05-03 17:25:00.812171 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3741 2024-05-03 17:25:00.812685 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6447 2024-05-03 17:25:00.812855 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5668 2024-05-03 14:37:59.814658 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-05-03 14:37:59.843238 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-05-03 14:37:59.843827 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-05-03 14:37:59.844147 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-05-03 14:37:59.843618 patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      417 2024-05-03 14:37:59.650663 patent_client-5.0.6/patent_client/_sync/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5546 2024-05-03 17:25:00.813039 patent_client-5.0.6/patent_client/_sync/uspto/odp/api.py
--rw-r--r--   0        0        0     2871 2024-05-03 17:25:00.813171 patent_client-5.0.6/patent_client/_sync/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-05-03 14:37:59.705978 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-05-03 14:37:59.707466 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-05-03 14:37:59.705680 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-05-03 14:37:59.706997 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-05-03 14:37:59.705491 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-05-03 14:37:59.704809 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-05-03 14:37:59.706290 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-05-03 14:37:59.707699 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-05-03 14:37:59.704983 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-05-03 14:37:59.705315 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-05-03 14:37:59.706607 patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     4979 2024-05-03 17:25:00.836567 patent_client-5.0.6/patent_client/_sync/uspto/odp/manager.py
--rw-r--r--   0        0        0     2003 2024-05-03 17:25:00.836840 patent_client-5.0.6/patent_client/_sync/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16273 2024-05-03 17:25:00.837155 patent_client-5.0.6/patent_client/_sync/uspto/odp/model.py
--rw-r--r--   0        0        0    12549 2024-05-03 17:25:00.837446 patent_client-5.0.6/patent_client/_sync/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2812 2024-05-03 14:37:59.649159 patent_client-5.0.6/patent_client/_sync/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-05-03 14:37:59.650478 patent_client-5.0.6/patent_client/_sync/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      891 2024-05-03 14:37:59.650234 patent_client-5.0.6/patent_client/_sync/uspto/odp/util.py
--rw-r--r--   0        0        0      548 2024-05-03 14:37:59.731670 patent_client-5.0.6/patent_client/_sync/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4838 2024-05-03 14:37:59.761494 patent_client-5.0.6/patent_client/_sync/uspto/peds/api.py
--rw-r--r--   0        0        0      986 2024-05-03 17:25:00.837929 patent_client-5.0.6/patent_client/_sync/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-05-03 14:37:59.800574 patent_client-5.0.6/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0     8619 2024-05-03 17:25:00.859149 patent_client-5.0.6/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8510 2024-05-03 17:25:00.859457 patent_client-5.0.6/patent_client/_sync/uspto/peds/manager.py
--rw-r--r--   0        0        0     9245 2024-05-03 17:25:00.859815 patent_client-5.0.6/patent_client/_sync/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    15280 2024-05-03 17:25:00.860150 patent_client-5.0.6/patent_client/_sync/uspto/peds/model.py
--rw-r--r--   0        0        0     6532 2024-05-03 14:37:59.731254 patent_client-5.0.6/patent_client/_sync/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-05-03 14:37:59.722594 patent_client-5.0.6/patent_client/_sync/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      604 2024-05-03 14:37:59.905537 patent_client-5.0.6/patent_client/_sync/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10513 2024-05-03 17:25:00.860352 patent_client-5.0.6/patent_client/_sync/uspto/ptab/api.py
--rw-r--r--   0        0        0      992 2024-05-03 17:25:00.860619 patent_client-5.0.6/patent_client/_sync/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-05-03 14:37:59.945524 patent_client-5.0.6/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-05-03 14:37:59.946098 patent_client-5.0.6/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2407 2024-05-03 17:25:00.864640 patent_client-5.0.6/patent_client/_sync/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2270 2024-05-03 17:25:00.864929 patent_client-5.0.6/patent_client/_sync/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8786 2024-05-03 17:25:00.865122 patent_client-5.0.6/patent_client/_sync/uspto/ptab/model.py
--rw-r--r--   0        0        0      658 2024-05-03 14:37:59.905006 patent_client-5.0.6/patent_client/_sync/uspto/ptab/util.py
--rw-r--r--   0        0        0      742 2024-05-03 14:37:59.464708 patent_client-5.0.6/patent_client/_sync/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     7172 2024-05-03 17:25:00.865428 patent_client-5.0.6/patent_client/_sync/uspto/public_search/api.py
--rw-r--r--   0        0        0      667 2024-05-03 17:25:00.865650 patent_client-5.0.6/patent_client/_sync/uspto/public_search/api_test.py
--rw-r--r--   0        0        0      416 2024-05-03 14:37:59.551065 patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2482 2024-05-03 14:37:59.554323 patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6964 2024-05-03 17:25:00.869269 patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     2010 2024-05-03 14:37:59.556752 patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1451 2024-05-03 14:37:59.477738 patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-05-03 14:37:59.463915 patent_client-5.0.6/patent_client/_sync/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-05-03 14:37:59.548153 patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-05-03 14:37:59.548647 patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-05-03 14:37:59.550751 patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-05-03 14:37:59.550202 patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-05-03 18:09:38.458612 patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-05-03 14:37:59.532547 patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4475 2024-05-03 17:25:00.870930 patent_client-5.0.6/patent_client/_sync/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7113 2024-05-03 17:25:00.871148 patent_client-5.0.6/patent_client/_sync/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      970 2024-05-03 17:25:00.872488 patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3495 2024-05-03 17:25:00.872682 patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7978 2024-05-03 17:25:00.872888 patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2659 2024-05-03 17:25:00.873059 patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1951 2024-05-03 14:37:59.449288 patent_client-5.0.6/patent_client/_sync/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4914 2024-05-03 17:25:00.873295 patent_client-5.0.6/patent_client/_sync/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-05-03 14:37:59.434686 patent_client-5.0.6/patent_client/_sync/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4472 2024-05-03 17:25:00.873509 patent_client-5.0.6/patent_client/_sync/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-05-03 14:37:59.484812 patent_client-5.0.6/patent_client/_sync/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      689 2024-05-03 14:37:59.463571 patent_client-5.0.6/patent_client/_sync/uspto/public_search/util.py
--rw-r--r--   0        0        0      121 2024-05-03 17:27:31.159772 patent_client-5.0.6/patent_client/odp.py
--rw-r--r--   0        0        0     6027 2024-05-03 17:25:00.874498 patent_client-5.0.6/patent_client/parser.py
--rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.6/patent_client/patches.py
--rw-r--r--   0        0        0     3262 2024-05-03 17:25:00.874850 patent_client-5.0.6/patent_client/session.py
--rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.6/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.6/patent_client/test_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.6/patent_client/util/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.6/patent_client/util/asyncio_util.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.6/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4313 2024-05-03 18:09:39.367651 patent_client-5.0.6/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.6/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6924 2024-05-03 18:09:39.370382 patent_client-5.0.6/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.6/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.6/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3522 2024-05-03 17:25:00.875271 patent_client-5.0.6/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.6/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.6/patent_client/util/format.py
--rw-r--r--   0        0        0     9700 2024-05-03 17:25:00.875510 patent_client-5.0.6/patent_client/util/manager.py
--rw-r--r--   0        0        0     3062 2024-05-03 17:25:00.875751 patent_client-5.0.6/patent_client/util/pydantic_util.py
--rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.6/patent_client/util/request_util.py
--rw-r--r--   0        0        0     1233 2024-05-03 17:25:00.876102 patent_client-5.0.6/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2024-05-03 18:17:31.998649 patent_client-5.0.6/patent_client/version.py
--rw-r--r--   0        0        0     3407 2024-05-03 18:17:31.999031 patent_client-5.0.6/pyproject.toml
--rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.7/LICENSE
+-rw-r--r--   0        0        0     6283 2024-05-02 17:06:23.093538 patent_client-5.0.7/README.md
+-rw-r--r--   0        0        0     1739 2024-05-03 17:25:00.646245 patent_client-5.0.7/patent_client/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-02 17:06:23.121290 patent_client-5.0.7/patent_client/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.7/patent_client/_async/epo/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.7/patent_client/_async/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.7/patent_client/_async/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-03 17:25:00.646675 patent_client-5.0.7/patent_client/_async/epo/ops/family/api.py
+-rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.7/patent_client/_async/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      356 2024-05-03 17:25:00.646963 patent_client-5.0.7/patent_client/_async/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.7/patent_client/_async/epo/ops/family/model.py
+-rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.7/patent_client/_async/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1503 2024-05-03 17:25:00.647248 patent_client-5.0.7/patent_client/_async/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.7/patent_client/_async/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.7/patent_client/_async/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 17:06:23.121738 patent_client-5.0.7/patent_client/_async/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.7/patent_client/_async/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      467 2024-05-03 17:25:00.653744 patent_client-5.0.7/patent_client/_async/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.7/patent_client/_async/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5434 2024-05-03 17:25:00.657228 patent_client-5.0.7/patent_client/_async/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.7/patent_client/_async/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4018 2024-05-03 17:25:00.661652 patent_client-5.0.7/patent_client/_async/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.7/patent_client/_async/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.7/patent_client/_async/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1415 2024-05-02 17:06:23.125551 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.7/patent_client/_async/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.7/patent_client/_async/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5472 2024-05-03 17:25:00.661893 patent_client-5.0.7/patent_client/_async/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2699 2024-05-03 17:25:00.662175 patent_client-5.0.7/patent_client/_async/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.7/patent_client/_async/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-03 18:55:44.783861 patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-03 18:55:44.787852 patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-03 18:55:44.797470 patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3204 2024-05-03 17:25:00.662696 patent_client-5.0.7/patent_client/_async/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2411 2024-05-03 17:25:00.662959 patent_client-5.0.7/patent_client/_async/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.7/patent_client/_async/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.7/patent_client/_async/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.7/patent_client/_async/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2078 2024-05-03 17:25:00.663177 patent_client-5.0.7/patent_client/_async/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.7/patent_client/_async/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3934 2024-05-03 17:25:00.663421 patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1640 2024-05-03 17:25:00.664113 patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3160 2024-05-03 17:25:00.664661 patent_client-5.0.7/patent_client/_async/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-03 18:55:44.929497 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-03 18:55:44.933520 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.7/patent_client/_async/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3478 2024-05-03 17:25:00.664935 patent_client-5.0.7/patent_client/_async/epo/ops/session.py
+-rw-r--r--   0        0        0     2881 2024-05-03 17:25:00.665195 patent_client-5.0.7/patent_client/_async/epo/ops/util.py
+-rw-r--r--   0        0        0     3220 2024-05-03 17:25:00.665599 patent_client-5.0.7/patent_client/_async/http_client.py
+-rw-r--r--   0        0        0      201 2024-05-02 17:06:23.136948 patent_client-5.0.7/patent_client/_async/odp.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.7/patent_client/_async/uspto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.7/patent_client/_async/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-03 17:25:00.665812 patent_client-5.0.7/patent_client/_async/uspto/assignment/api.py
+-rw-r--r--   0        0        0      921 2024-05-02 17:06:23.137157 patent_client-5.0.7/patent_client/_async/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     3595 2024-05-03 17:25:00.666143 patent_client-5.0.7/patent_client/_async/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.7/patent_client/_async/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3424 2024-05-03 17:25:00.666449 patent_client-5.0.7/patent_client/_async/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4158 2024-05-03 17:25:00.666715 patent_client-5.0.7/patent_client/_async/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5500 2024-05-03 17:25:00.666971 patent_client-5.0.7/patent_client/_async/uspto/assignment/model.py
+-rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.7/patent_client/_async/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.7/patent_client/_async/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3182 2024-05-03 17:25:00.667431 patent_client-5.0.7/patent_client/_async/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.7/patent_client/_async/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.7/patent_client/_async/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.7/patent_client/_async/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1553 2024-05-03 17:25:00.667735 patent_client-5.0.7/patent_client/_async/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1762 2024-05-03 17:25:00.667994 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     6897 2024-05-03 17:25:00.668558 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6031 2024-05-03 17:25:00.668826 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.7/patent_client/_async/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     6187 2024-05-03 18:56:17.340414 patent_client-5.0.7/patent_client/_async/uspto/odp/api.py
+-rw-r--r--   0        0        0     2818 2024-05-03 17:25:00.669417 patent_client-5.0.7/patent_client/_async/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5815 2024-05-03 18:56:17.114385 patent_client-5.0.7/patent_client/_async/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2127 2024-05-03 18:56:17.339737 patent_client-5.0.7/patent_client/_async/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    19339 2024-05-03 18:56:17.342376 patent_client-5.0.7/patent_client/_async/uspto/odp/model.py
+-rw-r--r--   0        0        0    12133 2024-05-03 17:25:00.670224 patent_client-5.0.7/patent_client/_async/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.7/patent_client/_async/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.7/patent_client/_async/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.7/patent_client/_async/uspto/odp/util.py
+-rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.7/patent_client/_async/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.7/patent_client/_async/uspto/peds/api.py
+-rw-r--r--   0        0        0      683 2024-05-03 17:25:00.670577 patent_client-5.0.7/patent_client/_async/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.7/patent_client/_async/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8619 2024-05-03 17:25:00.673086 patent_client-5.0.7/patent_client/_async/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8191 2024-05-03 17:25:00.673373 patent_client-5.0.7/patent_client/_async/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9623 2024-05-03 17:25:00.673653 patent_client-5.0.7/patent_client/_async/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    14958 2024-05-03 17:25:00.673984 patent_client-5.0.7/patent_client/_async/uspto/peds/model.py
+-rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.7/patent_client/_async/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.7/patent_client/_async/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      188 2024-05-02 17:06:23.210126 patent_client-5.0.7/patent_client/_async/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10134 2024-05-03 17:25:00.674181 patent_client-5.0.7/patent_client/_async/uspto/ptab/api.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.7/patent_client/_async/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.7/patent_client/_async/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.7/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2025 2024-05-03 17:25:00.674454 patent_client-5.0.7/patent_client/_async/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2249 2024-05-03 17:25:00.674630 patent_client-5.0.7/patent_client/_async/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8382 2024-05-03 17:25:00.674990 patent_client-5.0.7/patent_client/_async/uspto/ptab/model.py
+-rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.7/patent_client/_async/uspto/ptab/util.py
+-rw-r--r--   0        0        0      326 2024-05-02 17:06:23.210541 patent_client-5.0.7/patent_client/_async/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6921 2024-05-03 17:25:00.675209 patent_client-5.0.7/patent_client/_async/uspto/public_search/api.py
+-rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.7/patent_client/_async/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6548 2024-05-03 17:25:00.680068 patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1035 2024-05-02 17:06:23.211161 patent_client-5.0.7/patent_client/_async/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.7/patent_client/_async/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-03 18:55:47.207946 patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4132 2024-05-03 17:25:00.680395 patent_client-5.0.7/patent_client/_async/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7627 2024-05-03 17:25:00.680977 patent_client-5.0.7/patent_client/_async/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      554 2024-05-03 17:25:00.681546 patent_client-5.0.7/patent_client/_async/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3091 2024-05-03 17:25:00.681713 patent_client-5.0.7/patent_client/_async/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7574 2024-05-03 17:25:00.681893 patent_client-5.0.7/patent_client/_async/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2243 2024-05-03 17:25:00.682051 patent_client-5.0.7/patent_client/_async/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1535 2024-05-02 17:06:23.211470 patent_client-5.0.7/patent_client/_async/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4498 2024-05-03 17:25:00.682225 patent_client-5.0.7/patent_client/_async/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.7/patent_client/_async/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4056 2024-05-03 17:25:00.682391 patent_client-5.0.7/patent_client/_async/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.7/patent_client/_async/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.7/patent_client/_async/uspto/public_search/util.py
+-rw-r--r--   0        0        0     1249 2024-05-03 18:55:38.645407 patent_client-5.0.7/patent_client/_sync/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:39.217348 patent_client-5.0.7/patent_client/_sync/epo/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-03 18:55:39.229624 patent_client-5.0.7/patent_client/_sync/epo/ops/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:39.247425 patent_client-5.0.7/patent_client/_sync/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-03 18:55:39.250439 patent_client-5.0.7/patent_client/_sync/epo/ops/family/api.py
+-rw-r--r--   0        0        0      839 2024-05-03 18:56:17.798698 patent_client-5.0.7/patent_client/_sync/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-05-03 18:55:39.258069 patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-05-03 18:55:39.258453 patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-05-03 18:55:39.259339 patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-05-03 18:55:39.258977 patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      750 2024-05-03 18:55:39.252715 patent_client-5.0.7/patent_client/_sync/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1535 2024-05-03 18:55:39.249567 patent_client-5.0.7/patent_client/_sync/epo/ops/family/model.py
+-rw-r--r--   0        0        0      887 2024-05-03 18:56:17.787448 patent_client-5.0.7/patent_client/_sync/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1919 2024-05-03 18:55:39.255396 patent_client-5.0.7/patent_client/_sync/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      943 2024-05-03 18:55:39.247094 patent_client-5.0.7/patent_client/_sync/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:39.355070 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-03 18:55:39.359952 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      688 2024-05-03 18:56:17.793887 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-05-03 18:55:39.392347 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-05-03 18:55:39.390681 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-05-03 18:55:39.391971 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-05-03 18:55:39.391012 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-05-03 18:55:39.391276 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-05-03 18:55:39.391614 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-05-03 18:55:39.389223 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      847 2024-05-03 18:56:17.341267 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2791 2024-05-03 18:55:39.359139 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5767 2024-05-03 18:56:17.316036 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      866 2024-05-03 18:56:17.778728 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4434 2024-05-03 18:55:39.377641 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1632 2024-05-03 18:55:39.354149 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      530 2024-05-03 18:55:39.354936 patent_client-5.0.7/patent_client/_sync/epo/ops/legal/util.py
+-rw-r--r--   0        0        0      483 2024-05-03 18:55:39.230469 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1819 2024-05-03 18:55:39.234716 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     2023 2024-05-03 18:56:17.339715 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1533 2024-05-03 18:55:39.237165 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-05-03 18:55:39.230019 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-05-03 18:55:39.234995 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0     1179 2024-05-03 18:55:39.232253 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0     1368 2024-05-03 18:55:39.242048 patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:39.269246 patent_client-5.0.7/patent_client/_sync/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5742 2024-05-03 18:56:17.340709 patent_client-5.0.7/patent_client/_sync/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2878 2024-05-03 18:56:17.791142 patent_client-5.0.7/patent_client/_sync/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1917 2024-05-03 18:55:39.271947 patent_client-5.0.7/patent_client/_sync/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-05-03 18:55:39.350532 patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-03 18:56:04.464409 patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-05-03 18:55:39.349424 patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-05-03 18:55:39.349742 patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-03 18:56:04.467054 patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-03 18:56:04.477247 patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3494 2024-05-03 18:55:39.292003 patent_client-5.0.7/patent_client/_sync/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2383 2024-05-03 18:56:17.339040 patent_client-5.0.7/patent_client/_sync/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      737 2024-05-03 18:55:39.335622 patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-03 18:55:39.340791 patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1466 2024-05-03 18:55:39.348736 patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2470 2024-05-03 18:55:39.344623 patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0     1259 2024-05-03 18:55:39.346545 patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      701 2024-05-03 18:55:39.321277 patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     4350 2024-05-03 18:55:39.327776 patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0     1290 2024-05-03 18:55:39.334608 patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     2056 2024-05-03 18:55:39.330891 patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0     1066 2024-05-03 18:55:39.332571 patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3576 2024-05-03 18:55:39.269096 patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-05-03 18:55:39.293921 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-05-03 18:55:39.294925 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-05-03 18:55:39.294591 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-05-03 18:55:39.294213 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-03 18:56:04.603703 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-05-03 18:55:39.296463 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-03 18:56:04.607357 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-05-03 18:55:39.295452 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-05-03 18:55:39.292900 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-05-03 18:55:39.297963 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-05-03 18:55:39.297352 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-05-03 18:55:39.299617 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-05-03 18:55:39.300196 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-05-03 18:55:39.298483 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-05-03 18:55:39.298781 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-05-03 18:55:39.299332 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-05-03 18:55:39.297634 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-05-03 18:55:39.297035 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-05-03 18:55:39.299913 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-05-03 18:55:39.292530 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-05-03 18:55:39.295160 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-05-03 18:55:39.296184 patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3872 2024-05-03 18:55:39.228790 patent_client-5.0.7/patent_client/_sync/epo/ops/session.py
+-rw-r--r--   0        0        0     3129 2024-05-03 18:56:17.781401 patent_client-5.0.7/patent_client/_sync/epo/ops/util.py
+-rw-r--r--   0        0        0     3597 2024-05-03 18:55:38.642913 patent_client-5.0.7/patent_client/_sync/http_client.py
+-rw-r--r--   0        0        0      616 2024-05-03 18:55:38.646112 patent_client-5.0.7/patent_client/_sync/odp.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:38.646506 patent_client-5.0.7/patent_client/_sync/uspto/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:38.833128 patent_client-5.0.7/patent_client/_sync/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2922 2024-05-03 18:55:38.846143 patent_client-5.0.7/patent_client/_sync/uspto/assignment/api.py
+-rw-r--r--   0        0        0     1256 2024-05-03 18:56:17.800048 patent_client-5.0.7/patent_client/_sync/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     4011 2024-05-03 18:55:38.832819 patent_client-5.0.7/patent_client/_sync/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1565 2024-05-03 18:55:38.850208 patent_client-5.0.7/patent_client/_sync/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-05-03 18:55:38.870958 patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-05-03 18:55:38.872668 patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-05-03 18:55:38.867274 patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-05-03 18:55:38.868481 patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-05-03 18:55:38.868133 patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-05-03 18:55:38.869218 patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3766 2024-05-03 18:56:17.341256 patent_client-5.0.7/patent_client/_sync/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4209 2024-05-03 18:56:17.799568 patent_client-5.0.7/patent_client/_sync/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5904 2024-05-03 18:55:38.841873 patent_client-5.0.7/patent_client/_sync/uspto/assignment/model.py
+-rw-r--r--   0        0        0     2348 2024-05-03 18:55:38.827018 patent_client-5.0.7/patent_client/_sync/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:38.651016 patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-03 18:55:38.660165 patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1364 2024-05-03 18:56:17.338890 patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     3099 2024-05-03 18:56:17.339484 patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1923 2024-05-03 18:56:17.802782 patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1957 2024-05-03 18:55:38.654176 patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:39.091728 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2470 2024-05-03 18:56:17.339457 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1445 2024-05-03 18:56:17.797425 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-05-03 18:55:39.091552 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     2132 2024-05-03 18:55:39.111687 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7139 2024-05-03 18:56:17.770887 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3741 2024-05-03 18:56:17.340704 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6447 2024-05-03 18:55:39.090928 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5668 2024-05-03 18:55:39.081470 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-05-03 18:55:39.112053 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-05-03 18:55:39.112742 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-05-03 18:55:39.113020 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-05-03 18:55:39.112363 patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      417 2024-05-03 18:55:38.899923 patent_client-5.0.7/patent_client/_sync/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     6449 2024-05-03 18:56:17.340530 patent_client-5.0.7/patent_client/_sync/uspto/odp/api.py
+-rw-r--r--   0        0        0     2871 2024-05-03 18:56:17.338589 patent_client-5.0.7/patent_client/_sync/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-05-03 18:55:38.963394 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-05-03 18:55:38.964869 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-05-03 18:55:38.963108 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-05-03 18:55:38.964432 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-05-03 18:55:38.962430 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-05-03 18:55:38.961148 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-05-03 18:55:38.963708 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-05-03 18:55:38.968240 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-05-03 18:55:38.961500 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-05-03 18:55:38.961856 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-05-03 18:55:38.964022 patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5953 2024-05-03 18:56:17.341024 patent_client-5.0.7/patent_client/_sync/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2169 2024-05-03 18:56:17.341236 patent_client-5.0.7/patent_client/_sync/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    19521 2024-05-03 18:56:17.774912 patent_client-5.0.7/patent_client/_sync/uspto/odp/model.py
+-rw-r--r--   0        0        0    12549 2024-05-03 18:55:38.894164 patent_client-5.0.7/patent_client/_sync/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2812 2024-05-03 18:55:38.898375 patent_client-5.0.7/patent_client/_sync/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-05-03 18:55:38.899750 patent_client-5.0.7/patent_client/_sync/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      891 2024-05-03 18:55:38.899373 patent_client-5.0.7/patent_client/_sync/uspto/odp/util.py
+-rw-r--r--   0        0        0      548 2024-05-03 18:55:38.994234 patent_client-5.0.7/patent_client/_sync/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4838 2024-05-03 18:55:39.026922 patent_client-5.0.7/patent_client/_sync/uspto/peds/api.py
+-rw-r--r--   0        0        0      986 2024-05-03 18:56:17.338786 patent_client-5.0.7/patent_client/_sync/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-05-03 18:55:39.066051 patent_client-5.0.7/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8619 2024-05-03 18:55:39.065670 patent_client-5.0.7/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8510 2024-05-03 18:55:39.042417 patent_client-5.0.7/patent_client/_sync/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9245 2024-05-03 18:56:17.340538 patent_client-5.0.7/patent_client/_sync/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    15280 2024-05-03 18:56:17.777671 patent_client-5.0.7/patent_client/_sync/uspto/peds/model.py
+-rw-r--r--   0        0        0     6532 2024-05-03 18:55:38.993102 patent_client-5.0.7/patent_client/_sync/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-05-03 18:55:38.983304 patent_client-5.0.7/patent_client/_sync/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      604 2024-05-03 18:55:39.176656 patent_client-5.0.7/patent_client/_sync/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10513 2024-05-03 18:55:39.203917 patent_client-5.0.7/patent_client/_sync/uspto/ptab/api.py
+-rw-r--r--   0        0        0      992 2024-05-03 18:56:17.338580 patent_client-5.0.7/patent_client/_sync/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-05-03 18:55:39.216399 patent_client-5.0.7/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-05-03 18:55:39.217157 patent_client-5.0.7/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2407 2024-05-03 18:55:39.209281 patent_client-5.0.7/patent_client/_sync/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2270 2024-05-03 18:56:17.340015 patent_client-5.0.7/patent_client/_sync/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8786 2024-05-03 18:55:39.189369 patent_client-5.0.7/patent_client/_sync/uspto/ptab/model.py
+-rw-r--r--   0        0        0      658 2024-05-03 18:55:39.175684 patent_client-5.0.7/patent_client/_sync/uspto/ptab/util.py
+-rw-r--r--   0        0        0      742 2024-05-03 18:55:38.704897 patent_client-5.0.7/patent_client/_sync/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     7172 2024-05-03 18:55:38.715374 patent_client-5.0.7/patent_client/_sync/uspto/public_search/api.py
+-rw-r--r--   0        0        0      667 2024-05-03 18:56:17.338782 patent_client-5.0.7/patent_client/_sync/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0      416 2024-05-03 18:55:38.795740 patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-03 18:55:38.804995 patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6964 2024-05-03 18:55:38.817988 patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     2010 2024-05-03 18:55:38.807714 patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1451 2024-05-03 18:55:38.718716 patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-05-03 18:55:38.703982 patent_client-5.0.7/patent_client/_sync/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-05-03 18:55:38.792178 patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-05-03 18:55:38.792693 patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-05-03 18:55:38.795525 patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-05-03 18:55:38.795017 patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-03 18:56:06.832606 patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-05-03 18:55:38.774281 patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4475 2024-05-03 18:56:17.804571 patent_client-5.0.7/patent_client/_sync/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7113 2024-05-03 18:56:17.338935 patent_client-5.0.7/patent_client/_sync/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      970 2024-05-03 18:55:38.749837 patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3495 2024-05-03 18:55:38.755496 patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7978 2024-05-03 18:55:38.771613 patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2659 2024-05-03 18:55:38.759470 patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1951 2024-05-03 18:55:38.688529 patent_client-5.0.7/patent_client/_sync/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4914 2024-05-03 18:55:38.702399 patent_client-5.0.7/patent_client/_sync/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-05-03 18:55:38.673080 patent_client-5.0.7/patent_client/_sync/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4472 2024-05-03 18:55:38.695269 patent_client-5.0.7/patent_client/_sync/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-05-03 18:55:38.726165 patent_client-5.0.7/patent_client/_sync/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      689 2024-05-03 18:55:38.703364 patent_client-5.0.7/patent_client/_sync/uspto/public_search/util.py
+-rw-r--r--   0        0        0      121 2024-05-03 17:27:31.159772 patent_client-5.0.7/patent_client/odp.py
+-rw-r--r--   0        0        0     6027 2024-05-03 17:25:00.874498 patent_client-5.0.7/patent_client/parser.py
+-rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.7/patent_client/patches.py
+-rw-r--r--   0        0        0     3262 2024-05-03 17:25:00.874850 patent_client-5.0.7/patent_client/session.py
+-rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.7/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.7/patent_client/test_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.7/patent_client/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.7/patent_client/util/asyncio_util.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.7/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4313 2024-05-03 18:56:07.743234 patent_client-5.0.7/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.7/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6924 2024-05-03 18:56:07.746481 patent_client-5.0.7/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.7/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      735 2024-05-02 17:06:23.356360 patent_client-5.0.7/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3522 2024-05-03 17:25:00.875271 patent_client-5.0.7/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.7/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.7/patent_client/util/format.py
+-rw-r--r--   0        0        0     9700 2024-05-03 17:25:00.875510 patent_client-5.0.7/patent_client/util/manager.py
+-rw-r--r--   0        0        0     3062 2024-05-03 17:25:00.875751 patent_client-5.0.7/patent_client/util/pydantic_util.py
+-rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.7/patent_client/util/request_util.py
+-rw-r--r--   0        0        0     1233 2024-05-03 17:25:00.876102 patent_client-5.0.7/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2024-05-03 18:56:30.007919 patent_client-5.0.7/patent_client/version.py
+-rw-r--r--   0        0        0     3407 2024-05-03 18:56:30.008392 patent_client-5.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.7/PKG-INFO
```

### Comparing `patent_client-5.0.6/LICENSE` & `patent_client-5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/README.md` & `patent_client-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/__init__.py` & `patent_client-5.0.7/patent_client/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/__init__.py` & `patent_client-5.0.7/patent_client/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/model.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/model_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/schema.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/family/schema_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/model.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/national_codes.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/national_codes.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/schema.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/legal/schema_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/api.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/api_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/errors.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/errors.txt` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/messages.txt` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/model.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/number_service/schema.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/api.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/api_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/cql.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/manager.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/manager_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/model/biblio.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/model/fulltext.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/model/images.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/model/search.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/biblio.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/images.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/schema/search.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/schema_test.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/description_example.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/image_example.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/published/test/search_example.xml` & `patent_client-5.0.7/patent_client/_async/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/session.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/epo/ops/util.py` & `patent_client-5.0.7/patent_client/_async/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/http_client.py` & `patent_client-5.0.7/patent_client/_async/http_client.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/api_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/convert.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/convert_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/manager_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/model.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/assignment/model_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/bulk_data/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/bulk_data/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/bulk_data/api_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/bulk_data/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/bulk_data/manager_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/bulk_data/model.py` & `patent_client-5.0.7/patent_client/_async/uspto/bulk_data/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/api_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/model.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/model_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/query.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/query_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/app.json` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.7/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as tp
+from urllib.parse import quote
 
 from patent_client import SETTINGS
 
 from ...http_client import PatentClientSession
 from .model import (
     Assignment,
     Continuity,
@@ -15,14 +16,18 @@
     Transaction,
     USApplication,
     USApplicationBiblio,
 )
 from .util import prune
 
 
+def urlescape(s: str) -> str:
+    return quote(s, safe="")
+
+
 class ODPApi:
     base_url = "https://beta-api.uspto.gov"
 
     def __init__(self):
         if SETTINGS.odp_api_key is None:
             raise ValueError("ODP API key is not set")
         self.client = PatentClientSession(headers={"X-API-KEY": SETTINGS.odp_api_key})
@@ -57,74 +62,82 @@
         response.raise_for_status()
         return response.json()
 
     # Data Attributes
 
     async def get_application_data(self, application_id: str) -> USApplication:
         """Patent application data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}"
         response = await self.client.get(url)
         response.raise_for_status()
         return USApplication(**response.json()["patentBag"][0])
 
     async def get_application_biblio_data(self, application_id: str) -> USApplicationBiblio:
         """Patent application basic data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/application-data"
+        url = (
+            self.base_url
+            + f"/api/v1/patent/applications/{urlescape(application_id)}/application-data"
+        )
         response = await self.client.get(url)
         response.raise_for_status()
         return USApplicationBiblio(**response.json()["patentBag"][0])
 
     async def get_patent_term_adjustment_data(self, application_id: str) -> TermAdjustment:
         """Patent application term adjustment data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/adjustment"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/adjustment"
         response = await self.client.get(url)
         response.raise_for_status()
         return TermAdjustment(**response.json()["patentBag"][0]["patentTermAdjustmentData"])
 
     async def get_assignments(self, application_id: str) -> tp.List[Assignment]:
         """Patent application term adjustment data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/assignment"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/assignment"
         response = await self.client.get(url)
         response.raise_for_status()
         data = response.json()["patentBag"][0]["assignmentBag"]
         return [Assignment(**assignment) for assignment in data]
 
     async def get_attorney_data(self, application_id: str) -> CustomerNumber:
         """Patent application attorney data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/attorney"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/attorney"
         response = await self.client.get(url)
         response.raise_for_status()
         return CustomerNumber(**response.json()["patentBag"][0]["recordAttorney"])
 
     async def get_continuity_data(self, application_id: str) -> Continuity:
         """Patent application continuity data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/continuity"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/continuity"
         response = await self.client.get(url)
         response.raise_for_status()
         return Continuity(**response.json())
 
     async def get_foreign_priority_data(self, application_id: str) -> tp.List[ForeignPriority]:
         """Patent application foreign priority data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/foreign-priority"
+        url = (
+            self.base_url
+            + f"/api/v1/patent/applications/{urlescape(application_id)}/foreign-priority"
+        )
         response = await self.client.get(url)
         response.raise_for_status()
         return [
             ForeignPriority(**foreign_priority)
             for foreign_priority in response.json()["patentBag"][0]["foreignPriorityBag"]
         ]
 
     async def get_transactions(self, application_id: str) -> tp.List[Transaction]:
         """Patent application transactions by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/transactions"
+        url = (
+            self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/transactions"
+        )
         response = await self.client.get(url)
         response.raise_for_status()
         return [
             Transaction(**transaction)
             for transaction in response.json()["patentBag"][0]["transactionContentBag"]
         ]
 
     async def get_documents(self, application_id: str) -> tp.List[Document]:
         """Patent application documents by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/documents"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/documents"
         response = await self.client.get(url)
         response.raise_for_status()
         return [Document(**document) for document in response.json()["documentBag"]]
```

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/api_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/application.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/documents.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/search.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.7/patent_client/_async/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,19 @@
         if "query" in self.config.filter:
             return SearchRequest(**self.config.filter["query"][0], fields=fields)
         elif "q" in self.config.filter:
             return SearchRequest(q=self.config.filter["q"][0], fields=fields)
         else:
             return create_post_search_obj(self.config, fields=fields)
 
+    async def get(self, *args, **kwargs):
+        if len(args) == 1 and not kwargs:
+            return await api.get_application_data(args[0])
+        return await super().get(*args, **kwargs)
+
 
 class USApplicationBiblioManager(USApplicationManager):
     default_filter = "appl_id"
     default_fields = [
         "firstInventorToFileIndicator",
         "filingDate",
         "inventorBag",
@@ -83,14 +88,19 @@
         for start, rows in get_start_and_row_count(self.config.limit):
             page_query = query_obj.model_dump()
             page_query["pagination"] = {"offset": start, "limit": rows}
             page_query_obj = SearchRequest(**page_query)
             for result in (await api.post_search(page_query_obj))["patentBag"]:
                 yield self.response_model(**result)
 
+    async def get(self, *args, **kwargs):
+        if len(args) == 1 and not kwargs:
+            return await api.get_application_biblio_data(args[0])
+        return await super().get(*args, **kwargs)
+
 
 class AttributeManager(AsyncManager):
     def filter(self, *args, **kwargs):
         raise NotImplementedError("Filtering attributes is not supported")
 
     def get(self, *args, **kwargs):
         raise NotImplementedError("Getting attributes is not supported")
```

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/manager_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,7 +58,13 @@
 
 @pytest.mark.asyncio
 async def test_can_get_old_applications():
     result = await USApplication.objects.get("14230558")
     assert result.appl_id == "14230558"
     result = await USApplicationBiblio.objects.get("14230558")
     assert result.appl_id == "14230558"
+
+
+@pytest.mark.asyncio
+async def test_can_get_pct_application():
+    result = await USApplication.objects.get("PCT/US07/19317")
+    assert result.appl_id == "PCT/US07/19317"
```

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/model.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,53 +33,59 @@
     correspondent_name_text: Optional[str] = Field(alias="correspondentNameText", default=None)
 
 
 # Continuity
 
 
 class Relationship(BaseODPModel):
-    application_status_code: int = Field()
-    claim_type_code: str = Field(alias="claimParentageTypeCode")
-    filing_date: datetime.date
-    application_status_description: str = Field(alias="applicationStatusDescriptionText")
-    claim_type_description: str = Field(alias="claimParentageTypeCodeDescription")
-    parent_application_id: str = Field(alias="parentApplicationNumberText")
-    child_application_id: str = Field(alias="childApplicationNumberText")
+    application_status_code: Optional[int] = Field(default=None)
+    claim_type_code: Optional[str] = Field(alias="claimParentageTypeCode", default=None)
+    filing_date: Optional[datetime.date] = Field(default=None)
+    application_status_description: Optional[str] = Field(
+        alias="applicationStatusDescriptionText", default=None
+    )
+    claim_type_description: Optional[str] = Field(
+        alias="claimParentageTypeCodeDescription", default=None
+    )
+    parent_application_id: Optional[str] = Field(alias="parentApplicationNumberText", default=None)
+    child_application_id: Optional[str] = Field(alias="childApplicationNumberText", default=None)
 
 
 class Continuity(BaseODPModel):
-    count: int
-    request_identifier: str
+    count: Optional[int] = Field(default=None)
+    request_identifier: Optional[str] = Field(default=None)
     parent_continuity: Optional[list[Relationship]] = Field(
         alias=AliasPath(["patentBag", 0, "continuityBag", "parentContinuityBag"]),
-        default=None,
+        default_factory=list,
     )
     child_continuity: Optional[list[Relationship]] = Field(
         alias=AliasPath(["patentBag", 0, "continuityBag", "childContinuityBag"]),
-        default=None,
+        default_factory=list,
     )
 
 
 # Documents
 
 
 class DownloadOption(BaseODPModel):
-    mime_type_identifier: str
-    download_url: str
-    pages: int = Field(alias="pageTotalQuantity")
+    mime_type_identifier: Optional[str] = Field(default=None)
+    download_url: Optional[str] = Field(default=None)
+    pages: Optional[int] = Field(alias="pageTotalQuantity", default=None)
 
 
 class Document(BaseODPModel):
-    appl_id: str = Field(alias="applicationNumberText")
-    mail_date: datetime.datetime = Field(alias="officialDate")
-    document_identifier: str = Field(alias="documentIdentifier")
-    document_code: str = Field(alias="documentCode")
-    document_code_description: str = Field(alias="documentCodeDescriptionText")
-    direction_category: str = Field(alias="directionCategory")
-    download_option_bag: list[dict] = Field(alias="downloadOptionBag")
+    appl_id: Optional[str] = Field(alias="applicationNumberText", default=None)
+    mail_date: Optional[datetime.datetime] = Field(alias="officialDate", default=None)
+    document_identifier: Optional[str] = Field(alias="documentIdentifier", default=None)
+    document_code: Optional[str] = Field(alias="documentCode", default=None)
+    document_code_description: Optional[str] = Field(
+        alias="documentCodeDescriptionText", default=None
+    )
+    direction_category: Optional[str] = Field(alias="directionCategory", default=None)
+    download_option_bag: list[dict] = Field(alias="downloadOptionBag", default_factory=list)
 
     async def download(self, type="PDF", out_path=None):
         from .manager import api
 
         try:
             url = next(u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type)[
                 "downloadUrl"
@@ -93,98 +99,116 @@
         return await api.client.download(url, "GET", path=out_path)
 
 
 # Assignment
 
 
 class Assignor(BaseODPModel):
-    execution_date: datetime.date = Field(alias="executionDate")
-    assignor_name: str = Field(alias="assignorName")
+    execution_date: Optional[datetime.date] = Field(alias="executionDate", default=None)
+    assignor_name: Optional[str] = Field(alias="assignorName", default=None)
 
 
 class AssigneeAddress(BaseODPModel):
-    city_name: str = Field(alias="cityName")
-    geographic_region_code: str = Field(alias="geographicRegionCode")
-    postal_code: str = Field(alias="postalCode")
-    address_line_one_text: str = Field(alias="addressLineOneText")
+    city_name: Optional[str] = Field(alias="cityName", default=None)
+    geographic_region_code: Optional[str] = Field(alias="geographicRegionCode", default=None)
+    postal_code: Optional[str] = Field(alias="postalCode", default=None)
+    address_line_one_text: Optional[str] = Field(alias="addressLineOneText", default=None)
 
 
 class Assignee(BaseODPModel):
-    assignee_address: AssigneeAddress = Field(alias="assigneeAddress")
-    assignee_name_text: str = Field(alias="assigneeNameText")
+    assignee_address: Optional[AssigneeAddress] = Field(alias="assigneeAddress", default=None)
+    assignee_name_text: Optional[str] = Field(alias="assigneeNameText", default=None)
 
 
 class Assignment(BaseODPModel):
-    assignment_received_date: datetime.date = Field(alias="assignmentReceivedDate")
-    frame_number: str = Field(alias="frameNumber")
-    page_number: int = Field(alias="pageNumber")
-    reel_number_frame_number: str = Field(alias="reelNumber/frameNumber")
-    assignment_recorded_date: datetime.date = Field(alias="assignmentRecordedDate")
-    conveyance_text: str = Field(alias="conveyanceText")
-    assignment_mailed_date: datetime.date = Field(alias="assignmentMailedDate")
-    reel_number: str = Field(alias="reelNumber")
-    assignor_bag: list[Assignor] = Field(alias="assignorBag")
-    assignee_bag: list[Assignee] = Field(alias="assigneeBag")
-    correspondence_address: list[Address] = Field(alias="correspondenceAddress")
+    assignment_received_date: Optional[datetime.date] = Field(
+        alias="assignmentReceivedDate", default=None
+    )
+    frame_number: Optional[str] = Field(alias="frameNumber", default=None)
+    page_number: Optional[int] = Field(alias="pageNumber", default=None)
+    reel_number_frame_number: Optional[str] = Field(alias="reelNumber/frameNumber", default=None)
+    assignment_recorded_date: Optional[datetime.date] = Field(
+        alias="assignmentRecordedDate", default=None
+    )
+    conveyance_text: Optional[str] = Field(alias="conveyanceText", default=None)
+    assignment_mailed_date: Optional[datetime.date] = Field(
+        alias="assignmentMailedDate", default=None
+    )
+    reel_number: Optional[str] = Field(alias="reelNumber", default=None)
+    assignor_bag: list[Assignor] = Field(alias="assignorBag", default_factory=list)
+    assignee_bag: list[Assignee] = Field(alias="assigneeBag", default_factory=list)
+    correspondence_address: list[Address] = Field(
+        alias="correspondenceAddress", default_factory=list
+    )
 
 
 # Foreign Priority
 
 
 class ForeignPriority(BaseODPModel):
-    priority_number_text: str = Field(alias="priorityNumberText")
-    filing_date: datetime.date = Field(alias="filingDate")
-    country_name: str = Field(alias="countryName")
+    priority_number_text: Optional[str] = Field(alias="priorityNumberText", default=None)
+    filing_date: Optional[datetime.date] = Field(alias="filingDate", default=None)
+    country_name: Optional[str] = Field(alias="countryName", default=None)
 
 
 # Attorney
 
 
 class TelecommunicationAddress(BaseODPModel):
-    telecommunication_number: str = Field(alias="telecommunicationNumber")
-    usage_type_category: str = Field(alias="usageTypeCategory")
+    telecommunication_number: Optional[str] = Field(alias="telecommunicationNumber", default=None)
+    usage_type_category: Optional[str] = Field(alias="usageTypeCategory", default=None)
 
 
 class Attorney(BaseODPModel):
-    active_indicator: str = Field(alias="activeIndicator")
+    active_indicator: Optional[str] = Field(alias="activeIndicator", default=None)
     first_name: Optional[str] = Field(alias="firstName", default=None)
     last_name: Optional[str] = Field(alias="lastName", default=None)
-    registration_number: str = Field(alias="registrationNumber")
-    attorney_address_bag: list[Address] = Field(alias="attorneyAddressBag")
+    registration_number: Optional[str] = Field(alias="registrationNumber", default=None)
+    attorney_address_bag: list[Address] = Field(alias="attorneyAddressBag", default_factory=list)
     telecommunication_address_bag: list[TelecommunicationAddress] = Field(
-        alias="telecommunicationAddressBag"
+        alias="telecommunicationAddressBag", default_factory=list
+    )
+    registered_practitioner_category: Optional[str] = Field(
+        alias="registeredPractitionerCategory", default=None
     )
-    registered_practitioner_category: str = Field(alias="registeredPractitionerCategory")
     name_suffix: Optional[str] = Field(alias="nameSuffix", default=None)
 
 
 class CustomerNumber(BaseODPModel):
-    attorneys: list[Attorney] = Field(alias="attorneyBag")
-    customer_number: Optional[str] = Field(alias=AliasPath("customerNumber", "patronIdentifier"))
+    attorneys: list[Attorney] = Field(alias="attorneyBag", default_factory=list)
+    customer_number: Optional[str] = Field(
+        alias=AliasPath("customerNumber", "patronIdentifier"), default=None
+    )
     address: Optional[Address] = Field(
-        alias=AliasPath("customerNumber", "powerOfAttorneyAddressBag", 0)
+        alias=AliasPath("customerNumber", "powerOfAttorneyAddressBag", 0), default=None
     )
 
 
 # Transactions
 
 
 class Transaction(BaseODPModel):
-    recorded_date: datetime.date = Field(alias="recordedDate")
-    transaction_code: str = Field(alias="caseActionCode")
-    transaction_description: str = Field(alias="caseActionDescriptionText")
+    recorded_date: Optional[datetime.date] = Field(alias="recordedDate", default=None)
+    transaction_code: Optional[str] = Field(alias="caseActionCode", default=None)
+    transaction_description: Optional[str] = Field(alias="caseActionDescriptionText", default=None)
 
 
 # Adjustment Data
 class TermAdjustmentHistory(BaseODPModel):
-    applicant_day_delay_quantity: int = Field(alias="applicantDayDelayQuantity")
-    start_sequence_number: float = Field(alias="startSequenceNumber")
-    case_action_description_text: str = Field(alias="caseActionDescriptionText")
-    case_action_sequence_number: float = Field(alias="caseActionSequenceNumber")
-    action_date: datetime.date = Field(alias="actionDate")
+    applicant_day_delay_quantity: Optional[int] = Field(
+        alias="applicantDayDelayQuantity", default=None
+    )
+    start_sequence_number: Optional[float] = Field(alias="startSequenceNumber", default=None)
+    case_action_description_text: Optional[str] = Field(
+        alias="caseActionDescriptionText", default=None
+    )
+    case_action_sequence_number: Optional[float] = Field(
+        alias="caseActionSequenceNumber", default=None
+    )
+    action_date: Optional[datetime.date] = Field(alias="actionDate", default=None)
 
 
 class TermAdjustment(BaseODPModel):
     applicant_day_delay_quantity: Optional[int] = Field(
         alias="applicantDayDelayQuantity", default=None
     )
     overlapping_day_quantity: Optional[int] = Field(alias="overlappingDayQuantity", default=None)
@@ -197,53 +221,55 @@
     non_overlapping_day_quantity: Optional[int] = Field(
         alias="nonOverlappingDayQuantity", default=None
     )
     ip_office_day_delay_quantity: Optional[int] = Field(
         alias="ipOfficeDayDelayQuantity", default=None
     )
     history: Optional[list[TermAdjustmentHistory]] = Field(
-        alias="patentTermAdjustmentHistoryDataBag", default=None
+        alias="patentTermAdjustmentHistoryDataBag", default_factory=list
     )
 
 
 # Application Object
 
 YNBool = Annotated[bool, BeforeValidator(lambda v: v == "Y")]
 
 
 class Inventor(BaseODPModel):
-    first_name: str = Field(alias="firstName")
-    last_name: str = Field(alias="lastName")
-    full_name: str = Field(alias="inventorNameText")
-    addresses: list[Address] = Field(alias="correspondenceAddressBag")
+    first_name: Optional[str] = Field(alias="firstName", default=None)
+    last_name: Optional[str] = Field(alias="lastName", default=None)
+    full_name: Optional[str] = Field(alias="inventorNameText", default=None)
+    addresses: list[Address] = Field(alias="correspondenceAddressBag", default_factory=list)
 
 
 class Applicant(BaseODPModel):
-    applicant_name: str = Field(alias="applicantNameText")
-    addresses: list[Address] = Field(alias="correspondenceAddressBag")
-    app_status_code: int = Field(alias="applicationStatusCode")
-    app_status: str = Field(alias="applicationStatusDescriptionText")
+    applicant_name: Optional[str] = Field(alias="applicantNameText", default=None)
+    addresses: list[Address] = Field(alias="correspondenceAddressBag", default_factory=list)
+    app_status_code: Optional[int] = Field(alias="applicationStatusCode", default=None)
+    app_status: Optional[str] = Field(alias="applicationStatusDescriptionText", default=None)
 
 
 class USApplicationBiblio(BaseODPModel):
-    aia_indicator: YNBool = Field(alias="firstInventorToFileIndicator")
-    app_filing_date: datetime.date = Field(alias="filingDate")
-    inventors: list[Inventor] = Field(alias="inventorBag")
-    customer_number: int = Field(alias="customerNumber")
-    group_art_unit: str = Field(alias="groupArtUnitNumber")
-    invention_title: str = Field(alias="inventionTitle")
-    correspondence_address: list[Address] = Field(alias="correspondenceAddressBag")
-    app_conf_num: int = Field(alias="applicationConfirmationNumber")
+    aia_indicator: Optional[YNBool] = Field(alias="firstInventorToFileIndicator", default=None)
+    app_filing_date: Optional[datetime.date] = Field(alias="filingDate", default=None)
+    inventors: list[Inventor] = Field(alias="inventorBag", default_factory=list)
+    customer_number: Optional[int] = Field(alias="customerNumber", default=None)
+    group_art_unit: Optional[str] = Field(alias="groupArtUnitNumber", default=None)
+    invention_title: Optional[str] = Field(alias="inventionTitle", default=None)
+    correspondence_address: list[Address] = Field(
+        alias="correspondenceAddressBag", default_factory=list
+    )
+    app_conf_num: Optional[int] = Field(alias="applicationConfirmationNumber", default=None)
     atty_docket_num: Optional[str] = Field(alias="docketNumber", default=None)
-    appl_id: str = Field(alias="applicationNumberText")
-    first_inventor_name: str = Field(alias="firstInventorName")
+    appl_id: Optional[str] = Field(alias="applicationNumberText", default=None)
+    first_inventor_name: Optional[str] = Field(alias="firstInventorName", default=None)
     first_applicant_name: Optional[str] = Field(alias="firstApplicantName", default=None)
-    cpc_classifications: list[str] = Field(alias="cpcClassificationBag")
-    entity_status: str = Field(alias="businessEntityStatusCategory")
-    app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber")
+    cpc_classifications: list[str] = Field(alias="cpcClassificationBag", default_factory=list)
+    entity_status: Optional[str] = Field(alias="businessEntityStatusCategory", default=None)
+    app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber", default=None)
 
     @async_property
     async def bibliographic_data(self) -> "USApplicationBiblio":
         return await self._get_model(".model.USApplicationBiblio").objects.get(appl_id=self.appl_id)
 
     @async_property
     async def application(self) -> "USApplication":
@@ -289,83 +315,89 @@
 
     @async_property
     async def docs(self) -> list[Document]:
         return await self.documents
 
 
 class USApplication(BaseODPModel):
-    aia_indicator: YNBool = Field(alias="firstInventorToFileIndicator")
-    app_filing_date: datetime.date = Field(alias="filingDate")
-    inventors: list[Inventor] = Field(alias="inventorBag")
-    customer_number: int = Field(alias="customerNumber")
-    group_art_unit: str = Field(alias="groupArtUnitNumber")
-    invention_title: str = Field(alias="inventionTitle")
-    correspondence_address: list[Address] = Field(alias="correspondenceAddressBag")
-    app_conf_num: int = Field(alias="applicationConfirmationNumber")
+    aia_indicator: Optional[YNBool] = Field(alias="firstInventorToFileIndicator", default=None)
+    app_filing_date: Optional[datetime.date] = Field(alias="filingDate", default=None)
+    inventors: list[Inventor] = Field(alias="inventorBag", default_factory=list)
+    customer_number: Optional[int] = Field(alias="customerNumber", default=None)
+    group_art_unit: Optional[str] = Field(alias="groupArtUnitNumber", default=None)
+    invention_title: Optional[str] = Field(alias="inventionTitle", default=None)
+    correspondence_address: list[Address] = Field(
+        alias="correspondenceAddressBag", default_factory=list
+    )
+    app_conf_num: Optional[int] = Field(alias="applicationConfirmationNumber", default=None)
     atty_docket_num: Optional[str] = Field(alias="docketNumber", default=None)
-    appl_id: str = Field(alias="applicationNumberText")
-    first_inventor_name: str = Field(alias="firstInventorName")
+    appl_id: Optional[str] = Field(alias="applicationNumberText", default=None)
+    first_inventor_name: Optional[str] = Field(alias="firstInventorName", default=None)
     first_applicant_name: Optional[str] = Field(alias="firstApplicantName", default=None)
-    cpc_classifications: list[str] = Field(alias="cpcClassificationBag")
-    entity_status: str = Field(alias="businessEntityStatusCategory")
-    app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber")
-
-    app_type_code: str = Field(alias="applicationTypeCode")
-    national_stage_indicator: YNBool = Field(alias="nationalStageIndicator")
-
-    effective_filing_date: datetime.date = Field(alias="effectiveFilingDate")
-    cls_sub_cls: str = Field(alias="class/subclass")
-    assignments: list[Assignment] = Field(alias="assignmentBag")
-    attorneys: CustomerNumber = Field(alias="recordAttorney")
-    transactions: list[Transaction] = Field(alias="transactionContentBag")
+    cpc_classifications: list[str] = Field(alias="cpcClassificationBag", default_factory=list)
+    entity_status: Optional[str] = Field(alias="businessEntityStatusCategory", default=None)
+    app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber", default=None)
+
+    app_type_code: Optional[str] = Field(alias="applicationTypeCode", default=None)
+    national_stage_indicator: Optional[YNBool] = Field(alias="nationalStageIndicator", default=None)
+
+    effective_filing_date: Optional[datetime.date] = Field(
+        alias="effectiveFilingDate", default=None
+    )
+    cls_sub_cls: Optional[str] = Field(alias="class/subclass", default=None)
+    assignments: list[Assignment] = Field(alias="assignmentBag", default_factory=list)
+    attorneys: Optional[CustomerNumber] = Field(alias="recordAttorney", default=None)
+    transactions: list[Transaction] = Field(alias="transactionContentBag", default_factory=list)
     parent_applications: Optional[list[Relationship]] = Field(
-        alias=AliasPath("continuityBag", "parentContinuityBag"), default=None
+        alias=AliasPath("continuityBag", "parentContinuityBag"), default_factory=list
     )
     child_applications: Optional[list[Relationship]] = Field(
-        alias=AliasPath("continuityBag", "childContinuityBag"), default=None
+        alias=AliasPath("continuityBag", "childContinuityBag"), default_factory=list
+    )
+    patent_term_adjustment: Optional[TermAdjustment] = Field(
+        alias="patentTermAdjustmentData", default=None
     )
-    patent_term_adjustment: Optional[TermAdjustment] = Field(alias="patentTermAdjustmentData")
 
     @model_validator(mode="before")
     @classmethod
     def _validate_patent_term_adjustment(cls, v):
         if "patentTermAdjustmentData" in v and v["patentTermAdjustmentData"] == dict():
             v["patentTermAdjustmentData"] = None
         return v
 
 
 ## RESPONSE Models
 
 
 class SearchResult(BaseODPModel):
-    filing_date: datetime.date
-    appl_id: str = Field(alias="applicationNumberText")
-    invention_title: str = Field(alias="inventionTitle")
-    filing_date: datetime.date = Field(alias="filingDate")
+    filing_date: Optional[datetime.date] = Field(default=None)
+    appl_id: Optional[str] = Field(alias="applicationNumberText", default=None)
+    invention_title: Optional[str] = Field(alias="inventionTitle", default=None)
+    filing_date: Optional[datetime.date] = Field(default=None)
     patent_number: Optional[str] = Field(alias="patentNumber", default=None)
 
 
 class SearchResponse(BaseODPModel):
-    count: int
-    results: list[SearchResult] = Field(alias="patentBag")
-    request_id: str = Field(alias="requestIdentifier")
+    count: Optional[int] = Field(default=None)
+    results: list[SearchResult] = Field(alias="patentBag", default_factory=list)
+    request_id: Optional[str] = Field(alias="requestIdentifier", default=None)
 
 
 ## Request Models
 
 
 class Filter(BaseModel):
-    name: str
-    value: List[str]
+    name: Optional[str] = Field(default=None)
+    value: Optional[List[str]] = Field(default_factory=list)
 
 
 class Range(BaseModel):
-    field: str = Field(examples=["grantDate"])
-    valueFrom: str = Field(examples=["2020-01-01"])
-    valueTo: str = Field(examples=["2020-12-31"])
+    field: Optional[str] = Field(examples=["grantDate"], default=None)
+    valueFrom: Optional[str] = Field(examples=["2020-01-01"], default=None)
+    valueTo: Optional[str] = Field(examples=["2020-12-31"], default=None)
 
     @model_validator(mode="before")
     @classmethod
     def add_default_dates(cls, data: Any) -> Any:
         if data.get("valueFrom") is None:
             data["valueFrom"] = "1776-07-04"
         if data.get("valueTo") is None:
@@ -377,32 +409,32 @@
     asc = "asc"
     desc = "desc"
     Asc = "Asc"
     Desc = "Desc"
 
 
 class Sort(BaseModel):
-    field: str = Field(examples=["grantDate"])
-    order: SortOrder = Field(examples=[SortOrder.desc])
+    field: Optional[str] = Field(examples=["grantDate"], default=None)
+    order: Optional[SortOrder] = Field(examples=[SortOrder.desc], default=None)
 
 
 class Pagination(BaseModel):
-    offset: int = Field(examples=[0], default=0, ge=0)
-    limit: int = Field(examples=[25], default=25, ge=1)
+    offset: Optional[int] = Field(examples=[0], default=0, ge=0)
+    limit: Optional[int] = Field(examples=[25], default=25, ge=1)
 
 
 class SearchRequest(BaseModel):
-    q: str = Field(default="")
-    filters: Optional[List[Filter]] = Field(default=None)
-    rangeFilters: Optional[List[Range]] = Field(default=None)
-    sort: Optional[List[Sort]] = Field(default=None)
-    fields: Optional[List[str]] = Field(default=None)
+    q: Optional[str] = Field(default="")
+    filters: Optional[List[Filter]] = Field(default_factory=list)
+    rangeFilters: Optional[List[Range]] = Field(default_factory=list)
+    sort: Optional[List[Sort]] = Field(default_factory=list)
+    fields: Optional[List[str]] = Field(default_factory=list)
     pagination: Optional[Pagination] = Field(default=None)
-    facets: Optional[List[str]] = Field(default=None)
+    facets: Optional[List[str]] = Field(default_factory=list)
 
 
 class SearchGetRequest(BaseModel):
-    q: str = Field(default="")
-    sort: str = Field(default="filingDate")
-    fields: str = Field(default="")
-    offset: int = Field(default=0)
-    limit: int = Field(default=25)
+    q: Optional[str] = Field(default="")
+    sort: Optional[str] = Field(default="filingDate")
+    fields: Optional[str] = Field(default="")
+    offset: Optional[int] = Field(default=0)
+    limit: Optional[int] = Field(default=25)
```

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/model_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/query.py` & `patent_client-5.0.7/patent_client/_async/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/odp/query_fields.csv` & `patent_client-5.0.7/patent_client/_async/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/api_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.7/patent_client/_async/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.7/patent_client/_async/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/manager_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/model.py` & `patent_client-5.0.7/patent_client/_async/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/query.py` & `patent_client-5.0.7/patent_client/_async/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/peds/search_index.csv` & `patent_client-5.0.7/patent_client/_async/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/api_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/manager_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/ptab/model.py` & `patent_client-5.0.7/patent_client/_async/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/api.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/biblio.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/document.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/convert/shared.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/convert_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/count_query.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/manager.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/manager_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/model/__init__.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/model/biblio.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/model/document.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/model/shared.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/model_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/query.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/query_config.csv` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/query_test.py` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_async/uspto/public_search/search_query.json` & `patent_client-5.0.7/patent_client/_async/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/__init__.py` & `patent_client-5.0.7/patent_client/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/__init__.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/api.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/api_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/manager.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/model.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/model_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/schema.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/family/schema_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/api.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/api_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/manager.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/model.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/national_codes.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/national_codes.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/national_codes_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/national_codes_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/schema.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/schema_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/legal/util.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/legal/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/api.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/api_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/errors.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/errors.txt` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/messages.txt` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/model.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/number_service/schema.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/api.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/api_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/cql.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/manager.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/manager_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/__init__.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/biblio.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/fulltext.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/images.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/model/search.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/__init__.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/biblio.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/images.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema/search.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/schema_test.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/description_example.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/image_example.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/published/test/search_example.xml` & `patent_client-5.0.7/patent_client/_sync/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/session.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/epo/ops/util.py` & `patent_client-5.0.7/patent_client/_sync/epo/ops/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/http_client.py` & `patent_client-5.0.7/patent_client/_sync/http_client.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/odp.py` & `patent_client-5.0.7/patent_client/_sync/odp.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/convert.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/convert_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/manager_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/model.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/assignment/model_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/manager_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/bulk_data/model.py` & `patent_client-5.0.7/patent_client/_sync/uspto/bulk_data/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/model.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/model_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/query.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/query_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/app.json` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.7/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *              Source File: patent_client/_async/uspto/odp/api.py              *
 # ********************************************************************************
 
 import typing as tp
+from urllib.parse import quote
 
 from patent_client import SETTINGS
 
 from ...http_client import PatentClientSession
 from .model import (
     Assignment,
     Continuity,
@@ -21,100 +22,126 @@
     Transaction,
     USApplication,
     USApplicationBiblio,
 )
 from .util import prune
 
 
+def urlescape(s: str) -> str:
+    return quote(s, safe="")
+
+
 class ODPApi:
     base_url = "https://beta-api.uspto.gov"
 
     def __init__(self):
+        if SETTINGS.odp_api_key is None:
+            raise ValueError("ODP API key is not set")
         self.client = PatentClientSession(headers={"X-API-KEY": SETTINGS.odp_api_key})
 
     def post_search(self, search_request: SearchRequest = SearchRequest()) -> tp.Dict:
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = self.client.post(url, json=search_data, headers={"accept": "application/json"})
+        if response.status_code == 404 and "No matching records found" in response.text:
+            return {
+                "count": 0,
+                "patentBag": [],
+                "requestIdentifier": response.json()["requestIdentifier"],
+            }
         response.raise_for_status()
         return response.json()
 
     def get_search(self, search_request: SearchGetRequest = SearchGetRequest()) -> tp.Dict:
         """Patent application search by supplying query parameters
         Query parameters are optional. When no query parameters supplied, top 25 applications are returned"""
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = self.client.get(url, params=search_data)
+        if response.status_code == 404 and "No matching records found" in response.text:
+            return {
+                "count": 0,
+                "patentBag": [],
+                "requestIdentifier": response.json()["requestIdentifier"],
+            }
         response.raise_for_status()
         return response.json()
 
     # Data Attributes
 
     def get_application_data(self, application_id: str) -> USApplication:
         """Patent application data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}"
         response = self.client.get(url)
         response.raise_for_status()
         return USApplication(**response.json()["patentBag"][0])
 
     def get_application_biblio_data(self, application_id: str) -> USApplicationBiblio:
         """Patent application basic data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/application-data"
+        url = (
+            self.base_url
+            + f"/api/v1/patent/applications/{urlescape(application_id)}/application-data"
+        )
         response = self.client.get(url)
         response.raise_for_status()
         return USApplicationBiblio(**response.json()["patentBag"][0])
 
     def get_patent_term_adjustment_data(self, application_id: str) -> TermAdjustment:
         """Patent application term adjustment data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/adjustment"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/adjustment"
         response = self.client.get(url)
         response.raise_for_status()
         return TermAdjustment(**response.json()["patentBag"][0]["patentTermAdjustmentData"])
 
     def get_assignments(self, application_id: str) -> tp.List[Assignment]:
         """Patent application term adjustment data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/assignment"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/assignment"
         response = self.client.get(url)
         response.raise_for_status()
         data = response.json()["patentBag"][0]["assignmentBag"]
         return [Assignment(**assignment) for assignment in data]
 
     def get_attorney_data(self, application_id: str) -> CustomerNumber:
         """Patent application attorney data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/attorney"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/attorney"
         response = self.client.get(url)
         response.raise_for_status()
         return CustomerNumber(**response.json()["patentBag"][0]["recordAttorney"])
 
     def get_continuity_data(self, application_id: str) -> Continuity:
         """Patent application continuity data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/continuity"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/continuity"
         response = self.client.get(url)
         response.raise_for_status()
         return Continuity(**response.json())
 
     def get_foreign_priority_data(self, application_id: str) -> tp.List[ForeignPriority]:
         """Patent application foreign priority data by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/foreign-priority"
+        url = (
+            self.base_url
+            + f"/api/v1/patent/applications/{urlescape(application_id)}/foreign-priority"
+        )
         response = self.client.get(url)
         response.raise_for_status()
         return [
             ForeignPriority(**foreign_priority)
             for foreign_priority in response.json()["patentBag"][0]["foreignPriorityBag"]
         ]
 
     def get_transactions(self, application_id: str) -> tp.List[Transaction]:
         """Patent application transactions by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/transactions"
+        url = (
+            self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/transactions"
+        )
         response = self.client.get(url)
         response.raise_for_status()
         return [
             Transaction(**transaction)
             for transaction in response.json()["patentBag"][0]["transactionContentBag"]
         ]
 
     def get_documents(self, application_id: str) -> tp.List[Document]:
         """Patent application documents by application id"""
-        url = self.base_url + f"/api/v1/patent/applications/{application_id}/documents"
+        url = self.base_url + f"/api/v1/patent/applications/{urlescape(application_id)}/documents"
         response = self.client.get(url)
         response.raise_for_status()
         return [Document(**document) for document in response.json()["documentBag"]]
```

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/application.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/documents.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/search.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,39 +29,46 @@
 
 
 api = ODPApi()
 
 
 class USApplicationManager(Manager):
     default_filter = "appl_id"
-    default_fields = []
+    default_fields = ["applicationNumberText"]
     response_model = USApplication
 
     def count(self):
         return (api.post_search(self._create_search_obj(fields=["applicationNumberText"])))["count"]
 
     def _get_results(self) -> tp.Iterator["SearchResult"]:
         query_obj = self._create_search_obj()
         for start, rows in get_start_and_row_count(self.config.limit):
             page_query = query_obj.model_dump()
             page_query["pagination"] = {"offset": start, "limit": rows}
             page_query_obj = SearchRequest(**page_query)
             for result in (api.post_search(page_query_obj))["patentBag"]:
-                yield self.response_model(**result)
+                app_id = result["applicationNumberText"]
+                app = api.get_application_data(app_id)
+                yield app
 
     def _create_search_obj(self, fields: tp.Optional[tp.List[str]] = None):
         if fields is None:
             fields = self.default_fields
         if "query" in self.config.filter:
             return SearchRequest(**self.config.filter["query"][0], fields=fields)
         elif "q" in self.config.filter:
             return SearchRequest(q=self.config.filter["q"][0], fields=fields)
         else:
             return create_post_search_obj(self.config, fields=fields)
 
+    def get(self, *args, **kwargs):
+        if len(args) == 1 and not kwargs:
+            return api.get_application_data(args[0])
+        return super().get(*args, **kwargs)
+
 
 class USApplicationBiblioManager(USApplicationManager):
     default_filter = "appl_id"
     default_fields = [
         "firstInventorToFileIndicator",
         "filingDate",
         "inventorBag",
@@ -76,14 +83,28 @@
         "firstApplicantName",
         "cpcClassificationBag",
         "businessEntityStatusCategory",
         "earliestPublicationNumber",
     ]
     response_model = USApplicationBiblio
 
+    def _get_results(self) -> tp.Iterator["SearchResult"]:
+        query_obj = self._create_search_obj(fields=self.default_fields)
+        for start, rows in get_start_and_row_count(self.config.limit):
+            page_query = query_obj.model_dump()
+            page_query["pagination"] = {"offset": start, "limit": rows}
+            page_query_obj = SearchRequest(**page_query)
+            for result in (api.post_search(page_query_obj))["patentBag"]:
+                yield self.response_model(**result)
+
+    def get(self, *args, **kwargs):
+        if len(args) == 1 and not kwargs:
+            return api.get_application_biblio_data(args[0])
+        return super().get(*args, **kwargs)
+
 
 class AttributeManager(Manager):
     def filter(self, *args, **kwargs):
         raise NotImplementedError("Filtering attributes is not supported")
 
     def get(self, *args, **kwargs):
         raise NotImplementedError("Getting attributes is not supported")
```

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/model_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/query.py` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/query_fields.csv` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/odp/util.py` & `patent_client-5.0.7/patent_client/_sync/uspto/odp/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/__init__.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/fixtures/app_1_output.json` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/fixtures/app_1_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/manager_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/model.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/query.py` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/peds/search_index.csv` & `patent_client-5.0.7/patent_client/_sync/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/__init__.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/manager_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/model.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/ptab/util.py` & `patent_client-5.0.7/patent_client/_sync/uspto/ptab/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/__init__.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/api.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/api_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/biblio.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/document.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert/shared.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/convert_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/count_query.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/manager.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/manager_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/__init__.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/biblio.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/document.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/model/shared.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/model_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/query.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/query_config.csv` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/query_test.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/search_query.json` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/_sync/uspto/public_search/util.py` & `patent_client-5.0.7/patent_client/_sync/uspto/public_search/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/parser.py` & `patent_client-5.0.7/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/session.py` & `patent_client-5.0.7/patent_client/session.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/settings.py` & `patent_client-5.0.7/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/test_parser.py` & `patent_client-5.0.7/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/asyncio_util.py` & `patent_client-5.0.7/patent_client/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-5.0.7/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-5.0.7/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/examples/published_claims.json` & `patent_client-5.0.7/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/examples/published_claims.txt` & `patent_client-5.0.7/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/model.py` & `patent_client-5.0.7/patent_client/util/claims/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/parser.py` & `patent_client-5.0.7/patent_client/util/claims/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/claims/parser_test.py` & `patent_client-5.0.7/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/format.py` & `patent_client-5.0.7/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/manager.py` & `patent_client-5.0.7/patent_client/util/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/pydantic_util.py` & `patent_client-5.0.7/patent_client/util/pydantic_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/request_util.py` & `patent_client-5.0.7/patent_client/util/request_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/patent_client/util/test.py` & `patent_client-5.0.7/patent_client/util/test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.6/pyproject.toml` & `patent_client-5.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "5.0.6"
+version = "5.0.7"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
```

### Comparing `patent_client-5.0.6/PKG-INFO` & `patent_client-5.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-client
-Version: 5.0.6
+Version: 5.0.7
 Summary: A set of ORM-style clients for publicly available intellectual property data
 Home-page: https://github.com/parkerhancock/patent_client
 License: Apache Software License 2.0
 Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.9,<3.13
```

