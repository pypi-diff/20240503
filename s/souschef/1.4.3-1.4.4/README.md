# Comparing `tmp/souschef-1.4.3.tar.gz` & `tmp/souschef-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/souschef-1.4.3.tar", last modified: Fri Apr 12 16:09:13 2024, max compression
+gzip compressed data, was "dist/souschef-1.4.4.tar", last modified: Fri May  3 15:49:59 2024, max compression
```

## Comparing `souschef-1.4.3.tar` & `souschef-1.4.4.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/
--rw-r--r--   0 root         (0) root         (0)     5731 2024-02-17 22:37:08.000000 souschef-1.4.3/INSTALL.md
--rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.4.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2261 2024-04-12 16:09:13.000000 souschef-1.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.4.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.4.3/UPDATE.md
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-18 19:41:03.000000 souschef-1.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-12 16:09:13.000000 souschef-1.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1812 2024-04-12 16:08:13.000000 souschef-1.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef/
--rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/admin.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/billing/apps.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/billing/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/billing/migrations/
--rw-r--r--   0 root         (0) root         (0)     1201 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/migrations/0002_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      370 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/migrations/0003_auto_20161122_0515.py
--rw-r--r--   0 root         (0) root         (0)      374 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/migrations/0004_auto_20201030_1540.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5211 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/billing/templates/
--rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/base_billing.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/billing/templates/billing/
--rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/billing/add.html
--rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/billing/billing_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/billing/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/billing/templates/billing/partials/
--rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/billing/partials/statistics.html
--rw-r--r--   0 root         (0) root         (0)     5508 2021-07-16 15:48:25.000000 souschef-1.4.3/souschef/billing/templates/billing/partials/summary.html
--rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/billing/print_summary.html
--rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/billing/templates/billing/view.html
--rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.4.3/souschef/billing/templates/billing/view_orders.html
--rw-r--r--   0 root         (0) root         (0)     8556 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/tests.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/billing/urls.py
--rw-r--r--   0 root         (0) root         (0)    12279 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/billing/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/configsamples/
--rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.4.3/souschef/configsamples/nginx.conf
--rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.4.3/souschef/configsamples/souschef.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/cronscripts/
--rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.4.3/souschef/cronscripts/souschef_daily.sh
--rw-r--r--   0 root         (0) root         (0)      350 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/dataexec.py
--rw-r--r--   0 root         (0) root         (0)    76889 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/dataload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/datamigration/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/datamigration/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/datamigration/admin.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/datamigration/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/datamigration/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.4.3/souschef/datamigration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/datamigration/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.4.3/souschef/datamigration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2026 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/datamigration/management/commands/importaddresses.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/datamigration/management/commands/importclients.py
--rw-r--r--   0 root         (0) root         (0)     2890 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/datamigration/management/commands/importcontactaddresses.py
--rw-r--r--   0 root         (0) root         (0)     4190 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/datamigration/management/commands/importmeals.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/datamigration/management/commands/importorders.py
--rw-r--r--   0 root         (0) root         (0)     3299 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/datamigration/management/commands/importrelationships.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/datamigration/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/datamigration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/datamigration/models.py
--rw-r--r--   0 root         (0) root         (0)     6840 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/datamigration/tests.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/datamigration/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/delivery/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/delivery/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/delivery/admin.py
--rwxr-xr-x   0 root         (0) root         (0)       91 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/delivery/apps.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/delivery/filters.py
--rw-r--r--   0 root         (0) root         (0)     1426 2024-02-17 22:36:40.000000 souschef-1.4.3/souschef/delivery/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/delivery/migrations/
--rw-r--r--   0 root         (0) root         (0)      690 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/delivery/migrations/0001_fix004a.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/delivery/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      232 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/delivery/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/delivery/templates/
--rw-r--r--   0 root         (0) root         (0)    12210 2024-02-19 02:15:16.000000 souschef-1.4.3/souschef/delivery/templates/edit_delivery_route.html
--rw-r--r--   0 root         (0) root         (0)     3686 2024-03-06 02:24:13.000000 souschef-1.4.3/souschef/delivery/templates/ingredients.html
--rw-r--r--   0 root         (0) root         (0)     4380 2024-04-11 01:19:40.000000 souschef-1.4.3/souschef/delivery/templates/kitchen_count.html
--rw-r--r--   0 root         (0) root         (0)     1360 2024-03-06 02:24:13.000000 souschef-1.4.3/souschef/delivery/templates/kitchen_count_steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/delivery/templates/partials/
--rw-r--r--   0 root         (0) root         (0)     2622 2021-03-20 15:32:41.000000 souschef-1.4.3/souschef/delivery/templates/partials/generated_orders.html
--rw-r--r--   0 root         (0) root         (0)     1737 2021-03-19 19:57:48.000000 souschef-1.4.3/souschef/delivery/templates/partials/generated_orders_order_row_content.html
--rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.4.3/souschef/delivery/templates/partials/generated_orders_table_head.html
--rw-r--r--   0 root         (0) root         (0)     5472 2024-03-06 02:24:13.000000 souschef-1.4.3/souschef/delivery/templates/review_orders.html
--rw-r--r--   0 root         (0) root         (0)     3407 2024-02-19 02:15:16.000000 souschef-1.4.3/souschef/delivery/templates/route_sheet.html
--rw-r--r--   0 root         (0) root         (0)     5284 2024-04-09 15:26:23.000000 souschef-1.4.3/souschef/delivery/templates/routes.html
--rwxr-xr-x   0 root         (0) root         (0)    53637 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/delivery/tests.py
--rw-r--r--   0 root         (0) root         (0)     2877 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/delivery/tsp.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-09 15:26:23.000000 souschef-1.4.3/souschef/delivery/urls.py
--rwxr-xr-x   0 root         (0) root         (0)    80902 2024-04-11 01:19:40.000000 souschef-1.4.3/souschef/delivery/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/frontend/images/
--rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/frontend/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/frontend/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/frontend/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/frontend/images/katrina.jpg
--rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/meal/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/meal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-01 00:23:07.000000 souschef-1.4.3/souschef/meal/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/meal/apps.py
--rw-r--r--   0 root         (0) root         (0)     2269 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/meal/migrations/
--rw-r--r--   0 root         (0) root         (0)     7348 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0002_ingredient_ingredient_group.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0003_fix224a.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0004_fix004d.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0006_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0007_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/migrations/0008_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/meal/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8100 2024-04-11 01:19:40.000000 souschef-1.4.3/souschef/meal/models.py
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/meal/settings.py
--rw-r--r--   0 root         (0) root         (0)     8761 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/meal/tests.py
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/meal/urls.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/meal/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/admin.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/member/apps.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/factories.py
--rw-r--r--   0 root         (0) root         (0)    20434 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/member/forms.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/member/formsets.py
--rw-r--r--   0 root         (0) root         (0)      964 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/formsfield.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.4.3/souschef/member/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.4.3/souschef/member/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/member/management/commands/createclients.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/member/management/commands/createnotes.py
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-11 01:19:40.000000 souschef-1.4.3/souschef/member/management/commands/processscheduledstatuschange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/migrations/
--rw-r--r--   0 root         (0) root         (0)    15890 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0002_auto_20160605_1609.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0003_auto_20160615_2100.py
--rw-r--r--   0 root         (0) root         (0)     4445 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0005_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0006_client_meal_default_week.py
--rw-r--r--   0 root         (0) root         (0)      908 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0007_auto_20160726_1703.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0008_auto_20160727_2251.py
--rw-r--r--   0 root         (0) root         (0)      918 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0009_auto_20160728_1443.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0010_auto_20160803_2052.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0011_client_delivery_note.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0012_clientscheduledstatus.py
--rw-r--r--   0 root         (0) root         (0)      754 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0013_auto_20160820_2322.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0014_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0015_route_client_id_sequence.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0016_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0017_auto_20161020_2039.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0018_auto_20161110_2352.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0019_auto_20161111_1750.py
--rw-r--r--   0 root         (0) root         (0)      438 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0020_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0021_auto_20161125_2055.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0022_auto_20161215_1936.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0023_auto_20161220_1401.py
--rw-r--r--   0 root         (0) root         (0)     2680 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0024_auto_20161227_1819.py
--rw-r--r--   0 root         (0) root         (0)      672 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0025_route_vehicle.py
--rw-r--r--   0 root         (0) root         (0)     3723 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0026_change_to_emergency_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1372 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0027_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)     1904 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-04-11 01:19:40.000000 souschef-1.4.3/souschef/member/migrations/0029_member_address_fk_to_1to1.py
--rw-r--r--   0 root         (0) root         (0)     2584 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0030_route_deliveryhistory.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0032_relationship.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0033_auto_20170801_1607.py
--rw-r--r--   0 root         (0) root         (0)      554 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0034_auto_20170816_0850.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0035_auto_20210115_1155.py
--rw-r--r--   0 root         (0) root         (0)     1449 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0036_member_addresses.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0037_one_address_per_member.py
--rw-r--r--   0 root         (0) root         (0)      601 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/member/migrations/0038_member_verbose_names.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28565 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/member/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/signals/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/signals/__init__.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/member/signals/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef/member/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/client/
--rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/client/create/
--rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/create/form.html
--rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/create/steps.html
--rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/client/partials/
--rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/birthdays.html
--rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/filters.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/
--rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/address_information.html
--rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/basic_information.html
--rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/dietary_restriction.html
--rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/meal_defaults.html
--rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/payment_information.html
--rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/relationship_form.html
--rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/forms/relationships.html
--rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/partials/menu.html
--rw-r--r--   0 root         (0) root         (0)     2017 2021-06-18 20:11:28.000000 souschef-1.4.3/souschef/member/templates/client/partials/order_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/client/update/
--rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.4.3/souschef/member/templates/client/update/base.html
--rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.4.3/souschef/member/templates/client/update/status.html
--rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/update/step.html
--rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/update/steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/client/view/
--rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/address.html
--rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/allergies.html
--rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/delete_status_confirmation.html
--rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/information.html
--rw-r--r--   0 root         (0) root         (0)     2716 2021-06-11 15:40:13.000000 souschef-1.4.3/souschef/member/templates/client/view/notes.html
--rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.4.3/souschef/member/templates/client/view/orders.html
--rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/payment.html
--rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/referent.html
--rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/status.html
--rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/client/view/summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/member/templates/route/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/route/delivered_route_detail.html
--rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/route/delivery_history_detail.html
--rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/route/detail.html
--rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/route/edit.html
--rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/member/templates/route/list.html
--rw-r--r--   0 root         (0) root         (0)   160818 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/member/tests.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/member/urls.py
--rw-r--r--   0 root         (0) root         (0)    54776 2024-04-11 01:19:40.000000 souschef-1.4.3/souschef/member/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/note/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/note/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/note/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/note/apps.py
--rw-r--r--   0 root         (0) root         (0)      775 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/factories.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/note/migrations/
--rw-r--r--   0 root         (0) root         (0)     2230 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      607 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0002_auto_20160818_2104.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0003_auto_20160819_2037.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0004_notepriority.py
--rw-r--r--   0 root         (0) root         (0)     1286 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0005_note_priority_old_data_migration.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0006_change_priority_field.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0007_notecategory.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0008_auto_20170116_1441.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0009_auto_20170116_1543.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0010_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      987 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0011_auto_20170419_1109.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0012_note_is_deleted.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0013_date_modified.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/migrations/0014_date_created.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/note/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/note/templates/
--rw-r--r--   0 root         (0) root         (0)      909 2021-07-09 19:21:52.000000 souschef-1.4.3/souschef/note/templates/note_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     1720 2021-07-09 19:00:25.000000 souschef-1.4.3/souschef/note/templates/note_edit.html
--rw-r--r--   0 root         (0) root         (0)     2186 2021-07-09 19:00:30.000000 souschef-1.4.3/souschef/note/templates/notes_add.html
--rw-r--r--   0 root         (0) root         (0)     4080 2021-06-11 15:41:01.000000 souschef-1.4.3/souschef/note/templates/notes_client_list.html
--rw-r--r--   0 root         (0) root         (0)     5780 2021-07-23 15:17:48.000000 souschef-1.4.3/souschef/note/templates/notes_list.html
--rw-r--r--   0 root         (0) root         (0)     9225 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/tests.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/note/urls.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/note/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/notification/admin.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/notification/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/notification/migrations/
--rw-r--r--   0 root         (0) root         (0)     1247 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/notification/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/notification/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2024-02-11 21:15:42.000000 souschef-1.4.3/souschef/notification/models.py
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/notification/tests.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/notification/urls.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/notification/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/order/admin.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/order/apps.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/factories.py
--rw-r--r--   0 root         (0) root         (0)     5183 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.4.3/souschef/order/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.4.3/souschef/order/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/management/commands/createorders.py
--rw-r--r--   0 root         (0) root         (0)     1869 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/management/commands/generateorders.py
--rw-r--r--   0 root         (0) root         (0)     1330 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/management/commands/setordersdelivered.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/migrations/
--rw-r--r--   0 root         (0) root         (0)     4735 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      581 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0002_auto_20160614_1736.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0003_auto_20160615_1504.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      681 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0006_auto_20160803_2217.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0007_remove_order_item_component.py
--rw-r--r--   0 root         (0) root         (0)      633 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0008_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0009_auto_20161012_1919.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0010_auto_20161012_1921.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0011_auto_20161014_1901.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0012_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)     2226 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0013_orderstatuschange.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0014_auto_20161209_2045.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0015_auto_20170410_1029.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0016_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/migrations/0017_total_quantity_not_nullable.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1268 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/order/mixins.py
--rw-r--r--   0 root         (0) root         (0)    46300 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/order/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/templates/
--rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/templates/_form.html
--rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/templates/_order_info.html
--rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/templates/base_order.html
--rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/templates/create.html
--rw-r--r--   0 root         (0) root         (0)     4421 2021-03-26 14:22:55.000000 souschef-1.4.3/souschef/order/templates/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/templates/order/
--rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/templates/order/create_batch.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/order/templates/order/partials/
--rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/order/templates/order/partials/filters.html
--rw-r--r--   0 root         (0) root         (0)     1070 2021-07-09 19:21:52.000000 souschef-1.4.3/souschef/order/templates/order_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.4.3/souschef/order/templates/order_update_status.html
--rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.4.3/souschef/order/templates/update.html
--rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.4.3/souschef/order/templates/view.html
--rw-r--r--   0 root         (0) root         (0)    66186 2024-02-24 23:48:36.000000 souschef-1.4.3/souschef/order/tests.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/order/urls.py
--rw-r--r--   0 root         (0) root         (0)    14652 2024-02-19 02:15:16.000000 souschef-1.4.3/souschef/order/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/page/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/page/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/page/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/page/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/page/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/page/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/page/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef/page/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/page/templates/pages/
--rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/page/templates/pages/card.html
--rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/page/templates/pages/home.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/page/templates/registration/
--rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/page/templates/registration/login.html
--rw-r--r--   0 root         (0) root         (0)    10123 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/page/tests.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/page/urls.py
--rw-r--r--   0 root         (0) root         (0)     4830 2024-04-12 15:39:37.000000 souschef-1.4.3/souschef/page/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/pycrons/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.4.3/souschef/pycrons/__init__.py
--rw-r--r--   0 root         (0) root         (0)      461 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/pycrons/cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/sous_chef/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef/sous_chef/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef/sous_chef/assets/css/
--rw-r--r--   0 root         (0) root         (0)   655527 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/css/main.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/
--rw-r--r--   0 root         (0) root         (0)    98640 2024-04-12 16:08:51.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.eot
--rw-r--r--   0 root         (0) root         (0)   507628 2024-04-12 16:08:51.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.svg
--rw-r--r--   0 root         (0) root         (0)    98404 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    63728 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.woff
--rw-r--r--   0 root         (0) root         (0)    54488 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.woff2
--rw-r--r--   0 root         (0) root         (0)   106004 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.eot
--rw-r--r--   0 root         (0) root         (0)    93888 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.otf
--rw-r--r--   0 root         (0) root         (0)   390837 2024-04-12 16:08:56.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.svg
--rw-r--r--   0 root         (0) root         (0)   105784 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.ttf
--rw-r--r--   0 root         (0) root         (0)    50524 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.woff
--rw-r--r--   0 root         (0) root         (0)    40148 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.woff2
--rw-r--r--   0 root         (0) root         (0)    31156 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.eot
--rw-r--r--   0 root         (0) root         (0)   107201 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.svg
--rw-r--r--   0 root         (0) root         (0)    30928 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    14712 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.woff
--rw-r--r--   0 root         (0) root         (0)    12240 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/assets/images/
--rw-r--r--   0 root         (0) root         (0)   258972 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    11449 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/demo.png
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/favicon.png
--rw-r--r--   0 root         (0) root         (0)    28123 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/images/flags.png
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/images/geocoder.png
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/glyph-marker-icon.png
--rw-r--r--   0 root         (0) root         (0)     1287 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/glyph-marker-icon.svg
--rw-r--r--   0 root         (0) root         (0)    21977 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    26952 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/katrina.jpg
--rw-r--r--   0 root         (0) root         (0)     2306 2024-04-12 16:08:56.000000 souschef-1.4.3/souschef/sous_chef/assets/images/leaflet.routing.icons.png
--rw-r--r--   0 root         (0) root         (0)     4060 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
--rw-r--r--   0 root         (0) root         (0)     6363 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/logo-souschef-coul.png
--rw-r--r--   0 root         (0) root         (0)     6033 2024-04-12 16:09:08.000000 souschef-1.4.3/souschef/sous_chef/assets/images/logo-souschef-nb.png
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-12 16:09:08.000000 souschef-1.4.3/souschef/sous_chef/assets/images/logo.png
--rw-r--r--   0 root         (0) root         (0)    14323 2024-04-12 16:09:05.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-matte.png
--rw-r--r--   0 root         (0) root         (0)    30194 2024-04-12 16:09:05.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-matte@2x.png
--rw-r--r--   0 root         (0) root         (0)     7946 2024-04-12 16:09:05.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-plain.png
--rw-r--r--   0 root         (0) root         (0)      535 2024-04-12 16:09:05.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-shadow.png
--rw-r--r--   0 root         (0) root         (0)     1134 2024-04-12 16:09:05.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-shadow@2x.png
--rw-r--r--   0 root         (0) root         (0)    36367 2024-04-12 16:09:05.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-soft.png
--rw-r--r--   0 root         (0) root         (0)   146362 2024-04-12 16:09:07.000000 souschef-1.4.3/souschef/sous_chef/assets/images/markers-soft@2x.png
--rw-r--r--   0 root         (0) root         (0)      454 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/images/routing-icon.png
--rw-r--r--   0 root         (0) root         (0)     4831 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/images/throbber.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/assets/js/
--rw-r--r--   0 root         (0) root         (0)  1031323 2024-04-12 16:08:52.000000 souschef-1.4.3/souschef/sous_chef/assets/js/leaflet.js
--rw-r--r--   0 root         (0) root         (0)   627692 2024-04-12 16:08:55.000000 souschef-1.4.3/souschef/sous_chef/assets/js/leaflet.min.js
--rw-r--r--   0 root         (0) root         (0)    22295 2024-04-12 16:08:51.000000 souschef-1.4.3/souschef/sous_chef/assets/js/multidatespicker.js
--rw-r--r--   0 root         (0) root         (0)    10453 2024-04-12 16:08:51.000000 souschef-1.4.3/souschef/sous_chef/assets/js/multidatespicker.min.js
--rw-r--r--   0 root         (0) root         (0)  1111829 2024-04-12 16:08:58.000000 souschef-1.4.3/souschef/sous_chef/assets/js/sous-chef.js
--rw-r--r--   0 root         (0) root         (0)   399694 2024-04-12 16:09:04.000000 souschef-1.4.3/souschef/sous_chef/assets/js/sous-chef.min.js
--rw-r--r--   0 root         (0) root         (0)     1518 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/formats/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/formats/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/formats/en/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/formats/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/formats/en/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/formats/fr/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/formats/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      141 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/formats/fr/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/management/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/management/commands/makemessages.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/rules.py
--rw-r--r--   0 root         (0) root         (0)     7507 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/settings.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/sous_chef/settings_test.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/sous_chef/settings_test_fr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/templates/
--rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/templates/avatar/
--rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/avatar/change.html
--rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/avatar/confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3656 2021-07-23 15:25:58.000000 souschef-1.4.3/souschef/sous_chef/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/templates/dashboard/
--rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/dashboard/statistics.html
--rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/splash.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/templates/system/
--rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/system/_button_export.html
--rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templates/system/breadcrumb.html
--rw-r--r--   0 root         (0) root         (0)     2878 2021-07-09 19:03:35.000000 souschef-1.4.3/souschef/sous_chef/templates/system/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:13.000000 souschef-1.4.3/souschef/sous_chef/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/sous_chef/templatetags/sous_chef_extras.py
--rw-r--r--   0 root         (0) root         (0)     3420 2024-02-18 19:41:03.000000 souschef-1.4.3/souschef/sous_chef/tests.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-26 21:47:13.000000 souschef-1.4.3/souschef/sous_chef/urls.py
--rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.4.3/souschef/sous_chef/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:09:12.000000 souschef-1.4.3/souschef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2261 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15624 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 16:09:11.000000 souschef-1.4.3/souschef.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/
+-rw-r--r--   0 root         (0) root         (0)     5731 2024-02-17 22:37:08.000000 souschef-1.4.4/INSTALL.md
+-rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.4.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-05-03 15:49:59.000000 souschef-1.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.4.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.4.4/UPDATE.md
+-rw-r--r--   0 root         (0) root         (0)      249 2024-02-18 19:41:03.000000 souschef-1.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-03 15:49:59.000000 souschef-1.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-05-03 15:48:16.000000 souschef-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/
+-rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/admin.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/billing/apps.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/billing/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      459 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0002_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      370 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0003_auto_20161122_0515.py
+-rw-r--r--   0 root         (0) root         (0)      374 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/migrations/0004_auto_20201030_1540.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/templates/
+-rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/base_billing.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/templates/billing/
+-rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/add.html
+-rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/billing_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/billing/templates/billing/partials/
+-rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/partials/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     5508 2021-07-16 15:48:25.000000 souschef-1.4.4/souschef/billing/templates/billing/partials/summary.html
+-rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/print_summary.html
+-rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/billing/templates/billing/view.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.4.4/souschef/billing/templates/billing/view_orders.html
+-rw-r--r--   0 root         (0) root         (0)     8556 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/tests.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/billing/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12279 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/billing/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/configsamples/
+-rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.4.4/souschef/configsamples/nginx.conf
+-rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.4.4/souschef/configsamples/souschef.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/cronscripts/
+-rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.4.4/souschef/cronscripts/souschef_daily.sh
+-rw-r--r--   0 root         (0) root         (0)      350 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/dataexec.py
+-rw-r--r--   0 root         (0) root         (0)    76889 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/dataload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/datamigration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/admin.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.4.4/souschef/datamigration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.4.4/souschef/datamigration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importclients.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importcontactaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importmeals.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importorders.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/datamigration/management/commands/importrelationships.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/datamigration/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/datamigration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/models.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/datamigration/tests.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/datamigration/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/delivery/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/delivery/admin.py
+-rwxr-xr-x   0 root         (0) root         (0)       91 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/delivery/apps.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/delivery/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2024-02-17 22:36:40.000000 souschef-1.4.4/souschef/delivery/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/migrations/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/delivery/migrations/0001_fix004a.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/delivery/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      232 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/delivery/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/templates/
+-rw-r--r--   0 root         (0) root         (0)    12210 2024-02-19 02:15:16.000000 souschef-1.4.4/souschef/delivery/templates/edit_delivery_route.html
+-rw-r--r--   0 root         (0) root         (0)     3686 2024-03-06 02:24:13.000000 souschef-1.4.4/souschef/delivery/templates/ingredients.html
+-rw-r--r--   0 root         (0) root         (0)     4380 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/delivery/templates/kitchen_count.html
+-rw-r--r--   0 root         (0) root         (0)     1360 2024-03-06 02:24:13.000000 souschef-1.4.4/souschef/delivery/templates/kitchen_count_steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/delivery/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/templates/partials/generated_orders.html
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_order_row_content.html
+-rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_table_head.html
+-rw-r--r--   0 root         (0) root         (0)     5472 2024-03-06 02:24:13.000000 souschef-1.4.4/souschef/delivery/templates/review_orders.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2024-02-19 02:15:16.000000 souschef-1.4.4/souschef/delivery/templates/route_sheet.html
+-rw-r--r--   0 root         (0) root         (0)     5284 2024-04-09 15:26:23.000000 souschef-1.4.4/souschef/delivery/templates/routes.html
+-rwxr-xr-x   0 root         (0) root         (0)    53737 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/delivery/tsp.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-09 15:26:23.000000 souschef-1.4.4/souschef/delivery/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)    80975 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/delivery/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/frontend/images/
+-rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/frontend/images/katrina.jpg
+-rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/meal/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/meal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-01 00:23:07.000000 souschef-1.4.4/souschef/meal/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/meal/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7348 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0002_ingredient_ingredient_group.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0003_fix224a.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0004_fix004d.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0006_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0007_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/migrations/0008_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/meal/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/meal/models.py
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/settings.py
+-rw-r--r--   0 root         (0) root         (0)     8761 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/meal/tests.py
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/urls.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/meal/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/admin.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/apps.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/factories.py
+-rw-r--r--   0 root         (0) root         (0)    20424 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/member/forms.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/formsets.py
+-rw-r--r--   0 root         (0) root         (0)      964 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/formsfield.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.4.4/souschef/member/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.4.4/souschef/member/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/management/commands/createclients.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/management/commands/createnotes.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/member/management/commands/processscheduledstatuschange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/migrations/
+-rw-r--r--   0 root         (0) root         (0)    15890 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0002_auto_20160605_1609.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0003_auto_20160615_2100.py
+-rw-r--r--   0 root         (0) root         (0)     4445 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0005_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0006_client_meal_default_week.py
+-rw-r--r--   0 root         (0) root         (0)      908 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0007_auto_20160726_1703.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0008_auto_20160727_2251.py
+-rw-r--r--   0 root         (0) root         (0)      918 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0009_auto_20160728_1443.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0010_auto_20160803_2052.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0011_client_delivery_note.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0012_clientscheduledstatus.py
+-rw-r--r--   0 root         (0) root         (0)      754 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0013_auto_20160820_2322.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0014_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0015_route_client_id_sequence.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0016_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0017_auto_20161020_2039.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0018_auto_20161110_2352.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0019_auto_20161111_1750.py
+-rw-r--r--   0 root         (0) root         (0)      438 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0020_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0021_auto_20161125_2055.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0022_auto_20161215_1936.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0023_auto_20161220_1401.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0024_auto_20161227_1819.py
+-rw-r--r--   0 root         (0) root         (0)      672 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0025_route_vehicle.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0026_change_to_emergency_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0027_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/member/migrations/0029_member_address_fk_to_1to1.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0030_route_deliveryhistory.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0032_relationship.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0033_auto_20170801_1607.py
+-rw-r--r--   0 root         (0) root         (0)      554 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0034_auto_20170816_0850.py
+-rw-r--r--   0 root         (0) root         (0)      866 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0035_auto_20210115_1155.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0036_member_addresses.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0037_one_address_per_member.py
+-rw-r--r--   0 root         (0) root         (0)      601 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/member/migrations/0038_member_verbose_names.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29870 2024-05-03 15:39:44.000000 souschef-1.4.4/souschef/member/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/signals/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/signals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/signals/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/
+-rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/create/
+-rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/create/form.html
+-rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/create/steps.html
+-rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/partials/
+-rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/birthdays.html
+-rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/filters.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/
+-rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/address_information.html
+-rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/basic_information.html
+-rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/dietary_restriction.html
+-rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/meal_defaults.html
+-rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/payment_information.html
+-rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/relationship_form.html
+-rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/forms/relationships.html
+-rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/partials/menu.html
+-rw-r--r--   0 root         (0) root         (0)     2017 2021-06-18 20:11:28.000000 souschef-1.4.4/souschef/member/templates/client/partials/order_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/update/
+-rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.4.4/souschef/member/templates/client/update/base.html
+-rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.4.4/souschef/member/templates/client/update/status.html
+-rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/update/step.html
+-rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/update/steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/client/view/
+-rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/address.html
+-rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/allergies.html
+-rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/delete_status_confirmation.html
+-rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/information.html
+-rw-r--r--   0 root         (0) root         (0)     2716 2021-06-11 15:40:13.000000 souschef-1.4.4/souschef/member/templates/client/view/notes.html
+-rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.4.4/souschef/member/templates/client/view/orders.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/payment.html
+-rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/referent.html
+-rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/status.html
+-rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/client/view/summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/member/templates/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/delivered_route_detail.html
+-rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/delivery_history_detail.html
+-rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/detail.html
+-rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/edit.html
+-rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/member/templates/route/list.html
+-rw-r--r--   0 root         (0) root         (0)   165842 2024-05-03 15:46:57.000000 souschef-1.4.4/souschef/member/tests.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/member/urls.py
+-rw-r--r--   0 root         (0) root         (0)    54776 2024-04-11 01:19:40.000000 souschef-1.4.4/souschef/member/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/note/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/note/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/note/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/note/apps.py
+-rw-r--r--   0 root         (0) root         (0)      775 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/factories.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/note/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      607 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0002_auto_20160818_2104.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0003_auto_20160819_2037.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0004_notepriority.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0005_note_priority_old_data_migration.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0006_change_priority_field.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0007_notecategory.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0008_auto_20170116_1441.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0009_auto_20170116_1543.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0010_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      987 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0011_auto_20170419_1109.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0012_note_is_deleted.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0013_date_modified.py
+-rw-r--r--   0 root         (0) root         (0)      495 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/migrations/0014_date_created.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/note/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/note/templates/
+-rw-r--r--   0 root         (0) root         (0)      909 2021-07-09 19:21:52.000000 souschef-1.4.4/souschef/note/templates/note_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     1720 2021-07-09 19:00:25.000000 souschef-1.4.4/souschef/note/templates/note_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2186 2021-07-09 19:00:30.000000 souschef-1.4.4/souschef/note/templates/notes_add.html
+-rw-r--r--   0 root         (0) root         (0)     4080 2021-06-11 15:41:01.000000 souschef-1.4.4/souschef/note/templates/notes_client_list.html
+-rw-r--r--   0 root         (0) root         (0)     5780 2021-07-23 15:17:48.000000 souschef-1.4.4/souschef/note/templates/notes_list.html
+-rw-r--r--   0 root         (0) root         (0)     9225 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/tests.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/note/urls.py
+-rw-r--r--   0 root         (0) root         (0)     5709 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/note/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/admin.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/notification/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/notification/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/notification/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2024-02-11 21:15:42.000000 souschef-1.4.4/souschef/notification/models.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/tests.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/urls.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/notification/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/order/admin.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/order/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/factories.py
+-rw-r--r--   0 root         (0) root         (0)     5183 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.4.4/souschef/order/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.4.4/souschef/order/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/management/commands/createorders.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/management/commands/generateorders.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/management/commands/setordersdelivered.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4735 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      581 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0002_auto_20160614_1736.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0003_auto_20160615_1504.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      681 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0006_auto_20160803_2217.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0007_remove_order_item_component.py
+-rw-r--r--   0 root         (0) root         (0)      633 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0008_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0009_auto_20161012_1919.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0010_auto_20161012_1921.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0011_auto_20161014_1901.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0012_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0013_orderstatuschange.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0014_auto_20161209_2045.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0015_auto_20170410_1029.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0016_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/migrations/0017_total_quantity_not_nullable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/order/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    47013 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/order/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/templates/
+-rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/_form.html
+-rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/_order_info.html
+-rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/base_order.html
+-rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/create.html
+-rw-r--r--   0 root         (0) root         (0)     4481 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/order/templates/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/templates/order/
+-rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/order/create_batch.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/order/templates/order/partials/
+-rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/order/templates/order/partials/filters.html
+-rw-r--r--   0 root         (0) root         (0)     1070 2021-07-09 19:21:52.000000 souschef-1.4.4/souschef/order/templates/order_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.4.4/souschef/order/templates/order_update_status.html
+-rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.4.4/souschef/order/templates/update.html
+-rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.4.4/souschef/order/templates/view.html
+-rw-r--r--   0 root         (0) root         (0)    66186 2024-02-24 23:48:36.000000 souschef-1.4.4/souschef/order/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/order/urls.py
+-rw-r--r--   0 root         (0) root         (0)    14652 2024-02-19 02:15:16.000000 souschef-1.4.4/souschef/order/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/page/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/page/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/page/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/templates/pages/
+-rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/templates/pages/card.html
+-rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/templates/pages/home.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/page/templates/registration/
+-rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/page/templates/registration/login.html
+-rw-r--r--   0 root         (0) root         (0)    10143 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/page/tests.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/page/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-05-03 15:36:47.000000 souschef-1.4.4/souschef/page/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/pycrons/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.4.4/souschef/pycrons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/pycrons/cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/css/
+-rw-r--r--   0 root         (0) root         (0)   655527 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/css/main.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/
+-rw-r--r--   0 root         (0) root         (0)    98640 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   507628 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    98404 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    63728 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff
+-rw-r--r--   0 root         (0) root         (0)    54488 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)   106004 2024-05-03 15:49:33.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.eot
+-rw-r--r--   0 root         (0) root         (0)    93888 2024-05-03 15:49:33.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.otf
+-rw-r--r--   0 root         (0) root         (0)   390837 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.svg
+-rw-r--r--   0 root         (0) root         (0)   105784 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    50524 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff
+-rw-r--r--   0 root         (0) root         (0)    40148 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff2
+-rw-r--r--   0 root         (0) root         (0)    31156 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.eot
+-rw-r--r--   0 root         (0) root         (0)   107201 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.svg
+-rw-r--r--   0 root         (0) root         (0)    30928 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)    14712 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff
+-rw-r--r--   0 root         (0) root         (0)    12240 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/images/
+-rw-r--r--   0 root         (0) root         (0)   258972 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    11449 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/demo.png
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    28123 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/images/flags.png
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/images/geocoder.png
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.png
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.svg
+-rw-r--r--   0 root         (0) root         (0)    21977 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    26952 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/katrina.jpg
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-05-03 15:49:36.000000 souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.png
+-rw-r--r--   0 root         (0) root         (0)     4060 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
+-rw-r--r--   0 root         (0) root         (0)     6363 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-coul.png
+-rw-r--r--   0 root         (0) root         (0)     6033 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-nb.png
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-03 15:49:48.000000 souschef-1.4.4/souschef/sous_chef/assets/images/logo.png
+-rw-r--r--   0 root         (0) root         (0)    14323 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte.png
+-rw-r--r--   0 root         (0) root         (0)    30194 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte@2x.png
+-rw-r--r--   0 root         (0) root         (0)     7946 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-plain.png
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow.png
+-rw-r--r--   0 root         (0) root         (0)     1134 2024-05-03 15:49:46.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow@2x.png
+-rw-r--r--   0 root         (0) root         (0)    36367 2024-05-03 15:49:46.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft.png
+-rw-r--r--   0 root         (0) root         (0)   146362 2024-05-03 15:49:47.000000 souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft@2x.png
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-03 15:49:37.000000 souschef-1.4.4/souschef/sous_chef/assets/images/routing-icon.png
+-rw-r--r--   0 root         (0) root         (0)     4831 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/images/throbber.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/assets/js/
+-rw-r--r--   0 root         (0) root         (0)  1031323 2024-05-03 15:49:33.000000 souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.js
+-rw-r--r--   0 root         (0) root         (0)   627692 2024-05-03 15:49:36.000000 souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.min.js
+-rw-r--r--   0 root         (0) root         (0)    22295 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.js
+-rw-r--r--   0 root         (0) root         (0)    10453 2024-05-03 15:49:32.000000 souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.min.js
+-rw-r--r--   0 root         (0) root         (0)  1111829 2024-05-03 15:49:39.000000 souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.js
+-rw-r--r--   0 root         (0) root         (0)   399694 2024-05-03 15:49:45.000000 souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.min.js
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/formats/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/formats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/formats/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/formats/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/formats/en/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/formats/fr/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/formats/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      141 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/formats/fr/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/management/commands/makemessages.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/rules.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/settings.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/settings_test.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/settings_test_fr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/
+-rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/avatar/
+-rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/avatar/change.html
+-rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/avatar/confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3656 2021-07-23 15:25:58.000000 souschef-1.4.4/souschef/sous_chef/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/dashboard/
+-rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/dashboard/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/splash.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templates/system/
+-rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/system/_button_export.html
+-rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templates/system/breadcrumb.html
+-rw-r--r--   0 root         (0) root         (0)     2878 2021-07-09 19:03:35.000000 souschef-1.4.4/souschef/sous_chef/templates/system/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef/sous_chef/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/templatetags/sous_chef_extras.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-02-18 19:41:03.000000 souschef-1.4.4/souschef/sous_chef/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-26 21:47:13.000000 souschef-1.4.4/souschef/sous_chef/urls.py
+-rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.4.4/souschef/sous_chef/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15624 2024-05-03 15:49:59.000000 souschef-1.4.4/souschef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      476 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-03 15:49:58.000000 souschef-1.4.4/souschef.egg-info/top_level.txt
```

### Comparing `souschef-1.4.3/INSTALL.md` & `souschef-1.4.4/INSTALL.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/LICENSE.txt` & `souschef-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/PKG-INFO` & `souschef-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.4.3
+Version: 1.4.4
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/santropolroulant/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Keywords: meals-on-wheel
 Platform: UNKNOWN
