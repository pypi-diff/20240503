# Comparing `tmp/kiwitcms-github-marketplace-2.4.0.tar.gz` & `tmp/kiwitcms-github-marketplace-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-github-marketplace-2.4.0.tar", last modified: Sat Jan 13 18:40:29 2024, max compression
+gzip compressed data, was "kiwitcms-github-marketplace-2.5.0.tar", last modified: Fri May  3 19:17:32 2024, max compression
```

## Comparing `kiwitcms-github-marketplace-2.4.0.tar` & `kiwitcms-github-marketplace-2.5.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.935677 kiwitcms-github-marketplace-2.4.0/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.4.0/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.4.0/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    12236 2024-01-13 18:40:29.935677 kiwitcms-github-marketplace-2.4.0/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    11291 2024-01-13 18:39:56.000000 kiwitcms-github-marketplace-2.4.0/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    12236 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     1909 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       64 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       50 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       42 2024-01-13 18:40:29.000000 kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       50 2023-06-23 07:56:28.000000 kiwitcms-github-marketplace-2.4.0/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      129 2024-01-13 18:40:29.935677 kiwitcms-github-marketplace-2.4.0/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1783 2024-01-13 18:39:56.000000 kiwitcms-github-marketplace-2.4.0/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.933677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/checks.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/docker.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/mailchimp.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/menu.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     1532 2024-01-05 12:16:28.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0002_update_fields.py
--rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0003_sender_email_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0004_models_jsonfield.py
--rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0007_manualpurchase.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/models.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/quay/
--rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/quay/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/quay/quay_api_client.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     4687 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/quay/quay_session.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.930677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/static/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.930677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/static/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/static/tcms_github_marketplace/js/
--rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.931677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/email/
--rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_tenants/
--rw-rw-r--   0 senko     (1001) senko     (1001)     2562 2021-06-10 13:43:41.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templatetags/github_marketplace.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5632 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)    28019 2023-12-17 14:20:34.000000 kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-01-13 18:40:29.934677 kiwitcms-github-marketplace-2.4.0/tcms_settings_dir/
--rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.4.0/tcms_settings_dir/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.5.0/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    12795 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    11945 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.0/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.620196 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    12795 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     2055 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       64 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       68 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       42 2024-05-03 19:17:32.000000 kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      133 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/requirements.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      129 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1783 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.0/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/checks.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/docker.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/mailchimp.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/menu.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1532 2024-01-05 12:16:28.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0002_update_fields.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0003_sender_email_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0004_models_jsonfield.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0007_manualpurchase.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_api_client.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     4708 2024-04-17 13:31:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_session.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.618196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.618196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.621196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/js/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.618196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/email/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/include/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1030 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
+-rw-r--r--   0 senko     (1001) senko     (1001)      163 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/override_edit.html
+-rw-r--r--   0 senko     (1001) senko     (1001)     2629 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templatetags/github_marketplace.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5632 2023-04-28 11:18:45.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)    28284 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-03 19:17:32.622196 kiwitcms-github-marketplace-2.5.0/tcms_settings_dir/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.0/tcms_settings_dir/__init__.py
```

### Comparing `kiwitcms-github-marketplace-2.4.0/LICENSE` & `kiwitcms-github-marketplace-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/PKG-INFO` & `kiwitcms-github-marketplace-2.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.4.0
+Version: 2.5.0
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: kiwitcms-tenants>=2.0
-Requires-Dist: mailchimp3==3.0.21
-Requires-Dist: requests
 
 Marketplace integrations for Kiwi TCMS
 ======================================
 
 .. image:: https://codecov.io/gh/kiwitcms/github-marketplace/branch/master/graph/badge.svg?token=NQKAQMJ8N8
     :target: https://codecov.io/gh/kiwitcms/github-marketplace
     :alt: Code coverage badge
