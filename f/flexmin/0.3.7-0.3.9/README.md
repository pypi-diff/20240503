# Comparing `tmp/flexmin-0.3.7.tar.gz` & `tmp/flexmin-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexmin-0.3.7.tar", last modified: Thu Jan 12 14:40:14 2023, max compression
+gzip compressed data, was "flexmin-0.3.9.tar", last modified: Sun Jan 15 14:40:09 2023, max compression
```

## Comparing `flexmin-0.3.7.tar` & `flexmin-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-12 14:40:14.476300 flexmin-0.3.7/
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1487 2020-12-20 16:34:33.000000 flexmin-0.3.7/LICENSE
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     3835 2023-01-12 14:40:14.476300 flexmin-0.3.7/PKG-INFO
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     3082 2023-01-12 14:36:47.000000 flexmin-0.3.7/README.md
-drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-12 14:40:14.446300 flexmin-0.3.7/flexmin/
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)       73 2023-01-12 14:39:26.000000 flexmin-0.3.7/flexmin/__init__.py
-drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-12 14:40:14.469633 flexmin-0.3.7/flexmin/assets/
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1061 2020-12-20 16:34:34.000000 flexmin-0.3.7/flexmin/assets/assets.txt
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     2776 2023-01-12 14:40:03.000000 flexmin-0.3.7/flexmin/assets/config-examples.zip
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     7958 2023-01-12 14:39:58.000000 flexmin-0.3.7/flexmin/assets/config-templates.zip
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     9392 2023-01-12 14:39:52.000000 flexmin-0.3.7/flexmin/assets/configs.zip
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)  5795701 2023-01-12 14:39:47.000000 flexmin-0.3.7/flexmin/assets/py4web.zip
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)   126906 2023-01-12 14:39:35.000000 flexmin-0.3.7/flexmin/assets/scripts.zip
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     7669 2023-01-12 14:40:08.000000 flexmin-0.3.7/flexmin/assets/system.zip
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)    17164 2021-03-08 17:50:37.000000 flexmin-0.3.7/flexmin/flexmin_cli.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)    22904 2022-01-03 12:40:16.000000 flexmin-0.3.7/flexmin/flexmin_srv.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)    11712 2022-01-03 12:40:05.000000 flexmin-0.3.7/flexmin/flexmin_task.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)      340 2020-12-20 16:34:33.000000 flexmin-0.3.7/flexmin/run_checks.py
-drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-12 14:40:14.476300 flexmin-0.3.7/flexmin/utils/
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)        0 2020-06-06 12:37:07.000000 flexmin-0.3.7/flexmin/utils/__init__.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     5750 2020-12-20 16:34:34.000000 flexmin-0.3.7/flexmin/utils/output_prep.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     5457 2020-12-20 16:34:34.000000 flexmin-0.3.7/flexmin/utils/simplepam.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1766 2020-12-20 16:34:34.000000 flexmin-0.3.7/flexmin/utils/test.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     2320 2020-12-20 16:34:34.000000 flexmin-0.3.7/flexmin/utils/utilities.py
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)    30782 2020-09-19 07:16:24.000000 flexmin-0.3.7/flexmin/utils/yamlconfigs.py
-drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-12 14:40:14.449634 flexmin-0.3.7/flexmin.egg-info/
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     3835 2023-01-12 14:40:14.000000 flexmin-0.3.7/flexmin.egg-info/PKG-INFO
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)      719 2023-01-12 14:40:14.000000 flexmin-0.3.7/flexmin.egg-info/SOURCES.txt
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)        1 2023-01-12 14:40:14.000000 flexmin-0.3.7/flexmin.egg-info/dependency_links.txt
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)       52 2023-01-12 14:40:14.000000 flexmin-0.3.7/flexmin.egg-info/entry_points.txt
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)        1 2020-12-20 16:34:33.000000 flexmin-0.3.7/flexmin.egg-info/not-zip-safe
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)       32 2023-01-12 14:40:14.000000 flexmin-0.3.7/flexmin.egg-info/requires.txt
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)        8 2023-01-12 14:40:14.000000 flexmin-0.3.7/flexmin.egg-info/top_level.txt
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)       38 2023-01-12 14:40:14.476300 flexmin-0.3.7/setup.cfg
--rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1507 2023-01-12 14:37:20.000000 flexmin-0.3.7/setup.py
+drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-15 14:40:09.478888 flexmin-0.3.9/
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1487 2020-12-20 16:34:33.000000 flexmin-0.3.9/LICENSE
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     3867 2023-01-15 14:40:09.478888 flexmin-0.3.9/PKG-INFO
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     3082 2023-01-12 14:36:47.000000 flexmin-0.3.9/README.md
+drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-15 14:40:09.432222 flexmin-0.3.9/flexmin/
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)       73 2023-01-15 14:39:23.000000 flexmin-0.3.9/flexmin/__init__.py
+drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-15 14:40:09.472221 flexmin-0.3.9/flexmin/assets/
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1061 2020-12-20 16:34:34.000000 flexmin-0.3.9/flexmin/assets/assets.txt
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     2776 2023-01-15 14:39:58.000000 flexmin-0.3.9/flexmin/assets/config-examples.zip
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     7958 2023-01-15 14:39:52.000000 flexmin-0.3.9/flexmin/assets/config-templates.zip
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     9398 2023-01-15 14:39:47.000000 flexmin-0.3.9/flexmin/assets/configs.zip
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)  5795701 2023-01-15 14:39:42.000000 flexmin-0.3.9/flexmin/assets/py4web.zip
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)   127070 2023-01-15 14:39:30.000000 flexmin-0.3.9/flexmin/assets/scripts.zip
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     7669 2023-01-15 14:40:03.000000 flexmin-0.3.9/flexmin/assets/system.zip
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)    17164 2021-03-08 17:50:37.000000 flexmin-0.3.9/flexmin/flexmin_cli.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)    22904 2022-01-03 12:40:16.000000 flexmin-0.3.9/flexmin/flexmin_srv.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)    11712 2022-01-03 12:40:05.000000 flexmin-0.3.9/flexmin/flexmin_task.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)      340 2020-12-20 16:34:33.000000 flexmin-0.3.9/flexmin/run_checks.py
+drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-15 14:40:09.475554 flexmin-0.3.9/flexmin/utils/
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)        0 2020-06-06 12:37:07.000000 flexmin-0.3.9/flexmin/utils/__init__.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     5750 2020-12-20 16:34:34.000000 flexmin-0.3.9/flexmin/utils/output_prep.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     5457 2020-12-20 16:34:34.000000 flexmin-0.3.9/flexmin/utils/simplepam.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1766 2020-12-20 16:34:34.000000 flexmin-0.3.9/flexmin/utils/test.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     2320 2020-12-20 16:34:34.000000 flexmin-0.3.9/flexmin/utils/utilities.py
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)    30782 2020-09-19 07:16:24.000000 flexmin-0.3.9/flexmin/utils/yamlconfigs.py
+drwxr-xr-x   0 rcooke    (1000) rcooke    (1001)        0 2023-01-15 14:40:09.442221 flexmin-0.3.9/flexmin.egg-info/
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     3867 2023-01-15 14:40:09.000000 flexmin-0.3.9/flexmin.egg-info/PKG-INFO
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)      719 2023-01-15 14:40:09.000000 flexmin-0.3.9/flexmin.egg-info/SOURCES.txt
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)        1 2023-01-15 14:40:09.000000 flexmin-0.3.9/flexmin.egg-info/dependency_links.txt
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)       52 2023-01-15 14:40:09.000000 flexmin-0.3.9/flexmin.egg-info/entry_points.txt
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)        1 2020-12-20 16:34:33.000000 flexmin-0.3.9/flexmin.egg-info/not-zip-safe
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)       32 2023-01-15 14:40:09.000000 flexmin-0.3.9/flexmin.egg-info/requires.txt
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)        8 2023-01-15 14:40:09.000000 flexmin-0.3.9/flexmin.egg-info/top_level.txt
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)       38 2023-01-15 14:40:09.478888 flexmin-0.3.9/setup.cfg
+-rw-r--r--   0 rcooke    (1000) rcooke    (1001)     1539 2023-01-15 14:26:40.000000 flexmin-0.3.9/setup.py
```

### Comparing `flexmin-0.3.7/LICENSE` & `flexmin-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/PKG-INFO` & `flexmin-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: flexmin
-Version: 0.3.7
+Version: 0.3.9
 Summary: A flexible system admin web portal
-Home-page: 
+Home-page: https://www.futurscope.co.uk/flexmin
 Author: Richard Cooke
 Author-email: fm_1342@chrom3.co.uk
 Maintainer: Richard Cooke
 Maintainer-email: fm_1342@chrom3.co.uk
 License: BSD
 Platform: linux
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flexmin-0.3.7/README.md` & `flexmin-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/assets/assets.txt` & `flexmin-0.3.9/flexmin/assets/assets.txt`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/assets/config-examples.zip` & `flexmin-0.3.9/flexmin/assets/config-examples.zip`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/assets/configs.zip` & `flexmin-0.3.9/flexmin/assets/configs.zip`

 * *Files 24% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 9392 bytes, number of entries: 14
--rw-r--r--  3.0 unx      519 tx defN 23-Jan-12 14:39 py4web.nginx.yaml
--rw-r--r--  3.0 unx       35 tx stor 23-Jan-12 14:39 installed
--rw-r--r--  3.0 unx     1054 tx defN 23-Jan-12 14:39 flexmin.nginx.yaml
--rw-r--r--  3.0 unx     5990 tx defN 23-Jan-12 14:39 menu.yaml
--rw-r--r--  3.0 unx      746 tx defN 23-Jan-12 14:39 flexmin.conf
--rw-r--r--  3.0 unx      212 tx defN 23-Jan-12 14:39 dev_general_vlc.nginx.yaml
+Zip file size: 9398 bytes, number of entries: 14
+-rw-r--r--  3.0 unx      519 tx defN 23-Jan-15 14:39 py4web.nginx.yaml
+-rw-r--r--  3.0 unx       35 tx stor 23-Jan-15 14:39 installed
+-rw-r--r--  3.0 unx     1054 tx defN 23-Jan-15 14:39 flexmin.nginx.yaml
+-rw-r--r--  3.0 unx     5990 tx defN 23-Jan-15 14:39 menu.yaml
+-rw-r--r--  3.0 unx      746 tx defN 23-Jan-15 14:39 flexmin.conf
+-rw-r--r--  3.0 unx      212 tx defN 23-Jan-15 14:39 dev_general_vlc.nginx.yaml
 drwx------  3.0 unx        0 bx stor 21-Mar-05 18:43 private/
--rw-r--r--  3.0 unx     1115 tx defN 23-Jan-12 14:39 samecertbot_cli.ini
--rw-r--r--  3.0 unx      510 tx defN 23-Jan-12 14:39 dev.nginx.yaml
--rw-r--r--  3.0 unx     1114 tx defN 23-Jan-12 14:39 certbot_cli.ini
--rw-r--r--  3.0 unx      430 tx defN 23-Jan-12 14:39 dev_statisfy.nginx.yaml
--rw-r--r--  3.0 unx     4861 tx defN 23-Jan-12 14:39 menu.conf
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 dev_video_process.nginx.yaml
--rw-r--r--  3.0 unx      433 tx defN 23-Jan-12 14:39 dev_slideshow.nginx.yaml
-14 files, 17487 bytes uncompressed, 7116 bytes compressed:  59.3%
+-rw-r--r--  3.0 unx     1115 tx defN 23-Jan-15 14:39 samecertbot_cli.ini
+-rw-r--r--  3.0 unx      510 tx defN 23-Jan-15 14:39 dev.nginx.yaml
+-rw-r--r--  3.0 unx     1114 tx defN 23-Jan-15 14:39 certbot_cli.ini
+-rw-r--r--  3.0 unx      430 tx defN 23-Jan-15 14:39 dev_statisfy.nginx.yaml
+-rw-r--r--  3.0 unx     4861 tx defN 23-Jan-15 14:39 menu.conf
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 dev_video_process.nginx.yaml
+-rw-r--r--  3.0 unx      433 tx defN 23-Jan-15 14:39 dev_slideshow.nginx.yaml
+14 files, 17487 bytes uncompressed, 7122 bytes compressed:  59.3%
```

#### menu.yaml

```diff
@@ -41,15 +41,15 @@
         automatically propogate changes
     - item: nginx_certificates.sh;Manage Certificates;Manage the NGINX certificate files
     - item: nginx_logs.sh;View Logs;Lists log file config files for viewing.
   - group: uwsgi;uWSGI;uwsgi.png
     tasks:
     - item: uwsgi_overview.sh;Overview;Shows available and enabled uWSGI applications
     - item: uwsgi_editconfig.sh;Edit Configurations;Lists available uWSGI config files for editing
-    - item: uwsgi_logs.sh;View Logs;List available uWSGI logs for viewing
+    - item: uwsgi_logs.sh;Log Files;List available uWSGI logs for viewing
   - group: postgres;PostgreSQL;postgresql.png
     check_executable: {FM_PSQL}
     tasks:
     - item: postgres_users.sh;Users;Lists PostgreSQL Users and allows deletion
     - item: postgres_databases.sh;Databases;Lists PostgreSQL DBs and allows deletion
     - item: postgres_config.sh;Configuration;Edit PostgreSQL Config Files
     - item: postgres_backup.sh;Backup;Lists PostgreSQL DBs for Backup
```

#### menu.conf

```diff
@@ -22,15 +22,15 @@
 1;Overview;;nginx_viewconfig.sh;Lists available-site config files for selection and viewing.
 1;Edit Configurations;;nginx_editconfigs.sh;Edit the NGINX Configuration Files (yaml), automatically propogate changes
 1;Manage Certificates;;nginx_certificates.sh;Manage the NGINX certificate files
 1;View Logs;;nginx_logs.sh;Lists log file config files for viewing.
 0;uWSGI;uwsgi.png;;
 1;Overview;;uwsgi_overview.sh;Shows available and enabled uWSGI applications
 1;Edit Configurations;;uwsgi_editconfig.sh;Lists available uWSGI config files for editing
-1;View Logs;;uwsgi_logs.sh;List available uWSGI logs for viewing
+1;Log Files;;uwsgi_logs.sh;List available uWSGI logs for viewing
 0;PostgreSQL;postgresql.png;;
 1;Users;;postgres_users.sh;Lists PostgreSQL Users and allows deletion
 1;Databases;;postgres_databases.sh;Lists PostgreSQL DBs and allows deletion
 1;Configuration;;postgres_config.sh;Edit PostgreSQL Config Files
 1;Backup;;postgres_backup.sh;Lists PostgreSQL DBs for Backup
 1;Restore;;postgres_restore.sh;Lists PostgreSQL DBs for Backup
 0;SSH;ssh.png;;
```