```

### Comparing `souschef-1.4.3/README.md` & `souschef-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/UPDATE.md` & `souschef-1.4.4/UPDATE.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/setup.py` & `souschef-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="souschef",
-    version="1.4.3",
+    version="1.4.4",
     license="AGPL-3.0",
     author="Santropol Roulant and Savoir Faire Linux",
     author_email="info@santropolroulant.org",
     description="Webapp used to manage orders for meals-on-wheel delivery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/santropolroulant/sous-chef",
```

### Comparing `souschef-1.4.3/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg` & `souschef-1.4.4/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/migrations/0001_initial.py` & `souschef-1.4.4/souschef/billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/models.py` & `souschef-1.4.4/souschef/billing/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/add.html` & `souschef-1.4.4/souschef/billing/templates/billing/add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/billing_confirm_delete.html` & `souschef-1.4.4/souschef/billing/templates/billing/billing_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/list.html` & `souschef-1.4.4/souschef/billing/templates/billing/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/partials/statistics.html` & `souschef-1.4.4/souschef/billing/templates/billing/partials/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/partials/summary.html` & `souschef-1.4.4/souschef/billing/templates/billing/partials/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/print_summary.html` & `souschef-1.4.4/souschef/billing/templates/billing/print_summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/view.html` & `souschef-1.4.4/souschef/billing/templates/billing/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/templates/billing/view_orders.html` & `souschef-1.4.4/souschef/billing/templates/billing/view_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/tests.py` & `souschef-1.4.4/souschef/billing/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/urls.py` & `souschef-1.4.4/souschef/billing/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/billing/views.py` & `souschef-1.4.4/souschef/billing/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/configsamples/nginx.conf` & `souschef-1.4.4/souschef/configsamples/nginx.conf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/dataload.py` & `souschef-1.4.4/souschef/dataload.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/management/commands/importaddresses.py` & `souschef-1.4.4/souschef/datamigration/management/commands/importaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/management/commands/importclients.py` & `souschef-1.4.4/souschef/datamigration/management/commands/importclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/management/commands/importcontactaddresses.py` & `souschef-1.4.4/souschef/datamigration/management/commands/importcontactaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/management/commands/importmeals.py` & `souschef-1.4.4/souschef/datamigration/management/commands/importmeals.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/management/commands/importorders.py` & `souschef-1.4.4/souschef/datamigration/management/commands/importorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/management/commands/importrelationships.py` & `souschef-1.4.4/souschef/datamigration/management/commands/importrelationships.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/datamigration/tests.py` & `souschef-1.4.4/souschef/datamigration/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.assertEqual(dorothy.status, Client.ACTIVE)
         self.assertEqual(dorothy.birthdate, date(1938, 10, 10))
         self.assertEqual(
             date(created.year, created.month, created.day), date(2007, 9, 26)
         )
         self.assertEqual(dorothy.gender, "F")
         self.assertEqual(dorothy.language, "EN")
