# Comparing `tmp/mmisp_lib-0.1.1.tar.gz` & `tmp/mmisp_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmisp_lib-0.1.1.tar", last modified: Thu May  2 10:36:33 2024, max compression
+gzip compressed data, was "mmisp_lib-0.1.2.tar", last modified: Thu May  2 19:26:38 2024, max compression
```

## Comparing `mmisp_lib-0.1.1.tar` & `mmisp_lib-0.1.2.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.221535 mmisp_lib-0.1.1/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3076 2024-05-02 10:36:33.221535 mmisp_lib-0.1.1/PKG-INFO
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2050 2024-04-18 07:49:23.000000 mmisp_lib-0.1.1/README.md
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      947 2024-05-02 10:34:56.000000 mmisp_lib-0.1.1/pyproject.toml
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       38 2024-05-02 10:36:33.221535 mmisp_lib-0.1.1/setup.cfg
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.169534 mmisp_lib-0.1.1/src/
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.169534 mmisp_lib-0.1.1/src/mmisp/
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.169534 mmisp_lib-0.1.1/src/mmisp/api_schemas/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/__init__.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.177534 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1092 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/add_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      764 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/add_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      256 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/add_remove_tag_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      135 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/delete_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      226 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/delete_selected_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/delete_selected_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      675 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/edit_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      838 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/edit_attributes_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1163 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_all_attributes_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      901 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5547 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      756 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_describe_types_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      469 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/restore_attribute_reponse.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/search_attributes_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1162 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/search_attributes_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.181534 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      268 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/add_auth_key_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      431 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/add_auth_key_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      207 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/edit_auth_key_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      460 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/edit_auth_key_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      502 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      603 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      567 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.181534 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       97 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/exchange_token_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      102 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/password_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       81 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/start_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      364 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/start_login_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       80 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/authentication/token_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.185534 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      310 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/FreeTextImportWorkerBody.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      273 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      277 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5438 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_edit_get_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      808 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      236 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_remove_tag_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      248 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/delete_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/edit_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2143 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/get_all_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      158 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/get_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      926 2024-05-02 10:34:56.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/index_events_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      881 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/index_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      247 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/publish_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1347 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/search_events_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/search_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      249 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/events/unpublish_event_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.189534 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      190 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/cache_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      924 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/create_feed_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      164 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/enable_disable_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      128 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/fetch_feeds_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1234 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/get_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      126 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/toggle_feed_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      893 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/update_feed_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.193534 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      229 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      179 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      238 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/delete_force_update_import_galaxy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      323 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/export_galaxies_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1139 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/export_galaxies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      289 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/galaxy_schema.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      421 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/get_all_search_galaxies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      866 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/get_galaxy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      298 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/import_galaxies_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      514 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/search_galaxies_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.193534 mmisp_lib-0.1.1/src/mmisp/api_schemas/noticelists/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/noticelists/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      237 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/noticelists/get_all_noticelist_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      747 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/noticelists/get_noticelist_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.197534 mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      578 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/create_object_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1505 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/get_object_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1539 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/search_objects_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.197534 mmisp_lib-0.1.1/src/mmisp/api_schemas/organisations/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/organisations/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      583 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/organisations/organisation.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.197534 mmisp_lib-0.1.1/src/mmisp/api_schemas/roles/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/roles/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2980 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/roles/role.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.201534 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      131 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      113 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      130 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      118 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      428 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/create_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      862 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      524 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      140 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/delete_sharing_group_legacy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1443 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      340 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/sharing_group.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      138 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/sharing_group_org.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      146 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/sharing_group_server.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      357 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/update_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1062 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1084 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.201534 mmisp_lib-0.1.1/src/mmisp/api_schemas/sightings/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sightings/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1487 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sightings/create_sighting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      589 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/sightings/get_sighting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      230 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/standard_status_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.205534 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      392 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/create_tag_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      156 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/delete_tag_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      645 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/get_tag_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      690 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/search_tags_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      369 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/update_tag_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.205534 mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      566 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      632 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      367 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/get_taxonomy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      676 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.209535 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      301 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/get_uid_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      232 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/get_user_settings_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      161 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/search_user_setting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      209 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/search_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       93 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/set_user_setting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/set_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/user_settings/view_user_setting_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.209535 mmisp_lib-0.1.1/src/mmisp/api_schemas/users/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/users/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      910 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/users/user.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/users/users_view_me_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.209535 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      136 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/check_value_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/check_value_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     7189 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/create_warninglist_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      210 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/delete_warninglist_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      341 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/get_selected_all_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      183 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      191 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      204 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      952 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/warninglist_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.213534 mmisp_lib-0.1.1/src/mmisp/db/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/src/mmisp/db/config.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1099 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/src/mmisp/db/database.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.217535 mmisp_lib-0.1.1/src/mmisp/db/models/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3685 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/src/mmisp/db/models/attribute.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/auth_key.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2707 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/event.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1498 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/feed.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      858 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/galaxy.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2456 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/galaxy_cluster.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      846 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/identity_provider.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      888 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/noticelist.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1819 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/object.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      940 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/organisation.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2188 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/role.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1495 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/server.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1727 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/sharing_group.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      829 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/sighting.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      752 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/tag.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1434 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/taxonomy.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2068 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/user.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      997 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/user_setting.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1185 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/models/warninglist.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1181 2024-04-18 07:49:24.000000 mmisp_lib-0.1.1/src/mmisp/db/print_changes.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.221535 mmisp_lib-0.1.1/src/mmisp/lib/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/src/mmisp/lib/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)    53293 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/src/mmisp/lib/attributes.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.221535 mmisp_lib-0.1.1/src/mmisp_lib.egg-info/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3076 2024-05-02 10:36:33.000000 mmisp_lib-0.1.1/src/mmisp_lib.egg-info/PKG-INFO
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     8660 2024-05-02 10:36:33.000000 mmisp_lib-0.1.1/src/mmisp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        1 2024-05-02 10:36:33.000000 mmisp_lib-0.1.1/src/mmisp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      420 2024-05-02 10:36:33.000000 mmisp_lib-0.1.1/src/mmisp_lib.egg-info/requires.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        6 2024-05-02 10:36:33.000000 mmisp_lib-0.1.1/src/mmisp_lib.egg-info/top_level.txt
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 10:36:33.221535 mmisp_lib-0.1.1/tests/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       42 2024-04-30 12:43:28.000000 mmisp_lib-0.1.1/tests/test_dummy.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.363388 mmisp_lib-0.1.2/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3076 2024-05-02 19:26:38.363388 mmisp_lib-0.1.2/PKG-INFO
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2050 2024-04-18 07:49:23.000000 mmisp_lib-0.1.2/README.md
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      947 2024-05-02 19:26:24.000000 mmisp_lib-0.1.2/pyproject.toml
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       38 2024-05-02 19:26:38.363388 mmisp_lib-0.1.2/setup.cfg
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.343387 mmisp_lib-0.1.2/src/
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.343387 mmisp_lib-0.1.2/src/mmisp/
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.343387 mmisp_lib-0.1.2/src/mmisp/api_schemas/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/__init__.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.347387 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1092 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/add_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      764 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/add_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      256 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/add_remove_tag_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      135 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/delete_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      226 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/delete_selected_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/delete_selected_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      675 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/edit_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      838 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/edit_attributes_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1163 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_all_attributes_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      901 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1486 2024-05-02 19:26:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      813 2024-05-02 19:26:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_describe_types_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      469 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/restore_attribute_reponse.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3225 2024-05-02 19:26:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/search_attributes_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1119 2024-05-02 19:26:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/search_attributes_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.347387 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      268 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/add_auth_key_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      431 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/add_auth_key_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      207 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/edit_auth_key_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      460 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/edit_auth_key_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      502 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      603 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      567 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.347387 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       97 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/exchange_token_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      102 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/password_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       81 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/start_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      364 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/start_login_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       80 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/authentication/token_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      310 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/FreeTextImportWorkerBody.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      273 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      277 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5438 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_edit_get_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      808 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      236 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_remove_tag_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      248 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/delete_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/edit_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2143 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/get_all_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      158 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/get_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      926 2024-05-02 10:34:56.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/index_events_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      881 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/index_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      247 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/publish_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1347 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/search_events_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/search_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      249 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/events/unpublish_event_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      190 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/cache_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      924 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/create_feed_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      164 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/enable_disable_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      128 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/fetch_feeds_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1234 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/get_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      126 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/toggle_feed_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      893 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/update_feed_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      229 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      179 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      238 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/delete_force_update_import_galaxy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      323 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/export_galaxies_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1139 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/export_galaxies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      289 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/galaxy_schema.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      421 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/get_all_search_galaxies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      866 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/get_galaxy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      298 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/import_galaxies_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      514 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/search_galaxies_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/noticelists/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/noticelists/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      237 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/noticelists/get_all_noticelist_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      747 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/noticelists/get_noticelist_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      578 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/create_object_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1505 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/get_object_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1539 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/search_objects_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/organisations/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/organisations/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      583 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/organisations/organisation.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.351388 mmisp_lib-0.1.2/src/mmisp/api_schemas/roles/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/roles/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2980 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/roles/role.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      131 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      113 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      130 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      118 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      428 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/create_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      862 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      524 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      140 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/delete_sharing_group_legacy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1443 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      340 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/sharing_group.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      138 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/sharing_group_org.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      146 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/sharing_group_server.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      357 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/update_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1062 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1084 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/sightings/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sightings/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1487 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sightings/create_sighting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      589 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/sightings/get_sighting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      230 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/standard_status_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      392 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/create_tag_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      156 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/delete_tag_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      645 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/get_tag_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      690 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/search_tags_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      369 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/update_tag_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      566 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      632 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      367 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/get_taxonomy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      676 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      301 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/get_uid_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      232 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/get_user_settings_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      161 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/search_user_setting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      209 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/search_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       93 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/set_user_setting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/set_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/user_settings/view_user_setting_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/users/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/users/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      910 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/users/user.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/users/users_view_me_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.355388 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      136 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/check_value_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/check_value_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     7189 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/create_warninglist_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      210 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/delete_warninglist_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      341 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/get_selected_all_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      183 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      191 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      204 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      952 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/warninglist_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.359388 mmisp_lib-0.1.2/src/mmisp/db/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-30 12:43:28.000000 mmisp_lib-0.1.2/src/mmisp/db/config.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1099 2024-04-30 12:43:28.000000 mmisp_lib-0.1.2/src/mmisp/db/database.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.359388 mmisp_lib-0.1.2/src/mmisp/db/models/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3685 2024-04-30 12:43:28.000000 mmisp_lib-0.1.2/src/mmisp/db/models/attribute.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/auth_key.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2707 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/event.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1498 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/feed.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      858 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/galaxy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2456 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/galaxy_cluster.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      846 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/identity_provider.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      888 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/noticelist.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1819 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/object.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      940 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/organisation.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2188 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/role.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1495 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/server.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1727 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/sharing_group.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      829 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/sighting.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      752 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/tag.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1434 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/taxonomy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2068 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/user.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      997 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/user_setting.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1185 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/models/warninglist.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1181 2024-04-18 07:49:24.000000 mmisp_lib-0.1.2/src/mmisp/db/print_changes.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.359388 mmisp_lib-0.1.2/src/mmisp/lib/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-30 12:43:28.000000 mmisp_lib-0.1.2/src/mmisp/lib/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)    53293 2024-04-30 12:43:28.000000 mmisp_lib-0.1.2/src/mmisp/lib/attributes.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.359388 mmisp_lib-0.1.2/src/mmisp_lib.egg-info/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3076 2024-05-02 19:26:38.000000 mmisp_lib-0.1.2/src/mmisp_lib.egg-info/PKG-INFO
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     8660 2024-05-02 19:26:38.000000 mmisp_lib-0.1.2/src/mmisp_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        1 2024-05-02 19:26:38.000000 mmisp_lib-0.1.2/src/mmisp_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      420 2024-05-02 19:26:38.000000 mmisp_lib-0.1.2/src/mmisp_lib.egg-info/requires.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        6 2024-05-02 19:26:38.000000 mmisp_lib-0.1.2/src/mmisp_lib.egg-info/top_level.txt
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-02 19:26:38.359388 mmisp_lib-0.1.2/tests/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       42 2024-04-30 12:43:28.000000 mmisp_lib-0.1.2/tests/test_dummy.py
```

### Comparing `mmisp_lib-0.1.1/PKG-INFO` & `mmisp_lib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmisp-lib
-Version: 0.1.1
+Version: 0.1.2
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: SQLAlchemy[asyncio]==1.4.46
 Requires-Dist: pydantic==1.10.13
 Requires-Dist: uvicorn==0.24.0.post1
 Requires-Dist: python-dotenv==1.0.0