### Comparing `flexmin-0.3.7/flexmin/assets/py4web.zip` & `flexmin-0.3.9/flexmin/assets/py4web.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,1026 +1,1026 @@
 Zip file size: 5795701 bytes, number of entries: 1024
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/databases/
--rw-r--r--  3.0 unx      866 tx defN 23-Jan-12 14:39 flexmin/tasks.py
--rw-r--r--  3.0 unx    18327 tx defN 23-Jan-12 14:39 flexmin/controllers.py
--rw-r--r--  3.0 unx      937 tx defN 23-Jan-12 14:39 flexmin/models.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/modules/
--rw-r--r--  3.0 unx      893 tx defN 23-Jan-12 14:39 flexmin/modules/utils.py
--rw-r--r--  3.0 unx     3567 tx defN 23-Jan-12 14:39 flexmin/modules/fmw_logs.py
--rw-r--r--  3.0 unx     5087 tx defN 23-Jan-12 14:39 flexmin/modules/graph.py
--rw-r--r--  3.0 unx     2171 tx defN 23-Jan-12 14:39 flexmin/modules/test_graph.txt
--rw-r--r--  3.0 unx     8203 tx defN 23-Jan-12 14:39 flexmin/modules/output_prep.py
--rw-r--r--  3.0 unx     5377 tx defN 23-Jan-12 14:39 flexmin/modules/run_prep.py
--rw-r--r--  3.0 unx        1 tx stor 23-Jan-12 14:39 flexmin/modules/__init__.py
--rw-r--r--  3.0 unx      853 tx defN 23-Jan-12 14:39 flexmin/modules/fmw_test_vars.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/translations/
--rw-r--r--  3.0 unx       97 tx defN 23-Jan-12 14:39 flexmin/translations/it.json
--rw-r--r--  3.0 unx     4190 tx defN 23-Jan-12 14:39 flexmin/common.py
--rw-r--r--  3.0 unx      426 tx defN 23-Jan-12 14:39 flexmin/README.md
--rw-r--r--  3.0 unx      205 tx defN 23-Jan-12 14:39 flexmin/settings_private.py
--rw-r--r--  3.0 unx     2007 tx defN 23-Jan-12 14:39 flexmin/settings.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/css/
--rw-r--r--  3.0 unx     9610 tx defN 23-Jan-12 14:39 flexmin/static/css/layout.css
--rw-r--r--  3.0 unx   210485 tx defN 23-Jan-12 14:39 flexmin/static/css/bulma.css
--rw-r--r--  3.0 unx     3715 tx defN 23-Jan-12 14:39 flexmin/static/css/hidden_scroll.css
--rw-r--r--  3.0 unx    11598 tx defN 23-Jan-12 14:39 flexmin/static/css/flexmin.css
--rw-r--r--  3.0 unx     1150 bx defN 23-Jan-12 14:39 flexmin/static/flexmin.ico
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/
--rw-r--r--  3.0 unx     1111 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/arch-32.png
--rw-r--r--  3.0 unx      144 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/network.png
--rw-r--r--  3.0 unx      775 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/debian-24.png
--rw-r--r--  3.0 unx      394 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/test-24.png
--rw-r--r--  3.0 unx      557 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/debian.png
--rw-r--r--  3.0 unx      897 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/arch-24.png
--rw-r--r--  3.0 unx      410 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/debian-32.png
--rw-r--r--  3.0 unx      465 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/dnsmasq.png
--rw-r--r--  3.0 unx      777 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/dlna-24.png
--rw-r--r--  3.0 unx      136 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/manjaro.png
--rw-r--r--  3.0 unx      266 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/node.js.png
--rw-r--r--  3.0 unx      559 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/dlna.png
--rw-r--r--  3.0 unx      821 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/raspberrypi.png
--rw-r--r--  3.0 unx      831 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/system.png
--rw-r--r--  3.0 unx      831 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/os.png
--rw-r--r--  3.0 unx      791 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/ssh.png
--rw-r--r--  3.0 unx      313 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/django.png
--rw-r--r--  3.0 unx      387 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/lighttpd.png
--rw-r--r--  3.0 unx      520 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/django-32.png
--rw-r--r--  3.0 unx      223 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/certificates.png
--rw-r--r--  3.0 unx      650 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/mercurial.png
--rw-r--r--  3.0 unx      495 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/samba.png
--rw-r--r--  3.0 unx      608 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/arch.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/rsync.ico
--rw-r--r--  3.0 unx      838 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/postgresql.png
--rw-r--r--  3.0 unx      568 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/django-24.png
--rw-r--r--  3.0 unx      199 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/uwsgi.png
--rw-r--r--  3.0 unx      416 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/rsync.png
--rw-r--r--  3.0 unx      696 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/flexmin.png
--rw-r--r--  3.0 unx      178 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/manjaro-32.png
--rw-r--r--  3.0 unx      419 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/test-32.png
--rw-r--r--  3.0 unx      153 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/nginx.png
--rw-r--r--  3.0 unx     1440 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/raspberrypi-24.png
--rw-r--r--  3.0 unx      887 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/samba-32.png
--rw-r--r--  3.0 unx      840 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/py4web.png
--rw-r--r--  3.0 unx     1553 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/py4web-24.png
--rw-r--r--  3.0 unx      629 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/lighttpd-32.png
--rw-r--r--  3.0 unx     1020 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/dlna-32.png
--rw-r--r--  3.0 unx      246 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/web2py.png
--rw-r--r--  3.0 unx      300 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/filesystem.png
--rw-r--r--  3.0 unx     2126 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/py4web-32.png
--rw-r--r--  3.0 unx      799 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/lighttpd-24.png
--rw-r--r--  3.0 unx      667 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/flexpac.png
--rw-r--r--  3.0 unx      773 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/samba-24.png
--rw-r--r--  3.0 unx     1707 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/raspberrypi-32.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/ssh.ico
--rw-r--r--  3.0 unx      247 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/test.png
--rw-r--r--  3.0 unx      394 bx stor 23-Jan-12 14:39 flexmin/static/fm_icons/systemd.png
--rw-r--r--  3.0 unx      148 bx defN 23-Jan-12 14:39 flexmin/static/fm_icons/manjaro-24.png
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/images/
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/images/flexmin.ico
--rw-r--r--  3.0 unx     6546 bx defN 23-Jan-12 14:39 flexmin/static/images/flexmin-shade-220w.png
--rw-r--r--  3.0 unx     2091 bx defN 23-Jan-12 14:39 flexmin/static/images/white_opacity_40.png
--rw-r--r--  3.0 unx    19869 tx defN 23-Jan-12 14:39 flexmin/static/images/web_flexmin.svg
--rw-r--r--  3.0 unx     2090 bx defN 23-Jan-12 14:39 flexmin/static/images/popup_bg.png
--rw-r--r--  3.0 unx     2091 bx defN 23-Jan-12 14:39 flexmin/static/images/white_opacity_30.png
--rw-r--r--  3.0 unx      696 bx stor 23-Jan-12 14:39 flexmin/static/images/flexmin_ico.png
--rw-r--r--  3.0 unx    12799 bx defN 23-Jan-12 14:39 flexmin/static/images/glyphicons-halflings.png
--rw-r--r--  3.0 unx    13179 bx stor 23-Jan-12 14:39 flexmin/static/images/flexmin_logo.png
--rw-r--r--  3.0 unx      842 bx defN 23-Jan-12 14:39 flexmin/static/images/flexmin-bg-4000-8000.png
--rw-r--r--  3.0 unx    10835 bx stor 23-Jan-12 14:39 flexmin/static/images/flexmin-3d-220w.png
--rw-r--r--  3.0 unx     8916 bx stor 23-Jan-12 14:39 flexmin/static/images/flexmin_med.png
--rw-r--r--  3.0 unx     8777 bx defN 23-Jan-12 14:39 flexmin/static/images/glyphicons-halflings-white.png
--rw-r--r--  3.0 unx        1 tx stor 23-Jan-12 14:39 flexmin/static/README.md
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/icons/
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-031-circle-amber.ico
--rw-r--r--  3.0 unx      135 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-005-cross-red.png
--rw-r--r--  3.0 unx      154 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-004-cross-bld.png
--rw-r--r--  3.0 unx      170 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-037-key.png
--rw-r--r--  3.0 unx      144 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-016-tick-green-sml-bld.png
--rw-r--r--  3.0 unx      614 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-24-002-folder.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-029-circle-green-lrg.ico
--rw-r--r--  3.0 unx      167 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-030-circle-red.png
--rw-r--r--  3.0 unx      170 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-040-unlink.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-017-twisty-closed.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-015-tick-green-sml.ico
--rw-r--r--  3.0 unx      135 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-013-cross-red-sml.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-035-circle-green-sml.ico
--rw-r--r--  3.0 unx      172 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-006-cross-red-bld.png
--rw-r--r--  3.0 unx      145 tx defN 23-Jan-12 14:39 flexmin/static/icons/im-sprite.cmd
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-034-circle-amber-sml.ico
--rw-r--r--  3.0 unx       54 tx defN 23-Jan-12 14:39 flexmin/static/icons/links.txt
--rw-r--r--  3.0 unx      156 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-020-twisty-open-bld.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-032-circle-green.ico
--rw-r--r--  3.0 unx      172 tx defN 23-Jan-12 14:39 flexmin/static/icons/.hg_archival.txt
--rw-r--r--  3.0 unx      148 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-010-tick-bld.png
--rw-r--r--  3.0 unx      203 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-023-person.png
--rw-r--r--  3.0 unx      118 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-009-tick.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-009-tick.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-004-cross-bld.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-016-tick-green-sml-bld.ico
--rw-r--r--  3.0 unx     4226 bx defN 23-Jan-12 14:39 flexmin/static/icons/icons-16.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-018-twisty-closed-bld.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-033-circle-red-sml.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-024-group.ico
--rw-r--r--  3.0 unx      168 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-035-circle-green-sml.png
--rw-r--r--  3.0 unx     2611 tx defN 23-Jan-12 14:39 flexmin/static/icons/icons.styl
--rw-r--r--  3.0 unx     2963 bx defN 23-Jan-12 14:39 flexmin/static/icons/icons-16-0.png
--rw-r--r--  3.0 unx      185 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-002-doc.png
--rw-r--r--  3.0 unx      160 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-012-tick-green-bld.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-022-bullet-bld.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-023-person.ico
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-019-twisty-open.ico
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-037-key.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-036-write.ico
--rw-r--r--  3.0 unx      216 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-027-circle-red-lrg.png
--rw-r--r--  3.0 unx      117 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-017-twisty-closed.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-001-folder.ico
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-038-power.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-030-circle-red.ico
--rw-r--r--  3.0 unx      168 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-025-copy.png
--rw-r--r--  3.0 unx     1454 bx defN 23-Jan-12 14:39 flexmin/static/icons/icons-16-1.png
--rw-r--r--  3.0 unx      174 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-026-paste.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-039-info-blue.ico
--rw-r--r--  3.0 unx      136 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-021-bullet.png
--rw-r--r--  3.0 unx      119 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-015-tick-green-sml.png
--rw-r--r--  3.0 unx      246 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-024-group.png
--rw-r--r--  3.0 unx     4764 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-24-001-folder.ico
--rw-r--r--  3.0 unx      184 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-022-bullet-bld.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-005-cross-red.ico
--rw-r--r--  3.0 unx      193 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-029-circle-green-lrg.png
--rw-r--r--  3.0 unx      203 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-001-folder.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-014-cross-red-sml-bld.ico
--rw-r--r--  3.0 unx      170 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-033-circle-red-sml.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-013-cross-red-sml.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-007-upload.ico
--rw-r--r--  3.0 unx      173 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-007-upload.png
--rw-r--r--  3.0 unx       91 tx defN 23-Jan-12 14:39 flexmin/static/icons/im-sprite.sh
--rw-r--r--  3.0 unx      177 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-034-circle-amber-sml.png
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-026-paste.ico
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-027-circle-red-lrg.ico
--rw-r--r--  3.0 unx      135 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-011-tick-green.png
--rw-r--r--  3.0 unx      127 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-003-cross.png
--rw-r--r--  3.0 unx      183 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-014-cross-red-sml-bld.png
--rw-r--r--  3.0 unx      163 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-032-circle-green.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-010-tick-bld.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-020-twisty-open-bld.ico
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-002-doc.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-012-tick-green-bld.ico
--rw-r--r--  3.0 unx     1086 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-006-cross-red-bld.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-008-download.ico
--rw-r--r--  3.0 unx      160 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-008-download.png
--rw-r--r--  3.0 unx      166 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-031-circle-amber.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-021-bullet.ico
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-025-copy.ico
--rw-r--r--  3.0 unx      204 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-028-circle-amber-lrg.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-003-cross.ico
--rw-r--r--  3.0 unx      397 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-039-info-blue.png
--rw-r--r--  3.0 unx      226 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-036-write.png
--rw-r--r--  3.0 unx     6259 tx defN 23-Jan-12 14:39 flexmin/static/icons/icons.css
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-028-circle-amber-lrg.ico
--rw-r--r--  3.0 unx      138 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-019-twisty-open.png
--rw-r--r--  3.0 unx      202 bx stor 23-Jan-12 14:39 flexmin/static/icons/icon-16-038-power.png
--rw-r--r--  3.0 unx      141 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-018-twisty-closed-bld.png
--rw-r--r--  3.0 unx    32988 bx defN 23-Jan-12 14:39 flexmin/static/icons/icon-16-011-tick-green.ico
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/js/
--rw-r--r--  3.0 unx    68547 tx defN 23-Jan-12 14:39 flexmin/static/js/sugar.min.js
--rw-r--r--  3.0 unx     4940 tx defN 23-Jan-12 14:39 flexmin/static/js/utils.js
--rw-r--r--  3.0 unx    44228 tx defN 23-Jan-12 14:39 flexmin/static/js/fragmenty.coffee
--rw-r--r--  3.0 unx    16458 tx defN 23-Jan-12 14:39 flexmin/static/js/treenav.coffee
--rw-r--r--  3.0 unx    76004 tx defN 23-Jan-12 14:39 flexmin/static/js/vue.min.js
--rw-r--r--  3.0 unx    88145 tx defN 23-Jan-12 14:39 flexmin/static/js/jquery-3.4.1.min.js
--rw-r--r--  3.0 unx    29108 tx defN 23-Jan-12 14:39 flexmin/static/js/treenav.js.map
--rw-r--r--  3.0 unx   173825 tx defN 23-Jan-12 14:39 flexmin/static/js/moment.js
--rw-r--r--  3.0 unx    17033 tx defN 23-Jan-12 14:39 flexmin/static/js/treenav.js
--rw-r--r--  3.0 unx    78379 tx defN 23-Jan-12 14:39 flexmin/static/js/fragmenty.js.map
--rw-r--r--  3.0 unx    12132 tx defN 23-Jan-12 14:39 flexmin/static/js/axios.min.js
--rw-r--r--  3.0 unx    47851 tx defN 23-Jan-12 14:39 flexmin/static/js/fragmenty.js
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/databases/
+-rw-r--r--  3.0 unx      866 tx defN 23-Jan-15 14:39 flexmin/tasks.py
+-rw-r--r--  3.0 unx    18327 tx defN 23-Jan-15 14:39 flexmin/controllers.py
+-rw-r--r--  3.0 unx      937 tx defN 23-Jan-15 14:39 flexmin/models.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/modules/
+-rw-r--r--  3.0 unx      893 tx defN 23-Jan-15 14:39 flexmin/modules/utils.py
+-rw-r--r--  3.0 unx     3567 tx defN 23-Jan-15 14:39 flexmin/modules/fmw_logs.py
+-rw-r--r--  3.0 unx     5087 tx defN 23-Jan-15 14:39 flexmin/modules/graph.py
+-rw-r--r--  3.0 unx     2171 tx defN 23-Jan-15 14:39 flexmin/modules/test_graph.txt
+-rw-r--r--  3.0 unx     8203 tx defN 23-Jan-15 14:39 flexmin/modules/output_prep.py
+-rw-r--r--  3.0 unx     5377 tx defN 23-Jan-15 14:39 flexmin/modules/run_prep.py
+-rw-r--r--  3.0 unx        1 tx stor 23-Jan-15 14:39 flexmin/modules/__init__.py
+-rw-r--r--  3.0 unx      853 tx defN 23-Jan-15 14:39 flexmin/modules/fmw_test_vars.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/translations/
+-rw-r--r--  3.0 unx       97 tx defN 23-Jan-15 14:39 flexmin/translations/it.json
+-rw-r--r--  3.0 unx     4190 tx defN 23-Jan-15 14:39 flexmin/common.py
+-rw-r--r--  3.0 unx      426 tx defN 23-Jan-15 14:39 flexmin/README.md
+-rw-r--r--  3.0 unx      205 tx defN 23-Jan-15 14:39 flexmin/settings_private.py
+-rw-r--r--  3.0 unx     2007 tx defN 23-Jan-15 14:39 flexmin/settings.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/css/
+-rw-r--r--  3.0 unx     9610 tx defN 23-Jan-15 14:39 flexmin/static/css/layout.css
+-rw-r--r--  3.0 unx   210485 tx defN 23-Jan-15 14:39 flexmin/static/css/bulma.css
+-rw-r--r--  3.0 unx     3715 tx defN 23-Jan-15 14:39 flexmin/static/css/hidden_scroll.css
+-rw-r--r--  3.0 unx    11598 tx defN 23-Jan-15 14:39 flexmin/static/css/flexmin.css
+-rw-r--r--  3.0 unx     1150 bx defN 23-Jan-15 14:39 flexmin/static/flexmin.ico
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/
+-rw-r--r--  3.0 unx     1111 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/arch-32.png
+-rw-r--r--  3.0 unx      144 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/network.png
+-rw-r--r--  3.0 unx      775 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/debian-24.png
+-rw-r--r--  3.0 unx      394 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/test-24.png
+-rw-r--r--  3.0 unx      557 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/debian.png
+-rw-r--r--  3.0 unx      897 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/arch-24.png
+-rw-r--r--  3.0 unx      410 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/debian-32.png
+-rw-r--r--  3.0 unx      465 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/dnsmasq.png
+-rw-r--r--  3.0 unx      777 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/dlna-24.png
+-rw-r--r--  3.0 unx      136 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/manjaro.png
+-rw-r--r--  3.0 unx      266 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/node.js.png
+-rw-r--r--  3.0 unx      559 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/dlna.png
+-rw-r--r--  3.0 unx      821 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/raspberrypi.png
+-rw-r--r--  3.0 unx      831 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/system.png
+-rw-r--r--  3.0 unx      831 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/os.png
+-rw-r--r--  3.0 unx      791 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/ssh.png
+-rw-r--r--  3.0 unx      313 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/django.png
+-rw-r--r--  3.0 unx      387 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/lighttpd.png
+-rw-r--r--  3.0 unx      520 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/django-32.png
+-rw-r--r--  3.0 unx      223 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/certificates.png
+-rw-r--r--  3.0 unx      650 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/mercurial.png
+-rw-r--r--  3.0 unx      495 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/samba.png
+-rw-r--r--  3.0 unx      608 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/arch.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/rsync.ico
+-rw-r--r--  3.0 unx      838 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/postgresql.png
+-rw-r--r--  3.0 unx      568 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/django-24.png
+-rw-r--r--  3.0 unx      199 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/uwsgi.png
+-rw-r--r--  3.0 unx      416 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/rsync.png
+-rw-r--r--  3.0 unx      696 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/flexmin.png
+-rw-r--r--  3.0 unx      178 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/manjaro-32.png
+-rw-r--r--  3.0 unx      419 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/test-32.png
+-rw-r--r--  3.0 unx      153 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/nginx.png
+-rw-r--r--  3.0 unx     1440 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/raspberrypi-24.png
+-rw-r--r--  3.0 unx      887 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/samba-32.png
+-rw-r--r--  3.0 unx      840 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/py4web.png
+-rw-r--r--  3.0 unx     1553 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/py4web-24.png
+-rw-r--r--  3.0 unx      629 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/lighttpd-32.png
+-rw-r--r--  3.0 unx     1020 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/dlna-32.png
+-rw-r--r--  3.0 unx      246 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/web2py.png
+-rw-r--r--  3.0 unx      300 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/filesystem.png
+-rw-r--r--  3.0 unx     2126 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/py4web-32.png
+-rw-r--r--  3.0 unx      799 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/lighttpd-24.png
+-rw-r--r--  3.0 unx      667 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/flexpac.png
+-rw-r--r--  3.0 unx      773 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/samba-24.png
+-rw-r--r--  3.0 unx     1707 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/raspberrypi-32.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/ssh.ico
+-rw-r--r--  3.0 unx      247 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/test.png
+-rw-r--r--  3.0 unx      394 bx stor 23-Jan-15 14:39 flexmin/static/fm_icons/systemd.png
+-rw-r--r--  3.0 unx      148 bx defN 23-Jan-15 14:39 flexmin/static/fm_icons/manjaro-24.png
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/images/
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/images/flexmin.ico
+-rw-r--r--  3.0 unx     6546 bx defN 23-Jan-15 14:39 flexmin/static/images/flexmin-shade-220w.png
+-rw-r--r--  3.0 unx     2091 bx defN 23-Jan-15 14:39 flexmin/static/images/white_opacity_40.png
+-rw-r--r--  3.0 unx    19869 tx defN 23-Jan-15 14:39 flexmin/static/images/web_flexmin.svg
+-rw-r--r--  3.0 unx     2090 bx defN 23-Jan-15 14:39 flexmin/static/images/popup_bg.png
+-rw-r--r--  3.0 unx     2091 bx defN 23-Jan-15 14:39 flexmin/static/images/white_opacity_30.png
+-rw-r--r--  3.0 unx      696 bx stor 23-Jan-15 14:39 flexmin/static/images/flexmin_ico.png
+-rw-r--r--  3.0 unx    12799 bx defN 23-Jan-15 14:39 flexmin/static/images/glyphicons-halflings.png
+-rw-r--r--  3.0 unx    13179 bx stor 23-Jan-15 14:39 flexmin/static/images/flexmin_logo.png
+-rw-r--r--  3.0 unx      842 bx defN 23-Jan-15 14:39 flexmin/static/images/flexmin-bg-4000-8000.png
+-rw-r--r--  3.0 unx    10835 bx stor 23-Jan-15 14:39 flexmin/static/images/flexmin-3d-220w.png
+-rw-r--r--  3.0 unx     8916 bx stor 23-Jan-15 14:39 flexmin/static/images/flexmin_med.png
+-rw-r--r--  3.0 unx     8777 bx defN 23-Jan-15 14:39 flexmin/static/images/glyphicons-halflings-white.png
+-rw-r--r--  3.0 unx        1 tx stor 23-Jan-15 14:39 flexmin/static/README.md
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/icons/
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-031-circle-amber.ico
+-rw-r--r--  3.0 unx      135 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-005-cross-red.png
+-rw-r--r--  3.0 unx      154 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-004-cross-bld.png
+-rw-r--r--  3.0 unx      170 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-037-key.png
+-rw-r--r--  3.0 unx      144 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-016-tick-green-sml-bld.png
+-rw-r--r--  3.0 unx      614 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-24-002-folder.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-029-circle-green-lrg.ico
+-rw-r--r--  3.0 unx      167 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-030-circle-red.png
+-rw-r--r--  3.0 unx      170 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-040-unlink.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-017-twisty-closed.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-015-tick-green-sml.ico
+-rw-r--r--  3.0 unx      135 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-013-cross-red-sml.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-035-circle-green-sml.ico
+-rw-r--r--  3.0 unx      172 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-006-cross-red-bld.png
+-rw-r--r--  3.0 unx      145 tx defN 23-Jan-15 14:39 flexmin/static/icons/im-sprite.cmd
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-034-circle-amber-sml.ico
+-rw-r--r--  3.0 unx       54 tx defN 23-Jan-15 14:39 flexmin/static/icons/links.txt
+-rw-r--r--  3.0 unx      156 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-020-twisty-open-bld.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-032-circle-green.ico
+-rw-r--r--  3.0 unx      172 tx defN 23-Jan-15 14:39 flexmin/static/icons/.hg_archival.txt
+-rw-r--r--  3.0 unx      148 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-010-tick-bld.png
+-rw-r--r--  3.0 unx      203 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-023-person.png
+-rw-r--r--  3.0 unx      118 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-009-tick.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-009-tick.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-004-cross-bld.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-016-tick-green-sml-bld.ico
+-rw-r--r--  3.0 unx     4226 bx defN 23-Jan-15 14:39 flexmin/static/icons/icons-16.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-018-twisty-closed-bld.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-033-circle-red-sml.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-024-group.ico
+-rw-r--r--  3.0 unx      168 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-035-circle-green-sml.png
+-rw-r--r--  3.0 unx     2611 tx defN 23-Jan-15 14:39 flexmin/static/icons/icons.styl
+-rw-r--r--  3.0 unx     2963 bx defN 23-Jan-15 14:39 flexmin/static/icons/icons-16-0.png
+-rw-r--r--  3.0 unx      185 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-002-doc.png
+-rw-r--r--  3.0 unx      160 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-012-tick-green-bld.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-022-bullet-bld.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-023-person.ico
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-019-twisty-open.ico
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-037-key.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-036-write.ico
+-rw-r--r--  3.0 unx      216 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-027-circle-red-lrg.png
+-rw-r--r--  3.0 unx      117 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-017-twisty-closed.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-001-folder.ico
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-038-power.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-030-circle-red.ico
+-rw-r--r--  3.0 unx      168 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-025-copy.png
+-rw-r--r--  3.0 unx     1454 bx defN 23-Jan-15 14:39 flexmin/static/icons/icons-16-1.png
+-rw-r--r--  3.0 unx      174 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-026-paste.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-039-info-blue.ico
+-rw-r--r--  3.0 unx      136 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-021-bullet.png
+-rw-r--r--  3.0 unx      119 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-015-tick-green-sml.png
+-rw-r--r--  3.0 unx      246 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-024-group.png
+-rw-r--r--  3.0 unx     4764 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-24-001-folder.ico
+-rw-r--r--  3.0 unx      184 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-022-bullet-bld.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-005-cross-red.ico
+-rw-r--r--  3.0 unx      193 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-029-circle-green-lrg.png
+-rw-r--r--  3.0 unx      203 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-001-folder.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-014-cross-red-sml-bld.ico
+-rw-r--r--  3.0 unx      170 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-033-circle-red-sml.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-013-cross-red-sml.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-007-upload.ico
+-rw-r--r--  3.0 unx      173 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-007-upload.png
+-rw-r--r--  3.0 unx       91 tx defN 23-Jan-15 14:39 flexmin/static/icons/im-sprite.sh
+-rw-r--r--  3.0 unx      177 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-034-circle-amber-sml.png
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-026-paste.ico
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-027-circle-red-lrg.ico
+-rw-r--r--  3.0 unx      135 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-011-tick-green.png
+-rw-r--r--  3.0 unx      127 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-003-cross.png
+-rw-r--r--  3.0 unx      183 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-014-cross-red-sml-bld.png
+-rw-r--r--  3.0 unx      163 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-032-circle-green.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-010-tick-bld.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-020-twisty-open-bld.ico
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-002-doc.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-012-tick-green-bld.ico
+-rw-r--r--  3.0 unx     1086 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-006-cross-red-bld.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-008-download.ico
+-rw-r--r--  3.0 unx      160 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-008-download.png
+-rw-r--r--  3.0 unx      166 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-031-circle-amber.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-021-bullet.ico
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-025-copy.ico
+-rw-r--r--  3.0 unx      204 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-028-circle-amber-lrg.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-003-cross.ico
+-rw-r--r--  3.0 unx      397 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-039-info-blue.png
+-rw-r--r--  3.0 unx      226 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-036-write.png
+-rw-r--r--  3.0 unx     6259 tx defN 23-Jan-15 14:39 flexmin/static/icons/icons.css
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-028-circle-amber-lrg.ico
+-rw-r--r--  3.0 unx      138 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-019-twisty-open.png
+-rw-r--r--  3.0 unx      202 bx stor 23-Jan-15 14:39 flexmin/static/icons/icon-16-038-power.png
+-rw-r--r--  3.0 unx      141 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-018-twisty-closed-bld.png
+-rw-r--r--  3.0 unx    32988 bx defN 23-Jan-15 14:39 flexmin/static/icons/icon-16-011-tick-green.ico
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/js/
+-rw-r--r--  3.0 unx    68547 tx defN 23-Jan-15 14:39 flexmin/static/js/sugar.min.js
+-rw-r--r--  3.0 unx     4940 tx defN 23-Jan-15 14:39 flexmin/static/js/utils.js
+-rw-r--r--  3.0 unx    44228 tx defN 23-Jan-15 14:39 flexmin/static/js/fragmenty.coffee
+-rw-r--r--  3.0 unx    16458 tx defN 23-Jan-15 14:39 flexmin/static/js/treenav.coffee
+-rw-r--r--  3.0 unx    76004 tx defN 23-Jan-15 14:39 flexmin/static/js/vue.min.js
+-rw-r--r--  3.0 unx    88145 tx defN 23-Jan-15 14:39 flexmin/static/js/jquery-3.4.1.min.js
+-rw-r--r--  3.0 unx    29108 tx defN 23-Jan-15 14:39 flexmin/static/js/treenav.js.map
+-rw-r--r--  3.0 unx   173825 tx defN 23-Jan-15 14:39 flexmin/static/js/moment.js
+-rw-r--r--  3.0 unx    17033 tx defN 23-Jan-15 14:39 flexmin/static/js/treenav.js
+-rw-r--r--  3.0 unx    78379 tx defN 23-Jan-15 14:39 flexmin/static/js/fragmenty.js.map
+-rw-r--r--  3.0 unx    12132 tx defN 23-Jan-15 14:39 flexmin/static/js/axios.min.js
+-rw-r--r--  3.0 unx    47851 tx defN 23-Jan-15 14:39 flexmin/static/js/fragmenty.js
 drwxr-xr-x  3.0 unx        0 bx stor 20-Jul-18 10:23 flexmin/static/ace/
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/ace/src-min/
--rw-r--r--  3.0 unx     2680 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-cobalt.js
--rw-r--r--  3.0 unx     2688 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-gherkin.js
--rw-r--r--  3.0 unx    32956 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-ftl.js
--rw-r--r--  3.0 unx    11851 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-haskell.js
--rw-r--r--  3.0 unx    16788 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-sqlserver.js
--rw-r--r--  3.0 unx     2941 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-textmate.js
--rw-r--r--  3.0 unx     3127 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-mono_industrial.js
--rw-r--r--  3.0 unx    65868 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-rhtml.js
--rw-r--r--  3.0 unx    67925 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-razor.js
--rw-r--r--  3.0 unx     8479 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-asciidoc.js
--rw-r--r--  3.0 unx    65423 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-liquid.js
--rw-r--r--  3.0 unx     8701 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-apex.js
--rw-r--r--  3.0 unx     5397 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-vbscript.js
--rw-r--r--  3.0 unx     2968 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-pastel_on_dark.js
--rw-r--r--  3.0 unx     1588 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-spellcheck.js
--rw-r--r--  3.0 unx    61830 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-curly.js
--rw-r--r--  3.0 unx    59455 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-pgsql.js
--rw-r--r--  3.0 unx     3165 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-mixal.js
--rw-r--r--  3.0 unx  1633164 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-xquery.js
--rw-r--r--  3.0 unx     6840 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-mysql.js
--rw-r--r--  3.0 unx   217050 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-html.js
--rw-r--r--  3.0 unx     1425 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-properties.js
--rw-r--r--  3.0 unx     6516 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-tcl.js
--rw-r--r--  3.0 unx     9170 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-csharp.js
--rw-r--r--  3.0 unx     5399 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-livescript.js
--rw-r--r--  3.0 unx     8128 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-python.js
--rw-r--r--  3.0 unx     3222 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-sqlserver.js
--rw-r--r--  3.0 unx     9332 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-textarea.js
--rw-r--r--  3.0 unx     2647 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-solarized_dark.js
--rw-r--r--  3.0 unx     2696 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-solarized_light.js
--rw-r--r--  3.0 unx     2553 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-space.js
--rw-r--r--  3.0 unx   331682 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-coffee.js
--rw-r--r--  3.0 unx     3245 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-whitespace.js
--rw-r--r--  3.0 unx     1224 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-gitignore.js
--rw-r--r--  3.0 unx     9266 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-d.js
--rw-r--r--  3.0 unx    15910 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-ocaml.js
--rw-r--r--  3.0 unx     8317 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-redshift.js
--rw-r--r--  3.0 unx    63985 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-autohotkey.js
--rw-r--r--  3.0 unx    63476 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-visualforce.js
--rw-r--r--  3.0 unx    16939 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-vala.js
--rw-r--r--  3.0 unx    10652 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-nsis.js
--rw-r--r--  3.0 unx     3458 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-katzenmilch.js
--rw-r--r--  3.0 unx     4254 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-qml.js
--rw-r--r--  3.0 unx     5187 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-batchfile.js
--rw-r--r--  3.0 unx     2625 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-kr_theme.js
--rw-r--r--  3.0 unx     6851 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-haxe.js
--rw-r--r--  3.0 unx     2204 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-sql.js
--rw-r--r--  3.0 unx    55117 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-xml.js
--rw-r--r--  3.0 unx   473743 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-php.js
--rw-r--r--  3.0 unx     4016 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-static_highlight.js
--rw-r--r--  3.0 unx    20347 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-typescript.js
--rw-r--r--  3.0 unx    23819 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-java.js
--rw-r--r--  3.0 unx    39316 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-language_tools.js
--rw-r--r--  3.0 unx     1568 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-csp.js
--rw-r--r--  3.0 unx     5076 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-yaml.js
--rw-r--r--  3.0 unx    24007 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-scss.js
--rw-r--r--  3.0 unx     3148 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-edifact.js
--rw-r--r--  3.0 unx     2912 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-dracula.js
--rw-r--r--  3.0 unx    10453 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-ruby.js
--rw-r--r--  3.0 unx     7316 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-forth.js
--rw-r--r--  3.0 unx     9069 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-asl.js
--rw-r--r--  3.0 unx     5037 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-fsl.js
--rw-r--r--  3.0 unx    30080 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-erlang.js
--rw-r--r--  3.0 unx    20829 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-css.js
--rw-r--r--  3.0 unx    60818 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-html.js
--rw-r--r--  3.0 unx    46803 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-lua.js
--rw-r--r--  3.0 unx    16071 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-elixir.js
--rw-r--r--  3.0 unx     2536 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-vibrant_ink.js
--rw-r--r--  3.0 unx   233671 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-jsoniq.js
--rw-r--r--  3.0 unx     7959 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-csound_score.js
--rw-r--r--  3.0 unx     4258 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-beautify.js
--rw-r--r--  3.0 unx    71439 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-ejs.js
--rw-r--r--  3.0 unx     6026 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-logiql.js
--rw-r--r--  3.0 unx     8757 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-fortran.js
--rw-r--r--  3.0 unx    21771 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-sjs.js
--rw-r--r--  3.0 unx    78008 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-html_elixir.js
--rw-r--r--  3.0 unx    20840 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-wollok.js
--rw-r--r--  3.0 unx    20926 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-actionscript.js
--rw-r--r--  3.0 unx    47702 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-jade.js
--rw-r--r--  3.0 unx     3025 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-ini.js
--rw-r--r--  3.0 unx     7032 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-mushcode.js
--rw-r--r--  3.0 unx    63341 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-coldfusion.js
--rw-r--r--  3.0 unx     5258 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-elm.js
--rw-r--r--  3.0 unx   478207 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-php_laravel_blade.js
--rw-r--r--  3.0 unx     5732 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-applescript.js
--rw-r--r--  3.0 unx     5390 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-alda.js
--rw-r--r--  3.0 unx     6937 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-nim.js
--rw-r--r--  3.0 unx     1695 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-themelist.js
--rw-r--r--  3.0 unx    12924 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-red.js
--rw-r--r--  3.0 unx    11412 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-c_cpp.js
--rw-r--r--  3.0 unx    10323 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-crystal.js
--rw-r--r--  3.0 unx     4031 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-elastic_tabstops_lite.js
--rw-r--r--  3.0 unx     7461 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-puppet.js
--rw-r--r--  3.0 unx    14877 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-options.js
--rw-r--r--  3.0 unx    17977 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-perl6.js
--rw-r--r--  3.0 unx    14242 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-apache_conf.js
--rw-r--r--  3.0 unx     3147 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-crimson_editor.js
--rw-r--r--  3.0 unx   140785 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-css.js
--rw-r--r--  3.0 unx    11545 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-drools.js
--rw-r--r--  3.0 unx    42578 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-mask.js
--rw-r--r--  3.0 unx    16214 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-nginx.js
--rw-r--r--  3.0 unx     2408 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-clouds.js
--rw-r--r--  3.0 unx     5352 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-turtle.js
--rw-r--r--  3.0 unx    23112 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-scala.js
--rw-r--r--  3.0 unx    32595 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-json.js
--rw-r--r--  3.0 unx     6950 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-rust.js
--rw-r--r--  3.0 unx     3179 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-chaos.js
--rw-r--r--  3.0 unx     3952 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-keybinding_menu.js
--rw-r--r--  3.0 unx    72376 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-csound_document.js
--rw-r--r--  3.0 unx     1995 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-gruvbox.js
--rw-r--r--  3.0 unx     6917 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-makefile.js
--rw-r--r--  3.0 unx     2566 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-merbivore.js
--rw-r--r--  3.0 unx     8695 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-prolog.js
--rw-r--r--  3.0 unx     4398 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-c9search.js
--rw-r--r--  3.0 unx     2783 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-merbivore_soft.js
--rw-r--r--  3.0 unx     6831 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-scad.js
--rw-r--r--  3.0 unx     8183 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-sparql.js
--rw-r--r--  3.0 unx    20648 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-tsx.js
--rw-r--r--  3.0 unx     2448 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-textile.js
--rw-r--r--  3.0 unx     4054 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-snippets.js
--rw-r--r--  3.0 unx     2581 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-idle_fingers.js
--rw-r--r--  3.0 unx    50014 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-prompt.js
--rw-r--r--  3.0 unx     8389 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-clojure.js
--rw-r--r--  3.0 unx     3114 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-tex.js
--rw-r--r--  3.0 unx     6536 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-bro.js
--rw-r--r--  3.0 unx      836 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-plain_text.js
--rw-r--r--  3.0 unx     7778 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-coffee.js
--rw-r--r--  3.0 unx     3435 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-aql.js
--rw-r--r--  3.0 unx     2773 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-lucene.js
--rw-r--r--  3.0 unx    62174 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-django.js
--rw-r--r--  3.0 unx     4712 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-modelist.js
--rw-r--r--  3.0 unx     3565 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-tomorrow_night_eighties.js
--rw-r--r--  3.0 unx    20889 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-matlab.js
--rw-r--r--  3.0 unx    26979 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-lsl.js
--rw-r--r--  3.0 unx     3838 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-tomorrow_night_bright.js
--rw-r--r--  3.0 unx     5072 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-abc.js
--rw-r--r--  3.0 unx    22934 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-groovy.js
--rw-r--r--  3.0 unx     2828 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-twilight.js
--rw-r--r--  3.0 unx     3866 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-split.js
--rw-r--r--  3.0 unx    72574 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-markdown.js
--rw-r--r--  3.0 unx     4505 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-pascal.js
--rw-r--r--  3.0 unx    22820 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-less.js
--rw-r--r--  3.0 unx     3155 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-tomorrow_night.js
--rw-r--r--  3.0 unx    12257 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-kotlin.js
--rw-r--r--  3.0 unx     2703 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-monokai.js
--rw-r--r--  3.0 unx     7866 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-julia.js
--rw-r--r--  3.0 unx     7233 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-golang.js
--rw-r--r--  3.0 unx     9224 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-assembly_x86.js
--rw-r--r--  3.0 unx     8591 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-dockerfile.js
--rw-r--r--  3.0 unx     2453 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-eclipse.js
--rw-r--r--  3.0 unx     3039 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-chrome.js
--rw-r--r--  3.0 unx    55045 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-objectivec.js
--rw-r--r--  3.0 unx    69313 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-soy_template.js
--rw-r--r--  3.0 unx     6637 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-pig.js
--rw-r--r--  3.0 unx     5004 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-rdoc.js
--rw-r--r--  3.0 unx     7275 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-jsx.js
--rw-r--r--  3.0 unx     2634 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-cobol.js
--rw-r--r--  3.0 unx     5558 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-json.js
--rw-r--r--  3.0 unx   378890 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ace.js
--rw-r--r--  3.0 unx     3166 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-eiffel.js
--rw-r--r--  3.0 unx    13684 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-nix.js
--rw-r--r--  3.0 unx    64278 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-smarty.js
--rw-r--r--  3.0 unx    12170 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-xml.js
--rw-r--r--  3.0 unx    14733 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-stylus.js
--rw-r--r--  3.0 unx     1221 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-linking.js
--rw-r--r--  3.0 unx    32478 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-svg.js
--rw-r--r--  3.0 unx     7874 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/keybinding-sublime.js
--rw-r--r--  3.0 unx   102851 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/keybinding-vim.js
--rw-r--r--  3.0 unx    71770 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-html_ruby.js
--rw-r--r--  3.0 unx     2503 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-github.js
--rw-r--r--  3.0 unx     2565 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-dawn.js
--rw-r--r--  3.0 unx     5246 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-maze.js
--rw-r--r--  3.0 unx     7743 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-perl.js
--rw-r--r--  3.0 unx    14856 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-dart.js
--rw-r--r--  3.0 unx     6220 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-jssm.js
--rw-r--r--  3.0 unx     6203 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-json5.js
--rw-r--r--  3.0 unx    11907 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-searchbox.js
--rw-r--r--  3.0 unx     6086 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-jack.js
--rw-r--r--  3.0 unx    64256 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-nunjucks.js
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/swift.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/golang.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/puppet.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/mysql.js
--rw-r--r--  3.0 unx     1269 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/sql.js
--rw-r--r--  3.0 unx     4650 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/java.js
--rw-r--r--  3.0 unx      483 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/assembly_x86.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/tsx.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/rdoc.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/rust.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/yaml.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/powershell.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/perl6.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/rhtml.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/nsis.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/ini.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/julia.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/kotlin.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/haxe.js
--rw-r--r--  3.0 unx      483 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/soy_template.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/red.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/scala.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/dot.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/abap.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/scad.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/jssm.js
--rw-r--r--  3.0 unx     1647 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/dart.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/curly.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/alda.js
--rw-r--r--  3.0 unx     4330 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/django.js
--rw-r--r--  3.0 unx     4174 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/javascript.js
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/logtalk.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/plain_text.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/slim.js
--rw-r--r--  3.0 unx      879 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/diff.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/groovy.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/aql.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/zeek.js
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/luapage.js
--rw-r--r--  3.0 unx      450 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/d.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/jsx.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/nix.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/json5.js
--rw-r--r--  3.0 unx     1593 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/wollok.js
--rw-r--r--  3.0 unx     4648 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/edifact.js
--rw-r--r--  3.0 unx     2305 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/markdown.js
--rw-r--r--  3.0 unx      480 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/html_elixir.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/elixir.js
--rw-r--r--  3.0 unx      498 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/php_laravel_blade.js
--rw-r--r--  3.0 unx     2379 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/sh.js
--rw-r--r--  3.0 unx     3963 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/tex.js
--rw-r--r--  3.0 unx    35750 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/lsl.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/qml.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/ejs.js
--rw-r--r--  3.0 unx     2306 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/haskell.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/latex.js
--rw-r--r--  3.0 unx    19476 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/html.js
--rw-r--r--  3.0 unx     2046 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/jsoniq.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/sass.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/properties.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/csharp.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/prolog.js
--rw-r--r--  3.0 unx     3904 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/erlang.js
--rw-r--r--  3.0 unx     4002 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/python.js
--rw-r--r--  3.0 unx      493 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/razor.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/pascal.js
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/verilog.js
--rw-r--r--  3.0 unx      480 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/visualforce.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/text.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/fsharp.js
--rw-r--r--  3.0 unx      483 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/csound_score.js
--rw-r--r--  3.0 unx     7280 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/php.js
--rw-r--r--  3.0 unx      453 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/bro.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/typescript.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/json.js
--rw-r--r--  3.0 unx    19977 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/css.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/redshift.js
--rw-r--r--  3.0 unx      700 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/drools.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/logiql.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/dockerfile.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/pig.js
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/gherkin.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/cobol.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/xml.js
--rw-r--r--  3.0 unx      598 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/maze.js
--rw-r--r--  3.0 unx     3105 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/jsp.js
--rw-r--r--  3.0 unx      486 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/haskell_cabal.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/elm.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/asciidoc.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/nunjucks.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/pgsql.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/turtle.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/protobuf.js
--rw-r--r--  3.0 unx      474 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/batchfile.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/coldfusion.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/ada.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/praat.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/asl.js
--rw-r--r--  3.0 unx    19852 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/liquid.js
--rw-r--r--  3.0 unx     1274 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/abc.js
--rw-r--r--  3.0 unx    21607 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/ruby.js
--rw-r--r--  3.0 unx      835 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/lua.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/sparql.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/sjs.js
--rw-r--r--  3.0 unx      769 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/rst.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/vhdl.js
--rw-r--r--  3.0 unx     3455 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/vala.js
--rw-r--r--  3.0 unx      999 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/graphqlschema.js
--rw-r--r--  3.0 unx     2371 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/clojure.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/smarty.js
--rw-r--r--  3.0 unx      453 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/fsl.js
--rw-r--r--  3.0 unx      480 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/apache_conf.js
--rw-r--r--  3.0 unx     1545 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/io.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/less.js
--rw-r--r--  3.0 unx      871 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/textile.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/handlebars.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/space.js
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/fortran.js
--rw-r--r--  3.0 unx      530 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/makefile.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/scss.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/nginx.js
--rw-r--r--  3.0 unx      474 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/mediawiki.js
--rw-r--r--  3.0 unx      629 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/snippets.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/apex.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/lisp.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/mixal.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/nim.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/cirru.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/twig.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/eiffel.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/lucene.js
--rw-r--r--  3.0 unx      474 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/gitignore.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/toml.js
--rw-r--r--  3.0 unx      776 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/haml.js
--rw-r--r--  3.0 unx     2017 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/tcl.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/c9search.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/livescript.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/mask.js
--rw-r--r--  3.0 unx     1413 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/csound_orchestra.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/jack.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/forth.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/ocaml.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/jade.js
--rw-r--r--  3.0 unx      474 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/html_ruby.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/hjson.js
--rw-r--r--  3.0 unx      459 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/glsl.js
--rw-r--r--  3.0 unx      983 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/velocity.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/mel.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/prisma.js
--rw-r--r--  3.0 unx      480 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/applescript.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/stylus.js
--rw-r--r--  3.0 unx     2992 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/c_cpp.js
--rw-r--r--  3.0 unx      468 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/crystal.js
--rw-r--r--  3.0 unx      474 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/terraform.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/svg.js
--rw-r--r--  3.0 unx     5841 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/perl.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/objectivec.js
--rw-r--r--  3.0 unx    39441 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/gobstones.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/vbscript.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/ftl.js
--rw-r--r--  3.0 unx      477 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/autohotkey.js
--rw-r--r--  3.0 unx     2563 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/coffee.js
--rw-r--r--  3.0 unx     3309 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/actionscript.js
--rw-r--r--  3.0 unx      462 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/gcode.js
--rw-r--r--  3.0 unx     2046 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/xquery.js
--rw-r--r--  3.0 unx      471 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/mushcode.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/matlab.js
--rw-r--r--  3.0 unx     2472 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/sqlserver.js
--rw-r--r--  3.0 unx      465 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/scheme.js
--rw-r--r--  3.0 unx     2955 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/r.js
--rw-r--r--  3.0 unx      456 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/csp.js
--rw-r--r--  3.0 unx      641 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/snippets/csound_document.js
--rw-r--r--  3.0 unx     2740 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-diff.js
--rw-r--r--  3.0 unx    13106 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-protobuf.js
--rw-r--r--  3.0 unx     3955 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-code_lens.js
--rw-r--r--  3.0 unx    25264 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-mel.js
--rw-r--r--  3.0 unx     2381 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-kuroir.js
--rw-r--r--  3.0 unx    28182 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-gobstones.js
--rw-r--r--  3.0 unx     2705 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-gob.js
--rw-r--r--  3.0 unx    10718 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-praat.js
--rw-r--r--  3.0 unx    27798 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-ambiance.js
--rw-r--r--  3.0 unx    24274 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/keybinding-emacs.js
--rw-r--r--  3.0 unx     3976 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-scheme.js
--rw-r--r--  3.0 unx     3381 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-rst.js
--rw-r--r--  3.0 unx     2623 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-ada.js
--rw-r--r--  3.0 unx     9411 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-zeek.js
--rw-r--r--  3.0 unx     2408 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-vhdl.js
--rw-r--r--  3.0 unx     3371 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-tomorrow_night_blue.js
--rw-r--r--  3.0 unx     9691 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-mediawiki.js
--rw-r--r--  3.0 unx     7554 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-sh.js
--rw-r--r--  3.0 unx     7149 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-terraform.js
--rw-r--r--  3.0 unx   164176 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-javascript.js
--rw-r--r--  3.0 unx     3470 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-dreamweaver.js
--rw-r--r--  3.0 unx     2586 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-rtl.js
--rw-r--r--  3.0 unx    39828 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-haml.js
--rw-r--r--  3.0 unx    40969 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-csound_orchestra.js
--rw-r--r--  3.0 unx    10920 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-logtalk.js
--rw-r--r--  3.0 unx     5666 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-io.js
--rw-r--r--  3.0 unx     7256 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-swift.js
--rw-r--r--  3.0 unx     2244 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-xcode.js
--rw-r--r--  3.0 unx     2520 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-toml.js
--rw-r--r--  3.0 unx    15973 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-sass.js
--rw-r--r--  3.0 unx     5357 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-latex.js
--rw-r--r--  3.0 unx     2412 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-nord_dark.js
--rw-r--r--  3.0 unx    13571 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-glsl.js
--rw-r--r--  3.0 unx     5821 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/keybinding-vscode.js
--rw-r--r--  3.0 unx    18573 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-javascript.js
--rw-r--r--  3.0 unx     6805 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-iplastic.js
--rw-r--r--  3.0 unx    64445 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-twig.js
--rw-r--r--  3.0 unx     3815 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-graphqlschema.js
--rw-r--r--  3.0 unx    24713 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-emmet.js
--rw-r--r--  3.0 unx     6126 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-abap.js
--rw-r--r--  3.0 unx     5499 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-r.js
--rw-r--r--  3.0 unx     6297 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-hjson.js
--rw-r--r--  3.0 unx     1785 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-gcode.js
--rw-r--r--  3.0 unx   231054 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-xquery.js
--rw-r--r--  3.0 unx     7903 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-lua.js
--rw-r--r--  3.0 unx     3242 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-terminal.js
--rw-r--r--  3.0 unx    62691 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-handlebars.js
--rw-r--r--  3.0 unx    77632 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/worker-php.js
--rw-r--r--  3.0 unx    65593 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-velocity.js
--rw-r--r--  3.0 unx     8573 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-prisma.js
--rw-r--r--  3.0 unx     3332 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-cirru.js
--rw-r--r--  3.0 unx    15430 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-settings_menu.js
--rw-r--r--  3.0 unx    33020 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-powershell.js
--rw-r--r--  3.0 unx    69552 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-luapage.js
--rw-r--r--  3.0 unx     2885 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-tomorrow.js
--rw-r--r--  3.0 unx     2607 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-haskell_cabal.js
--rw-r--r--  3.0 unx     1277 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-statusbar.js
--rw-r--r--  3.0 unx     3223 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-verilog.js
--rw-r--r--  3.0 unx      328 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-text.js
--rw-r--r--  3.0 unx     7887 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-dot.js
--rw-r--r--  3.0 unx    37480 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-jsp.js
--rw-r--r--  3.0 unx     2768 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/theme-clouds_midnight.js
--rw-r--r--  3.0 unx      335 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/ext-error_marker.js
--rw-r--r--  3.0 unx     5765 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-fsharp.js
--rw-r--r--  3.0 unx   101890 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-slim.js
--rw-r--r--  3.0 unx     2281 tx defN 23-Jan-12 14:39 flexmin/static/ace/src-min/mode-lisp.js
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/static/components/
--rw-r--r--  3.0 unx     4687 tx defN 23-Jan-12 14:39 flexmin/static/components/auth.js
--rw-r--r--  3.0 unx     8195 tx defN 23-Jan-12 14:39 flexmin/static/components/auth.html
--rw-r--r--  3.0 unx      376 tx defN 23-Jan-12 14:39 flexmin/__init__.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 flexmin/templates/
--rw-r--r--  3.0 unx     1227 tx defN 23-Jan-12 14:39 flexmin/templates/menu.html
--rw-r--r--  3.0 unx     1072 tx defN 23-Jan-12 14:39 flexmin/templates/index.html
--rw-r--r--  3.0 unx     4983 tx defN 23-Jan-12 14:39 flexmin/templates/action.html
--rw-r--r--  3.0 unx    13247 tx defN 23-Jan-12 14:39 flexmin/templates/action_tables.html
--rw-r--r--  3.0 unx     7217 tx defN 23-Jan-12 14:39 flexmin/templates/action_forms.html
--rw-r--r--  3.0 unx      228 tx defN 23-Jan-12 14:39 flexmin/templates/generic.html
--rw-r--r--  3.0 unx        1 tx stor 23-Jan-12 14:39 flexmin/templates/README.md
--rw-r--r--  3.0 unx      706 tx defN 23-Jan-12 14:39 flexmin/templates/login.html
--rw-r--r--  3.0 unx      918 tx defN 23-Jan-12 14:39 flexmin/templates/reload.html
--rw-r--r--  3.0 unx     5178 tx defN 23-Jan-12 14:39 flexmin/templates/history.html
--rw-r--r--  3.0 unx     3397 tx defN 23-Jan-12 14:39 flexmin/templates/layout.html
--rw-r--r--  3.0 unx      414 tx defN 23-Jan-12 14:39 flexmin/templates/auth.html
--rw-r--r--  3.0 unx      103 tx defN 23-Jan-12 14:39 flexmin/templates/test.html
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/
--rw-r--r--  3.0 unx     5212 tx defN 23-Jan-12 14:39 _dashboard/diff2kryten.py
--rw-r--r--  3.0 unx     3965 tx defN 23-Jan-12 14:39 _dashboard/utils.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/__pycache__/
--rw-r--r--  3.0 unx     4680 bx defN 23-Jan-12 14:39 _dashboard/__pycache__/diff2kryten.cpython-38.pyc
--rw-r--r--  3.0 unx    13210 bx defN 23-Jan-12 14:39 _dashboard/__pycache__/__init__.cpython-38.pyc
--rw-r--r--  3.0 unx     3923 bx defN 23-Jan-12 14:39 _dashboard/__pycache__/utils.cpython-38.pyc
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/translations/
--rw-r--r--  3.0 unx        1 tx stor 23-Jan-12 14:39 _dashboard/translations/README.md
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/ace/src-min/
+-rw-r--r--  3.0 unx     2680 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-cobalt.js
+-rw-r--r--  3.0 unx     2688 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-gherkin.js
+-rw-r--r--  3.0 unx    32956 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-ftl.js
+-rw-r--r--  3.0 unx    11851 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-haskell.js
+-rw-r--r--  3.0 unx    16788 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-sqlserver.js
+-rw-r--r--  3.0 unx     2941 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-textmate.js
+-rw-r--r--  3.0 unx     3127 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-mono_industrial.js
+-rw-r--r--  3.0 unx    65868 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-rhtml.js
+-rw-r--r--  3.0 unx    67925 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-razor.js
+-rw-r--r--  3.0 unx     8479 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-asciidoc.js
+-rw-r--r--  3.0 unx    65423 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-liquid.js
+-rw-r--r--  3.0 unx     8701 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-apex.js
+-rw-r--r--  3.0 unx     5397 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-vbscript.js
+-rw-r--r--  3.0 unx     2968 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-pastel_on_dark.js
+-rw-r--r--  3.0 unx     1588 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-spellcheck.js
+-rw-r--r--  3.0 unx    61830 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-curly.js
+-rw-r--r--  3.0 unx    59455 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-pgsql.js
+-rw-r--r--  3.0 unx     3165 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-mixal.js
+-rw-r--r--  3.0 unx  1633164 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-xquery.js
+-rw-r--r--  3.0 unx     6840 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-mysql.js
+-rw-r--r--  3.0 unx   217050 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-html.js
+-rw-r--r--  3.0 unx     1425 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-properties.js
+-rw-r--r--  3.0 unx     6516 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-tcl.js
+-rw-r--r--  3.0 unx     9170 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-csharp.js
+-rw-r--r--  3.0 unx     5399 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-livescript.js
+-rw-r--r--  3.0 unx     8128 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-python.js
+-rw-r--r--  3.0 unx     3222 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-sqlserver.js
+-rw-r--r--  3.0 unx     9332 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-textarea.js
+-rw-r--r--  3.0 unx     2647 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-solarized_dark.js
+-rw-r--r--  3.0 unx     2696 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-solarized_light.js
+-rw-r--r--  3.0 unx     2553 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-space.js
+-rw-r--r--  3.0 unx   331682 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-coffee.js
+-rw-r--r--  3.0 unx     3245 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-whitespace.js
+-rw-r--r--  3.0 unx     1224 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-gitignore.js
+-rw-r--r--  3.0 unx     9266 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-d.js
+-rw-r--r--  3.0 unx    15910 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-ocaml.js
+-rw-r--r--  3.0 unx     8317 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-redshift.js
+-rw-r--r--  3.0 unx    63985 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-autohotkey.js
+-rw-r--r--  3.0 unx    63476 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-visualforce.js
+-rw-r--r--  3.0 unx    16939 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-vala.js
+-rw-r--r--  3.0 unx    10652 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-nsis.js
+-rw-r--r--  3.0 unx     3458 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-katzenmilch.js
+-rw-r--r--  3.0 unx     4254 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-qml.js
+-rw-r--r--  3.0 unx     5187 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-batchfile.js
+-rw-r--r--  3.0 unx     2625 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-kr_theme.js
+-rw-r--r--  3.0 unx     6851 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-haxe.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-sql.js
+-rw-r--r--  3.0 unx    55117 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-xml.js
+-rw-r--r--  3.0 unx   473743 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-php.js
+-rw-r--r--  3.0 unx     4016 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-static_highlight.js
+-rw-r--r--  3.0 unx    20347 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-typescript.js
+-rw-r--r--  3.0 unx    23819 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-java.js
+-rw-r--r--  3.0 unx    39316 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-language_tools.js
+-rw-r--r--  3.0 unx     1568 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-csp.js
+-rw-r--r--  3.0 unx     5076 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-yaml.js
+-rw-r--r--  3.0 unx    24007 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-scss.js
+-rw-r--r--  3.0 unx     3148 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-edifact.js
+-rw-r--r--  3.0 unx     2912 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-dracula.js
+-rw-r--r--  3.0 unx    10453 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-ruby.js
+-rw-r--r--  3.0 unx     7316 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-forth.js
+-rw-r--r--  3.0 unx     9069 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-asl.js
+-rw-r--r--  3.0 unx     5037 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-fsl.js
+-rw-r--r--  3.0 unx    30080 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-erlang.js
+-rw-r--r--  3.0 unx    20829 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-css.js
+-rw-r--r--  3.0 unx    60818 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-html.js
+-rw-r--r--  3.0 unx    46803 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-lua.js
+-rw-r--r--  3.0 unx    16071 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-elixir.js
+-rw-r--r--  3.0 unx     2536 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-vibrant_ink.js
+-rw-r--r--  3.0 unx   233671 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-jsoniq.js
+-rw-r--r--  3.0 unx     7959 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-csound_score.js
+-rw-r--r--  3.0 unx     4258 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-beautify.js
+-rw-r--r--  3.0 unx    71439 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-ejs.js
+-rw-r--r--  3.0 unx     6026 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-logiql.js
+-rw-r--r--  3.0 unx     8757 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-fortran.js
+-rw-r--r--  3.0 unx    21771 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-sjs.js
+-rw-r--r--  3.0 unx    78008 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-html_elixir.js
+-rw-r--r--  3.0 unx    20840 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-wollok.js
+-rw-r--r--  3.0 unx    20926 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-actionscript.js
+-rw-r--r--  3.0 unx    47702 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-jade.js
+-rw-r--r--  3.0 unx     3025 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-ini.js
+-rw-r--r--  3.0 unx     7032 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-mushcode.js
+-rw-r--r--  3.0 unx    63341 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-coldfusion.js
+-rw-r--r--  3.0 unx     5258 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-elm.js
+-rw-r--r--  3.0 unx   478207 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-php_laravel_blade.js
+-rw-r--r--  3.0 unx     5732 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-applescript.js
+-rw-r--r--  3.0 unx     5390 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-alda.js
+-rw-r--r--  3.0 unx     6937 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-nim.js
+-rw-r--r--  3.0 unx     1695 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-themelist.js
+-rw-r--r--  3.0 unx    12924 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-red.js
+-rw-r--r--  3.0 unx    11412 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-c_cpp.js
+-rw-r--r--  3.0 unx    10323 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-crystal.js
+-rw-r--r--  3.0 unx     4031 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-elastic_tabstops_lite.js
+-rw-r--r--  3.0 unx     7461 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-puppet.js
+-rw-r--r--  3.0 unx    14877 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-options.js
+-rw-r--r--  3.0 unx    17977 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-perl6.js
+-rw-r--r--  3.0 unx    14242 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-apache_conf.js
+-rw-r--r--  3.0 unx     3147 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-crimson_editor.js
+-rw-r--r--  3.0 unx   140785 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-css.js
+-rw-r--r--  3.0 unx    11545 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-drools.js
+-rw-r--r--  3.0 unx    42578 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-mask.js
+-rw-r--r--  3.0 unx    16214 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-nginx.js
+-rw-r--r--  3.0 unx     2408 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-clouds.js
+-rw-r--r--  3.0 unx     5352 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-turtle.js
+-rw-r--r--  3.0 unx    23112 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-scala.js
+-rw-r--r--  3.0 unx    32595 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-json.js
+-rw-r--r--  3.0 unx     6950 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-rust.js
+-rw-r--r--  3.0 unx     3179 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-chaos.js
+-rw-r--r--  3.0 unx     3952 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-keybinding_menu.js
+-rw-r--r--  3.0 unx    72376 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-csound_document.js
+-rw-r--r--  3.0 unx     1995 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-gruvbox.js
+-rw-r--r--  3.0 unx     6917 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-makefile.js
+-rw-r--r--  3.0 unx     2566 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-merbivore.js
+-rw-r--r--  3.0 unx     8695 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-prolog.js
+-rw-r--r--  3.0 unx     4398 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-c9search.js
+-rw-r--r--  3.0 unx     2783 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-merbivore_soft.js
+-rw-r--r--  3.0 unx     6831 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-scad.js
+-rw-r--r--  3.0 unx     8183 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-sparql.js
+-rw-r--r--  3.0 unx    20648 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-tsx.js
+-rw-r--r--  3.0 unx     2448 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-textile.js
+-rw-r--r--  3.0 unx     4054 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-snippets.js
+-rw-r--r--  3.0 unx     2581 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-idle_fingers.js
+-rw-r--r--  3.0 unx    50014 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-prompt.js
+-rw-r--r--  3.0 unx     8389 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-clojure.js
+-rw-r--r--  3.0 unx     3114 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-tex.js
+-rw-r--r--  3.0 unx     6536 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-bro.js
+-rw-r--r--  3.0 unx      836 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-plain_text.js
+-rw-r--r--  3.0 unx     7778 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-coffee.js
+-rw-r--r--  3.0 unx     3435 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-aql.js
+-rw-r--r--  3.0 unx     2773 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-lucene.js
+-rw-r--r--  3.0 unx    62174 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-django.js
+-rw-r--r--  3.0 unx     4712 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-modelist.js
+-rw-r--r--  3.0 unx     3565 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-tomorrow_night_eighties.js
+-rw-r--r--  3.0 unx    20889 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-matlab.js
+-rw-r--r--  3.0 unx    26979 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-lsl.js
+-rw-r--r--  3.0 unx     3838 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-tomorrow_night_bright.js
+-rw-r--r--  3.0 unx     5072 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-abc.js
+-rw-r--r--  3.0 unx    22934 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-groovy.js
+-rw-r--r--  3.0 unx     2828 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-twilight.js
+-rw-r--r--  3.0 unx     3866 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-split.js
+-rw-r--r--  3.0 unx    72574 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-markdown.js
+-rw-r--r--  3.0 unx     4505 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-pascal.js
+-rw-r--r--  3.0 unx    22820 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-less.js
+-rw-r--r--  3.0 unx     3155 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-tomorrow_night.js
+-rw-r--r--  3.0 unx    12257 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-kotlin.js
+-rw-r--r--  3.0 unx     2703 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-monokai.js
+-rw-r--r--  3.0 unx     7866 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-julia.js
+-rw-r--r--  3.0 unx     7233 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-golang.js
+-rw-r--r--  3.0 unx     9224 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-assembly_x86.js
+-rw-r--r--  3.0 unx     8591 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-dockerfile.js
+-rw-r--r--  3.0 unx     2453 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-eclipse.js
+-rw-r--r--  3.0 unx     3039 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-chrome.js
+-rw-r--r--  3.0 unx    55045 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-objectivec.js
+-rw-r--r--  3.0 unx    69313 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-soy_template.js
+-rw-r--r--  3.0 unx     6637 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-pig.js
+-rw-r--r--  3.0 unx     5004 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-rdoc.js
+-rw-r--r--  3.0 unx     7275 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-jsx.js
+-rw-r--r--  3.0 unx     2634 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-cobol.js
+-rw-r--r--  3.0 unx     5558 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-json.js
+-rw-r--r--  3.0 unx   378890 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ace.js
+-rw-r--r--  3.0 unx     3166 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-eiffel.js
+-rw-r--r--  3.0 unx    13684 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-nix.js
+-rw-r--r--  3.0 unx    64278 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-smarty.js
+-rw-r--r--  3.0 unx    12170 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-xml.js
+-rw-r--r--  3.0 unx    14733 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-stylus.js
+-rw-r--r--  3.0 unx     1221 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-linking.js
+-rw-r--r--  3.0 unx    32478 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-svg.js
+-rw-r--r--  3.0 unx     7874 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/keybinding-sublime.js
+-rw-r--r--  3.0 unx   102851 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/keybinding-vim.js
+-rw-r--r--  3.0 unx    71770 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-html_ruby.js
+-rw-r--r--  3.0 unx     2503 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-github.js
+-rw-r--r--  3.0 unx     2565 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-dawn.js
+-rw-r--r--  3.0 unx     5246 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-maze.js
+-rw-r--r--  3.0 unx     7743 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-perl.js
+-rw-r--r--  3.0 unx    14856 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-dart.js
+-rw-r--r--  3.0 unx     6220 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-jssm.js
+-rw-r--r--  3.0 unx     6203 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-json5.js
+-rw-r--r--  3.0 unx    11907 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-searchbox.js
+-rw-r--r--  3.0 unx     6086 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-jack.js
+-rw-r--r--  3.0 unx    64256 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-nunjucks.js
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/swift.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/golang.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/puppet.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/mysql.js
+-rw-r--r--  3.0 unx     1269 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/sql.js
+-rw-r--r--  3.0 unx     4650 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/java.js
+-rw-r--r--  3.0 unx      483 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/assembly_x86.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/tsx.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/rdoc.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/rust.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/yaml.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/powershell.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/perl6.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/rhtml.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/nsis.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/ini.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/julia.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/kotlin.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/haxe.js
+-rw-r--r--  3.0 unx      483 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/soy_template.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/red.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/scala.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/dot.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/abap.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/scad.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/jssm.js
+-rw-r--r--  3.0 unx     1647 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/dart.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/curly.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/alda.js
+-rw-r--r--  3.0 unx     4330 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/django.js
+-rw-r--r--  3.0 unx     4174 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/javascript.js
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/logtalk.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/plain_text.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/slim.js
+-rw-r--r--  3.0 unx      879 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/diff.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/groovy.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/aql.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/zeek.js
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/luapage.js
+-rw-r--r--  3.0 unx      450 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/d.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/jsx.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/nix.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/json5.js
+-rw-r--r--  3.0 unx     1593 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/wollok.js
+-rw-r--r--  3.0 unx     4648 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/edifact.js
+-rw-r--r--  3.0 unx     2305 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/markdown.js
+-rw-r--r--  3.0 unx      480 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/html_elixir.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/elixir.js
+-rw-r--r--  3.0 unx      498 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/php_laravel_blade.js
+-rw-r--r--  3.0 unx     2379 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/sh.js
+-rw-r--r--  3.0 unx     3963 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/tex.js
+-rw-r--r--  3.0 unx    35750 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/lsl.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/qml.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/ejs.js
+-rw-r--r--  3.0 unx     2306 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/haskell.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/latex.js
+-rw-r--r--  3.0 unx    19476 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/html.js
+-rw-r--r--  3.0 unx     2046 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/jsoniq.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/sass.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/properties.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/csharp.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/prolog.js
+-rw-r--r--  3.0 unx     3904 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/erlang.js
+-rw-r--r--  3.0 unx     4002 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/python.js
+-rw-r--r--  3.0 unx      493 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/razor.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/pascal.js
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/verilog.js
+-rw-r--r--  3.0 unx      480 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/visualforce.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/text.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/fsharp.js
+-rw-r--r--  3.0 unx      483 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/csound_score.js
+-rw-r--r--  3.0 unx     7280 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/php.js
+-rw-r--r--  3.0 unx      453 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/bro.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/typescript.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/json.js
+-rw-r--r--  3.0 unx    19977 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/css.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/redshift.js
+-rw-r--r--  3.0 unx      700 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/drools.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/logiql.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/dockerfile.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/pig.js
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/gherkin.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/cobol.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/xml.js
+-rw-r--r--  3.0 unx      598 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/maze.js
+-rw-r--r--  3.0 unx     3105 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/jsp.js
+-rw-r--r--  3.0 unx      486 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/haskell_cabal.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/elm.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/asciidoc.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/nunjucks.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/pgsql.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/turtle.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/protobuf.js
+-rw-r--r--  3.0 unx      474 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/batchfile.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/coldfusion.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/ada.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/praat.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/asl.js
+-rw-r--r--  3.0 unx    19852 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/liquid.js
+-rw-r--r--  3.0 unx     1274 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/abc.js
+-rw-r--r--  3.0 unx    21607 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/ruby.js
+-rw-r--r--  3.0 unx      835 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/lua.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/sparql.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/sjs.js
+-rw-r--r--  3.0 unx      769 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/rst.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/vhdl.js
+-rw-r--r--  3.0 unx     3455 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/vala.js
+-rw-r--r--  3.0 unx      999 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/graphqlschema.js
+-rw-r--r--  3.0 unx     2371 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/clojure.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/smarty.js
+-rw-r--r--  3.0 unx      453 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/fsl.js
+-rw-r--r--  3.0 unx      480 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/apache_conf.js
+-rw-r--r--  3.0 unx     1545 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/io.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/less.js
+-rw-r--r--  3.0 unx      871 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/textile.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/handlebars.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/space.js
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/fortran.js
+-rw-r--r--  3.0 unx      530 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/makefile.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/scss.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/nginx.js
+-rw-r--r--  3.0 unx      474 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/mediawiki.js
+-rw-r--r--  3.0 unx      629 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/snippets.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/apex.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/lisp.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/mixal.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/nim.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/cirru.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/twig.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/eiffel.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/lucene.js
+-rw-r--r--  3.0 unx      474 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/gitignore.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/toml.js
+-rw-r--r--  3.0 unx      776 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/haml.js
+-rw-r--r--  3.0 unx     2017 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/tcl.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/c9search.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/livescript.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/mask.js
+-rw-r--r--  3.0 unx     1413 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/csound_orchestra.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/jack.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/forth.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/ocaml.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/jade.js
+-rw-r--r--  3.0 unx      474 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/html_ruby.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/hjson.js
+-rw-r--r--  3.0 unx      459 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/glsl.js
+-rw-r--r--  3.0 unx      983 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/velocity.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/mel.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/prisma.js
+-rw-r--r--  3.0 unx      480 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/applescript.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/stylus.js
+-rw-r--r--  3.0 unx     2992 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/c_cpp.js
+-rw-r--r--  3.0 unx      468 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/crystal.js
+-rw-r--r--  3.0 unx      474 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/terraform.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/svg.js
+-rw-r--r--  3.0 unx     5841 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/perl.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/objectivec.js
+-rw-r--r--  3.0 unx    39441 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/gobstones.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/vbscript.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/ftl.js
+-rw-r--r--  3.0 unx      477 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/autohotkey.js
+-rw-r--r--  3.0 unx     2563 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/coffee.js
+-rw-r--r--  3.0 unx     3309 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/actionscript.js
+-rw-r--r--  3.0 unx      462 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/gcode.js
+-rw-r--r--  3.0 unx     2046 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/xquery.js
+-rw-r--r--  3.0 unx      471 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/mushcode.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/matlab.js
+-rw-r--r--  3.0 unx     2472 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/sqlserver.js
+-rw-r--r--  3.0 unx      465 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/scheme.js
+-rw-r--r--  3.0 unx     2955 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/r.js
+-rw-r--r--  3.0 unx      456 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/csp.js
+-rw-r--r--  3.0 unx      641 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/snippets/csound_document.js
+-rw-r--r--  3.0 unx     2740 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-diff.js
+-rw-r--r--  3.0 unx    13106 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-protobuf.js
+-rw-r--r--  3.0 unx     3955 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-code_lens.js
+-rw-r--r--  3.0 unx    25264 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-mel.js
+-rw-r--r--  3.0 unx     2381 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-kuroir.js
+-rw-r--r--  3.0 unx    28182 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-gobstones.js
+-rw-r--r--  3.0 unx     2705 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-gob.js
+-rw-r--r--  3.0 unx    10718 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-praat.js
+-rw-r--r--  3.0 unx    27798 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-ambiance.js
+-rw-r--r--  3.0 unx    24274 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/keybinding-emacs.js
+-rw-r--r--  3.0 unx     3976 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-scheme.js
+-rw-r--r--  3.0 unx     3381 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-rst.js
+-rw-r--r--  3.0 unx     2623 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-ada.js
+-rw-r--r--  3.0 unx     9411 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-zeek.js
+-rw-r--r--  3.0 unx     2408 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-vhdl.js
+-rw-r--r--  3.0 unx     3371 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-tomorrow_night_blue.js
+-rw-r--r--  3.0 unx     9691 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-mediawiki.js
+-rw-r--r--  3.0 unx     7554 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-sh.js
+-rw-r--r--  3.0 unx     7149 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-terraform.js
+-rw-r--r--  3.0 unx   164176 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-javascript.js
+-rw-r--r--  3.0 unx     3470 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-dreamweaver.js
+-rw-r--r--  3.0 unx     2586 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-rtl.js
+-rw-r--r--  3.0 unx    39828 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-haml.js
+-rw-r--r--  3.0 unx    40969 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-csound_orchestra.js
+-rw-r--r--  3.0 unx    10920 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-logtalk.js
+-rw-r--r--  3.0 unx     5666 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-io.js
+-rw-r--r--  3.0 unx     7256 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-swift.js
+-rw-r--r--  3.0 unx     2244 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-xcode.js
+-rw-r--r--  3.0 unx     2520 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-toml.js
+-rw-r--r--  3.0 unx    15973 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-sass.js
+-rw-r--r--  3.0 unx     5357 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-latex.js
+-rw-r--r--  3.0 unx     2412 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-nord_dark.js
+-rw-r--r--  3.0 unx    13571 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-glsl.js
+-rw-r--r--  3.0 unx     5821 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/keybinding-vscode.js
+-rw-r--r--  3.0 unx    18573 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-javascript.js
+-rw-r--r--  3.0 unx     6805 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-iplastic.js
+-rw-r--r--  3.0 unx    64445 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-twig.js
+-rw-r--r--  3.0 unx     3815 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-graphqlschema.js
+-rw-r--r--  3.0 unx    24713 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-emmet.js
+-rw-r--r--  3.0 unx     6126 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-abap.js
+-rw-r--r--  3.0 unx     5499 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-r.js
+-rw-r--r--  3.0 unx     6297 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-hjson.js
+-rw-r--r--  3.0 unx     1785 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-gcode.js
+-rw-r--r--  3.0 unx   231054 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-xquery.js
+-rw-r--r--  3.0 unx     7903 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-lua.js
+-rw-r--r--  3.0 unx     3242 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-terminal.js
+-rw-r--r--  3.0 unx    62691 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-handlebars.js
+-rw-r--r--  3.0 unx    77632 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/worker-php.js
+-rw-r--r--  3.0 unx    65593 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-velocity.js
+-rw-r--r--  3.0 unx     8573 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-prisma.js
+-rw-r--r--  3.0 unx     3332 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-cirru.js
+-rw-r--r--  3.0 unx    15430 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-settings_menu.js
+-rw-r--r--  3.0 unx    33020 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-powershell.js
+-rw-r--r--  3.0 unx    69552 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-luapage.js
+-rw-r--r--  3.0 unx     2885 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-tomorrow.js
+-rw-r--r--  3.0 unx     2607 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-haskell_cabal.js
+-rw-r--r--  3.0 unx     1277 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-statusbar.js
+-rw-r--r--  3.0 unx     3223 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-verilog.js
+-rw-r--r--  3.0 unx      328 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-text.js
+-rw-r--r--  3.0 unx     7887 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-dot.js
+-rw-r--r--  3.0 unx    37480 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-jsp.js
+-rw-r--r--  3.0 unx     2768 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/theme-clouds_midnight.js
+-rw-r--r--  3.0 unx      335 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/ext-error_marker.js
+-rw-r--r--  3.0 unx     5765 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-fsharp.js
+-rw-r--r--  3.0 unx   101890 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-slim.js
+-rw-r--r--  3.0 unx     2281 tx defN 23-Jan-15 14:39 flexmin/static/ace/src-min/mode-lisp.js
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/static/components/
+-rw-r--r--  3.0 unx     4687 tx defN 23-Jan-15 14:39 flexmin/static/components/auth.js
+-rw-r--r--  3.0 unx     8195 tx defN 23-Jan-15 14:39 flexmin/static/components/auth.html
+-rw-r--r--  3.0 unx      376 tx defN 23-Jan-15 14:39 flexmin/__init__.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 flexmin/templates/
+-rw-r--r--  3.0 unx     1227 tx defN 23-Jan-15 14:39 flexmin/templates/menu.html
+-rw-r--r--  3.0 unx     1072 tx defN 23-Jan-15 14:39 flexmin/templates/index.html
+-rw-r--r--  3.0 unx     4983 tx defN 23-Jan-15 14:39 flexmin/templates/action.html
+-rw-r--r--  3.0 unx    13247 tx defN 23-Jan-15 14:39 flexmin/templates/action_tables.html
+-rw-r--r--  3.0 unx     7217 tx defN 23-Jan-15 14:39 flexmin/templates/action_forms.html
+-rw-r--r--  3.0 unx      228 tx defN 23-Jan-15 14:39 flexmin/templates/generic.html
+-rw-r--r--  3.0 unx        1 tx stor 23-Jan-15 14:39 flexmin/templates/README.md
+-rw-r--r--  3.0 unx      706 tx defN 23-Jan-15 14:39 flexmin/templates/login.html
+-rw-r--r--  3.0 unx      918 tx defN 23-Jan-15 14:39 flexmin/templates/reload.html
+-rw-r--r--  3.0 unx     5178 tx defN 23-Jan-15 14:39 flexmin/templates/history.html
+-rw-r--r--  3.0 unx     3397 tx defN 23-Jan-15 14:39 flexmin/templates/layout.html
+-rw-r--r--  3.0 unx      414 tx defN 23-Jan-15 14:39 flexmin/templates/auth.html
+-rw-r--r--  3.0 unx      103 tx defN 23-Jan-15 14:39 flexmin/templates/test.html
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/
+-rw-r--r--  3.0 unx     5212 tx defN 23-Jan-15 14:39 _dashboard/diff2kryten.py
+-rw-r--r--  3.0 unx     3965 tx defN 23-Jan-15 14:39 _dashboard/utils.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/__pycache__/
+-rw-r--r--  3.0 unx     4680 bx defN 23-Jan-15 14:39 _dashboard/__pycache__/diff2kryten.cpython-38.pyc
+-rw-r--r--  3.0 unx    13210 bx defN 23-Jan-15 14:39 _dashboard/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--  3.0 unx     3923 bx defN 23-Jan-15 14:39 _dashboard/__pycache__/utils.cpython-38.pyc
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/translations/
+-rw-r--r--  3.0 unx        1 tx stor 23-Jan-15 14:39 _dashboard/translations/README.md
 drwxr-xr-x  3.0 unx        0 bx stor 20-Jul-28 14:03 _dashboard/static/
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/css/
--rw-r--r--  3.0 unx     5742 tx defN 23-Jan-12 14:39 _dashboard/static/css/future.css
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/images/
--rw-r--r--  3.0 unx    13366 bx defN 23-Jan-12 14:39 _dashboard/static/images/alert-orange.gif
--rw-r--r--  3.0 unx    12305 bx defN 23-Jan-12 14:39 _dashboard/static/images/alert-blue.gif
--rw-r--r--  3.0 unx  1010153 bx defN 23-Jan-12 14:39 _dashboard/static/images/widget.gif
--rw-r--r--  3.0 unx    12025 bx defN 23-Jan-12 14:39 _dashboard/static/images/alert-red.gif
--rw-r--r--  3.0 unx    13380 bx defN 23-Jan-12 14:39 _dashboard/static/images/alert-yellow.gif
--rw-r--r--  3.0 unx     7927 bx defN 23-Jan-12 14:39 _dashboard/static/images/forkme.png
--rw-r--r--  3.0 unx    11068 bx defN 23-Jan-12 14:39 _dashboard/static/images/alert-green.gif
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/js/
--rw-r--r--  3.0 unx      405 tx defN 23-Jan-12 14:39 _dashboard/static/js/dbadmin.js
--rw-r--r--  3.0 unx    68547 tx defN 23-Jan-12 14:39 _dashboard/static/js/sugar.min.js
--rw-r--r--  3.0 unx     4963 tx defN 23-Jan-12 14:39 _dashboard/static/js/utils.js
--rw-r--r--  3.0 unx    76004 tx defN 23-Jan-12 14:39 _dashboard/static/js/vue.min.js
--rw-r--r--  3.0 unx    88145 tx defN 23-Jan-12 14:39 _dashboard/static/js/jquery.min.js
--rw-r--r--  3.0 unx     9231 tx defN 23-Jan-12 14:39 _dashboard/static/js/index.js
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/js/ace/
--rw-r--r--  3.0 unx     2353 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-cobalt.js
--rw-r--r--  3.0 unx     2380 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-gherkin.js
--rw-r--r--  3.0 unx    30624 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-ftl.js
--rw-r--r--  3.0 unx    11468 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-haskell.js
--rw-r--r--  3.0 unx    16415 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-sqlserver.js
--rw-r--r--  3.0 unx     2585 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-textmate.js
--rw-r--r--  3.0 unx     2791 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-mono_industrial.js
--rw-r--r--  3.0 unx    62955 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-rhtml.js
--rw-r--r--  3.0 unx    64984 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-razor.js
--rw-r--r--  3.0 unx     8159 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-asciidoc.js
--rw-r--r--  3.0 unx    30271 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-liquid.js
--rw-r--r--  3.0 unx     5073 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-vbscript.js
--rw-r--r--  3.0 unx     2633 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-pastel_on_dark.js
--rw-r--r--  3.0 unx     1440 bx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-spellcheck.js
--rw-r--r--  3.0 unx    58909 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-curly.js
--rw-r--r--  3.0 unx    55911 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-pgsql.js
--rw-r--r--  3.0 unx  1177601 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-xquery.js
--rw-r--r--  3.0 unx     6523 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-mysql.js
--rw-r--r--  3.0 unx   217401 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-html.js
--rw-r--r--  3.0 unx     1099 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-properties.js
--rw-r--r--  3.0 unx     6120 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-tcl.js
--rw-r--r--  3.0 unx     8840 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-csharp.js
--rw-r--r--  3.0 unx     4984 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-livescript.js
--rw-r--r--  3.0 unx     4681 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-python.js
--rw-r--r--  3.0 unx     2892 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-sqlserver.js
--rw-r--r--  3.0 unx     9112 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-textarea.js
--rw-r--r--  3.0 unx     2312 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-solarized_dark.js
--rw-r--r--  3.0 unx     2360 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-solarized_light.js
--rw-r--r--  3.0 unx     2236 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-space.js
--rw-r--r--  3.0 unx   190654 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-coffee.js
--rw-r--r--  3.0 unx     2572 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-whitespace.js
--rw-r--r--  3.0 unx      899 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-gitignore.js
--rw-r--r--  3.0 unx     8947 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-d.js
--rw-r--r--  3.0 unx    15600 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-ocaml.js
--rw-r--r--  3.0 unx    63640 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-autohotkey.js
--rw-r--r--  3.0 unx    16578 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-vala.js
--rw-r--r--  3.0 unx    10035 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-nsis.js
--rw-r--r--  3.0 unx     3126 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-katzenmilch.js
--rw-r--r--  3.0 unx     4856 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-batchfile.js
--rw-r--r--  3.0 unx     2296 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-kr_theme.js
--rw-r--r--  3.0 unx     6540 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-haxe.js
--rw-r--r--  3.0 unx     1811 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-sql.js
--rw-r--r--  3.0 unx    11914 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-old_ie.js
--rw-r--r--  3.0 unx    55541 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-xml.js
--rw-r--r--  3.0 unx   470435 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-php.js
--rw-r--r--  3.0 unx     2819 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-static_highlight.js
--rw-r--r--  3.0 unx    20198 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-typescript.js
--rw-r--r--  3.0 unx    21805 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-java.js
--rw-r--r--  3.0 unx    34464 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-language_tools.js
--rw-r--r--  3.0 unx     3994 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-yaml.js
--rw-r--r--  3.0 unx    12951 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-scss.js
--rw-r--r--  3.0 unx    10025 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-ruby.js
--rw-r--r--  3.0 unx     6989 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-forth.js
--rw-r--r--  3.0 unx    19962 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-live_script.js
--rw-r--r--  3.0 unx    29711 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-erlang.js
--rw-r--r--  3.0 unx    18046 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-css.js
--rw-r--r--  3.0 unx    57890 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-html.js
--rw-r--r--  3.0 unx    47114 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-lua.js
--rw-r--r--  3.0 unx    15753 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-elixir.js
--rw-r--r--  3.0 unx     2204 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-vibrant_ink.js
--rw-r--r--  3.0 unx   232939 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-jsoniq.js
--rw-r--r--  3.0 unx     3818 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-beautify.js
--rw-r--r--  3.0 unx    68412 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-ejs.js
--rw-r--r--  3.0 unx     5712 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-logiql.js
--rw-r--r--  3.0 unx     8428 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-fortran.js
--rw-r--r--  3.0 unx    21273 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-sjs.js
--rw-r--r--  3.0 unx    75093 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-html_elixir.js
--rw-r--r--  3.0 unx    20269 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-wollok.js
--rw-r--r--  3.0 unx    20545 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-actionscript.js
--rw-r--r--  3.0 unx    49991 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-jade.js
--rw-r--r--  3.0 unx     2710 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-ini.js
--rw-r--r--  3.0 unx     6712 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-mushcode.js
--rw-r--r--  3.0 unx    60415 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-coldfusion.js
--rw-r--r--  3.0 unx     4933 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-elm.js
--rw-r--r--  3.0 unx     5399 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-applescript.js
--rw-r--r--  3.0 unx     1470 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-themelist.js
--rw-r--r--  3.0 unx    10840 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-c_cpp.js
--rw-r--r--  3.0 unx     3840 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-elastic_tabstops_lite.js
--rw-r--r--  3.0 unx    13909 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-apache_conf.js
--rw-r--r--  3.0 unx     2812 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-crimson_editor.js
--rw-r--r--  3.0 unx   140879 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-css.js
--rw-r--r--  3.0 unx    10785 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-drools.js
--rw-r--r--  3.0 unx    40358 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-mask.js
--rw-r--r--  3.0 unx    31151 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-swig.js
--rw-r--r--  3.0 unx     2081 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-clouds.js
--rw-r--r--  3.0 unx    22619 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-scala.js
--rw-r--r--  3.0 unx    32911 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-json.js
--rw-r--r--  3.0 unx     6495 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-rust.js
--rw-r--r--  3.0 unx     2842 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-chaos.js
--rw-r--r--  3.0 unx     3640 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-keybinding_menu.js
--rw-r--r--  3.0 unx     5959 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-mips_assembler.js
--rw-r--r--  3.0 unx     6554 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-makefile.js
--rw-r--r--  3.0 unx     2236 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-merbivore.js
--rw-r--r--  3.0 unx     8367 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-prolog.js
--rw-r--r--  3.0 unx     4104 bx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-c9search.js
--rw-r--r--  3.0 unx     2448 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-merbivore_soft.js
--rw-r--r--  3.0 unx     6520 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-scad.js
--rw-r--r--  3.0 unx    20510 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-tsx.js
--rw-r--r--  3.0 unx     2087 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-textile.js
--rw-r--r--  3.0 unx     3687 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-snippets.js
--rw-r--r--  3.0 unx     2248 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-idle_fingers.js
--rw-r--r--  3.0 unx     8028 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-clojure.js
--rw-r--r--  3.0 unx     2761 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-tex.js
--rw-r--r--  3.0 unx     6211 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-bro.js
--rw-r--r--  3.0 unx      506 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-plain_text.js
--rw-r--r--  3.0 unx     7416 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-coffee.js
--rw-r--r--  3.0 unx     1173 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-lucene.js
--rw-r--r--  3.0 unx    59262 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-django.js
--rw-r--r--  3.0 unx     3729 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-modelist.js
--rw-r--r--  3.0 unx     3221 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-tomorrow_night_eighties.js
--rw-r--r--  3.0 unx    20567 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-matlab.js
--rw-r--r--  3.0 unx    26620 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-lsl.js
--rw-r--r--  3.0 unx     3496 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-tomorrow_night_bright.js
--rw-r--r--  3.0 unx     4709 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-abc.js
--rw-r--r--  3.0 unx    22440 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-groovy.js
--rw-r--r--  3.0 unx     2499 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-twilight.js
--rw-r--r--  3.0 unx     4193 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-split.js
--rw-r--r--  3.0 unx    64800 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-markdown.js
--rw-r--r--  3.0 unx     4559 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-pascal.js
--rw-r--r--  3.0 unx    20085 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-less.js
--rw-r--r--  3.0 unx     2820 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-tomorrow_night.js
--rw-r--r--  3.0 unx    11837 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-kotlin.js
--rw-r--r--  3.0 unx     2375 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-monokai.js
--rw-r--r--  3.0 unx     7539 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-julia.js
--rw-r--r--  3.0 unx     6913 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-golang.js
--rw-r--r--  3.0 unx     8898 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-assembly_x86.js
--rw-r--r--  3.0 unx     8226 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-dockerfile.js
--rw-r--r--  3.0 unx     2125 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-eclipse.js
--rw-r--r--  3.0 unx     2712 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-chrome.js
--rw-r--r--  3.0 unx    54512 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-objectivec.js
--rw-r--r--  3.0 unx    66385 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-soy_template.js
--rw-r--r--  3.0 unx     3994 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-rdoc.js
--rw-r--r--  3.0 unx     6965 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-jsx.js
--rw-r--r--  3.0 unx     2313 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-cobol.js
--rw-r--r--  3.0 unx     5097 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-json.js
--rw-r--r--  3.0 unx   354781 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ace.js
--rw-r--r--  3.0 unx     2844 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-eiffel.js
--rw-r--r--  3.0 unx    13129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-nix.js
--rw-r--r--  3.0 unx    61356 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-smarty.js
--rw-r--r--  3.0 unx    11847 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-xml.js
--rw-r--r--  3.0 unx    12235 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-stylus.js
--rw-r--r--  3.0 unx      825 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-linking.js
--rw-r--r--  3.0 unx    31988 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-svg.js
--rw-r--r--  3.0 unx    96918 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/keybinding-vim.js
--rw-r--r--  3.0 unx    68741 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-html_ruby.js
--rw-r--r--  3.0 unx     2176 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-github.js
--rw-r--r--  3.0 unx     2240 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-dawn.js
--rw-r--r--  3.0 unx     4881 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-maze.js
--rw-r--r--  3.0 unx     7382 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-perl.js
--rw-r--r--  3.0 unx    14198 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-dart.js
--rw-r--r--  3.0 unx    10005 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-searchbox.js
--rw-r--r--  3.0 unx     5764 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-jack.js
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/swift.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/golang.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/mysql.js
--rw-r--r--  3.0 unx      942 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/sql.js
--rw-r--r--  3.0 unx     4322 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/java.js
--rw-r--r--  3.0 unx      147 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/assembly_x86.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/tsx.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/rdoc.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/rust.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/yaml.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/powershell.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/rhtml.js
--rw-r--r--  3.0 unx      127 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/nsis.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/ini.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/julia.js
--rw-r--r--  3.0 unx      134 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/live_script.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/kotlin.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/haxe.js
--rw-r--r--  3.0 unx      147 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/soy_template.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/scala.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/dot.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/abap.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/scad.js
--rw-r--r--  3.0 unx     1319 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/dart.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/curly.js
--rw-r--r--  3.0 unx     4000 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/django.js
--rw-r--r--  3.0 unx     3840 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/javascript.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/plain_text.js
--rw-r--r--  3.0 unx      551 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/diff.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/groovy.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/lean.js
--rw-r--r--  3.0 unx      137 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/luapage.js
--rw-r--r--  3.0 unx      125 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/d.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/jsx.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/nix.js
--rw-r--r--  3.0 unx     1263 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/wollok.js
--rw-r--r--  3.0 unx     1973 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/markdown.js
--rw-r--r--  3.0 unx      145 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/html_elixir.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/elixir.js
--rw-r--r--  3.0 unx     2055 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/sh.js
--rw-r--r--  3.0 unx     3636 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/tex.js
--rw-r--r--  3.0 unx    35423 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/lsl.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/ejs.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/swig.js
--rw-r--r--  3.0 unx     1975 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/haskell.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/latex.js
--rw-r--r--  3.0 unx      136 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/mipsassembler.js
--rw-r--r--  3.0 unx    18271 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/html.js
--rw-r--r--  3.0 unx     1716 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/jsoniq.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/sass.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/properties.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/csharp.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/prolog.js
--rw-r--r--  3.0 unx     3574 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/erlang.js
--rw-r--r--  3.0 unx     3672 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/python.js
--rw-r--r--  3.0 unx      164 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/razor.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/pascal.js
--rw-r--r--  3.0 unx      137 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/verilog.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/text.js
--rw-r--r--  3.0 unx     6763 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/php.js
--rw-r--r--  3.0 unx      126 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/bro.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/typescript.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/json.js
--rw-r--r--  3.0 unx    19650 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/css.js
--rw-r--r--  3.0 unx      370 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/drools.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/logiql.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/dockerfile.js
--rw-r--r--  3.0 unx      137 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/gherkin.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/cobol.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/xml.js
--rw-r--r--  3.0 unx      270 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/maze.js
--rw-r--r--  3.0 unx     2778 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/jsp.js
--rw-r--r--  3.0 unx      149 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/haskell_cabal.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/elm.js
--rw-r--r--  3.0 unx      139 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/asciidoc.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/pgsql.js
--rw-r--r--  3.0 unx      132 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/protobuf.js
--rw-r--r--  3.0 unx      141 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/batchfile.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/coldfusion.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/ada.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/praat.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/liquid.js
--rw-r--r--  3.0 unx      947 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/abc.js
--rw-r--r--  3.0 unx    21279 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/ruby.js
--rw-r--r--  3.0 unx      508 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/lua.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/sjs.js
--rw-r--r--  3.0 unx      442 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/rst.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/vhdl.js
--rw-r--r--  3.0 unx     3127 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/vala.js
--rw-r--r--  3.0 unx     2040 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/clojure.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/smarty.js
--rw-r--r--  3.0 unx      145 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/apache_conf.js
--rw-r--r--  3.0 unx     1219 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/io.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/less.js
--rw-r--r--  3.0 unx      540 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/textile.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/handlebars.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/space.js
--rw-r--r--  3.0 unx      137 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/fortran.js
--rw-r--r--  3.0 unx      198 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/makefile.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/scss.js
--rw-r--r--  3.0 unx      297 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/snippets.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/lisp.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/cirru.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/twig.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/eiffel.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/lucene.js
--rw-r--r--  3.0 unx      141 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/gitignore.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/toml.js
--rw-r--r--  3.0 unx      448 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/haml.js
--rw-r--r--  3.0 unx     1690 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/tcl.js
--rw-r--r--  3.0 unx      139 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/c9search.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/livescript.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/mask.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/jack.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/forth.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/ocaml.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/jade.js
--rw-r--r--  3.0 unx      141 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/html_ruby.js
--rw-r--r--  3.0 unx      128 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/hjson.js
--rw-r--r--  3.0 unx      131 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/glsl.js
--rw-r--r--  3.0 unx      651 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/velocity.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/mel.js
--rw-r--r--  3.0 unx      145 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/applescript.js
--rw-r--r--  3.0 unx      151 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/mips_assembler.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/stylus.js
--rw-r--r--  3.0 unx     2663 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/c_cpp.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/svg.js
--rw-r--r--  3.0 unx     5513 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/perl.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/objectivec.js
--rw-r--r--  3.0 unx      607 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/gobstones.js
--rw-r--r--  3.0 unx      139 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/vbscript.js
--rw-r--r--  3.0 unx      129 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/ftl.js
--rw-r--r--  3.0 unx      143 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/autohotkey.js
--rw-r--r--  3.0 unx     2233 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/coffee.js
--rw-r--r--  3.0 unx     2973 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/actionscript.js
--rw-r--r--  3.0 unx      133 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/gcode.js
--rw-r--r--  3.0 unx     1716 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/xquery.js
--rw-r--r--  3.0 unx      139 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/mushcode.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/matlab.js
--rw-r--r--  3.0 unx     2139 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/sqlserver.js
--rw-r--r--  3.0 unx      135 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/scheme.js
--rw-r--r--  3.0 unx     2630 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/snippets/r.js
--rw-r--r--  3.0 unx     2409 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-diff.js
--rw-r--r--  3.0 unx    12546 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-protobuf.js
--rw-r--r--  3.0 unx    24939 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-mel.js
--rw-r--r--  3.0 unx     2054 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-kuroir.js
--rw-r--r--  3.0 unx    20332 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-gobstones.js
--rw-r--r--  3.0 unx    10260 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-praat.js
--rw-r--r--  3.0 unx     3189 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-mipsassembler.js
--rw-r--r--  3.0 unx    27779 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-ambiance.js
--rw-r--r--  3.0 unx    24465 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/keybinding-emacs.js
--rw-r--r--  3.0 unx     3658 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-scheme.js
--rw-r--r--  3.0 unx     3024 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-rst.js
--rw-r--r--  3.0 unx     1762 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-ada.js
--rw-r--r--  3.0 unx     2088 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-vhdl.js
--rw-r--r--  3.0 unx     3031 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-tomorrow_night_blue.js
--rw-r--r--  3.0 unx     7189 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-sh.js
--rw-r--r--  3.0 unx   164518 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-javascript.js
--rw-r--r--  3.0 unx     3138 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-dreamweaver.js
--rw-r--r--  3.0 unx    37225 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-haml.js
--rw-r--r--  3.0 unx     5665 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-io.js
--rw-r--r--  3.0 unx     6929 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-swift.js
--rw-r--r--  3.0 unx     1918 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-xcode.js
--rw-r--r--  3.0 unx     2204 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-toml.js
--rw-r--r--  3.0 unx    10220 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-sass.js
--rw-r--r--  3.0 unx     3874 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-latex.js
--rw-r--r--  3.0 unx    13008 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-glsl.js
--rw-r--r--  3.0 unx     5576 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-lean.js
--rw-r--r--  3.0 unx    18060 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-javascript.js
--rw-r--r--  3.0 unx     6360 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-chromevox.js
--rw-r--r--  3.0 unx     6476 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-iplastic.js
--rw-r--r--  3.0 unx    61525 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-twig.js
--rw-r--r--  3.0 unx    21478 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-emmet.js
--rw-r--r--  3.0 unx     5813 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-abap.js
--rw-r--r--  3.0 unx     5005 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-r.js
--rw-r--r--  3.0 unx     5970 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-hjson.js
--rw-r--r--  3.0 unx     1464 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-gcode.js
--rw-r--r--  3.0 unx   230322 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-xquery.js
--rw-r--r--  3.0 unx     7283 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-lua.js
--rw-r--r--  3.0 unx     2913 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-terminal.js
--rw-r--r--  3.0 unx    59769 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-handlebars.js
--rw-r--r--  3.0 unx    78297 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/worker-php.js
--rw-r--r--  3.0 unx    62630 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-velocity.js
--rw-r--r--  3.0 unx     3003 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-cirru.js
--rw-r--r--  3.0 unx    12293 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-settings_menu.js
--rw-r--r--  3.0 unx    32692 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-powershell.js
--rw-r--r--  3.0 unx    66336 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-luapage.js
--rw-r--r--  3.0 unx     2556 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-tomorrow.js
--rw-r--r--  3.0 unx     2282 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-haskell_cabal.js
--rw-r--r--  3.0 unx     1088 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-statusbar.js
--rw-r--r--  3.0 unx     2689 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-verilog.js
--rw-r--r--  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/js/ace/mode-text.js
--rw-r--r--  3.0 unx     7595 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-dot.js
--rw-r--r--  3.0 unx    34689 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-jsp.js
--rw-r--r--  3.0 unx     2432 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/theme-clouds_midnight.js
--rw-r--r--  3.0 unx      140 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/ext-error_marker.js
--rw-r--r--  3.0 unx     1961 tx defN 23-Jan-12 14:39 _dashboard/static/js/ace/mode-lisp.js
--rw-r--r--  3.0 unx    12132 tx defN 23-Jan-12 14:39 _dashboard/static/js/axios.min.js
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/static/components/
--rw-r--r--  3.0 unx     7012 tx defN 23-Jan-12 14:39 _dashboard/static/components/mtable.js
--rw-r--r--  3.0 unx     6369 tx defN 23-Jan-12 14:39 _dashboard/static/components/mtable.html
--rw-r--r--  3.0 unx    14452 tx defN 23-Jan-12 14:39 _dashboard/__init__.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 _dashboard/templates/
--rw-r--r--  3.0 unx      993 tx defN 23-Jan-12 14:39 _dashboard/templates/dbadmin.html
--rw-r--r--  3.0 unx    11021 tx defN 23-Jan-12 14:39 _dashboard/templates/index.html
--rw-r--r--  3.0 unx     1924 tx defN 23-Jan-12 14:39 _dashboard/templates/gitlog.html
--rw-r--r--  3.0 unx     1141 tx defN 23-Jan-12 14:39 _dashboard/templates/ticket.html
--rw-r--r--  3.0 unx      277 tx defN 23-Jan-12 14:39 app.py
--rw-r--r--  3.0 unx        0 bx stor 23-Jan-12 14:39 __init__.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/css/
+-rw-r--r--  3.0 unx     5742 tx defN 23-Jan-15 14:39 _dashboard/static/css/future.css
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/images/
+-rw-r--r--  3.0 unx    13366 bx defN 23-Jan-15 14:39 _dashboard/static/images/alert-orange.gif
+-rw-r--r--  3.0 unx    12305 bx defN 23-Jan-15 14:39 _dashboard/static/images/alert-blue.gif
+-rw-r--r--  3.0 unx  1010153 bx defN 23-Jan-15 14:39 _dashboard/static/images/widget.gif
+-rw-r--r--  3.0 unx    12025 bx defN 23-Jan-15 14:39 _dashboard/static/images/alert-red.gif
+-rw-r--r--  3.0 unx    13380 bx defN 23-Jan-15 14:39 _dashboard/static/images/alert-yellow.gif
+-rw-r--r--  3.0 unx     7927 bx defN 23-Jan-15 14:39 _dashboard/static/images/forkme.png
+-rw-r--r--  3.0 unx    11068 bx defN 23-Jan-15 14:39 _dashboard/static/images/alert-green.gif
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/js/
+-rw-r--r--  3.0 unx      405 tx defN 23-Jan-15 14:39 _dashboard/static/js/dbadmin.js
+-rw-r--r--  3.0 unx    68547 tx defN 23-Jan-15 14:39 _dashboard/static/js/sugar.min.js
+-rw-r--r--  3.0 unx     4963 tx defN 23-Jan-15 14:39 _dashboard/static/js/utils.js
+-rw-r--r--  3.0 unx    76004 tx defN 23-Jan-15 14:39 _dashboard/static/js/vue.min.js
+-rw-r--r--  3.0 unx    88145 tx defN 23-Jan-15 14:39 _dashboard/static/js/jquery.min.js
+-rw-r--r--  3.0 unx     9231 tx defN 23-Jan-15 14:39 _dashboard/static/js/index.js
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/js/ace/
+-rw-r--r--  3.0 unx     2353 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-cobalt.js
+-rw-r--r--  3.0 unx     2380 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-gherkin.js
+-rw-r--r--  3.0 unx    30624 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-ftl.js
+-rw-r--r--  3.0 unx    11468 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-haskell.js
+-rw-r--r--  3.0 unx    16415 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-sqlserver.js
+-rw-r--r--  3.0 unx     2585 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-textmate.js
+-rw-r--r--  3.0 unx     2791 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-mono_industrial.js
+-rw-r--r--  3.0 unx    62955 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-rhtml.js
+-rw-r--r--  3.0 unx    64984 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-razor.js
+-rw-r--r--  3.0 unx     8159 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-asciidoc.js
+-rw-r--r--  3.0 unx    30271 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-liquid.js
+-rw-r--r--  3.0 unx     5073 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-vbscript.js
+-rw-r--r--  3.0 unx     2633 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-pastel_on_dark.js
+-rw-r--r--  3.0 unx     1440 bx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-spellcheck.js
+-rw-r--r--  3.0 unx    58909 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-curly.js
+-rw-r--r--  3.0 unx    55911 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-pgsql.js
+-rw-r--r--  3.0 unx  1177601 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-xquery.js
+-rw-r--r--  3.0 unx     6523 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-mysql.js
+-rw-r--r--  3.0 unx   217401 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-html.js
+-rw-r--r--  3.0 unx     1099 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-properties.js
+-rw-r--r--  3.0 unx     6120 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-tcl.js
+-rw-r--r--  3.0 unx     8840 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-csharp.js
+-rw-r--r--  3.0 unx     4984 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-livescript.js
+-rw-r--r--  3.0 unx     4681 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-python.js
+-rw-r--r--  3.0 unx     2892 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-sqlserver.js
+-rw-r--r--  3.0 unx     9112 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-textarea.js
+-rw-r--r--  3.0 unx     2312 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-solarized_dark.js
+-rw-r--r--  3.0 unx     2360 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-solarized_light.js
+-rw-r--r--  3.0 unx     2236 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-space.js
+-rw-r--r--  3.0 unx   190654 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-coffee.js
+-rw-r--r--  3.0 unx     2572 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-whitespace.js
+-rw-r--r--  3.0 unx      899 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-gitignore.js
+-rw-r--r--  3.0 unx     8947 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-d.js
+-rw-r--r--  3.0 unx    15600 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-ocaml.js
+-rw-r--r--  3.0 unx    63640 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-autohotkey.js
+-rw-r--r--  3.0 unx    16578 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-vala.js
+-rw-r--r--  3.0 unx    10035 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-nsis.js
+-rw-r--r--  3.0 unx     3126 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-katzenmilch.js
+-rw-r--r--  3.0 unx     4856 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-batchfile.js
+-rw-r--r--  3.0 unx     2296 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-kr_theme.js
+-rw-r--r--  3.0 unx     6540 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-haxe.js
+-rw-r--r--  3.0 unx     1811 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-sql.js
+-rw-r--r--  3.0 unx    11914 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-old_ie.js
+-rw-r--r--  3.0 unx    55541 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-xml.js
+-rw-r--r--  3.0 unx   470435 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-php.js
+-rw-r--r--  3.0 unx     2819 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-static_highlight.js
+-rw-r--r--  3.0 unx    20198 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-typescript.js
+-rw-r--r--  3.0 unx    21805 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-java.js
+-rw-r--r--  3.0 unx    34464 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-language_tools.js
+-rw-r--r--  3.0 unx     3994 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-yaml.js
+-rw-r--r--  3.0 unx    12951 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-scss.js
+-rw-r--r--  3.0 unx    10025 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-ruby.js
+-rw-r--r--  3.0 unx     6989 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-forth.js
+-rw-r--r--  3.0 unx    19962 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-live_script.js
+-rw-r--r--  3.0 unx    29711 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-erlang.js
+-rw-r--r--  3.0 unx    18046 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-css.js
+-rw-r--r--  3.0 unx    57890 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-html.js
+-rw-r--r--  3.0 unx    47114 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-lua.js
+-rw-r--r--  3.0 unx    15753 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-elixir.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-vibrant_ink.js
+-rw-r--r--  3.0 unx   232939 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-jsoniq.js
+-rw-r--r--  3.0 unx     3818 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-beautify.js
+-rw-r--r--  3.0 unx    68412 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-ejs.js
+-rw-r--r--  3.0 unx     5712 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-logiql.js
+-rw-r--r--  3.0 unx     8428 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-fortran.js
+-rw-r--r--  3.0 unx    21273 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-sjs.js
+-rw-r--r--  3.0 unx    75093 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-html_elixir.js
+-rw-r--r--  3.0 unx    20269 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-wollok.js
+-rw-r--r--  3.0 unx    20545 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-actionscript.js
+-rw-r--r--  3.0 unx    49991 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-jade.js
+-rw-r--r--  3.0 unx     2710 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-ini.js
+-rw-r--r--  3.0 unx     6712 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-mushcode.js
+-rw-r--r--  3.0 unx    60415 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-coldfusion.js
+-rw-r--r--  3.0 unx     4933 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-elm.js
+-rw-r--r--  3.0 unx     5399 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-applescript.js
+-rw-r--r--  3.0 unx     1470 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-themelist.js
+-rw-r--r--  3.0 unx    10840 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-c_cpp.js
+-rw-r--r--  3.0 unx     3840 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-elastic_tabstops_lite.js
+-rw-r--r--  3.0 unx    13909 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-apache_conf.js
+-rw-r--r--  3.0 unx     2812 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-crimson_editor.js
+-rw-r--r--  3.0 unx   140879 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-css.js
+-rw-r--r--  3.0 unx    10785 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-drools.js
+-rw-r--r--  3.0 unx    40358 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-mask.js
+-rw-r--r--  3.0 unx    31151 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-swig.js
+-rw-r--r--  3.0 unx     2081 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-clouds.js
+-rw-r--r--  3.0 unx    22619 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-scala.js
+-rw-r--r--  3.0 unx    32911 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-json.js
+-rw-r--r--  3.0 unx     6495 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-rust.js
+-rw-r--r--  3.0 unx     2842 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-chaos.js
+-rw-r--r--  3.0 unx     3640 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-keybinding_menu.js
+-rw-r--r--  3.0 unx     5959 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-mips_assembler.js
+-rw-r--r--  3.0 unx     6554 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-makefile.js
+-rw-r--r--  3.0 unx     2236 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-merbivore.js
+-rw-r--r--  3.0 unx     8367 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-prolog.js
+-rw-r--r--  3.0 unx     4104 bx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-c9search.js
+-rw-r--r--  3.0 unx     2448 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-merbivore_soft.js
+-rw-r--r--  3.0 unx     6520 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-scad.js
+-rw-r--r--  3.0 unx    20510 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-tsx.js
+-rw-r--r--  3.0 unx     2087 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-textile.js
+-rw-r--r--  3.0 unx     3687 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-snippets.js
+-rw-r--r--  3.0 unx     2248 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-idle_fingers.js
+-rw-r--r--  3.0 unx     8028 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-clojure.js
+-rw-r--r--  3.0 unx     2761 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-tex.js
+-rw-r--r--  3.0 unx     6211 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-bro.js
+-rw-r--r--  3.0 unx      506 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-plain_text.js
+-rw-r--r--  3.0 unx     7416 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-coffee.js
+-rw-r--r--  3.0 unx     1173 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-lucene.js
+-rw-r--r--  3.0 unx    59262 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-django.js
+-rw-r--r--  3.0 unx     3729 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-modelist.js
+-rw-r--r--  3.0 unx     3221 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-tomorrow_night_eighties.js
+-rw-r--r--  3.0 unx    20567 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-matlab.js
+-rw-r--r--  3.0 unx    26620 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-lsl.js
+-rw-r--r--  3.0 unx     3496 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-tomorrow_night_bright.js
+-rw-r--r--  3.0 unx     4709 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-abc.js
+-rw-r--r--  3.0 unx    22440 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-groovy.js
+-rw-r--r--  3.0 unx     2499 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-twilight.js
+-rw-r--r--  3.0 unx     4193 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-split.js
+-rw-r--r--  3.0 unx    64800 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-markdown.js
+-rw-r--r--  3.0 unx     4559 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-pascal.js
+-rw-r--r--  3.0 unx    20085 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-less.js
+-rw-r--r--  3.0 unx     2820 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-tomorrow_night.js
+-rw-r--r--  3.0 unx    11837 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-kotlin.js
+-rw-r--r--  3.0 unx     2375 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-monokai.js
+-rw-r--r--  3.0 unx     7539 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-julia.js
+-rw-r--r--  3.0 unx     6913 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-golang.js
+-rw-r--r--  3.0 unx     8898 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-assembly_x86.js
+-rw-r--r--  3.0 unx     8226 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-dockerfile.js
+-rw-r--r--  3.0 unx     2125 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-eclipse.js
+-rw-r--r--  3.0 unx     2712 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-chrome.js
+-rw-r--r--  3.0 unx    54512 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-objectivec.js
+-rw-r--r--  3.0 unx    66385 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-soy_template.js
+-rw-r--r--  3.0 unx     3994 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-rdoc.js
+-rw-r--r--  3.0 unx     6965 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-jsx.js
+-rw-r--r--  3.0 unx     2313 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-cobol.js
+-rw-r--r--  3.0 unx     5097 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-json.js
+-rw-r--r--  3.0 unx   354781 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ace.js
+-rw-r--r--  3.0 unx     2844 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-eiffel.js
+-rw-r--r--  3.0 unx    13129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-nix.js
+-rw-r--r--  3.0 unx    61356 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-smarty.js
+-rw-r--r--  3.0 unx    11847 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-xml.js
+-rw-r--r--  3.0 unx    12235 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-stylus.js
+-rw-r--r--  3.0 unx      825 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-linking.js
+-rw-r--r--  3.0 unx    31988 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-svg.js
+-rw-r--r--  3.0 unx    96918 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/keybinding-vim.js
+-rw-r--r--  3.0 unx    68741 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-html_ruby.js
+-rw-r--r--  3.0 unx     2176 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-github.js
+-rw-r--r--  3.0 unx     2240 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-dawn.js
+-rw-r--r--  3.0 unx     4881 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-maze.js
+-rw-r--r--  3.0 unx     7382 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-perl.js
+-rw-r--r--  3.0 unx    14198 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-dart.js
+-rw-r--r--  3.0 unx    10005 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-searchbox.js
+-rw-r--r--  3.0 unx     5764 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-jack.js
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/swift.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/golang.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/mysql.js
+-rw-r--r--  3.0 unx      942 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/sql.js
+-rw-r--r--  3.0 unx     4322 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/java.js
+-rw-r--r--  3.0 unx      147 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/assembly_x86.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/tsx.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/rdoc.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/rust.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/yaml.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/powershell.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/rhtml.js
+-rw-r--r--  3.0 unx      127 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/nsis.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/ini.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/julia.js
+-rw-r--r--  3.0 unx      134 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/live_script.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/kotlin.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/haxe.js
+-rw-r--r--  3.0 unx      147 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/soy_template.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/scala.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/dot.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/abap.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/scad.js
+-rw-r--r--  3.0 unx     1319 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/dart.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/curly.js
+-rw-r--r--  3.0 unx     4000 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/django.js
+-rw-r--r--  3.0 unx     3840 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/javascript.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/plain_text.js
+-rw-r--r--  3.0 unx      551 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/diff.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/groovy.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/lean.js
+-rw-r--r--  3.0 unx      137 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/luapage.js
+-rw-r--r--  3.0 unx      125 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/d.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/jsx.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/nix.js
+-rw-r--r--  3.0 unx     1263 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/wollok.js
+-rw-r--r--  3.0 unx     1973 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/markdown.js
+-rw-r--r--  3.0 unx      145 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/html_elixir.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/elixir.js
+-rw-r--r--  3.0 unx     2055 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/sh.js
+-rw-r--r--  3.0 unx     3636 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/tex.js
+-rw-r--r--  3.0 unx    35423 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/lsl.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/ejs.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/swig.js
+-rw-r--r--  3.0 unx     1975 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/haskell.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/latex.js
+-rw-r--r--  3.0 unx      136 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/mipsassembler.js
+-rw-r--r--  3.0 unx    18271 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/html.js
+-rw-r--r--  3.0 unx     1716 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/jsoniq.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/sass.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/properties.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/csharp.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/prolog.js
+-rw-r--r--  3.0 unx     3574 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/erlang.js
+-rw-r--r--  3.0 unx     3672 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/python.js
+-rw-r--r--  3.0 unx      164 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/razor.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/pascal.js
+-rw-r--r--  3.0 unx      137 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/verilog.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/text.js
+-rw-r--r--  3.0 unx     6763 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/php.js
+-rw-r--r--  3.0 unx      126 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/bro.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/typescript.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/json.js
+-rw-r--r--  3.0 unx    19650 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/css.js
+-rw-r--r--  3.0 unx      370 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/drools.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/logiql.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/dockerfile.js
+-rw-r--r--  3.0 unx      137 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/gherkin.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/cobol.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/xml.js
+-rw-r--r--  3.0 unx      270 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/maze.js
+-rw-r--r--  3.0 unx     2778 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/jsp.js
+-rw-r--r--  3.0 unx      149 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/haskell_cabal.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/elm.js
+-rw-r--r--  3.0 unx      139 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/asciidoc.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/pgsql.js
+-rw-r--r--  3.0 unx      132 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/protobuf.js
+-rw-r--r--  3.0 unx      141 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/batchfile.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/coldfusion.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/ada.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/praat.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/liquid.js
+-rw-r--r--  3.0 unx      947 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/abc.js
+-rw-r--r--  3.0 unx    21279 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/ruby.js
+-rw-r--r--  3.0 unx      508 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/lua.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/sjs.js
+-rw-r--r--  3.0 unx      442 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/rst.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/vhdl.js
+-rw-r--r--  3.0 unx     3127 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/vala.js
+-rw-r--r--  3.0 unx     2040 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/clojure.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/smarty.js
+-rw-r--r--  3.0 unx      145 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/apache_conf.js
+-rw-r--r--  3.0 unx     1219 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/io.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/less.js
+-rw-r--r--  3.0 unx      540 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/textile.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/handlebars.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/space.js
+-rw-r--r--  3.0 unx      137 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/fortran.js
+-rw-r--r--  3.0 unx      198 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/makefile.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/scss.js
+-rw-r--r--  3.0 unx      297 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/snippets.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/lisp.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/cirru.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/twig.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/eiffel.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/lucene.js
+-rw-r--r--  3.0 unx      141 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/gitignore.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/toml.js
+-rw-r--r--  3.0 unx      448 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/haml.js
+-rw-r--r--  3.0 unx     1690 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/tcl.js
+-rw-r--r--  3.0 unx      139 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/c9search.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/livescript.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/mask.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/jack.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/forth.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/ocaml.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/jade.js
+-rw-r--r--  3.0 unx      141 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/html_ruby.js
+-rw-r--r--  3.0 unx      128 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/hjson.js
+-rw-r--r--  3.0 unx      131 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/glsl.js
+-rw-r--r--  3.0 unx      651 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/velocity.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/mel.js
+-rw-r--r--  3.0 unx      145 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/applescript.js
+-rw-r--r--  3.0 unx      151 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/mips_assembler.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/stylus.js
+-rw-r--r--  3.0 unx     2663 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/c_cpp.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/svg.js
+-rw-r--r--  3.0 unx     5513 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/perl.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/objectivec.js
+-rw-r--r--  3.0 unx      607 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/gobstones.js
+-rw-r--r--  3.0 unx      139 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/vbscript.js
+-rw-r--r--  3.0 unx      129 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/ftl.js
+-rw-r--r--  3.0 unx      143 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/autohotkey.js
+-rw-r--r--  3.0 unx     2233 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/coffee.js
+-rw-r--r--  3.0 unx     2973 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/actionscript.js
+-rw-r--r--  3.0 unx      133 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/gcode.js
+-rw-r--r--  3.0 unx     1716 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/xquery.js
+-rw-r--r--  3.0 unx      139 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/mushcode.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/matlab.js
+-rw-r--r--  3.0 unx     2139 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/sqlserver.js
+-rw-r--r--  3.0 unx      135 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/scheme.js
+-rw-r--r--  3.0 unx     2630 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/snippets/r.js
+-rw-r--r--  3.0 unx     2409 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-diff.js
+-rw-r--r--  3.0 unx    12546 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-protobuf.js
+-rw-r--r--  3.0 unx    24939 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-mel.js
+-rw-r--r--  3.0 unx     2054 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-kuroir.js
+-rw-r--r--  3.0 unx    20332 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-gobstones.js
+-rw-r--r--  3.0 unx    10260 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-praat.js
+-rw-r--r--  3.0 unx     3189 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-mipsassembler.js
+-rw-r--r--  3.0 unx    27779 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-ambiance.js
+-rw-r--r--  3.0 unx    24465 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/keybinding-emacs.js
+-rw-r--r--  3.0 unx     3658 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-scheme.js
+-rw-r--r--  3.0 unx     3024 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-rst.js
+-rw-r--r--  3.0 unx     1762 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-ada.js
+-rw-r--r--  3.0 unx     2088 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-vhdl.js
+-rw-r--r--  3.0 unx     3031 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-tomorrow_night_blue.js
+-rw-r--r--  3.0 unx     7189 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-sh.js
+-rw-r--r--  3.0 unx   164518 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-javascript.js
+-rw-r--r--  3.0 unx     3138 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-dreamweaver.js
+-rw-r--r--  3.0 unx    37225 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-haml.js
+-rw-r--r--  3.0 unx     5665 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-io.js
+-rw-r--r--  3.0 unx     6929 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-swift.js
+-rw-r--r--  3.0 unx     1918 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-xcode.js
+-rw-r--r--  3.0 unx     2204 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-toml.js
+-rw-r--r--  3.0 unx    10220 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-sass.js
+-rw-r--r--  3.0 unx     3874 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-latex.js
+-rw-r--r--  3.0 unx    13008 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-glsl.js
+-rw-r--r--  3.0 unx     5576 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-lean.js
+-rw-r--r--  3.0 unx    18060 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-javascript.js
+-rw-r--r--  3.0 unx     6360 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-chromevox.js
+-rw-r--r--  3.0 unx     6476 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-iplastic.js
+-rw-r--r--  3.0 unx    61525 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-twig.js
+-rw-r--r--  3.0 unx    21478 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-emmet.js
+-rw-r--r--  3.0 unx     5813 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-abap.js
+-rw-r--r--  3.0 unx     5005 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-r.js
+-rw-r--r--  3.0 unx     5970 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-hjson.js
+-rw-r--r--  3.0 unx     1464 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-gcode.js
+-rw-r--r--  3.0 unx   230322 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-xquery.js
+-rw-r--r--  3.0 unx     7283 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-lua.js
+-rw-r--r--  3.0 unx     2913 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-terminal.js
+-rw-r--r--  3.0 unx    59769 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-handlebars.js
+-rw-r--r--  3.0 unx    78297 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/worker-php.js
+-rw-r--r--  3.0 unx    62630 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-velocity.js
+-rw-r--r--  3.0 unx     3003 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-cirru.js
+-rw-r--r--  3.0 unx    12293 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-settings_menu.js
+-rw-r--r--  3.0 unx    32692 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-powershell.js
+-rw-r--r--  3.0 unx    66336 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-luapage.js
+-rw-r--r--  3.0 unx     2556 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-tomorrow.js
+-rw-r--r--  3.0 unx     2282 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-haskell_cabal.js
+-rw-r--r--  3.0 unx     1088 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-statusbar.js
+-rw-r--r--  3.0 unx     2689 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-verilog.js
+-rw-r--r--  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/js/ace/mode-text.js
+-rw-r--r--  3.0 unx     7595 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-dot.js
+-rw-r--r--  3.0 unx    34689 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-jsp.js
+-rw-r--r--  3.0 unx     2432 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/theme-clouds_midnight.js
+-rw-r--r--  3.0 unx      140 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/ext-error_marker.js
+-rw-r--r--  3.0 unx     1961 tx defN 23-Jan-15 14:39 _dashboard/static/js/ace/mode-lisp.js
+-rw-r--r--  3.0 unx    12132 tx defN 23-Jan-15 14:39 _dashboard/static/js/axios.min.js
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/static/components/
+-rw-r--r--  3.0 unx     7012 tx defN 23-Jan-15 14:39 _dashboard/static/components/mtable.js
+-rw-r--r--  3.0 unx     6369 tx defN 23-Jan-15 14:39 _dashboard/static/components/mtable.html
+-rw-r--r--  3.0 unx    14452 tx defN 23-Jan-15 14:39 _dashboard/__init__.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 _dashboard/templates/
+-rw-r--r--  3.0 unx      993 tx defN 23-Jan-15 14:39 _dashboard/templates/dbadmin.html
+-rw-r--r--  3.0 unx    11021 tx defN 23-Jan-15 14:39 _dashboard/templates/index.html
+-rw-r--r--  3.0 unx     1924 tx defN 23-Jan-15 14:39 _dashboard/templates/gitlog.html
+-rw-r--r--  3.0 unx     1141 tx defN 23-Jan-15 14:39 _dashboard/templates/ticket.html
+-rw-r--r--  3.0 unx      277 tx defN 23-Jan-15 14:39 app.py
+-rw-r--r--  3.0 unx        0 bx stor 23-Jan-15 14:39 __init__.py
 1024 files, 18409318 bytes uncompressed, 5581195 bytes compressed:  69.7%