-        self.assertEqual(dorothy.delivery_type, "O")
+        self.assertEqual(dorothy.delivery_type, Client.ONGOING_DELIVERY)
         self.assertEqual(dorothy.route.name, "McGill")
         self.assertEqual(dorothy.delivery_note, "Code entree: 17")
         self.assertEqual(dorothy.alert, "communicate with her sister")
 
     def test_import_member_status(self):
         self.assertEqual(Client.active.all().count(), 2)
         self.assertEqual(Client.ongoing.all().count(), 2)
```

### Comparing `souschef-1.4.3/souschef/delivery/filters.py` & `souschef-1.4.4/souschef/delivery/filters.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/forms.py` & `souschef-1.4.4/souschef/delivery/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/migrations/0001_fix004a.py` & `souschef-1.4.4/souschef/delivery/migrations/0001_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/edit_delivery_route.html` & `souschef-1.4.4/souschef/delivery/templates/edit_delivery_route.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/ingredients.html` & `souschef-1.4.4/souschef/delivery/templates/ingredients.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/kitchen_count.html` & `souschef-1.4.4/souschef/delivery/templates/kitchen_count.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/kitchen_count_steps.html` & `souschef-1.4.4/souschef/delivery/templates/kitchen_count_steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/partials/generated_orders.html` & `souschef-1.4.4/souschef/delivery/templates/partials/generated_orders.html`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 {% has_perm 'sous_chef.edit' request.user as can_edit_data %}
 {% if has_ordered_orders %}
 <table id="generated-orders-table" class="ui very basic stripped compact celled table">
   {% include 'partials/generated_orders_table_head.html' %}
   <tbody>
     {# Display orders in error at top #}
     {% for order in orders %}
-      {% if order.status == 'O' and order.client.is_in_error_for_the_kitchen_count %}
+      {% if order.status == 'O' and order.is_in_error_for_the_kitchen_count %}
       <tr class="error">
         {% include 'partials/generated_orders_order_row_content.html' %}
       </tr>
       {% endif %}
     {% endfor %}
 
     {# Then display orders not in error #}
     {% for order in orders %}
-      {% if order.status == 'O' and not order.client.is_in_error_for_the_kitchen_count %}
+      {% if order.status == 'O' and not order.is_in_error_for_the_kitchen_count %}
       <tr>
         {% include 'partials/generated_orders_order_row_content.html' %}
       </tr>
       {% endif %}
     {% endfor %}
   </tbody>
 </table>
@@ -41,16 +41,16 @@
   <tbody>
     {% for order in orders %}
     {% if order.status == 'C' %}
       <tr class="warning">
         <td class="center aligned"><strong><i class="hashtag icon"></i>{{order.id}}</strong></td>
         <td>
           <a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client.member}}</a>
-          {% if order.client.status != 'A' %}
-          ({{ order.client.status_verbose }})
+          {% if order.client_planned_status_at_delivery != 'A' %}
+          ({{ order.client_planned_status_at_delivery_verbose }})
           {% endif %}
         </td>
         <td>{{order.delivery_date}}</td>
         <td>{{order.client.route}}</td>
         <td class="center aligned">{{order.get_status_display}}</td>
         <td class="center aligned"><i class="dollar icon"></i>{{order.price}}</td>
         <td>
```