@@ -83,25 +80,40 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.5.0 (03 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Allow edits to ``Tenant.extra_emails`` field by overriding the HTML templates
+  so we can expose this inside the UI. This new field is shown when creating
+  a new tenant or editing an existing one
+- FastSpring webhooks handler will also try matching the
+  ``Tenant.extra_emails`` field before updating the expiration period.
+  This will handle the situation where ``Tenant.owner`` is no longer the one
+  who pays for the subscription
+- Pin transitive dependencies to reduce the possibility of installing
+  vulnerable packages
+- Fix potentially uninitilized local variable
+- Start using psycopg 3 for testing
+
+
 v2.4.0 (13 Jan 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Build and test with Python 3.11 & fix an import error
 - Update key name for error responses from Quay.io
 - Start testing with upstream Postgres container image, v16 currently.
   Note that installing ``btree_gin`` extension is commented out inside
   ``tcms_github_marketplace/migrations/0001_initial.py``
 
 
-
 v2.3.8 (24 Aug 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Fix a potential crash inside the Subscriptions page
 
 
 v2.3.7 (23 Jun 2023)
```

### Comparing `kiwitcms-github-marketplace-2.4.0/README.rst` & `kiwitcms-github-marketplace-2.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -59,25 +59,40 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.5.0 (03 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Allow edits to ``Tenant.extra_emails`` field by overriding the HTML templates
+  so we can expose this inside the UI. This new field is shown when creating
+  a new tenant or editing an existing one
+- FastSpring webhooks handler will also try matching the
+  ``Tenant.extra_emails`` field before updating the expiration period.
+  This will handle the situation where ``Tenant.owner`` is no longer the one
+  who pays for the subscription
+- Pin transitive dependencies to reduce the possibility of installing
+  vulnerable packages
+- Fix potentially uninitilized local variable
+- Start using psycopg 3 for testing
+
+
 v2.4.0 (13 Jan 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Build and test with Python 3.11 & fix an import error
 - Update key name for error responses from Quay.io
 - Start testing with upstream Postgres container image, v16 currently.
   Note that installing ``btree_gin`` extension is commented out inside
   ``tcms_github_marketplace/migrations/0001_initial.py``
 
 
-
 v2.3.8 (24 Aug 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Fix a potential crash inside the Subscriptions page
 
 
 v2.3.7 (23 Jun 2023)
```

### Comparing `kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/PKG-INFO` & `kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.4.0
+Version: 2.5.0
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: kiwitcms-tenants>=2.0
-Requires-Dist: mailchimp3==3.0.21
-Requires-Dist: requests
 
 Marketplace integrations for Kiwi TCMS
 ======================================
 
 .. image:: https://codecov.io/gh/kiwitcms/github-marketplace/branch/master/graph/badge.svg?token=NQKAQMJ8N8
     :target: https://codecov.io/gh/kiwitcms/github-marketplace
     :alt: Code coverage badge
@@ -83,25 +80,40 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.5.0 (03 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Allow edits to ``Tenant.extra_emails`` field by overriding the HTML templates
+  so we can expose this inside the UI. This new field is shown when creating
+  a new tenant or editing an existing one
+- FastSpring webhooks handler will also try matching the
+  ``Tenant.extra_emails`` field before updating the expiration period.
+  This will handle the situation where ``Tenant.owner`` is no longer the one
+  who pays for the subscription
+- Pin transitive dependencies to reduce the possibility of installing
+  vulnerable packages
+- Fix potentially uninitilized local variable
+- Start using psycopg 3 for testing
+
+
 v2.4.0 (13 Jan 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Build and test with Python 3.11 & fix an import error
 - Update key name for error responses from Quay.io
 - Start testing with upstream Postgres container image, v16 currently.
   Note that installing ``btree_gin`` extension is commented out inside
   ``tcms_github_marketplace/migrations/0001_initial.py``
 
 
-
 v2.3.8 (24 Aug 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Fix a potential crash inside the Subscriptions page
 
 
 v2.3.7 (23 Jun 2023)
```

### Comparing `kiwitcms-github-marketplace-2.4.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt` & `kiwitcms-github-marketplace-2.5.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -33,11 +33,13 @@
 tcms_github_marketplace/quay/__init__.py
 tcms_github_marketplace/quay/quay_api_client.py
 tcms_github_marketplace/quay/quay_session.py
 tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
 tcms_github_marketplace/templates/email/manual_subscription_notification.txt
 tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
 tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
+tcms_github_marketplace/templates/tcms_tenants/override_edit.html
 tcms_github_marketplace/templates/tcms_tenants/override_new.html
+tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
 tcms_github_marketplace/templatetags/__init__.py
 tcms_github_marketplace/templatetags/github_marketplace.py
 tcms_settings_dir/__init__.py
```

### Comparing `kiwitcms-github-marketplace-2.4.0/setup.py` & `kiwitcms-github-marketplace-2.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name="kiwitcms-github-marketplace",
-    version="2.4.0",
+    version="2.5.0",
     description="GitHub Marketplace integration for Kiwi TCMS",
     long_description=get_long_description(),
     author="Kiwi TCMS",
     author_email="info@kiwitcms.org",
     url="https://github.com/kiwitcms/github-marketplace/",
     license="GPLv3+",
     install_requires=get_install_requires("requirements.txt"),
```

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/admin.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/checks.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/docker.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/docker.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/mailchimp.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/mailchimp.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0001_initial.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0002_update_fields.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0002_update_fields.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/migrations/0007_manualpurchase.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/migrations/0007_manualpurchase.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/models.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/models.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/quay/quay_api_client.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_api_client.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/quay/quay_session.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/quay/quay_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,16 @@
 
         Args:
             endpoint (str)
                 API specific endpoint for the request.
         Returns:
             str: Full URL of the endpoint.
         """
+        schema = ""
+
         if self.api == "docker":
             schema = "{0}{1}/v2/{2}"
         elif self.api == "quay":
             schema = "{0}{1}/api/v1/{2}"
 
         if "http://" not in self.hostname and "https://" not in self.hostname:
             return schema.format("https://", self.hostname.rstrip("/"), endpoint)
```

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 {% extends "tcms_tenants/new.html" %}
 {% load i18n %}
 
 {% block extra_contents %}
+    {% include 'tcms_tenants/include/tenant_extra_emails.html' %}
+
     <div class="form-group">
         <label class="col-md-1 col-lg-1">{% trans "Paid until" %}</label>
         <div class="col-sm-11 col-md-8 col-lg-5 {% if form.paid_until.errors %}has-error{% endif %}">
             <label>{{ form.paid_until.value }}</label>
             {{ form.paid_until }}
             {{ form.paid_until.errors }}
         </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "tcms_tenants/new.html" %} {% load i18n %} {% block extra_contents
-%}
+%} {% include 'tcms_tenants/include/tenant_extra_emails.html' %}
 {% trans "Paid until" %}
 {{ form.paid_until.value }} {{ form.paid_until }} {{ form.paid_until.errors }}
 {% trans "Owner" %}
 {{ request.user }} {% if request.user.is_superuser %} (superuser) {% endif %}
 {{ form.organization }} {% if form.organization.value %}
 {% trans 'Organization' %}
 {{ form.organization.value }}
```

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/urls.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/urls.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/utils.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/utils.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.4.0/tcms_github_marketplace/views.py` & `kiwitcms-github-marketplace-2.5.0/tcms_github_marketplace/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=missing-permission-required, no-self-use
 #
-# Copyright (c) 2019-2023 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 #
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 import json
 import os
 from datetime import datetime
 
@@ -292,25 +292,31 @@
     def find_paid_tenant(self, purchase):
         """
         On FastSpring buyers can change their email addresses over time and
         we may end-up in a situation where the email address on a Purchase does
         not match an existing tenant owner. That's why we look into historical
         records and try to find all unique addresses associated with a Customer.
 
+        Also try matching the current ``purchase.sender`` against
+        ``Tenant.extra_emails`` for the situation where ``Tenant.owner`` is no
+        longer the one who pays the subscription.
+
         WARNING: Tenant.organization doesn't matter for FastSpring purchases!
         """
         all_senders = Purchase.objects.filter(
             action="purchased",
             vendor=self.purchase_vendor,
             subscription=purchase.subscription,
         ).values_list("sender", flat=True)
 
         query = super().find_paid_tenant(purchase)
         return query.filter(
-            Q(owner__email__in=all_senders) | Q(owner__username__in=all_senders),
+            Q(owner__email__in=all_senders)
+            | Q(owner__username__in=all_senders)
+            | Q(extra_emails__icontains=purchase.sender),
         )
 
     def find_sku(self, purchase):
         """
         SKU can be found in several different places
         """
         # this method is also called from purchase_should_have_tenant() which
```