```

### Comparing `flexmin-0.3.7/flexmin/assets/scripts.zip` & `flexmin-0.3.9/flexmin/assets/scripts.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,135 +1,135 @@
-Zip file size: 126906 bytes, number of entries: 133
--rwxr-xr--  3.0 unx     3099 tx defN 23-Jan-12 14:39 ssl_details.sh
--rwxr-xr--  3.0 unx     4219 tx defN 23-Jan-12 14:39 postgres_databases.sh
--rwxr-xr--  3.0 unx     2132 tx defN 23-Jan-12 14:39 net_hostname.sh
--rwxr-xr--  3.0 unx     1033 tx defN 23-Jan-12 14:39 ssl_compare.sh
--rwxr-xr--  3.0 unx     1025 tx defN 23-Jan-12 14:39 sys_crontab.sh
--rwxr-xr--  3.0 unx     2253 tx defN 23-Jan-12 14:39 postgres_backup.sh
--rwxr-xr--  3.0 unx     5593 tx defN 23-Jan-12 14:39 django_manage_project.sh
--rwxr-xr--  3.0 unx     3423 tx defN 23-Jan-12 14:39 web2py_apps.sh
--rwxr-xr--  3.0 unx     3278 tx defN 23-Jan-12 14:39 django_project_detail.sh
--rwxr-xr--  3.0 unx     3256 tx defN 23-Jan-12 14:39 rsync_modules.sh
--rwxr-xr--  3.0 unx     2852 tx defN 23-Jan-12 14:39 django_projects.sh
--rwxr-xr--  3.0 unx     1351 tx defN 23-Jan-12 14:39 rsync_config.sh
--rwxr-xr--  3.0 unx     5916 tx defN 23-Jan-12 14:39 nginx_viewconfig.sh
--rwxr-xr--  3.0 unx     3004 tx defN 23-Jan-12 14:39 sys_users.sh
--rwxr-xr--  3.0 unx     1665 tx defN 23-Jan-12 14:39 flexmin_verify.sh
--rwxr-xr--  3.0 unx     5738 tx defN 23-Jan-12 14:39 sys_download.sh
--rwxr-xr--  3.0 unx     2154 tx defN 23-Jan-12 14:39 flexmin_editparameters.py
--rwxr-xr--  3.0 unx      295 tx defN 23-Jan-12 14:39 minidlna_config.sh
--rwxr-xr--  3.0 unx      898 tx defN 23-Jan-12 14:39 ssl_renew.sh
--rwxr-xr--  3.0 unx     1631 tx defN 23-Jan-12 14:39 uwsgi_startup.sh
--rwxr-xr--  3.0 unx     3554 tx defN 23-Jan-12 14:39 fmw_logs.py
--rwxr-xr--  3.0 unx     4185 tx defN 23-Jan-12 14:39 sysd_services.sh
--rwxr-xr--  3.0 unx     1177 tx defN 23-Jan-12 14:39 ssl_import.sh
--rwxr-xr--  3.0 unx     1078 tx defN 23-Jan-12 14:39 uwsgi_editconfig.sh
--rwxr-xr--  3.0 unx     4542 tx defN 23-Jan-12 14:39 nginx_editconfigs.sh
--rwxr-xr--  3.0 unx     1138 tx defN 23-Jan-12 14:39 certbot_config.sh
--rwxr-xr--  3.0 unx     5775 tx defN 23-Jan-12 14:39 certbot_manage.sh
--rwxr-xr--  3.0 unx     3072 tx defN 23-Jan-12 14:39 rsync_users.sh
--rwxr-xr--  3.0 unx      889 tx defN 23-Jan-12 14:39 net_portinfo.sh
--rwxr-xr--  3.0 unx     2322 tx defN 23-Jan-12 14:39 postgres_users.sh
--rwxr-xr--  3.0 unx      269 tx defN 23-Jan-12 14:39 net_viewrouting.sh
--rwxr-xr--  3.0 unx     7743 tx defN 23-Jan-12 14:39 ssh_userconf.sh
--rwxr-xr--  3.0 unx     7301 tx defN 23-Jan-12 14:39 sys_folders.sh
--rwxr-xr--  3.0 unx     1177 tx defN 23-Jan-12 14:39 flexmin_editparams.sh
--rwxr-xr--  3.0 unx     6698 tx defN 23-Jan-12 14:39 web2py_backup.sh
--rwxr-xr--  3.0 unx     1899 tx defN 23-Jan-12 14:39 ssl_selfcert.sh
--rwxr-xr--  3.0 unx     1956 tx defN 23-Jan-12 14:39 sys_general.sh
--rwxr-xr--  3.0 unx     2423 tx defN 23-Jan-12 14:39 flexmin_package.sh
--rwxr-xr--  3.0 unx      676 tx defN 23-Jan-12 14:39 flexmin_listparams.sh
--rwxr-xr--  3.0 unx     1759 tx defN 23-Jan-12 14:39 flexmin_editmenu.py
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 freebsd/
--rwxr-xr--  3.0 unx     2129 tx defN 23-Jan-12 14:39 freebsd/bsd_pkgupgrade.sh
--rwxr-xr--  3.0 unx     5762 tx defN 23-Jan-12 14:39 freebsd/bsd_services.sh
--rwxr-xr--  3.0 unx     1629 tx defN 23-Jan-12 14:39 freebsd/uwsgi_startup.sh
--rwxr-xr--  3.0 unx     1846 tx defN 23-Jan-12 14:39 freebsd/bsd_pkg.sh
--rwxr-xr--  3.0 unx      715 tx defN 23-Jan-12 14:39 freebsd/net_portinfo.sh
--rwxr-xr--  3.0 unx      732 tx defN 23-Jan-12 14:39 freebsd/net_viewrouting.sh
--rwxr-xr--  3.0 unx     1261 tx defN 23-Jan-12 14:39 freebsd/bsd_hostname.sh
--rwxr-xr--  3.0 unx     2694 tx defN 23-Jan-12 14:39 freebsd/bsd_users.sh
--rwxr-xr--  3.0 unx     1426 tx defN 23-Jan-12 14:39 freebsd/bsd_groups.sh
--rwxr-xr--  3.0 unx     2480 tx defN 23-Jan-12 14:39 freebsd/bsd_time.sh
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 freebsd/helpers/
--rwxr-xr--  3.0 unx      729 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_sshd.sh
--rwxr-xr--  3.0 unx      732 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_ntp.sh
--rwxr-xr--  3.0 unx      733 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_nginx.sh
--rwxr-xr--  3.0 unx      729 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_rsyncd.sh
--rwxr-xr--  3.0 unx      897 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_djangod.sh
--rwxr-xr--  3.0 unx      733 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_flexmin.sh
--rwxr-xr--  3.0 unx      891 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_gruntd.sh
--rwxr-xr--  3.0 unx     1337 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_postgresql.sh
--rwxr-xr--  3.0 unx      741 tx defN 23-Jan-12 14:39 freebsd/helpers/bsd_services_uwsgi.sh
--rwxr-xr--  3.0 unx      219 tx defN 23-Jan-12 14:39 freebsd/net_dns.sh
--rwxr-xr--  3.0 unx     7315 tx defN 23-Jan-12 14:39 freebsd/net_editconfig.sh
--rwxr-xr--  3.0 unx      912 tx defN 23-Jan-12 14:39 nginx_logs.sh
--rwxr-xr--  3.0 unx      878 tx defN 23-Jan-12 14:39 postgres_config.sh
--rwxr-xr--  3.0 unx     2969 tx defN 23-Jan-12 14:39 ssh_userkeys.sh
--rwxr-xr--  3.0 unx     3328 tx defN 23-Jan-12 14:39 flexmin_logs.sh
--rwxr-xr--  3.0 unx     3055 tx defN 23-Jan-12 14:39 common.sh
--rwxr-xr--  3.0 unx     5388 tx defN 23-Jan-12 14:39 sys_folderperms.sh
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 redundant/
--rwxr-xr--  3.0 unx     1583 tx defN 23-Jan-12 14:39 redundant/node_npm.sh
--rwxr-xr--  3.0 unx      821 tx defN 23-Jan-12 14:39 redundant/node_grunt.sh
--rwxr-xr--  3.0 unx      827 tx defN 23-Jan-12 14:39 redundant/node_config.sh
--rwxr-xr--  3.0 unx     1665 tx defN 23-Jan-12 14:39 ssh_editconfig.sh
--rwxr-xr--  3.0 unx     4007 tx defN 23-Jan-12 14:39 fmw_backups.py
--rwxr-xr--  3.0 unx      910 tx defN 23-Jan-12 14:39 dnsmasq_info.sh
--rwxr-xr--  3.0 unx      580 tx defN 23-Jan-12 14:39 samba_config.sh
-drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-12 14:39 helpers/
--rwxr-xr--  3.0 unx        2 tx stor 23-Jan-12 14:39 helpers/sysd_services_filters.sh
--rwxr-xr--  3.0 unx     1272 tx defN 23-Jan-12 14:39 helpers/generic_editconfig.sh
--rwxr-xr--  3.0 unx      395 tx defN 23-Jan-12 14:39 helpers/django_check.sh
--rwxr-xr--  3.0 unx      547 tx defN 23-Jan-12 14:39 helpers/uwsgi_check.sh
--rwxr-xr--  3.0 unx     1127 tx defN 23-Jan-12 14:39 helpers/postgres_recreatedb.sh
--rwxr-xr--  3.0 unx      419 tx defN 23-Jan-12 14:39 helpers/certbot_check.sh
--rwxr-xr--  3.0 unx      395 tx defN 23-Jan-12 14:39 helpers/rsync_check.sh
--rwxr-xr--  3.0 unx     3132 tx defN 23-Jan-12 14:39 helpers/certbot_ftp.py
--rwxr-xr--  3.0 unx      729 tx defN 23-Jan-12 14:39 helpers/nginx_configs.sh
--rwxr-xr--  3.0 unx       57 tx defN 23-Jan-12 14:39 helpers/sys_folders_test.sh
--rwxr-xr--  3.0 unx      356 tx defN 23-Jan-12 14:39 helpers/certbot_cleanup.sh
--rwxr-xr--  3.0 unx     1471 tx defN 23-Jan-12 14:39 helpers/net_manager.sh
--rwxr-xr--  3.0 unx     3668 tx defN 23-Jan-12 14:39 helpers/generic_yaml_editconfig.sh
--rwxr-xr--  3.0 unx      442 tx defN 23-Jan-12 14:39 helpers/certbot_auth.sh
--rwxr-xr--  3.0 unx     1179 tx defN 23-Jan-12 14:39 helpers/postgres_check.sh
--rwxr-xr--  3.0 unx      389 tx defN 23-Jan-12 14:39 helpers/hg_check.sh
--rwxr-xr--  3.0 unx      493 tx defN 23-Jan-12 14:39 helpers/raspberry_info.sh
--rwxr-xr--  3.0 unx     1653 tx defN 23-Jan-12 14:39 helpers/folder_set_perms.sh
--rwxr-xr--  3.0 unx     4874 tx defN 23-Jan-12 14:39 helpers/sys_folderperms.sh
--rwxr-xr--  3.0 unx      463 tx defN 23-Jan-12 14:39 helpers/backup_check.sh
--rwxr-xr--  3.0 unx     1607 tx defN 23-Jan-12 14:39 helpers/web2py_appinstall.sh
--rwxr-xr--  3.0 unx     1874 tx defN 23-Jan-12 14:39 helpers/cron.sh
--rwxr-xr--  3.0 unx      575 tx defN 23-Jan-12 14:39 helpers/cert_check.sh
--rwxr-xr--  3.0 unx        2 tx stor 23-Jan-12 14:39 helpers/cpanel.py
--rwxr-xr--  3.0 unx      672 tx defN 23-Jan-12 14:39 helpers/uwsgi_configs.sh
--rwxr-xr--  3.0 unx      918 tx defN 23-Jan-12 14:39 helpers/samba_check.sh
--rwxr-xr--  3.0 unx     8698 tx defN 23-Jan-12 14:39 helpers/generic_viewedit_list.sh
--rwxr-xr--  3.0 unx     2054 tx defN 23-Jan-12 14:39 sys_diskusage.sh
--rwxr-xr--  3.0 unx     1087 tx defN 23-Jan-12 14:39 uwsgi_logs.sh
--rwxr-xr--  3.0 unx     4219 tx defN 23-Jan-12 14:39 web2py_main.sh
--rwxr-xr--  3.0 unx     3966 tx defN 23-Jan-12 14:39 samba_users.sh
--rwxr-xr--  3.0 unx     3739 tx defN 23-Jan-12 14:39 uwsgi_overview.sh
--rwxr-xr--  3.0 unx     3992 tx defN 23-Jan-12 14:39 net_dns.sh
--rwxr-xr--  3.0 unx        1 tx stor 23-Jan-12 14:39 __init__.py
--rwxr-xr--  3.0 unx     6832 tx defN 23-Jan-12 14:39 disk_info.sh
--rwxr-xr--  3.0 unx     8463 tx defN 23-Jan-12 14:39 net_editconfig.sh
--rwxr-xr--  3.0 unx     1166 tx defN 23-Jan-12 14:39 flexmin_editmenus.sh
--rwxr-xr--  3.0 unx     3353 tx defN 23-Jan-12 14:39 backup_batch.sh
--rwxr-xr--  3.0 unx      334 tx defN 23-Jan-12 14:39 lighttp_config.sh
--rw-r--r--  3.0 unx        0 bx stor 23-Jan-12 14:39 pypi_update.log
--rwxr-xr--  3.0 unx     1317 tx defN 23-Jan-12 14:39 netman_editconfig.sh
--rwxr-xr--  3.0 unx     3047 tx defN 23-Jan-12 14:39 rsync_userconf.sh
--rwxr-xr--  3.0 unx     1937 tx defN 23-Jan-12 14:39 postgres_restore.sh
--rwxr-xr--  3.0 unx      616 tx defN 23-Jan-12 14:39 nginx_stats.sh
--rwxr-xr--  3.0 unx     1009 tx defN 23-Jan-12 14:39 flexmin_login.py
--rwxr-xr--  3.0 unx     1485 tx defN 23-Jan-12 14:39 ssl_reqcomplete.sh
--rwxr-xr--  3.0 unx     4524 tx defN 23-Jan-12 14:39 rsync_client.sh
--rwxr-xr--  3.0 unx     4676 tx defN 23-Jan-12 14:39 sys_backups.sh
--rwxr-xr--  3.0 unx     5339 tx defN 23-Jan-12 14:39 dnsmasq_manage.sh
--rwxr-xr--  3.0 unx     1598 tx defN 23-Jan-12 14:39 web2py_handlers.sh
--rwxr-xr--  3.0 unx     1672 tx defN 23-Jan-12 14:39 ssl_keyandreq.sh
--rwxr-xr--  3.0 unx     3369 tx defN 23-Jan-12 14:39 sys_time.sh
--rwxr-xr--  3.0 unx     2707 tx defN 23-Jan-12 14:39 flexmin_batch.py
--rwxr-xr--  3.0 unx     4196 tx defN 23-Jan-12 14:39 nginx_certificates.sh
--rwxr-xr--  3.0 unx     3786 tx defN 23-Jan-12 14:39 py4web_apps.sh
-133 files, 294994 bytes uncompressed, 104586 bytes compressed:  64.5%
+Zip file size: 127070 bytes, number of entries: 133
+-rwxr-xr--  3.0 unx     3099 tx defN 23-Jan-15 14:39 ssl_details.sh
+-rwxr-xr--  3.0 unx     4219 tx defN 23-Jan-15 14:39 postgres_databases.sh
+-rwxr-xr--  3.0 unx     2132 tx defN 23-Jan-15 14:39 net_hostname.sh
+-rwxr-xr--  3.0 unx     1033 tx defN 23-Jan-15 14:39 ssl_compare.sh
+-rwxr-xr--  3.0 unx     1025 tx defN 23-Jan-15 14:39 sys_crontab.sh
+-rwxr-xr--  3.0 unx     2253 tx defN 23-Jan-15 14:39 postgres_backup.sh
+-rwxr-xr--  3.0 unx     5593 tx defN 23-Jan-15 14:39 django_manage_project.sh
+-rwxr-xr--  3.0 unx     3423 tx defN 23-Jan-15 14:39 web2py_apps.sh
+-rwxr-xr--  3.0 unx     3278 tx defN 23-Jan-15 14:39 django_project_detail.sh
+-rwxr-xr--  3.0 unx     3256 tx defN 23-Jan-15 14:39 rsync_modules.sh
+-rwxr-xr--  3.0 unx     2852 tx defN 23-Jan-15 14:39 django_projects.sh
+-rwxr-xr--  3.0 unx     1351 tx defN 23-Jan-15 14:39 rsync_config.sh
+-rwxr-xr--  3.0 unx     5916 tx defN 23-Jan-15 14:39 nginx_viewconfig.sh
+-rwxr-xr--  3.0 unx     3004 tx defN 23-Jan-15 14:39 sys_users.sh
+-rwxr-xr--  3.0 unx     1665 tx defN 23-Jan-15 14:39 flexmin_verify.sh
+-rwxr-xr--  3.0 unx     5738 tx defN 23-Jan-15 14:39 sys_download.sh
+-rwxr-xr--  3.0 unx     2154 tx defN 23-Jan-15 14:39 flexmin_editparameters.py
+-rwxr-xr--  3.0 unx      295 tx defN 23-Jan-15 14:39 minidlna_config.sh
+-rwxr-xr--  3.0 unx      898 tx defN 23-Jan-15 14:39 ssl_renew.sh
+-rwxr-xr--  3.0 unx     1631 tx defN 23-Jan-15 14:39 uwsgi_startup.sh
+-rwxr-xr--  3.0 unx     3554 tx defN 23-Jan-15 14:39 fmw_logs.py
+-rwxr-xr--  3.0 unx     4185 tx defN 23-Jan-15 14:39 sysd_services.sh
+-rwxr-xr--  3.0 unx     1177 tx defN 23-Jan-15 14:39 ssl_import.sh
+-rwxr-xr--  3.0 unx     1078 tx defN 23-Jan-15 14:39 uwsgi_editconfig.sh
+-rwxr-xr--  3.0 unx     4542 tx defN 23-Jan-15 14:39 nginx_editconfigs.sh
+-rwxr-xr--  3.0 unx     1138 tx defN 23-Jan-15 14:39 certbot_config.sh
+-rwxr-xr--  3.0 unx     5775 tx defN 23-Jan-15 14:39 certbot_manage.sh
+-rwxr-xr--  3.0 unx     3072 tx defN 23-Jan-15 14:39 rsync_users.sh
+-rwxr-xr--  3.0 unx      889 tx defN 23-Jan-15 14:39 net_portinfo.sh
+-rwxr-xr--  3.0 unx     2322 tx defN 23-Jan-15 14:39 postgres_users.sh
+-rwxr-xr--  3.0 unx      269 tx defN 23-Jan-15 14:39 net_viewrouting.sh
+-rwxr-xr--  3.0 unx     7743 tx defN 23-Jan-15 14:39 ssh_userconf.sh
+-rwxr-xr--  3.0 unx     7301 tx defN 23-Jan-15 14:39 sys_folders.sh
+-rwxr-xr--  3.0 unx     1177 tx defN 23-Jan-15 14:39 flexmin_editparams.sh
+-rwxr-xr--  3.0 unx     6698 tx defN 23-Jan-15 14:39 web2py_backup.sh
+-rwxr-xr--  3.0 unx     1899 tx defN 23-Jan-15 14:39 ssl_selfcert.sh
+-rwxr-xr--  3.0 unx     1956 tx defN 23-Jan-15 14:39 sys_general.sh
+-rwxr-xr--  3.0 unx     2423 tx defN 23-Jan-15 14:39 flexmin_package.sh
+-rwxr-xr--  3.0 unx      676 tx defN 23-Jan-15 14:39 flexmin_listparams.sh
+-rwxr-xr--  3.0 unx     1759 tx defN 23-Jan-15 14:39 flexmin_editmenu.py
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 freebsd/
+-rwxr-xr--  3.0 unx     2129 tx defN 23-Jan-15 14:39 freebsd/bsd_pkgupgrade.sh
+-rwxr-xr--  3.0 unx     5762 tx defN 23-Jan-15 14:39 freebsd/bsd_services.sh
+-rwxr-xr--  3.0 unx     1629 tx defN 23-Jan-15 14:39 freebsd/uwsgi_startup.sh
+-rwxr-xr--  3.0 unx     1846 tx defN 23-Jan-15 14:39 freebsd/bsd_pkg.sh
+-rwxr-xr--  3.0 unx      715 tx defN 23-Jan-15 14:39 freebsd/net_portinfo.sh
+-rwxr-xr--  3.0 unx      732 tx defN 23-Jan-15 14:39 freebsd/net_viewrouting.sh
+-rwxr-xr--  3.0 unx     1261 tx defN 23-Jan-15 14:39 freebsd/bsd_hostname.sh
+-rwxr-xr--  3.0 unx     2694 tx defN 23-Jan-15 14:39 freebsd/bsd_users.sh
+-rwxr-xr--  3.0 unx     1426 tx defN 23-Jan-15 14:39 freebsd/bsd_groups.sh
+-rwxr-xr--  3.0 unx     2480 tx defN 23-Jan-15 14:39 freebsd/bsd_time.sh
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 freebsd/helpers/
+-rwxr-xr--  3.0 unx      729 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_sshd.sh
+-rwxr-xr--  3.0 unx      732 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_ntp.sh
+-rwxr-xr--  3.0 unx      733 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_nginx.sh
+-rwxr-xr--  3.0 unx      729 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_rsyncd.sh
+-rwxr-xr--  3.0 unx      897 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_djangod.sh
+-rwxr-xr--  3.0 unx      733 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_flexmin.sh
+-rwxr-xr--  3.0 unx      891 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_gruntd.sh
+-rwxr-xr--  3.0 unx     1337 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_postgresql.sh
+-rwxr-xr--  3.0 unx      741 tx defN 23-Jan-15 14:39 freebsd/helpers/bsd_services_uwsgi.sh
+-rwxr-xr--  3.0 unx      219 tx defN 23-Jan-15 14:39 freebsd/net_dns.sh
+-rwxr-xr--  3.0 unx     7315 tx defN 23-Jan-15 14:39 freebsd/net_editconfig.sh
+-rwxr-xr--  3.0 unx      912 tx defN 23-Jan-15 14:39 nginx_logs.sh
+-rwxr-xr--  3.0 unx      878 tx defN 23-Jan-15 14:39 postgres_config.sh
+-rwxr-xr--  3.0 unx     2969 tx defN 23-Jan-15 14:39 ssh_userkeys.sh
+-rwxr-xr--  3.0 unx     3328 tx defN 23-Jan-15 14:39 flexmin_logs.sh
+-rwxr-xr--  3.0 unx     3055 tx defN 23-Jan-15 14:39 common.sh
+-rwxr-xr--  3.0 unx     5388 tx defN 23-Jan-15 14:39 sys_folderperms.sh
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 redundant/
+-rwxr-xr--  3.0 unx     1583 tx defN 23-Jan-15 14:39 redundant/node_npm.sh
+-rwxr-xr--  3.0 unx      821 tx defN 23-Jan-15 14:39 redundant/node_grunt.sh
+-rwxr-xr--  3.0 unx      827 tx defN 23-Jan-15 14:39 redundant/node_config.sh
+-rwxr-xr--  3.0 unx     1665 tx defN 23-Jan-15 14:39 ssh_editconfig.sh
+-rwxr-xr--  3.0 unx     4007 tx defN 23-Jan-15 14:39 fmw_backups.py
+-rwxr-xr--  3.0 unx      910 tx defN 23-Jan-15 14:39 dnsmasq_info.sh
+-rwxr-xr--  3.0 unx      580 tx defN 23-Jan-15 14:39 samba_config.sh
+drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-15 14:39 helpers/
+-rwxr-xr--  3.0 unx        2 tx stor 23-Jan-15 14:39 helpers/sysd_services_filters.sh
+-rwxr-xr--  3.0 unx     1272 tx defN 23-Jan-15 14:39 helpers/generic_editconfig.sh
+-rwxr-xr--  3.0 unx      395 tx defN 23-Jan-15 14:39 helpers/django_check.sh
+-rwxr-xr--  3.0 unx      547 tx defN 23-Jan-15 14:39 helpers/uwsgi_check.sh
+-rwxr-xr--  3.0 unx     1127 tx defN 23-Jan-15 14:39 helpers/postgres_recreatedb.sh
+-rwxr-xr--  3.0 unx      419 tx defN 23-Jan-15 14:39 helpers/certbot_check.sh
+-rwxr-xr--  3.0 unx      395 tx defN 23-Jan-15 14:39 helpers/rsync_check.sh
+-rwxr-xr--  3.0 unx     3132 tx defN 23-Jan-15 14:39 helpers/certbot_ftp.py
+-rwxr-xr--  3.0 unx      729 tx defN 23-Jan-15 14:39 helpers/nginx_configs.sh
+-rwxr-xr--  3.0 unx       57 tx defN 23-Jan-15 14:39 helpers/sys_folders_test.sh
+-rwxr-xr--  3.0 unx      356 tx defN 23-Jan-15 14:39 helpers/certbot_cleanup.sh
+-rwxr-xr--  3.0 unx     1471 tx defN 23-Jan-15 14:39 helpers/net_manager.sh
+-rwxr-xr--  3.0 unx     3668 tx defN 23-Jan-15 14:39 helpers/generic_yaml_editconfig.sh
+-rwxr-xr--  3.0 unx      442 tx defN 23-Jan-15 14:39 helpers/certbot_auth.sh
+-rwxr-xr--  3.0 unx     1179 tx defN 23-Jan-15 14:39 helpers/postgres_check.sh
+-rwxr-xr--  3.0 unx      389 tx defN 23-Jan-15 14:39 helpers/hg_check.sh
+-rwxr-xr--  3.0 unx      493 tx defN 23-Jan-15 14:39 helpers/raspberry_info.sh
+-rwxr-xr--  3.0 unx     1653 tx defN 23-Jan-15 14:39 helpers/folder_set_perms.sh
+-rwxr-xr--  3.0 unx     4874 tx defN 23-Jan-15 14:39 helpers/sys_folderperms.sh
+-rwxr-xr--  3.0 unx      463 tx defN 23-Jan-15 14:39 helpers/backup_check.sh
+-rwxr-xr--  3.0 unx     1607 tx defN 23-Jan-15 14:39 helpers/web2py_appinstall.sh
+-rwxr-xr--  3.0 unx     1874 tx defN 23-Jan-15 14:39 helpers/cron.sh
+-rwxr-xr--  3.0 unx      575 tx defN 23-Jan-15 14:39 helpers/cert_check.sh
+-rwxr-xr--  3.0 unx        2 tx stor 23-Jan-15 14:39 helpers/cpanel.py
+-rwxr-xr--  3.0 unx      672 tx defN 23-Jan-15 14:39 helpers/uwsgi_configs.sh
+-rwxr-xr--  3.0 unx      918 tx defN 23-Jan-15 14:39 helpers/samba_check.sh
+-rwxr-xr--  3.0 unx     8698 tx defN 23-Jan-15 14:39 helpers/generic_viewedit_list.sh
+-rwxr-xr--  3.0 unx     2054 tx defN 23-Jan-15 14:39 sys_diskusage.sh
+-rwxr-xr--  3.0 unx     1087 tx defN 23-Jan-15 14:39 uwsgi_logs.sh
+-rwxr-xr--  3.0 unx     4219 tx defN 23-Jan-15 14:39 web2py_main.sh
+-rwxr-xr--  3.0 unx     3966 tx defN 23-Jan-15 14:39 samba_users.sh
+-rwxr-xr--  3.0 unx     4604 tx defN 23-Jan-15 14:39 uwsgi_overview.sh
+-rwxr-xr--  3.0 unx     3992 tx defN 23-Jan-15 14:39 net_dns.sh
+-rwxr-xr--  3.0 unx        1 tx stor 23-Jan-15 14:39 __init__.py
+-rwxr-xr--  3.0 unx     6832 tx defN 23-Jan-15 14:39 disk_info.sh
+-rwxr-xr--  3.0 unx     8463 tx defN 23-Jan-15 14:39 net_editconfig.sh
+-rwxr-xr--  3.0 unx     1166 tx defN 23-Jan-15 14:39 flexmin_editmenus.sh
+-rwxr-xr--  3.0 unx     3353 tx defN 23-Jan-15 14:39 backup_batch.sh
+-rwxr-xr--  3.0 unx      334 tx defN 23-Jan-15 14:39 lighttp_config.sh
+-rw-r--r--  3.0 unx        0 bx stor 23-Jan-15 14:39 pypi_update.log
+-rwxr-xr--  3.0 unx     1317 tx defN 23-Jan-15 14:39 netman_editconfig.sh
+-rwxr-xr--  3.0 unx     3047 tx defN 23-Jan-15 14:39 rsync_userconf.sh
+-rwxr-xr--  3.0 unx     1937 tx defN 23-Jan-15 14:39 postgres_restore.sh
+-rwxr-xr--  3.0 unx      616 tx defN 23-Jan-15 14:39 nginx_stats.sh
+-rwxr-xr--  3.0 unx     1009 tx defN 23-Jan-15 14:39 flexmin_login.py
+-rwxr-xr--  3.0 unx     1485 tx defN 23-Jan-15 14:39 ssl_reqcomplete.sh
+-rwxr-xr--  3.0 unx     4524 tx defN 23-Jan-15 14:39 rsync_client.sh
+-rwxr-xr--  3.0 unx     4676 tx defN 23-Jan-15 14:39 sys_backups.sh
+-rwxr-xr--  3.0 unx     5339 tx defN 23-Jan-15 14:39 dnsmasq_manage.sh
+-rwxr-xr--  3.0 unx     1598 tx defN 23-Jan-15 14:39 web2py_handlers.sh
+-rwxr-xr--  3.0 unx     1672 tx defN 23-Jan-15 14:39 ssl_keyandreq.sh
+-rwxr-xr--  3.0 unx     3369 tx defN 23-Jan-15 14:39 sys_time.sh
+-rwxr-xr--  3.0 unx     2707 tx defN 23-Jan-15 14:39 flexmin_batch.py
+-rwxr-xr--  3.0 unx     4196 tx defN 23-Jan-15 14:39 nginx_certificates.sh
+-rwxr-xr--  3.0 unx     3786 tx defN 23-Jan-15 14:39 py4web_apps.sh
+133 files, 295859 bytes uncompressed, 104750 bytes compressed:  64.6%
```

#### uwsgi_overview.sh

```diff
@@ -23,15 +23,21 @@
   echo "      header: [Configuration, My Path!0]"
   echo "      delimiter_row: '\n'"
   echo "      delimiter: ';'"
   echo "      actions: per_row"
   echo "      data: |"
   for uc in `find ${FM_UWSGI_ROOT} -mindepth 1 -maxdepth 1 -type f -name "*"`
   do