#### html2text {}

```diff
@@ -3,17 +3,17 @@
 {% has_perm 'sous_chef.edit' request.user as can_edit_data %} {% if
 has_ordered_orders %}
 {% endif %} {% if has_cancelled_orders %}
 ********** {{%% ttrraannss ""CCaanncceelllleedd OOrrddeerrss"" %%}} **********
 {% trans 'These clients will not receive a meal today, but their order can be
 enabled if needed (by viewing the order and setting the status to "Ordered").'
 %}
-            _{_{_o_r_d_e_r_._c_l_i_e_n_t_._m_e_m_b_e_r_}_} {%
-            if order.client.status !=
-{{           'A' %} ({                   {                      {                     {                           {
-{{oorrddeerr..iidd}}}} {                           {order.delivery_date}} {order.client.route}} {order.get_status_display}} {order.price}}
-            order.client.status_verbose
+            _{_{_o_r_d_e_r_._c_l_i_e_n_t_._m_e_m_b_e_r_}_} {% if
+            order.client_planned_status_at_delivery != 'A'
+{{           %} ({                                           {                      {                     {                           {
+{{oorrddeerr..iidd}}}} {                                               {order.delivery_date}} {order.client.route}} {order.get_status_display}} {order.price}}
+            order.client_planned_status_at_delivery_verbose
             }}) {% endif %}
 {% endif %} {% if not has_ordered_orders and not has_cancelled_orders %}
 {% trans 'No orders found.' %}
 {% endif %} {% if can_edit_data %}
 {% endif %}
```