```

### Comparing `mmisp_lib-0.1.1/README.md` & `mmisp_lib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/pyproject.toml` & `mmisp_lib-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmisp-lib"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = []
 readme = "README.md"
 requires-python = ">=3.11.0"
 
 
 dependencies = [
```

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/add_attribute_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/add_attribute_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/add_attribute_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/add_attribute_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/edit_attribute_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/edit_attribute_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/edit_attributes_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/edit_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_all_attributes_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_all_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_attribute_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_attribute_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/get_describe_types_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/get_describe_types_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from pydantic import BaseModel
 
-from mmisp.lib.attributes import AttributeCategories, default_category, inverted_categories, to_ids
+from mmisp.lib.attributes import (
+    AttributeCategories,
+    default_category,
+    inverted_categories,
+    mapper_val_safe_clsname,
+    to_ids,
+)
 
 
 class GetDescribeTypesAttributes(BaseModel):
     sane_defaults: dict = {}
     for k, v in to_ids.items():
         sane_defaults.update(
             {
                 k: {
                     "default_category": default_category[k],
                     "to_ids": v,
                 }
             }
         )
 
-    types: list[str] = list(default_category.keys())
+    types: list[str] = list(mapper_val_safe_clsname.keys())
 
     categories: list[str] = [member.value for member in AttributeCategories]
 
     category_type_mappings: dict = inverted_categories
 
 
 class GetDescribeTypesResponse(BaseModel):
```

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/search_attributes_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/search_attributes_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     decay_speed: int
     threshold: int
     default_base_score: int
     base_score_config: SearchAttributesModelOverridesBaseScoreConfig
 
 
 class SearchAttributesBody(BaseModel):
-    returnFormat: str
+    returnFormat: str = "json"
     page: int | None = None
     limit: int | None = None
     value: str | None = None
     value1: str | None = None
     value2: str | None = None
     type: str | None = None
     category: str | None = None
```

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/attributes/search_attributes_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/attributes/search_attributes_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,15 +38,12 @@
     last_seen: str | None = None
     Event: SearchAttributesEvent | None = None
     Object: SearchAttributesObject | None = None
     Tag: list[GetAttributeTag] = []
 
 
 class SearchAttributesAttributes(BaseModel):
-    Attribute: SearchAttributesAttributesDetails
+    Attribute: list[SearchAttributesAttributesDetails]
 
 
 class SearchAttributesResponse(BaseModel):
-    response: list[SearchAttributesAttributes]
-
-    class Config:
-        orm_mode = True
+    response: SearchAttributesAttributes
```

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_edit_get_event_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_edit_get_event_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/add_event_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/add_event_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/edit_event_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/edit_event_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/get_all_events_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/get_all_events_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/index_events_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/index_events_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/index_events_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/index_events_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/events/search_events_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/events/search_events_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/create_feed_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/create_feed_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/get_feed_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/get_feed_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/feeds/update_feed_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/feeds/update_feed_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/export_galaxies_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/export_galaxies_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/get_galaxy_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/get_galaxy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/galaxies/search_galaxies_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/galaxies/search_galaxies_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/noticelists/get_noticelist_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/noticelists/get_noticelist_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/create_object_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/create_object_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/get_object_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/get_object_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/objects/search_objects_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/objects/search_objects_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/organisations/organisation.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/organisations/organisation.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/roles/role.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/roles/role.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sightings/create_sighting_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sightings/create_sighting_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/sightings/get_sighting_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/sightings/get_sighting_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/get_tag_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/get_tag_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/tags/search_tags_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/tags/search_tags_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/users/user.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/users/user.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/create_warninglist_body.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/create_warninglist_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/api_schemas/warninglists/warninglist_response.py` & `mmisp_lib-0.1.2/src/mmisp/api_schemas/warninglists/warninglist_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/database.py` & `mmisp_lib-0.1.2/src/mmisp/db/database.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/attribute.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/attribute.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/auth_key.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/auth_key.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/event.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/event.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/feed.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/feed.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/galaxy.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/galaxy.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/galaxy_cluster.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/galaxy_cluster.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/identity_provider.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/identity_provider.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/noticelist.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/noticelist.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/object.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/object.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/organisation.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/organisation.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/role.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/role.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/server.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/server.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/sharing_group.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/sharing_group.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/sighting.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/sighting.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/tag.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/tag.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/taxonomy.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/taxonomy.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/user.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/user.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/user_setting.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/models/warninglist.py` & `mmisp_lib-0.1.2/src/mmisp/db/models/warninglist.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/db/print_changes.py` & `mmisp_lib-0.1.2/src/mmisp/db/print_changes.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp/lib/attributes.py` & `mmisp_lib-0.1.2/src/mmisp/lib/attributes.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.1/src/mmisp_lib.egg-info/PKG-INFO` & `mmisp_lib-0.1.2/src/mmisp_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmisp-lib
-Version: 0.1.1
+Version: 0.1.2
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: SQLAlchemy[asyncio]==1.4.46
 Requires-Dist: pydantic==1.10.13
 Requires-Dist: uvicorn==0.24.0.post1
 Requires-Dist: python-dotenv==1.0.0
```

### Comparing `mmisp_lib-0.1.1/src/mmisp_lib.egg-info/SOURCES.txt` & `mmisp_lib-0.1.2/src/mmisp_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