-    echo "        ${uc/$FM_UWSGI_ROOT\//};;!delete.?view"
+    logfile=$(grep -r "^logto" ${uc} | sed 's/^logto\s*=\s*//')
+    if [ ! -z "${logfile}" ]
+    then
+      echo "        ${uc/$FM_UWSGI_ROOT\//};;!delete.?view.?view_log"
+    else
+      echo "        ${uc/$FM_UWSGI_ROOT\//};;!delete.?view"
+    fi
   done
   
   # -------- Optional Configurations ------------
   if [ "$UWSGI_AVAIL" != "$UWSGI_ENABLED" ]  # using available/enabled pattern
   then
     echo "  - table:"
     echo "      title: Optional Configurations"
@@ -39,33 +45,59 @@
     echo "      second_col: 1"
     echo "      delimiter_row: '\n'"
     echo "      delimiter: ';'"
     echo "      actions: per_row"
     echo "      data: |"
     for uc in `find ${UWSGI_AVAIL} -mindepth 1 -maxdepth 1 -name "*"`
     do
-        #uw_inc=$(grep -vE '^\s*#' ${uc} | grep -o -E 'include[ ]*[^\;]*' | grep -v "_params" | sed 's/include\s*//')
-        if [ -f ${UWSGI_ENABLED}${uc/$UWSGI_AVAIL/} ]
-        then
-        echo "        ${uc/$UWSGI_AVAIL\//};/${UWSGI_AVAIL/$FM_UWSGI_ROOT\//};enabled*green;reload.disable.!delete.?view"
-        else
-        echo "        ${uc/$UWSGI_AVAIL\//};/${UWSGI_AVAIL/$FM_UWSGI_ROOT\//};disabled*red;enable.!delete.?view"
-        fi
+      logfile=$(grep -r "^logto" ${uc} | sed 's/^logto\s*=\s*//')
+      if [ ! -z "${logfile}" ]
+      then
+        actions="!delete.?view.?view_log"
+      else
+        actions="!delete.?view"
+      fi
+      #uw_inc=$(grep -vE '^\s*#' ${uc} | grep -o -E 'include[ ]*[^\;]*' | grep -v "_params" | sed 's/include\s*//')
+      if [ -f ${UWSGI_ENABLED}${uc/$UWSGI_AVAIL/} ]
+      then
+        echo "        ${uc/$UWSGI_AVAIL\//};/${UWSGI_AVAIL/$FM_UWSGI_ROOT\//};enabled*green;reload.disable.${actions}"
+      else
+        echo "        ${uc/$UWSGI_AVAIL\//};/${UWSGI_AVAIL/$FM_UWSGI_ROOT\//};disabled*red;enable.${actions}"
+      fi
     done
   fi
   
   # -------- Scoket Configuration Info ------------
   echo "  - table:"
   echo "      title: uWSGI Socket Configuration"
   echo "      header: [Config File, Socket]"
   echo "      delimiter: ';'"
   echo "      data: |"
   grep -rw -E "^[\t\s]*socket" ${FM_UWSGI_ROOT}/ \
        | sed "s|$FM_UWSGI_ROOT/||" \
        | sed -r 's/\:[\t\s]*socket[ ]*=[ ]*/;/' | sed 's/^/        /'