### Comparing `souschef-1.4.3/souschef/delivery/templates/partials/generated_orders_order_row_content.html` & `souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_order_row_content.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load i18n %}
 
 <td class="center aligned"><strong><i class="hashtag icon"></i>{{order.id}}</strong></td>
 <td>
   <a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client.member}}</a>
-  {% if order.client.status != 'A' %}
-  ({{ order.client.status_verbose }})
+  {% if order.client_planned_status_at_delivery != 'A' %}
+  ({{ order.client_planned_status_at_delivery_verbose }})
   {% endif %}
 </td>
 <td>{{order.delivery_date}}</td>
 <td>
   {% if order.client.route %}
     {{order.client.route}}
     {% if not order.client.is_geolocalized %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% load i18n %}
 {{{{oorrddeerr..iidd}}}}
-_{_{_o_r_d_e_r_._c_l_i_e_n_t_._m_e_m_b_e_r_}_} {% if order.client.status != 'A' %} ({
-{ order.client.status_verbose }}) {% endif %}
+_{_{_o_r_d_e_r_._c_l_i_e_n_t_._m_e_m_b_e_r_}_} {% if order.client_planned_status_at_delivery != 'A' %}
+({{ order.client_planned_status_at_delivery_verbose }}) {% endif %}
 {{order.delivery_date}}
 {% if order.client.route %} {{order.client.route}} {% if not
 order.client.is_geolocalized %} {% endif %} {% else %} {% endif %}
 {{order.get_status_display}}
 {{order.price}}
 {% if can_edit_data %} {% endif %}
```

### Comparing `souschef-1.4.3/souschef/delivery/templates/partials/generated_orders_table_head.html` & `souschef-1.4.4/souschef/delivery/templates/partials/generated_orders_table_head.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/review_orders.html` & `souschef-1.4.4/souschef/delivery/templates/review_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/route_sheet.html` & `souschef-1.4.4/souschef/delivery/templates/route_sheet.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/templates/routes.html` & `souschef-1.4.4/souschef/delivery/templates/routes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/tests.py` & `souschef-1.4.4/souschef/delivery/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,15 +861,15 @@
         for day, _ in DAYS_OF_WEEK:
             for key_tmpl, value in data.items():
                 meals_default[key_tmpl.format(day)] = value
 
         ongoing_clients = ClientFactory.create_batch(
             10,
             status=Client.ACTIVE,
-            delivery_type="O",
+            delivery_type=Client.ONGOING_DELIVERY,
             meal_default_week=meals_default,
             route=RouteFactory(),
         )
 
         # The meal schedule should exclude today.
         schedule_delivery = []
         weekday = datetime.date.today().weekday()
