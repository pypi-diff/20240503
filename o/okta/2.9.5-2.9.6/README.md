# Comparing `tmp/okta-2.9.5.tar.gz` & `tmp/okta-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okta-2.9.5.tar", last modified: Fri Dec 15 20:33:15 2023, max compression
+gzip compressed data, was "okta-2.9.6.tar", last modified: Fri May  3 18:15:44 2024, max compression
```

## Comparing `okta-2.9.5.tar` & `okta-2.9.6.tar`

### file list

```diff
@@ -1,881 +1,881 @@
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.714028 okta-2.9.5/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    25789 2023-12-15 20:32:20.000000 okta-2.9.5/CHANGELOG.md
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9809 2023-07-26 15:09:45.000000 okta-2.9.5/LICENSE.md
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      554 2023-07-26 15:09:45.000000 okta-2.9.5/LONG_DESCRIPTION.md
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      112 2023-07-26 15:09:45.000000 okta-2.9.5/MANIFEST.in
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1326 2023-12-15 20:33:15.714028 okta-2.9.5/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    38660 2023-12-13 16:09:31.000000 okta-2.9.5/README.md
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.009906 okta-2.9.5/okta/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       22 2023-12-15 20:32:20.000000 okta-2.9.5/okta/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      726 2023-07-26 15:09:45.000000 okta-2.9.5/okta/api_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6004 2023-12-13 16:09:31.000000 okta-2.9.5/okta/api_response.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.009906 okta-2.9.5/okta/cache/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.5/okta/cache/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2418 2023-07-26 15:09:45.000000 okta-2.9.5/okta/cache/cache.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1262 2023-07-26 15:09:45.000000 okta-2.9.5/okta/cache/no_op_cache.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4366 2023-07-26 15:09:45.000000 okta-2.9.5/okta/cache/okta_cache.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6758 2023-07-26 15:09:45.000000 okta-2.9.5/okta/client.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.013907 okta-2.9.5/okta/config/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.5/okta/config/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6456 2023-07-26 15:09:45.000000 okta-2.9.5/okta/config/config_setter.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6647 2023-07-26 15:09:45.000000 okta-2.9.5/okta/config/config_validator.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3538 2023-07-26 15:09:45.000000 okta-2.9.5/okta/constants.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2570 2023-07-26 15:09:45.000000 okta-2.9.5/okta/error_messages.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.021908 okta-2.9.5/okta/errors/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.5/okta/errors/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      194 2023-07-26 15:09:45.000000 okta-2.9.5/okta/errors/error.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      335 2023-07-26 15:09:45.000000 okta-2.9.5/okta/errors/http_error.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      904 2023-07-26 15:09:45.000000 okta-2.9.5/okta/errors/okta_api_error.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.033910 okta-2.9.5/okta/exceptions/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       65 2023-07-26 15:09:45.000000 okta-2.9.5/okta/exceptions/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      150 2023-07-26 15:09:45.000000 okta-2.9.5/okta/exceptions/exceptions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1076 2023-07-26 15:09:45.000000 okta-2.9.5/okta/helpers.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6776 2023-07-26 15:09:45.000000 okta-2.9.5/okta/http_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4767 2023-07-26 15:09:45.000000 okta-2.9.5/okta/jwt.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      510 2023-07-26 15:09:45.000000 okta-2.9.5/okta/logger.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.429979 okta-2.9.5/okta/models/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    71986 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1133 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1865 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_constraint.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2520 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_constraints.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2756 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1961 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_rule_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2101 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_rule_application_sign_on.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3386 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_rule_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1320 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/access_policy_rule_custom_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1396 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/acs_endpoint.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2076 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/activate_factor_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      918 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/allowed_for_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1598 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_and_instance_condition_evaluator_app_or_instance.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2006 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_and_instance_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1672 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_instance_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2865 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_link.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4128 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_user.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2010 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_user_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1284 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/app_user_password_credential.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7225 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1769 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_accessibility.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2758 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2916 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_credentials_o_auth_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1254 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_credentials_scheme.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2574 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_credentials_signing.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      867 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_credentials_signing_use.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1817 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_credentials_username_template.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3026 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_feature.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2198 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_group_assignment.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1301 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_licensing.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3728 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2413 2023-08-24 13:16:58.000000 okta-2.9.5/okta/models/application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1446 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_settings_notes.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1865 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_settings_notifications.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2296 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_settings_notifications_vpn.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1878 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_settings_notifications_vpn_network.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1419 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_sign_on_mode.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2379 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_visibility.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1415 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/application_visibility_hide.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1685 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/assign_role_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1953 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authentication_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1054 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authentication_provider_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4773 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2099 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3379 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator_provider_configuration.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1346 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator_provider_configuration_user_name_plate.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4439 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      888 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1089 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authenticator_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3924 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1961 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      922 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_credentials_rotation_mode.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3298 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_credentials_signing_config.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      869 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_credentials_use.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4136 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4025 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_policy_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1935 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_policy_rule_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4078 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/authorization_server_policy_rule_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2756 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/auto_login_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1940 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/auto_login_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1514 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/auto_login_application_settings_sign_on.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1888 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/basic_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1532 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/basic_application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2908 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/basic_auth_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2594 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/before_scheduled_action_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2131 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/bookmark_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1912 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/bookmark_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1604 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/bookmark_application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2258 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/brand.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2031 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/browser_plugin_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1843 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/call_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1524 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/call_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1957 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/capabilities_create_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2488 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/capabilities_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3393 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/capabilities_update_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4028 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/catalog_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      898 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/catalog_application_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      885 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/change_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2474 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/change_password_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1903 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/channel_binding.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1413 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/client_policy_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2371 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/client_secret.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1320 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/client_secret_metadata.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1671 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/compliance.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1316 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/context_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1319 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/create_session_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3277 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/create_user_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1666 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/csr.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2590 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/csr_metadata.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2417 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/csr_metadata_subject.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1432 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/csr_metadata_subject_alt_names.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2119 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/custom_hotp_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1333 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/custom_hotp_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1549 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/device_access_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2416 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/device_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1762 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/device_policy_rule_condition_platform.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2392 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/dns_record.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      858 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/dns_record_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4310 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2361 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain_certificate.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1666 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain_certificate_metadata.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      916 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain_certificate_source_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      845 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain_certificate_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1463 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain_list_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1109 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/domain_validation_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1402 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/duration.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1488 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_template.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2030 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_template_content.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2516 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_template_customization.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1807 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_template_customization_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1345 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_template_test_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      934 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_template_touch_point_variant.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1852 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1278 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/email_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      879 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/enabled_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1118 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/end_user_dashboard_touch_point_variant.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1036 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/error_page_touch_point_variant.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3833 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_hook.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2101 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_hook_channel.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2510 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_hook_channel_config.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2195 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_hook_channel_config_auth_scheme.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_hook_channel_config_auth_scheme_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1430 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_hook_channel_config_header.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1541 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/event_subscriptions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1069 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/factor_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1237 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/factor_result_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1094 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/factor_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1304 2023-08-24 13:16:58.000000 okta-2.9.5/okta/models/factor_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3605 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/feature.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2384 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/feature_stage.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      872 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/feature_stage_state.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      860 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/feature_stage_value.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      852 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/feature_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      872 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/fips_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1350 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/forgot_password_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1427 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/grant_type_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3752 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1640 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1660 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3131 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3866 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1963 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_action.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2512 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1418 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_expression.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1428 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_group_assignment.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1658 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_group_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2478 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_people_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      915 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1656 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_rule_user_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4144 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_schema.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7221 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_schema_attribute.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2430 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_schema_base.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2412 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_schema_base_properties.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1873 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_schema_custom.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2376 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_schema_definitions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      921 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/group_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1885 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/hardware_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1329 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/hardware_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3750 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2387 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_application_user.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3365 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1520 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_credentials_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1636 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_credentials_signing.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2062 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_credentials_trust.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3437 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1608 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/identity_provider_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1573 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/idp_policy_rule_action.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1416 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/idp_policy_rule_action_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/iframe_embed_scope_allowed_apps.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1260 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/image_upload_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1444 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inactivity_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4044 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2109 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_channel.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2684 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_channel_config.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1586 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_channel_config_auth_scheme.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1434 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_channel_config_headers.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1097 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_payload.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1558 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1574 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_response_command_value.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1721 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_response_commands.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      882 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1350 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/inline_hook_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2905 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/ion_field.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2861 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/ion_form.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3823 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/json_web_key.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1234 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/jwk_use.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1150 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/knowledge_constraint.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1761 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/lifecycle_create_setting_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1769 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/lifecycle_deactivate_setting_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1677 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/lifecycle_expiration_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2634 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/linked_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2273 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/linked_object_details.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      852 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/linked_object_details_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1918 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_actor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4835 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_authentication_context.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1151 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_authentication_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3207 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1186 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_credential_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1047 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_credential_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1291 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_debug_context.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8585 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_event.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2454 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_geographical_context.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1390 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_geolocation.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2397 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_ip_address.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1380 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_issuer.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1418 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_outcome.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1480 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1911 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_security_context.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      912 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_severity.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1953 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_target.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1548 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_transaction.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1604 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/log_user_agent.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1573 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/mdm_enrollment_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1163 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/multifactor_enrollment_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2309 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/multifactor_enrollment_policy_authenticator_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      995 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/multifactor_enrollment_policy_authenticator_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1558 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/multifactor_enrollment_policy_authenticator_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2486 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/multifactor_enrollment_policy_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      914 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/multifactor_enrollment_policy_settings_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5481 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1931 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone_address.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      879 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone_address_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1442 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone_location.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      865 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      885 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/network_zone_usage.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1487 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/notification_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1384 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_actor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3638 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_claim.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1407 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_claim_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2048 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3777 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_refresh_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2464 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_scope.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4812 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_scope_consent_grant.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      905 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_scope_consent_grant_source.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      905 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_scope_consent_grant_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1451 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_scopes_mediation_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3110 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_2_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1997 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_application_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1157 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_authorization_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1135 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_endpoint_authentication_method.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1487 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_grant_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/o_auth_response_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1964 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1844 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2822 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1925 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy_rule_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3332 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy_rule_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3028 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy_rule_signon_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1936 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/okta_sign_on_policy_rule_signon_session_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2958 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      927 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_consent_method.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1633 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_idp_initiated_login.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      962 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_issuer_mode.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2032 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8880 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_settings_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1515 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_settings_client_keys.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2194 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_settings_refresh_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      961 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_application_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      918 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/open_id_connect_refresh_token_rotation_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2040 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_2_org_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1877 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_2_org_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1750 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_2_org_application_settings_app.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_contact_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2049 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_contact_type_obj.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1505 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_contact_user.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1597 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_okta_communication_setting.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      895 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_okta_support_setting.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2239 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_okta_support_settings_obj.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1577 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_preferences.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4373 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/org_setting.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2568 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_credential.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2563 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_credential_hash.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      997 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_credential_hash_algorithm.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1272 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_credential_hook.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1803 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_dictionary.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1296 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_dictionary_common.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1460 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_expiration_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2633 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1631 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_authentication_provider_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2737 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1941 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_delegation_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1345 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_delegation_settings_options.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3473 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_password_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1927 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_password_settings_age.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3328 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_password_settings_complexity.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2261 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_password_settings_lockout.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2113 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_email.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2039 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_email_properties.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1412 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_email_recovery_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1324 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_factor_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4208 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_factors.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2137 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_question.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1341 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_question_complexity.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1999 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_question_properties.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1873 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_recovery_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2779 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1288 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_rule_action.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3537 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_rule_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2533 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_rule_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3409 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_policy_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2921 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/password_setting_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2095 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/platform_condition_evaluator_platform.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2413 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/platform_condition_evaluator_platform_operating_system.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1525 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/platform_condition_evaluator_platform_operating_system_version.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1912 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/platform_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4098 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1957 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_account_link.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1851 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_account_link_filter.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1429 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_account_link_filter_groups.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1838 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_network_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2348 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_people_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3743 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5548 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_rule_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1823 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_rule_actions_enroll.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      933 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_rule_actions_enroll_self.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1315 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_rule_auth_context_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17081 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_rule_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3294 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_subject.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1018 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_subject_match_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1198 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1296 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/policy_user_name_template.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2019 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/possession_constraint.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1332 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/pre_registration_inline_hook.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1155 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_enrollment_policy.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2104 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_enrollment_policy_rule.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4128 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_enrollment_policy_rule_action.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2069 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_enrollment_policy_rule_actions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1405 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_enrollment_policy_rule_activation_requirement.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1636 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_enrollment_policy_rule_profile_attribute.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2904 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_mapping.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2111 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_mapping_property.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      911 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_mapping_property_push_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1782 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_mapping_source.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1745 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/profile_setting_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5651 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1885 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_algorithm_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1470 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_algorithm_type_signature.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2408 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_algorithms.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1752 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_endpoint.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5698 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_endpoints.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1815 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_relay_state.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      898 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_relay_state_format.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1299 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/protocol_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2829 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2712 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_conditions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2876 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_connection.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      908 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_connection_auth_scheme.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2091 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_connection_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1867 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_connection_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      944 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_connection_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1308 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_deprovisioned_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2066 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_groups.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1300 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/provisioning_suspended_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2745 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/push_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2177 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/push_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1462 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/recovery_question_credential.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      921 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/required_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1342 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/reset_password_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1342 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/response_links.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1429 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/risk_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1290 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/risk_score_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4257 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/role.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      871 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/role_assignment_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      870 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/role_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1394 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/role_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1941 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/saml_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1896 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/saml_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8478 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/saml_application_settings_sign_on.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2253 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/saml_attribute_statement.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1296 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/scheduled_user_lifecycle_action.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3681 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/scheme_application_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2353 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/scope.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      912 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/scope_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3017 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/secure_password_store_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2008 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/secure_password_store_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3170 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/secure_password_store_application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1639 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/security_question.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1947 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/security_question_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1673 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/security_question_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      854 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/seed_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4344 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/session.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1107 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/session_authentication_method.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1953 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/session_identity_provider.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1024 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/session_identity_provider_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      932 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/session_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1038 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sign_in_page_touch_point_variant.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1248 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sign_on_inline_hook.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1607 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/single_logout.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3275 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sms_template.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1203 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sms_template_translations.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      869 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sms_template_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1834 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sms_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1313 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sms_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2257 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/social_auth_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1379 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/sp_certificate.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3055 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/subscription.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      910 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/subscription_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2028 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/swa_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1872 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/swa_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2525 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/swa_application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2128 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/swa_three_field_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1960 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/swa_three_field_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2734 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/swa_three_field_application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1303 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/temp_password.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6683 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/theme.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7143 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/theme_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2203 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/threat_insight_configuration.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2938 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/token_authorization_server_policy_rule_action.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1316 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/token_authorization_server_policy_rule_action_inline_hook.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1852 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/token_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1323 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/token_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1858 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/totp_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1321 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/totp_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3013 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/trusted_origin.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1842 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/u_2_f_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1319 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/u_2_f_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5966 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1538 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_activation_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1638 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3298 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_credentials.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4580 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1292 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_id_string.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1491 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_identifier_condition_evaluator_pattern.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1965 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_identifier_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1329 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_identity_provider_link_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1570 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_lifecycle_attribute_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      863 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_next_login.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5288 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9044 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3948 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7383 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1432 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1912 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_items.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2310 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_master.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1446 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_master_priority.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      958 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_master_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1474 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_permission.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      880 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_scope.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      989 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      895 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_attribute_union.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2422 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_base.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    20607 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_base_properties.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2362 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_definitions.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1841 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_properties.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1584 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_properties_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1285 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_properties_profile_item.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1871 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_schema_public.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1149 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_status.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1292 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_status_policy_rule_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2895 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_type.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1646 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_type_condition.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      899 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/user_verification_enum.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2334 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/verification_method.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2645 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/verify_factor_request.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2153 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/verify_user_factor_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1883 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/web_authn_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1556 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/web_authn_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1834 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/web_user_factor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1319 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/web_user_factor_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2184 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/ws_federation_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1948 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/ws_federation_application_settings.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3702 2023-07-26 15:09:45.000000 okta-2.9.5/okta/models/ws_federation_application_settings_application.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3219 2023-12-15 20:32:20.000000 okta-2.9.5/okta/oauth.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      559 2023-07-26 15:09:45.000000 okta-2.9.5/okta/okta_collection.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1133 2023-07-26 15:09:45.000000 okta-2.9.5/okta/okta_object.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14815 2023-07-26 15:09:45.000000 okta-2.9.5/okta/request_executor.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.445982 okta-2.9.5/okta/resource_clients/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/__init__.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    69769 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/application_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8451 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/authenticator_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    48673 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/authorization_server_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    31436 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/brand_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7393 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/domain_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9726 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/event_hook_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6809 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/feature_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    35516 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/group_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3320 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/group_schema_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    38911 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/identity_provider_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11226 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/inline_hook_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5396 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/linked_object_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2704 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/log_event_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9428 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/network_zone_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21125 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/org_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17185 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/policy_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5166 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/profile_mapping_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5600 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/session_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8523 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/sms_template_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8827 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/subscription_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3534 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/threat_insight_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9257 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/trusted_origin_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    71332 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/user_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13729 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/user_factor_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5913 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/user_schema_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8256 2023-07-26 15:09:45.000000 okta-2.9.5/okta/resource_clients/user_type_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      685 2023-07-26 15:09:45.000000 okta-2.9.5/okta/user_agent.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1806 2023-07-26 15:09:45.000000 okta-2.9.5/okta/utils.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.009906 okta-2.9.5/okta.egg-info/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1326 2023-12-15 20:33:14.000000 okta-2.9.5/okta.egg-info/PKG-INFO
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    46372 2023-12-15 20:33:14.000000 okta-2.9.5/okta.egg-info/SOURCES.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2023-12-15 20:33:14.000000 okta-2.9.5/okta.egg-info/dependency_links.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       86 2023-12-15 20:33:14.000000 okta-2.9.5/okta.egg-info/requires.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        5 2023-12-15 20:33:14.000000 okta-2.9.5/okta.egg-info/top_level.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      190 2023-08-24 13:16:58.000000 okta-2.9.5/requirements.txt
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      105 2023-12-15 20:33:15.714028 okta-2.9.5/setup.cfg
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1546 2023-08-24 13:16:58.000000 okta-2.9.5/setup.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.449982 okta-2.9.5/tests/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      370 2023-07-26 15:09:45.000000 okta-2.9.5/tests/README.md
--rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.5/tests/__init__.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.449982 okta-2.9.5/tests/__pycache__/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      137 2023-07-26 15:13:40.000000 okta-2.9.5/tests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2950 2023-07-26 15:13:40.000000 okta-2.9.5/tests/__pycache__/conftest.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14647 2023-07-26 15:13:40.000000 okta-2.9.5/tests/__pycache__/mocks.cpython-310.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3422 2023-07-26 15:09:45.000000 okta-2.9.5/tests/conftest.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.473986 okta-2.9.5/tests/integration/
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.505992 okta-2.9.5/tests/integration/__pycache__/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)   120759 2023-07-26 15:13:40.000000 okta-2.9.5/tests/integration/__pycache__/test_applications_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    93116 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_auth_server_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8269 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_authenticators_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    29727 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_brands_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4031 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_domains_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    37171 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_event_hooks_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    33975 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_factors_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8298 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_features_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8468 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_group_schema_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    45922 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_groups_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    77148 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_identity_providers.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    27318 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_inline_hooks_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18182 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_linked_objects_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11114 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_log_events_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8022 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_network_zone_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19002 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_org_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    79164 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_policies_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8487 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_subscription_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    24441 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_templates_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3432 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_threat_insight_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15354 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_trusted_origins_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8252 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_user_schema_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17533 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_user_types_it.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    43173 2023-07-26 15:13:41.000000 okta-2.9.5/tests/integration/__pycache__/test_users_it.cpython-310-pytest-7.4.0.pyc
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:14.981901 okta-2.9.5/tests/integration/cassettes/
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.533997 okta-2.9.5/tests/integration/cassettes/test_applications_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19180 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_activate_deactivate_delete_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    31204 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_remove_assigned_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28936 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_update_assigned_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21786 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_group_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    22404 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_user_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28443 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_clone_app_key.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13742 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13906 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_three_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13600 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_basic_auth_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13372 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_bookmark_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14597 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_open_id_connect_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13938 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_secure_password_store_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18913 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_app_key.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13683 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_csr.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18771 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_app_keys.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21157 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_consent_grant.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17977 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_csr.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16053 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_default_provisioning_connection_for_application.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    42503 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_list_assign_users_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18367 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_grant_consent_to_scope.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14035 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_app_keys.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14729 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_apps.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    31455 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_assign_group_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    27322 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_remove_assign_group_app.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28599 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_consent_grant.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    23494 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_csr.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.558001 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28907 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_activate_server.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9840 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_auth_server.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18895 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_claim.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18735 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_scope.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    22760 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_auth_server_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21929 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_claim.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21769 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_scope.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19727 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_auth_server_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14405 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_created_auth_server.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13310 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_keys.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19687 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_policies.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16164 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_servers.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    31111 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_authorization_server_policy_rules.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    25723 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_claims.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    20951 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_scopes.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14004 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_rotate_auth_server_keys.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18991 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19748 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21954 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_deactivate_delete_server.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    22135 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_claim.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18749 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_scope.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.558001 okta-2.9.5/tests/integration/cassettes/test_authenticators_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14781 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_activate_and_deactivate_authenticator.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10848 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_get_authenticator.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6955 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_list_authenticators.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16495 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_update_authenticator.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.566002 okta-2.9.5/tests/integration/cassettes/test_brands_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    34541 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_create_delete_email_template_customizations.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11293 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_background_image.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11275 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_favicon.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11269 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_logo.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7191 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12586 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand_theme.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18488 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    48570 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template_customization_preview.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    35743 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_update_email_template_customization.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8067 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brand_themes.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3588 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brands.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    30926 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_template_customizations.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14258 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_templates.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15303 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    22507 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand_theme.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.570003 okta-2.9.5/tests/integration/cassettes/test_domains_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6897 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_domains_it/TestDomainResource.test_create_and_delete_domain.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10697 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_domains_it/TestDomainResource.test_get_domain.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3260 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_domains_it/TestDomainResource.test_list_domains.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.574004 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28257 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_activate_event_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13599 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_create_get_event_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17232 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_deactivate_event_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16553 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_delete_event_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    35202 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_list_event_hooks.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21033 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_update_event_hook.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.574004 okta-2.9.5/tests/integration/cassettes/test_factors_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    22639 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_delete_factor.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16879 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_enroll_sms_factor.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16947 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_get_factor.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12578 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_list_factors_new_user.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.578004 okta-2.9.5/tests/integration/cassettes/test_features_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13143 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_get_feature.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12530 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependencies.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12526 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependents.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9748 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_features.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.578004 okta-2.9.5/tests/integration/cassettes/test_group_schema_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9988 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_add_and_remove_custom_attribute.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4626 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_get_group_schema.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16854 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_update_custom_attribute.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.590006 okta-2.9.5/tests/integration/cassettes/test_groups_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12557 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_create_get_group.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    23144 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_assigned_applications.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17093 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_profile_custom_attributes.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21180 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_roles_operations.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    44512 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_rule_operations.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21706 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_add.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    37792 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_remove.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    26826 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_users_operations.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11208 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_list_groups.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    25661 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_remove_group.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9610 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_search_group.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13138 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_update_group.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.598008 okta-2.9.5/tests/integration/cassettes/test_identity_providers/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    32313 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_activate_deactivate_idp.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14827 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_facebook_idp.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15325 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_generic_idp.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14881 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_linkedin_idp.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    35993 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_clone_idp_signing_key.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12454 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_create_get_key.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18268 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_idp.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10572 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_key.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19406 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_csr.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    20302 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_idp_signing_key.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28752 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idp_signing_keys.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15389 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idps.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12519 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_keys.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    25250 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_revoke_csr.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    23772 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_update_idp.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.602008 okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    24165 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_activate_deactivate_inline_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13375 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_create_get_inline_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12762 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_delete_inline_hook.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    34340 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_list_inline_hooks.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17009 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_update_inline_hook.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.602008 okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12126 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_add_get_linked_object.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11974 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_delete_linked_object.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15004 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_get_all_linked_objects.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.606009 okta-2.9.5/tests/integration/cassettes/test_network_zone_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11032 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_create_and_delete_network_zone.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4317 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_list_network_zones.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15869 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_update_network_zone.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.610010 okta-2.9.5/tests/integration/cassettes/test_org_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10806 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_extend_okta_support.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3437 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_communication_settings.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3434 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_support_settings.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3479 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_types.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3390 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3420 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_preferences.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4103 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_settings.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7001 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_grant_revoke_okta_support.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3458 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_hide_okta_ui_footer.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3704 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_in_users_to_okta_communication_emails.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3452 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_out_users_from_okta_communication_emails.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12329 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_partial_setting_update.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13929 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_setting_update.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3457 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_show_okta_ui_footer.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10188 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_update_org_contact_user.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.618011 okta-2.9.5/tests/integration/cassettes/test_policies_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14878 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    28875 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy_rule.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16587 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_password_policy_rule.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9554 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9554 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16085 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_rule.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15638 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_with_group_conditions.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11042 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_password_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12503 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19092 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy_rules.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    22722 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policies_by_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16045 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policy_rules.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16527 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    23462 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy_rule.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.622012 okta-2.9.5/tests/integration/cassettes/test_subscription_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3664 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_get_role_subscription_by_notification_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7237 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_list_role_subsription.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16959 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_role_by_notification_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    20527 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_user.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.622012 okta-2.9.5/tests/integration/cassettes/test_templates_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9200 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_get_sms_template.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9388 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_list_sms_templates.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12164 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_delete_sms_template.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15906 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_partial_update_sms_template.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15793 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_update_sms_template.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.626013 okta-2.9.5/tests/integration/cassettes/test_threat_insight_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3535 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_get_threat_insight_configuration.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11009 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_update_threat_insight_configuration.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.630013 okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19424 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_activate_deactivate_origin.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9310 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_create_get_origin.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12278 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_delete_origin.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9922 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_list_origins.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16015 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_update_origin.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.642016 okta-2.9.5/tests/integration/cassettes/test_user_schema_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10039 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_get_user_schema.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    44389 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_update_user_profile.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.658018 okta-2.9.5/tests/integration/cassettes/test_user_types_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5948 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_create_user_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12230 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_delete_user_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9266 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_get_user_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16249 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_list_user_types.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12626 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_replace_user_type.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12623 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_update_user_type.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.658018 okta-2.9.5/tests/integration/cassettes/test_users_it/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17114 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_activate_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    21149 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_assign_user_to_role.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    20238 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_recovery_question.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16924 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_user_password.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19345 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_create_get_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12540 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_expire_password_get_temporary.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    12585 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_get_reset_password_link_for_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    14147 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_list_user_subscriptions.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    24049 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_suspend_user.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    16513 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_update_user_profile.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    36853 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_group_target_to_role.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    27965 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_pagination.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.666020 okta-2.9.5/tests/integration/data/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7486 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/data/brand_theme_background.png
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5430 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/data/brand_theme_favicon.ico
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8541 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/data/brand_theme_logo.png
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2284 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/data/logo.png
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    82009 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_applications_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    60958 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_auth_server_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2853 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_authenticators_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    19405 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_brands_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1651 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_domains_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    23537 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_event_hooks_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18410 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_factors_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3747 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_features_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4193 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_group_schema_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    30837 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_groups_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    69374 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_identity_providers.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    17569 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_inline_hooks_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11114 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_linked_objects_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6139 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_log_events_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4077 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_network_zone_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9379 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_org_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    43729 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_policies_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3795 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_subscription_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    13343 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_templates_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1194 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_threat_insight_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9807 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_trusted_origins_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3380 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_user_schema_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    10187 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_user_types_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    32137 2023-07-26 15:09:45.000000 okta-2.9.5/tests/integration/test_users_it.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15503 2023-07-26 15:09:45.000000 okta-2.9.5/tests/mocks.py
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.686023 okta-2.9.5/tests/unit/
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.694024 okta-2.9.5/tests/unit/__pycache__/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5981 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_api_response.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    18350 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_applications_ut.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9280 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_cache.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    41450 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_client.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1282 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_constants.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11067 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_domains.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3506 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_helpers.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    15459 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_http_client.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1875 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_jwt.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     2331 2023-07-26 15:13:41.000000 okta-2.9.5/tests/unit/__pycache__/test_logger.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3185 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_models.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3254 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_oauth.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     7066 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_request_executor.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9109 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_retry_logic.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9632 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_sign_on_modes.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5042 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_user_profile.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11608 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_user_schema.cpython-310-pytest-7.4.0.pyc
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1312 2023-07-26 15:13:42.000000 okta-2.9.5/tests/unit/__pycache__/test_utils.cpython-310-pytest-7.4.0.pyc
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.706026 okta-2.9.5/tests/unit/cassettes/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)   199562 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_client_error_call_SSWS.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)   199566 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_client_error_call_oauth.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5127 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_client_success_call_SSWS.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_create_group_different_inputs[group_obj0].yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_create_group_different_inputs[group_obj1].yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_create_group_different_inputs[group_obj2].yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.710027 okta-2.9.5/tests/unit/cassettes/test_http_client/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)   199564 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_error_call_SSWS.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)   199568 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_error_call_oauth.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5143 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_success_call_SSWS.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5131 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_success_call_oauth.yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.710027 okta-2.9.5/tests/unit/cassettes/test_models/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj0].yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj1].yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj2].yaml
-drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2023-12-15 20:33:15.710027 okta-2.9.5/tests/unit/files/
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      206 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/files/PK-sample-global.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      202 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/files/PK-sample-local.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       86 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/files/SSWS-sample-global.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)       84 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/files/SSWS-sample-local.yaml
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3781 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_api_response.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    11054 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_applications_ut.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     3342 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_cache.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)    31686 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      460 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_constants.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     8075 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_domains.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      985 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_helpers.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9053 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_http_client.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      902 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_jwt.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1086 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_logger.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1958 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_models.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1040 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_oauth.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      775 2023-12-15 20:32:20.000000 okta-2.9.5/tests/unit/test_oauth_clear_access_token.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5272 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_request_executor.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     5700 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_retry_logic.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     9287 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_sign_on_modes.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     1902 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_user_profile.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)     4490 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_user_schema.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      488 2023-07-26 15:09:45.000000 okta-2.9.5/tests/unit/test_utils.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      376 2023-07-26 15:09:45.000000 okta-2.9.5/tests/utils.py
--rw-rw-r--   0 bryan     (1000) bryan     (1000)      654 2023-07-26 15:09:45.000000 okta-2.9.5/tox.ini
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.603728 okta-2.9.6/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    25789 2023-12-15 20:32:20.000000 okta-2.9.6/CHANGELOG.md
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9809 2023-07-26 15:09:45.000000 okta-2.9.6/LICENSE.md
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      554 2023-07-26 15:09:45.000000 okta-2.9.6/LONG_DESCRIPTION.md
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      112 2023-07-26 15:09:45.000000 okta-2.9.6/MANIFEST.in
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1326 2024-05-03 18:15:44.607728 okta-2.9.6/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    38660 2023-12-13 16:09:31.000000 okta-2.9.6/README.md
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.223720 okta-2.9.6/okta/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       22 2024-05-03 16:12:28.000000 okta-2.9.6/okta/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      726 2023-07-26 15:09:45.000000 okta-2.9.6/okta/api_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6004 2023-12-13 16:09:31.000000 okta-2.9.6/okta/api_response.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.223720 okta-2.9.6/okta/cache/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.6/okta/cache/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2418 2023-07-26 15:09:45.000000 okta-2.9.6/okta/cache/cache.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1262 2023-07-26 15:09:45.000000 okta-2.9.6/okta/cache/no_op_cache.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4366 2023-07-26 15:09:45.000000 okta-2.9.6/okta/cache/okta_cache.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6758 2023-07-26 15:09:45.000000 okta-2.9.6/okta/client.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.227720 okta-2.9.6/okta/config/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.6/okta/config/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6456 2023-07-26 15:09:45.000000 okta-2.9.6/okta/config/config_setter.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6647 2023-07-26 15:09:45.000000 okta-2.9.6/okta/config/config_validator.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3538 2023-07-26 15:09:45.000000 okta-2.9.6/okta/constants.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2570 2023-07-26 15:09:45.000000 okta-2.9.6/okta/error_messages.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.227720 okta-2.9.6/okta/errors/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.6/okta/errors/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      194 2023-07-26 15:09:45.000000 okta-2.9.6/okta/errors/error.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      335 2023-07-26 15:09:45.000000 okta-2.9.6/okta/errors/http_error.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      904 2023-07-26 15:09:45.000000 okta-2.9.6/okta/errors/okta_api_error.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.231720 okta-2.9.6/okta/exceptions/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       65 2023-07-26 15:09:45.000000 okta-2.9.6/okta/exceptions/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      150 2023-07-26 15:09:45.000000 okta-2.9.6/okta/exceptions/exceptions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1076 2023-07-26 15:09:45.000000 okta-2.9.6/okta/helpers.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6776 2023-07-26 15:09:45.000000 okta-2.9.6/okta/http_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4767 2023-07-26 15:09:45.000000 okta-2.9.6/okta/jwt.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      510 2023-07-26 15:09:45.000000 okta-2.9.6/okta/logger.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.391723 okta-2.9.6/okta/models/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    71986 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1133 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1865 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_constraint.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2520 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_constraints.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2756 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1961 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_rule_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2101 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_rule_application_sign_on.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3386 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_rule_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1320 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/access_policy_rule_custom_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1396 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/acs_endpoint.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2076 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/activate_factor_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      918 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/allowed_for_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1598 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_and_instance_condition_evaluator_app_or_instance.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2006 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_and_instance_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1672 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_instance_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2865 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_link.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4128 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_user.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2010 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_user_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1284 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/app_user_password_credential.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7225 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1769 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_accessibility.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2758 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2916 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_credentials_o_auth_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1254 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_credentials_scheme.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2574 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_credentials_signing.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      867 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_credentials_signing_use.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1817 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_credentials_username_template.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3026 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_feature.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2198 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_group_assignment.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1301 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_licensing.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3728 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2413 2023-08-24 13:16:58.000000 okta-2.9.6/okta/models/application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1446 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_settings_notes.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1865 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_settings_notifications.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2296 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_settings_notifications_vpn.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1878 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_settings_notifications_vpn_network.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1419 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_sign_on_mode.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2379 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_visibility.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1415 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/application_visibility_hide.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1685 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/assign_role_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1953 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authentication_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1054 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authentication_provider_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4773 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2099 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3379 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator_provider_configuration.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1346 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator_provider_configuration_user_name_plate.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4439 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      888 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1089 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authenticator_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3924 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1961 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      922 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_credentials_rotation_mode.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3298 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_credentials_signing_config.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      869 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_credentials_use.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4136 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4025 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_policy_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1935 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_policy_rule_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4078 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/authorization_server_policy_rule_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2756 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/auto_login_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1940 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/auto_login_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1514 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/auto_login_application_settings_sign_on.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1888 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/basic_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1532 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/basic_application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2908 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/basic_auth_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2594 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/before_scheduled_action_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2131 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/bookmark_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1912 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/bookmark_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1604 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/bookmark_application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2258 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/brand.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2031 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/browser_plugin_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1843 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/call_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1524 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/call_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1957 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/capabilities_create_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2488 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/capabilities_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3393 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/capabilities_update_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4028 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/catalog_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      898 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/catalog_application_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      885 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/change_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2474 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/change_password_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1903 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/channel_binding.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1413 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/client_policy_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2371 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/client_secret.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1320 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/client_secret_metadata.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1671 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/compliance.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1316 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/context_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1319 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/create_session_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3277 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/create_user_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1666 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/csr.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2590 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/csr_metadata.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2417 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/csr_metadata_subject.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1432 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/csr_metadata_subject_alt_names.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2119 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/custom_hotp_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1333 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/custom_hotp_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1549 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/device_access_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2416 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/device_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1762 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/device_policy_rule_condition_platform.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2392 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/dns_record.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      858 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/dns_record_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4310 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2361 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain_certificate.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1666 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain_certificate_metadata.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      916 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain_certificate_source_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      845 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain_certificate_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1463 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain_list_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1109 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/domain_validation_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1402 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/duration.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1488 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_template.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2030 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_template_content.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2516 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_template_customization.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1807 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_template_customization_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1345 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_template_test_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      934 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_template_touch_point_variant.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1852 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1278 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/email_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      879 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/enabled_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1118 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/end_user_dashboard_touch_point_variant.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1036 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/error_page_touch_point_variant.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3833 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_hook.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2101 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_hook_channel.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2510 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_hook_channel_config.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2195 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_hook_channel_config_auth_scheme.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_hook_channel_config_auth_scheme_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1430 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_hook_channel_config_header.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1541 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/event_subscriptions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1069 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/factor_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1237 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/factor_result_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1094 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/factor_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1304 2023-08-24 13:16:58.000000 okta-2.9.6/okta/models/factor_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3605 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/feature.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2384 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/feature_stage.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      872 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/feature_stage_state.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      860 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/feature_stage_value.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      852 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/feature_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      872 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/fips_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1350 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/forgot_password_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1427 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/grant_type_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3752 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1640 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1660 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3131 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3866 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1963 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_action.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2512 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1418 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_expression.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1428 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_group_assignment.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1658 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_group_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2478 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_people_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      915 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1656 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_rule_user_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4144 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_schema.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7221 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_schema_attribute.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2430 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_schema_base.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2412 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_schema_base_properties.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1873 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_schema_custom.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2376 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_schema_definitions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      921 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/group_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1885 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/hardware_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1329 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/hardware_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3750 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2387 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_application_user.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3365 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1520 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_credentials_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1636 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_credentials_signing.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2062 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_credentials_trust.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3437 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1608 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/identity_provider_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1573 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/idp_policy_rule_action.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1416 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/idp_policy_rule_action_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/iframe_embed_scope_allowed_apps.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1260 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/image_upload_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1444 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inactivity_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4044 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2109 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_channel.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2684 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_channel_config.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1586 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_channel_config_auth_scheme.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1434 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_channel_config_headers.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1097 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_payload.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1558 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1574 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_response_command_value.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1721 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_response_commands.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      882 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1350 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/inline_hook_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2905 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/ion_field.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2861 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/ion_form.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3823 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/json_web_key.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1234 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/jwk_use.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1150 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/knowledge_constraint.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1761 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/lifecycle_create_setting_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1769 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/lifecycle_deactivate_setting_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1677 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/lifecycle_expiration_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2634 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/linked_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2273 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/linked_object_details.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      852 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/linked_object_details_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1918 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_actor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4835 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_authentication_context.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1151 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_authentication_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3207 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1186 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_credential_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1047 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_credential_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1291 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_debug_context.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8585 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_event.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2454 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_geographical_context.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1390 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_geolocation.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2397 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_ip_address.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1380 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_issuer.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1418 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_outcome.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1480 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1911 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_security_context.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      912 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_severity.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1953 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_target.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1548 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_transaction.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1604 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/log_user_agent.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1573 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/mdm_enrollment_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1163 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/multifactor_enrollment_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2309 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/multifactor_enrollment_policy_authenticator_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      995 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/multifactor_enrollment_policy_authenticator_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1558 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/multifactor_enrollment_policy_authenticator_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2486 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/multifactor_enrollment_policy_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      914 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/multifactor_enrollment_policy_settings_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5481 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1931 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone_address.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      879 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone_address_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1442 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone_location.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      865 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      885 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/network_zone_usage.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1487 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/notification_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1384 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_actor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3638 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_claim.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1407 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_claim_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2048 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3777 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_refresh_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2464 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_scope.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4812 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_scope_consent_grant.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      905 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_scope_consent_grant_source.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      905 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_scope_consent_grant_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1451 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_scopes_mediation_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3110 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_2_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1997 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_application_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1157 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_authorization_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1135 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_endpoint_authentication_method.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1487 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_grant_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      907 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/o_auth_response_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1964 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1844 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2822 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1925 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy_rule_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3332 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy_rule_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3028 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy_rule_signon_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1936 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/okta_sign_on_policy_rule_signon_session_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2958 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      927 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_consent_method.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1633 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_idp_initiated_login.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      962 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_issuer_mode.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2032 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8880 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_settings_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1515 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_settings_client_keys.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2194 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_settings_refresh_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      961 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_application_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      918 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/open_id_connect_refresh_token_rotation_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2040 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_2_org_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1877 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_2_org_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1750 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_2_org_application_settings_app.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      884 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_contact_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2049 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_contact_type_obj.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1505 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_contact_user.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1597 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_okta_communication_setting.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      895 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_okta_support_setting.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2239 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_okta_support_settings_obj.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1577 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_preferences.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4373 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/org_setting.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2568 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_credential.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2563 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_credential_hash.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      997 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_credential_hash_algorithm.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1272 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_credential_hook.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1803 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_dictionary.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1296 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_dictionary_common.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1460 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_expiration_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2633 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1631 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_authentication_provider_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2737 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1941 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_delegation_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1345 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_delegation_settings_options.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3473 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_password_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1927 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_password_settings_age.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3328 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_password_settings_complexity.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2261 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_password_settings_lockout.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2113 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_email.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2039 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_email_properties.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1412 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_email_recovery_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1324 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_factor_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4208 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_factors.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2137 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_question.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1341 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_question_complexity.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1999 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_question_properties.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1873 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_recovery_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2779 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1288 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_rule_action.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3537 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_rule_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2533 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_rule_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3409 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_policy_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2921 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/password_setting_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2095 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/platform_condition_evaluator_platform.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2413 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/platform_condition_evaluator_platform_operating_system.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1525 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/platform_condition_evaluator_platform_operating_system_version.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1912 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/platform_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4098 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1957 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_account_link.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1851 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_account_link_filter.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1429 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_account_link_filter_groups.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1838 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_network_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2348 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_people_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3743 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5548 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_rule_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1823 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_rule_actions_enroll.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      933 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_rule_actions_enroll_self.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1315 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_rule_auth_context_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17081 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_rule_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3294 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_subject.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1018 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_subject_match_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1198 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1296 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/policy_user_name_template.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2019 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/possession_constraint.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1332 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/pre_registration_inline_hook.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1155 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_enrollment_policy.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2104 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_enrollment_policy_rule.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4128 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_enrollment_policy_rule_action.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2069 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_enrollment_policy_rule_actions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1405 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_enrollment_policy_rule_activation_requirement.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1636 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_enrollment_policy_rule_profile_attribute.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2904 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_mapping.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2111 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_mapping_property.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      911 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_mapping_property_push_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1782 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_mapping_source.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1745 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/profile_setting_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5651 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1885 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_algorithm_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1470 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_algorithm_type_signature.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2408 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_algorithms.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1752 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_endpoint.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5698 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_endpoints.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1815 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_relay_state.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      898 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_relay_state_format.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1299 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/protocol_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2829 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2712 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_conditions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2876 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_connection.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      908 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_connection_auth_scheme.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2091 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_connection_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1867 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_connection_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      944 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_connection_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1308 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_deprovisioned_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2066 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_groups.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1300 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/provisioning_suspended_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2745 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/push_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2177 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/push_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1462 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/recovery_question_credential.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      921 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/required_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1342 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/reset_password_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1342 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/response_links.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1429 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/risk_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1290 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/risk_score_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4257 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/role.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      871 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/role_assignment_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      870 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/role_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1394 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/role_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1941 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/saml_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1896 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/saml_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8478 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/saml_application_settings_sign_on.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2253 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/saml_attribute_statement.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1296 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/scheduled_user_lifecycle_action.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3681 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/scheme_application_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2353 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/scope.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      912 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/scope_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3017 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/secure_password_store_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2008 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/secure_password_store_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3170 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/secure_password_store_application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1639 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/security_question.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1947 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/security_question_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1673 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/security_question_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      854 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/seed_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4344 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/session.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1107 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/session_authentication_method.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1953 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/session_identity_provider.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1024 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/session_identity_provider_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      932 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/session_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1038 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sign_in_page_touch_point_variant.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1248 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sign_on_inline_hook.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1607 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/single_logout.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3275 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sms_template.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1203 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sms_template_translations.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      869 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sms_template_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1834 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sms_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1313 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sms_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2257 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/social_auth_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1379 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/sp_certificate.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3055 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/subscription.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      910 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/subscription_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2028 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/swa_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1872 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/swa_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2525 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/swa_application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2128 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/swa_three_field_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1960 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/swa_three_field_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2734 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/swa_three_field_application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1303 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/temp_password.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6683 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/theme.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7143 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/theme_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2203 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/threat_insight_configuration.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2938 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/token_authorization_server_policy_rule_action.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1316 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/token_authorization_server_policy_rule_action_inline_hook.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1852 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/token_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1323 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/token_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1858 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/totp_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1321 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/totp_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3013 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/trusted_origin.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1842 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/u_2_f_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1319 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/u_2_f_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5966 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1538 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_activation_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1638 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3298 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_credentials.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4580 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1292 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_id_string.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1491 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_identifier_condition_evaluator_pattern.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1965 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_identifier_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1329 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_identity_provider_link_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1570 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_lifecycle_attribute_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      863 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_next_login.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5288 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9044 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3948 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7383 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1432 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1912 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_items.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2310 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_master.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1446 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_master_priority.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      958 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_master_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1474 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_permission.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      880 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_scope.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      989 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      895 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_attribute_union.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2422 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_base.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    20607 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_base_properties.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2362 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_definitions.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1841 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_properties.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1584 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_properties_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1285 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_properties_profile_item.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1871 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_schema_public.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1149 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_status.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1292 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_status_policy_rule_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2895 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_type.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1646 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_type_condition.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      899 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/user_verification_enum.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2334 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/verification_method.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2645 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/verify_factor_request.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2153 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/verify_user_factor_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1883 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/web_authn_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1556 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/web_authn_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1834 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/web_user_factor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1319 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/web_user_factor_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2184 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/ws_federation_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1948 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/ws_federation_application_settings.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3702 2023-07-26 15:09:45.000000 okta-2.9.6/okta/models/ws_federation_application_settings_application.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3219 2023-12-15 20:32:20.000000 okta-2.9.6/okta/oauth.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      559 2023-07-26 15:09:45.000000 okta-2.9.6/okta/okta_collection.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1133 2023-07-26 15:09:45.000000 okta-2.9.6/okta/okta_object.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14815 2023-07-26 15:09:45.000000 okta-2.9.6/okta/request_executor.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.403724 okta-2.9.6/okta/resource_clients/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/__init__.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    69769 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/application_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8451 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/authenticator_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    48673 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/authorization_server_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    31436 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/brand_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7393 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/domain_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9726 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/event_hook_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6809 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/feature_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    35516 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/group_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3320 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/group_schema_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    38911 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/identity_provider_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11226 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/inline_hook_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5396 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/linked_object_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2704 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/log_event_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9428 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/network_zone_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21125 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/org_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17185 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/policy_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5166 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/profile_mapping_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5600 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/session_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8523 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/sms_template_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8827 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/subscription_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3534 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/threat_insight_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9257 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/trusted_origin_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    71332 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/user_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13729 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/user_factor_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5913 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/user_schema_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8256 2023-07-26 15:09:45.000000 okta-2.9.6/okta/resource_clients/user_type_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      685 2023-07-26 15:09:45.000000 okta-2.9.6/okta/user_agent.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1806 2023-07-26 15:09:45.000000 okta-2.9.6/okta/utils.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.223720 okta-2.9.6/okta.egg-info/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1326 2024-05-03 18:15:44.000000 okta-2.9.6/okta.egg-info/PKG-INFO
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    46372 2024-05-03 18:15:44.000000 okta-2.9.6/okta.egg-info/SOURCES.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        1 2024-05-03 18:15:44.000000 okta-2.9.6/okta.egg-info/dependency_links.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       86 2024-05-03 18:15:44.000000 okta-2.9.6/okta.egg-info/requires.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        5 2024-05-03 18:15:44.000000 okta-2.9.6/okta.egg-info/top_level.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      215 2024-04-16 22:10:15.000000 okta-2.9.6/requirements.txt
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      105 2024-05-03 18:15:44.607728 okta-2.9.6/setup.cfg
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1546 2023-08-24 13:16:58.000000 okta-2.9.6/setup.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.403724 okta-2.9.6/tests/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      370 2023-07-26 15:09:45.000000 okta-2.9.6/tests/README.md
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)        0 2023-07-26 15:09:45.000000 okta-2.9.6/tests/__init__.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.403724 okta-2.9.6/tests/__pycache__/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      137 2023-07-26 15:13:40.000000 okta-2.9.6/tests/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2950 2023-07-26 15:13:40.000000 okta-2.9.6/tests/__pycache__/conftest.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14647 2023-07-26 15:13:40.000000 okta-2.9.6/tests/__pycache__/mocks.cpython-310.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3422 2023-07-26 15:09:45.000000 okta-2.9.6/tests/conftest.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.411724 okta-2.9.6/tests/integration/
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.427724 okta-2.9.6/tests/integration/__pycache__/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)   120759 2023-07-26 15:13:40.000000 okta-2.9.6/tests/integration/__pycache__/test_applications_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    93116 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_auth_server_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8269 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_authenticators_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    29727 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_brands_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4031 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_domains_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    37171 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_event_hooks_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    33975 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_factors_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8298 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_features_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8468 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_group_schema_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    45922 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_groups_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    77148 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_identity_providers.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    27318 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_inline_hooks_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18182 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_linked_objects_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11114 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_log_events_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8022 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_network_zone_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19002 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_org_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    79164 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_policies_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8487 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_subscription_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    24441 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_templates_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3432 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_threat_insight_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15354 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_trusted_origins_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8252 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_user_schema_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17533 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_user_types_it.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    43173 2023-07-26 15:13:41.000000 okta-2.9.6/tests/integration/__pycache__/test_users_it.cpython-310-pytest-7.4.0.pyc
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.207720 okta-2.9.6/tests/integration/cassettes/
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.443724 okta-2.9.6/tests/integration/cassettes/test_applications_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19180 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_activate_deactivate_delete_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    31204 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_remove_assigned_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28936 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_update_assigned_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21786 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_group_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    22404 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_user_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28443 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_clone_app_key.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13742 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13906 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_three_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13600 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_basic_auth_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13372 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_bookmark_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14597 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_open_id_connect_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13938 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_secure_password_store_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18913 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_app_key.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13683 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_csr.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18771 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_app_keys.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21157 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_consent_grant.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17977 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_csr.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16053 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_default_provisioning_connection_for_application.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    42503 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_list_assign_users_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18367 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_grant_consent_to_scope.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14035 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_app_keys.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14729 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_apps.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    31455 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_assign_group_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    27322 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_remove_assign_group_app.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28599 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_consent_grant.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    23494 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_csr.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.467725 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28907 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_activate_server.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9840 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_auth_server.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18895 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_claim.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18735 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_scope.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    22760 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_auth_server_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21929 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_claim.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21769 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_scope.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19727 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_auth_server_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14405 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_created_auth_server.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13310 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_keys.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19687 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_policies.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16164 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_servers.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    31111 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_authorization_server_policy_rules.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    25723 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_claims.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    20951 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_scopes.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14004 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_rotate_auth_server_keys.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18991 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19748 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21954 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_deactivate_delete_server.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    22135 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_claim.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18749 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_scope.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.471725 okta-2.9.6/tests/integration/cassettes/test_authenticators_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14781 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_activate_and_deactivate_authenticator.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10848 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_get_authenticator.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6955 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_list_authenticators.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16495 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_update_authenticator.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.491725 okta-2.9.6/tests/integration/cassettes/test_brands_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    34541 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_create_delete_email_template_customizations.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11293 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_background_image.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11275 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_favicon.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11269 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_logo.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7191 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12586 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand_theme.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18488 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    48570 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template_customization_preview.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    35743 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_update_email_template_customization.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8067 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brand_themes.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3588 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brands.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    30926 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_template_customizations.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14258 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_templates.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15303 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    22507 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand_theme.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.495725 okta-2.9.6/tests/integration/cassettes/test_domains_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6897 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_domains_it/TestDomainResource.test_create_and_delete_domain.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10697 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_domains_it/TestDomainResource.test_get_domain.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3260 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_domains_it/TestDomainResource.test_list_domains.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.499725 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28257 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_activate_event_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13599 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_create_get_event_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17232 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_deactivate_event_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16553 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_delete_event_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    35202 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_list_event_hooks.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21033 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_update_event_hook.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.499725 okta-2.9.6/tests/integration/cassettes/test_factors_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    22639 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_delete_factor.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16879 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_enroll_sms_factor.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16947 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_get_factor.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12578 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_list_factors_new_user.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.503726 okta-2.9.6/tests/integration/cassettes/test_features_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13143 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_get_feature.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12530 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependencies.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12526 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependents.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9748 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_features.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.503726 okta-2.9.6/tests/integration/cassettes/test_group_schema_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9988 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_add_and_remove_custom_attribute.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4626 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_get_group_schema.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16854 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_update_custom_attribute.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.507726 okta-2.9.6/tests/integration/cassettes/test_groups_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12557 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_create_get_group.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    23144 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_assigned_applications.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17093 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_profile_custom_attributes.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21180 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_roles_operations.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    44512 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_rule_operations.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21706 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_add.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    37792 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_remove.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    26826 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_users_operations.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11208 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_list_groups.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    25661 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_remove_group.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9610 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_search_group.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13138 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_update_group.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.519726 okta-2.9.6/tests/integration/cassettes/test_identity_providers/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    32313 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_activate_deactivate_idp.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14827 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_facebook_idp.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15325 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_generic_idp.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14881 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_linkedin_idp.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    35993 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_clone_idp_signing_key.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12454 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_create_get_key.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18268 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_idp.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10572 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_key.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19406 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_csr.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    20302 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_idp_signing_key.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28752 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idp_signing_keys.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15389 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idps.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12519 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_keys.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    25250 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_revoke_csr.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    23772 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_update_idp.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.519726 okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    24165 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_activate_deactivate_inline_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13375 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_create_get_inline_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12762 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_delete_inline_hook.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    34340 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_list_inline_hooks.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17009 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_update_inline_hook.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.523726 okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12126 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_add_get_linked_object.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11974 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_delete_linked_object.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15004 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_get_all_linked_objects.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.523726 okta-2.9.6/tests/integration/cassettes/test_network_zone_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11032 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_create_and_delete_network_zone.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4317 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_list_network_zones.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15869 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_update_network_zone.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.523726 okta-2.9.6/tests/integration/cassettes/test_org_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10806 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_extend_okta_support.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3437 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_communication_settings.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3434 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_support_settings.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3479 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_types.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3390 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3420 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_preferences.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4103 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_settings.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7001 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_grant_revoke_okta_support.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3458 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_hide_okta_ui_footer.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3704 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_in_users_to_okta_communication_emails.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3452 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_out_users_from_okta_communication_emails.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12329 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_partial_setting_update.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13929 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_setting_update.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3457 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_show_okta_ui_footer.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10188 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_update_org_contact_user.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.535726 okta-2.9.6/tests/integration/cassettes/test_policies_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14878 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    28875 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy_rule.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16587 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_password_policy_rule.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9554 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9554 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16085 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_rule.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15638 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_with_group_conditions.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11042 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_password_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12503 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19092 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy_rules.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    22722 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policies_by_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16045 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policy_rules.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16527 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    23462 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy_rule.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.535726 okta-2.9.6/tests/integration/cassettes/test_subscription_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3664 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_get_role_subscription_by_notification_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7237 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_list_role_subsription.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16959 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_role_by_notification_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    20527 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_user.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.535726 okta-2.9.6/tests/integration/cassettes/test_templates_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9200 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_get_sms_template.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9388 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_list_sms_templates.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12164 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_delete_sms_template.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15906 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_partial_update_sms_template.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15793 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_update_sms_template.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.539726 okta-2.9.6/tests/integration/cassettes/test_threat_insight_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3535 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_get_threat_insight_configuration.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11009 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_update_threat_insight_configuration.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.551726 okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19424 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_activate_deactivate_origin.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9310 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_create_get_origin.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12278 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_delete_origin.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9922 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_list_origins.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16015 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_update_origin.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.551726 okta-2.9.6/tests/integration/cassettes/test_user_schema_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10039 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_get_user_schema.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    44389 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_update_user_profile.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.551726 okta-2.9.6/tests/integration/cassettes/test_user_types_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5948 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_create_user_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12230 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_delete_user_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9266 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_get_user_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16249 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_list_user_types.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12626 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_replace_user_type.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12623 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_update_user_type.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.551726 okta-2.9.6/tests/integration/cassettes/test_users_it/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17114 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_activate_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    21149 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_assign_user_to_role.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    20238 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_recovery_question.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16924 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_user_password.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19345 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_create_get_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12540 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_expire_password_get_temporary.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    12585 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_get_reset_password_link_for_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    14147 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_list_user_subscriptions.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    24049 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_suspend_user.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    16513 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_update_user_profile.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    36853 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_group_target_to_role.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    27965 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_pagination.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.563727 okta-2.9.6/tests/integration/data/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7486 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/data/brand_theme_background.png
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5430 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/data/brand_theme_favicon.ico
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8541 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/data/brand_theme_logo.png
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2284 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/data/logo.png
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    82009 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_applications_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    60958 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_auth_server_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2853 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_authenticators_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    19405 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_brands_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1651 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_domains_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    23537 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_event_hooks_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18410 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_factors_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3747 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_features_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4193 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_group_schema_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    30837 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_groups_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    69374 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_identity_providers.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    17569 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_inline_hooks_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11114 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_linked_objects_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6139 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_log_events_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4077 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_network_zone_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9379 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_org_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    43729 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_policies_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3795 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_subscription_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    13343 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_templates_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1194 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_threat_insight_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9807 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_trusted_origins_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3380 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_user_schema_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    10187 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_user_types_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    32137 2023-07-26 15:09:45.000000 okta-2.9.6/tests/integration/test_users_it.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15503 2023-07-26 15:09:45.000000 okta-2.9.6/tests/mocks.py
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.571727 okta-2.9.6/tests/unit/
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.575727 okta-2.9.6/tests/unit/__pycache__/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5981 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_api_response.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    18350 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_applications_ut.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9280 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_cache.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    41450 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_client.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1282 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_constants.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11067 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_domains.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3506 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_helpers.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    15459 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_http_client.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1875 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_jwt.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     2331 2023-07-26 15:13:41.000000 okta-2.9.6/tests/unit/__pycache__/test_logger.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3185 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_models.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3254 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_oauth.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     7066 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_request_executor.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9109 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_retry_logic.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9632 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_sign_on_modes.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5042 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_user_profile.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11608 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_user_schema.cpython-310-pytest-7.4.0.pyc
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1312 2023-07-26 15:13:42.000000 okta-2.9.6/tests/unit/__pycache__/test_utils.cpython-310-pytest-7.4.0.pyc
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.591727 okta-2.9.6/tests/unit/cassettes/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)   199562 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_client_error_call_SSWS.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)   199566 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_client_error_call_oauth.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5127 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_client_success_call_SSWS.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_create_group_different_inputs[group_obj0].yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_create_group_different_inputs[group_obj1].yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_create_group_different_inputs[group_obj2].yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.595727 okta-2.9.6/tests/unit/cassettes/test_http_client/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)   199564 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_error_call_SSWS.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)   199568 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_error_call_oauth.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5143 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_success_call_SSWS.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5131 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_success_call_oauth.yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.595727 okta-2.9.6/tests/unit/cassettes/test_models/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj0].yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj1].yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     6124 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj2].yaml
+drwxrwxr-x   0 bryan     (1000) bryan     (1000)        0 2024-05-03 18:15:44.603728 okta-2.9.6/tests/unit/files/
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      206 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/files/PK-sample-global.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      202 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/files/PK-sample-local.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       86 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/files/SSWS-sample-global.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)       84 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/files/SSWS-sample-local.yaml
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3781 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_api_response.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    11054 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_applications_ut.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     3342 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_cache.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)    31686 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      460 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_constants.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     8075 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_domains.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      985 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_helpers.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9053 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_http_client.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      902 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_jwt.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1086 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_logger.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1958 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_models.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1040 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_oauth.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      775 2023-12-15 20:32:20.000000 okta-2.9.6/tests/unit/test_oauth_clear_access_token.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5272 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_request_executor.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     5700 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_retry_logic.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     9287 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_sign_on_modes.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     1902 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_user_profile.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)     4490 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_user_schema.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      488 2023-07-26 15:09:45.000000 okta-2.9.6/tests/unit/test_utils.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      376 2023-07-26 15:09:45.000000 okta-2.9.6/tests/utils.py
+-rw-rw-r--   0 bryan     (1000) bryan     (1000)      654 2023-07-26 15:09:45.000000 okta-2.9.6/tox.ini
```

### Comparing `okta-2.9.5/CHANGELOG.md` & `okta-2.9.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/LICENSE.md` & `okta-2.9.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/LONG_DESCRIPTION.md` & `okta-2.9.6/LONG_DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/PKG-INFO` & `okta-2.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okta
-Version: 2.9.5
+Version: 2.9.6
 Summary: Python SDK for the Okta Management API
 Home-page: https://github.com/okta/okta-sdk-python
 Author: Okta, Inc.
 Author-email: devex@okta.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `okta-2.9.5/README.md` & `okta-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/api_client.py` & `okta-2.9.6/okta/api_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/api_response.py` & `okta-2.9.6/okta/api_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/cache/cache.py` & `okta-2.9.6/okta/cache/cache.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/cache/no_op_cache.py` & `okta-2.9.6/okta/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/cache/okta_cache.py` & `okta-2.9.6/okta/cache/okta_cache.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/client.py` & `okta-2.9.6/okta/client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/config/config_setter.py` & `okta-2.9.6/okta/config/config_setter.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/config/config_validator.py` & `okta-2.9.6/okta/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/constants.py` & `okta-2.9.6/okta/constants.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/error_messages.py` & `okta-2.9.6/okta/error_messages.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/errors/okta_api_error.py` & `okta-2.9.6/okta/errors/okta_api_error.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/helpers.py` & `okta-2.9.6/okta/helpers.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/http_client.py` & `okta-2.9.6/okta/http_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/jwt.py` & `okta-2.9.6/okta/jwt.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/__init__.py` & `okta-2.9.6/okta/models/__init__.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy.py` & `okta-2.9.6/okta/models/access_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_constraint.py` & `okta-2.9.6/okta/models/access_policy_constraint.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_constraints.py` & `okta-2.9.6/okta/models/access_policy_constraints.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_rule.py` & `okta-2.9.6/okta/models/access_policy_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_rule_actions.py` & `okta-2.9.6/okta/models/access_policy_rule_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_rule_application_sign_on.py` & `okta-2.9.6/okta/models/access_policy_rule_application_sign_on.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_rule_conditions.py` & `okta-2.9.6/okta/models/access_policy_rule_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/access_policy_rule_custom_condition.py` & `okta-2.9.6/okta/models/access_policy_rule_custom_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/acs_endpoint.py` & `okta-2.9.6/okta/models/acs_endpoint.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/activate_factor_request.py` & `okta-2.9.6/okta/models/activate_factor_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/allowed_for_enum.py` & `okta-2.9.6/okta/models/allowed_for_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_and_instance_condition_evaluator_app_or_instance.py` & `okta-2.9.6/okta/models/app_and_instance_condition_evaluator_app_or_instance.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_and_instance_policy_rule_condition.py` & `okta-2.9.6/okta/models/app_and_instance_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_instance_policy_rule_condition.py` & `okta-2.9.6/okta/models/app_instance_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_link.py` & `okta-2.9.6/okta/models/app_link.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_user.py` & `okta-2.9.6/okta/models/app_user.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_user_credentials.py` & `okta-2.9.6/okta/models/app_user_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/app_user_password_credential.py` & `okta-2.9.6/okta/models/app_user_password_credential.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application.py` & `okta-2.9.6/okta/models/application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_accessibility.py` & `okta-2.9.6/okta/models/application_accessibility.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_credentials.py` & `okta-2.9.6/okta/models/application_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_credentials_o_auth_client.py` & `okta-2.9.6/okta/models/application_credentials_o_auth_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_credentials_scheme.py` & `okta-2.9.6/okta/models/application_credentials_scheme.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_credentials_signing.py` & `okta-2.9.6/okta/models/application_credentials_signing.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_credentials_signing_use.py` & `okta-2.9.6/okta/models/application_credentials_signing_use.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_credentials_username_template.py` & `okta-2.9.6/okta/models/application_credentials_username_template.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_feature.py` & `okta-2.9.6/okta/models/application_feature.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_group_assignment.py` & `okta-2.9.6/okta/models/application_group_assignment.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_licensing.py` & `okta-2.9.6/okta/models/application_licensing.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_settings.py` & `okta-2.9.6/okta/models/application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_settings_application.py` & `okta-2.9.6/okta/models/application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_settings_notes.py` & `okta-2.9.6/okta/models/application_settings_notes.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_settings_notifications.py` & `okta-2.9.6/okta/models/application_settings_notifications.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_settings_notifications_vpn.py` & `okta-2.9.6/okta/models/application_settings_notifications_vpn.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_settings_notifications_vpn_network.py` & `okta-2.9.6/okta/models/application_settings_notifications_vpn_network.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_sign_on_mode.py` & `okta-2.9.6/okta/models/application_sign_on_mode.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_visibility.py` & `okta-2.9.6/okta/models/application_visibility.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/application_visibility_hide.py` & `okta-2.9.6/okta/models/application_visibility_hide.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/assign_role_request.py` & `okta-2.9.6/okta/models/assign_role_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authentication_provider.py` & `okta-2.9.6/okta/models/authentication_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authentication_provider_type.py` & `okta-2.9.6/okta/models/authentication_provider_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator.py` & `okta-2.9.6/okta/models/authenticator.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator_provider.py` & `okta-2.9.6/okta/models/authenticator_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator_provider_configuration.py` & `okta-2.9.6/okta/models/authenticator_provider_configuration.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator_provider_configuration_user_name_plate.py` & `okta-2.9.6/okta/models/authenticator_provider_configuration_user_name_plate.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator_settings.py` & `okta-2.9.6/okta/models/authenticator_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator_status.py` & `okta-2.9.6/okta/models/authenticator_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authenticator_type.py` & `okta-2.9.6/okta/models/authenticator_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server.py` & `okta-2.9.6/okta/models/authorization_server.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_credentials.py` & `okta-2.9.6/okta/models/authorization_server_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_credentials_rotation_mode.py` & `okta-2.9.6/okta/models/authorization_server_credentials_rotation_mode.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_credentials_signing_config.py` & `okta-2.9.6/okta/models/authorization_server_credentials_signing_config.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_credentials_use.py` & `okta-2.9.6/okta/models/authorization_server_credentials_use.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_policy.py` & `okta-2.9.6/okta/models/authorization_server_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_policy_rule.py` & `okta-2.9.6/okta/models/authorization_server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_policy_rule_actions.py` & `okta-2.9.6/okta/models/authorization_server_policy_rule_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/authorization_server_policy_rule_conditions.py` & `okta-2.9.6/okta/models/authorization_server_policy_rule_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/auto_login_application.py` & `okta-2.9.6/okta/models/auto_login_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/auto_login_application_settings.py` & `okta-2.9.6/okta/models/auto_login_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/auto_login_application_settings_sign_on.py` & `okta-2.9.6/okta/models/auto_login_application_settings_sign_on.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/basic_application_settings.py` & `okta-2.9.6/okta/models/basic_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/basic_application_settings_application.py` & `okta-2.9.6/okta/models/basic_application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/basic_auth_application.py` & `okta-2.9.6/okta/models/basic_auth_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/before_scheduled_action_policy_rule_condition.py` & `okta-2.9.6/okta/models/before_scheduled_action_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/bookmark_application.py` & `okta-2.9.6/okta/models/bookmark_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/bookmark_application_settings.py` & `okta-2.9.6/okta/models/bookmark_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/bookmark_application_settings_application.py` & `okta-2.9.6/okta/models/bookmark_application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/brand.py` & `okta-2.9.6/okta/models/brand.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/browser_plugin_application.py` & `okta-2.9.6/okta/models/browser_plugin_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/call_user_factor.py` & `okta-2.9.6/okta/models/call_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/call_user_factor_profile.py` & `okta-2.9.6/okta/models/call_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/capabilities_create_object.py` & `okta-2.9.6/okta/models/capabilities_create_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/capabilities_object.py` & `okta-2.9.6/okta/models/capabilities_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/capabilities_update_object.py` & `okta-2.9.6/okta/models/capabilities_update_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/catalog_application.py` & `okta-2.9.6/okta/models/catalog_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/catalog_application_status.py` & `okta-2.9.6/okta/models/catalog_application_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/change_enum.py` & `okta-2.9.6/okta/models/change_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/change_password_request.py` & `okta-2.9.6/okta/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/channel_binding.py` & `okta-2.9.6/okta/models/channel_binding.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/client_policy_condition.py` & `okta-2.9.6/okta/models/client_policy_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/client_secret.py` & `okta-2.9.6/okta/models/client_secret.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/client_secret_metadata.py` & `okta-2.9.6/okta/models/client_secret_metadata.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/compliance.py` & `okta-2.9.6/okta/models/compliance.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/context_policy_rule_condition.py` & `okta-2.9.6/okta/models/context_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/create_session_request.py` & `okta-2.9.6/okta/models/create_session_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/create_user_request.py` & `okta-2.9.6/okta/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/csr.py` & `okta-2.9.6/okta/models/csr.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/csr_metadata.py` & `okta-2.9.6/okta/models/csr_metadata.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/csr_metadata_subject.py` & `okta-2.9.6/okta/models/csr_metadata_subject.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/csr_metadata_subject_alt_names.py` & `okta-2.9.6/okta/models/csr_metadata_subject_alt_names.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/custom_hotp_user_factor.py` & `okta-2.9.6/okta/models/custom_hotp_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/custom_hotp_user_factor_profile.py` & `okta-2.9.6/okta/models/custom_hotp_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/device_access_policy_rule_condition.py` & `okta-2.9.6/okta/models/device_access_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/device_policy_rule_condition.py` & `okta-2.9.6/okta/models/device_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/device_policy_rule_condition_platform.py` & `okta-2.9.6/okta/models/device_policy_rule_condition_platform.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/dns_record.py` & `okta-2.9.6/okta/models/dns_record.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/dns_record_type.py` & `okta-2.9.6/okta/models/dns_record_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain.py` & `okta-2.9.6/okta/models/domain.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain_certificate.py` & `okta-2.9.6/okta/models/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain_certificate_metadata.py` & `okta-2.9.6/okta/models/domain_certificate_metadata.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain_certificate_source_type.py` & `okta-2.9.6/okta/models/domain_certificate_source_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain_certificate_type.py` & `okta-2.9.6/okta/models/domain_certificate_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain_list_response.py` & `okta-2.9.6/okta/models/domain_list_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/domain_validation_status.py` & `okta-2.9.6/okta/models/domain_validation_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/duration.py` & `okta-2.9.6/okta/models/duration.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_template.py` & `okta-2.9.6/okta/models/email_template.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_template_content.py` & `okta-2.9.6/okta/models/email_template_content.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_template_customization.py` & `okta-2.9.6/okta/models/email_template_customization.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_template_customization_request.py` & `okta-2.9.6/okta/models/email_template_customization_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_template_test_request.py` & `okta-2.9.6/okta/models/email_template_test_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_template_touch_point_variant.py` & `okta-2.9.6/okta/models/email_template_touch_point_variant.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_user_factor.py` & `okta-2.9.6/okta/models/email_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/email_user_factor_profile.py` & `okta-2.9.6/okta/models/email_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/enabled_status.py` & `okta-2.9.6/okta/models/enabled_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/end_user_dashboard_touch_point_variant.py` & `okta-2.9.6/okta/models/end_user_dashboard_touch_point_variant.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/error_page_touch_point_variant.py` & `okta-2.9.6/okta/models/error_page_touch_point_variant.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_hook.py` & `okta-2.9.6/okta/models/event_hook.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_hook_channel.py` & `okta-2.9.6/okta/models/event_hook_channel.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_hook_channel_config.py` & `okta-2.9.6/okta/models/event_hook_channel_config.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_hook_channel_config_auth_scheme.py` & `okta-2.9.6/okta/models/event_hook_channel_config_auth_scheme.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_hook_channel_config_auth_scheme_type.py` & `okta-2.9.6/okta/models/event_hook_channel_config_auth_scheme_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_hook_channel_config_header.py` & `okta-2.9.6/okta/models/event_hook_channel_config_header.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/event_subscriptions.py` & `okta-2.9.6/okta/models/event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/factor_provider.py` & `okta-2.9.6/okta/models/factor_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/factor_result_type.py` & `okta-2.9.6/okta/models/factor_result_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/factor_status.py` & `okta-2.9.6/okta/models/factor_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/factor_type.py` & `okta-2.9.6/okta/models/factor_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/feature.py` & `okta-2.9.6/okta/models/feature.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/feature_stage.py` & `okta-2.9.6/okta/models/feature_stage.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/feature_stage_state.py` & `okta-2.9.6/okta/models/feature_stage_state.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/feature_stage_value.py` & `okta-2.9.6/okta/models/feature_stage_value.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/feature_type.py` & `okta-2.9.6/okta/models/feature_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/fips_enum.py` & `okta-2.9.6/okta/models/fips_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/forgot_password_response.py` & `okta-2.9.6/okta/models/forgot_password_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/grant_type_policy_rule_condition.py` & `okta-2.9.6/okta/models/grant_type_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group.py` & `okta-2.9.6/okta/models/group.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_condition.py` & `okta-2.9.6/okta/models/group_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_policy_rule_condition.py` & `okta-2.9.6/okta/models/group_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_profile.py` & `okta-2.9.6/okta/models/group_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule.py` & `okta-2.9.6/okta/models/group_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_action.py` & `okta-2.9.6/okta/models/group_rule_action.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_conditions.py` & `okta-2.9.6/okta/models/group_rule_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_expression.py` & `okta-2.9.6/okta/models/group_rule_expression.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_group_assignment.py` & `okta-2.9.6/okta/models/group_rule_group_assignment.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_group_condition.py` & `okta-2.9.6/okta/models/group_rule_group_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_people_condition.py` & `okta-2.9.6/okta/models/group_rule_people_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_status.py` & `okta-2.9.6/okta/models/group_rule_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_rule_user_condition.py` & `okta-2.9.6/okta/models/group_rule_user_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_schema.py` & `okta-2.9.6/okta/models/group_schema.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_schema_attribute.py` & `okta-2.9.6/okta/models/group_schema_attribute.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_schema_base.py` & `okta-2.9.6/okta/models/group_schema_base.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_schema_base_properties.py` & `okta-2.9.6/okta/models/group_schema_base_properties.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_schema_custom.py` & `okta-2.9.6/okta/models/group_schema_custom.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_schema_definitions.py` & `okta-2.9.6/okta/models/group_schema_definitions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/group_type.py` & `okta-2.9.6/okta/models/group_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/hardware_user_factor.py` & `okta-2.9.6/okta/models/hardware_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/hardware_user_factor_profile.py` & `okta-2.9.6/okta/models/hardware_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider.py` & `okta-2.9.6/okta/models/identity_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_application_user.py` & `okta-2.9.6/okta/models/identity_provider_application_user.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_credentials.py` & `okta-2.9.6/okta/models/identity_provider_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_credentials_client.py` & `okta-2.9.6/okta/models/identity_provider_credentials_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_credentials_signing.py` & `okta-2.9.6/okta/models/identity_provider_credentials_signing.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_credentials_trust.py` & `okta-2.9.6/okta/models/identity_provider_credentials_trust.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_policy.py` & `okta-2.9.6/okta/models/identity_provider_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/identity_provider_policy_rule_condition.py` & `okta-2.9.6/okta/models/identity_provider_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/idp_policy_rule_action.py` & `okta-2.9.6/okta/models/idp_policy_rule_action.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/idp_policy_rule_action_provider.py` & `okta-2.9.6/okta/models/idp_policy_rule_action_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/iframe_embed_scope_allowed_apps.py` & `okta-2.9.6/okta/models/iframe_embed_scope_allowed_apps.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/image_upload_response.py` & `okta-2.9.6/okta/models/image_upload_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inactivity_policy_rule_condition.py` & `okta-2.9.6/okta/models/inactivity_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook.py` & `okta-2.9.6/okta/models/inline_hook.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_channel.py` & `okta-2.9.6/okta/models/inline_hook_channel.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_channel_config.py` & `okta-2.9.6/okta/models/inline_hook_channel_config.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_channel_config_auth_scheme.py` & `okta-2.9.6/okta/models/inline_hook_channel_config_auth_scheme.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_channel_config_headers.py` & `okta-2.9.6/okta/models/inline_hook_channel_config_headers.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_payload.py` & `okta-2.9.6/okta/models/inline_hook_payload.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_response.py` & `okta-2.9.6/okta/models/inline_hook_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_response_command_value.py` & `okta-2.9.6/okta/models/inline_hook_response_command_value.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_response_commands.py` & `okta-2.9.6/okta/models/inline_hook_response_commands.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_status.py` & `okta-2.9.6/okta/models/inline_hook_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/inline_hook_type.py` & `okta-2.9.6/okta/models/inline_hook_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/ion_field.py` & `okta-2.9.6/okta/models/ion_field.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/ion_form.py` & `okta-2.9.6/okta/models/ion_form.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/json_web_key.py` & `okta-2.9.6/okta/models/json_web_key.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/jwk_use.py` & `okta-2.9.6/okta/models/jwk_use.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/knowledge_constraint.py` & `okta-2.9.6/okta/models/knowledge_constraint.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/lifecycle_create_setting_object.py` & `okta-2.9.6/okta/models/lifecycle_create_setting_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/lifecycle_deactivate_setting_object.py` & `okta-2.9.6/okta/models/lifecycle_deactivate_setting_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/lifecycle_expiration_policy_rule_condition.py` & `okta-2.9.6/okta/models/lifecycle_expiration_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/linked_object.py` & `okta-2.9.6/okta/models/linked_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/linked_object_details.py` & `okta-2.9.6/okta/models/linked_object_details.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/linked_object_details_type.py` & `okta-2.9.6/okta/models/linked_object_details_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_actor.py` & `okta-2.9.6/okta/models/log_actor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_authentication_context.py` & `okta-2.9.6/okta/models/log_authentication_context.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_authentication_provider.py` & `okta-2.9.6/okta/models/log_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_client.py` & `okta-2.9.6/okta/models/log_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_credential_provider.py` & `okta-2.9.6/okta/models/log_credential_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_credential_type.py` & `okta-2.9.6/okta/models/log_credential_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_debug_context.py` & `okta-2.9.6/okta/models/log_debug_context.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_event.py` & `okta-2.9.6/okta/models/log_event.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_geographical_context.py` & `okta-2.9.6/okta/models/log_geographical_context.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_geolocation.py` & `okta-2.9.6/okta/models/log_geolocation.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_ip_address.py` & `okta-2.9.6/okta/models/log_ip_address.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_issuer.py` & `okta-2.9.6/okta/models/log_issuer.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_outcome.py` & `okta-2.9.6/okta/models/log_outcome.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_request.py` & `okta-2.9.6/okta/models/log_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_security_context.py` & `okta-2.9.6/okta/models/log_security_context.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_severity.py` & `okta-2.9.6/okta/models/log_severity.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_target.py` & `okta-2.9.6/okta/models/log_target.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_transaction.py` & `okta-2.9.6/okta/models/log_transaction.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/log_user_agent.py` & `okta-2.9.6/okta/models/log_user_agent.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/mdm_enrollment_policy_rule_condition.py` & `okta-2.9.6/okta/models/mdm_enrollment_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/multifactor_enrollment_policy.py` & `okta-2.9.6/okta/models/multifactor_enrollment_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/multifactor_enrollment_policy_authenticator_settings.py` & `okta-2.9.6/okta/models/multifactor_enrollment_policy_authenticator_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/multifactor_enrollment_policy_authenticator_status.py` & `okta-2.9.6/okta/models/multifactor_enrollment_policy_authenticator_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/multifactor_enrollment_policy_authenticator_type.py` & `okta-2.9.6/okta/models/multifactor_enrollment_policy_authenticator_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/multifactor_enrollment_policy_settings.py` & `okta-2.9.6/okta/models/multifactor_enrollment_policy_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/multifactor_enrollment_policy_settings_type.py` & `okta-2.9.6/okta/models/multifactor_enrollment_policy_settings_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone.py` & `okta-2.9.6/okta/models/network_zone.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone_address.py` & `okta-2.9.6/okta/models/network_zone_address.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone_address_type.py` & `okta-2.9.6/okta/models/network_zone_address_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone_location.py` & `okta-2.9.6/okta/models/network_zone_location.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone_status.py` & `okta-2.9.6/okta/models/network_zone_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone_type.py` & `okta-2.9.6/okta/models/network_zone_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/network_zone_usage.py` & `okta-2.9.6/okta/models/network_zone_usage.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/notification_type.py` & `okta-2.9.6/okta/models/notification_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_actor.py` & `okta-2.9.6/okta/models/o_auth_2_actor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_claim.py` & `okta-2.9.6/okta/models/o_auth_2_claim.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_claim_conditions.py` & `okta-2.9.6/okta/models/o_auth_2_claim_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_client.py` & `okta-2.9.6/okta/models/o_auth_2_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_refresh_token.py` & `okta-2.9.6/okta/models/o_auth_2_refresh_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_scope.py` & `okta-2.9.6/okta/models/o_auth_2_scope.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_scope_consent_grant.py` & `okta-2.9.6/okta/models/o_auth_2_scope_consent_grant.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_scope_consent_grant_source.py` & `okta-2.9.6/okta/models/o_auth_2_scope_consent_grant_source.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_scope_consent_grant_status.py` & `okta-2.9.6/okta/models/o_auth_2_scope_consent_grant_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_scopes_mediation_policy_rule_condition.py` & `okta-2.9.6/okta/models/o_auth_2_scopes_mediation_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_2_token.py` & `okta-2.9.6/okta/models/o_auth_2_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_application_credentials.py` & `okta-2.9.6/okta/models/o_auth_application_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_authorization_policy.py` & `okta-2.9.6/okta/models/o_auth_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_endpoint_authentication_method.py` & `okta-2.9.6/okta/models/o_auth_endpoint_authentication_method.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_grant_type.py` & `okta-2.9.6/okta/models/o_auth_grant_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/o_auth_response_type.py` & `okta-2.9.6/okta/models/o_auth_response_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy.py` & `okta-2.9.6/okta/models/okta_sign_on_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy_conditions.py` & `okta-2.9.6/okta/models/okta_sign_on_policy_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy_rule.py` & `okta-2.9.6/okta/models/okta_sign_on_policy_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy_rule_actions.py` & `okta-2.9.6/okta/models/okta_sign_on_policy_rule_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy_rule_conditions.py` & `okta-2.9.6/okta/models/okta_sign_on_policy_rule_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy_rule_signon_actions.py` & `okta-2.9.6/okta/models/okta_sign_on_policy_rule_signon_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/okta_sign_on_policy_rule_signon_session_actions.py` & `okta-2.9.6/okta/models/okta_sign_on_policy_rule_signon_session_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application.py` & `okta-2.9.6/okta/models/open_id_connect_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_consent_method.py` & `okta-2.9.6/okta/models/open_id_connect_application_consent_method.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_idp_initiated_login.py` & `okta-2.9.6/okta/models/open_id_connect_application_idp_initiated_login.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_issuer_mode.py` & `okta-2.9.6/okta/models/open_id_connect_application_issuer_mode.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_settings.py` & `okta-2.9.6/okta/models/open_id_connect_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_settings_client.py` & `okta-2.9.6/okta/models/open_id_connect_application_settings_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_settings_client_keys.py` & `okta-2.9.6/okta/models/open_id_connect_application_settings_client_keys.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_settings_refresh_token.py` & `okta-2.9.6/okta/models/open_id_connect_application_settings_refresh_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_application_type.py` & `okta-2.9.6/okta/models/open_id_connect_application_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/open_id_connect_refresh_token_rotation_type.py` & `okta-2.9.6/okta/models/open_id_connect_refresh_token_rotation_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_2_org_application.py` & `okta-2.9.6/okta/models/org_2_org_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_2_org_application_settings.py` & `okta-2.9.6/okta/models/org_2_org_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_2_org_application_settings_app.py` & `okta-2.9.6/okta/models/org_2_org_application_settings_app.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_contact_type.py` & `okta-2.9.6/okta/models/org_contact_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_contact_type_obj.py` & `okta-2.9.6/okta/models/org_contact_type_obj.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_contact_user.py` & `okta-2.9.6/okta/models/org_contact_user.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_okta_communication_setting.py` & `okta-2.9.6/okta/models/org_okta_communication_setting.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_okta_support_setting.py` & `okta-2.9.6/okta/models/org_okta_support_setting.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_okta_support_settings_obj.py` & `okta-2.9.6/okta/models/org_okta_support_settings_obj.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_preferences.py` & `okta-2.9.6/okta/models/org_preferences.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/org_setting.py` & `okta-2.9.6/okta/models/org_setting.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_credential.py` & `okta-2.9.6/okta/models/password_credential.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_credential_hash.py` & `okta-2.9.6/okta/models/password_credential_hash.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_credential_hash_algorithm.py` & `okta-2.9.6/okta/models/password_credential_hash_algorithm.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_credential_hook.py` & `okta-2.9.6/okta/models/password_credential_hook.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_dictionary.py` & `okta-2.9.6/okta/models/password_dictionary.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_dictionary_common.py` & `okta-2.9.6/okta/models/password_dictionary_common.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_expiration_policy_rule_condition.py` & `okta-2.9.6/okta/models/password_expiration_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy.py` & `okta-2.9.6/okta/models/password_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_authentication_provider_condition.py` & `okta-2.9.6/okta/models/password_policy_authentication_provider_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_conditions.py` & `okta-2.9.6/okta/models/password_policy_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_delegation_settings.py` & `okta-2.9.6/okta/models/password_policy_delegation_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_delegation_settings_options.py` & `okta-2.9.6/okta/models/password_policy_delegation_settings_options.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_password_settings.py` & `okta-2.9.6/okta/models/password_policy_password_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_password_settings_age.py` & `okta-2.9.6/okta/models/password_policy_password_settings_age.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_password_settings_complexity.py` & `okta-2.9.6/okta/models/password_policy_password_settings_complexity.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_password_settings_lockout.py` & `okta-2.9.6/okta/models/password_policy_password_settings_lockout.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_email.py` & `okta-2.9.6/okta/models/password_policy_recovery_email.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_email_properties.py` & `okta-2.9.6/okta/models/password_policy_recovery_email_properties.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_email_recovery_token.py` & `okta-2.9.6/okta/models/password_policy_recovery_email_recovery_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_factor_settings.py` & `okta-2.9.6/okta/models/password_policy_recovery_factor_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_factors.py` & `okta-2.9.6/okta/models/password_policy_recovery_factors.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_question.py` & `okta-2.9.6/okta/models/password_policy_recovery_question.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_question_complexity.py` & `okta-2.9.6/okta/models/password_policy_recovery_question_complexity.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_question_properties.py` & `okta-2.9.6/okta/models/password_policy_recovery_question_properties.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_recovery_settings.py` & `okta-2.9.6/okta/models/password_policy_recovery_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_rule.py` & `okta-2.9.6/okta/models/password_policy_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_rule_action.py` & `okta-2.9.6/okta/models/password_policy_rule_action.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_rule_actions.py` & `okta-2.9.6/okta/models/password_policy_rule_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_rule_conditions.py` & `okta-2.9.6/okta/models/password_policy_rule_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_policy_settings.py` & `okta-2.9.6/okta/models/password_policy_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/password_setting_object.py` & `okta-2.9.6/okta/models/password_setting_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/platform_condition_evaluator_platform.py` & `okta-2.9.6/okta/models/platform_condition_evaluator_platform.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/platform_condition_evaluator_platform_operating_system.py` & `okta-2.9.6/okta/models/platform_condition_evaluator_platform_operating_system.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/platform_condition_evaluator_platform_operating_system_version.py` & `okta-2.9.6/okta/models/platform_condition_evaluator_platform_operating_system_version.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/platform_policy_rule_condition.py` & `okta-2.9.6/okta/models/platform_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy.py` & `okta-2.9.6/okta/models/policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_account_link.py` & `okta-2.9.6/okta/models/policy_account_link.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_account_link_filter.py` & `okta-2.9.6/okta/models/policy_account_link_filter.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_account_link_filter_groups.py` & `okta-2.9.6/okta/models/policy_account_link_filter_groups.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_network_condition.py` & `okta-2.9.6/okta/models/policy_network_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_people_condition.py` & `okta-2.9.6/okta/models/policy_people_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_rule.py` & `okta-2.9.6/okta/models/policy_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_rule_actions.py` & `okta-2.9.6/okta/models/policy_rule_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_rule_actions_enroll.py` & `okta-2.9.6/okta/models/policy_rule_actions_enroll.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_rule_actions_enroll_self.py` & `okta-2.9.6/okta/models/policy_rule_actions_enroll_self.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_rule_auth_context_condition.py` & `okta-2.9.6/okta/models/policy_rule_auth_context_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_rule_conditions.py` & `okta-2.9.6/okta/models/policy_rule_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_subject.py` & `okta-2.9.6/okta/models/policy_subject.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_subject_match_type.py` & `okta-2.9.6/okta/models/policy_subject_match_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_type.py` & `okta-2.9.6/okta/models/policy_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/policy_user_name_template.py` & `okta-2.9.6/okta/models/policy_user_name_template.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/possession_constraint.py` & `okta-2.9.6/okta/models/possession_constraint.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/pre_registration_inline_hook.py` & `okta-2.9.6/okta/models/pre_registration_inline_hook.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_enrollment_policy.py` & `okta-2.9.6/okta/models/profile_enrollment_policy.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_enrollment_policy_rule.py` & `okta-2.9.6/okta/models/profile_enrollment_policy_rule.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_enrollment_policy_rule_action.py` & `okta-2.9.6/okta/models/profile_enrollment_policy_rule_action.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_enrollment_policy_rule_actions.py` & `okta-2.9.6/okta/models/profile_enrollment_policy_rule_actions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_enrollment_policy_rule_activation_requirement.py` & `okta-2.9.6/okta/models/profile_enrollment_policy_rule_activation_requirement.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_enrollment_policy_rule_profile_attribute.py` & `okta-2.9.6/okta/models/profile_enrollment_policy_rule_profile_attribute.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_mapping.py` & `okta-2.9.6/okta/models/profile_mapping.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_mapping_property.py` & `okta-2.9.6/okta/models/profile_mapping_property.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_mapping_property_push_status.py` & `okta-2.9.6/okta/models/profile_mapping_property_push_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_mapping_source.py` & `okta-2.9.6/okta/models/profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/profile_setting_object.py` & `okta-2.9.6/okta/models/profile_setting_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol.py` & `okta-2.9.6/okta/models/protocol.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_algorithm_type.py` & `okta-2.9.6/okta/models/protocol_algorithm_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_algorithm_type_signature.py` & `okta-2.9.6/okta/models/protocol_algorithm_type_signature.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_algorithms.py` & `okta-2.9.6/okta/models/protocol_algorithms.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_endpoint.py` & `okta-2.9.6/okta/models/protocol_endpoint.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_endpoints.py` & `okta-2.9.6/okta/models/protocol_endpoints.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_relay_state.py` & `okta-2.9.6/okta/models/protocol_relay_state.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_relay_state_format.py` & `okta-2.9.6/okta/models/protocol_relay_state_format.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/protocol_settings.py` & `okta-2.9.6/okta/models/protocol_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning.py` & `okta-2.9.6/okta/models/provisioning.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_conditions.py` & `okta-2.9.6/okta/models/provisioning_conditions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_connection.py` & `okta-2.9.6/okta/models/provisioning_connection.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_connection_auth_scheme.py` & `okta-2.9.6/okta/models/provisioning_connection_auth_scheme.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_connection_profile.py` & `okta-2.9.6/okta/models/provisioning_connection_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_connection_request.py` & `okta-2.9.6/okta/models/provisioning_connection_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_connection_status.py` & `okta-2.9.6/okta/models/provisioning_connection_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_deprovisioned_condition.py` & `okta-2.9.6/okta/models/provisioning_deprovisioned_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_groups.py` & `okta-2.9.6/okta/models/provisioning_groups.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/provisioning_suspended_condition.py` & `okta-2.9.6/okta/models/provisioning_suspended_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/push_user_factor.py` & `okta-2.9.6/okta/models/push_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/push_user_factor_profile.py` & `okta-2.9.6/okta/models/push_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/recovery_question_credential.py` & `okta-2.9.6/okta/models/recovery_question_credential.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/required_enum.py` & `okta-2.9.6/okta/models/required_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/reset_password_token.py` & `okta-2.9.6/okta/models/reset_password_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/response_links.py` & `okta-2.9.6/okta/models/response_links.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/risk_policy_rule_condition.py` & `okta-2.9.6/okta/models/risk_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/risk_score_policy_rule_condition.py` & `okta-2.9.6/okta/models/risk_score_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/role.py` & `okta-2.9.6/okta/models/role.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/role_assignment_type.py` & `okta-2.9.6/okta/models/role_assignment_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/role_status.py` & `okta-2.9.6/okta/models/role_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/role_type.py` & `okta-2.9.6/okta/models/role_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/saml_application.py` & `okta-2.9.6/okta/models/saml_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/saml_application_settings.py` & `okta-2.9.6/okta/models/saml_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/saml_application_settings_sign_on.py` & `okta-2.9.6/okta/models/saml_application_settings_sign_on.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/saml_attribute_statement.py` & `okta-2.9.6/okta/models/saml_attribute_statement.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/scheduled_user_lifecycle_action.py` & `okta-2.9.6/okta/models/scheduled_user_lifecycle_action.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/scheme_application_credentials.py` & `okta-2.9.6/okta/models/scheme_application_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/scope.py` & `okta-2.9.6/okta/models/scope.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/scope_type.py` & `okta-2.9.6/okta/models/scope_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/secure_password_store_application.py` & `okta-2.9.6/okta/models/secure_password_store_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/secure_password_store_application_settings.py` & `okta-2.9.6/okta/models/secure_password_store_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/secure_password_store_application_settings_application.py` & `okta-2.9.6/okta/models/secure_password_store_application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/security_question.py` & `okta-2.9.6/okta/models/security_question.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/security_question_user_factor.py` & `okta-2.9.6/okta/models/security_question_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/security_question_user_factor_profile.py` & `okta-2.9.6/okta/models/security_question_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/seed_enum.py` & `okta-2.9.6/okta/models/seed_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/session.py` & `okta-2.9.6/okta/models/session.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/session_authentication_method.py` & `okta-2.9.6/okta/models/session_authentication_method.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/session_identity_provider.py` & `okta-2.9.6/okta/models/session_identity_provider.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/session_identity_provider_type.py` & `okta-2.9.6/okta/models/session_identity_provider_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/session_status.py` & `okta-2.9.6/okta/models/session_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sign_in_page_touch_point_variant.py` & `okta-2.9.6/okta/models/sign_in_page_touch_point_variant.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sign_on_inline_hook.py` & `okta-2.9.6/okta/models/sign_on_inline_hook.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/single_logout.py` & `okta-2.9.6/okta/models/single_logout.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sms_template.py` & `okta-2.9.6/okta/models/sms_template.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sms_template_translations.py` & `okta-2.9.6/okta/models/sms_template_translations.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sms_template_type.py` & `okta-2.9.6/okta/models/sms_template_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sms_user_factor.py` & `okta-2.9.6/okta/models/sms_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sms_user_factor_profile.py` & `okta-2.9.6/okta/models/sms_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/social_auth_token.py` & `okta-2.9.6/okta/models/social_auth_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/sp_certificate.py` & `okta-2.9.6/okta/models/sp_certificate.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/subscription.py` & `okta-2.9.6/okta/models/subscription.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/subscription_status.py` & `okta-2.9.6/okta/models/subscription_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/swa_application.py` & `okta-2.9.6/okta/models/swa_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/swa_application_settings.py` & `okta-2.9.6/okta/models/swa_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/swa_application_settings_application.py` & `okta-2.9.6/okta/models/swa_application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/swa_three_field_application.py` & `okta-2.9.6/okta/models/swa_three_field_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/swa_three_field_application_settings.py` & `okta-2.9.6/okta/models/swa_three_field_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/swa_three_field_application_settings_application.py` & `okta-2.9.6/okta/models/swa_three_field_application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/temp_password.py` & `okta-2.9.6/okta/models/temp_password.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/theme.py` & `okta-2.9.6/okta/models/theme.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/theme_response.py` & `okta-2.9.6/okta/models/theme_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/threat_insight_configuration.py` & `okta-2.9.6/okta/models/threat_insight_configuration.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/token_authorization_server_policy_rule_action.py` & `okta-2.9.6/okta/models/token_authorization_server_policy_rule_action.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/token_authorization_server_policy_rule_action_inline_hook.py` & `okta-2.9.6/okta/models/token_authorization_server_policy_rule_action_inline_hook.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/token_user_factor.py` & `okta-2.9.6/okta/models/token_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/token_user_factor_profile.py` & `okta-2.9.6/okta/models/token_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/totp_user_factor.py` & `okta-2.9.6/okta/models/totp_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/totp_user_factor_profile.py` & `okta-2.9.6/okta/models/totp_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/trusted_origin.py` & `okta-2.9.6/okta/models/trusted_origin.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/u_2_f_user_factor.py` & `okta-2.9.6/okta/models/u_2_f_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/u_2_f_user_factor_profile.py` & `okta-2.9.6/okta/models/u_2_f_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user.py` & `okta-2.9.6/okta/models/user.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_activation_token.py` & `okta-2.9.6/okta/models/user_activation_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_condition.py` & `okta-2.9.6/okta/models/user_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_credentials.py` & `okta-2.9.6/okta/models/user_credentials.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_factor.py` & `okta-2.9.6/okta/models/user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_id_string.py` & `okta-2.9.6/okta/models/user_id_string.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_identifier_condition_evaluator_pattern.py` & `okta-2.9.6/okta/models/user_identifier_condition_evaluator_pattern.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_identifier_policy_rule_condition.py` & `okta-2.9.6/okta/models/user_identifier_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_identity_provider_link_request.py` & `okta-2.9.6/okta/models/user_identity_provider_link_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_lifecycle_attribute_policy_rule_condition.py` & `okta-2.9.6/okta/models/user_lifecycle_attribute_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_next_login.py` & `okta-2.9.6/okta/models/user_next_login.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_policy_rule_condition.py` & `okta-2.9.6/okta/models/user_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_profile.py` & `okta-2.9.6/okta/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema.py` & `okta-2.9.6/okta/models/user_schema.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute.py` & `okta-2.9.6/okta/models/user_schema_attribute.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_enum.py` & `okta-2.9.6/okta/models/user_schema_attribute_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_items.py` & `okta-2.9.6/okta/models/user_schema_attribute_items.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_master.py` & `okta-2.9.6/okta/models/user_schema_attribute_master.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_master_priority.py` & `okta-2.9.6/okta/models/user_schema_attribute_master_priority.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_master_type.py` & `okta-2.9.6/okta/models/user_schema_attribute_master_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_permission.py` & `okta-2.9.6/okta/models/user_schema_attribute_permission.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_scope.py` & `okta-2.9.6/okta/models/user_schema_attribute_scope.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_type.py` & `okta-2.9.6/okta/models/user_schema_attribute_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_attribute_union.py` & `okta-2.9.6/okta/models/user_schema_attribute_union.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_base.py` & `okta-2.9.6/okta/models/user_schema_base.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_base_properties.py` & `okta-2.9.6/okta/models/user_schema_base_properties.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_definitions.py` & `okta-2.9.6/okta/models/user_schema_definitions.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_properties.py` & `okta-2.9.6/okta/models/user_schema_properties.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_properties_profile.py` & `okta-2.9.6/okta/models/user_schema_properties_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_properties_profile_item.py` & `okta-2.9.6/okta/models/user_schema_properties_profile_item.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_schema_public.py` & `okta-2.9.6/okta/models/user_schema_public.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_status.py` & `okta-2.9.6/okta/models/user_status.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_status_policy_rule_condition.py` & `okta-2.9.6/okta/models/user_status_policy_rule_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_type.py` & `okta-2.9.6/okta/models/user_type.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_type_condition.py` & `okta-2.9.6/okta/models/user_type_condition.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/user_verification_enum.py` & `okta-2.9.6/okta/models/user_verification_enum.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/verification_method.py` & `okta-2.9.6/okta/models/verification_method.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/verify_factor_request.py` & `okta-2.9.6/okta/models/verify_factor_request.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/verify_user_factor_response.py` & `okta-2.9.6/okta/models/verify_user_factor_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/web_authn_user_factor.py` & `okta-2.9.6/okta/models/web_authn_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/web_authn_user_factor_profile.py` & `okta-2.9.6/okta/models/web_authn_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/web_user_factor.py` & `okta-2.9.6/okta/models/web_user_factor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/web_user_factor_profile.py` & `okta-2.9.6/okta/models/web_user_factor_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/ws_federation_application.py` & `okta-2.9.6/okta/models/ws_federation_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/ws_federation_application_settings.py` & `okta-2.9.6/okta/models/ws_federation_application_settings.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/models/ws_federation_application_settings_application.py` & `okta-2.9.6/okta/models/ws_federation_application_settings_application.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/oauth.py` & `okta-2.9.6/okta/oauth.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/okta_collection.py` & `okta-2.9.6/okta/okta_collection.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/okta_object.py` & `okta-2.9.6/okta/okta_object.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/request_executor.py` & `okta-2.9.6/okta/request_executor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/application_client.py` & `okta-2.9.6/okta/resource_clients/application_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/authenticator_client.py` & `okta-2.9.6/okta/resource_clients/authenticator_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/authorization_server_client.py` & `okta-2.9.6/okta/resource_clients/authorization_server_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/brand_client.py` & `okta-2.9.6/okta/resource_clients/brand_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/domain_client.py` & `okta-2.9.6/okta/resource_clients/domain_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/event_hook_client.py` & `okta-2.9.6/okta/resource_clients/event_hook_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/feature_client.py` & `okta-2.9.6/okta/resource_clients/feature_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/group_client.py` & `okta-2.9.6/okta/resource_clients/group_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/group_schema_client.py` & `okta-2.9.6/okta/resource_clients/group_schema_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/identity_provider_client.py` & `okta-2.9.6/okta/resource_clients/identity_provider_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/inline_hook_client.py` & `okta-2.9.6/okta/resource_clients/inline_hook_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/linked_object_client.py` & `okta-2.9.6/okta/resource_clients/linked_object_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/log_event_client.py` & `okta-2.9.6/okta/resource_clients/log_event_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/network_zone_client.py` & `okta-2.9.6/okta/resource_clients/network_zone_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/org_client.py` & `okta-2.9.6/okta/resource_clients/org_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/policy_client.py` & `okta-2.9.6/okta/resource_clients/policy_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/profile_mapping_client.py` & `okta-2.9.6/okta/resource_clients/profile_mapping_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/session_client.py` & `okta-2.9.6/okta/resource_clients/session_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/sms_template_client.py` & `okta-2.9.6/okta/resource_clients/sms_template_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/subscription_client.py` & `okta-2.9.6/okta/resource_clients/subscription_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/threat_insight_client.py` & `okta-2.9.6/okta/resource_clients/threat_insight_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/trusted_origin_client.py` & `okta-2.9.6/okta/resource_clients/trusted_origin_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/user_client.py` & `okta-2.9.6/okta/resource_clients/user_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/user_factor_client.py` & `okta-2.9.6/okta/resource_clients/user_factor_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/user_schema_client.py` & `okta-2.9.6/okta/resource_clients/user_schema_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/resource_clients/user_type_client.py` & `okta-2.9.6/okta/resource_clients/user_type_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/user_agent.py` & `okta-2.9.6/okta/user_agent.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta/utils.py` & `okta-2.9.6/okta/utils.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/okta.egg-info/PKG-INFO` & `okta-2.9.6/okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okta
-Version: 2.9.5
+Version: 2.9.6
 Summary: Python SDK for the Okta Management API
 Home-page: https://github.com/okta/okta-sdk-python
 Author: Okta, Inc.
 Author-email: devex@okta.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `okta-2.9.5/okta.egg-info/SOURCES.txt` & `okta-2.9.6/okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/setup.py` & `okta-2.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/__pycache__/conftest.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/__pycache__/conftest.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/__pycache__/mocks.cpython-310.pyc` & `okta-2.9.6/tests/__pycache__/mocks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/conftest.py` & `okta-2.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_applications_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_applications_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_auth_server_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_auth_server_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_authenticators_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_authenticators_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_brands_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_brands_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_domains_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_domains_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_event_hooks_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_event_hooks_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_factors_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_factors_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_features_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_features_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_group_schema_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_group_schema_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_groups_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_groups_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_identity_providers.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_identity_providers.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_inline_hooks_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_inline_hooks_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_linked_objects_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_linked_objects_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_log_events_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_log_events_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_network_zone_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_network_zone_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_org_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_org_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_policies_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_policies_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_subscription_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_subscription_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_templates_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_templates_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_threat_insight_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_threat_insight_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_trusted_origins_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_trusted_origins_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_user_schema_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_user_schema_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_user_types_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_user_types_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/__pycache__/test_users_it.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/integration/__pycache__/test_users_it.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_activate_deactivate_delete_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_activate_deactivate_delete_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_remove_assigned_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_remove_assigned_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_update_assigned_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_app_update_assigned_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_group_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_group_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_user_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_assign_user_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_clone_app_key.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_clone_app_key.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_three_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_SWA_three_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_basic_auth_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_basic_auth_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_bookmark_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_bookmark_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_open_id_connect_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_open_id_connect_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_secure_password_store_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_create_secure_password_store_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_app_key.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_app_key.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_csr.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_generate_csr.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_app_keys.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_app_keys.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_consent_grant.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_consent_grant.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_csr.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_csr.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_default_provisioning_connection_for_application.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_default_provisioning_connection_for_application.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_list_assign_users_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_get_list_assign_users_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_grant_consent_to_scope.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_grant_consent_to_scope.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_app_keys.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_app_keys.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_apps.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_apps.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_assign_group_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_list_assign_group_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_remove_assign_group_app.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_remove_assign_group_app.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_consent_grant.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_consent_grant.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_csr.yaml` & `okta-2.9.6/tests/integration/cassettes/test_applications_it/TestApplicationsResource.test_revoke_csr.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_activate_server.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_activate_server.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_auth_server.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_auth_server.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_claim.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_claim.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_scope.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_create_get_oauth2_scope.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_auth_server_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_auth_server_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_claim.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_claim.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_scope.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_delete_oauth2_scope.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_auth_server_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_auth_server_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_created_auth_server.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_get_created_auth_server.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_keys.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_keys.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_policies.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_server_policies.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_servers.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_auth_servers.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_authorization_server_policy_rules.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_authorization_server_policy_rules.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_claims.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_claims.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_scopes.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_list_oauth2_scopes.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_rotate_auth_server_keys.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_rotate_auth_server_keys.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_auth_server_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_deactivate_delete_server.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_deactivate_delete_server.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_claim.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_claim.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_scope.yaml` & `okta-2.9.6/tests/integration/cassettes/test_auth_server_it/TestAuthorizationServerResource.test_update_oauth2_scope.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_activate_and_deactivate_authenticator.yaml` & `okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_activate_and_deactivate_authenticator.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_get_authenticator.yaml` & `okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_get_authenticator.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_list_authenticators.yaml` & `okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_list_authenticators.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_update_authenticator.yaml` & `okta-2.9.6/tests/integration/cassettes/test_authenticators_it/TestAuthenticatorsResource.test_update_authenticator.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_create_delete_email_template_customizations.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_create_delete_email_template_customizations.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_background_image.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_background_image.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_favicon.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_favicon.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_logo.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_delete_brand_theme_logo.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand_theme.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_brand_theme.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template_customization_preview.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_email_template_customization_preview.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_update_email_template_customization.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_get_update_email_template_customization.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brand_themes.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brand_themes.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brands.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_brands.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_template_customizations.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_template_customizations.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_templates.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_list_email_templates.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand_theme.yaml` & `okta-2.9.6/tests/integration/cassettes/test_brands_it/TestBrandsResource.test_update_brand_theme.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_domains_it/TestDomainResource.test_create_and_delete_domain.yaml` & `okta-2.9.6/tests/integration/cassettes/test_domains_it/TestDomainResource.test_create_and_delete_domain.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_domains_it/TestDomainResource.test_get_domain.yaml` & `okta-2.9.6/tests/integration/cassettes/test_domains_it/TestDomainResource.test_get_domain.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_domains_it/TestDomainResource.test_list_domains.yaml` & `okta-2.9.6/tests/integration/cassettes/test_domains_it/TestDomainResource.test_list_domains.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_activate_event_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_activate_event_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_create_get_event_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_create_get_event_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_deactivate_event_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_deactivate_event_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_delete_event_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_delete_event_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_list_event_hooks.yaml` & `okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_list_event_hooks.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_update_event_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_event_hooks_it/TestEventHooksResource.test_update_event_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_delete_factor.yaml` & `okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_delete_factor.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_enroll_sms_factor.yaml` & `okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_enroll_sms_factor.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_get_factor.yaml` & `okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_get_factor.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_list_factors_new_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_factors_it/TestFactorsResource.test_list_factors_new_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_get_feature.yaml` & `okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_get_feature.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependencies.yaml` & `okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependencies.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependents.yaml` & `okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_feature_dependents.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_features.yaml` & `okta-2.9.6/tests/integration/cassettes/test_features_it/TestFeaturesResource.test_list_features.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_add_and_remove_custom_attribute.yaml` & `okta-2.9.6/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_add_and_remove_custom_attribute.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_get_group_schema.yaml` & `okta-2.9.6/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_get_group_schema.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_update_custom_attribute.yaml` & `okta-2.9.6/tests/integration/cassettes/test_group_schema_it/TestGroupSchemaResource.test_update_custom_attribute.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_create_get_group.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_create_get_group.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_assigned_applications.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_assigned_applications.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_profile_custom_attributes.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_profile_custom_attributes.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_roles_operations.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_roles_operations.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_rule_operations.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_rule_operations.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_add.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_add.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_remove.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_target_remove.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_users_operations.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_group_users_operations.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_list_groups.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_list_groups.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_remove_group.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_remove_group.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_search_group.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_search_group.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_update_group.yaml` & `okta-2.9.6/tests/integration/cassettes/test_groups_it/TestGroupsResource.test_update_group.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_activate_deactivate_idp.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_activate_deactivate_idp.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_facebook_idp.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_facebook_idp.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_generic_idp.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_generic_idp.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_linkedin_idp.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_add_get_linkedin_idp.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_clone_idp_signing_key.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_clone_idp_signing_key.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_create_get_key.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_create_get_key.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_idp.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_idp.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_key.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_delete_key.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_csr.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_csr.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_idp_signing_key.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_generate_get_idp_signing_key.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idp_signing_keys.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idp_signing_keys.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idps.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_idps.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_keys.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_list_keys.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_revoke_csr.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_revoke_csr.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_update_idp.yaml` & `okta-2.9.6/tests/integration/cassettes/test_identity_providers/TestIdentityProvidersResource.test_update_idp.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_activate_deactivate_inline_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_activate_deactivate_inline_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_create_get_inline_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_create_get_inline_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_delete_inline_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_delete_inline_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_list_inline_hooks.yaml` & `okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_list_inline_hooks.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_update_inline_hook.yaml` & `okta-2.9.6/tests/integration/cassettes/test_inline_hooks_it/TestInlineHooksResource.test_update_inline_hook.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_add_get_linked_object.yaml` & `okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_add_get_linked_object.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_delete_linked_object.yaml` & `okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_delete_linked_object.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_get_all_linked_objects.yaml` & `okta-2.9.6/tests/integration/cassettes/test_linked_objects_it/TestLinkedObjectsResource.test_get_all_linked_objects.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_create_and_delete_network_zone.yaml` & `okta-2.9.6/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_create_and_delete_network_zone.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_list_network_zones.yaml` & `okta-2.9.6/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_list_network_zones.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_update_network_zone.yaml` & `okta-2.9.6/tests/integration/cassettes/test_network_zone_it/TestNetworkZoneResource.test_update_network_zone.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_extend_okta_support.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_extend_okta_support.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_communication_settings.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_communication_settings.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_support_settings.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_okta_support_settings.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_types.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_types.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_contact_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_preferences.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_preferences.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_settings.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_get_org_settings.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_grant_revoke_okta_support.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_grant_revoke_okta_support.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_hide_okta_ui_footer.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_hide_okta_ui_footer.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_in_users_to_okta_communication_emails.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_in_users_to_okta_communication_emails.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_out_users_from_okta_communication_emails.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_opt_out_users_from_okta_communication_emails.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_partial_setting_update.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_partial_setting_update.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_setting_update.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_setting_update.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_show_okta_ui_footer.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_show_okta_ui_footer.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_org_it/TestOrgResource.test_update_org_contact_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_org_it/TestOrgResource.test_update_org_contact_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy_rule.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_activate_deactivate_policy_rule.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_password_policy_rule.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_password_policy_rule.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_rule.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_rule.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_with_group_conditions.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_get_sign_on_policy_with_group_conditions.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_password_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_create_password_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy_rules.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_delete_policy_rules.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policies_by_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policies_by_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policy_rules.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_list_policy_rules.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy_rule.yaml` & `okta-2.9.6/tests/integration/cassettes/test_policies_it/TestPoliciesResource.test_update_policy_rule.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_get_role_subscription_by_notification_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_get_role_subscription_by_notification_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_list_role_subsription.yaml` & `okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_list_role_subsription.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_role_by_notification_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_role_by_notification_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_subscription_it/TestSubscriptionResource.test_subscribe_unsubscribe_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_get_sms_template.yaml` & `okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_get_sms_template.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_list_sms_templates.yaml` & `okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_create_list_sms_templates.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_delete_sms_template.yaml` & `okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_delete_sms_template.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_partial_update_sms_template.yaml` & `okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_partial_update_sms_template.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_update_sms_template.yaml` & `okta-2.9.6/tests/integration/cassettes/test_templates_it/TestTemplatesResource.test_update_sms_template.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_get_threat_insight_configuration.yaml` & `okta-2.9.6/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_get_threat_insight_configuration.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_update_threat_insight_configuration.yaml` & `okta-2.9.6/tests/integration/cassettes/test_threat_insight_it/TestThreatInsightConfiguration.test_update_threat_insight_configuration.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_activate_deactivate_origin.yaml` & `okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_activate_deactivate_origin.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_create_get_origin.yaml` & `okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_create_get_origin.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_delete_origin.yaml` & `okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_delete_origin.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_list_origins.yaml` & `okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_list_origins.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_update_origin.yaml` & `okta-2.9.6/tests/integration/cassettes/test_trusted_origins_it/TestTrustedOriginsResource.test_update_origin.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_get_user_schema.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_get_user_schema.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_update_user_profile.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_schema_it/TestUserSchemaResource.test_update_user_profile.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_create_user_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_create_user_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_delete_user_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_delete_user_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_get_user_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_get_user_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_list_user_types.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_list_user_types.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_replace_user_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_replace_user_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_update_user_type.yaml` & `okta-2.9.6/tests/integration/cassettes/test_user_types_it/TestUserTypesResource.test_update_user_type.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_activate_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_activate_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_assign_user_to_role.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_assign_user_to_role.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_recovery_question.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_recovery_question.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_user_password.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_change_user_password.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_create_get_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_create_get_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_expire_password_get_temporary.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_expire_password_get_temporary.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_get_reset_password_link_for_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_get_reset_password_link_for_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_list_user_subscriptions.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_list_user_subscriptions.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_suspend_user.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_suspend_user.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_update_user_profile.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_update_user_profile.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_group_target_to_role.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_group_target_to_role.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_pagination.yaml` & `okta-2.9.6/tests/integration/cassettes/test_users_it/TestUsersResource.test_user_pagination.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/data/brand_theme_background.png` & `okta-2.9.6/tests/integration/data/brand_theme_background.png`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/data/brand_theme_favicon.ico` & `okta-2.9.6/tests/integration/data/brand_theme_favicon.ico`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/data/brand_theme_logo.png` & `okta-2.9.6/tests/integration/data/brand_theme_logo.png`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/data/logo.png` & `okta-2.9.6/tests/integration/data/logo.png`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_applications_it.py` & `okta-2.9.6/tests/integration/test_applications_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_auth_server_it.py` & `okta-2.9.6/tests/integration/test_auth_server_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_authenticators_it.py` & `okta-2.9.6/tests/integration/test_authenticators_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_brands_it.py` & `okta-2.9.6/tests/integration/test_brands_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_domains_it.py` & `okta-2.9.6/tests/integration/test_domains_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_event_hooks_it.py` & `okta-2.9.6/tests/integration/test_event_hooks_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_factors_it.py` & `okta-2.9.6/tests/integration/test_factors_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_features_it.py` & `okta-2.9.6/tests/integration/test_features_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_group_schema_it.py` & `okta-2.9.6/tests/integration/test_group_schema_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_groups_it.py` & `okta-2.9.6/tests/integration/test_groups_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_identity_providers.py` & `okta-2.9.6/tests/integration/test_identity_providers.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_inline_hooks_it.py` & `okta-2.9.6/tests/integration/test_inline_hooks_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_linked_objects_it.py` & `okta-2.9.6/tests/integration/test_linked_objects_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_log_events_it.py` & `okta-2.9.6/tests/integration/test_log_events_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_network_zone_it.py` & `okta-2.9.6/tests/integration/test_network_zone_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_org_it.py` & `okta-2.9.6/tests/integration/test_org_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_policies_it.py` & `okta-2.9.6/tests/integration/test_policies_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_subscription_it.py` & `okta-2.9.6/tests/integration/test_subscription_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_templates_it.py` & `okta-2.9.6/tests/integration/test_templates_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_threat_insight_it.py` & `okta-2.9.6/tests/integration/test_threat_insight_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_trusted_origins_it.py` & `okta-2.9.6/tests/integration/test_trusted_origins_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_user_schema_it.py` & `okta-2.9.6/tests/integration/test_user_schema_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_user_types_it.py` & `okta-2.9.6/tests/integration/test_user_types_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/integration/test_users_it.py` & `okta-2.9.6/tests/integration/test_users_it.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/mocks.py` & `okta-2.9.6/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_api_response.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_api_response.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_applications_ut.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_applications_ut.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_cache.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_cache.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_client.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_client.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_constants.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_constants.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_domains.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_domains.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_helpers.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_helpers.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_http_client.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_http_client.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_jwt.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_jwt.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_logger.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_logger.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_models.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_models.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_oauth.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_oauth.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_request_executor.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_request_executor.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_retry_logic.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_retry_logic.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_sign_on_modes.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_sign_on_modes.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_user_profile.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_user_profile.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_user_schema.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_user_schema.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/__pycache__/test_utils.cpython-310-pytest-7.4.0.pyc` & `okta-2.9.6/tests/unit/__pycache__/test_utils.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_client_error_call_SSWS.yaml` & `okta-2.9.6/tests/unit/cassettes/test_client_error_call_SSWS.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_client_error_call_oauth.yaml` & `okta-2.9.6/tests/unit/cassettes/test_client_error_call_oauth.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_client_success_call_SSWS.yaml` & `okta-2.9.6/tests/unit/cassettes/test_client_success_call_SSWS.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_create_group_different_inputs[group_obj0].yaml` & `okta-2.9.6/tests/unit/cassettes/test_create_group_different_inputs[group_obj0].yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_create_group_different_inputs[group_obj1].yaml` & `okta-2.9.6/tests/unit/cassettes/test_create_group_different_inputs[group_obj1].yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_create_group_different_inputs[group_obj2].yaml` & `okta-2.9.6/tests/unit/cassettes/test_create_group_different_inputs[group_obj2].yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_error_call_SSWS.yaml` & `okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_error_call_SSWS.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_error_call_oauth.yaml` & `okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_error_call_oauth.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_success_call_SSWS.yaml` & `okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_success_call_SSWS.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_http_client/test_client_success_call_oauth.yaml` & `okta-2.9.6/tests/unit/cassettes/test_http_client/test_client_success_call_oauth.yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj0].yaml` & `okta-2.9.6/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj0].yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj1].yaml` & `okta-2.9.6/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj1].yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj2].yaml` & `okta-2.9.6/tests/unit/cassettes/test_models/test_create_group_different_inputs[group_obj2].yaml`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_api_response.py` & `okta-2.9.6/tests/unit/test_api_response.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_applications_ut.py` & `okta-2.9.6/tests/unit/test_applications_ut.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_cache.py` & `okta-2.9.6/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_client.py` & `okta-2.9.6/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_domains.py` & `okta-2.9.6/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_helpers.py` & `okta-2.9.6/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_http_client.py` & `okta-2.9.6/tests/unit/test_http_client.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_jwt.py` & `okta-2.9.6/tests/unit/test_jwt.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_logger.py` & `okta-2.9.6/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_models.py` & `okta-2.9.6/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_oauth.py` & `okta-2.9.6/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_oauth_clear_access_token.py` & `okta-2.9.6/tests/unit/test_oauth_clear_access_token.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_request_executor.py` & `okta-2.9.6/tests/unit/test_request_executor.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_retry_logic.py` & `okta-2.9.6/tests/unit/test_retry_logic.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_sign_on_modes.py` & `okta-2.9.6/tests/unit/test_sign_on_modes.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_user_profile.py` & `okta-2.9.6/tests/unit/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tests/unit/test_user_schema.py` & `okta-2.9.6/tests/unit/test_user_schema.py`

 * *Files identical despite different names*

### Comparing `okta-2.9.5/tox.ini` & `okta-2.9.6/tox.ini`

 * *Files identical despite different names*