+       
+elif [ "$2" == "view_log" ]
+then
+  echo "title: View Log (Last 150 lines)"
+  echo "method: popup"
+  echo "---"
+  if [ -f "${FM_UWSGI_ROOT}/${1}" ]
+  then
+    logfile=$(grep -r "^logto" "${FM_UWSGI_ROOT}/${1}" | sed 's/^logto\s*=\s*//')
+  elif [ -f "${UWSGI_AVAIL}/${1}" ]
+  then
+    logfile=$(grep -r "^logto" "${UWSGI_AVAIL}/${1}" | sed 's/^logto\s*=\s*//')
+  fi
+  if [ -r ${logfile} ]
+  then
+      tail -n 150 ${logfile}
+  else
+      echo "ERROR: cannot read ${logfile}"
+  fi   
   
 elif [ "$2" == "enable" ]
 then
   # 1=name 2=enable
   echo "title: Enabling ${1}"
   echo "method: popup"
   echo "next_action: reload_pane"
```

### Comparing `flexmin-0.3.7/flexmin/assets/system.zip` & `flexmin-0.3.9/flexmin/assets/system.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 7669 bytes, number of entries: 12
 -rw-r--r--  3.0 unx      230 tx defN 20-Dec-20 16:34 py4web.ini
 -rw-r--r--  3.0 unx     1006 tx defN 20-Dec-20 16:34 setup_prereq_checks.sh
 -rw-r--r--  3.0 unx      113 tx defN 20-Dec-20 16:34 flexmin.service.debian