@@ -933,47 +933,47 @@
             "dessert_wednesday_quantity": 1,
         }
         cls.route1 = RouteFactory()
         cls.route2 = RouteFactory()
         cls.c_valid = ClientFactory(
             pk=10,
             status=Client.ACTIVE,
-            delivery_type="O",  # ongoing
+            delivery_type=Client.ONGOING_DELIVERY,  # ongoing
             route=cls.route1,
             meal_default_week=meal_default_week,
             member=MemberFactory(
                 firstname="Valid", lastname="Valid", address=AddressFactory()
             ),
         )
         cls.c_nr = ClientFactory(
             pk=20,
             status=Client.ACTIVE,
-            delivery_type="O",  # ongoing
+            delivery_type=Client.ONGOING_DELIVERY,  # ongoing
             route=None,
             meal_default_week=meal_default_week,
             member=MemberFactory(
                 firstname="Nronly", lastname="Nronly", address=AddressFactory()
             ),
         )
         cls.c_ng = ClientFactory(
             pk=30,
             status=Client.ACTIVE,
-            delivery_type="O",  # ongoing
+            delivery_type=Client.ONGOING_DELIVERY,  # ongoing
             route=cls.route2,
             meal_default_week=meal_default_week,
             member=MemberFactory(
                 firstname="Ngonly",
                 lastname="Ngonly",
                 address=AddressFactory(latitude=None),
             ),
         )
         cls.c_nrng = ClientFactory(
             pk=40,
             status=Client.ACTIVE,
-            delivery_type="O",  # ongoing
+            delivery_type=Client.ONGOING_DELIVERY,  # ongoing
             route=None,
             meal_default_week=meal_default_week,
             member=MemberFactory(
                 firstname="Nrng",
                 lastname="Nrng",
                 address=AddressFactory(longitude=None),
             ),
```

### Comparing `souschef-1.4.3/souschef/delivery/tsp.py` & `souschef-1.4.4/souschef/delivery/tsp.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/urls.py` & `souschef-1.4.4/souschef/delivery/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/delivery/views.py` & `souschef-1.4.4/souschef/delivery/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
+
 import collections
 import json
 import os
 import textwrap
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import date, datetime
 from pathlib import Path
-from typing import List
 
 import labels  # package pylabels
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin.models import LogEntry
 from django.contrib.auth.mixins import (
     LoginRequiredMixin,
@@ -58,14 +59,15 @@
     Menu,
     Menu_component,
 )
 from souschef.member.models import (
     Client,
     DeliveryHistory,
     Route,
+    get_ongoing_clients_at_date,
 )
 from souschef.order.models import (
     ORDER_STATUS_CANCELLED,
     ORDER_STATUS_ORDERED,
     SIZE_CHOICES_LARGE,
     SIZE_CHOICES_REGULAR,
     Order,
@@ -127,15 +129,15 @@
     return len([o for o in orders if o.status == status])
 
 
 def get_has_orders_in_status(orders, status):
     return get_number_of_orders_in_status(orders, status) > 0
 
 
-def get_kitchen_count_context(delivery_date):
+def get_kitchen_count_context(delivery_date: date):
     orders = get_orders_for_kitchen_count(
         delivery_date=delivery_date,
         order_statuses=(ORDER_STATUS_ORDERED, ORDER_STATUS_CANCELLED),
     )
 
     return {
         "orders": orders,
@@ -1410,15 +1412,15 @@
     return f"{lastname}, {firstname[:2]}."
 
 
 @dataclass
 class PreparationLine:
     preparation_method: str
     quantity: int
-    client_names: List[str]
+    client_names: list[str]
 
 
 def kcr_make_preparation_lines(kitchen_list, client_filter):
     """Get food preparation method for clients not having clashing (incompatible)
     ingredients."""
     if client_filter == "only_clients_with_incompatible_ingredients":
 
@@ -2242,13 +2244,13 @@
 
 class RefreshOrderView(LoginRequiredMixin, PermissionRequiredMixin, generic.View):
     permission_required = "sous_chef.edit"
 
     def post(self, request):
         delivery_date = to_delivery_date(request.POST["generateOrderDate"])
         if delivery_date and delivery_date >= datetime.now().date():
-            clients = Client.ongoing.all()
+            clients = get_ongoing_clients_at_date(delivery_date)
             Order.objects.auto_create_orders(delivery_date, clients)
         else:
             print(f"RefreshOrderView: Invalid date provided: {delivery_date}")
         context = get_kitchen_count_context(delivery_date)
         return render(request, "partials/generated_orders.html", context)
```

### Comparing `souschef-1.4.3/souschef/frontend/images/bg1.jpg` & `souschef-1.4.4/souschef/frontend/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/frontend/images/jenny.jpg` & `souschef-1.4.4/souschef/frontend/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/frontend/images/joe.jpg` & `souschef-1.4.4/souschef/frontend/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/frontend/images/katrina.jpg` & `souschef-1.4.4/souschef/frontend/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/admin.py` & `souschef-1.4.4/souschef/meal/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/factories.py` & `souschef-1.4.4/souschef/meal/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0001_fix161f.py` & `souschef-1.4.4/souschef/meal/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0002_ingredient_ingredient_group.py` & `souschef-1.4.4/souschef/meal/migrations/0002_ingredient_ingredient_group.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0003_fix224a.py` & `souschef-1.4.4/souschef/meal/migrations/0003_fix224a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0005_fix241b.py` & `souschef-1.4.4/souschef/meal/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0006_auto_20160826_0007.py` & `souschef-1.4.4/souschef/meal/migrations/0006_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0007_auto_20170313_1442.py` & `souschef-1.4.4/souschef/meal/migrations/0007_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/migrations/0008_auto_20180704_1613.py` & `souschef-1.4.4/souschef/meal/migrations/0008_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/models.py` & `souschef-1.4.4/souschef/meal/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/meal/tests.py` & `souschef-1.4.4/souschef/meal/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/admin.py` & `souschef-1.4.4/souschef/member/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/factories.py` & `souschef-1.4.4/souschef/member/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/forms.py` & `souschef-1.4.4/souschef/member/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         This only applies to ongoing clients!
 
         Regardless of meal schedules, when a main dish is set, we should
         enforce the setting of its size.
         """
         super().clean()
 
-        if self.cleaned_data.get("delivery_type") == "O":
+        if self.cleaned_data.get("delivery_type") == Client.ONGOING_DELIVERY:
             # Ongoing
             meals_schedule = self.cleaned_data.get("meals_schedule")
             if meals_schedule is None:
                 meals_schedule = []
         else:
             # Episodic
             meals_schedule = []
@@ -275,17 +275,15 @@
                             "delivery."
                         )
                         % {"weekday": day_displays[day]},
                     )
 
         for day, _day_display in DAYS_OF_WEEK:
             # If the main dish is set, size should also be set.
-            main_dish_quantity = self.cleaned_data.get(
-                f"main_dish_{day}_quantity"
-            )
+            main_dish_quantity = self.cleaned_data.get(f"main_dish_{day}_quantity")
             fieldname_size = f"size_{day}"
             if main_dish_quantity and not self.cleaned_data.get(fieldname_size):
                 self.add_error(
                     fieldname_size, _("Size is required when the main dish is set.")
                 )
```

### Comparing `souschef-1.4.3/souschef/member/formsfield.py` & `souschef-1.4.4/souschef/member/formsfield.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/management/commands/createclients.py` & `souschef-1.4.4/souschef/member/management/commands/createclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/management/commands/processscheduledstatuschange.py` & `souschef-1.4.4/souschef/member/management/commands/processscheduledstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0001_fix161f.py` & `souschef-1.4.4/souschef/member/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0002_auto_20160605_1609.py` & `souschef-1.4.4/souschef/member/migrations/0002_auto_20160605_1609.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0003_auto_20160615_2100.py` & `souschef-1.4.4/souschef/member/migrations/0003_auto_20160615_2100.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0004_fix004a.py` & `souschef-1.4.4/souschef/member/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0005_fix004a.py` & `souschef-1.4.4/souschef/member/migrations/0005_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0007_auto_20160726_1703.py` & `souschef-1.4.4/souschef/member/migrations/0007_auto_20160726_1703.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0009_auto_20160728_1443.py` & `souschef-1.4.4/souschef/member/migrations/0009_auto_20160728_1443.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0012_clientscheduledstatus.py` & `souschef-1.4.4/souschef/member/migrations/0012_clientscheduledstatus.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0013_auto_20160820_2322.py` & `souschef-1.4.4/souschef/member/migrations/0013_auto_20160820_2322.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0014_auto_20160826_0007.py` & `souschef-1.4.4/souschef/member/migrations/0014_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0016_auto_20160912_1509.py` & `souschef-1.4.4/souschef/member/migrations/0016_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0017_auto_20161020_2039.py` & `souschef-1.4.4/souschef/member/migrations/0017_auto_20161020_2039.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0018_auto_20161110_2352.py` & `souschef-1.4.4/souschef/member/migrations/0018_auto_20161110_2352.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0019_auto_20161111_1750.py` & `souschef-1.4.4/souschef/member/migrations/0019_auto_20161111_1750.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0022_auto_20161215_1936.py` & `souschef-1.4.4/souschef/member/migrations/0022_auto_20161215_1936.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0023_auto_20161220_1401.py` & `souschef-1.4.4/souschef/member/migrations/0023_auto_20161220_1401.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0024_auto_20161227_1819.py` & `souschef-1.4.4/souschef/member/migrations/0024_auto_20161227_1819.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0025_route_vehicle.py` & `souschef-1.4.4/souschef/member/migrations/0025_route_vehicle.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0026_change_to_emergency_contacts.py` & `souschef-1.4.4/souschef/member/migrations/0026_change_to_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0027_auto_20170313_1442.py` & `souschef-1.4.4/souschef/member/migrations/0027_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py` & `souschef-1.4.4/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0029_member_address_fk_to_1to1.py` & `souschef-1.4.4/souschef/member/migrations/0029_member_address_fk_to_1to1.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0030_route_deliveryhistory.py` & `souschef-1.4.4/souschef/member/migrations/0030_route_deliveryhistory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0031_client_option_allow_reverse_relation.py` & `souschef-1.4.4/souschef/member/migrations/0031_client_option_allow_reverse_relation.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0032_relationship.py` & `souschef-1.4.4/souschef/member/migrations/0032_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0033_auto_20170801_1607.py` & `souschef-1.4.4/souschef/member/migrations/0033_auto_20170801_1607.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0034_auto_20170816_0850.py` & `souschef-1.4.4/souschef/member/migrations/0034_auto_20170816_0850.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0035_auto_20210115_1155.py` & `souschef-1.4.4/souschef/member/migrations/0035_auto_20210115_1155.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0036_member_addresses.py` & `souschef-1.4.4/souschef/member/migrations/0036_member_addresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0037_one_address_per_member.py` & `souschef-1.4.4/souschef/member/migrations/0037_one_address_per_member.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/migrations/0038_member_verbose_names.py` & `souschef-1.4.4/souschef/member/migrations/0038_member_verbose_names.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/models.py` & `souschef-1.4.4/souschef/member/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import json
 
 from annoying.fields import JSONField
 from django.db import models
 from django.db.models import Q
 from django.db.models.functions import Extract
@@ -426,24 +428,41 @@
                 Q(status=Client.ACTIVE)
                 | Q(status=Client.PAUSED)
                 | Q(status=Client.PENDING)
             )
         )
 
 
+def get_ongoing_clients_at_date(
+    the_date: datetime.date, today: datetime.date | None = None
+) -> list["Client"]:  # noqa: UP037
+    today = today or datetime.date.today()
+
+    # This way of doing things will not work with a very large client database.
+    # Hard-to-write optimized SQL queries would be required.
+    return [
+        client
+        for client in Client.objects.filter(delivery_type="O")
+        if client.get_status_planned_at_date(the_date, today) == Client.ACTIVE
+    ]
+
+
 class Client(models.Model):
     # Characters are used to keep a backward-compatibility
     # with the previous system.
     PENDING = "D"
     ACTIVE = "A"
     PAUSED = "S"
     STOPNOCONTACT = "N"
     STOPCONTACT = "C"
     DECEASED = "I"
 
+    ONGOING_DELIVERY = "O"
+    EPISODIC_DELIVERY = "E"
+
     CLIENT_STATUS = (
         (PENDING, _("Pending")),
         (ACTIVE, _("Active")),
         (PAUSED, _("Paused")),
         (STOPNOCONTACT, _("Stop: no contact")),
         (STOPCONTACT, _("Stop: contact")),
         (DECEASED, _("Deceased")),
@@ -578,17 +597,21 @@
             2000, self.birthdate.month, self.birthdate.day
         ) <= datetime.date(2000, today.month, today.day):
             age = today.year - self.birthdate.year
         else:
             age = today.year - self.birthdate.year - 1
         return age
 
+    @classmethod
+    def get_verbose_status(cls, status: str) -> str:
+        return dict(cls.CLIENT_STATUS).get(status, _("Unknown"))
+
     @property
     def status_verbose(self):
-        return dict(self.CLIENT_STATUS).get(self.status, _("Unknown"))
+        return self.get_verbose_status(self.status)
 
     @property
     def delivery_type_verbose(self):
         return dict(DELIVERY_TYPE).get(self.delivery_type, _("Unknown"))
 
     @property
     def orders(self):
@@ -680,47 +703,69 @@
         Intended to be called only for Ongoing clients. For episodic clients
         or if `simple_meals_schedule` is not set, it returns empty tuple.
         """
         defaults = self.meals_default
         prefs = []
         simple_meals_schedule = self.simple_meals_schedule
 
-        if self.delivery_type == "E" or simple_meals_schedule is None:
+        if (
+            self.delivery_type == self.EPISODIC_DELIVERY
+            or simple_meals_schedule is None
+        ):
             return ()
         else:
             for day, meal_schedule in defaults:
                 if day in simple_meals_schedule:
                     prefs.append((day, meal_schedule))
             return prefs
 
-    @property
-    def is_in_error_for_the_kitchen_count(self):
-        """Return True if the client is in error for the Kitchen Count
-        orders list page.
-
-        The client is in error if either:
-        - is not not geolocalized;
-        - it has no route;
-        - it is not active.
-        """
-        return not self.is_geolocalized or not self.route or self.status != "A"
-
     def set_simple_meals_schedule(self, schedule):
         """
         Set the delivery days for the client.
         @param schedule
             A python list of days.
         """
         meal_schedule_option, _ = Option.objects.get_or_create(name="meals_schedule")
         client_option, _ = Client_option.objects.update_or_create(
             client=self,
             option=meal_schedule_option,
             defaults={"value": json.dumps(schedule)},
         )
 
+    def get_status_planned_at_date(
+        self, the_date: datetime.date, today: datetime.date | None = None
+    ):
+        """
+        Get the planned `status` the client will have at date `the_date`.
+
+        Applies the latest scheduled `ClientScheduledStatus` and return the resulting
+        state.
+
+        `today` can be overriden for unit tests.
+        """
+        today = today or datetime.date.today()
+
+        planned_status = self.status
+
+        status_changes = (
+            self.scheduled_statuses.filter(
+                change_date__gte=today,
+                change_date__lte=the_date,
+                change_state=ClientScheduledStatus.END,
+                operation_status=ClientScheduledStatus.TOBEPROCESSED,
+            )
+            .order_by("-change_date")
+            .all()
+        )
+
+        if status_changes:
+            planned_status = status_changes[0].status_to
+
+        return planned_status
+
 
 class ClientScheduledStatus(models.Model):
     START = "START"
     END = "END"
 
     CHANGE_STATUS = (
         (START, _("Start")),
```

### Comparing `souschef-1.4.3/souschef/member/templates/client/base.html` & `souschef-1.4.4/souschef/member/templates/client/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/create/form.html` & `souschef-1.4.4/souschef/member/templates/client/create/form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/create/steps.html` & `souschef-1.4.4/souschef/member/templates/client/create/steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/list.html` & `souschef-1.4.4/souschef/member/templates/client/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/birthdays.html` & `souschef-1.4.4/souschef/member/templates/client/partials/birthdays.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/filters.html` & `souschef-1.4.4/souschef/member/templates/client/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/address_information.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/address_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/basic_information.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/basic_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/dietary_restriction.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/dietary_restriction.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/meal_defaults.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/meal_defaults.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/payment_information.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/payment_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/relationship_form.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/relationship_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/forms/relationships.html` & `souschef-1.4.4/souschef/member/templates/client/partials/forms/relationships.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/menu.html` & `souschef-1.4.4/souschef/member/templates/client/partials/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/partials/order_list.html` & `souschef-1.4.4/souschef/member/templates/client/partials/order_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/update/base.html` & `souschef-1.4.4/souschef/member/templates/client/update/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/update/status.html` & `souschef-1.4.4/souschef/member/templates/client/update/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/allergies.html` & `souschef-1.4.4/souschef/member/templates/client/view/allergies.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/delete_status_confirmation.html` & `souschef-1.4.4/souschef/member/templates/client/view/delete_status_confirmation.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/information.html` & `souschef-1.4.4/souschef/member/templates/client/view/information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/notes.html` & `souschef-1.4.4/souschef/member/templates/client/view/notes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/orders.html` & `souschef-1.4.4/souschef/member/templates/client/view/orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/payment.html` & `souschef-1.4.4/souschef/member/templates/client/view/payment.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/referent.html` & `souschef-1.4.4/souschef/member/templates/client/view/referent.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/status.html` & `souschef-1.4.4/souschef/member/templates/client/view/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/client/view/summary.html` & `souschef-1.4.4/souschef/member/templates/client/view/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/route/delivery_history_detail.html` & `souschef-1.4.4/souschef/member/templates/route/delivery_history_detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/route/detail.html` & `souschef-1.4.4/souschef/member/templates/route/detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/route/edit.html` & `souschef-1.4.4/souschef/member/templates/route/edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/templates/route/list.html` & `souschef-1.4.4/souschef/member/templates/route/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/tests.py` & `souschef-1.4.4/souschef/member/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -328,15 +328,15 @@
 
 class ClientMealDefaultWeekTestCase(TestCase):
     fixtures = ["routes"]
 
     @classmethod
     def setUpTestData(cls):
         cls.clientTest = ClientFactory(
-            delivery_type="O",
+            delivery_type=Client.ONGOING_DELIVERY,
             meal_default_week={
                 "main_dish_monday_quantity": 1,
                 "size_monday": "R",
                 "diabetic_monday_quantity": 2,
                 "fruit_salad_monday_quantity": 1,
                 "main_dish_tuesday_quantity": 0,
                 "size_tuesday": "L",
@@ -725,15 +725,15 @@
             "payment_information-postal_code": "H2C 3G4",
             "wizard_goto_step": "",
         }
 
         restriction_information_data = {
             "client_wizard-current_step": "dietary_restriction",
             "dietary_restriction-status": "on",
-            "dietary_restriction-delivery_type": "O",
+            "dietary_restriction-delivery_type": Client.ONGOING_DELIVERY,
             "dietary_restriction-meals_schedule": ["monday", "wednesday"],
             "dietary_restriction-meal_default": "1",
             "dietary_restriction-restrictions": [
                 self.restricted_item_1.id,
                 self.restricted_item_2.id,
             ],
             "dietary_restriction-food_preparation": self.food_preparation.id,
@@ -818,15 +818,15 @@
         # test_client_birthdate:
         self.assertEqual(client.birthdate, date(1990, 12, 12))
 
         # test_client_gender:
         self.assertEqual(client.gender, "M")
 
         # test client delivery type
-        self.assertEqual(client.delivery_type, "O")
+        self.assertEqual(client.delivery_type, Client.ONGOING_DELIVERY)
 
         # test_relationship_name:
         self.assertEqual(
             client.relationship_set.first().member.firstname, "Relationship"
         )
         self.assertEqual(client.relationship_set.first().member.lastname, "Testing")
 
@@ -1392,15 +1392,15 @@
         )
 
     def _test_step_dietary_restriction_without_errors(self):
         # Data for the address_information step without errors.
         restriction_information_data = {
             "client_wizard-current_step": "dietary_restriction",
             "dietary_restriction-status": "on",
-            "dietary_restriction-delivery_type": "O",
+            "dietary_restriction-delivery_type": Client.ONGOING_DELIVERY,
             "dietary_restriction-meals_schedule": "monday",
             "dietary_restriction-meal_default": "1",
             "wizard_goto_step": "",
         }
         for day in [restriction_information_data["dietary_restriction-meals_schedule"]]:
             restriction_information_data[f"dietary_restriction-size_{day}"] = "R"
             for component, _ in COMPONENT_GROUP_CHOICES:
@@ -2295,15 +2295,15 @@
         data = load_initial_data(client)
         # Make sure the status stays unchanged
         status = client.status
         # Update some data
         data.update(
             {
                 "status": "A",
-                "delivery_type": "O",
+                "delivery_type": Client.ONGOING_DELIVERY,
                 "meals_schedule": ["monday"],
             }
         )
         for day in data["meals_schedule"]:
             data[f"size_{day}"] = "R"
             for component, _ in COMPONENT_GROUP_CHOICES:
                 name = f"{component}_{day}_quantity"
@@ -2321,30 +2321,30 @@
             follow=True,
         )
         self.assertEqual(response.status_code, 200)
 
         # Reload client data as it should have been changed in the database
         client = Client.objects.get(id=client.id)
         self.assertEqual(client.status, status)
-        self.assertEqual(client.delivery_type, "O")
+        self.assertEqual(client.delivery_type, Client.ONGOING_DELIVERY)
 
     def test_meal_default_should_be_set_for_scheduled_delivery_days(self):
         """
         On delivery days, at least one of the quantities should be set for an
         ongoing client.
         """
         client = ClientFactory()
         data = load_initial_data(client)
         form = ClientRestrictionsInformation(data=data)
         self.assertFalse(form.is_valid())
 
         data.update(
             {
                 "status": client.status == Client.ACTIVE,
-                "delivery_type": "O",
+                "delivery_type": Client.ONGOING_DELIVERY,
                 "meals_schedule": ["monday"],
             }
         )
         for day in ["tuesday", "sunday"]:
             data[f"size_{day}"] = "R"
             for component, _ in COMPONENT_GROUP_CHOICES:
                 name = f"{component}_{day}_quantity"
@@ -3025,14 +3025,135 @@
         url = reverse("member:clientStatusScheduler", kwargs={"pk": client.id})
         # Run
         response = self.client.get(url)
         # Check
         self.assertEqual(response.status_code, 200)
 
 
+class ClientGetStatusPlannedAtDateTestCase(SousChefTestMixin, TestCase):
+    fixtures = ["routes.json"]
+    TODAY = date(2024, 4, 29)
+
+    def setUp(self):
+        self.client = ClientFactory()
+        self.client.status = Client.ACTIVE
+        # ensure client has no scheduled changes -- otherwise our tests won't work
+        self.assertFalse(self.client.scheduled_statuses.all())
+
+    def test_no_planned_changes__active_client(self):
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY, today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.ACTIVE)
+
+    def test_no_planned_changes__paused_client(self):
+        self.client.status = Client.PAUSED
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY, today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.PAUSED)
+
+    def test_planned_change_before_date(self):
+        change1 = ClientScheduledStatus.objects.create(
+            client=self.client,
+            status_from=Client.ACTIVE,
+            status_to=Client.PAUSED,
+            reason="test",
+            change_date=self.TODAY - timedelta(days=10),
+            change_state=ClientScheduledStatus.END,
+            operation_status=ClientScheduledStatus.TOBEPROCESSED,
+        )
+        ClientScheduledStatus.objects.create(
+            client=self.client,
+            status_from=Client.PAUSED,
+            status_to=Client.ACTIVE,
+            reason="test",
+            change_date=self.TODAY - timedelta(days=1),
+            change_state=ClientScheduledStatus.END,
+            operation_status=ClientScheduledStatus.TOBEPROCESSED,
+            pair=change1,
+        )
+        # Scheduled status is not considered because it is in the past
+        # (and was never processed)
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY, today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.ACTIVE)
+
+    def test_planned_change_after_date(self):
+        change1 = ClientScheduledStatus.objects.create(
+            client=self.client,
+            status_from=Client.ACTIVE,
+            status_to=Client.PAUSED,
+            reason="test",
+            change_date=self.TODAY + timedelta(days=1),
+            change_state=ClientScheduledStatus.END,
+            operation_status=ClientScheduledStatus.TOBEPROCESSED,
+        )
+        ClientScheduledStatus.objects.create(
+            client=self.client,
+            status_from=Client.PAUSED,
+            status_to=Client.ACTIVE,
+            reason="test",
+            change_date=self.TODAY + timedelta(days=10),
+            change_state=ClientScheduledStatus.END,
+            operation_status=ClientScheduledStatus.TOBEPROCESSED,
+            pair=change1,
+        )
+        # Scheduled status is not considered because it is after the provided date
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY, today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.ACTIVE)
+
+    def test_planned_change_in_range(self):
+        change1 = ClientScheduledStatus.objects.create(
+            client=self.client,
+            status_from=Client.ACTIVE,
+            status_to=Client.PAUSED,
+            reason="test",
+            change_date=self.TODAY + timedelta(days=1),
+            change_state=ClientScheduledStatus.END,
+            operation_status=ClientScheduledStatus.TOBEPROCESSED,
+        )
+        ClientScheduledStatus.objects.create(
+            client=self.client,
+            status_from=Client.PAUSED,
+            status_to=Client.STOPCONTACT,
+            reason="test",
+            change_date=self.TODAY + timedelta(days=10),
+            change_state=ClientScheduledStatus.END,
+            operation_status=ClientScheduledStatus.TOBEPROCESSED,
+            pair=change1,
+        )
+        # Scheduled status is considered because it is in the range scheduled changes
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY + timedelta(days=1), today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.PAUSED)
+
+        # status is planned to go to STOPCONTACT on TODAY + 10 days
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY + timedelta(days=10), today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.STOPCONTACT)
+
+        # status will be STOPCONTACT in 11 days
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY + timedelta(days=11), today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.STOPCONTACT)
+
+        # As tested before, "today" the client is ACTIVE
+        planned_status = self.client.get_status_planned_at_date(
+            self.TODAY, today=self.TODAY
+        )
+        self.assertEqual(planned_status, Client.ACTIVE)
+
+
 class DeleteRestrictionViewTestCase(SousChefTestMixin, TestCase):
     fixtures = ["routes.json"]
 
     def test_redirects_users_who_do_not_have_edit_permission(self):
         # Setup
         user = User.objects.create_user(
             username="foo", email="foo@example.com", password="secure"
```

### Comparing `souschef-1.4.3/souschef/member/urls.py` & `souschef-1.4.4/souschef/member/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/member/views.py` & `souschef-1.4.4/souschef/member/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/admin.py` & `souschef-1.4.4/souschef/note/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/factories.py` & `souschef-1.4.4/souschef/note/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/forms.py` & `souschef-1.4.4/souschef/note/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0001_initial.py` & `souschef-1.4.4/souschef/note/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0002_auto_20160818_2104.py` & `souschef-1.4.4/souschef/note/migrations/0002_auto_20160818_2104.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0004_notepriority.py` & `souschef-1.4.4/souschef/note/migrations/0004_notepriority.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0005_note_priority_old_data_migration.py` & `souschef-1.4.4/souschef/note/migrations/0005_note_priority_old_data_migration.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0007_notecategory.py` & `souschef-1.4.4/souschef/note/migrations/0007_notecategory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0008_auto_20170116_1441.py` & `souschef-1.4.4/souschef/note/migrations/0008_auto_20170116_1441.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0009_auto_20170116_1543.py` & `souschef-1.4.4/souschef/note/migrations/0009_auto_20170116_1543.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0010_auto_20170313_1442.py` & `souschef-1.4.4/souschef/note/migrations/0010_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0011_auto_20170419_1109.py` & `souschef-1.4.4/souschef/note/migrations/0011_auto_20170419_1109.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/migrations/0013_date_modified.py` & `souschef-1.4.4/souschef/note/migrations/0013_date_modified.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/models.py` & `souschef-1.4.4/souschef/note/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/templates/note_confirm_delete.html` & `souschef-1.4.4/souschef/note/templates/note_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/templates/note_edit.html` & `souschef-1.4.4/souschef/note/templates/note_edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/templates/notes_add.html` & `souschef-1.4.4/souschef/note/templates/notes_add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/templates/notes_client_list.html` & `souschef-1.4.4/souschef/note/templates/notes_client_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/templates/notes_list.html` & `souschef-1.4.4/souschef/note/templates/notes_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/tests.py` & `souschef-1.4.4/souschef/note/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/urls.py` & `souschef-1.4.4/souschef/note/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/note/views.py` & `souschef-1.4.4/souschef/note/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/notification/migrations/0001_fix161f.py` & `souschef-1.4.4/souschef/notification/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/notification/models.py` & `souschef-1.4.4/souschef/notification/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/admin.py` & `souschef-1.4.4/souschef/order/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/factories.py` & `souschef-1.4.4/souschef/order/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/forms.py` & `souschef-1.4.4/souschef/order/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/management/commands/generateorders.py` & `souschef-1.4.4/souschef/order/management/commands/generateorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/management/commands/setordersdelivered.py` & `souschef-1.4.4/souschef/order/management/commands/setordersdelivered.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0001_fix161f.py` & `souschef-1.4.4/souschef/order/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0002_auto_20160614_1736.py` & `souschef-1.4.4/souschef/order/migrations/0002_auto_20160614_1736.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0003_auto_20160615_1504.py` & `souschef-1.4.4/souschef/order/migrations/0003_auto_20160615_1504.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0004_fix004a.py` & `souschef-1.4.4/souschef/order/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0005_fix241b.py` & `souschef-1.4.4/souschef/order/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0006_auto_20160803_2217.py` & `souschef-1.4.4/souschef/order/migrations/0006_auto_20160803_2217.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0008_auto_20160912_1509.py` & `souschef-1.4.4/souschef/order/migrations/0008_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0009_auto_20161012_1919.py` & `souschef-1.4.4/souschef/order/migrations/0009_auto_20161012_1919.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0011_auto_20161014_1901.py` & `souschef-1.4.4/souschef/order/migrations/0011_auto_20161014_1901.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0013_orderstatuschange.py` & `souschef-1.4.4/souschef/order/migrations/0013_orderstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0014_auto_20161209_2045.py` & `souschef-1.4.4/souschef/order/migrations/0014_auto_20161209_2045.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0015_auto_20170410_1029.py` & `souschef-1.4.4/souschef/order/migrations/0015_auto_20170410_1029.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/migrations/0016_auto_20180704_1613.py` & `souschef-1.4.4/souschef/order/migrations/0016_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/mixins.py` & `souschef-1.4.4/souschef/order/mixins.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/models.py` & `souschef-1.4.4/souschef/order/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,16 +165,16 @@
     def auto_create_orders(self, delivery_date, clients):
         """
         Automatically creates orders and order items for the given delivery
         date and given client list.
         Order items will be created based on client's meals schedule.
 
         Parameters:
-          delivery_date : date on which orders are to be delivered
-          clients : a list of one or many client objects
+          delivery_date: date on which orders are to be delivered
+          clients: a list of one or many client objects
 
         Returns:
           Created orders.
         """
         created_orders = []
         weekday = delivery_date.weekday()  # Monday is 0, Sunday is 6
         day = DAYS_OF_WEEK[weekday][0]  # 0 -> 'monday', 6 -> 'sunday'
@@ -663,14 +663,38 @@
             if self.includes_a_bill is True:
                 for item in self.orders.all():
                     if item.is_a_client_bill:
                         item.delete()
         else:
             raise ValueError("Order.includes_a_bill only accepts " "boolean values.")
 
+    @property
+    def client_planned_status_at_delivery(self):
+        return self.client.get_status_planned_at_date(self.delivery_date)
+
+    @property
+    def client_planned_status_at_delivery_verbose(self):
+        return self.client.get_verbose_status(self.client_planned_status_at_delivery)
+
+    @property
+    def is_in_error_for_the_kitchen_count(self):
+        """Return True if the order is in error for the Kitchen Count
+        orders list page.
+
+        This is based on the client, which either:
+        - is not geolocalized;
+        - has no route;
+        - is not active at the delivery date.
+        """
+        return (
+            not self.client.is_geolocalized
+            or not self.client.route
+            or self.client_planned_status_at_delivery != "A"
+        )
+
 
 # Order.get_kitchen_items helper functions.
 
 
 def named_tuple_fetchall(cursor):
     """Fetch all rows from a database 'cursor', returning namedtuples.
 
@@ -951,23 +975,23 @@
       meal_menu.id AS menuid,
       meal_menu_component.id AS mencomid,
       meal_component.id AS component_id, meal_component.component_group,
       meal_component.name AS component_name
     FROM member_member
       JOIN member_client ON member_client.member_id = member_member.id
       JOIN member_route ON member_route.id = member_client.route_id
-      JOIN meal_menu ON meal_menu.date =                      %(delivery_date)s
+      JOIN meal_menu ON meal_menu.date = %(delivery_date)s
       JOIN order_order ON order_order.client_id = member_client.id
       JOIN order_order_item ON order_order_item.order_id = order_order.id
       JOIN meal_menu_component ON meal_menu_component.menu_id = meal_menu.id
       JOIN meal_component ON
         meal_component.id = meal_menu_component.component_id AND
-          meal_component.component_group = order_order_item.component_group
-    WHERE order_order.delivery_date =                     %(delivery_date)s AND
-      order_order.status !=                                 %(order_cancelled)s
+        meal_component.component_group = order_order_item.component_group
+    WHERE order_order.delivery_date = %(delivery_date)s AND
+      order_order.status != %(order_cancelled)s
     ORDER BY member_member.lastname, member_member.firstname
     """
     values = {
         "delivery_date": delivery_date,
         "order_cancelled": ORDER_STATUS_CANCELLED,
     }
     return sql_exec(query, values, "****** Delivery List ******")
```

### Comparing `souschef-1.4.3/souschef/order/templates/_form.html` & `souschef-1.4.4/souschef/order/templates/_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/_order_info.html` & `souschef-1.4.4/souschef/order/templates/_order_info.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/create.html` & `souschef-1.4.4/souschef/order/templates/create.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/list.html` & `souschef-1.4.4/souschef/order/templates/list.html`

 * *Files 5% similar despite different names*

```diff
@@ -50,20 +50,20 @@
     <th class="">{% trans 'Amount' %}
         <i class="help-text question grey icon link" data-content="{% trans 'Total amount in $CAD.' %}"></i>
     </th>
     <th class="">{% trans 'Actions' %}</th>
   </thead>
   <tbody>
     {% for order in orders %}
-      <tr {% if order.status == 'O' and order.client.status != 'A' %}class="error"{% endif %}>
+      <tr {% if order.status == 'O' and order.client_planned_status_at_delivery != 'A' %}class="error"{% endif %}>
         <td><strong><i class="hashtag icon"></i>{{order.id}}</strong></td>
         <td>
             <a href="{% url 'member:client_information' pk=order.client.id %}">{{order.client.member}}</a>
-            {% if order.client.status != 'A' %}
-            ({{ order.client.status_verbose }})
+            {% if order.client_planned_status_at_delivery != 'A' %}
+            ({{ order.client_planned_status_at_delivery_verbose }})
             {% endif %}
         </td>
         <td>{{order.delivery_date}}</td>
         <td class="center aligned">{{order.get_status_display}}</td>
         <td><i class="dollar icon"></i>{{order.price}}</td>
         <td>
           <a class="ui basic icon button"  href="{% url 'order:view' pk=order.id %}"><i class="icon unhide"></i></a>
```

### Comparing `souschef-1.4.3/souschef/order/templates/order/create_batch.html` & `souschef-1.4.4/souschef/order/templates/order/create_batch.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/order/partials/filters.html` & `souschef-1.4.4/souschef/order/templates/order/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/order_confirm_delete.html` & `souschef-1.4.4/souschef/order/templates/order_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/order_update_status.html` & `souschef-1.4.4/souschef/order/templates/order_update_status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/update.html` & `souschef-1.4.4/souschef/order/templates/update.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/templates/view.html` & `souschef-1.4.4/souschef/order/templates/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/tests.py` & `souschef-1.4.4/souschef/order/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/urls.py` & `souschef-1.4.4/souschef/order/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/order/views.py` & `souschef-1.4.4/souschef/order/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/page/templates/pages/home.html` & `souschef-1.4.4/souschef/page/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/page/templates/registration/login.html` & `souschef-1.4.4/souschef/page/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/page/tests.py` & `souschef-1.4.4/souschef/page/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     "compote_saturday_quantity": 666,
                     "dessert_saturday_quantity": 666,
                     "diabetic_sunday_quantity": 666,
                     "fruit_salad_sunday_quantity": 666,
                 },
             )
 
