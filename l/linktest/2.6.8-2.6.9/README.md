# Comparing `tmp/linktest-2.6.8.tar.gz` & `tmp/linktest-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.6.8.tar", last modified: Mon Apr 29 07:27:56 2024, max compression
+gzip compressed data, was "linktest-2.6.9.tar", last modified: Fri May  3 08:12:29 2024, max compression
```

## Comparing `linktest-2.6.8.tar` & `linktest-2.6.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-29 07:27:56.610276 linktest-2.6.8/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-29 07:27:56.610064 linktest-2.6.8/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-29 07:27:56.602541 linktest-2.6.8/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-29 03:12:25.000000 linktest-2.6.8/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33114 2024-04-28 14:55:18.000000 linktest-2.6.8/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   106863 2024-04-27 08:18:49.000000 linktest-2.6.8/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-04-29 06:53:03.000000 linktest-2.6.8/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-04-29 07:18:52.000000 linktest-2.6.8/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9047 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-29 03:12:31.000000 linktest-2.6.8/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13822 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13840 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13810 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-27 08:09:28.000000 linktest-2.6.8/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-29 07:27:56.609767 linktest-2.6.8/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-29 07:27:56.000000 linktest-2.6.8/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-04-29 07:27:56.000000 linktest-2.6.8/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-29 07:27:56.000000 linktest-2.6.8/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-29 07:27:56.000000 linktest-2.6.8/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-29 07:27:56.000000 linktest-2.6.8/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-29 07:27:56.610322 linktest-2.6.8/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-29 07:27:49.000000 linktest-2.6.8/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-03 08:12:29.124882 linktest-2.6.9/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-03 08:12:29.124641 linktest-2.6.9/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-03 08:12:29.122381 linktest-2.6.9/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-03 08:06:35.000000 linktest-2.6.9/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16095 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33522 2024-05-03 07:25:36.000000 linktest-2.6.9/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103469 2024-05-03 08:01:39.000000 linktest-2.6.9/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-04-30 08:36:58.000000 linktest-2.6.9/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9047 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-03 08:06:44.000000 linktest-2.6.9/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-04-30 08:35:06.000000 linktest-2.6.9/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13822 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13840 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13810 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14254 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-29 07:35:03.000000 linktest-2.6.9/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-03 08:12:29.124148 linktest-2.6.9/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-03 08:12:28.000000 linktest-2.6.9/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-03 08:12:28.000000 linktest-2.6.9/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-03 08:12:28.000000 linktest-2.6.9/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-03 08:12:28.000000 linktest-2.6.9/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-03 08:12:28.000000 linktest-2.6.9/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-03 08:12:29.124926 linktest-2.6.9/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-03 08:12:23.000000 linktest-2.6.9/setup.py
```

### Comparing `linktest-2.6.8/linktest/appium_utils.py` & `linktest-2.6.9/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/auto_generate_testcase_list.py` & `linktest-2.6.9/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.6.9/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/base_testcase.py` & `linktest-2.6.9/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/clean_data.py` & `linktest-2.6.9/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/conver_xml_into_db.py` & `linktest-2.6.9/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/database_helper.py` & `linktest-2.6.9/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/date_utilities.py` & `linktest-2.6.9/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/doctor.py` & `linktest-2.6.9/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/framework_log.py` & `linktest-2.6.9/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/generate_html_log.py` & `linktest-2.6.9/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/get_adb_devices.py` & `linktest-2.6.9/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/get_ios_devices_list.py` & `linktest-2.6.9/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/get_platform_info.py` & `linktest-2.6.9/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/get_project_info.py` & `linktest-2.6.9/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/html_report.py` & `linktest-2.6.9/linktest/html_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,31 +451,33 @@
                         report_file_handler.write(
                             " <a title='%s'> (" % 'Please see the execution logs for more details' + failed_testcase.exception_info + ") </a>")
                     except BaseException:
                         print(traceback.format_exc())
 
                     if failed_testcase.rerun_tag == 0:
                         try:
-                            report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> &nbsp;[TXT </font></a>" %
-                                failed_testcase.log_file_path)
-                            report_file_handler.write(
-                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML]</font></a>" %
-                                failed_testcase.log_file_path.replace("test.log", "test.html"))
+                            if getattr(settings, 'LOG_TO_FILE', False):
+                                report_file_handler.write(
+                                    "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> &nbsp;[TXT </font></a>" %
+                                    failed_testcase.log_file_path)
+                                report_file_handler.write(
+                                    " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML]</font></a>" %
+                                    failed_testcase.log_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                     elif failed_testcase.rerun_tag == 1:
                         try:
-                            report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
-                                failed_testcase.log_file_path)
-                            report_file_handler.write(
-                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
-                                failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
+                            if getattr(settings, 'LOG_TO_FILE', False):
+                                report_file_handler.write(
+                                    "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
+                                    failed_testcase.log_file_path)
+                                report_file_handler.write(
+                                    " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
+                                    failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center' >")
                     report_file_handler.write("<font>")
@@ -545,38 +547,40 @@
                         report_file_handler.write("<font color='orange'> - Miss Attribute</font>")
 
                     report_file_handler.write("</font>")
                     report_file_handler.write("</font></a>")
 
                     try:
                         if passed_testcase.rerun_tag == 0:
-                            report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
-                                passed_testcase.log_file_path)
-                            report_file_handler.write(
-                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
-                                passed_testcase.log_file_path.replace("test.log", "test.html"))
+                            if getattr(settings, 'LOG_TO_FILE', False):
+                                report_file_handler.write(
+                                    "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
+                                    passed_testcase.log_file_path)
+                                report_file_handler.write(
+                                    " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
+                                    passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     try:
                         if passed_testcase.rerun_tag == 1:
-                            report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a title='Log' href='%s'> &nbsp;[TXT </a>" %
-                                passed_testcase.log_file_path.replace("test.rerun.log", "test.log"))
-                            report_file_handler.write(
-                                " | <a target='_blank' title='HTML Log' href='%s'> HTML] </a>" %
-                                passed_testcase.log_file_path.replace("test.rerun.log", "test.html"))
-
-                            report_file_handler.write(
-                                "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a title='rerun_Log' href='%s'> &nbsp;[TXT </a>" %
-                                passed_testcase.log_file_path)
-                            report_file_handler.write(
-                                " | <a target='_blank' title='rerun_Log' href='%s'> HTML] </a>" %
-                                passed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
+                            if getattr(settings, 'LOG_TO_FILE', False):
+                                report_file_handler.write(
+                                    "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a title='Log' href='%s'> &nbsp;[TXT </a>" %
+                                    passed_testcase.log_file_path.replace("test.rerun.log", "test.log"))
+                                report_file_handler.write(
+                                    " | <a target='_blank' title='HTML Log' href='%s'> HTML] </a>" %
+                                    passed_testcase.log_file_path.replace("test.rerun.log", "test.html"))
+
+                                report_file_handler.write(
+                                    "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a title='rerun_Log' href='%s'> &nbsp;[TXT </a>" %
+                                    passed_testcase.log_file_path)
+                                report_file_handler.write(
+                                    " | <a target='_blank' title='rerun_Log' href='%s'> HTML] </a>" %
+                                    passed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center'>")
                     report_file_handler.write("<font color='#333'>")
```

### Comparing `linktest-2.6.8/linktest/logged_requests.py` & `linktest-2.6.9/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/main.py` & `linktest-2.6.9/linktest/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,22 +504,18 @@
 default_log_format = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
 default_level = logging.DEBUG
 
 # Read from settings
 log_format = getattr(settings, 'LOG_FORMAT', default_log_format)
 level = getattr(settings, 'LOG_LEVEL', default_level)
 
-log_to_file_flag = getattr(settings, 'LOG_TO_FILE', None)
-log_to_console_flag = getattr(settings, 'LOG_TO_CONSOLE', None)
 ####### testcase log settings end #######
 
 
 class TestCaseExecutor(threading.Thread):
-    # rerun_failed_testcases = []
-    # rerun_passed_testcases = []
     failed_testcases = []
     passed_testcases = []
     error_testcases = []
     executing_ios_testcase_flag = False
     testcase_queue = collections.deque()
     report_lock = threading.Lock()
     appium_lock = threading.Lock()
@@ -549,23 +545,23 @@
 
             if not os.path.exists(testcase_full_folder):
                 os.makedirs(testcase_full_folder)
 
             logfile_full_name = testcase_full_folder + os.sep + logger_name
 
             # Add FileHandler if LOG_TO_FILE is set to True in settings
-            if log_to_file_flag:
+            if getattr(settings, 'LOG_TO_FILE', False):
                 handlers.append(logging.FileHandler(logfile_full_name))
 
             # Add StreamHandler if LOG_TO_CONSOLE is set to True in settings
-            if log_to_console_flag:
+            if getattr(settings, 'LOG_TO_CONSOLE', False):
                 handlers.append(logging.StreamHandler(sys.stdout))
 
             # If no handlers are specified, add FileHandler & StreamHandler as default, Note: None is not False
-            if log_to_file_flag is None and log_to_console_flag is None:
+            if getattr(settings, 'LOG_TO_FILE', None) and getattr(settings, 'LOG_TO_CONSOLE', None):
                 handlers.append(logging.FileHandler(logfile_full_name))
                 handlers.append(logging.StreamHandler(sys.stdout))
 
             # Define basic configuration
             logging.basicConfig(
                 # Define logging level
                 level=level,
@@ -1250,15 +1246,20 @@
                             setattr(TestCaseExecutor, device_name, False)
 
                         if getattr(settings, 'LOG_TO_FILE', False):
                             with open(executing_testcase.logfile_full_name, "r", encoding="utf-8", errors="ignore") as logfile_full_name:
                                 execution_log = logfile_full_name.read()
                                 executing_testcase.execution_log = execution_log
                     finally:
-                        generate_html_log.generate_html_log(executing_testcase)
+                        try:
+                            if getattr(settings, 'LOG_TO_FILE', False):
+                                generate_html_log.generate_html_log(executing_testcase)
+                        except BaseException:
+                            traceback.print_exc()
+                            executing_testcase.logger.error(traceback.format_exc())
 
                         if os.sep + "jenkins" + os.sep + "workspace" + os.sep in project_info.project_path:
                             TestCaseExecutor.jenkins_job_name = \
                                 project_info.project_path.split(os.sep + "jenkins" + os.sep + "workspace" + os.sep)[
                                     1].split(os.sep)[0]
 
                 try:
@@ -1439,14 +1440,21 @@
             for argv in argv_dict.keys():
                 if argv not in updated_argv:
                     argv_list_not_found.append(argv)
 
             print("***************** WARNING: below argv not found in settings/__init__.py *****************")
             print(argv_list_not_found)
 
+            for nof_found_arv in argv_list_not_found:
+                print("***************** WARNING: %s *****************" % nof_found_arv)
+                with open(settings_file_path, "a") as settings_new_file:
+                    print("%s = %s \n" % (nof_found_arv, argv_dict[nof_found_arv]))
+
+                    settings_new_file.writelines("\n%s = %s \n" % (nof_found_arv, argv_dict[nof_found_arv]))
+
         try:
             importlib.reload(settings)
         except BaseException:
             traceback.print_exc()
 
 
 def run_with(args=None):
@@ -2015,15 +2023,15 @@
         if not settings.DEBUG_RUN:
             close_browsers_and_webdrivers()
         else:
             clean_appium_env()
 
 
         try:
-            if hasattr(settings, "generate_xunit_result") and settings.generate_xunit_result is True:
+            if getattr(settings, "generate_xunit_result", False):
                 xml_report.generate_xunit_result(TestCaseExecutor.passed_testcases,
                                                  TestCaseExecutor.failed_testcases,
                                                  output_folder,
                                                  begin_time
                                                  )
                 print("generate xml report done...")
         except BaseException:
@@ -2088,90 +2096,29 @@
                             rerun_flag=1 if settings.RERUN_FLAG else 0
                         )
             except BaseException:
                 traceback.print_exc()
             finally:
                 pass
 
-        # print("=*=*=" * 20 + os.linesep + "Execution Done! More details please see blow html report:" + os.linesep + "file:///" + output_folder + os.sep + "report.html")
-
-        if hasattr(settings, "COPY_REPORT_TO_SPECIFIED_PATH"):
-            if settings.COPY_REPORT_TO_SPECIFIED_PATH is True:
-                if not hasattr(settings, "SPECIFIED_REPORT_PATH") or not hasattr(settings, "SPECIFIED_REPORT_HOST_IP") \
-                        or not hasattr(settings, "SPECIFIED_REPORT_HOST_PORT") or not hasattr(settings,
-                                                                                              "SPECIFIED_REPORT_HOST_USERNAME") \
-                        or not hasattr(settings, "SPECIFIED_REPORT_HOST_PASSWORD"):
-                    raise Exception("如果 COPY_REPORT_TO_SPECIFIED_PATH = True, 则必须设置：SPECIFIED_REPORT_PATH & "
-                                    "SPECIFIED_REPORT_HOST_IP & SPECIFIED_REPORT_HOST_PORT & SPECIFIED_REPORT_HOST_USERNAME & SPECIFIED_REPORT_HOST_PASSWORD")
-
-                # # send report to server
-                # def scp_report_to_specified_path(file_path=output_folder):
-                #     ssh_client = paramiko.SSHClient()
-                #     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy)
-                #     ssh_client.connect(settings.SPECIFIED_REPORT_HOST_IP, settings.SPECIFIED_REPORT_HOST_PORT,
-                #                        settings.SPECIFIED_REPORT_HOST_USERNAME, settings.SPECIFIED_REPORT_HOST_PASSWORD)
-                #     scpclient = SCPClient(ssh_client.get_transport(), socket_timeout=15.0)
-                #     # local_path = file_path
-                #
-                #     try:
-                #         scpclient.put(file_path, settings.SPECIFIED_REPORT_PATH, recursive=True, )
-                #     except FileNotFoundError as e:
-                #         print(e)
-                #         print("系统找不到指定文件" + file_path)
-                #     else:
-                #         print("文件上传成功" + output_folder)
-                #     finally:
-                #         ssh_client.close()
-
-                # scp_report_to_specified_path(output_folder)
-
         # 如果最后执行完所有的testcase 并且GlobalDataList 不为空，则自动保存GlobalDataList
         if len(BaseTestCase.GlobalDataList) > 0:
+            file_path = os.path.join(output_folder, "global_data_list.py")
             try:
-                with open(output_folder + os.sep + "global_data_list.py", "w") as f:
-                    f.write("global_data_list = " + str(BaseTestCase.GlobalDataList))
+                with open(file_path, "w", encoding='utf-8') as f:
+                    f.write("global_data_list = " + json.dumps(BaseTestCase.GlobalDataList, indent=4, ensure_ascii=False))
 
-                print("Global Data List:")
-                print(output_folder + os.sep + "global_data_list.py")
-            except BaseException:
-                print("------------------- write global_data_list error!")
-                traceback.print_exc()
+                print("Global Data List File Path:")
+                print(file_path)
+            except OSError as e:
+                print("Error writing global_data_list to file:")
+                print(str(e))
+            except Exception as e:
+                print("An unexpected error occurred:")
+                print(str(e))
 
         return output_folder, BaseTestCase.GlobalExecutedCaseList[-1].logfile_full_name
 
-        #  todo: 需要再优化一下，save_log_to_db 不应该和 SAVE_SCREENSHOTS_PATH 耦合！！
-        # if hasattr(settings, "SAVE_LOG_TO_DB"):
-        #     if settings.SAVE_LOG_TO_DB is True:
-        #         if not hasattr(settings, "SAVE_SCREENSHOTS_PATH"):
-        #             raise Exception("如果 SAVE_LOG_TO_DB = True, 则必须设置：SAVE_SCREENSHOTS_PATH")
-        #
-        #         # only copy the screenshot for Non backend_testcases
-        #         if non_backend_testcase_count > 0:
-        #             import shutil
-        #
-        #             def ignore_pyc_files(dirname, filenames):
-        #                 ig_list = []
-        #                 for name in filenames:
-        #                     if name.endswith('.pyc') or name.endswith(".log") or name.endswith("html") or name.endswith(
-        #                             "xml"):
-        #                         ig_list.append(name)
-        #                 return ig_list
-        #
-        #             try:
-        #                 # TODO: here should copy the screenshots to the dashboard server's static/screenshots
-        #                 shutil.copytree(output_folder,
-        #                                 settings.SAVE_SCREENSHOTS_PATH +
-        #                                 output_folder.split(os.sep)[-1],
-        #                                 ignore=ignore_pyc_files)
-        #                 print("==== copy screenshots done ====")
-        #                 print(settings.SAVE_SCREENSHOTS_PATH + output_folder.split(os.sep)[-1])
-        #             except shutil.Error as e:
-        #                 for src, dst, msg in e.args[0]:
-        #                     # src is source name
-        #                     # dst is destination name
-        #                     # msg is error message from exception
-        #                     print(dst, src, msg)
-
 
 if __name__ == "__main__":
     close_browsers_and_webdrivers()
     run_with(sys.argv)
```

### Comparing `linktest-2.6.8/linktest/memory_usage.py` & `linktest-2.6.9/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/re_func.py` & `linktest-2.6.9/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/run.py` & `linktest-2.6.9/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/run_testcase_thread.py` & `linktest-2.6.9/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/scp_report_to_specified_path.py` & `linktest-2.6.9/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/selenium_helper.py` & `linktest-2.6.9/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/timeout_thread.py` & `linktest-2.6.9/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/ui_testcase.py` & `linktest-2.6.9/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/update_config.py` & `linktest-2.6.9/linktest/update_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,7 +84,15 @@
 
         for argv in argv_dict.keys():
             if argv not in updated_argv:
                 argv_list_not_found.append(argv)
 
         print("***************** WARNING: below argv not found in settings/__init__.py *****************")
         print(argv_list_not_found)
+
+        for nof_found_arv in argv_list_not_found:
+            print("***************** WARNING: %s *****************" % nof_found_arv)
+            with open(settings_file_path, "a") as settings_new_file:
+                print("%s = %s \n" % (nof_found_arv, argv_dict[nof_found_arv]))
+
+                settings_new_file.writelines("%s = %s \n" % (nof_found_arv, argv_dict[nof_found_arv]))
+
```

### Comparing `linktest-2.6.8/linktest/webdriver_wrapper.py` & `linktest-2.6.9/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/webdriver_wrapper_chrome.py` & `linktest-2.6.9/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/webdriver_wrapper_edge.py` & `linktest-2.6.9/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/webdriver_wrapper_firefox.py` & `linktest-2.6.9/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/webdriver_wrapper_ie.py` & `linktest-2.6.9/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/webdriver_wrapper_safari.py` & `linktest-2.6.9/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest/xml_report.py` & `linktest-2.6.9/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.6.8/linktest.egg-info/SOURCES.txt` & `linktest-2.6.9/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