--rw-r--r--  3.0 unx      107 tx defN 23-Jan-12 14:40 flexmin.service
+-rw-r--r--  3.0 unx      107 tx defN 23-Jan-15 14:40 flexmin.service
 -rw-r--r--  3.0 unx       77 tx defN 20-Dec-20 16:34 py4web_pw.sh
 -rw-r--r--  3.0 unx      513 tx defN 20-Dec-20 16:34 setup_pathcheck.sh
 -rw-r--r--  3.0 unx       73 tx defN 20-Dec-20 16:34 emperor.ini
 -rw-r--r--  3.0 unx    13357 tx defN 21-Mar-06 14:31 setup.sh
 -rw-r--r--  3.0 unx      612 tx defN 20-Dec-20 16:34 flexmin.nginx
--rw-r--r--  3.0 unx      294 tx defN 23-Jan-12 14:40 flexmin.ini
--rw-r--r--  3.0 unx      320 tx defN 23-Jan-12 14:40 uwsgi-socket@flexmin.service
+-rw-r--r--  3.0 unx      294 tx defN 23-Jan-15 14:40 flexmin.ini
+-rw-r--r--  3.0 unx      320 tx defN 23-Jan-15 14:40 uwsgi-socket@flexmin.service
 -rw-r--r--  3.0 unx      328 tx defN 20-Dec-20 16:34 uwsgi-socket@py4web.service
 12 files, 17030 bytes uncompressed, 5717 bytes compressed:  66.4%