-            if delivery_type == "O":
+            if delivery_type == Client.ONGOING_DELIVERY:
                 # Ongoing: only two delivery days!
                 Client_option.objects.create(
                     client=client_factory,
                     option=meals_schedule_option,
                     value=json.dumps(["tuesday", "wednesday"]),
                 )
```

### Comparing `souschef-1.4.3/souschef/page/views.py` & `souschef-1.4.4/souschef/page/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 meals_schedule = dict(client.meals_schedule)
 
                 # For each day, if there's a schedule, count schedule.
                 for day, _ in DAYS_OF_WEEK:
                     if day in meals_schedule:
                         schedules[day] += meals_schedule[day].get("main_dish") or 0
 
-                if client.delivery_type == "E":  # Episodic
+                if client.delivery_type == Client.EPISODIC_DELIVERY:
                     meals_default = dict(client.meals_default)
                     for day, _ in DAYS_OF_WEEK:
                         episodic_defaults[day] += (
                             meals_default[day].get(
                                 "main_dish",
                             )
                             or 0
```

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/css/main.min.css` & `souschef-1.4.4/souschef/sous_chef/assets/css/main.min.css`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.eot` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.svg` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.ttf` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.woff` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/brand-icons.woff2` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.eot` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.otf` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.otf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.svg` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.ttf` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.woff` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/icons.woff2` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.eot` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.svg` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.ttf` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.woff` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/fonts/outline-icons.woff2` & `souschef-1.4.4/souschef/sous_chef/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/bg1.jpg` & `souschef-1.4.4/souschef/sous_chef/assets/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/demo.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/demo.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/favicon.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/flags.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/glyph-marker-icon.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/glyph-marker-icon.svg` & `souschef-1.4.4/souschef/sous_chef/assets/images/glyph-marker-icon.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/jenny.jpg` & `souschef-1.4.4/souschef/sous_chef/assets/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/joe.jpg` & `souschef-1.4.4/souschef/sous_chef/assets/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/katrina.jpg` & `souschef-1.4.4/souschef/sous_chef/assets/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/leaflet.routing.icons.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/leaflet.routing.icons.svg` & `souschef-1.4.4/souschef/sous_chef/assets/images/leaflet.routing.icons.svg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/logo-souschef-coul.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-coul.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/logo-souschef-nb.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/logo-souschef-nb.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/logo.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-matte.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-matte@2x.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-matte@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-plain.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-plain.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-shadow.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-shadow@2x.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-shadow@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-soft.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/markers-soft@2x.png` & `souschef-1.4.4/souschef/sous_chef/assets/images/markers-soft@2x.png`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/images/throbber.gif` & `souschef-1.4.4/souschef/sous_chef/assets/images/throbber.gif`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/js/leaflet.js` & `souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/js/leaflet.min.js` & `souschef-1.4.4/souschef/sous_chef/assets/js/leaflet.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/js/multidatespicker.js` & `souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/js/multidatespicker.min.js` & `souschef-1.4.4/souschef/sous_chef/assets/js/multidatespicker.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/js/sous-chef.js` & `souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/assets/js/sous-chef.min.js` & `souschef-1.4.4/souschef/sous_chef/assets/js/sous-chef.min.js`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/context_processors.py` & `souschef-1.4.4/souschef/sous_chef/context_processors.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/management/commands/makemessages.py` & `souschef-1.4.4/souschef/sous_chef/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/settings.py` & `souschef-1.4.4/souschef/sous_chef/settings.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/404.html` & `souschef-1.4.4/souschef/sous_chef/templates/404.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/avatar/change.html` & `souschef-1.4.4/souschef/sous_chef/templates/avatar/change.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/avatar/confirm_delete.html` & `souschef-1.4.4/souschef/sous_chef/templates/avatar/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/base.html` & `souschef-1.4.4/souschef/sous_chef/templates/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/dashboard/statistics.html` & `souschef-1.4.4/souschef/sous_chef/templates/dashboard/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/splash.html` & `souschef-1.4.4/souschef/sous_chef/templates/splash.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/templates/system/menu.html` & `souschef-1.4.4/souschef/sous_chef/templates/system/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/tests.py` & `souschef-1.4.4/souschef/sous_chef/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef/sous_chef/urls.py` & `souschef-1.4.4/souschef/sous_chef/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.3/souschef.egg-info/PKG-INFO` & `souschef-1.4.4/souschef.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.4.3
+Version: 1.4.4
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/santropolroulant/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Keywords: meals-on-wheel
 Platform: UNKNOWN
```

### Comparing `souschef-1.4.3/souschef.egg-info/SOURCES.txt` & `souschef-1.4.4/souschef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