```

### Comparing `flexmin-0.3.7/flexmin/flexmin_cli.py` & `flexmin-0.3.9/flexmin/flexmin_cli.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/flexmin_srv.py` & `flexmin-0.3.9/flexmin/flexmin_srv.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/flexmin_task.py` & `flexmin-0.3.9/flexmin/flexmin_task.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/utils/output_prep.py` & `flexmin-0.3.9/flexmin/utils/output_prep.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/utils/simplepam.py` & `flexmin-0.3.9/flexmin/utils/simplepam.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/utils/test.py` & `flexmin-0.3.9/flexmin/utils/test.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/utils/utilities.py` & `flexmin-0.3.9/flexmin/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin/utils/yamlconfigs.py` & `flexmin-0.3.9/flexmin/utils/yamlconfigs.py`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/flexmin.egg-info/PKG-INFO` & `flexmin-0.3.9/flexmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: flexmin
-Version: 0.3.7
+Version: 0.3.9
 Summary: A flexible system admin web portal
-Home-page: 
+Home-page: https://www.futurscope.co.uk/flexmin
 Author: Richard Cooke
 Author-email: fm_1342@chrom3.co.uk
 Maintainer: Richard Cooke
 Maintainer-email: fm_1342@chrom3.co.uk
 License: BSD
 Platform: linux
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flexmin-0.3.7/flexmin.egg-info/SOURCES.txt` & `flexmin-0.3.9/flexmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexmin-0.3.7/setup.py` & `flexmin-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def get_version():
     regex = re.compile("__version__\s*\=\s*['\"](?P<version>.+?)['\"]")
     return regex.findall(open("flexmin/__init__.py").read())[0]
 
 setup(
     name="flexmin",
     version=get_version(),
-    url="",
+    url="https://www.futurscope.co.uk/flexmin",
     license="BSD",
     author="Richard Cooke",
     author_email="fm_1342@chrom3.co.uk",
     maintainer="Richard Cooke",
     maintainer_email="fm_1342@chrom3.co.uk",
     description="A flexible system admin web portal",
     long_description=long_description,
@@ -30,15 +30,15 @@
         "click",
         "pyyaml"
     ],
     entry_points={"console_scripts": ["flexmin=flexmin.flexmin_cli:cli"],},
     zip_safe=False,
     platforms="linux",
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

