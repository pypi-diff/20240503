# Comparing `tmp/xnote-web-0.0.9.tar.gz` & `tmp/xnote-web-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnote-web-0.0.9.tar", last modified: Sun Mar 31 06:48:26 2024, max compression
+gzip compressed data, was "xnote-web-0.1.0.tar", last modified: Fri May  3 04:09:11 2024, max compression
```

## Comparing `xnote-web-0.0.9.tar` & `xnote-web-0.1.0.tar`

### file list

```diff
@@ -1,1212 +1,1217 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.389029 xnote-web-0.0.9/
--rw-rw-rw-   0        0        0    35147 2021-10-01 10:27:00.000000 xnote-web-0.0.9/COPYING
--rw-rw-rw-   0        0        0      259 2023-10-27 13:17:40.000000 xnote-web-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5759 2024-03-31 06:48:26.387026 xnote-web-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5416 2024-03-16 14:56:17.000000 xnote-web-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.733454 xnote-web-0.0.9/config/
--rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.0.9/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.776471 xnote-web-0.0.9/config/boot/
--rw-rw-rw-   0        0        0     3595 2024-03-16 14:56:17.000000 xnote-web-0.0.9/config/boot/boot.default.properties
--rw-rw-rw-   0        0        0      413 2022-05-29 13:03:06.000000 xnote-web-0.0.9/config/boot/boot.local.follower.properties
--rw-rw-rw-   0        0        0      612 2022-10-06 02:04:52.000000 xnote-web-0.0.9/config/boot/boot.local.leveldb.properties
--rw-rw-rw-   0        0        0      768 2023-07-15 13:09:54.000000 xnote-web-0.0.9/config/boot/boot.local.properties
--rw-rw-rw-   0        0        0      116 2023-04-06 04:04:41.000000 xnote-web-0.0.9/config/boot/boot.min.properties
--rw-rw-rw-   0        0        0      557 2024-03-16 14:56:17.000000 xnote-web-0.0.9/config/boot/boot.sae.properties
--rw-rw-rw-   0        0        0      113 2022-08-14 10:12:12.000000 xnote-web-0.0.9/config/boot/boot.sqlite.properties
--rw-rw-rw-   0        0        0      201 2024-03-16 14:56:17.000000 xnote-web-0.0.9/config/boot/boot.test.properties
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.779555 xnote-web-0.0.9/config/cron/
--rw-rw-rw-   0        0        0     1572 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/cron/cron.json
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.801853 xnote-web-0.0.9/config/file/
--rw-rw-rw-   0        0        0       20 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/file/audio.properties
--rw-rw-rw-   0        0        0      142 2023-03-04 06:34:27.000000 xnote-web-0.0.9/config/file/code.properties
--rw-rw-rw-   0        0        0      181 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/file/image.properties
--rw-rw-rw-   0        0        0      448 2022-04-17 03:52:32.000000 xnote-web-0.0.9/config/file/mime-types.properties
--rw-rw-rw-   0        0        0      298 2023-10-27 13:17:40.000000 xnote-web-0.0.9/config/file/preview.properties
--rw-rw-rw-   0        0        0      580 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/file/text.properties
--rw-rw-rw-   0        0        0       35 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/file/video.properties
--rw-rw-rw-   0        0        0       27 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/file/zip.properties
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.807279 xnote-web-0.0.9/config/lang/
--rw-rw-rw-   0        0        0      794 2022-03-19 10:57:33.000000 xnote-web-0.0.9/config/lang/en.properties
--rw-rw-rw-   0        0        0     2259 2023-07-16 02:37:42.000000 xnote-web-0.0.9/config/lang/zh.properties
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.815112 xnote-web-0.0.9/config/note/
--rw-rw-rw-   0        0        0      231 2022-07-15 15:16:19.000000 xnote-web-0.0.9/config/note/category.ddc.properties
--rw-rw-rw-   0        0        0      135 2022-07-15 16:06:41.000000 xnote-web-0.0.9/config/note/category.properties
--rw-rw-rw-   0        0        0      857 2022-11-26 16:30:19.000000 xnote-web-0.0.9/config/note/smart_group.ini
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.824670 xnote-web-0.0.9/config/plugin/
--rw-rw-rw-   0        0        0     6718 2024-03-16 14:56:17.000000 xnote-web-0.0.9/config/plugin/form_plugin.tpl.py
--rw-rw-rw-   0        0        0      798 2024-03-16 14:56:17.000000 xnote-web-0.0.9/config/plugin/plugin.tpl.py
--rw-rw-rw-   0        0        0      179 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/plugin/plugins.ini
--rw-rw-rw-   0        0        0      141 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/requirements.full.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/requirements.min.txt
--rw-rw-rw-   0        0        0       25 2023-10-27 13:17:40.000000 xnote-web-0.0.9/config/requirements.mysql.txt
--rw-rw-rw-   0        0        0       88 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/requirements.test.txt
--rw-rw-rw-   0        0        0      127 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/requirements.txt
--rw-rw-rw-   0        0        0      126 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/requirements.win.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.828986 xnote-web-0.0.9/config/user/
--rw-rw-rw-   0        0        0       76 2021-10-01 10:27:00.000000 xnote-web-0.0.9/config/user/invalid_names.list
--rw-rw-rw-   0        0        0      818 2023-06-30 12:24:59.000000 xnote-web-0.0.9/config/user/user_config.default.properties
--rw-rw-rw-   0        0        0       23 2024-03-31 06:42:05.000000 xnote-web-0.0.9/config/version.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.862228 xnote-web-0.0.9/docs/
--rw-rw-rw-   0        0        0     2792 2022-11-26 16:30:19.000000 xnote-web-0.0.9/docs/architecture.md
--rw-rw-rw-   0        0        0    18566 2024-03-16 14:56:17.000000 xnote-web-0.0.9/docs/changelog.md
--rw-rw-rw-   0        0        0     3008 2022-05-28 11:20:41.000000 xnote-web-0.0.9/docs/code_style.md
--rw-rw-rw-   0        0        0      567 2022-03-13 14:33:54.000000 xnote-web-0.0.9/docs/code_style_css.md
--rw-rw-rw-   0        0        0     2257 2022-11-26 16:30:19.000000 xnote-web-0.0.9/docs/commands.md
--rw-rw-rw-   0        0        0     3025 2023-10-27 13:17:40.000000 xnote-web-0.0.9/docs/database.md
--rw-rw-rw-   0        0        0     1799 2023-10-27 13:17:40.000000 xnote-web-0.0.9/docs/db_migrate.md
--rw-rw-rw-   0        0        0     1364 2022-11-26 16:30:19.000000 xnote-web-0.0.9/docs/plugins.md
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.972739 xnote-web-0.0.9/docs/screenshots/
--rw-rw-rw-   0        0        0    43384 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/architecture.png
--rw-rw-rw-   0        0        0    13063 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/architecture.svg
--rw-rw-rw-   0        0        0    57359 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/architecture_2.png
--rw-rw-rw-   0        0        0   112396 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/command_listdir.png
--rw-rw-rw-   0        0        0    81824 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/command_rmfolder.png
--rw-rw-rw-   0        0        0   139528 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/screenshot01.png
--rw-rw-rw-   0        0        0   236777 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/screenshot02.png
--rw-rw-rw-   0        0        0   101099 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/screenshot03.png
--rw-rw-rw-   0        0        0    24412 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/task_web.PNG
--rw-rw-rw-   0        0        0    29284 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.2_editor.PNG
--rw-rw-rw-   0        0        0    43162 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.2_list.PNG
--rw-rw-rw-   0        0        0   225642 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.2_mobile.png
--rw-rw-rw-   0        0        0    23527 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.2_search.png
--rw-rw-rw-   0        0        0    54676 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.3_desktop01.png
--rw-rw-rw-   0        0        0   153849 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.4.png
--rw-rw-rw-   0        0        0   235750 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v1.5.png
--rw-rw-rw-   0        0        0   214791 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.0.png
--rw-rw-rw-   0        0        0   187105 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.1_home.png
--rw-rw-rw-   0        0        0   202760 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.2_20190331.png
--rw-rw-rw-   0        0        0   179408 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.3_20190411.png
--rw-rw-rw-   0        0        0   214443 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.3_home.png
--rw-rw-rw-   0        0        0    99255 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.4_home.png
--rw-rw-rw-   0        0        0   103529 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.4_home2.png
--rw-rw-rw-   0        0        0    82664 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.5_20200502.png
--rw-rw-rw-   0        0        0   121009 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.5_home.png
--rw-rw-rw-   0        0        0    78846 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.5_recent.png
--rw-rw-rw-   0        0        0    66479 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.6_home.png
--rw-rw-rw-   0        0        0   107994 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.7_home.png
--rw-rw-rw-   0        0        0    88658 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.8_home.png
--rw-rw-rw-   0        0        0   120643 2022-11-26 16:30:19.000000 xnote-web-0.0.9/docs/screenshots/xnote_v2.9.2_home.png
--rw-rw-rw-   0        0        0   110782 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote_v20191111.png
--rw-rw-rw-   0        0        0   158216 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/screenshots/xnote架构.png
--rw-rw-rw-   0        0        0       16 2021-10-01 10:27:00.000000 xnote-web-0.0.9/docs/search_extension.md
--rw-rw-rw-   0        0        0      456 2024-03-16 14:56:17.000000 xnote-web-0.0.9/docs/upload_to_pip.md
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.994741 xnote-web-0.0.9/handlers/
--rw-rw-rw-   0        0        0       26 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.000742 xnote-web-0.0.9/handlers/admin/
--rw-rw-rw-   0        0        0        0 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/admin/__init__.py
--rw-rw-rw-   0        0        0     1439 2024-03-31 03:21:12.000000 xnote-web-0.0.9/handlers/admin/func_admin.py
--rw-rw-rw-   0        0        0     5567 2024-03-31 03:21:40.000000 xnote-web-0.0.9/handlers/admin/job_admin.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.030042 xnote-web-0.0.9/handlers/api/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/__init__.py
--rw-rw-rw-   0        0        0      705 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/alarm.py
--rw-rw-rw-   0        0        0      727 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/check_network.py
--rw-rw-rw-   0        0        0     1249 2023-03-11 14:27:18.000000 xnote-web-0.0.9/handlers/api/getip.py
--rw-rw-rw-   0        0        0      365 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/http_headers.py
--rw-rw-rw-   0        0        0     1466 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/ipv6.py
--rw-rw-rw-   0        0        0     3563 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/readbook.py
--rw-rw-rw-   0        0        0     1020 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/report_time.py
--rw-rw-rw-   0        0        0     1986 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/api/report_weather.py
--rw-rw-rw-   0        0        0      604 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/api/tts.py
--rw-rw-rw-   0        0        0       30 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/base.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.060970 xnote-web-0.0.9/handlers/code/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/code/__init__.py
--rw-rw-rw-   0        0        0     7726 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/code/code_edit.html
--rw-rw-rw-   0        0        0     4717 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/code/code_edit.py
--rw-rw-rw-   0        0        0     2573 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/code/code_lines.html
--rw-rw-rw-   0        0        0     6066 2022-04-30 02:31:41.000000 xnote-web-0.0.9/handlers/code/code_lines.py
--rw-rw-rw-   0        0        0     3278 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/code/code_search.html
--rw-rw-rw-   0        0        0     8351 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/code/code_search.py
--rw-rw-rw-   0        0        0     2480 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/code/preview.html
--rw-rw-rw-   0        0        0     5556 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/code/preview.py
--rw-rw-rw-   0        0        0     5912 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/code/wiki_edit.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.096840 xnote-web-0.0.9/handlers/common/
--rw-rw-rw-   0        0        0      472 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/README.md
--rw-rw-rw-   0        0        0      121 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/back.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.102241 xnote-web-0.0.9/handlers/common/base/
--rw-rw-rw-   0        0        0      410 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/base/README.md
--rw-rw-rw-   0        0        0     1358 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/base/pagination.html
--rw-rw-rw-   0        0        0     2156 2023-11-19 08:31:53.000000 xnote-web-0.0.9/handlers/common/base.html
--rw-rw-rw-   0        0        0       79 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/base_bottom.html
--rw-rw-rw-   0        0        0      927 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/base_footer.html
--rw-rw-rw-   0        0        0     2414 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/common/base_head.html
--rw-rw-rw-   0        0        0      988 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/common/base_nav.html
--rw-rw-rw-   0        0        0      185 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/base_simple.html
--rw-rw-rw-   0        0        0      645 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/base_title.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.105972 xnote-web-0.0.9/handlers/common/button/
--rw-rw-rw-   0        0        0      149 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/button/back_button.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.108263 xnote-web-0.0.9/handlers/common/date/
--rw-rw-rw-   0        0        0     2820 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/common/date/month_picker.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.112264 xnote-web-0.0.9/handlers/common/form/
--rw-rw-rw-   0        0        0     3602 2024-03-31 06:34:38.000000 xnote-web-0.0.9/handlers/common/form/form.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.118265 xnote-web-0.0.9/handlers/common/hook/
--rw-rw-rw-   0        0        0      137 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/hook/message_search_btn_hook.html
--rw-rw-rw-   0        0        0      526 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/hook/search_box_hook.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.124751 xnote-web-0.0.9/handlers/common/layout/
--rw-rw-rw-   0        0        0     3870 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/common/layout/base_layout.html
--rw-rw-rw-   0        0        0       67 2023-04-06 10:45:42.000000 xnote-web-0.0.9/handlers/common/layout/wide_left.html
--rw-rw-rw-   0        0        0      702 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/mod_notice.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.135285 xnote-web-0.0.9/handlers/common/nav/
--rw-rw-rw-   0        0        0     2919 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/common/nav/base_nav_left.html
--rw-rw-rw-   0        0        0     1374 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/nav/base_nav_project.html
--rw-rw-rw-   0        0        0      654 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/nav/base_nav_top.html
--rw-rw-rw-   0        0        0      799 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/nav/content_nav.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.139783 xnote-web-0.0.9/handlers/common/page/
--rw-rw-rw-   0        0        0      497 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/page/notfound.html
--rw-rw-rw-   0        0        0     1358 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/pagination.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.168410 xnote-web-0.0.9/handlers/common/script/
--rw-rw-rw-   0        0        0     1251 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/common/script/adjust.html
--rw-rw-rw-   0        0        0      420 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/script/debug_script.html
--rw-rw-rw-   0        0        0      965 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/script/geo_location.html
--rw-rw-rw-   0        0        0      460 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/common/script/image_fix_1.html
--rw-rw-rw-   0        0        0     4529 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/common/script/image_fix_2.html
--rw-rw-rw-   0        0        0      455 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/common/script/load_vue.html
--rw-rw-rw-   0        0        0      764 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/common/script/require_init.html
--rw-rw-rw-   0        0        0      256 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/common/script/safe_script.html
--rw-rw-rw-   0        0        0     3234 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/common/script/textarea_script.html
--rw-rw-rw-   0        0        0      463 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/common/script/translate_script.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.177320 xnote-web-0.0.9/handlers/common/search/
--rw-rw-rw-   0        0        0      758 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/search/search_box.html
--rw-rw-rw-   0        0        0      750 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/search/search_mobile.html
--rw-rw-rw-   0        0        0       43 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/search_box.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.181479 xnote-web-0.0.9/handlers/common/sidebar/
--rw-rw-rw-   0        0        0      724 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/sidebar/app_index.html
--rw-rw-rw-   0        0        0       43 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/sidebar/default.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.184138 xnote-web-0.0.9/handlers/common/table/
--rw-rw-rw-   0        0        0     3316 2024-03-31 06:26:51.000000 xnote-web-0.0.9/handlers/common/table/table.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.187475 xnote-web-0.0.9/handlers/common/text/
--rw-rw-rw-   0        0        0       41 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/common/text/empty_text.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.193147 xnote-web-0.0.9/handlers/common/theme/
--rw-rw-rw-   0        0        0     2331 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/common/theme/sidebar.html
--rw-rw-rw-   0        0        0     1683 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/common/theme/sidebar_left.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.196239 xnote-web-0.0.9/handlers/common/title/
--rw-rw-rw-   0        0        0      273 2021-10-31 03:54:18.000000 xnote-web-0.0.9/handlers/common/title/base_title.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.257015 xnote-web-0.0.9/handlers/cron/
--rw-rw-rw-   0        0        0      142 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/cron/__init__.py
--rw-rw-rw-   0        0        0      999 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/cron/cron_stats.py
--rw-rw-rw-   0        0        0     3344 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/cron/diskclean.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.329302 xnote-web-0.0.9/handlers/dict/
--rw-rw-rw-   0        0        0      136 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/dict/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.339448 xnote-web-0.0.9/handlers/dict/component/
--rw-rw-rw-   0        0        0      798 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/dict/component/dict_sidebar.html
--rw-rw-rw-   0        0        0     2483 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/dict/dao_relevant.py
--rw-rw-rw-   0        0        0     5490 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/dict/dict.py
--rw-rw-rw-   0        0        0     2620 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/dict/dict_dao.py
--rw-rw-rw-   0        0        0     2000 2022-05-21 15:50:36.000000 xnote-web-0.0.9/handlers/dict/dict_relevant.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.364076 xnote-web-0.0.9/handlers/dict/page/
--rw-rw-rw-   0        0        0     1899 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/dict/page/dict_add.html
--rw-rw-rw-   0        0        0     1255 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/dict/page/dict_edit.html
--rw-rw-rw-   0        0        0     1305 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/dict/page/dict_list.html
--rw-rw-rw-   0        0        0     2650 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/dict/page/dict_update.html
--rw-rw-rw-   0        0        0     3767 2022-05-15 04:37:11.000000 xnote-web-0.0.9/handlers/dict/page/relevant_list.html
--rw-rw-rw-   0        0        0      589 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/error.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.475047 xnote-web-0.0.9/handlers/fs/
--rw-rw-rw-   0        0        0      142 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/fs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.507107 xnote-web-0.0.9/handlers/fs/component/
--rw-rw-rw-   0        0        0     2927 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/fs/component/clipboard-dialog.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.512104 xnote-web-0.0.9/handlers/fs/component/css/
--rw-rw-rw-   0        0        0      103 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/fs/component/css/fs_css.html
--rw-rw-rw-   0        0        0     1505 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/component/filelist_gallery.html
--rw-rw-rw-   0        0        0     1053 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/fs/component/filelist_simple.html
--rw-rw-rw-   0        0        0      893 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/component/fs_sidebar.html
--rw-rw-rw-   0        0        0      408 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/component/fs_title.html
--rw-rw-rw-   0        0        0     4086 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/component/move_file_dialog.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.533700 xnote-web-0.0.9/handlers/fs/component/options/
--rw-rw-rw-   0        0        0      673 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/fs/component/options/fs_options.html
--rw-rw-rw-   0        0        0     3238 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/fs/component/options/fs_options_buttons.html
--rw-rw-rw-   0        0        0     2132 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/fs/component/options/fs_options_buttons.mobile.html
--rw-rw-rw-   0        0        0     2942 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/fs/component/options_css.html
--rw-rw-rw-   0        0        0     1910 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/component/plugins-dialog.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.542703 xnote-web-0.0.9/handlers/fs/component/script/
--rw-rw-rw-   0        0        0    14268 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/component/script/file_op_script.html
--rw-rw-rw-   0        0        0    24168 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs.py
--rw-rw-rw-   0        0        0     2642 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/fs_add.py
--rw-rw-rw-   0        0        0      867 2022-05-21 16:20:57.000000 xnote-web-0.0.9/handlers/fs/fs_api.py
--rw-rw-rw-   0        0        0     1862 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/fs/fs_cache.py
--rw-rw-rw-   0        0        0     2806 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs_find.py
--rw-rw-rw-   0        0        0     6768 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs_helper.py
--rw-rw-rw-   0        0        0     4615 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs_hex.py
--rw-rw-rw-   0        0        0     2428 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/fs_image.py
--rw-rw-rw-   0        0        0     7046 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs_index.py
--rw-rw-rw-   0        0        0     1004 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/fs/fs_mode.py
--rw-rw-rw-   0        0        0     4700 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/fs/fs_plugins.py
--rw-rw-rw-   0        0        0     3635 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/fs/fs_preview.py
--rw-rw-rw-   0        0        0     5410 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs_text.py
--rw-rw-rw-   0        0        0    13748 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/fs_upload.py
--rw-rw-rw-   0        0        0     1902 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/mod_aside.html
--rw-rw-rw-   0        0        0     6622 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/mod_fs_upload.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.585531 xnote-web-0.0.9/handlers/fs/page/
--rw-rw-rw-   0        0        0     2121 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/page/fs.html
--rw-rw-rw-   0        0        0     1974 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/fs/page/fs_bookmark.html
--rw-rw-rw-   0        0        0     3165 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/fs/page/fs_grid.html
--rw-rw-rw-   0        0        0     2778 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/page/fs_index.html
--rw-rw-rw-   0        0        0      352 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/fs/page/fs_not_readable.html
--rw-rw-rw-   0        0        0     2540 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/fs/page/fs_plugins.html
--rw-rw-rw-   0        0        0     1788 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/fs/page/fs_shell.html
--rw-rw-rw-   0        0        0     4442 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/fs/page/fs_sidebar.html
--rw-rw-rw-   0        0        0     5629 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/fs/page/fs_text.html
--rw-rw-rw-   0        0        0     4920 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/fs/page/fs_text_v1.html
--rw-rw-rw-   0        0        0     3078 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/fs/page/fs_upload.html
--rw-rw-rw-   0        0        0     2093 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/index.html
--rw-rw-rw-   0        0        0     1517 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/index.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.613632 xnote-web-0.0.9/handlers/message/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/message/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.621126 xnote-web-0.0.9/handlers/message/ajax/
--rw-rw-rw-   0        0        0     4497 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/message/ajax/message_ajax.html
--rw-rw-rw-   0        0        0     2711 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/message/ajax/message_tag_ajax.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.640942 xnote-web-0.0.9/handlers/message/card/
--rw-rw-rw-   0        0        0    17381 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/card/deleted_msg_left.html
--rw-rw-rw-   0        0        0     4712 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/message/card/deleted_msg_left_new.html
--rw-rw-rw-   0        0        0      585 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/message/card/deleted_msg_right.html
--rw-rw-rw-   0        0        0     1401 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/card/message_system_tag.html
--rw-rw-rw-   0        0        0     1429 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/message/card/msg_edit_card.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.695844 xnote-web-0.0.9/handlers/message/component/
--rw-rw-rw-   0        0        0      977 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/component/message_date_right.html
--rw-rw-rw-   0        0        0     3782 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/message/component/message_edit.html
--rw-rw-rw-   0        0        0      787 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/message/component/message_event.html
--rw-rw-rw-   0        0        0      415 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/message/component/message_header.html
--rw-rw-rw-   0        0        0     2860 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/component/message_input.html
--rw-rw-rw-   0        0        0     1230 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/message/component/message_keyword_info.html
--rw-rw-rw-   0        0        0     2059 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/component/message_list.html
--rw-rw-rw-   0        0        0     1956 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/component/message_sub_link.html
--rw-rw-rw-   0        0        0     1181 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/component/message_tab.html
--rw-rw-rw-   0        0        0      821 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/component/message_tab_log.html
--rw-rw-rw-   0        0        0      833 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/component/message_tab_task.html
--rw-rw-rw-   0        0        0      669 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/component/message_tag_list.html
--rw-rw-rw-   0        0        0      977 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/message/component/message_title.html
--rw-rw-rw-   0        0        0     3343 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/component/message_todo_inner.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.699336 xnote-web-0.0.9/handlers/message/component/right/
--rw-rw-rw-   0        0        0     1169 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/component/right/tags.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.701782 xnote-web-0.0.9/handlers/message/component/script/
--rw-rw-rw-   0        0        0     1009 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/message/component/script/tab_script.html
--rw-rw-rw-   0        0        0     1939 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/message/component/select_topic_dialog.html
--rw-rw-rw-   0        0        0      765 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/message/component/show_topic_dialog.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.706005 xnote-web-0.0.9/handlers/message/component/tag/
--rw-rw-rw-   0        0        0      884 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/component/tag/orderby_tab.html
--rw-rw-rw-   0        0        0    33301 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/dao.py
--rw-rw-rw-   0        0        0    35414 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/message.py
--rw-rw-rw-   0        0        0      904 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/message_model.py
--rw-rw-rw-   0        0        0     3647 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/message_search.py
--rw-rw-rw-   0        0        0     3058 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/message_tag.py
--rw-rw-rw-   0        0        0     2646 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/message_task.py
--rw-rw-rw-   0        0        0    17095 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/message_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.734384 xnote-web-0.0.9/handlers/message/page/
--rw-rw-rw-   0        0        0     1064 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/message/page/message.html
--rw-rw-rw-   0        0        0     2226 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/page/message_calendar.html
--rw-rw-rw-   0        0        0     2214 2024-03-16 14:56:17.000000 xnote-web-0.0.9/handlers/message/page/message_list_by_day.html
--rw-rw-rw-   0        0        0     3752 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/page/message_list_view.html
--rw-rw-rw-   0        0        0     4057 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/message/page/message_search.html
--rw-rw-rw-   0        0        0     2716 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/page/message_tag_select.html
--rw-rw-rw-   0        0        0     1608 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/message/page/message_tag_view.html
--rw-rw-rw-   0        0        0      178 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/message/page/message_todo.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.741484 xnote-web-0.0.9/handlers/message/page/old/
--rw-rw-rw-   0        0        0     1967 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/page/old/dairy.html
--rw-rw-rw-   0        0        0    12904 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/message/page/old/message_calendar_old.html
--rw-rw-rw-   0        0        0     3251 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/message/page/task_index.html
--rw-rw-rw-   0        0        0      823 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/mod_fs_path.html
--rw-rw-rw-   0        0        0       36 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/mod_pagenation.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.856223 xnote-web-0.0.9/handlers/note/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.885635 xnote-web-0.0.9/handlers/note/ajax/
--rw-rw-rw-   0        0        0     2587 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/ajax/comment_edit_dialog.html
--rw-rw-rw-   0        0        0     1265 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/note/ajax/comment_list.html
--rw-rw-rw-   0        0        0     1281 2022-02-11 14:35:52.000000 xnote-web-0.0.9/handlers/note/ajax/edit_symbol_dialog.html
--rw-rw-rw-   0        0        0      134 2022-01-25 14:37:52.000000 xnote-web-0.0.9/handlers/note/ajax/group_detail_dialog.html
--rw-rw-rw-   0        0        0     3167 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/ajax/group_option_dialog.html
--rw-rw-rw-   0        0        0      407 2022-02-11 14:35:52.000000 xnote-web-0.0.9/handlers/note/ajax/option_dialog.html
--rw-rw-rw-   0        0        0       62 2022-02-11 14:35:52.000000 xnote-web-0.0.9/handlers/note/ajax/select_note_dialog.html
--rw-rw-rw-   0        0        0     1192 2022-03-12 15:02:09.000000 xnote-web-0.0.9/handlers/note/ajax/share_group_dialog.html
--rw-rw-rw-   0        0        0      726 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/ajax/share_note_dialog.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.934369 xnote-web-0.0.9/handlers/note/card/
--rw-rw-rw-   0        0        0      277 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/card/README.md
--rw-rw-rw-   0        0        0      939 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/hot_notes.html
--rw-rw-rw-   0        0        0      950 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/note_contents_left.html
--rw-rw-rw-   0        0        0      936 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/card/note_date_picker.html
--rw-rw-rw-   0        0        0      977 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/note_groups.html
--rw-rw-rw-   0        0        0      994 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/note_types.html
--rw-rw-rw-   0        0        0      128 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/card/plan_detail.html
--rw-rw-rw-   0        0        0      952 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/plan_note_card.html
--rw-rw-rw-   0        0        0      952 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/plan_sidebar.html
--rw-rw-rw-   0        0        0     1063 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/recent_created_notes.html
--rw-rw-rw-   0        0        0     1138 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/recent_update_groups.html
--rw-rw-rw-   0        0        0     1352 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/recent_update_notes.html
--rw-rw-rw-   0        0        0     1195 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/sticky_notes.html
--rw-rw-rw-   0        0        0     1096 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/card/task_memo.html
--rw-rw-rw-   0        0        0     8850 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/comment.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.993487 xnote-web-0.0.9/handlers/note/component/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:23.995979 xnote-web-0.0.9/handlers/note/component/attribute/
--rw-rw-rw-   0        0        0     1024 2022-07-17 10:20:13.000000 xnote-web-0.0.9/handlers/note/component/attribute/note_category.html
--rw-rw-rw-   0        0        0     2699 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/component/batch_move.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.001403 xnote-web-0.0.9/handlers/note/component/button/
--rw-rw-rw-   0        0        0      317 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/button/fixed_bottom_buttons.html
--rw-rw-rw-   0        0        0      199 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/button/fixed_buttons.html
--rw-rw-rw-   0        0        0      581 2022-07-14 14:34:40.000000 xnote-web-0.0.9/handlers/note/component/create_note_header.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.006879 xnote-web-0.0.9/handlers/note/component/css/
--rw-rw-rw-   0        0        0     1574 2022-04-04 06:46:25.000000 xnote-web-0.0.9/handlers/note/component/css/edit_css.html
--rw-rw-rw-   0        0        0      788 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/component/css/gallery_css.html
--rw-rw-rw-   0        0        0      818 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/detail_left.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.031800 xnote-web-0.0.9/handlers/note/component/editor/
--rw-rw-rw-   0        0        0      552 2022-04-19 15:15:43.000000 xnote-web-0.0.9/handlers/note/component/editor/editor_default_vars.html
--rw-rw-rw-   0        0        0     3141 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/component/editor/gallery.html
--rw-rw-rw-   0        0        0     6424 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/editor/markdown.html
--rw-rw-rw-   0        0        0    15648 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/editor/markdown_edit.html
--rw-rw-rw-   0        0        0     6150 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/editor/markdown_edit.mobile.html
--rw-rw-rw-   0        0        0     2051 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/component/editor/post.html
--rw-rw-rw-   0        0        0     1509 2022-04-01 14:26:37.000000 xnote-web-0.0.9/handlers/note/component/editor/table_lang.html
--rw-rw-rw-   0        0        0     2521 2022-04-04 15:50:05.000000 xnote-web-0.0.9/handlers/note/component/editor/table_myexcel.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.042504 xnote-web-0.0.9/handlers/note/component/filter/
--rw-rw-rw-   0        0        0      766 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/filter/group_tag_filter.html
--rw-rw-rw-   0        0        0      762 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/filter/note_tag_filter.html
--rw-rw-rw-   0        0        0      556 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/component/filter/type_filter.html
--rw-rw-rw-   0        0        0     1971 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/group_select.html
--rw-rw-rw-   0        0        0     3375 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/group_select_tree.html
--rw-rw-rw-   0        0        0       55 2022-04-22 14:59:54.000000 xnote-web-0.0.9/handlers/note/component/group_special_folder.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.048122 xnote-web-0.0.9/handlers/note/component/header/
--rw-rw-rw-   0        0        0     1096 2022-02-11 14:35:52.000000 xnote-web-0.0.9/handlers/note/component/header/common_header.html
--rw-rw-rw-   0        0        0      844 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/header/group_detail_header.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.050361 xnote-web-0.0.9/handlers/note/component/mobile/
--rw-rw-rw-   0        0        0      855 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/mobile/group_category_switch.html
--rw-rw-rw-   0        0        0     3460 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/mod_aside.html
--rw-rw-rw-   0        0        0      495 2022-06-26 11:06:28.000000 xnote-web-0.0.9/handlers/note/component/note_ext_info.html
--rw-rw-rw-   0        0        0     2899 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/note_list_component.html
--rw-rw-rw-   0        0        0      318 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/component/note_orderby.html
--rw-rw-rw-   0        0        0      668 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/note_orderby_select.html
--rw-rw-rw-   0        0        0      804 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/note_path.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.065155 xnote-web-0.0.9/handlers/note/component/option/
--rw-rw-rw-   0        0        0     1403 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/option/create_option.html
--rw-rw-rw-   0        0        0      756 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/note/component/option/group_option.html
--rw-rw-rw-   0        0        0     1303 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/option/group_option_dropdown.html
--rw-rw-rw-   0        0        0     5053 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/option/note_dropdown.html
--rw-rw-rw-   0        0        0      725 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/root_dropdown.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.104009 xnote-web-0.0.9/handlers/note/component/script/
--rw-rw-rw-   0        0        0      219 2022-01-25 14:37:52.000000 xnote-web-0.0.9/handlers/note/component/script/all_script.html
--rw-rw-rw-   0        0        0     2619 2022-07-15 06:43:03.000000 xnote-web-0.0.9/handlers/note/component/script/create_script.html
--rw-rw-rw-   0        0        0     1164 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/note/component/script/delete_script.html
--rw-rw-rw-   0        0        0     1513 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/script/group_select_script.html
--rw-rw-rw-   0        0        0      697 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/component/script/note_copy_script.html
--rw-rw-rw-   0        0        0     7434 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/script/note_option_script.html
--rw-rw-rw-   0        0        0      367 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/script/note_template.html
--rw-rw-rw-   0        0        0      125 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/script/orderby_script.html
--rw-rw-rw-   0        0        0      936 2022-03-07 15:10:58.000000 xnote-web-0.0.9/handlers/note/component/script/rename_script.html
--rw-rw-rw-   0        0        0     1443 2022-01-25 14:37:52.000000 xnote-web-0.0.9/handlers/note/component/script/share_script.html
--rw-rw-rw-   0        0        0      677 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/script/status_script.html
--rw-rw-rw-   0        0        0     3733 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/script/tag_manage_script.html
--rw-rw-rw-   0        0        0     2185 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/script/tag_script.html
--rw-rw-rw-   0        0        0     4092 2022-01-25 14:37:52.000000 xnote-web-0.0.9/handlers/note/component/share_dialog.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.123062 xnote-web-0.0.9/handlers/note/component/sidebar/
--rw-rw-rw-   0        0        0     1173 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/sidebar/group_list_sidebar.html
--rw-rw-rw-   0        0        0     1034 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/sidebar/group_manage_sidebar.html
--rw-rw-rw-   0        0        0     1672 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/sidebar/group_sidebar.html
--rw-rw-rw-   0        0        0     1370 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/sidebar/markdown_edit_sidebar.html
--rw-rw-rw-   0        0        0     1794 2024-01-27 06:07:10.000000 xnote-web-0.0.9/handlers/note/component/sidebar/note_sidebar.html
--rw-rw-rw-   0        0        0      324 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/sidebar/share_sidebar.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.126060 xnote-web-0.0.9/handlers/note/component/sort/
--rw-rw-rw-   0        0        0      694 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/sort/note_sort_tab.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.132331 xnote-web-0.0.9/handlers/note/component/timeline/
--rw-rw-rw-   0        0        0     4522 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/component/timeline/timeline_body.html
--rw-rw-rw-   0        0        0      716 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/timeline/timeline_create_option.html
--rw-rw-rw-   0        0        0     1794 2022-06-05 05:50:24.000000 xnote-web-0.0.9/handlers/note/component/view_css.html
--rw-rw-rw-   0        0        0      807 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/view_footer.html
--rw-rw-rw-   0        0        0     1368 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/component/view_header.html
--rw-rw-rw-   0        0        0     1798 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/component/view_header_tag.html
--rw-rw-rw-   0        0        0     1672 2022-03-12 01:39:04.000000 xnote-web-0.0.9/handlers/note/constant.py
--rw-rw-rw-   0        0        0    62424 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/dao.py
--rw-rw-rw-   0        0        0     2162 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/dao_api.py
--rw-rw-rw-   0        0        0     2532 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/dao_book.py
--rw-rw-rw-   0        0        0     1276 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/dao_category.py
--rw-rw-rw-   0        0        0     6741 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/dao_comment.py
--rw-rw-rw-   0        0        0     2140 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/dao_delete.py
--rw-rw-rw-   0        0        0     3383 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/dao_draft.py
--rw-rw-rw-   0        0        0      687 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/note/dao_edit.py
--rw-rw-rw-   0        0        0     8364 2023-11-05 02:18:54.000000 xnote-web-0.0.9/handlers/note/dao_log.py
--rw-rw-rw-   0        0        0      879 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/dao_read.py
--rw-rw-rw-   0        0        0     4314 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/dao_share.py
--rw-rw-rw-   0        0        0    12681 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/dao_tag.py
--rw-rw-rw-   0        0        0    11086 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/html_importer.py
--rw-rw-rw-   0        0        0     2397 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/note_api.py
--rw-rw-rw-   0        0        0      487 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/note_calendar.py
--rw-rw-rw-   0        0        0     2934 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/note/note_category.py
--rw-rw-rw-   0        0        0     1381 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/note_checklist.py
--rw-rw-rw-   0        0        0    28876 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/note_edit.py
--rw-rw-rw-   0        0        0      491 2022-07-09 01:18:05.000000 xnote-web-0.0.9/handlers/note/note_fix.py
--rw-rw-rw-   0        0        0    31590 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/note_group.py
--rw-rw-rw-   0        0        0     1005 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/note_helper.py
--rw-rw-rw-   0        0        0     3144 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/note_stat.py
--rw-rw-rw-   0        0        0     8581 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/note_tag.py
--rw-rw-rw-   0        0        0    21187 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/note_timeline.py
--rw-rw-rw-   0        0        0    16587 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/note_view.py
--rw-rw-rw-   0        0        0     4669 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/note_workspace.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.212965 xnote-web-0.0.9/handlers/note/page/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.229150 xnote-web-0.0.9/handlers/note/page/batch/
--rw-rw-rw-   0        0        0      553 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/page/batch/gallery_manage.html
--rw-rw-rw-   0        0        0     7504 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/page/batch/group_manage.html
--rw-rw-rw-   0        0        0      632 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/note/page/batch/group_manage_category.html
--rw-rw-rw-   0        0        0     5580 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/batch/note_manage.html
--rw-rw-rw-   0        0        0      774 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/page/category.html
--rw-rw-rw-   0        0        0     5298 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/comment.html
--rw-rw-rw-   0        0        0      431 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/note/page/comment_user_page.html
--rw-rw-rw-   0        0        0     5726 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/create.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.254805 xnote-web-0.0.9/handlers/note/page/detail/
--rw-rw-rw-   0        0        0     2152 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/detail/checklist_detail.html
--rw-rw-rw-   0        0        0     2452 2023-04-06 04:04:41.000000 xnote-web-0.0.9/handlers/note/page/detail/form_detail.html
--rw-rw-rw-   0        0        0     1261 2024-03-16 14:56:18.000000 xnote-web-0.0.9/handlers/note/page/detail/group_detail.html
--rw-rw-rw-   0        0        0     1169 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/note/page/detail/group_detail_body.html
--rw-rw-rw-   0        0        0     1715 2023-04-06 04:04:41.000000 xnote-web-0.0.9/handlers/note/page/detail/note_detail.html
--rw-rw-rw-   0        0        0     5694 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/detail/table_detail.html
--rw-rw-rw-   0        0        0     1503 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/note/page/group_list.html
--rw-rw-rw-   0        0        0      764 2023-12-16 03:36:03.000000 xnote-web-0.0.9/handlers/note/page/group_list_nav_desktop.html
--rw-rw-rw-   0        0        0      862 2023-12-16 03:36:03.000000 xnote-web-0.0.9/handlers/note/page/group_list_nav_mobile.html
--rw-rw-rw-   0        0        0     1708 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/history_list.html
--rw-rw-rw-   0        0        0     4262 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/html_importer.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.270853 xnote-web-0.0.9/handlers/note/page/index/
--rw-rw-rw-   0        0        0      971 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/page/index/note_index.html
--rw-rw-rw-   0        0        0     1278 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/index/note_workspace.html
--rw-rw-rw-   0        0        0      907 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/index/note_workspace.mobile.html
--rw-rw-rw-   0        0        0     1008 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/page/index/note_workspace2.html
--rw-rw-rw-   0        0        0     3604 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/list_by_date.html
--rw-rw-rw-   0        0        0    12731 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/note_calendar.html
--rw-rw-rw-   0        0        0      606 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/note_default.html
--rw-rw-rw-   0        0        0     1426 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/note_list.html
--rw-rw-rw-   0        0        0     1508 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/note_recent.html
--rw-rw-rw-   0        0        0     2003 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/note/page/note_share.html
--rw-rw-rw-   0        0        0     1292 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/note_tools.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.300562 xnote-web-0.0.9/handlers/note/page/old/
--rw-rw-rw-   0        0        0      740 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/old/category_old.html
--rw-rw-rw-   0        0        0     1425 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/note/page/old/create_log.html
--rw-rw-rw-   0        0        0      807 2022-06-18 00:42:54.000000 xnote-web-0.0.9/handlers/note/page/old/group_list_archived.html
--rw-rw-rw-   0        0        0     2324 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/old/list_by_date_old.html
--rw-rw-rw-   0        0        0       92 2022-01-25 14:37:52.000000 xnote-web-0.0.9/handlers/note/page/old/notice.html
--rw-rw-rw-   0        0        0     4194 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/old/project_list_old.html
--rw-rw-rw-   0        0        0     2150 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/old/upload_file.html
--rw-rw-rw-   0        0        0     1267 2023-04-06 04:04:41.000000 xnote-web-0.0.9/handlers/note/page/print.html
--rw-rw-rw-   0        0        0     1286 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/note/page/taglist.html
--rw-rw-rw-   0        0        0      783 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/note/page/tagname.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.305569 xnote-web-0.0.9/handlers/note/page/timeline/
--rw-rw-rw-   0        0        0     1902 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/note/page/timeline/timeline.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.316146 xnote-web-0.0.9/handlers/plan/
--rw-rw-rw-   0        0        0        0 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/plan/__init__.py
--rw-rw-rw-   0        0        0     2118 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plan/dao.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.319384 xnote-web-0.0.9/handlers/plan/page/
--rw-rw-rw-   0        0        0     3773 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plan/page/month_plan.html
--rw-rw-rw-   0        0        0     3641 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.340737 xnote-web-0.0.9/handlers/plugin/
--rw-rw-rw-   0        0        0      123 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/plugin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.355411 xnote-web-0.0.9/handlers/plugin/base/
--rw-rw-rw-   0        0        0     2051 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/plugin/base/base_form_plugin.html
--rw-rw-rw-   0        0        0     1118 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/plugin/base/base_plugin.html
--rw-rw-rw-   0        0        0      510 2022-06-19 09:05:51.000000 xnote-web-0.0.9/handlers/plugin/base/base_plugin_body.html
--rw-rw-rw-   0        0        0     2228 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plugin/base/base_plugin_title.html
--rw-rw-rw-   0        0        0     3037 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plugin/dao.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.367170 xnote-web-0.0.9/handlers/plugin/header/
--rw-rw-rw-   0        0        0      818 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/plugin/header/plugin_category.html
--rw-rw-rw-   0        0        0      930 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/plugin/header/plugin_header_normal.html
--rw-rw-rw-   0        0        0      254 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/plugin/header/plugin_header_note.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.384377 xnote-web-0.0.9/handlers/plugin/page/
--rw-rw-rw-   0        0        0      999 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/plugin/page/grid.html
--rw-rw-rw-   0        0        0     4756 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/plugin/page/plugins_v1.html
--rw-rw-rw-   0        0        0     1677 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/plugin/page/plugins_v2.html
--rw-rw-rw-   0        0        0     1341 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/plugin/page/plugins_v3.html
--rw-rw-rw-   0        0        0     3969 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plugin/plugin_create.py
--rw-rw-rw-   0        0        0    28433 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plugin/plugin_page.py
--rw-rw-rw-   0        0        0     1812 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/plugin/plugin_upload.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.437292 xnote-web-0.0.9/handlers/search/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/search/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.445292 xnote-web-0.0.9/handlers/search/ajax/
--rw-rw-rw-   0        0        0      641 2022-02-11 14:35:52.000000 xnote-web-0.0.9/handlers/search/ajax/search_dialog.html
--rw-rw-rw-   0        0        0      977 2022-02-11 14:35:52.000000 xnote-web-0.0.9/handlers/search/ajax/search_dialog_detail.html
--rw-rw-rw-   0        0        0     1364 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/search/api.py
--rw-rw-rw-   0        0        0      958 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/search/calc.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.457284 xnote-web-0.0.9/handlers/search/component/
--rw-rw-rw-   0        0        0     1367 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/search/component/search_pagination.html
--rw-rw-rw-   0        0        0     1034 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/search/component/search_sidebar.html
--rw-rw-rw-   0        0        0     2172 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/search/component/search_tab.html
--rw-rw-rw-   0        0        0     3278 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/search/dictionary.py
--rw-rw-rw-   0        0        0      910 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/search/mute.py
--rw-rw-rw-   0        0        0     1428 2022-03-10 14:02:41.000000 xnote-web-0.0.9/handlers/search/note.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.466289 xnote-web-0.0.9/handlers/search/page/
--rw-rw-rw-   0        0        0     1967 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/search/page/search_history.html
--rw-rw-rw-   0        0        0     5839 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/search/page/search_result.html
--rw-rw-rw-   0        0        0      617 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/search/pydoc.py
--rw-rw-rw-   0        0        0     2905 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/search/reminder.py
--rw-rw-rw-   0        0        0     1778 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/search/scripts.py
--rw-rw-rw-   0        0        0     1245 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/search/search.html
--rw-rw-rw-   0        0        0    18128 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/search/search.py
--rw-rw-rw-   0        0        0      440 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/search/search_aside.html
--rw-rw-rw-   0        0        0     1874 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/search/search_rules.html
--rw-rw-rw-   0        0        0     2878 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/search/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.473495 xnote-web-0.0.9/handlers/settings/
--rw-rw-rw-   0        0        0      123 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.488936 xnote-web-0.0.9/handlers/settings/component/
--rw-rw-rw-   0        0        0     2855 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/settings/component/admin_settings.html
--rw-rw-rw-   0        0        0     4751 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/settings/component/note_settings.html
--rw-rw-rw-   0        0        0     1278 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/settings/component/search_settings.html
--rw-rw-rw-   0        0        0      868 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/settings/component/settings_sidebar.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.495999 xnote-web-0.0.9/handlers/settings/page/
--rw-rw-rw-   0        0        0     1951 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/settings/page/properties.html
--rw-rw-rw-   0        0        0     2097 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/settings/page/settings.html
--rw-rw-rw-   0        0        0     7109 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/settings/settings.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.605024 xnote-web-0.0.9/handlers/system/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/system/__init__.py
--rw-rw-rw-   0        0        0    14847 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/backup.py
--rw-rw-rw-   0        0        0     2773 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/cache_admin.py
--rw-rw-rw-   0        0        0     4849 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/clipboard.py
--rw-rw-rw-   0        0        0     3628 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/system/command.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.631862 xnote-web-0.0.9/handlers/system/component/
--rw-rw-rw-   0        0        0     1425 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/component/admin_nav.html
--rw-rw-rw-   0        0        0      979 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/component/db_kv_nav.html
--rw-rw-rw-   0        0        0     1051 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/component/db_nav.html
--rw-rw-rw-   0        0        0      463 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/system/component/system_css.html
--rw-rw-rw-   0        0        0      597 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/component/system_log_tab.html
--rw-rw-rw-   0        0        0     1445 2022-07-02 01:04:41.000000 xnote-web-0.0.9/handlers/system/component/system_sync_cluster_info.html
--rw-rw-rw-   0        0        0     3450 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/component/system_sync_follower_view.html
--rw-rw-rw-   0        0        0      564 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/component/thread_nav.html
--rw-rw-rw-   0        0        0     6894 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/crontab.py
--rw-rw-rw-   0        0        0    19523 2024-03-23 04:03:30.000000 xnote-web-0.0.9/handlers/system/db_admin.py
--rw-rw-rw-   0        0        0     3959 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/db_index.py
--rw-rw-rw-   0        0        0     8098 2023-10-21 00:22:22.000000 xnote-web-0.0.9/handlers/system/db_migrate_tools.py
--rw-rw-rw-   0        0        0     1808 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/db_refresh.py
--rw-rw-rw-   0        0        0     3968 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/db_shell.py
--rw-rw-rw-   0        0        0     1132 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/db_upgrade.py
--rw-rw-rw-   0        0        0      534 2022-05-06 04:45:28.000000 xnote-web-0.0.9/handlers/system/develop_controller.py
--rw-rw-rw-   0        0        0     1697 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/handler_profile.py
--rw-rw-rw-   0        0        0     1823 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/mod_aside.html
--rw-rw-rw-   0        0        0      567 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/network_profile.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.686404 xnote-web-0.0.9/handlers/system/page/
--rw-rw-rw-   0        0        0     2797 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/cache_admin.html
--rw-rw-rw-   0        0        0     2586 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/page/crontab.html
--rw-rw-rw-   0        0        0     2259 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/system/page/crontab_edit.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.722136 xnote-web-0.0.9/handlers/system/page/db/
--rw-rw-rw-   0        0        0     6102 2024-03-23 04:04:13.000000 xnote-web-0.0.9/handlers/system/page/db/db_admin.html
--rw-rw-rw-   0        0        0     2055 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/page/db/db_backup.html
--rw-rw-rw-   0        0        0     2555 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/db/db_index.html
--rw-rw-rw-   0        0        0     1192 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/page/db/db_index_v2.html
--rw-rw-rw-   0        0        0     2342 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/page/db/db_meta.html
--rw-rw-rw-   0        0        0     1557 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/db/db_struct.html
--rw-rw-rw-   0        0        0      649 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/db/driver_info.html
--rw-rw-rw-   0        0        0     1091 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/page/db/sqldb_detail.html
--rw-rw-rw-   0        0        0     1412 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/page/db/sqldb_list.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.728134 xnote-web-0.0.9/handlers/system/page/develop/
--rw-rw-rw-   0        0        0        0 2022-05-06 04:45:10.000000 xnote-web-0.0.9/handlers/system/page/develop/component_demo.html
--rw-rw-rw-   0        0        0      902 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/develop/index.html
--rw-rw-rw-   0        0        0      931 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/system/page/history.html
--rw-rw-rw-   0        0        0     1726 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/page/module_detail.html
--rw-rw-rw-   0        0        0     1046 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/page/module_list.html
--rw-rw-rw-   0        0        0     5954 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/page/script.html
--rw-rw-rw-   0        0        0     2949 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/sqlite.html
--rw-rw-rw-   0        0        0      651 2022-06-18 13:08:01.000000 xnote-web-0.0.9/handlers/system/page/system_admin.html
--rw-rw-rw-   0        0        0     2661 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/page/system_index.html
--rw-rw-rw-   0        0        0     2291 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/system_info.html
--rw-rw-rw-   0        0        0      651 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/system/page/system_info_text.html
--rw-rw-rw-   0        0        0     4173 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/system_sync.html
--rw-rw-rw-   0        0        0      590 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/page/template_cache.html
--rw-rw-rw-   0        0        0     1360 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/page/thread_info.html
--rw-rw-rw-   0        0        0     6736 2023-03-04 06:34:27.000000 xnote-web-0.0.9/handlers/system/script.py
--rw-rw-rw-   0        0        0     3566 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/stats.py
--rw-rw-rw-   0        0        0     7998 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system.py
--rw-rw-rw-   0        0        0      708 2022-04-03 14:17:05.000000 xnote-web-0.0.9/handlers/system/system_boot.py
--rw-rw-rw-   0        0        0     2513 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/system_event.py
--rw-rw-rw-   0        0        0     5213 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/system_info.py
--rw-rw-rw-   0        0        0     7523 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_log.py
--rw-rw-rw-   0        0        0     4428 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/system_module.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.753387 xnote-web-0.0.9/handlers/system/system_sync/
--rw-rw-rw-   0        0        0      772 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/system_sync/models.py
--rw-rw-rw-   0        0        0     1386 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_sync/node_base.py
--rw-rw-rw-   0        0        0    19983 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_sync/node_follower.py
--rw-rw-rw-   0        0        0     9517 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_sync/node_leader.py
--rw-rw-rw-   0        0        0    12355 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_sync/system_sync_controller.py
--rw-rw-rw-   0        0        0     7071 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_sync/system_sync_indexer.py
--rw-rw-rw-   0        0        0    10245 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/system/system_sync/system_sync_proxy.py
--rw-rw-rw-   0        0        0      444 2023-04-06 15:44:02.000000 xnote-web-0.0.9/handlers/system/system_todo.py
--rw-rw-rw-   0        0        0      676 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/system/template_cache.py
--rw-rw-rw-   0        0        0      848 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/system/thread_info.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.767585 xnote-web-0.0.9/handlers/test/
--rw-rw-rw-   0        0        0      128 2022-01-25 14:37:52.000000 xnote-web-0.0.9/handlers/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.771912 xnote-web-0.0.9/handlers/test/component/
--rw-rw-rw-   0        0        0     1034 2024-03-31 03:24:19.000000 xnote-web-0.0.9/handlers/test/component/example_nav.html
--rw-rw-rw-   0        0        0      193 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/test/exception.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.792356 xnote-web-0.0.9/handlers/test/page/
--rw-rw-rw-   0        0        0      697 2022-06-26 11:21:01.000000 xnote-web-0.0.9/handlers/test/page/example_btn.html
--rw-rw-rw-   0        0        0     1378 2022-05-07 14:15:21.000000 xnote-web-0.0.9/handlers/test/page/example_dialog.html
--rw-rw-rw-   0        0        0      866 2022-03-13 13:50:59.000000 xnote-web-0.0.9/handlers/test/page/example_dropdown.html
--rw-rw-rw-   0        0        0     1537 2022-04-17 03:52:32.000000 xnote-web-0.0.9/handlers/test/page/example_hammer.html
--rw-rw-rw-   0        0        0      102 2022-03-11 12:10:15.000000 xnote-web-0.0.9/handlers/test/page/example_index.html
--rw-rw-rw-   0        0        0     1707 2022-03-13 13:45:19.000000 xnote-web-0.0.9/handlers/test/page/example_tab.html
--rw-rw-rw-   0        0        0     1032 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/test/page/example_tag.html
--rw-rw-rw-   0        0        0     1679 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/test/test_dbutil_handler.py
--rw-rw-rw-   0        0        0      977 2024-03-31 06:02:23.000000 xnote-web-0.0.9/handlers/test/test_handler.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.906021 xnote-web-0.0.9/handlers/tools/
--rw-rw-rw-   0        0        0      105 2022-04-17 09:04:15.000000 xnote-web-0.0.9/handlers/tools/__init__.py
--rw-rw-rw-   0        0        0     2198 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/barcode.html
--rw-rw-rw-   0        0        0     1035 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/tools/base64.html
--rw-rw-rw-   0        0        0      371 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/base_title.html
--rw-rw-rw-   0        0        0     3539 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/tools/browser_info.html
--rw-rw-rw-   0        0        0     4077 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/camera.html
--rw-rw-rw-   0        0        0     1353 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/chat_demo.html
--rw-rw-rw-   0        0        0    10087 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/code_template.html
--rw-rw-rw-   0        0        0     3818 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/color.html
--rw-rw-rw-   0        0        0     1486 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/datetime.html
--rw-rw-rw-   0        0        0     5346 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/tools/hex.html
--rw-rw-rw-   0        0        0      426 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/iframe_viewer.html
--rw-rw-rw-   0        0        0     6029 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/img2gray.html
--rw-rw-rw-   0        0        0     7694 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/img_merge.html
--rw-rw-rw-   0        0        0     6002 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/img_split.html
--rw-rw-rw-   0        0        0      619 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/md5.html
--rw-rw-rw-   0        0        0     4769 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/tools/multi_win.html
--rw-rw-rw-   0        0        0     3033 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/notebook.html
--rw-rw-rw-   0        0        0      342 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/notebook.py
--rw-rw-rw-   0        0        0     2101 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/port_scanner.py
--rw-rw-rw-   0        0        0     1020 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/qrcode.html
--rw-rw-rw-   0        0        0     2424 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/random_string.html
--rw-rw-rw-   0        0        0     1000 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/responsive.html
--rw-rw-rw-   0        0        0     4119 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/tools/runjs.html
--rw-rw-rw-   0        0        0     1224 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/search_compare.html
--rw-rw-rw-   0        0        0      774 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/tools/sha1.html
--rw-rw-rw-   0        0        0     1937 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/tools/shell.html
--rw-rw-rw-   0        0        0     3906 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/speech_recognition.html
--rw-rw-rw-   0        0        0      896 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/tools/tcc.html
--rw-rw-rw-   0        0        0     1409 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/tools/terminal.html
--rw-rw-rw-   0        0        0     8164 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/tools/text_convert.html
--rw-rw-rw-   0        0        0     3732 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/tools/text_diff.html
--rw-rw-rw-   0        0        0     3297 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/text_set.html
--rw-rw-rw-   0        0        0     1011 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/tools.py
--rw-rw-rw-   0        0        0      487 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/tts.html
--rw-rw-rw-   0        0        0     1249 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/tools/urlcoder.html
--rw-rw-rw-   0        0        0     7610 2022-11-26 16:30:19.000000 xnote-web-0.0.9/handlers/tools/vue_test.html
--rw-rw-rw-   0        0        0     5326 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/tools/webuploader.html
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.919655 xnote-web-0.0.9/handlers/user/
--rw-rw-rw-   0        0        0      287 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/user/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.923310 xnote-web-0.0.9/handlers/user/component/
--rw-rw-rw-   0        0        0     1241 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/user/component/user_script.html
--rw-rw-rw-   0        0        0      347 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/user/dao.py
--rw-rw-rw-   0        0        0     4949 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/user/login.py
--rw-rw-rw-   0        0        0      255 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/user/logout.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.943400 xnote-web-0.0.9/handlers/user/page/
--rw-rw-rw-   0        0        0     1516 2023-04-06 15:52:08.000000 xnote-web-0.0.9/handlers/user/page/change_password.html
--rw-rw-rw-   0        0        0     3357 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/user/page/login.html
--rw-rw-rw-   0        0        0      912 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/user/page/user.html
--rw-rw-rw-   0        0        0     3551 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/user/page/user_list.html
--rw-rw-rw-   0        0        0     2440 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/user/page/user_manage.html
--rw-rw-rw-   0        0        0      802 2023-10-27 13:17:40.000000 xnote-web-0.0.9/handlers/user/page/user_op_log.html
--rw-rw-rw-   0        0        0     1522 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/user/page/userinfo.html
--rw-rw-rw-   0        0        0     6400 2024-03-16 14:56:19.000000 xnote-web-0.0.9/handlers/user/user.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.950338 xnote-web-0.0.9/handlers/webdav/
--rw-rw-rw-   0        0        0      123 2021-10-01 10:27:00.000000 xnote-web-0.0.9/handlers/webdav/__init__.py
--rw-rw-rw-   0        0        0     5704 2023-06-30 12:24:59.000000 xnote-web-0.0.9/handlers/webdav/webdav.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:24.972929 xnote-web-0.0.9/lib/
--rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.0.9/lib/__init__.py
--rw-rw-rw-   0        0        0    33040 2022-05-22 05:10:24.000000 xnote-web-0.0.9/lib/html2text.py
--rw-rw-rw-   0        0        0   451584 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/leveldb-x64.dll
--rw-rw-rw-   0        0        0   367104 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/leveldb.dll
--rw-rw-rw-   0        0        0    37736 2023-10-27 13:17:40.000000 xnote-web-0.0.9/lib/leveldbpy.py
--rw-rw-rw-   0        0        0     6529 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/smallseg.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.023849 xnote-web-0.0.9/lib/web/
--rw-rw-rw-   0        0        0      754 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/__init__.py
--rw-rw-rw-   0        0        0    25946 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/application.py
--rw-rw-rw-   0        0        0     8714 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/browser.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.028578 xnote-web-0.0.9/lib/web/contrib/
--rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/contrib/__init__.py
--rw-rw-rw-   0        0        0     3457 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/contrib/template.py
--rw-rw-rw-   0        0        0    56068 2023-12-02 10:30:00.000000 xnote-web-0.0.9/lib/web/db.py
--rw-rw-rw-   0        0        0    13157 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/debugerror.py
--rw-rw-rw-   0        0        0    13983 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/form.py
--rw-rw-rw-   0        0        0     4619 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/http.py
--rw-rw-rw-   0        0        0    13278 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/httpserver.py
--rw-rw-rw-   0        0        0     6507 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/net.py
--rw-rw-rw-   0        0        0      877 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/py3helpers.py
--rw-rw-rw-   0        0        0    10921 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/session.py
--rw-rw-rw-   0        0        0    49690 2022-11-26 16:30:19.000000 xnote-web-0.0.9/lib/web/template.py
--rw-rw-rw-   0        0        0     2261 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/test.py
--rw-rw-rw-   0        0        0    42559 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/utils.py
--rw-rw-rw-   0        0        0    17704 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/webapi.py
--rw-rw-rw-   0        0        0     3707 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/webopenid.py
--rw-rw-rw-   0        0        0     2452 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.046205 xnote-web-0.0.9/lib/web/wsgiserver/
--rw-rw-rw-   0        0        0     1542 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/wsgiserver/LICENSE.txt
--rw-rw-rw-   0        0        0      580 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/wsgiserver/__init__.py
--rw-rw-rw-   0        0        0     4032 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/wsgiserver/ssl_builtin.py
--rw-rw-rw-   0        0        0     9223 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/wsgiserver/ssl_pyopenssl.py
--rw-rw-rw-   0        0        0    89663 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/web/wsgiserver/wsgiserver2.py
--rw-rw-rw-   0        0        0    79905 2022-02-26 02:25:16.000000 xnote-web-0.0.9/lib/web/wsgiserver/wsgiserver3.py
--rw-rw-rw-   0        0        0    22355 2021-10-01 10:27:00.000000 xnote-web-0.0.9/lib/wget.py
--rw-rw-rw-   0        0        0       42 2024-03-31 06:48:26.390029 xnote-web-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      985 2024-03-31 06:47:45.000000 xnote-web-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.060101 xnote-web-0.0.9/static/
--rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.063101 xnote-web-0.0.9/static/audio/
--rw-rw-rw-   0        0        0    26675 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/audio/todo_done.mp3
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.099488 xnote-web-0.0.9/static/css/
--rw-rw-rw-   0        0        0    83723 2024-03-17 03:21:24.000000 xnote-web-0.0.9/static/css/app.build.css
--rw-rw-rw-   0        0        0     1926 2024-03-16 14:56:19.000000 xnote-web-0.0.9/static/css/app.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.142054 xnote-web-0.0.9/static/css/base/
--rw-rw-rw-   0        0        0     3150 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/css/base/common-button.css
--rw-rw-rw-   0        0        0      273 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/css/base/common-dialog.css
--rw-rw-rw-   0        0        0     1570 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/css/base/common-dropdown.css
--rw-rw-rw-   0        0        0     2212 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/base/common-icon.css
--rw-rw-rw-   0        0        0     1476 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/css/base/common-layout.css
--rw-rw-rw-   0        0        0      651 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/base/common-markdown.css
--rw-rw-rw-   0        0        0     1312 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/css/base/common-mobile.css
--rw-rw-rw-   0        0        0      927 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/css/base/common-page.css
--rw-rw-rw-   0        0        0      603 2023-04-16 02:40:01.000000 xnote-web-0.0.9/static/css/base/common-photo.css
--rw-rw-rw-   0        0        0     2241 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/css/base/common-tab.css
--rw-rw-rw-   0        0        0     2137 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/css/base/common-tag.css
--rw-rw-rw-   0        0        0    18296 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/css/base/common.css
--rw-rw-rw-   0        0        0      424 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/css/base/layout-second-nav.css
--rw-rw-rw-   0        0        0      368 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/css/base/reset-wide.css
--rw-rw-rw-   0        0        0     2609 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/css/base/reset.css
--rw-rw-rw-   0        0        0     1795 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/css/common-card.css
--rw-rw-rw-   0        0        0     3943 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/common-left.css
--rw-rw-rw-   0        0        0      802 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/common-react.css
--rw-rw-rw-   0        0        0    31004 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0     4476 2023-06-30 12:24:59.000000 xnote-web-0.0.9/static/css/message.css
--rw-rw-rw-   0        0        0     5431 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/css/note.css
--rw-rw-rw-   0        0        0      704 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/plugins.css
--rw-rw-rw-   0        0        0      269 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/search.css
--rw-rw-rw-   0        0        0     2066 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/css/timeline.css
--rw-rw-rw-   0        0        0     1286 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/css/todo.css
--rw-rw-rw-   0        0        0    16958 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/favicon.ico
--rw-rw-rw-   0        0        0    16372 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/favicon.png
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.149055 xnote-web-0.0.9/static/fonts/
--rw-rw-rw-   0        0        0    83588 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    66624 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.224562 xnote-web-0.0.9/static/image/
--rw-rw-rw-   0        0        0     1277 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/checked.png
--rw-rw-rw-   0        0        0     2593 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/file.png
--rw-rw-rw-   0        0        0      985 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/file2.png
--rw-rw-rw-   0        0        0      120 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/folder.gif
--rw-rw-rw-   0        0        0      340 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/folder2.png
--rw-rw-rw-   0        0        0     5696 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/folder3.png
--rw-rw-rw-   0        0        0      496 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_application.png
--rw-rw-rw-   0        0        0      956 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_application.svg
--rw-rw-rw-   0        0        0      128 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_csv.png
--rw-rw-rw-   0        0        0     1493 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_dict.png
--rw-rw-rw-   0        0        0      838 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_dict.svg
--rw-rw-rw-   0        0        0      465 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_folder_settings.png
--rw-rw-rw-   0        0        0     1024 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_recent.png
--rw-rw-rw-   0        0        0     1359 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_recent.svg
--rw-rw-rw-   0        0        0      696 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_right.png
--rw-rw-rw-   0        0        0      821 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_script.png
--rw-rw-rw-   0        0        0     1890 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_script.svg
--rw-rw-rw-   0        0        0     1194 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_search.png
--rw-rw-rw-   0        0        0     1122 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_search.svg
--rw-rw-rw-   0        0        0      958 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_settings_applications.png
--rw-rw-rw-   0        0        0     2120 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_settings_applications.svg
--rw-rw-rw-   0        0        0     1353 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_shell.png
--rw-rw-rw-   0        0        0      743 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_shell.svg
--rw-rw-rw-   0        0        0     2901 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icon_txt.png
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.237241 xnote-web-0.0.9/static/image/icons/
--rw-rw-rw-   0        0        0     1707 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icons/icon_barcode.png
--rw-rw-rw-   0        0        0     3158 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icons/icon_game.png
--rw-rw-rw-   0        0        0     5203 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icons/icon_network.png
--rw-rw-rw-   0        0        0     1375 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/image/icons/icon_work.png
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.278034 xnote-web-0.0.9/static/js/
--rw-rw-rw-   0        0        0     2294 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/Lexer.js
--rw-rw-rw-   0        0        0      657 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/admin.js
--rw-rw-rw-   0        0        0   102892 2024-03-31 06:06:00.000000 xnote-web-0.0.9/static/js/app.build.js
--rw-rw-rw-   0        0        0     7644 2023-06-30 12:24:59.000000 xnote-web-0.0.9/static/js/app.js
--rw-rw-rw-   0        0        0      472 2023-06-30 12:24:59.000000 xnote-web-0.0.9/static/js/autocss.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.297783 xnote-web-0.0.9/static/js/base/
--rw-rw-rw-   0        0        0     1309 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/base/ajax.js
--rw-rw-rw-   0        0        0     4375 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/base/array.js
--rw-rw-rw-   0        0        0      726 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/base/datetime.js
--rw-rw-rw-   0        0        0      731 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/base/jq-ext.js
--rw-rw-rw-   0        0        0      580 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/base/misc.js
--rw-rw-rw-   0        0        0     8338 2023-12-02 11:08:59.000000 xnote-web-0.0.9/static/js/base/string.js
--rw-rw-rw-   0        0        0     3173 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/base/url.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.300236 xnote-web-0.0.9/static/js/codemirror-addon/
--rw-rw-rw-   0        0        0    11711 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/codemirror-addon/xnote-search.js
--rw-rw-rw-   0        0        0    21933 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/colors.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.304253 xnote-web-0.0.9/static/js/components/
--rw-rw-rw-   0        0        0      786 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/components/date-picker.js
--rw-rw-rw-   0        0        0     7614 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/console.js
--rw-rw-rw-   0        0        0     2706 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/editor-csv.js
--rw-rw-rw-   0        0        0     9949 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/editor.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.306993 xnote-web-0.0.9/static/js/fs/
--rw-rw-rw-   0        0        0     1607 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/fs/fs.js
--rw-rw-rw-   0        0        0    16458 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/marked-ext.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.309588 xnote-web-0.0.9/static/js/message/
--rw-rw-rw-   0        0        0    11638 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/message/message.js
--rw-rw-rw-   0        0        0    15989 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/note.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.316291 xnote-web-0.0.9/static/js/old/
--rw-rw-rw-   0        0        0     5071 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/old/TagEditor.js
--rw-rw-rw-   0        0        0     2489 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/old/fileEditor.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.319518 xnote-web-0.0.9/static/js/plan/
--rw-rw-rw-   0        0        0     2543 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/plan/plan.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.322959 xnote-web-0.0.9/static/js/plugin/
--rw-rw-rw-   0        0        0     1811 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/plugin/plugin.form.js
--rw-rw-rw-   0        0        0     4091 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/upload.js
--rw-rw-rw-   0        0        0    14750 2023-12-02 11:09:33.000000 xnote-web-0.0.9/static/js/utils.build.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.373295 xnote-web-0.0.9/static/js/xnote-ui/
--rw-rw-rw-   0        0        0    11058 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/layer.photos.js
--rw-rw-rw-   0        0        0      703 2023-06-30 12:24:59.000000 xnote-web-0.0.9/static/js/xnote-ui/x-audio.js
--rw-rw-rw-   0        0        0      190 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-core.js
--rw-rw-rw-   0        0        0     2072 2023-04-16 02:40:01.000000 xnote-web-0.0.9/static/js/xnote-ui/x-device.js
--rw-rw-rw-   0        0        0    15513 2024-03-31 06:06:00.000000 xnote-web-0.0.9/static/js/xnote-ui/x-dialog.js
--rw-rw-rw-   0        0        0     3063 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-dropdown.js
--rw-rw-rw-   0        0        0     4092 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-event.js
--rw-rw-rw-   0        0        0      327 2023-06-30 12:24:59.000000 xnote-web-0.0.9/static/js/xnote-ui/x-ext.js
--rw-rw-rw-   0        0        0     8478 2024-03-16 14:56:20.000000 xnote-web-0.0.9/static/js/xnote-ui/x-init.js
--rw-rw-rw-   0        0        0      674 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-layout.js
--rw-rw-rw-   0        0        0     1365 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-photo.js
--rw-rw-rw-   0        0        0     1962 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-tab.js
--rw-rw-rw-   0        0        0     1257 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/js/xnote-ui/x-template.js
--rw-rw-rw-   0        0        0     8558 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/js/xnote-ui/x-upload.js
--rw-rw-rw-   0        0        0     3590 2023-06-30 12:24:59.000000 xnote-web-0.0.9/static/js/xnote-ui/x-url.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.391937 xnote-web-0.0.9/static/lib/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.395928 xnote-web-0.0.9/static/lib/JsBarcode/
--rw-rw-rw-   0        0        0    61195 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/JsBarcode/JsBarcode.all.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.399047 xnote-web-0.0.9/static/lib/art-template/
--rw-rw-rw-   0        0        0    17325 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/art-template/template-web-4.13.2.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.402634 xnote-web-0.0.9/static/lib/base64.js/
--rw-rw-rw-   0        0        0     2280 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/base64.js/base64.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.406420 xnote-web-0.0.9/static/lib/bootstrap/
--rw-rw-rw-   0        0        0   122544 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/bootstrap/bootstrap-3.3.5.min.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.411036 xnote-web-0.0.9/static/lib/clipboard/
--rw-rw-rw-   0        0        0    10760 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/clipboard/clipboard-2.0.4.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.418304 xnote-web-0.0.9/static/lib/codemirror/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.425741 xnote-web-0.0.9/static/lib/codemirror/5.41.0/
--rw-rw-rw-   0        0        0     5920 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/5.41.0/codemirror.min.css
--rw-rw-rw-   0        0        0   167495 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/codemirror/5.41.0/codemirror.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.434103 xnote-web-0.0.9/static/lib/codemirror/5.65.12/
--rw-rw-rw-   0        0        0     9064 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/5.65.12/codemirror.css
--rw-rw-rw-   0        0        0   411661 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/5.65.12/codemirror.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.641851 xnote-web-0.0.9/static/lib/codemirror/addon/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.441511 xnote-web-0.0.9/static/lib/codemirror/addon/dialog/
--rw-rw-rw-   0        0        0      539 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/dialog/dialog.css
--rw-rw-rw-   0        0        0     5336 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/dialog/dialog.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.469592 xnote-web-0.0.9/static/lib/codemirror/addon/hint/
--rw-rw-rw-   0        0        0     1722 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/anyword-hint.js
--rw-rw-rw-   0        0        0     2226 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/css-hint.js
--rw-rw-rw-   0        0        0    11767 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/html-hint.js
--rw-rw-rw-   0        0        0     6731 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/javascript-hint.js
--rw-rw-rw-   0        0        0      659 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/show-hint.css
--rw-rw-rw-   0        0        0    17150 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/show-hint.js
--rw-rw-rw-   0        0        0     9851 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/sql-hint.js
--rw-rw-rw-   0        0        0     4846 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/hint/xml-hint.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.479786 xnote-web-0.0.9/static/lib/codemirror/addon/search/
--rw-rw-rw-   0        0        0     2067 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/search/jump-to-line.js
--rw-rw-rw-   0        0        0    10935 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/search/search.js
--rw-rw-rw-   0        0        0    12261 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/addon/search/searchcursor.js
--rw-rw-rw-   0        0        0     5920 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/codemirror.min.css
--rw-rw-rw-   0        0        0   167495 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/codemirror/codemirror.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.482569 xnote-web-0.0.9/static/lib/codemirror/keymap/
--rw-rw-rw-   0        0        0    25979 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/keymap/sublime.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.510117 xnote-web-0.0.9/static/lib/codemirror/mode/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.513764 xnote-web-0.0.9/static/lib/codemirror/mode/clike/
--rw-rw-rw-   0        0        0    31730 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/clike/clike.js
--rw-rw-rw-   0        0        0    24791 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/codemirror/mode/css.min.js
--rw-rw-rw-   0        0        0    31934 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/javascript.js
--rw-rw-rw-   0        0        0    26408 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/markdown.js
--rw-rw-rw-   0        0        0    18501 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/php.js
--rw-rw-rw-   0        0        0     2249 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/properties.js
--rw-rw-rw-   0        0        0    12819 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/python.js
--rw-rw-rw-   0        0        0     4141 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/shell.js
--rw-rw-rw-   0        0        0    26353 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/mode/sql.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.521979 xnote-web-0.0.9/static/lib/codemirror/theme/
--rw-rw-rw-   0        0        0     1182 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/theme/eclipse.css
--rw-rw-rw-   0        0        0     1665 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/codemirror/theme/monokai.min.css
--rw-rw-rw-   0        0        0     2269 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/codemirror/theme/xq-light.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.527001 xnote-web-0.0.9/static/lib/csv.js/
--rw-rw-rw-   0        0        0    13851 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/csv.js/csv.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.534497 xnote-web-0.0.9/static/lib/d3/
--rw-rw-rw-   0        0        0   347498 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/d3/d3.js
--rw-rw-rw-   0        0        0   151729 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/d3/d3.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.538499 xnote-web-0.0.9/static/lib/exif-js/
--rw-rw-rw-   0        0        0    41513 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/exif-js/exif.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.541824 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/
--rw-rw-rw-   0        0        0      330 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/HELP-US-OUT.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.549240 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/css/
--rw-rw-rw-   0        0        0    39751 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/css/font-awesome.css
--rw-rw-rw-   0        0        0    31004 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/css/font-awesome.min.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.571551 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/
--rw-rw-rw-   0        0        0   134808 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.610257 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/
--rw-rw-rw-   0        0        0      747 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/animated.less
--rw-rw-rw-   0        0        0      610 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/bordered-pulled.less
--rw-rw-rw-   0        0        0      464 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/core.less
--rw-rw-rw-   0        0        0      125 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/fixed-width.less
--rw-rw-rw-   0        0        0      513 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/font-awesome.less
--rw-rw-rw-   0        0        0    50501 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/icons.less
--rw-rw-rw-   0        0        0      383 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/larger.less
--rw-rw-rw-   0        0        0      396 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/list.less
--rw-rw-rw-   0        0        0     1663 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/mixins.less
--rw-rw-rw-   0        0        0      786 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/path.less
--rw-rw-rw-   0        0        0      642 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/rotated-flipped.less
--rw-rw-rw-   0        0        0      123 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/screen-reader.less
--rw-rw-rw-   0        0        0      496 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/stacked.less
--rw-rw-rw-   0        0        0    23363 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/variables.less
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.652617 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/
--rw-rw-rw-   0        0        0      749 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_animated.scss
--rw-rw-rw-   0        0        0      617 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_bordered-pulled.scss
--rw-rw-rw-   0        0        0      471 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_core.scss
--rw-rw-rw-   0        0        0      126 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_fixed-width.scss
--rw-rw-rw-   0        0        0    51287 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_icons.scss
--rw-rw-rw-   0        0        0      388 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_larger.scss
--rw-rw-rw-   0        0        0      397 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_list.scss
--rw-rw-rw-   0        0        0     1697 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_mixins.scss
--rw-rw-rw-   0        0        0      798 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_path.scss
--rw-rw-rw-   0        0        0      692 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_rotated-flipped.scss
--rw-rw-rw-   0        0        0      139 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_screen-reader.scss
--rw-rw-rw-   0        0        0      502 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_stacked.scss
--rw-rw-rw-   0        0        0    23444 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_variables.scss
--rw-rw-rw-   0        0        0      448 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/font-awesome.scss
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.658433 xnote-web-0.0.9/static/lib/highlight.js/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.656244 xnote-web-0.0.9/static/lib/highlight.js/11.6.0/
--rw-rw-rw-   0        0        0   120388 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/lib/highlight.js/11.6.0/highlight.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.660244 xnote-web-0.0.9/static/lib/highlight.js/11.6.0/styles/
--rw-rw-rw-   0        0        0     1144 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/lib/highlight.js/11.6.0/styles/default.min.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.659439 xnote-web-0.0.9/static/lib/highlight.js/11.7.0/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.663596 xnote-web-0.0.9/static/lib/highlight.js/11.7.0/styles/
--rw-rw-rw-   0        0        0     1158 2023-10-27 13:17:40.000000 xnote-web-0.0.9/static/lib/highlight.js/11.7.0/styles/a11y-dark.min.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.660837 xnote-web-0.0.9/static/lib/jexcel/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.708565 xnote-web-0.0.9/static/lib/jexcel/2.0.2/
--rw-rw-rw-   0        0        0     8809 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jexcel.js
--rw-rw-rw-   0        0        0     2605 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jexcel.min.js
--rw-rw-rw-   0        0        0     5311 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.css
--rw-rw-rw-   0        0        0    35343 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.js
--rw-rw-rw-   0        0        0     4113 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.min.css
--rw-rw-rw-   0        0        0    13730 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.min.js
--rw-rw-rw-   0        0        0    11415 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.css
--rw-rw-rw-   0        0        0    30620 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.js
--rw-rw-rw-   0        0        0     9071 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.min.css
--rw-rw-rw-   0        0        0    11974 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.min.js
--rw-rw-rw-   0        0        0    12095 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.css
--rw-rw-rw-   0        0        0   208970 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.js
--rw-rw-rw-   0        0        0     9179 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.min.css
--rw-rw-rw-   0        0        0    74272 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.712768 xnote-web-0.0.9/static/lib/jquery/
--rw-rw-rw-   0        0        0    97168 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jquery/jquery-1.12.4.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.719426 xnote-web-0.0.9/static/lib/jquery-url-parser/
--rw-rw-rw-   0        0        0     9036 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jquery-url-parser/purl.js
--rw-rw-rw-   0        0        0     4487 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jquery-url-parser/purl.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.722696 xnote-web-0.0.9/static/lib/jquery.qrcode/
--rw-rw-rw-   0        0        0    14023 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jquery.qrcode/jquery.qrcode.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.731500 xnote-web-0.0.9/static/lib/jquery.terminal/
--rw-rw-rw-   0        0        0     2126 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jquery.terminal/dterm.js
--rw-rw-rw-   0        0        0     8268 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.css
--rw-rw-rw-   0        0        0    77663 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.735354 xnote-web-0.0.9/static/lib/jsdiff/
--rw-rw-rw-   0        0        0    32769 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jsdiff/diff.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.752925 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/
--rw-rw-rw-   0        0        0    11017 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/README.md
--rw-rw-rw-   0        0        0      647 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/WEBCOMPONENT.md
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.761632 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/deps/
--rw-rw-rw-   0        0        0    63460 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.css
--rw-rw-rw-   0        0        0   373913 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.775720 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/
--rw-rw-rw-   0        0        0    20709 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.css
--rw-rw-rw-   0        0        0   561932 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.js
--rw-rw-rw-   0        0        0     5435 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.theme.css
--rw-rw-rw-   0        0        0      143 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.798951 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/
--rw-rw-rw-   0        0        0     1725 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/de_DE.json
--rw-rw-rw-   0        0        0     1568 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/en_GB.json
--rw-rw-rw-   0        0        0     1919 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/fr_FR.json
--rw-rw-rw-   0        0        0     1656 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/it_IT.json
--rw-rw-rw-   0        0        0     1706 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/pt_BR.json
--rw-rw-rw-   0        0        0     1444 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/zh_CN.json
--rw-rw-rw-   0        0        0     1015 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/package.json
--rw-rw-rw-   0        0        0     1709 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/webcomponent-spreadsheet.md
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.803298 xnote-web-0.0.9/static/lib/layDate-v5.0.9/
--rw-rw-rw-   0        0        0    27379 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layDate-v5.0.9/laydate.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.671968 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.807438 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.822343 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/
--rw-rw-rw-   0        0        0     2456 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.eot
--rw-rw-rw-   0        0        0     3119 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.svg
--rw-rw-rw-   0        0        0     2272 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.ttf
--rw-rw-rw-   0        0        0     1492 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.woff
--rw-rw-rw-   0        0        0     7980 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/laydate.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.830760 xnote-web-0.0.9/static/lib/layer/
--rw-rw-rw-   0        0        0    40713 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layer/layer.full.js
--rw-rw-rw-   0        0        0    22117 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layer/layer.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.836761 xnote-web-0.0.9/static/lib/layer/mobile/
--rw-rw-rw-   0        0        0     3303 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layer/mobile/layer.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.841136 xnote-web-0.0.9/static/lib/layer/mobile/need/
--rw-rw-rw-   0        0        0     5260 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/mobile/need/layer.css
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:22.680482 xnote-web-0.0.9/static/lib/layer/theme/
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.862438 xnote-web-0.0.9/static/lib/layer/theme/default/
--rw-rw-rw-   0        0        0     5911 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/theme/default/icon-ext.png
--rw-rw-rw-   0        0        0    11493 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/theme/default/icon.png
--rw-rw-rw-   0        0        0    14367 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/theme/default/layer.css
--rw-rw-rw-   0        0        0     5793 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/theme/default/loading-0.gif
--rw-rw-rw-   0        0        0      701 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/theme/default/loading-1.gif
--rw-rw-rw-   0        0        0     1787 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/layer/theme/default/loading-2.gif
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.833760 xnote-web-0.0.9/static/lib/layer.mobile-v2.0/
--rw-rw-rw-   0        0        0       56 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/layer.mobile-v2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.866467 xnote-web-0.0.9/static/lib/marked/
--rw-rw-rw-   0        0        0    30358 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/marked/marked.js
--rw-rw-rw-   0        0        0     6709 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/md5.js
--rw-rw-rw-   0        0        0      708 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/package-lock.json
--rw-rw-rw-   0        0        0       57 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/package.json
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.869689 xnote-web-0.0.9/static/lib/quarkjs/
--rw-rw-rw-   0        0        0    46947 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/quarkjs/quark.base-1.0.0.min.js
--rw-rw-rw-   0        0        0    15329 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/require-2.1.17.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.873691 xnote-web-0.0.9/static/lib/requirejs/
--rw-rw-rw-   0        0        0    17699 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/requirejs/require-2.3.6.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.880024 xnote-web-0.0.9/static/lib/string-format/
--rw-rw-rw-   0        0        0     3143 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/string-format/string-format.js
--rw-rw-rw-   0        0        0     2218 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/string-format/string-format.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.887821 xnote-web-0.0.9/static/lib/string.js/
--rw-rw-rw-   0        0        0    22555 2023-04-06 14:57:19.000000 xnote-web-0.0.9/static/lib/string.js/string-3.3.1.min.js
--rw-rw-rw-   0        0        0    38381 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/string.js/string.js
--rw-rw-rw-   0        0        0     1813 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/utf.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.895922 xnote-web-0.0.9/static/lib/vue/
--rw-rw-rw-   0        0        0    76673 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/vue/vue-2.2.6.min.js
--rw-rw-rw-   0        0        0   106768 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/vue/vue-2.7.9.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.899921 xnote-web-0.0.9/static/lib/wangEditor/
--rw-rw-rw-   0        0        0    66013 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/wangEditor/wangEditor-3.1.1.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.915087 xnote-web-0.0.9/static/lib/webuploader/
--rw-rw-rw-   0        0        0     1078 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/webuploader/README.md
--rw-rw-rw-   0        0        0   143099 2023-04-06 14:57:20.000000 xnote-web-0.0.9/static/lib/webuploader/Uploader.swf
--rw-rw-rw-   0        0        0      543 2023-04-06 14:57:39.000000 xnote-web-0.0.9/static/lib/webuploader/webuploader.css
--rw-rw-rw-   0        0        0    70755 2023-04-06 14:57:40.000000 xnote-web-0.0.9/static/lib/webuploader/webuploader.nolog.min.js
--rw-rw-rw-   0        0        0    21080 2023-04-06 14:57:20.000000 xnote-web-0.0.9/static/xnote.pdn
--rw-rw-rw-   0        0        0     3454 2023-04-06 14:57:20.000000 xnote-web-0.0.9/static/xnote.png
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.983845 xnote-web-0.0.9/tests/
--rw-rw-rw-   0        0        0      258 2022-05-01 06:45:23.000000 xnote-web-0.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0      287 2023-10-27 13:17:40.000000 xnote-web-0.0.9/tests/a.py
--rw-rw-rw-   0        0        0     3258 2024-03-31 06:37:13.000000 xnote-web-0.0.9/tests/test_admin.py
--rw-rw-rw-   0        0        0    15279 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_app.py
--rw-rw-rw-   0        0        0     6635 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_base.py
--rw-rw-rw-   0        0        0     1421 2022-05-01 07:09:21.000000 xnote-web-0.0.9/tests/test_dict.py
--rw-rw-rw-   0        0        0     1631 2023-03-04 06:34:27.000000 xnote-web-0.0.9/tests/test_exif.py
--rw-rw-rw-   0        0        0     3158 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_fs.py
--rw-rw-rw-   0        0        0    10420 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_message.py
--rw-rw-rw-   0        0        0    29005 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_note.py
--rw-rw-rw-   0        0        0     1248 2022-11-26 16:30:19.000000 xnote-web-0.0.9/tests/test_search.py
--rw-rw-rw-   0        0        0    11261 2023-10-27 13:17:40.000000 xnote-web-0.0.9/tests/test_system_sync.py
--rw-rw-rw-   0        0        0      734 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_user.py
--rw-rw-rw-   0        0        0     5654 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_xauth.py
--rw-rw-rw-   0        0        0     1150 2021-10-01 10:27:00.000000 xnote-web-0.0.9/tests/test_xmanager.py
--rw-rw-rw-   0        0        0    15673 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_xutils.py
--rw-rw-rw-   0        0        0     2066 2023-10-27 13:17:40.000000 xnote-web-0.0.9/tests/test_xutils_cache.py
--rw-rw-rw-   0        0        0    31902 2024-03-31 06:41:51.000000 xnote-web-0.0.9/tests/test_xutils_db.py
--rw-rw-rw-   0        0        0     1798 2023-06-30 12:24:59.000000 xnote-web-0.0.9/tests/test_xutils_db_hash_table.py
--rw-rw-rw-   0        0        0     9209 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_xutils_db_table.py
--rw-rw-rw-   0        0        0     3292 2024-03-16 14:56:20.000000 xnote-web-0.0.9/tests/test_xutils_sqldb.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:25.986899 xnote-web-0.0.9/xnote/
--rw-rw-rw-   0        0        0       40 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.036161 xnote-web-0.0.9/xnote/core/
--rw-rw-rw-   0        0        0     1952 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/__init__.py
--rw-rw-rw-   0        0        0     3874 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/autoreload.py
--rw-rw-rw-   0        0        0    27122 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/xauth.py
--rw-rw-rw-   0        0        0    29099 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/xconfig.py
--rw-rw-rw-   0        0        0    29243 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/xmanager.py
--rw-rw-rw-   0        0        0      155 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/xmanager_log.py
--rw-rw-rw-   0        0        0    12575 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/xnote_app.py
--rw-rw-rw-   0        0        0     5371 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/xnote_code_builder.py
--rw-rw-rw-   0        0        0      422 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/xnote_event.py
--rw-rw-rw-   0        0        0      919 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/xnote_hooks.py
--rw-rw-rw-   0        0        0      887 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/xnote_trace.py
--rw-rw-rw-   0        0        0     1467 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote/core/xnote_user_config.py
--rw-rw-rw-   0        0        0    25389 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/xtables.py
--rw-rw-rw-   0        0        0     7100 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/core/xtables_kv.py
--rw-rw-rw-   0        0        0    17713 2024-03-31 03:20:52.000000 xnote-web-0.0.9/xnote/core/xtemplate.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.053468 xnote-web-0.0.9/xnote/plugin/
--rw-rw-rw-   0        0        0       66 2024-03-31 03:18:38.000000 xnote-web-0.0.9/xnote/plugin/__init__.py
--rw-rw-rw-   0        0        0     1881 2024-03-31 03:15:40.000000 xnote-web-0.0.9/xnote/plugin/component.py
--rw-rw-rw-   0        0        0     2115 2024-03-31 06:21:08.000000 xnote-web-0.0.9/xnote/plugin/form.py
--rw-rw-rw-   0        0        0     7261 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/plugin/plugin.py
--rw-rw-rw-   0        0        0     2452 2024-03-31 03:44:04.000000 xnote-web-0.0.9/xnote/plugin/table.py
--rw-rw-rw-   0        0        0     3428 2024-03-31 05:47:24.000000 xnote-web-0.0.9/xnote/plugin/table_plugin.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.065102 xnote-web-0.0.9/xnote/service/
--rw-rw-rw-   0        0        0      378 2024-03-24 03:19:16.000000 xnote-web-0.0.9/xnote/service/__init__.py
--rw-rw-rw-   0        0        0     2196 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/service/comment_service.py
--rw-rw-rw-   0        0        0     3667 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/service/job_service.py
--rw-rw-rw-   0        0        0     3117 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote/service/tag_service.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.129771 xnote-web-0.0.9/xnote_migrate/
--rw-rw-rw-   0        0        0      887 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/__init__.py
--rw-rw-rw-   0        0        0     3007 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/base.py
--rw-rw-rw-   0        0        0      473 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_000.py
--rw-rw-rw-   0        0        0     1314 2023-11-05 02:18:54.000000 xnote-web-0.0.9/xnote_migrate/upgrade_001.py
--rw-rw-rw-   0        0        0     1359 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_002.py
--rw-rw-rw-   0        0        0     2341 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_003.py
--rw-rw-rw-   0        0        0      661 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_004.py
--rw-rw-rw-   0        0        0      826 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_005.py
--rw-rw-rw-   0        0        0      472 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_006.py
--rw-rw-rw-   0        0        0      729 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_007.py
--rw-rw-rw-   0        0        0      459 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_008.py
--rw-rw-rw-   0        0        0      994 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_009.py
--rw-rw-rw-   0        0        0     1321 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_010.py
--rw-rw-rw-   0        0        0     1413 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_011.py
--rw-rw-rw-   0        0        0     2974 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_012.py
--rw-rw-rw-   0        0        0      604 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_013.py
--rw-rw-rw-   0        0        0      922 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_014.py
--rw-rw-rw-   0        0        0     2595 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_015.py
--rw-rw-rw-   0        0        0     2292 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xnote_migrate/upgrade_016.py
--rw-rw-rw-   0        0        0    11779 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote_migrate/upgrade_017.py
--rw-rw-rw-   0        0        0     7433 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xnote_migrate/upgrade_018.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.166303 xnote-web-0.0.9/xnote_web.egg-info/
--rw-rw-rw-   0        0        0     5759 2024-03-31 06:48:20.000000 xnote-web-0.0.9/xnote_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    35026 2024-03-31 06:48:22.000000 xnote-web-0.0.9/xnote_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 06:48:20.000000 xnote-web-0.0.9/xnote_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-03-31 06:48:20.000000 xnote-web-0.0.9/xnote_web.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.258538 xnote-web-0.0.9/xutils/
--rw-rw-rw-   0        0        0     9514 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/__init__.py
--rw-rw-rw-   0        0        0     1631 2023-03-11 14:27:18.000000 xnote-web-0.0.9/xutils/base.py
--rw-rw-rw-   0        0        0    23648 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/cacheutil.py
--rw-rw-rw-   0        0        0      274 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/csvutil.py
--rw-rw-rw-   0        0        0    10216 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/dateutil.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.351680 xnote-web-0.0.9/xutils/db/
--rw-rw-rw-   0        0        0      128 2022-03-19 02:03:55.000000 xnote-web-0.0.9/xutils/db/__init__.py
--rw-rw-rw-   0        0        0     6574 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/binlog.py
--rw-rw-rw-   0        0        0    26827 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/db/dbutil_base.py
--rw-rw-rw-   0        0        0     3699 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/dbutil_cache.py
--rw-rw-rw-   0        0        0     4774 2023-06-30 12:24:59.000000 xnote-web-0.0.9/xutils/db/dbutil_deque.py
--rw-rw-rw-   0        0        0     4756 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/dbutil_hash.py
--rw-rw-rw-   0        0        0      697 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/dbutil_helper.py
--rw-rw-rw-   0        0        0     4006 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/db/dbutil_id_gen.py
--rw-rw-rw-   0        0        0     2692 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/dbutil_set.py
--rw-rw-rw-   0        0        0     8502 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/dbutil_sortedset.py
--rw-rw-rw-   0        0        0    30513 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/db/dbutil_table.py
--rw-rw-rw-   0        0        0    11927 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/db/dbutil_table_index.py
--rw-rw-rw-   0        0        0    13903 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/db/dbutil_table_v2.py
--rw-rw-rw-   0        0        0     1941 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/driver_leveldb.py
--rw-rw-rw-   0        0        0     4696 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/driver_leveldbpy.py
--rw-rw-rw-   0        0        0     9596 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/driver_lmdb.py
--rw-rw-rw-   0        0        0    17289 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/db/driver_mysql.py
--rw-rw-rw-   0        0        0     3280 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/driver_mysql_enhance.py
--rw-rw-rw-   0        0        0    11514 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/driver_sqlite.py
--rw-rw-rw-   0        0        0     4064 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/driver_ssdb.py
--rw-rw-rw-   0        0        0     7816 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/encode.py
--rw-rw-rw-   0        0        0     2374 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/db/filters.py
--rw-rw-rw-   0        0        0     2690 2023-04-06 04:04:41.000000 xnote-web-0.0.9/xutils/db/lock.py
--rw-rw-rw-   0        0        0     4615 2022-05-17 15:05:38.000000 xnote-web-0.0.9/xutils/db/shard.py
--rw-rw-rw-   0        0        0     1908 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/dbutil.py
--rw-rw-rw-   0        0        0     9214 2023-11-11 11:01:44.000000 xnote-web-0.0.9/xutils/exeutil.py
--rw-rw-rw-   0        0        0    22991 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/fsutil.py
--rw-rw-rw-   0        0        0     1837 2022-01-25 14:37:52.000000 xnote-web-0.0.9/xutils/func_util.py
--rw-rw-rw-   0        0        0     8708 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/functions.py
--rw-rw-rw-   0        0        0     1080 2021-10-01 10:27:00.000000 xnote-web-0.0.9/xutils/htmlutil.py
--rw-rw-rw-   0        0        0     3868 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/imports.py
--rw-rw-rw-   0        0        0     7692 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/interfaces.py
--rw-rw-rw-   0        0        0      783 2023-06-30 12:24:59.000000 xnote-web-0.0.9/xutils/jsonutil.py
--rw-rw-rw-   0        0        0      317 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/lists.py
--rw-rw-rw-   0        0        0     2255 2022-05-04 14:57:31.000000 xnote-web-0.0.9/xutils/lockutil.py
--rw-rw-rw-   0        0        0    11834 2023-06-30 12:24:59.000000 xnote-web-0.0.9/xutils/logutil.py
--rw-rw-rw-   0        0        0     3426 2023-04-16 02:40:02.000000 xnote-web-0.0.9/xutils/mem_util.py
--rw-rw-rw-   0        0        0    10953 2023-12-02 11:46:25.000000 xnote-web-0.0.9/xutils/netutil.py
--rw-rw-rw-   0        0        0      216 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/numutil.py
--rw-rw-rw-   0        0        0    30698 2023-03-04 06:34:27.000000 xnote-web-0.0.9/xutils/six.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.365538 xnote-web-0.0.9/xutils/sqldb/
--rw-rw-rw-   0        0        0      382 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/sqldb/__init__.py
--rw-rw-rw-   0        0        0    12725 2023-11-26 15:25:45.000000 xnote-web-0.0.9/xutils/sqldb/table_manager.py
--rw-rw-rw-   0        0        0    10584 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/sqldb/table_proxy.py
--rw-rw-rw-   0        0        0      450 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/sqldb/utils.py
--rw-rw-rw-   0        0        0    18850 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/text_parser.py
--rw-rw-rw-   0        0        0     2741 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/text_parser_properties.py
--rw-rw-rw-   0        0        0    22978 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/textutil.py
--rw-rw-rw-   0        0        0      651 2023-03-04 06:34:27.000000 xnote-web-0.0.9/xutils/textutil_url.py
--rw-rw-rw-   0        0        0     7496 2023-01-22 10:01:14.000000 xnote-web-0.0.9/xutils/tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-03-31 06:48:26.383568 xnote-web-0.0.9/xutils/tornado/
--rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/tornado/__init__.py
--rw-rw-rw-   0        0        0    14538 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/tornado/escape.py
--rw-rw-rw-   0        0        0    10906 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/tornado/log.py
--rw-rw-rw-   0        0        0    37310 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/tornado/template.py
--rw-rw-rw-   0        0        0    13605 2023-10-27 13:17:40.000000 xnote-web-0.0.9/xutils/tornado/util.py
--rw-rw-rw-   0        0        0     8287 2024-03-16 14:56:20.000000 xnote-web-0.0.9/xutils/webutil.py
--rw-rw-rw-   0        0        0     2378 2021-10-01 10:27:00.000000 xnote-web-0.0.9/xutils/ziputil.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.430080 xnote-web-0.1.0/
+-rw-rw-rw-   0        0        0    35147 2021-10-01 10:27:00.000000 xnote-web-0.1.0/COPYING
+-rw-rw-rw-   0        0        0      259 2023-10-27 13:17:40.000000 xnote-web-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5759 2024-05-03 04:09:11.426935 xnote-web-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5416 2024-03-16 14:56:17.000000 xnote-web-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.026140 xnote-web-0.1.0/config/
+-rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.1.0/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.093944 xnote-web-0.1.0/config/boot/
+-rw-rw-rw-   0        0        0     3661 2024-04-05 04:01:41.000000 xnote-web-0.1.0/config/boot/boot.default.properties
+-rw-rw-rw-   0        0        0      413 2022-05-29 13:03:06.000000 xnote-web-0.1.0/config/boot/boot.local.follower.properties
+-rw-rw-rw-   0        0        0      612 2022-10-06 02:04:52.000000 xnote-web-0.1.0/config/boot/boot.local.leveldb.properties
+-rw-rw-rw-   0        0        0       98 2024-04-20 13:28:50.000000 xnote-web-0.1.0/config/boot/boot.local.mem.properties
+-rw-rw-rw-   0        0        0      792 2024-04-20 13:35:54.000000 xnote-web-0.1.0/config/boot/boot.local.properties
+-rw-rw-rw-   0        0        0      116 2023-04-06 04:04:41.000000 xnote-web-0.1.0/config/boot/boot.min.properties
+-rw-rw-rw-   0        0        0      581 2024-04-21 03:04:26.000000 xnote-web-0.1.0/config/boot/boot.sae.properties
+-rw-rw-rw-   0        0        0      113 2022-08-14 10:12:12.000000 xnote-web-0.1.0/config/boot/boot.sqlite.properties
+-rw-rw-rw-   0        0        0      201 2024-03-16 14:56:17.000000 xnote-web-0.1.0/config/boot/boot.test.properties
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.098128 xnote-web-0.1.0/config/cron/
+-rw-rw-rw-   0        0        0     1572 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/cron/cron.json
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.126393 xnote-web-0.1.0/config/file/
+-rw-rw-rw-   0        0        0       20 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/file/audio.properties
+-rw-rw-rw-   0        0        0      142 2023-03-04 06:34:27.000000 xnote-web-0.1.0/config/file/code.properties
+-rw-rw-rw-   0        0        0      181 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/file/image.properties
+-rw-rw-rw-   0        0        0      448 2022-04-17 03:52:32.000000 xnote-web-0.1.0/config/file/mime-types.properties
+-rw-rw-rw-   0        0        0      298 2023-10-27 13:17:40.000000 xnote-web-0.1.0/config/file/preview.properties
+-rw-rw-rw-   0        0        0      580 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/file/text.properties
+-rw-rw-rw-   0        0        0       35 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/file/video.properties
+-rw-rw-rw-   0        0        0       27 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/file/zip.properties
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.134519 xnote-web-0.1.0/config/lang/
+-rw-rw-rw-   0        0        0      794 2022-03-19 10:57:33.000000 xnote-web-0.1.0/config/lang/en.properties
+-rw-rw-rw-   0        0        0     2259 2023-07-16 02:37:42.000000 xnote-web-0.1.0/config/lang/zh.properties
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.143016 xnote-web-0.1.0/config/note/
+-rw-rw-rw-   0        0        0      231 2022-07-15 15:16:19.000000 xnote-web-0.1.0/config/note/category.ddc.properties
+-rw-rw-rw-   0        0        0      135 2022-07-15 16:06:41.000000 xnote-web-0.1.0/config/note/category.properties
+-rw-rw-rw-   0        0        0      857 2022-11-26 16:30:19.000000 xnote-web-0.1.0/config/note/smart_group.ini
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.154596 xnote-web-0.1.0/config/plugin/
+-rw-rw-rw-   0        0        0     6718 2024-03-16 14:56:17.000000 xnote-web-0.1.0/config/plugin/form_plugin.tpl.py
+-rw-rw-rw-   0        0        0      798 2024-03-16 14:56:17.000000 xnote-web-0.1.0/config/plugin/plugin.tpl.py
+-rw-rw-rw-   0        0        0      179 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/plugin/plugins.ini
+-rw-rw-rw-   0        0        0      141 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/requirements.full.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/requirements.min.txt
+-rw-rw-rw-   0        0        0       25 2023-10-27 13:17:40.000000 xnote-web-0.1.0/config/requirements.mysql.txt
+-rw-rw-rw-   0        0        0       88 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/requirements.test.txt
+-rw-rw-rw-   0        0        0      127 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/requirements.txt
+-rw-rw-rw-   0        0        0      126 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/requirements.win.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.160066 xnote-web-0.1.0/config/user/
+-rw-rw-rw-   0        0        0       76 2021-10-01 10:27:00.000000 xnote-web-0.1.0/config/user/invalid_names.list
+-rw-rw-rw-   0        0        0      818 2023-06-30 12:24:59.000000 xnote-web-0.1.0/config/user/user_config.default.properties
+-rw-rw-rw-   0        0        0       23 2024-05-02 14:09:14.000000 xnote-web-0.1.0/config/version.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.194989 xnote-web-0.1.0/docs/
+-rw-rw-rw-   0        0        0     2792 2022-11-26 16:30:19.000000 xnote-web-0.1.0/docs/architecture.md
+-rw-rw-rw-   0        0        0    18566 2024-03-16 14:56:17.000000 xnote-web-0.1.0/docs/changelog.md
+-rw-rw-rw-   0        0        0     3008 2022-05-28 11:20:41.000000 xnote-web-0.1.0/docs/code_style.md
+-rw-rw-rw-   0        0        0      567 2022-03-13 14:33:54.000000 xnote-web-0.1.0/docs/code_style_css.md
+-rw-rw-rw-   0        0        0     2257 2022-11-26 16:30:19.000000 xnote-web-0.1.0/docs/commands.md
+-rw-rw-rw-   0        0        0     3025 2023-10-27 13:17:40.000000 xnote-web-0.1.0/docs/database.md
+-rw-rw-rw-   0        0        0     1799 2023-10-27 13:17:40.000000 xnote-web-0.1.0/docs/db_migrate.md
+-rw-rw-rw-   0        0        0     1364 2022-11-26 16:30:19.000000 xnote-web-0.1.0/docs/plugins.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.418787 xnote-web-0.1.0/docs/screenshots/
+-rw-rw-rw-   0        0        0    43384 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/architecture.png
+-rw-rw-rw-   0        0        0    13063 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/architecture.svg
+-rw-rw-rw-   0        0        0    57359 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/architecture_2.png
+-rw-rw-rw-   0        0        0   112396 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/command_listdir.png
+-rw-rw-rw-   0        0        0    81824 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/command_rmfolder.png
+-rw-rw-rw-   0        0        0   139528 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/screenshot01.png
+-rw-rw-rw-   0        0        0   236777 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/screenshot02.png
+-rw-rw-rw-   0        0        0   101099 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/screenshot03.png
+-rw-rw-rw-   0        0        0    24412 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/task_web.PNG
+-rw-rw-rw-   0        0        0    29284 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.2_editor.PNG
+-rw-rw-rw-   0        0        0    43162 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.2_list.PNG
+-rw-rw-rw-   0        0        0   225642 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.2_mobile.png
+-rw-rw-rw-   0        0        0    23527 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.2_search.png
+-rw-rw-rw-   0        0        0    54676 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.3_desktop01.png
+-rw-rw-rw-   0        0        0   153849 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.4.png
+-rw-rw-rw-   0        0        0   235750 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v1.5.png
+-rw-rw-rw-   0        0        0   214791 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.0.png
+-rw-rw-rw-   0        0        0   187105 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.1_home.png
+-rw-rw-rw-   0        0        0   202760 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.2_20190331.png
+-rw-rw-rw-   0        0        0   179408 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.3_20190411.png
+-rw-rw-rw-   0        0        0   214443 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.3_home.png
+-rw-rw-rw-   0        0        0    99255 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.4_home.png
+-rw-rw-rw-   0        0        0   103529 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.4_home2.png
+-rw-rw-rw-   0        0        0    82664 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.5_20200502.png
+-rw-rw-rw-   0        0        0   121009 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.5_home.png
+-rw-rw-rw-   0        0        0    78846 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.5_recent.png
+-rw-rw-rw-   0        0        0    66479 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.6_home.png
+-rw-rw-rw-   0        0        0   107994 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.7_home.png
+-rw-rw-rw-   0        0        0    88658 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.8_home.png
+-rw-rw-rw-   0        0        0   120643 2022-11-26 16:30:19.000000 xnote-web-0.1.0/docs/screenshots/xnote_v2.9.2_home.png
+-rw-rw-rw-   0        0        0   110782 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote_v20191111.png
+-rw-rw-rw-   0        0        0   158216 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/screenshots/xnote架构.png
+-rw-rw-rw-   0        0        0       16 2021-10-01 10:27:00.000000 xnote-web-0.1.0/docs/search_extension.md
+-rw-rw-rw-   0        0        0      456 2024-03-16 14:56:17.000000 xnote-web-0.1.0/docs/upload_to_pip.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.445227 xnote-web-0.1.0/handlers/
+-rw-rw-rw-   0        0        0       26 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.454491 xnote-web-0.1.0/handlers/admin/
+-rw-rw-rw-   0        0        0        0 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/admin/__init__.py
+-rw-rw-rw-   0        0        0     1439 2024-03-31 03:21:12.000000 xnote-web-0.1.0/handlers/admin/func_admin.py
+-rw-rw-rw-   0        0        0     5756 2024-04-20 08:50:50.000000 xnote-web-0.1.0/handlers/admin/job_admin.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.487678 xnote-web-0.1.0/handlers/api/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/__init__.py
+-rw-rw-rw-   0        0        0      705 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/alarm.py
+-rw-rw-rw-   0        0        0      727 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/check_network.py
+-rw-rw-rw-   0        0        0     1249 2023-03-11 14:27:18.000000 xnote-web-0.1.0/handlers/api/getip.py
+-rw-rw-rw-   0        0        0      365 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/http_headers.py
+-rw-rw-rw-   0        0        0     1466 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/ipv6.py
+-rw-rw-rw-   0        0        0     3563 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/readbook.py
+-rw-rw-rw-   0        0        0     1020 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/report_time.py
+-rw-rw-rw-   0        0        0     1986 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/api/report_weather.py
+-rw-rw-rw-   0        0        0      604 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/api/tts.py
+-rw-rw-rw-   0        0        0       30 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/base.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.522795 xnote-web-0.1.0/handlers/code/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/code/__init__.py
+-rw-rw-rw-   0        0        0     7726 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/code/code_edit.html
+-rw-rw-rw-   0        0        0     4717 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/code/code_edit.py
+-rw-rw-rw-   0        0        0     2573 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/code/code_lines.html
+-rw-rw-rw-   0        0        0     6066 2022-04-30 02:31:41.000000 xnote-web-0.1.0/handlers/code/code_lines.py
+-rw-rw-rw-   0        0        0     3278 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/code/code_search.html
+-rw-rw-rw-   0        0        0     8351 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/code/code_search.py
+-rw-rw-rw-   0        0        0     2480 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/code/preview.html
+-rw-rw-rw-   0        0        0     5556 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/code/preview.py
+-rw-rw-rw-   0        0        0     5912 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/code/wiki_edit.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.570951 xnote-web-0.1.0/handlers/common/
+-rw-rw-rw-   0        0        0      472 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/README.md
+-rw-rw-rw-   0        0        0      121 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/back.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.577328 xnote-web-0.1.0/handlers/common/base/
+-rw-rw-rw-   0        0        0      410 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/base/README.md
+-rw-rw-rw-   0        0        0     1358 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/base/pagination.html
+-rw-rw-rw-   0        0        0     2156 2023-11-19 08:31:53.000000 xnote-web-0.1.0/handlers/common/base.html
+-rw-rw-rw-   0        0        0       79 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/base_bottom.html
+-rw-rw-rw-   0        0        0      927 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/base_footer.html
+-rw-rw-rw-   0        0        0     2414 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/common/base_head.html
+-rw-rw-rw-   0        0        0      988 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/common/base_nav.html
+-rw-rw-rw-   0        0        0      185 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/base_simple.html
+-rw-rw-rw-   0        0        0      645 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/base_title.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.581619 xnote-web-0.1.0/handlers/common/button/
+-rw-rw-rw-   0        0        0      149 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/button/back_button.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.585619 xnote-web-0.1.0/handlers/common/date/
+-rw-rw-rw-   0        0        0     2820 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/common/date/month_picker.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.589924 xnote-web-0.1.0/handlers/common/form/
+-rw-rw-rw-   0        0        0     3630 2024-04-13 12:07:35.000000 xnote-web-0.1.0/handlers/common/form/form.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.600924 xnote-web-0.1.0/handlers/common/hook/
+-rw-rw-rw-   0        0        0      137 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/hook/message_search_btn_hook.html
+-rw-rw-rw-   0        0        0      526 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/hook/search_box_hook.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.606304 xnote-web-0.1.0/handlers/common/layout/
+-rw-rw-rw-   0        0        0     3870 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/common/layout/base_layout.html
+-rw-rw-rw-   0        0        0       67 2023-04-06 10:45:42.000000 xnote-web-0.1.0/handlers/common/layout/wide_left.html
+-rw-rw-rw-   0        0        0      702 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/mod_notice.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.622690 xnote-web-0.1.0/handlers/common/nav/
+-rw-rw-rw-   0        0        0     2919 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/common/nav/base_nav_left.html
+-rw-rw-rw-   0        0        0     1374 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/nav/base_nav_project.html
+-rw-rw-rw-   0        0        0      654 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/nav/base_nav_top.html
+-rw-rw-rw-   0        0        0      799 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/nav/content_nav.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.626774 xnote-web-0.1.0/handlers/common/page/
+-rw-rw-rw-   0        0        0      497 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/page/notfound.html
+-rw-rw-rw-   0        0        0     1358 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/pagination.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.664324 xnote-web-0.1.0/handlers/common/script/
+-rw-rw-rw-   0        0        0     1251 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/common/script/adjust.html
+-rw-rw-rw-   0        0        0      420 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/script/debug_script.html
+-rw-rw-rw-   0        0        0      965 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/script/geo_location.html
+-rw-rw-rw-   0        0        0      460 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/common/script/image_fix_1.html
+-rw-rw-rw-   0        0        0     4529 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/common/script/image_fix_2.html
+-rw-rw-rw-   0        0        0      455 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/common/script/load_vue.html
+-rw-rw-rw-   0        0        0      764 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/common/script/require_init.html
+-rw-rw-rw-   0        0        0      256 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/common/script/safe_script.html
+-rw-rw-rw-   0        0        0     3234 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/common/script/textarea_script.html
+-rw-rw-rw-   0        0        0      463 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/common/script/translate_script.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.671324 xnote-web-0.1.0/handlers/common/search/
+-rw-rw-rw-   0        0        0      758 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/search/search_box.html
+-rw-rw-rw-   0        0        0      750 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/search/search_mobile.html
+-rw-rw-rw-   0        0        0       43 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/search_box.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.678324 xnote-web-0.1.0/handlers/common/sidebar/
+-rw-rw-rw-   0        0        0      724 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/sidebar/app_index.html
+-rw-rw-rw-   0        0        0       43 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/sidebar/default.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.682326 xnote-web-0.1.0/handlers/common/table/
+-rw-rw-rw-   0        0        0     3491 2024-04-21 04:39:30.000000 xnote-web-0.1.0/handlers/common/table/table.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.685323 xnote-web-0.1.0/handlers/common/text/
+-rw-rw-rw-   0        0        0       41 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/common/text/empty_text.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.691159 xnote-web-0.1.0/handlers/common/theme/
+-rw-rw-rw-   0        0        0     2331 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/common/theme/sidebar.html
+-rw-rw-rw-   0        0        0     1683 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/common/theme/sidebar_left.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.695514 xnote-web-0.1.0/handlers/common/title/
+-rw-rw-rw-   0        0        0      273 2021-10-31 03:54:18.000000 xnote-web-0.1.0/handlers/common/title/base_title.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.704293 xnote-web-0.1.0/handlers/cron/
+-rw-rw-rw-   0        0        0      142 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/cron/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/cron/cron_stats.py
+-rw-rw-rw-   0        0        0     3344 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/cron/diskclean.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.721921 xnote-web-0.1.0/handlers/dict/
+-rw-rw-rw-   0        0        0      136 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/dict/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.725224 xnote-web-0.1.0/handlers/dict/component/
+-rw-rw-rw-   0        0        0      798 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/dict/component/dict_sidebar.html
+-rw-rw-rw-   0        0        0     2483 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/dict/dao_relevant.py
+-rw-rw-rw-   0        0        0     5490 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/dict/dict.py
+-rw-rw-rw-   0        0        0     2620 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/dict/dict_dao.py
+-rw-rw-rw-   0        0        0     2000 2022-05-21 15:50:36.000000 xnote-web-0.1.0/handlers/dict/dict_relevant.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.745475 xnote-web-0.1.0/handlers/dict/page/
+-rw-rw-rw-   0        0        0     1899 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/dict/page/dict_add.html
+-rw-rw-rw-   0        0        0     1255 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/dict/page/dict_edit.html
+-rw-rw-rw-   0        0        0     1305 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/dict/page/dict_list.html
+-rw-rw-rw-   0        0        0     2650 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/dict/page/dict_update.html
+-rw-rw-rw-   0        0        0     3767 2022-05-15 04:37:11.000000 xnote-web-0.1.0/handlers/dict/page/relevant_list.html
+-rw-rw-rw-   0        0        0      589 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/error.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.807553 xnote-web-0.1.0/handlers/fs/
+-rw-rw-rw-   0        0        0      142 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/fs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.845483 xnote-web-0.1.0/handlers/fs/component/
+-rw-rw-rw-   0        0        0     2927 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/fs/component/clipboard-dialog.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.851566 xnote-web-0.1.0/handlers/fs/component/css/
+-rw-rw-rw-   0        0        0      103 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/fs/component/css/fs_css.html
+-rw-rw-rw-   0        0        0     1505 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/component/filelist_gallery.html
+-rw-rw-rw-   0        0        0     1174 2024-04-05 13:23:50.000000 xnote-web-0.1.0/handlers/fs/component/filelist_simple.html
+-rw-rw-rw-   0        0        0      893 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/component/fs_sidebar.html
+-rw-rw-rw-   0        0        0      408 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/component/fs_title.html
+-rw-rw-rw-   0        0        0     4086 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/component/move_file_dialog.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.861427 xnote-web-0.1.0/handlers/fs/component/options/
+-rw-rw-rw-   0        0        0      673 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/fs/component/options/fs_options.html
+-rw-rw-rw-   0        0        0     3238 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/fs/component/options/fs_options_buttons.html
+-rw-rw-rw-   0        0        0     2132 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/fs/component/options/fs_options_buttons.mobile.html
+-rw-rw-rw-   0        0        0     2942 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/fs/component/options_css.html
+-rw-rw-rw-   0        0        0     1910 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/component/plugins-dialog.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.866850 xnote-web-0.1.0/handlers/fs/component/script/
+-rw-rw-rw-   0        0        0    13910 2024-05-02 13:44:58.000000 xnote-web-0.1.0/handlers/fs/component/script/file_op_script.html
+-rw-rw-rw-   0        0        0    24179 2024-05-02 14:02:24.000000 xnote-web-0.1.0/handlers/fs/fs.py
+-rw-rw-rw-   0        0        0     2642 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/fs_add.py
+-rw-rw-rw-   0        0        0      867 2022-05-21 16:20:57.000000 xnote-web-0.1.0/handlers/fs/fs_api.py
+-rw-rw-rw-   0        0        0     1862 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/fs/fs_cache.py
+-rw-rw-rw-   0        0        0     2806 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/fs_find.py
+-rw-rw-rw-   0        0        0     6768 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/fs_helper.py
+-rw-rw-rw-   0        0        0     4615 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/fs_hex.py
+-rw-rw-rw-   0        0        0     2428 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/fs_image.py
+-rw-rw-rw-   0        0        0     7046 2024-04-03 14:52:41.000000 xnote-web-0.1.0/handlers/fs/fs_index.py
+-rw-rw-rw-   0        0        0     1004 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/fs/fs_mode.py
+-rw-rw-rw-   0        0        0     4700 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/fs/fs_plugins.py
+-rw-rw-rw-   0        0        0     3635 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/fs/fs_preview.py
+-rw-rw-rw-   0        0        0     5410 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/fs_text.py
+-rw-rw-rw-   0        0        0    14864 2024-05-02 13:42:44.000000 xnote-web-0.1.0/handlers/fs/fs_upload.py
+-rw-rw-rw-   0        0        0     1902 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/mod_aside.html
+-rw-rw-rw-   0        0        0     6622 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/mod_fs_upload.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.907639 xnote-web-0.1.0/handlers/fs/page/
+-rw-rw-rw-   0        0        0     2180 2024-05-02 13:34:45.000000 xnote-web-0.1.0/handlers/fs/page/fs.html
+-rw-rw-rw-   0        0        0     1974 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/fs/page/fs_bookmark.html
+-rw-rw-rw-   0        0        0     3165 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/fs/page/fs_grid.html
+-rw-rw-rw-   0        0        0     2778 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/page/fs_index.html
+-rw-rw-rw-   0        0        0      352 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/fs/page/fs_not_readable.html
+-rw-rw-rw-   0        0        0     2540 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/fs/page/fs_plugins.html
+-rw-rw-rw-   0        0        0     1788 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/fs/page/fs_shell.html
+-rw-rw-rw-   0        0        0     4442 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/fs/page/fs_sidebar.html
+-rw-rw-rw-   0        0        0     5629 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/fs/page/fs_text.html
+-rw-rw-rw-   0        0        0     4920 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/fs/page/fs_text_v1.html
+-rw-rw-rw-   0        0        0     3078 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/fs/page/fs_upload.html
+-rw-rw-rw-   0        0        0     2093 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/index.html
+-rw-rw-rw-   0        0        0     1517 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/index.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.935817 xnote-web-0.1.0/handlers/message/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/message/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.942939 xnote-web-0.1.0/handlers/message/ajax/
+-rw-rw-rw-   0        0        0     4497 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/message/ajax/message_ajax.html
+-rw-rw-rw-   0        0        0     2711 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/message/ajax/message_tag_ajax.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:07.961805 xnote-web-0.1.0/handlers/message/card/
+-rw-rw-rw-   0        0        0    17381 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/card/deleted_msg_left.html
+-rw-rw-rw-   0        0        0     4712 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/message/card/deleted_msg_left_new.html
+-rw-rw-rw-   0        0        0      585 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/message/card/deleted_msg_right.html
+-rw-rw-rw-   0        0        0     1401 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/card/message_system_tag.html
+-rw-rw-rw-   0        0        0     1429 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/message/card/msg_edit_card.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.022566 xnote-web-0.1.0/handlers/message/component/
+-rw-rw-rw-   0        0        0      977 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/component/message_date_right.html
+-rw-rw-rw-   0        0        0     3782 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/message/component/message_edit.html
+-rw-rw-rw-   0        0        0      787 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/message/component/message_event.html
+-rw-rw-rw-   0        0        0      415 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/message/component/message_header.html
+-rw-rw-rw-   0        0        0     2860 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/component/message_input.html
+-rw-rw-rw-   0        0        0     1230 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/message/component/message_keyword_info.html
+-rw-rw-rw-   0        0        0     2059 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/component/message_list.html
+-rw-rw-rw-   0        0        0     1956 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/component/message_sub_link.html
+-rw-rw-rw-   0        0        0     1181 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/component/message_tab.html
+-rw-rw-rw-   0        0        0      821 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/component/message_tab_log.html
+-rw-rw-rw-   0        0        0      833 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/component/message_tab_task.html
+-rw-rw-rw-   0        0        0      669 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/component/message_tag_list.html
+-rw-rw-rw-   0        0        0      977 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/message/component/message_title.html
+-rw-rw-rw-   0        0        0     3343 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/component/message_todo_inner.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.028227 xnote-web-0.1.0/handlers/message/component/right/
+-rw-rw-rw-   0        0        0     1169 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/component/right/tags.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.032068 xnote-web-0.1.0/handlers/message/component/script/
+-rw-rw-rw-   0        0        0     1009 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/message/component/script/tab_script.html
+-rw-rw-rw-   0        0        0     1939 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/message/component/select_topic_dialog.html
+-rw-rw-rw-   0        0        0      765 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/message/component/show_topic_dialog.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.035663 xnote-web-0.1.0/handlers/message/component/tag/
+-rw-rw-rw-   0        0        0      884 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/component/tag/orderby_tab.html
+-rw-rw-rw-   0        0        0    33301 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/dao.py
+-rw-rw-rw-   0        0        0    35414 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/message.py
+-rw-rw-rw-   0        0        0      904 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/message_model.py
+-rw-rw-rw-   0        0        0     3647 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/message_search.py
+-rw-rw-rw-   0        0        0     3058 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/message_tag.py
+-rw-rw-rw-   0        0        0     2646 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/message_task.py
+-rw-rw-rw-   0        0        0    17095 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/message_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.072317 xnote-web-0.1.0/handlers/message/page/
+-rw-rw-rw-   0        0        0     1064 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/message/page/message.html
+-rw-rw-rw-   0        0        0     2226 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/page/message_calendar.html
+-rw-rw-rw-   0        0        0     2214 2024-03-16 14:56:17.000000 xnote-web-0.1.0/handlers/message/page/message_list_by_day.html
+-rw-rw-rw-   0        0        0     3752 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/page/message_list_view.html
+-rw-rw-rw-   0        0        0     4057 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/message/page/message_search.html
+-rw-rw-rw-   0        0        0     2716 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/page/message_tag_select.html
+-rw-rw-rw-   0        0        0     1608 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/message/page/message_tag_view.html
+-rw-rw-rw-   0        0        0      178 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/message/page/message_todo.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.080801 xnote-web-0.1.0/handlers/message/page/old/
+-rw-rw-rw-   0        0        0     1967 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/page/old/dairy.html
+-rw-rw-rw-   0        0        0    12904 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/message/page/old/message_calendar_old.html
+-rw-rw-rw-   0        0        0     3251 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/message/page/task_index.html
+-rw-rw-rw-   0        0        0      823 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/mod_fs_path.html
+-rw-rw-rw-   0        0        0       36 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/mod_pagenation.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.177555 xnote-web-0.1.0/handlers/note/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.262578 xnote-web-0.1.0/handlers/note/ajax/
+-rw-rw-rw-   0        0        0     2587 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/ajax/comment_edit_dialog.html
+-rw-rw-rw-   0        0        0     1265 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/note/ajax/comment_list.html
+-rw-rw-rw-   0        0        0     1281 2022-02-11 14:35:52.000000 xnote-web-0.1.0/handlers/note/ajax/edit_symbol_dialog.html
+-rw-rw-rw-   0        0        0      134 2022-01-25 14:37:52.000000 xnote-web-0.1.0/handlers/note/ajax/group_detail_dialog.html
+-rw-rw-rw-   0        0        0     3167 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/ajax/group_option_dialog.html
+-rw-rw-rw-   0        0        0      407 2022-02-11 14:35:52.000000 xnote-web-0.1.0/handlers/note/ajax/option_dialog.html
+-rw-rw-rw-   0        0        0       62 2022-02-11 14:35:52.000000 xnote-web-0.1.0/handlers/note/ajax/select_note_dialog.html
+-rw-rw-rw-   0        0        0     1192 2022-03-12 15:02:09.000000 xnote-web-0.1.0/handlers/note/ajax/share_group_dialog.html
+-rw-rw-rw-   0        0        0      726 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/ajax/share_note_dialog.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.339420 xnote-web-0.1.0/handlers/note/card/
+-rw-rw-rw-   0        0        0      277 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/card/README.md
+-rw-rw-rw-   0        0        0      939 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/hot_notes.html
+-rw-rw-rw-   0        0        0      950 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/note_contents_left.html
+-rw-rw-rw-   0        0        0      936 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/card/note_date_picker.html
+-rw-rw-rw-   0        0        0      977 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/note_groups.html
+-rw-rw-rw-   0        0        0      994 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/note_types.html
+-rw-rw-rw-   0        0        0      128 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/card/plan_detail.html
+-rw-rw-rw-   0        0        0      952 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/plan_note_card.html
+-rw-rw-rw-   0        0        0      952 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/plan_sidebar.html
+-rw-rw-rw-   0        0        0     1063 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/recent_created_notes.html
+-rw-rw-rw-   0        0        0     1138 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/recent_update_groups.html
+-rw-rw-rw-   0        0        0     1352 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/recent_update_notes.html
+-rw-rw-rw-   0        0        0     1195 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/sticky_notes.html
+-rw-rw-rw-   0        0        0     1096 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/card/task_memo.html
+-rw-rw-rw-   0        0        0     8850 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/comment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.412782 xnote-web-0.1.0/handlers/note/component/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.416721 xnote-web-0.1.0/handlers/note/component/attribute/
+-rw-rw-rw-   0        0        0     1024 2022-07-17 10:20:13.000000 xnote-web-0.1.0/handlers/note/component/attribute/note_category.html
+-rw-rw-rw-   0        0        0     2699 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/component/batch_move.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.423538 xnote-web-0.1.0/handlers/note/component/button/
+-rw-rw-rw-   0        0        0      317 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/button/fixed_bottom_buttons.html
+-rw-rw-rw-   0        0        0      199 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/button/fixed_buttons.html
+-rw-rw-rw-   0        0        0      581 2022-07-14 14:34:40.000000 xnote-web-0.1.0/handlers/note/component/create_note_header.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.432561 xnote-web-0.1.0/handlers/note/component/css/
+-rw-rw-rw-   0        0        0     1574 2022-04-04 06:46:25.000000 xnote-web-0.1.0/handlers/note/component/css/edit_css.html
+-rw-rw-rw-   0        0        0      788 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/component/css/gallery_css.html
+-rw-rw-rw-   0        0        0      818 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/detail_left.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.465401 xnote-web-0.1.0/handlers/note/component/editor/
+-rw-rw-rw-   0        0        0      552 2022-04-19 15:15:43.000000 xnote-web-0.1.0/handlers/note/component/editor/editor_default_vars.html
+-rw-rw-rw-   0        0        0     3141 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/component/editor/gallery.html
+-rw-rw-rw-   0        0        0     6424 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/editor/markdown.html
+-rw-rw-rw-   0        0        0    15648 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/editor/markdown_edit.html
+-rw-rw-rw-   0        0        0     6150 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/editor/markdown_edit.mobile.html
+-rw-rw-rw-   0        0        0     2051 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/component/editor/post.html
+-rw-rw-rw-   0        0        0     1509 2022-04-01 14:26:37.000000 xnote-web-0.1.0/handlers/note/component/editor/table_lang.html
+-rw-rw-rw-   0        0        0     2521 2022-04-04 15:50:05.000000 xnote-web-0.1.0/handlers/note/component/editor/table_myexcel.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.477174 xnote-web-0.1.0/handlers/note/component/filter/
+-rw-rw-rw-   0        0        0      766 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/filter/group_tag_filter.html
+-rw-rw-rw-   0        0        0      762 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/filter/note_tag_filter.html
+-rw-rw-rw-   0        0        0      556 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/component/filter/type_filter.html
+-rw-rw-rw-   0        0        0     1971 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/group_select.html
+-rw-rw-rw-   0        0        0     3375 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/group_select_tree.html
+-rw-rw-rw-   0        0        0       55 2022-04-22 14:59:54.000000 xnote-web-0.1.0/handlers/note/component/group_special_folder.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.484176 xnote-web-0.1.0/handlers/note/component/header/
+-rw-rw-rw-   0        0        0     1096 2022-02-11 14:35:52.000000 xnote-web-0.1.0/handlers/note/component/header/common_header.html
+-rw-rw-rw-   0        0        0      844 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/header/group_detail_header.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.487175 xnote-web-0.1.0/handlers/note/component/mobile/
+-rw-rw-rw-   0        0        0      855 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/mobile/group_category_switch.html
+-rw-rw-rw-   0        0        0     3460 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/mod_aside.html
+-rw-rw-rw-   0        0        0      495 2022-06-26 11:06:28.000000 xnote-web-0.1.0/handlers/note/component/note_ext_info.html
+-rw-rw-rw-   0        0        0     2899 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/note_list_component.html
+-rw-rw-rw-   0        0        0      318 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/component/note_orderby.html
+-rw-rw-rw-   0        0        0      668 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/note_orderby_select.html
+-rw-rw-rw-   0        0        0      804 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/note_path.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.502558 xnote-web-0.1.0/handlers/note/component/option/
+-rw-rw-rw-   0        0        0     1403 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/option/create_option.html
+-rw-rw-rw-   0        0        0      756 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/note/component/option/group_option.html
+-rw-rw-rw-   0        0        0     1303 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/option/group_option_dropdown.html
+-rw-rw-rw-   0        0        0     5053 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/option/note_dropdown.html
+-rw-rw-rw-   0        0        0      725 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/root_dropdown.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.553084 xnote-web-0.1.0/handlers/note/component/script/
+-rw-rw-rw-   0        0        0      219 2022-01-25 14:37:52.000000 xnote-web-0.1.0/handlers/note/component/script/all_script.html
+-rw-rw-rw-   0        0        0     2619 2022-07-15 06:43:03.000000 xnote-web-0.1.0/handlers/note/component/script/create_script.html
+-rw-rw-rw-   0        0        0     1164 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/note/component/script/delete_script.html
+-rw-rw-rw-   0        0        0     1513 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/script/group_select_script.html
+-rw-rw-rw-   0        0        0      697 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/component/script/note_copy_script.html
+-rw-rw-rw-   0        0        0     7434 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/script/note_option_script.html
+-rw-rw-rw-   0        0        0      367 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/script/note_template.html
+-rw-rw-rw-   0        0        0      125 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/script/orderby_script.html
+-rw-rw-rw-   0        0        0      936 2022-03-07 15:10:58.000000 xnote-web-0.1.0/handlers/note/component/script/rename_script.html
+-rw-rw-rw-   0        0        0     1443 2022-01-25 14:37:52.000000 xnote-web-0.1.0/handlers/note/component/script/share_script.html
+-rw-rw-rw-   0        0        0      677 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/script/status_script.html
+-rw-rw-rw-   0        0        0     3733 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/script/tag_manage_script.html
+-rw-rw-rw-   0        0        0     2185 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/script/tag_script.html
+-rw-rw-rw-   0        0        0     4092 2022-01-25 14:37:52.000000 xnote-web-0.1.0/handlers/note/component/share_dialog.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.577143 xnote-web-0.1.0/handlers/note/component/sidebar/
+-rw-rw-rw-   0        0        0     1173 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/sidebar/group_list_sidebar.html
+-rw-rw-rw-   0        0        0     1034 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/sidebar/group_manage_sidebar.html
+-rw-rw-rw-   0        0        0     1672 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/sidebar/group_sidebar.html
+-rw-rw-rw-   0        0        0     1370 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/sidebar/markdown_edit_sidebar.html
+-rw-rw-rw-   0        0        0     1794 2024-01-27 06:07:10.000000 xnote-web-0.1.0/handlers/note/component/sidebar/note_sidebar.html
+-rw-rw-rw-   0        0        0      324 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/sidebar/share_sidebar.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.581260 xnote-web-0.1.0/handlers/note/component/sort/
+-rw-rw-rw-   0        0        0      694 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/sort/note_sort_tab.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.588037 xnote-web-0.1.0/handlers/note/component/timeline/
+-rw-rw-rw-   0        0        0     4522 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/component/timeline/timeline_body.html
+-rw-rw-rw-   0        0        0      716 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/timeline/timeline_create_option.html
+-rw-rw-rw-   0        0        0     1794 2022-06-05 05:50:24.000000 xnote-web-0.1.0/handlers/note/component/view_css.html
+-rw-rw-rw-   0        0        0      807 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/view_footer.html
+-rw-rw-rw-   0        0        0     1368 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/component/view_header.html
+-rw-rw-rw-   0        0        0     1798 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/component/view_header_tag.html
+-rw-rw-rw-   0        0        0     1672 2022-03-12 01:39:04.000000 xnote-web-0.1.0/handlers/note/constant.py
+-rw-rw-rw-   0        0        0    62424 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/dao.py
+-rw-rw-rw-   0        0        0     2162 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/dao_api.py
+-rw-rw-rw-   0        0        0     2532 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/dao_book.py
+-rw-rw-rw-   0        0        0     1276 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/dao_category.py
+-rw-rw-rw-   0        0        0     6741 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/dao_comment.py
+-rw-rw-rw-   0        0        0     2140 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/dao_delete.py
+-rw-rw-rw-   0        0        0     3383 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/dao_draft.py
+-rw-rw-rw-   0        0        0      687 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/note/dao_edit.py
+-rw-rw-rw-   0        0        0     8364 2023-11-05 02:18:54.000000 xnote-web-0.1.0/handlers/note/dao_log.py
+-rw-rw-rw-   0        0        0      879 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/dao_read.py
+-rw-rw-rw-   0        0        0     4314 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/dao_share.py
+-rw-rw-rw-   0        0        0    12681 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/dao_tag.py
+-rw-rw-rw-   0        0        0    11086 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/html_importer.py
+-rw-rw-rw-   0        0        0     2397 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/note_api.py
+-rw-rw-rw-   0        0        0      487 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/note_calendar.py
+-rw-rw-rw-   0        0        0     2934 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/note/note_category.py
+-rw-rw-rw-   0        0        0     1381 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/note_checklist.py
+-rw-rw-rw-   0        0        0    28876 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/note_edit.py
+-rw-rw-rw-   0        0        0      491 2022-07-09 01:18:05.000000 xnote-web-0.1.0/handlers/note/note_fix.py
+-rw-rw-rw-   0        0        0    31590 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/note_group.py
+-rw-rw-rw-   0        0        0     1005 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/note_helper.py
+-rw-rw-rw-   0        0        0     3144 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/note_stat.py
+-rw-rw-rw-   0        0        0     8581 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/note_tag.py
+-rw-rw-rw-   0        0        0    21187 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/note_timeline.py
+-rw-rw-rw-   0        0        0    16587 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/note_view.py
+-rw-rw-rw-   0        0        0     4669 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/note_workspace.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.665792 xnote-web-0.1.0/handlers/note/page/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.683297 xnote-web-0.1.0/handlers/note/page/batch/
+-rw-rw-rw-   0        0        0      637 2024-04-05 13:29:57.000000 xnote-web-0.1.0/handlers/note/page/batch/gallery_manage.html
+-rw-rw-rw-   0        0        0     7504 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/page/batch/group_manage.html
+-rw-rw-rw-   0        0        0      632 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/note/page/batch/group_manage_category.html
+-rw-rw-rw-   0        0        0     5580 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/batch/note_manage.html
+-rw-rw-rw-   0        0        0      774 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/page/category.html
+-rw-rw-rw-   0        0        0     5298 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/comment.html
+-rw-rw-rw-   0        0        0      431 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/note/page/comment_user_page.html
+-rw-rw-rw-   0        0        0     5726 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/create.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.706848 xnote-web-0.1.0/handlers/note/page/detail/
+-rw-rw-rw-   0        0        0     2152 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/detail/checklist_detail.html
+-rw-rw-rw-   0        0        0     2452 2023-04-06 04:04:41.000000 xnote-web-0.1.0/handlers/note/page/detail/form_detail.html
+-rw-rw-rw-   0        0        0     1261 2024-03-16 14:56:18.000000 xnote-web-0.1.0/handlers/note/page/detail/group_detail.html
+-rw-rw-rw-   0        0        0     1169 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/note/page/detail/group_detail_body.html
+-rw-rw-rw-   0        0        0     1715 2023-04-06 04:04:41.000000 xnote-web-0.1.0/handlers/note/page/detail/note_detail.html
+-rw-rw-rw-   0        0        0     5694 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/detail/table_detail.html
+-rw-rw-rw-   0        0        0     1503 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/note/page/group_list.html
+-rw-rw-rw-   0        0        0      764 2023-12-16 03:36:03.000000 xnote-web-0.1.0/handlers/note/page/group_list_nav_desktop.html
+-rw-rw-rw-   0        0        0      862 2023-12-16 03:36:03.000000 xnote-web-0.1.0/handlers/note/page/group_list_nav_mobile.html
+-rw-rw-rw-   0        0        0     1708 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/history_list.html
+-rw-rw-rw-   0        0        0     4262 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/html_importer.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.722531 xnote-web-0.1.0/handlers/note/page/index/
+-rw-rw-rw-   0        0        0      971 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/page/index/note_index.html
+-rw-rw-rw-   0        0        0     1278 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/index/note_workspace.html
+-rw-rw-rw-   0        0        0      907 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/index/note_workspace.mobile.html
+-rw-rw-rw-   0        0        0     1008 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/page/index/note_workspace2.html
+-rw-rw-rw-   0        0        0     3604 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/list_by_date.html
+-rw-rw-rw-   0        0        0    12810 2024-04-05 13:32:08.000000 xnote-web-0.1.0/handlers/note/page/note_calendar.html
+-rw-rw-rw-   0        0        0      606 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/note_default.html
+-rw-rw-rw-   0        0        0     1426 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/note_list.html
+-rw-rw-rw-   0        0        0     1508 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/note_recent.html
+-rw-rw-rw-   0        0        0     2003 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/note/page/note_share.html
+-rw-rw-rw-   0        0        0     1292 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/note_tools.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.749302 xnote-web-0.1.0/handlers/note/page/old/
+-rw-rw-rw-   0        0        0      740 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/old/category_old.html
+-rw-rw-rw-   0        0        0     1425 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/note/page/old/create_log.html
+-rw-rw-rw-   0        0        0      807 2022-06-18 00:42:54.000000 xnote-web-0.1.0/handlers/note/page/old/group_list_archived.html
+-rw-rw-rw-   0        0        0     2324 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/old/list_by_date_old.html
+-rw-rw-rw-   0        0        0       92 2022-01-25 14:37:52.000000 xnote-web-0.1.0/handlers/note/page/old/notice.html
+-rw-rw-rw-   0        0        0     4194 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/old/project_list_old.html
+-rw-rw-rw-   0        0        0     2150 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/old/upload_file.html
+-rw-rw-rw-   0        0        0     1267 2023-04-06 04:04:41.000000 xnote-web-0.1.0/handlers/note/page/print.html
+-rw-rw-rw-   0        0        0     1286 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/note/page/taglist.html
+-rw-rw-rw-   0        0        0      783 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/note/page/tagname.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.753302 xnote-web-0.1.0/handlers/note/page/timeline/
+-rw-rw-rw-   0        0        0     1902 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/note/page/timeline/timeline.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.767087 xnote-web-0.1.0/handlers/plan/
+-rw-rw-rw-   0        0        0        0 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/plan/__init__.py
+-rw-rw-rw-   0        0        0     2118 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plan/dao.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.771087 xnote-web-0.1.0/handlers/plan/page/
+-rw-rw-rw-   0        0        0     3773 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plan/page/month_plan.html
+-rw-rw-rw-   0        0        0     3641 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.788984 xnote-web-0.1.0/handlers/plugin/
+-rw-rw-rw-   0        0        0      123 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.803747 xnote-web-0.1.0/handlers/plugin/base/
+-rw-rw-rw-   0        0        0     2051 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/plugin/base/base_form_plugin.html
+-rw-rw-rw-   0        0        0     1118 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/plugin/base/base_plugin.html
+-rw-rw-rw-   0        0        0      510 2022-06-19 09:05:51.000000 xnote-web-0.1.0/handlers/plugin/base/base_plugin_body.html
+-rw-rw-rw-   0        0        0     2228 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plugin/base/base_plugin_title.html
+-rw-rw-rw-   0        0        0     3037 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plugin/dao.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.819215 xnote-web-0.1.0/handlers/plugin/header/
+-rw-rw-rw-   0        0        0      818 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/plugin/header/plugin_category.html
+-rw-rw-rw-   0        0        0      930 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/plugin/header/plugin_header_normal.html
+-rw-rw-rw-   0        0        0      254 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/plugin/header/plugin_header_note.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.835550 xnote-web-0.1.0/handlers/plugin/page/
+-rw-rw-rw-   0        0        0      999 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/plugin/page/grid.html
+-rw-rw-rw-   0        0        0     4756 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/plugin/page/plugins_v1.html
+-rw-rw-rw-   0        0        0     1677 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/plugin/page/plugins_v2.html
+-rw-rw-rw-   0        0        0     1341 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/plugin/page/plugins_v3.html
+-rw-rw-rw-   0        0        0     3969 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plugin/plugin_create.py
+-rw-rw-rw-   0        0        0    28433 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plugin/plugin_page.py
+-rw-rw-rw-   0        0        0     1812 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/plugin/plugin_upload.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.886683 xnote-web-0.1.0/handlers/search/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/search/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.892934 xnote-web-0.1.0/handlers/search/ajax/
+-rw-rw-rw-   0        0        0      641 2022-02-11 14:35:52.000000 xnote-web-0.1.0/handlers/search/ajax/search_dialog.html
+-rw-rw-rw-   0        0        0      977 2022-02-11 14:35:52.000000 xnote-web-0.1.0/handlers/search/ajax/search_dialog_detail.html
+-rw-rw-rw-   0        0        0     1364 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/search/api.py
+-rw-rw-rw-   0        0        0      958 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/search/calc.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.905121 xnote-web-0.1.0/handlers/search/component/
+-rw-rw-rw-   0        0        0     1367 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/search/component/search_pagination.html
+-rw-rw-rw-   0        0        0     1034 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/search/component/search_sidebar.html
+-rw-rw-rw-   0        0        0     2172 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/search/component/search_tab.html
+-rw-rw-rw-   0        0        0     3278 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/search/dictionary.py
+-rw-rw-rw-   0        0        0      910 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/search/mute.py
+-rw-rw-rw-   0        0        0     1428 2022-03-10 14:02:41.000000 xnote-web-0.1.0/handlers/search/note.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.913136 xnote-web-0.1.0/handlers/search/page/
+-rw-rw-rw-   0        0        0     1967 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/search/page/search_history.html
+-rw-rw-rw-   0        0        0     5839 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/search/page/search_result.html
+-rw-rw-rw-   0        0        0      617 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/search/pydoc.py
+-rw-rw-rw-   0        0        0     2905 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/search/reminder.py
+-rw-rw-rw-   0        0        0     1778 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/search/scripts.py
+-rw-rw-rw-   0        0        0     1245 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/search/search.html
+-rw-rw-rw-   0        0        0    18128 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/search/search.py
+-rw-rw-rw-   0        0        0      440 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/search/search_aside.html
+-rw-rw-rw-   0        0        0     1874 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/search/search_rules.html
+-rw-rw-rw-   0        0        0     2878 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/search/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.919855 xnote-web-0.1.0/handlers/settings/
+-rw-rw-rw-   0        0        0      123 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.937012 xnote-web-0.1.0/handlers/settings/component/
+-rw-rw-rw-   0        0        0     2855 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/settings/component/admin_settings.html
+-rw-rw-rw-   0        0        0     4751 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/settings/component/note_settings.html
+-rw-rw-rw-   0        0        0     1278 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/settings/component/search_settings.html
+-rw-rw-rw-   0        0        0      868 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/settings/component/settings_sidebar.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:08.943928 xnote-web-0.1.0/handlers/settings/page/
+-rw-rw-rw-   0        0        0     1951 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/settings/page/properties.html
+-rw-rw-rw-   0        0        0     2097 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/settings/page/settings.html
+-rw-rw-rw-   0        0        0     7109 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/settings/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.048875 xnote-web-0.1.0/handlers/system/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/system/__init__.py
+-rw-rw-rw-   0        0        0    14937 2024-04-21 14:30:26.000000 xnote-web-0.1.0/handlers/system/backup.py
+-rw-rw-rw-   0        0        0     2773 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/cache_admin.py
+-rw-rw-rw-   0        0        0     4849 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/clipboard.py
+-rw-rw-rw-   0        0        0     3628 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/system/command.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.081684 xnote-web-0.1.0/handlers/system/component/
+-rw-rw-rw-   0        0        0     1425 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/component/admin_nav.html
+-rw-rw-rw-   0        0        0      979 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/component/db_kv_nav.html
+-rw-rw-rw-   0        0        0     1051 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/component/db_nav.html
+-rw-rw-rw-   0        0        0      463 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/system/component/system_css.html
+-rw-rw-rw-   0        0        0      597 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/component/system_log_tab.html
+-rw-rw-rw-   0        0        0     1445 2022-07-02 01:04:41.000000 xnote-web-0.1.0/handlers/system/component/system_sync_cluster_info.html
+-rw-rw-rw-   0        0        0     3450 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/component/system_sync_follower_view.html
+-rw-rw-rw-   0        0        0      564 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/component/thread_nav.html
+-rw-rw-rw-   0        0        0     9561 2024-04-20 08:36:25.000000 xnote-web-0.1.0/handlers/system/crontab.py
+-rw-rw-rw-   0        0        0      719 2024-04-20 08:34:48.000000 xnote-web-0.1.0/handlers/system/dao_cron.py
+-rw-rw-rw-   0        0        0    19557 2024-04-15 15:37:16.000000 xnote-web-0.1.0/handlers/system/db_admin.py
+-rw-rw-rw-   0        0        0     3959 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/db_index.py
+-rw-rw-rw-   0        0        0     8098 2023-10-21 00:22:22.000000 xnote-web-0.1.0/handlers/system/db_migrate_tools.py
+-rw-rw-rw-   0        0        0     1808 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/db_refresh.py
+-rw-rw-rw-   0        0        0     3968 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/db_shell.py
+-rw-rw-rw-   0        0        0     1132 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/db_upgrade.py
+-rw-rw-rw-   0        0        0      534 2022-05-06 04:45:28.000000 xnote-web-0.1.0/handlers/system/develop_controller.py
+-rw-rw-rw-   0        0        0     2165 2024-04-13 14:16:03.000000 xnote-web-0.1.0/handlers/system/handler_profile.py
+-rw-rw-rw-   0        0        0     1823 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/mod_aside.html
+-rw-rw-rw-   0        0        0      567 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/network_profile.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.134926 xnote-web-0.1.0/handlers/system/page/
+-rw-rw-rw-   0        0        0     2797 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/cache_admin.html
+-rw-rw-rw-   0        0        0     2586 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/page/crontab.html
+-rw-rw-rw-   0        0        0     2259 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/system/page/crontab_edit.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.166930 xnote-web-0.1.0/handlers/system/page/db/
+-rw-rw-rw-   0        0        0     6164 2024-04-15 15:37:25.000000 xnote-web-0.1.0/handlers/system/page/db/db_admin.html
+-rw-rw-rw-   0        0        0     2055 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/page/db/db_backup.html
+-rw-rw-rw-   0        0        0     2555 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/db/db_index.html
+-rw-rw-rw-   0        0        0     1192 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/page/db/db_index_v2.html
+-rw-rw-rw-   0        0        0     2342 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/page/db/db_meta.html
+-rw-rw-rw-   0        0        0     1557 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/db/db_struct.html
+-rw-rw-rw-   0        0        0      649 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/db/driver_info.html
+-rw-rw-rw-   0        0        0     1091 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/page/db/sqldb_detail.html
+-rw-rw-rw-   0        0        0     1412 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/page/db/sqldb_list.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.173358 xnote-web-0.1.0/handlers/system/page/develop/
+-rw-rw-rw-   0        0        0        0 2022-05-06 04:45:10.000000 xnote-web-0.1.0/handlers/system/page/develop/component_demo.html
+-rw-rw-rw-   0        0        0      971 2024-03-31 10:54:40.000000 xnote-web-0.1.0/handlers/system/page/develop/index.html
+-rw-rw-rw-   0        0        0      931 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/system/page/history.html
+-rw-rw-rw-   0        0        0     1726 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/page/module_detail.html
+-rw-rw-rw-   0        0        0     1046 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/page/module_list.html
+-rw-rw-rw-   0        0        0     5954 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/page/script.html
+-rw-rw-rw-   0        0        0     2949 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/sqlite.html
+-rw-rw-rw-   0        0        0      651 2022-06-18 13:08:01.000000 xnote-web-0.1.0/handlers/system/page/system_admin.html
+-rw-rw-rw-   0        0        0     2661 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/page/system_index.html
+-rw-rw-rw-   0        0        0     2291 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/system_info.html
+-rw-rw-rw-   0        0        0      651 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/system/page/system_info_text.html
+-rw-rw-rw-   0        0        0     4173 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/system_sync.html
+-rw-rw-rw-   0        0        0      590 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/system/page/template_cache.html
+-rw-rw-rw-   0        0        0     1360 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/page/thread_info.html
+-rw-rw-rw-   0        0        0     6736 2023-03-04 06:34:27.000000 xnote-web-0.1.0/handlers/system/script.py
+-rw-rw-rw-   0        0        0     3566 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/stats.py
+-rw-rw-rw-   0        0        0     8047 2024-04-20 08:44:06.000000 xnote-web-0.1.0/handlers/system/system.py
+-rw-rw-rw-   0        0        0      708 2022-04-03 14:17:05.000000 xnote-web-0.1.0/handlers/system/system_boot.py
+-rw-rw-rw-   0        0        0     2513 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/system_event.py
+-rw-rw-rw-   0        0        0     5213 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/system_info.py
+-rw-rw-rw-   0        0        0     7523 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_log.py
+-rw-rw-rw-   0        0        0     4428 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/system_module.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.198223 xnote-web-0.1.0/handlers/system/system_sync/
+-rw-rw-rw-   0        0        0      772 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/system_sync/models.py
+-rw-rw-rw-   0        0        0     1386 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_sync/node_base.py
+-rw-rw-rw-   0        0        0    19983 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_sync/node_follower.py
+-rw-rw-rw-   0        0        0     9517 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_sync/node_leader.py
+-rw-rw-rw-   0        0        0    12355 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_sync/system_sync_controller.py
+-rw-rw-rw-   0        0        0     7071 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_sync/system_sync_indexer.py
+-rw-rw-rw-   0        0        0    10245 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/system/system_sync/system_sync_proxy.py
+-rw-rw-rw-   0        0        0      444 2023-04-06 15:44:02.000000 xnote-web-0.1.0/handlers/system/system_todo.py
+-rw-rw-rw-   0        0        0      676 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/system/template_cache.py
+-rw-rw-rw-   0        0        0      852 2024-04-03 14:55:09.000000 xnote-web-0.1.0/handlers/system/thread_info.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.255226 xnote-web-0.1.0/handlers/test/
+-rw-rw-rw-   0        0        0      128 2022-01-25 14:37:52.000000 xnote-web-0.1.0/handlers/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.259225 xnote-web-0.1.0/handlers/test/component/
+-rw-rw-rw-   0        0        0     1034 2024-03-31 03:24:19.000000 xnote-web-0.1.0/handlers/test/component/example_nav.html
+-rw-rw-rw-   0        0        0      193 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/test/exception.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.309819 xnote-web-0.1.0/handlers/test/page/
+-rw-rw-rw-   0        0        0      697 2022-06-26 11:21:01.000000 xnote-web-0.1.0/handlers/test/page/example_btn.html
+-rw-rw-rw-   0        0        0     1378 2022-05-07 14:15:21.000000 xnote-web-0.1.0/handlers/test/page/example_dialog.html
+-rw-rw-rw-   0        0        0      866 2022-03-13 13:50:59.000000 xnote-web-0.1.0/handlers/test/page/example_dropdown.html
+-rw-rw-rw-   0        0        0     1537 2022-04-17 03:52:32.000000 xnote-web-0.1.0/handlers/test/page/example_hammer.html
+-rw-rw-rw-   0        0        0      102 2022-03-11 12:10:15.000000 xnote-web-0.1.0/handlers/test/page/example_index.html
+-rw-rw-rw-   0        0        0     1707 2022-03-13 13:45:19.000000 xnote-web-0.1.0/handlers/test/page/example_tab.html
+-rw-rw-rw-   0        0        0     1032 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/test/page/example_tag.html
+-rw-rw-rw-   0        0        0     1695 2024-04-13 12:09:36.000000 xnote-web-0.1.0/handlers/test/test_dbutil_handler.py
+-rw-rw-rw-   0        0        0      977 2024-03-31 06:02:23.000000 xnote-web-0.1.0/handlers/test/test_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.445671 xnote-web-0.1.0/handlers/tools/
+-rw-rw-rw-   0        0        0      105 2022-04-17 09:04:15.000000 xnote-web-0.1.0/handlers/tools/__init__.py
+-rw-rw-rw-   0        0        0     2198 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/barcode.html
+-rw-rw-rw-   0        0        0     1035 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/tools/base64.html
+-rw-rw-rw-   0        0        0      371 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/base_title.html
+-rw-rw-rw-   0        0        0     3539 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/tools/browser_info.html
+-rw-rw-rw-   0        0        0     4077 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/camera.html
+-rw-rw-rw-   0        0        0     1353 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/chat_demo.html
+-rw-rw-rw-   0        0        0    10087 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/code_template.html
+-rw-rw-rw-   0        0        0     3818 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/color.html
+-rw-rw-rw-   0        0        0     1486 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/datetime.html
+-rw-rw-rw-   0        0        0     5346 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/tools/hex.html
+-rw-rw-rw-   0        0        0      426 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/iframe_viewer.html
+-rw-rw-rw-   0        0        0     6029 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/img2gray.html
+-rw-rw-rw-   0        0        0     7694 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/img_merge.html
+-rw-rw-rw-   0        0        0     6002 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/img_split.html
+-rw-rw-rw-   0        0        0      619 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/md5.html
+-rw-rw-rw-   0        0        0     4769 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/tools/multi_win.html
+-rw-rw-rw-   0        0        0     3033 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/notebook.html
+-rw-rw-rw-   0        0        0      342 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/notebook.py
+-rw-rw-rw-   0        0        0     2101 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/port_scanner.py
+-rw-rw-rw-   0        0        0     1020 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/qrcode.html
+-rw-rw-rw-   0        0        0     2424 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/random_string.html
+-rw-rw-rw-   0        0        0     1000 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/responsive.html
+-rw-rw-rw-   0        0        0     4119 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/tools/runjs.html
+-rw-rw-rw-   0        0        0     1224 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/search_compare.html
+-rw-rw-rw-   0        0        0      774 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/tools/sha1.html
+-rw-rw-rw-   0        0        0     1937 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/tools/shell.html
+-rw-rw-rw-   0        0        0     3906 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/speech_recognition.html
+-rw-rw-rw-   0        0        0      896 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/tools/tcc.html
+-rw-rw-rw-   0        0        0     1409 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/tools/terminal.html
+-rw-rw-rw-   0        0        0     8164 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/tools/text_convert.html
+-rw-rw-rw-   0        0        0     3732 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/tools/text_diff.html
+-rw-rw-rw-   0        0        0     3297 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/text_set.html
+-rw-rw-rw-   0        0        0     1011 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/tools.py
+-rw-rw-rw-   0        0        0      487 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/tts.html
+-rw-rw-rw-   0        0        0     1249 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/tools/urlcoder.html
+-rw-rw-rw-   0        0        0     7610 2022-11-26 16:30:19.000000 xnote-web-0.1.0/handlers/tools/vue_test.html
+-rw-rw-rw-   0        0        0     5326 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/tools/webuploader.html
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.462670 xnote-web-0.1.0/handlers/user/
+-rw-rw-rw-   0        0        0      287 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/user/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.466670 xnote-web-0.1.0/handlers/user/component/
+-rw-rw-rw-   0        0        0     1241 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/user/component/user_script.html
+-rw-rw-rw-   0        0        0      347 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/user/dao.py
+-rw-rw-rw-   0        0        0     4949 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/user/login.py
+-rw-rw-rw-   0        0        0      255 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/user/logout.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.490603 xnote-web-0.1.0/handlers/user/page/
+-rw-rw-rw-   0        0        0     1516 2023-04-06 15:52:08.000000 xnote-web-0.1.0/handlers/user/page/change_password.html
+-rw-rw-rw-   0        0        0     3357 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/user/page/login.html
+-rw-rw-rw-   0        0        0      912 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/user/page/user.html
+-rw-rw-rw-   0        0        0     3551 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/user/page/user_list.html
+-rw-rw-rw-   0        0        0     2440 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/user/page/user_manage.html
+-rw-rw-rw-   0        0        0      802 2023-10-27 13:17:40.000000 xnote-web-0.1.0/handlers/user/page/user_op_log.html
+-rw-rw-rw-   0        0        0     1522 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/user/page/userinfo.html
+-rw-rw-rw-   0        0        0     6400 2024-03-16 14:56:19.000000 xnote-web-0.1.0/handlers/user/user.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.498791 xnote-web-0.1.0/handlers/webdav/
+-rw-rw-rw-   0        0        0      123 2021-10-01 10:27:00.000000 xnote-web-0.1.0/handlers/webdav/__init__.py
+-rw-rw-rw-   0        0        0     5704 2023-06-30 12:24:59.000000 xnote-web-0.1.0/handlers/webdav/webdav.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.542110 xnote-web-0.1.0/lib/
+-rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.1.0/lib/__init__.py
+-rw-rw-rw-   0        0        0    33040 2022-05-22 05:10:24.000000 xnote-web-0.1.0/lib/html2text.py
+-rw-rw-rw-   0        0        0   451584 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/leveldb-x64.dll
+-rw-rw-rw-   0        0        0   367104 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/leveldb.dll
+-rw-rw-rw-   0        0        0    37736 2023-10-27 13:17:40.000000 xnote-web-0.1.0/lib/leveldbpy.py
+-rw-rw-rw-   0        0        0     6529 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/smallseg.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.599204 xnote-web-0.1.0/lib/web/
+-rw-rw-rw-   0        0        0      754 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/__init__.py
+-rw-rw-rw-   0        0        0    25946 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/application.py
+-rw-rw-rw-   0        0        0     8714 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.605934 xnote-web-0.1.0/lib/web/contrib/
+-rw-rw-rw-   0        0        0        0 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/contrib/__init__.py
+-rw-rw-rw-   0        0        0     3457 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/contrib/template.py
+-rw-rw-rw-   0        0        0    56068 2023-12-02 10:30:00.000000 xnote-web-0.1.0/lib/web/db.py
+-rw-rw-rw-   0        0        0    13157 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/debugerror.py
+-rw-rw-rw-   0        0        0    13983 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/form.py
+-rw-rw-rw-   0        0        0     4619 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/http.py
+-rw-rw-rw-   0        0        0    13278 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/httpserver.py
+-rw-rw-rw-   0        0        0     6507 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/net.py
+-rw-rw-rw-   0        0        0      877 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/py3helpers.py
+-rw-rw-rw-   0        0        0    10921 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/session.py
+-rw-rw-rw-   0        0        0    49690 2022-11-26 16:30:19.000000 xnote-web-0.1.0/lib/web/template.py
+-rw-rw-rw-   0        0        0     2261 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/test.py
+-rw-rw-rw-   0        0        0    42559 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/utils.py
+-rw-rw-rw-   0        0        0    17704 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/webapi.py
+-rw-rw-rw-   0        0        0     3707 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/webopenid.py
+-rw-rw-rw-   0        0        0     2452 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.626914 xnote-web-0.1.0/lib/web/wsgiserver/
+-rw-rw-rw-   0        0        0     1542 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/wsgiserver/LICENSE.txt
+-rw-rw-rw-   0        0        0      580 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/wsgiserver/__init__.py
+-rw-rw-rw-   0        0        0     4032 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/wsgiserver/ssl_builtin.py
+-rw-rw-rw-   0        0        0     9223 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/wsgiserver/ssl_pyopenssl.py
+-rw-rw-rw-   0        0        0    89663 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/web/wsgiserver/wsgiserver2.py
+-rw-rw-rw-   0        0        0    79905 2022-02-26 02:25:16.000000 xnote-web-0.1.0/lib/web/wsgiserver/wsgiserver3.py
+-rw-rw-rw-   0        0        0    22355 2021-10-01 10:27:00.000000 xnote-web-0.1.0/lib/wget.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 04:09:11.430080 xnote-web-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      985 2024-05-03 04:08:52.000000 xnote-web-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.645211 xnote-web-0.1.0/static/
+-rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.648257 xnote-web-0.1.0/static/audio/
+-rw-rw-rw-   0        0        0    26675 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/audio/todo_done.mp3
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.691262 xnote-web-0.1.0/static/css/
+-rw-rw-rw-   0        0        0    83858 2024-05-02 13:38:51.000000 xnote-web-0.1.0/static/css/app.build.css
+-rw-rw-rw-   0        0        0     1926 2024-03-16 14:56:19.000000 xnote-web-0.1.0/static/css/app.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.748385 xnote-web-0.1.0/static/css/base/
+-rw-rw-rw-   0        0        0     3205 2024-05-02 13:38:50.000000 xnote-web-0.1.0/static/css/base/common-button.css
+-rw-rw-rw-   0        0        0      273 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/css/base/common-dialog.css
+-rw-rw-rw-   0        0        0     1570 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/css/base/common-dropdown.css
+-rw-rw-rw-   0        0        0     2212 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/base/common-icon.css
+-rw-rw-rw-   0        0        0     1476 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/css/base/common-layout.css
+-rw-rw-rw-   0        0        0      651 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/base/common-markdown.css
+-rw-rw-rw-   0        0        0     1312 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/css/base/common-mobile.css
+-rw-rw-rw-   0        0        0      927 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/css/base/common-page.css
+-rw-rw-rw-   0        0        0      603 2023-04-16 02:40:01.000000 xnote-web-0.1.0/static/css/base/common-photo.css
+-rw-rw-rw-   0        0        0     2241 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/css/base/common-tab.css
+-rw-rw-rw-   0        0        0     2137 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/css/base/common-tag.css
+-rw-rw-rw-   0        0        0    18296 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/css/base/common.css
+-rw-rw-rw-   0        0        0      424 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/css/base/layout-second-nav.css
+-rw-rw-rw-   0        0        0      368 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/css/base/reset-wide.css
+-rw-rw-rw-   0        0        0     2689 2024-04-13 12:48:39.000000 xnote-web-0.1.0/static/css/base/reset.css
+-rw-rw-rw-   0        0        0     1795 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/css/common-card.css
+-rw-rw-rw-   0        0        0     3943 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/common-left.css
+-rw-rw-rw-   0        0        0      802 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/common-react.css
+-rw-rw-rw-   0        0        0    31004 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0     4476 2023-06-30 12:24:59.000000 xnote-web-0.1.0/static/css/message.css
+-rw-rw-rw-   0        0        0     5431 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/css/note.css
+-rw-rw-rw-   0        0        0      704 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/plugins.css
+-rw-rw-rw-   0        0        0      269 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/search.css
+-rw-rw-rw-   0        0        0     2066 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/css/timeline.css
+-rw-rw-rw-   0        0        0     1286 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/css/todo.css
+-rw-rw-rw-   0        0        0    16958 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/favicon.ico
+-rw-rw-rw-   0        0        0    16372 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/favicon.png
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.756487 xnote-web-0.1.0/static/fonts/
+-rw-rw-rw-   0        0        0    83588 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    66624 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.847382 xnote-web-0.1.0/static/image/
+-rw-rw-rw-   0        0        0     1277 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/checked.png
+-rw-rw-rw-   0        0        0     2593 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/file.png
+-rw-rw-rw-   0        0        0      985 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/file2.png
+-rw-rw-rw-   0        0        0      120 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/folder.gif
+-rw-rw-rw-   0        0        0      340 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/folder2.png
+-rw-rw-rw-   0        0        0     5696 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/folder3.png
+-rw-rw-rw-   0        0        0      496 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_application.png
+-rw-rw-rw-   0        0        0      956 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_application.svg
+-rw-rw-rw-   0        0        0      128 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_csv.png
+-rw-rw-rw-   0        0        0     1493 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_dict.png
+-rw-rw-rw-   0        0        0      838 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_dict.svg
+-rw-rw-rw-   0        0        0      465 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_folder_settings.png
+-rw-rw-rw-   0        0        0     1024 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_recent.png
+-rw-rw-rw-   0        0        0     1359 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_recent.svg
+-rw-rw-rw-   0        0        0      696 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_right.png
+-rw-rw-rw-   0        0        0      821 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_script.png
+-rw-rw-rw-   0        0        0     1890 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_script.svg
+-rw-rw-rw-   0        0        0     1194 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_search.png
+-rw-rw-rw-   0        0        0     1122 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_search.svg
+-rw-rw-rw-   0        0        0      958 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_settings_applications.png
+-rw-rw-rw-   0        0        0     2120 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_settings_applications.svg
+-rw-rw-rw-   0        0        0     1353 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_shell.png
+-rw-rw-rw-   0        0        0      743 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_shell.svg
+-rw-rw-rw-   0        0        0     2901 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icon_txt.png
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.862201 xnote-web-0.1.0/static/image/icons/
+-rw-rw-rw-   0        0        0     1707 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icons/icon_barcode.png
+-rw-rw-rw-   0        0        0     3158 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icons/icon_game.png
+-rw-rw-rw-   0        0        0     5203 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icons/icon_network.png
+-rw-rw-rw-   0        0        0     1375 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/image/icons/icon_work.png
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.914743 xnote-web-0.1.0/static/js/
+-rw-rw-rw-   0        0        0     2294 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/Lexer.js
+-rw-rw-rw-   0        0        0      657 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/admin.js
+-rw-rw-rw-   0        0        0   103599 2024-05-02 14:01:09.000000 xnote-web-0.1.0/static/js/app.build.js
+-rw-rw-rw-   0        0        0     7644 2023-06-30 12:24:59.000000 xnote-web-0.1.0/static/js/app.js
+-rw-rw-rw-   0        0        0      472 2023-06-30 12:24:59.000000 xnote-web-0.1.0/static/js/autocss.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.939698 xnote-web-0.1.0/static/js/base/
+-rw-rw-rw-   0        0        0     1309 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/base/ajax.js
+-rw-rw-rw-   0        0        0     4375 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/base/array.js
+-rw-rw-rw-   0        0        0      726 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/base/datetime.js
+-rw-rw-rw-   0        0        0      731 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/base/jq-ext.js
+-rw-rw-rw-   0        0        0      580 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/base/misc.js
+-rw-rw-rw-   0        0        0     8338 2023-12-02 11:08:59.000000 xnote-web-0.1.0/static/js/base/string.js
+-rw-rw-rw-   0        0        0     3173 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/base/url.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.943151 xnote-web-0.1.0/static/js/codemirror-addon/
+-rw-rw-rw-   0        0        0    11711 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/codemirror-addon/xnote-search.js
+-rw-rw-rw-   0        0        0    21933 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/colors.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.947445 xnote-web-0.1.0/static/js/components/
+-rw-rw-rw-   0        0        0      786 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/components/date-picker.js
+-rw-rw-rw-   0        0        0     7614 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/console.js
+-rw-rw-rw-   0        0        0     2706 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/editor-csv.js
+-rw-rw-rw-   0        0        0     9949 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/editor.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.950863 xnote-web-0.1.0/static/js/fs/
+-rw-rw-rw-   0        0        0     2314 2024-05-02 13:58:06.000000 xnote-web-0.1.0/static/js/fs/fs.js
+-rw-rw-rw-   0        0        0    16458 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/marked-ext.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:09.975003 xnote-web-0.1.0/static/js/message/
+-rw-rw-rw-   0        0        0    11638 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/message/message.js
+-rw-rw-rw-   0        0        0    15989 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/note.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.005003 xnote-web-0.1.0/static/js/old/
+-rw-rw-rw-   0        0        0     5071 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/old/TagEditor.js
+-rw-rw-rw-   0        0        0     2489 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/old/fileEditor.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.009001 xnote-web-0.1.0/static/js/plan/
+-rw-rw-rw-   0        0        0     2543 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/plan/plan.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.037002 xnote-web-0.1.0/static/js/plugin/
+-rw-rw-rw-   0        0        0     1811 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/plugin/plugin.form.js
+-rw-rw-rw-   0        0        0     4091 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/upload.js
+-rw-rw-rw-   0        0        0    14750 2023-12-02 11:09:33.000000 xnote-web-0.1.0/static/js/utils.build.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.138981 xnote-web-0.1.0/static/js/xnote-ui/
+-rw-rw-rw-   0        0        0    11058 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/layer.photos.js
+-rw-rw-rw-   0        0        0      703 2023-06-30 12:24:59.000000 xnote-web-0.1.0/static/js/xnote-ui/x-audio.js
+-rw-rw-rw-   0        0        0      190 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-core.js
+-rw-rw-rw-   0        0        0     2072 2023-04-16 02:40:01.000000 xnote-web-0.1.0/static/js/xnote-ui/x-device.js
+-rw-rw-rw-   0        0        0    15513 2024-03-31 06:06:00.000000 xnote-web-0.1.0/static/js/xnote-ui/x-dialog.js
+-rw-rw-rw-   0        0        0     3063 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-dropdown.js
+-rw-rw-rw-   0        0        0     4092 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-event.js
+-rw-rw-rw-   0        0        0      327 2023-06-30 12:24:59.000000 xnote-web-0.1.0/static/js/xnote-ui/x-ext.js
+-rw-rw-rw-   0        0        0     8478 2024-03-16 14:56:20.000000 xnote-web-0.1.0/static/js/xnote-ui/x-init.js
+-rw-rw-rw-   0        0        0      674 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-layout.js
+-rw-rw-rw-   0        0        0     1365 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-photo.js
+-rw-rw-rw-   0        0        0     1962 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-tab.js
+-rw-rw-rw-   0        0        0     1257 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/js/xnote-ui/x-template.js
+-rw-rw-rw-   0        0        0     8558 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/js/xnote-ui/x-upload.js
+-rw-rw-rw-   0        0        0     3590 2023-06-30 12:24:59.000000 xnote-web-0.1.0/static/js/xnote-ui/x-url.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.160030 xnote-web-0.1.0/static/lib/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.164390 xnote-web-0.1.0/static/lib/JsBarcode/
+-rw-rw-rw-   0        0        0    61195 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/JsBarcode/JsBarcode.all.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.167923 xnote-web-0.1.0/static/lib/art-template/
+-rw-rw-rw-   0        0        0    17325 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/art-template/template-web-4.13.2.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.171747 xnote-web-0.1.0/static/lib/base64.js/
+-rw-rw-rw-   0        0        0     2280 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/base64.js/base64.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.174943 xnote-web-0.1.0/static/lib/bootstrap/
+-rw-rw-rw-   0        0        0   122544 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/bootstrap/bootstrap-3.3.5.min.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.180645 xnote-web-0.1.0/static/lib/clipboard/
+-rw-rw-rw-   0        0        0    10760 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/clipboard/clipboard-2.0.4.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.187408 xnote-web-0.1.0/static/lib/codemirror/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.197745 xnote-web-0.1.0/static/lib/codemirror/5.41.0/
+-rw-rw-rw-   0        0        0     5920 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/5.41.0/codemirror.min.css
+-rw-rw-rw-   0        0        0   167495 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/codemirror/5.41.0/codemirror.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.204454 xnote-web-0.1.0/static/lib/codemirror/5.65.12/
+-rw-rw-rw-   0        0        0     9064 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/5.65.12/codemirror.css
+-rw-rw-rw-   0        0        0   411661 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/5.65.12/codemirror.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:06.916386 xnote-web-0.1.0/static/lib/codemirror/addon/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.214831 xnote-web-0.1.0/static/lib/codemirror/addon/dialog/
+-rw-rw-rw-   0        0        0      539 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/dialog/dialog.css
+-rw-rw-rw-   0        0        0     5336 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/dialog/dialog.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.247258 xnote-web-0.1.0/static/lib/codemirror/addon/hint/
+-rw-rw-rw-   0        0        0     1722 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/anyword-hint.js
+-rw-rw-rw-   0        0        0     2226 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/css-hint.js
+-rw-rw-rw-   0        0        0    11767 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/html-hint.js
+-rw-rw-rw-   0        0        0     6731 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/javascript-hint.js
+-rw-rw-rw-   0        0        0      659 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/show-hint.css
+-rw-rw-rw-   0        0        0    17150 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/show-hint.js
+-rw-rw-rw-   0        0        0     9851 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/sql-hint.js
+-rw-rw-rw-   0        0        0     4846 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/hint/xml-hint.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.258783 xnote-web-0.1.0/static/lib/codemirror/addon/search/
+-rw-rw-rw-   0        0        0     2067 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/search/jump-to-line.js
+-rw-rw-rw-   0        0        0    10935 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/search/search.js
+-rw-rw-rw-   0        0        0    12261 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/addon/search/searchcursor.js
+-rw-rw-rw-   0        0        0     5920 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/codemirror.min.css
+-rw-rw-rw-   0        0        0   167495 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/codemirror/codemirror.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.264007 xnote-web-0.1.0/static/lib/codemirror/keymap/
+-rw-rw-rw-   0        0        0    25979 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/keymap/sublime.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.294172 xnote-web-0.1.0/static/lib/codemirror/mode/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.298280 xnote-web-0.1.0/static/lib/codemirror/mode/clike/
+-rw-rw-rw-   0        0        0    31730 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/clike/clike.js
+-rw-rw-rw-   0        0        0    24791 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/codemirror/mode/css.min.js
+-rw-rw-rw-   0        0        0    31934 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/javascript.js
+-rw-rw-rw-   0        0        0    26408 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/markdown.js
+-rw-rw-rw-   0        0        0    18501 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/php.js
+-rw-rw-rw-   0        0        0     2249 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/properties.js
+-rw-rw-rw-   0        0        0    12819 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/python.js
+-rw-rw-rw-   0        0        0     4141 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/shell.js
+-rw-rw-rw-   0        0        0    26353 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/mode/sql.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.312080 xnote-web-0.1.0/static/lib/codemirror/theme/
+-rw-rw-rw-   0        0        0     1182 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/theme/eclipse.css
+-rw-rw-rw-   0        0        0     1665 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/codemirror/theme/monokai.min.css
+-rw-rw-rw-   0        0        0     2269 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/codemirror/theme/xq-light.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.317108 xnote-web-0.1.0/static/lib/csv.js/
+-rw-rw-rw-   0        0        0    13851 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/csv.js/csv.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.324758 xnote-web-0.1.0/static/lib/d3/
+-rw-rw-rw-   0        0        0   347498 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/d3/d3.js
+-rw-rw-rw-   0        0        0   151729 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/d3/d3.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.329576 xnote-web-0.1.0/static/lib/exif-js/
+-rw-rw-rw-   0        0        0    41513 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/exif-js/exif.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.333323 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/
+-rw-rw-rw-   0        0        0      330 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/HELP-US-OUT.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.340576 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/css/
+-rw-rw-rw-   0        0        0    39751 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/css/font-awesome.css
+-rw-rw-rw-   0        0        0    31004 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/css/font-awesome.min.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.369595 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/
+-rw-rw-rw-   0        0        0   134808 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.433475 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/
+-rw-rw-rw-   0        0        0      747 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/animated.less
+-rw-rw-rw-   0        0        0      610 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/bordered-pulled.less
+-rw-rw-rw-   0        0        0      464 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/core.less
+-rw-rw-rw-   0        0        0      125 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/fixed-width.less
+-rw-rw-rw-   0        0        0      513 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/font-awesome.less
+-rw-rw-rw-   0        0        0    50501 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/icons.less
+-rw-rw-rw-   0        0        0      383 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/larger.less
+-rw-rw-rw-   0        0        0      396 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/list.less
+-rw-rw-rw-   0        0        0     1663 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/mixins.less
+-rw-rw-rw-   0        0        0      786 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/path.less
+-rw-rw-rw-   0        0        0      642 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/rotated-flipped.less
+-rw-rw-rw-   0        0        0      123 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/screen-reader.less
+-rw-rw-rw-   0        0        0      496 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/stacked.less
+-rw-rw-rw-   0        0        0    23363 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/variables.less
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.498875 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/
+-rw-rw-rw-   0        0        0      749 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_animated.scss
+-rw-rw-rw-   0        0        0      617 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_bordered-pulled.scss
+-rw-rw-rw-   0        0        0      471 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_core.scss
+-rw-rw-rw-   0        0        0      126 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_fixed-width.scss
+-rw-rw-rw-   0        0        0    51287 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_icons.scss
+-rw-rw-rw-   0        0        0      388 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_larger.scss
+-rw-rw-rw-   0        0        0      397 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_list.scss
+-rw-rw-rw-   0        0        0     1697 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_mixins.scss
+-rw-rw-rw-   0        0        0      798 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_path.scss
+-rw-rw-rw-   0        0        0      692 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_rotated-flipped.scss
+-rw-rw-rw-   0        0        0      139 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_screen-reader.scss
+-rw-rw-rw-   0        0        0      502 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_stacked.scss
+-rw-rw-rw-   0        0        0    23444 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_variables.scss
+-rw-rw-rw-   0        0        0      448 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/font-awesome.scss
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:06.934234 xnote-web-0.1.0/static/lib/highlight.js/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.503273 xnote-web-0.1.0/static/lib/highlight.js/11.6.0/
+-rw-rw-rw-   0        0        0   120388 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/lib/highlight.js/11.6.0/highlight.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.506439 xnote-web-0.1.0/static/lib/highlight.js/11.6.0/styles/
+-rw-rw-rw-   0        0        0     1144 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/lib/highlight.js/11.6.0/styles/default.min.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:06.935270 xnote-web-0.1.0/static/lib/highlight.js/11.7.0/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.510897 xnote-web-0.1.0/static/lib/highlight.js/11.7.0/styles/
+-rw-rw-rw-   0        0        0     1158 2023-10-27 13:17:40.000000 xnote-web-0.1.0/static/lib/highlight.js/11.7.0/styles/a11y-dark.min.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:06.936822 xnote-web-0.1.0/static/lib/jexcel/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.567309 xnote-web-0.1.0/static/lib/jexcel/2.0.2/
+-rw-rw-rw-   0        0        0     8809 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jexcel.js
+-rw-rw-rw-   0        0        0     2605 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jexcel.min.js
+-rw-rw-rw-   0        0        0     5311 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.css
+-rw-rw-rw-   0        0        0    35343 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.js
+-rw-rw-rw-   0        0        0     4113 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.min.css
+-rw-rw-rw-   0        0        0    13730 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.min.js
+-rw-rw-rw-   0        0        0    11415 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.css
+-rw-rw-rw-   0        0        0    30620 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.js
+-rw-rw-rw-   0        0        0     9071 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.min.css
+-rw-rw-rw-   0        0        0    11974 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.min.js
+-rw-rw-rw-   0        0        0    12095 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.css
+-rw-rw-rw-   0        0        0   208970 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.js
+-rw-rw-rw-   0        0        0     9179 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.min.css
+-rw-rw-rw-   0        0        0    74272 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.571961 xnote-web-0.1.0/static/lib/jquery/
+-rw-rw-rw-   0        0        0    97168 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jquery/jquery-1.12.4.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.579175 xnote-web-0.1.0/static/lib/jquery-url-parser/
+-rw-rw-rw-   0        0        0     9036 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jquery-url-parser/purl.js
+-rw-rw-rw-   0        0        0     4487 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jquery-url-parser/purl.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.583646 xnote-web-0.1.0/static/lib/jquery.qrcode/
+-rw-rw-rw-   0        0        0    14023 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jquery.qrcode/jquery.qrcode.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.597221 xnote-web-0.1.0/static/lib/jquery.terminal/
+-rw-rw-rw-   0        0        0     2126 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jquery.terminal/dterm.js
+-rw-rw-rw-   0        0        0     8268 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.css
+-rw-rw-rw-   0        0        0    77663 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.600065 xnote-web-0.1.0/static/lib/jsdiff/
+-rw-rw-rw-   0        0        0    32769 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jsdiff/diff.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.620632 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/
+-rw-rw-rw-   0        0        0    11017 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/README.md
+-rw-rw-rw-   0        0        0      647 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/WEBCOMPONENT.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.631225 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/deps/
+-rw-rw-rw-   0        0        0    63460 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.css
+-rw-rw-rw-   0        0        0   373913 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.646610 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/
+-rw-rw-rw-   0        0        0    20709 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.css
+-rw-rw-rw-   0        0        0   561932 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.js
+-rw-rw-rw-   0        0        0     5435 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.theme.css
+-rw-rw-rw-   0        0        0      143 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.670573 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/
+-rw-rw-rw-   0        0        0     1725 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/de_DE.json
+-rw-rw-rw-   0        0        0     1568 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/en_GB.json
+-rw-rw-rw-   0        0        0     1919 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/fr_FR.json
+-rw-rw-rw-   0        0        0     1656 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/it_IT.json
+-rw-rw-rw-   0        0        0     1706 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/pt_BR.json
+-rw-rw-rw-   0        0        0     1444 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/zh_CN.json
+-rw-rw-rw-   0        0        0     1015 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/package.json
+-rw-rw-rw-   0        0        0     1709 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/webcomponent-spreadsheet.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.673714 xnote-web-0.1.0/static/lib/layDate-v5.0.9/
+-rw-rw-rw-   0        0        0    27379 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layDate-v5.0.9/laydate.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:06.950856 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.678717 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.696287 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/
+-rw-rw-rw-   0        0        0     2456 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.eot
+-rw-rw-rw-   0        0        0     3119 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.svg
+-rw-rw-rw-   0        0        0     2272 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.ttf
+-rw-rw-rw-   0        0        0     1492 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.woff
+-rw-rw-rw-   0        0        0     7980 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/laydate.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.703899 xnote-web-0.1.0/static/lib/layer/
+-rw-rw-rw-   0        0        0    40713 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layer/layer.full.js
+-rw-rw-rw-   0        0        0    22117 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layer/layer.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.712142 xnote-web-0.1.0/static/lib/layer/mobile/
+-rw-rw-rw-   0        0        0     3303 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layer/mobile/layer.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.715826 xnote-web-0.1.0/static/lib/layer/mobile/need/
+-rw-rw-rw-   0        0        0     5260 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/mobile/need/layer.css
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:06.959033 xnote-web-0.1.0/static/lib/layer/theme/
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.738724 xnote-web-0.1.0/static/lib/layer/theme/default/
+-rw-rw-rw-   0        0        0     5911 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/theme/default/icon-ext.png
+-rw-rw-rw-   0        0        0    11493 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/theme/default/icon.png
+-rw-rw-rw-   0        0        0    14367 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/theme/default/layer.css
+-rw-rw-rw-   0        0        0     5793 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/theme/default/loading-0.gif
+-rw-rw-rw-   0        0        0      701 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/theme/default/loading-1.gif
+-rw-rw-rw-   0        0        0     1787 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/layer/theme/default/loading-2.gif
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.707386 xnote-web-0.1.0/static/lib/layer.mobile-v2.0/
+-rw-rw-rw-   0        0        0       56 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/layer.mobile-v2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.741397 xnote-web-0.1.0/static/lib/marked/
+-rw-rw-rw-   0        0        0    30358 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/marked/marked.js
+-rw-rw-rw-   0        0        0     6709 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/md5.js
+-rw-rw-rw-   0        0        0      708 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/package-lock.json
+-rw-rw-rw-   0        0        0       57 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/package.json
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.747097 xnote-web-0.1.0/static/lib/quarkjs/
+-rw-rw-rw-   0        0        0    46947 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/quarkjs/quark.base-1.0.0.min.js
+-rw-rw-rw-   0        0        0    15329 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/require-2.1.17.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.750787 xnote-web-0.1.0/static/lib/requirejs/
+-rw-rw-rw-   0        0        0    17699 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/requirejs/require-2.3.6.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.759088 xnote-web-0.1.0/static/lib/string-format/
+-rw-rw-rw-   0        0        0     3143 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/string-format/string-format.js
+-rw-rw-rw-   0        0        0     2218 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/string-format/string-format.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.768184 xnote-web-0.1.0/static/lib/string.js/
+-rw-rw-rw-   0        0        0    22555 2023-04-06 14:57:19.000000 xnote-web-0.1.0/static/lib/string.js/string-3.3.1.min.js
+-rw-rw-rw-   0        0        0    38381 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/string.js/string.js
+-rw-rw-rw-   0        0        0     1813 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/utf.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.775694 xnote-web-0.1.0/static/lib/vue/
+-rw-rw-rw-   0        0        0    76673 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/vue/vue-2.2.6.min.js
+-rw-rw-rw-   0        0        0   106768 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/vue/vue-2.7.9.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.780399 xnote-web-0.1.0/static/lib/wangEditor/
+-rw-rw-rw-   0        0        0    66013 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/wangEditor/wangEditor-3.1.1.min.js
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.796587 xnote-web-0.1.0/static/lib/webuploader/
+-rw-rw-rw-   0        0        0     1078 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/webuploader/README.md
+-rw-rw-rw-   0        0        0   143099 2023-04-06 14:57:20.000000 xnote-web-0.1.0/static/lib/webuploader/Uploader.swf
+-rw-rw-rw-   0        0        0      543 2023-04-06 14:57:39.000000 xnote-web-0.1.0/static/lib/webuploader/webuploader.css
+-rw-rw-rw-   0        0        0    70755 2023-04-06 14:57:40.000000 xnote-web-0.1.0/static/lib/webuploader/webuploader.nolog.min.js
+-rw-rw-rw-   0        0        0    21080 2023-04-06 14:57:20.000000 xnote-web-0.1.0/static/xnote.pdn
+-rw-rw-rw-   0        0        0     3454 2023-04-06 14:57:20.000000 xnote-web-0.1.0/static/xnote.png
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.872131 xnote-web-0.1.0/tests/
+-rw-rw-rw-   0        0        0      258 2022-05-01 06:45:23.000000 xnote-web-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      287 2023-10-27 13:17:40.000000 xnote-web-0.1.0/tests/a.py
+-rw-rw-rw-   0        0        0     3258 2024-03-31 06:37:13.000000 xnote-web-0.1.0/tests/test_admin.py
+-rw-rw-rw-   0        0        0    14637 2024-04-20 08:42:38.000000 xnote-web-0.1.0/tests/test_app.py
+-rw-rw-rw-   0        0        0     6635 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_base.py
+-rw-rw-rw-   0        0        0     1421 2022-05-01 07:09:21.000000 xnote-web-0.1.0/tests/test_dict.py
+-rw-rw-rw-   0        0        0     1631 2023-03-04 06:34:27.000000 xnote-web-0.1.0/tests/test_exif.py
+-rw-rw-rw-   0        0        0     3158 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_fs.py
+-rw-rw-rw-   0        0        0    10420 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_message.py
+-rw-rw-rw-   0        0        0    29005 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_note.py
+-rw-rw-rw-   0        0        0     1248 2022-11-26 16:30:19.000000 xnote-web-0.1.0/tests/test_search.py
+-rw-rw-rw-   0        0        0     2016 2024-04-03 17:07:22.000000 xnote-web-0.1.0/tests/test_service.py
+-rw-rw-rw-   0        0        0    11261 2023-10-27 13:17:40.000000 xnote-web-0.1.0/tests/test_system_sync.py
+-rw-rw-rw-   0        0        0      734 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_user.py
+-rw-rw-rw-   0        0        0     5654 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_xauth.py
+-rw-rw-rw-   0        0        0     1150 2021-10-01 10:27:00.000000 xnote-web-0.1.0/tests/test_xmanager.py
+-rw-rw-rw-   0        0        0    15739 2024-05-02 14:09:10.000000 xnote-web-0.1.0/tests/test_xutils.py
+-rw-rw-rw-   0        0        0     1999 2024-04-05 11:03:00.000000 xnote-web-0.1.0/tests/test_xutils_cache.py
+-rw-rw-rw-   0        0        0    31902 2024-03-31 06:41:51.000000 xnote-web-0.1.0/tests/test_xutils_db.py
+-rw-rw-rw-   0        0        0     2111 2024-04-15 15:43:16.000000 xnote-web-0.1.0/tests/test_xutils_db_hash_table.py
+-rw-rw-rw-   0        0        0     9209 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_xutils_db_table.py
+-rw-rw-rw-   0        0        0     3292 2024-03-16 14:56:20.000000 xnote-web-0.1.0/tests/test_xutils_sqldb.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.876837 xnote-web-0.1.0/xnote/
+-rw-rw-rw-   0        0        0       40 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.927417 xnote-web-0.1.0/xnote/core/
+-rw-rw-rw-   0        0        0     1952 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/core/__init__.py
+-rw-rw-rw-   0        0        0     3874 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/core/autoreload.py
+-rw-rw-rw-   0        0        0    27122 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/core/xauth.py
+-rw-rw-rw-   0        0        0    29928 2024-05-03 04:08:17.000000 xnote-web-0.1.0/xnote/core/xconfig.py
+-rw-rw-rw-   0        0        0    29243 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/core/xmanager.py
+-rw-rw-rw-   0        0        0      155 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/core/xmanager_log.py
+-rw-rw-rw-   0        0        0    12899 2024-04-21 03:01:03.000000 xnote-web-0.1.0/xnote/core/xnote_app.py
+-rw-rw-rw-   0        0        0     5371 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/core/xnote_code_builder.py
+-rw-rw-rw-   0        0        0      422 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/core/xnote_event.py
+-rw-rw-rw-   0        0        0      919 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/core/xnote_hooks.py
+-rw-rw-rw-   0        0        0      887 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/core/xnote_trace.py
+-rw-rw-rw-   0        0        0     1467 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote/core/xnote_user_config.py
+-rw-rw-rw-   0        0        0    26293 2024-04-05 04:04:25.000000 xnote-web-0.1.0/xnote/core/xtables.py
+-rw-rw-rw-   0        0        0     7100 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/core/xtables_kv.py
+-rw-rw-rw-   0        0        0    17841 2024-03-31 13:37:06.000000 xnote-web-0.1.0/xnote/core/xtemplate.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.947885 xnote-web-0.1.0/xnote/plugin/
+-rw-rw-rw-   0        0        0       66 2024-03-31 03:18:38.000000 xnote-web-0.1.0/xnote/plugin/__init__.py
+-rw-rw-rw-   0        0        0     1881 2024-03-31 03:15:40.000000 xnote-web-0.1.0/xnote/plugin/component.py
+-rw-rw-rw-   0        0        0     2327 2024-04-13 12:08:25.000000 xnote-web-0.1.0/xnote/plugin/form.py
+-rw-rw-rw-   0        0        0     7261 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/plugin/plugin.py
+-rw-rw-rw-   0        0        0     3135 2024-04-21 11:15:41.000000 xnote-web-0.1.0/xnote/plugin/table.py
+-rw-rw-rw-   0        0        0     3591 2024-04-13 12:11:10.000000 xnote-web-0.1.0/xnote/plugin/table_plugin.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:10.963890 xnote-web-0.1.0/xnote/service/
+-rw-rw-rw-   0        0        0      409 2024-04-03 16:02:24.000000 xnote-web-0.1.0/xnote/service/__init__.py
+-rw-rw-rw-   0        0        0     2196 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/service/comment_service.py
+-rw-rw-rw-   0        0        0     3665 2024-04-03 15:59:03.000000 xnote-web-0.1.0/xnote/service/job_service.py
+-rw-rw-rw-   0        0        0     3255 2024-04-03 17:01:19.000000 xnote-web-0.1.0/xnote/service/lock_service.py
+-rw-rw-rw-   0        0        0     3117 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote/service/tag_service.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.115063 xnote-web-0.1.0/xnote_migrate/
+-rw-rw-rw-   0        0        0      887 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/__init__.py
+-rw-rw-rw-   0        0        0     3007 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/base.py
+-rw-rw-rw-   0        0        0      473 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_000.py
+-rw-rw-rw-   0        0        0     1314 2023-11-05 02:18:54.000000 xnote-web-0.1.0/xnote_migrate/upgrade_001.py
+-rw-rw-rw-   0        0        0     1359 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_002.py
+-rw-rw-rw-   0        0        0     2341 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_003.py
+-rw-rw-rw-   0        0        0      661 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_004.py
+-rw-rw-rw-   0        0        0      826 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_005.py
+-rw-rw-rw-   0        0        0      472 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_006.py
+-rw-rw-rw-   0        0        0      729 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_007.py
+-rw-rw-rw-   0        0        0      459 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_008.py
+-rw-rw-rw-   0        0        0      994 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_009.py
+-rw-rw-rw-   0        0        0     1321 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_010.py
+-rw-rw-rw-   0        0        0     1413 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_011.py
+-rw-rw-rw-   0        0        0     2974 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_012.py
+-rw-rw-rw-   0        0        0      604 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_013.py
+-rw-rw-rw-   0        0        0      922 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_014.py
+-rw-rw-rw-   0        0        0     2595 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_015.py
+-rw-rw-rw-   0        0        0     2292 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xnote_migrate/upgrade_016.py
+-rw-rw-rw-   0        0        0    11779 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xnote_migrate/upgrade_017.py
+-rw-rw-rw-   0        0        0     7433 2024-04-05 10:58:27.000000 xnote-web-0.1.0/xnote_migrate/upgrade_018.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.132260 xnote-web-0.1.0/xnote_web.egg-info/
+-rw-rw-rw-   0        0        0     5759 2024-05-03 04:09:04.000000 xnote-web-0.1.0/xnote_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    35173 2024-05-03 04:09:06.000000 xnote-web-0.1.0/xnote_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 04:09:05.000000 xnote-web-0.1.0/xnote_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-03 04:09:05.000000 xnote-web-0.1.0/xnote_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.230408 xnote-web-0.1.0/xutils/
+-rw-rw-rw-   0        0        0     9355 2024-05-02 13:42:29.000000 xnote-web-0.1.0/xutils/__init__.py
+-rw-rw-rw-   0        0        0     1799 2024-04-05 11:12:15.000000 xnote-web-0.1.0/xutils/base.py
+-rw-rw-rw-   0        0        0    23004 2024-04-12 15:08:43.000000 xnote-web-0.1.0/xutils/cacheutil.py
+-rw-rw-rw-   0        0        0      274 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/csvutil.py
+-rw-rw-rw-   0        0        0    10684 2024-04-27 04:44:35.000000 xnote-web-0.1.0/xutils/dateutil.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.388116 xnote-web-0.1.0/xutils/db/
+-rw-rw-rw-   0        0        0      128 2022-03-19 02:03:55.000000 xnote-web-0.1.0/xutils/db/__init__.py
+-rw-rw-rw-   0        0        0     6574 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/binlog.py
+-rw-rw-rw-   0        0        0    27014 2024-04-20 08:17:52.000000 xnote-web-0.1.0/xutils/db/dbutil_base.py
+-rw-rw-rw-   0        0        0     3699 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/dbutil_cache.py
+-rw-rw-rw-   0        0        0     4774 2023-06-30 12:24:59.000000 xnote-web-0.1.0/xutils/db/dbutil_deque.py
+-rw-rw-rw-   0        0        0     7165 2024-04-13 13:46:10.000000 xnote-web-0.1.0/xutils/db/dbutil_hash.py
+-rw-rw-rw-   0        0        0      697 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/dbutil_helper.py
+-rw-rw-rw-   0        0        0     4006 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/db/dbutil_id_gen.py
+-rw-rw-rw-   0        0        0     2692 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/dbutil_set.py
+-rw-rw-rw-   0        0        0     8502 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/dbutil_sortedset.py
+-rw-rw-rw-   0        0        0    30513 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/db/dbutil_table.py
+-rw-rw-rw-   0        0        0    11927 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/db/dbutil_table_index.py
+-rw-rw-rw-   0        0        0    13903 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/db/dbutil_table_v2.py
+-rw-rw-rw-   0        0        0     1941 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/driver_leveldb.py
+-rw-rw-rw-   0        0        0     4696 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/driver_leveldbpy.py
+-rw-rw-rw-   0        0        0     9596 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/driver_lmdb.py
+-rw-rw-rw-   0        0        0    17289 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/db/driver_mysql.py
+-rw-rw-rw-   0        0        0     3280 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/driver_mysql_enhance.py
+-rw-rw-rw-   0        0        0    11514 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/driver_sqlite.py
+-rw-rw-rw-   0        0        0     4064 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/driver_ssdb.py
+-rw-rw-rw-   0        0        0     7816 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/encode.py
+-rw-rw-rw-   0        0        0     2374 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/db/filters.py
+-rw-rw-rw-   0        0        0     2690 2023-04-06 04:04:41.000000 xnote-web-0.1.0/xutils/db/lock.py
+-rw-rw-rw-   0        0        0     4615 2022-05-17 15:05:38.000000 xnote-web-0.1.0/xutils/db/shard.py
+-rw-rw-rw-   0        0        0     1908 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/dbutil.py
+-rw-rw-rw-   0        0        0     9214 2023-11-11 11:01:44.000000 xnote-web-0.1.0/xutils/exeutil.py
+-rw-rw-rw-   0        0        0    23736 2024-05-03 04:01:25.000000 xnote-web-0.1.0/xutils/fsutil.py
+-rw-rw-rw-   0        0        0     1837 2022-01-25 14:37:52.000000 xnote-web-0.1.0/xutils/func_util.py
+-rw-rw-rw-   0        0        0     9109 2024-04-27 04:46:04.000000 xnote-web-0.1.0/xutils/functions.py
+-rw-rw-rw-   0        0        0     1080 2021-10-01 10:27:00.000000 xnote-web-0.1.0/xutils/htmlutil.py
+-rw-rw-rw-   0        0        0     4008 2024-04-05 10:56:40.000000 xnote-web-0.1.0/xutils/imports.py
+-rw-rw-rw-   0        0        0     7853 2024-04-20 12:48:58.000000 xnote-web-0.1.0/xutils/interfaces.py
+-rw-rw-rw-   0        0        0      896 2024-05-01 16:02:36.000000 xnote-web-0.1.0/xutils/jsonutil.py
+-rw-rw-rw-   0        0        0      317 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/lists.py
+-rw-rw-rw-   0        0        0     2410 2024-04-20 13:08:53.000000 xnote-web-0.1.0/xutils/lockutil.py
+-rw-rw-rw-   0        0        0    11834 2023-06-30 12:24:59.000000 xnote-web-0.1.0/xutils/logutil.py
+-rw-rw-rw-   0        0        0     3426 2023-04-16 02:40:02.000000 xnote-web-0.1.0/xutils/mem_util.py
+-rw-rw-rw-   0        0        0    10953 2023-12-02 11:46:25.000000 xnote-web-0.1.0/xutils/netutil.py
+-rw-rw-rw-   0        0        0      216 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/numutil.py
+-rw-rw-rw-   0        0        0    30698 2023-03-04 06:34:27.000000 xnote-web-0.1.0/xutils/six.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.405963 xnote-web-0.1.0/xutils/sqldb/
+-rw-rw-rw-   0        0        0      382 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/sqldb/__init__.py
+-rw-rw-rw-   0        0        0      728 2024-04-05 04:05:21.000000 xnote-web-0.1.0/xutils/sqldb/table_config.py
+-rw-rw-rw-   0        0        0    13227 2024-04-05 04:46:39.000000 xnote-web-0.1.0/xutils/sqldb/table_manager.py
+-rw-rw-rw-   0        0        0    10228 2024-04-21 14:00:24.000000 xnote-web-0.1.0/xutils/sqldb/table_proxy.py
+-rw-rw-rw-   0        0        0      450 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/sqldb/utils.py
+-rw-rw-rw-   0        0        0    18969 2024-05-03 04:05:40.000000 xnote-web-0.1.0/xutils/text_parser.py
+-rw-rw-rw-   0        0        0     2741 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/text_parser_properties.py
+-rw-rw-rw-   0        0        0    23168 2024-04-04 03:39:24.000000 xnote-web-0.1.0/xutils/textutil.py
+-rw-rw-rw-   0        0        0      651 2023-03-04 06:34:27.000000 xnote-web-0.1.0/xutils/textutil_url.py
+-rw-rw-rw-   0        0        0     7496 2023-01-22 10:01:14.000000 xnote-web-0.1.0/xutils/tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 04:09:11.422935 xnote-web-0.1.0/xutils/tornado/
+-rw-rw-rw-   0        0        0        0 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/tornado/__init__.py
+-rw-rw-rw-   0        0        0    14538 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/tornado/escape.py
+-rw-rw-rw-   0        0        0    10906 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/tornado/log.py
+-rw-rw-rw-   0        0        0    37310 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/tornado/template.py
+-rw-rw-rw-   0        0        0    13605 2023-10-27 13:17:40.000000 xnote-web-0.1.0/xutils/tornado/util.py
+-rw-rw-rw-   0        0        0     8287 2024-03-16 14:56:20.000000 xnote-web-0.1.0/xutils/webutil.py
+-rw-rw-rw-   0        0        0     2394 2024-04-29 17:03:11.000000 xnote-web-0.1.0/xutils/ziputil.py
```

### Comparing `xnote-web-0.0.9/COPYING` & `xnote-web-0.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/PKG-INFO` & `xnote-web-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnote-web
-Version: 0.0.9
+Version: 0.1.0
 Summary: xnote-web框架
 Author: mark
 Author-email: 578749341@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `xnote-web-0.0.9/README.md` & `xnote-web-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/boot/boot.default.properties` & `xnote-web-0.1.0/config/boot/boot.default.properties`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,18 @@
 db_profile_table_proxy = false
 db_profile_table_proxy.type = bool
 
 # 系统日志最大长度
 db_sys_log_max_size = 10000
 db_sys_log_max_size.type = int
 
+# 自动触发DDL
+db_auto_ddl = true
+db_auto_ddl.type = bool
+
 # leveldb缓存配置
 block_cache_size = 16777216 # 16M
 block_cache_size.type = int
 
 # leveldb的写入缓冲配置(MemTable的大小)
 write_buffer_size = 4194304 # 4M
 write_buffer_size.type = int
```

### Comparing `xnote-web-0.0.9/config/boot/boot.local.leveldb.properties` & `xnote-web-0.1.0/config/boot/boot.local.leveldb.properties`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/boot/boot.local.properties` & `xnote-web-0.1.0/config/boot/boot.local.properties`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 fast_reload = true
 
 # 是否开启WEBDAV
 webdav = false
 
 # 数据库驱动
 db_driver = sqlite
+record_db_name = $temp
 db_profile_table_proxy = true
 db_profile_table_proxy.type = bool
 
 # leveldb配置
 block_cache_size = 1
 write_buffer_size = 1
 max_open_files = 10
```

### Comparing `xnote-web-0.0.9/config/cron/cron.json` & `xnote-web-0.1.0/config/cron/cron.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/file/text.properties` & `xnote-web-0.1.0/config/file/text.properties`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/lang/en.properties` & `xnote-web-0.1.0/config/lang/en.properties`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/lang/zh.properties` & `xnote-web-0.1.0/config/lang/zh.properties`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/note/smart_group.ini` & `xnote-web-0.1.0/config/note/smart_group.ini`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/plugin/form_plugin.tpl.py` & `xnote-web-0.1.0/config/plugin/form_plugin.tpl.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/plugin/plugin.tpl.py` & `xnote-web-0.1.0/config/plugin/plugin.tpl.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/config/user/user_config.default.properties` & `xnote-web-0.1.0/config/user/user_config.default.properties`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/architecture.md` & `xnote-web-0.1.0/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/changelog.md` & `xnote-web-0.1.0/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/code_style.md` & `xnote-web-0.1.0/docs/code_style.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/code_style_css.md` & `xnote-web-0.1.0/docs/code_style_css.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/commands.md` & `xnote-web-0.1.0/docs/commands.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/database.md` & `xnote-web-0.1.0/docs/database.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/db_migrate.md` & `xnote-web-0.1.0/docs/db_migrate.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/plugins.md` & `xnote-web-0.1.0/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/architecture.png` & `xnote-web-0.1.0/docs/screenshots/architecture.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/architecture.svg` & `xnote-web-0.1.0/docs/screenshots/architecture.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/architecture_2.png` & `xnote-web-0.1.0/docs/screenshots/architecture_2.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/command_listdir.png` & `xnote-web-0.1.0/docs/screenshots/command_listdir.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/command_rmfolder.png` & `xnote-web-0.1.0/docs/screenshots/command_rmfolder.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/screenshot01.png` & `xnote-web-0.1.0/docs/screenshots/screenshot01.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/screenshot02.png` & `xnote-web-0.1.0/docs/screenshots/screenshot02.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/screenshot03.png` & `xnote-web-0.1.0/docs/screenshots/screenshot03.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/task_web.PNG` & `xnote-web-0.1.0/docs/screenshots/task_web.PNG`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.2_editor.PNG` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.2_editor.PNG`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.2_list.PNG` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.2_list.PNG`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.2_mobile.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.2_mobile.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.2_search.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.2_search.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.3_desktop01.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.3_desktop01.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.4.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.4.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v1.5.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v1.5.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.0.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.0.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.1_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.1_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.2_20190331.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.2_20190331.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.3_20190411.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.3_20190411.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.3_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.3_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.4_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.4_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.4_home2.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.4_home2.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.5_20200502.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.5_20200502.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.5_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.5_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.5_recent.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.5_recent.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.6_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.6_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.7_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.7_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.8_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.8_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v2.9.2_home.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v2.9.2_home.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote_v20191111.png` & `xnote-web-0.1.0/docs/screenshots/xnote_v20191111.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/docs/screenshots/xnote架构.png` & `xnote-web-0.1.0/docs/screenshots/xnote架构.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/admin/func_admin.py` & `xnote-web-0.1.0/handlers/admin/func_admin.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/admin/job_admin.py` & `xnote-web-0.1.0/handlers/admin/job_admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2024-03-10 22:56:56
 @LastEditors  : xupingmao
-@LastEditTime : 2024-03-31 11:21:40
+@LastEditTime : 2024-04-20 16:50:19
 @FilePath     : /xnote/handlers/admin/job_admin.py
 @Description  : 描述
 """
-
+import time
 from xnote.core.xtemplate import BasePlugin
 from xutils import Storage
 from xutils import webutil
 from xnote.plugin import DataTable, DataForm
 from xnote.service import JobService, SysJob, JobStatusEnum
 from xnote.core import xauth
+from xutils import dateutil
 import xutils
 import json
 
 HTML = r"""
 <div class="card">
     {% include common/table/table.html %}
 </div>
@@ -66,17 +67,17 @@
         job_id = xutils.get_argument_int("job_id")
         job_info = JobService.get_job_by_id(job_id=job_id)
         kw = Storage()
         kw.job_info = xutils.tojson(xutils.obj2dict(job_info), format=True)
 
         if job_info != None:
             form = DataForm()
-            form.add_row("ID", "id", value=str(job_info.id))
-            form.add_row("创建时间", "ctime", value=job_info.ctime)
-            form.add_row("更新时间", "mtime", value=job_info.mtime)
+            form.add_row("ID", "id", value=str(job_info.id), readonly=True)
+            form.add_row("创建时间", "ctime", value=job_info.ctime, readonly=True)
+            form.add_row("更新时间", "mtime", value=job_info.mtime, readonly=True)
             
             row = form.add_row("任务类型", "job_type", value=str(job_info.job_type), type="select")
             row.add_option("数据库备份", "db_backup")
             row.add_option("测试", "test")
             
             form.add_row("任务参数", "job_params", value=job_info.job_params, type="textarea")
             form.add_row("任务结果", "job_result", value=job_info.job_result, type="textarea")
@@ -134,15 +135,15 @@
         
         for job_info in job_list:
             row = job_info.__dict__
             row["status_title"] = JobStatusEnum.get_title_by_status(job_info.job_status)
             row["view_url"] = f"?action=view&job_id={job_info.id}"
             row["edit_url"] = f"?action=edit&job_id={job_info.id}"
             row["delete_url"] = f"?action=delete&job_id={job_info.id}"
-            row["delete_msg"] = "确认删除记录吗?"
+            row["delete_msg"] = f"确认删除记录【{job_info.id}】吗?"
             table.add_row(row)
         
         pagination = webutil.Pagination(page=1, total=total)
         kw = Storage()
         kw.table = table
         kw.page = page
         kw.page_max = pagination.page_max
@@ -154,14 +155,16 @@
 class JobTestHandler:
     
     @xauth.login_required("admin")
     def GET(self):
         job_info = SysJob()
         job_info.job_type = "test"
         with JobService.run_with_job(job_info):
+            time.sleep(1)
             job_info.job_result = "success"
+            job_info.mtime = dateutil.format_datetime()
         return webutil.SuccessResult()
     
 xurls = (
     r"/admin/jobs", JobHandler,
     r"/admin/test_job", JobTestHandler
 )
```

### Comparing `xnote-web-0.0.9/handlers/api/alarm.py` & `xnote-web-0.1.0/handlers/api/alarm.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/check_network.py` & `xnote-web-0.1.0/handlers/api/check_network.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/getip.py` & `xnote-web-0.1.0/handlers/api/getip.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/ipv6.py` & `xnote-web-0.1.0/handlers/api/ipv6.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/readbook.py` & `xnote-web-0.1.0/handlers/api/readbook.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/report_time.py` & `xnote-web-0.1.0/handlers/api/report_time.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/report_weather.py` & `xnote-web-0.1.0/handlers/api/report_weather.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/api/tts.py` & `xnote-web-0.1.0/handlers/api/tts.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/code_edit.html` & `xnote-web-0.1.0/handlers/code/code_edit.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/code_edit.py` & `xnote-web-0.1.0/handlers/code/code_edit.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/code_lines.html` & `xnote-web-0.1.0/handlers/code/code_lines.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/code_lines.py` & `xnote-web-0.1.0/handlers/code/code_lines.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/code_search.html` & `xnote-web-0.1.0/handlers/code/code_search.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/code_search.py` & `xnote-web-0.1.0/handlers/code/code_search.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/preview.html` & `xnote-web-0.1.0/handlers/code/preview.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/preview.py` & `xnote-web-0.1.0/handlers/code/preview.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/code/wiki_edit.html` & `xnote-web-0.1.0/handlers/code/wiki_edit.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/base/pagination.html` & `xnote-web-0.1.0/handlers/common/base/pagination.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/base.html` & `xnote-web-0.1.0/handlers/common/base.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/base_footer.html` & `xnote-web-0.1.0/handlers/common/base_footer.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/base_head.html` & `xnote-web-0.1.0/handlers/common/base_head.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/base_nav.html` & `xnote-web-0.1.0/handlers/common/base_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/base_title.html` & `xnote-web-0.1.0/handlers/common/base_title.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/date/month_picker.html` & `xnote-web-0.1.0/handlers/common/date/month_picker.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/form/form.html` & `xnote-web-0.1.0/handlers/common/form/form.html`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 <div class="form-body">
     <form id="xnoteForm{{_xnote_form.id}}">
         {% for row in _xnote_form.rows %}
             <div class="form-row {{row.css_class}}">
                 <label>{{row.title}}</label>
                 {% if row.type == "input" %}
-                    <input type="text" name="{{row.field}}" placeholder="{{row.placeholder}}" value="{{row.value}}">
+                    <input type="text" name="{{row.field}}" placeholder="{{row.placeholder}}" value="{{row.value}}" {{row.get_readonly_attr()}}>
                 {% end %}
                 {% if row.type == "textarea" %}
                     <textarea name="{{row.field}}" placeholder="{{row.placeholder}}">{{row.value}}</textarea>
                 {% end %}
                 {% if row.type == "select" %}
                     <select name="{{row.field}}" value="{{row.value}}">
                         {% for option in row.options %}
```

### Comparing `xnote-web-0.0.9/handlers/common/hook/search_box_hook.html` & `xnote-web-0.1.0/handlers/common/hook/search_box_hook.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/layout/base_layout.html` & `xnote-web-0.1.0/handlers/common/layout/base_layout.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/mod_notice.html` & `xnote-web-0.1.0/handlers/common/mod_notice.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/nav/base_nav_left.html` & `xnote-web-0.1.0/handlers/common/nav/base_nav_left.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/nav/base_nav_project.html` & `xnote-web-0.1.0/handlers/common/nav/base_nav_project.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/nav/base_nav_top.html` & `xnote-web-0.1.0/handlers/common/nav/base_nav_top.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/nav/content_nav.html` & `xnote-web-0.1.0/handlers/common/nav/content_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/pagination.html` & `xnote-web-0.1.0/handlers/common/pagination.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/script/adjust.html` & `xnote-web-0.1.0/handlers/common/script/adjust.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/script/geo_location.html` & `xnote-web-0.1.0/handlers/common/script/geo_location.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/script/image_fix_2.html` & `xnote-web-0.1.0/handlers/common/script/image_fix_2.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/script/require_init.html` & `xnote-web-0.1.0/handlers/common/script/require_init.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/script/textarea_script.html` & `xnote-web-0.1.0/handlers/common/script/textarea_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/search/search_box.html` & `xnote-web-0.1.0/handlers/common/search/search_box.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/search/search_mobile.html` & `xnote-web-0.1.0/handlers/common/search/search_mobile.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/sidebar/app_index.html` & `xnote-web-0.1.0/handlers/common/sidebar/app_index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/table/table.html` & `xnote-web-0.1.0/handlers/common/table/table.html`

 * *Files 20% similar despite different names*

```diff
@@ -13,38 +13,40 @@
             <th>操作</th>
         {% end %}
     </tr>
 
     {% for row in _xnote_table.rows %}
         <tr class="hover-tr">
             {% for head in _xnote_table.heads %}
-                {% if head.link_field != "" %}
-                <td><a href="{{row.get(head.link_field)}}">{{row.get(head.field)}}</a></td>
+                <td class="{{head.get_css_class(row)}}">
+                {% if head.has_link(row) %}
+                    <a href="{{head.get_link(row)}}">{{row.get(head.field)}}</a></td>
                 {% else %}
-                <td>{{row.get(head.field)}}</td>
+                    {{row.get(head.field)}}
                 {% end %}
+                </td>
             {% end %} 
 
             {% if len(_xnote_table.actions) > 0 %}
                 <td>
                     {% for action in _xnote_table.actions %}
-                        {% if action.type == "link" %}
-                            <a href="{{row.get(action.link_field)}}">{{action.title}}</a>
+                        {% if action.type == "link" and action.get_link(row) != None %}
+                            <a href="{{action.get_link(row)}}">{{action.title}}</a>
                         {% end %}
-                        {% if action.type == "button" %}
+                        {% if action.type == "button" and action.get_link(row) != None %}
                             <button class="btn-default {{action.css_class}}" onclick="xnote.table.handleAction(this)" 
-                            data-url="{{row.get(action.link_field)}}" data-title="{{action.get_title(row)}}">{{action.get_title(row)}}</button>
+                            data-url="{{action.get_link(row)}}" data-title="{{action.get_title(row)}}">{{action.get_title(row)}}</button>
                         {% end %}
-                        {% if action.type == "confirm" %}
+                        {% if action.type == "confirm" and action.get_link(row) != None %}
                             <button class="btn-default {{action.css_class}}" onclick="xnote.table.handleConfirmAction(this)" 
-                            data-url="{{row.get(action.link_field)}}" data-msg="{{action.get_msg(row)}}">{{action.get_title(row)}}</button>
+                            data-url="{{action.get_link(row)}}" data-msg="{{action.get_msg(row)}}">{{action.get_title(row)}}</button>
                         {% end %}
-                        {% if action.type == "edit_form" %}
+                        {% if action.type == "edit_form" and action.get_link(row) != None %}
                             <button class="btn-default {{action.css_class}}" onclick="xnote.table.handleEditForm(this)"
-                            data-url="{{row.get(action.link_field)}}" data-title="{{action.get_title(row)}}">{{action.get_title(row)}}</button>
+                            data-url="{{action.get_link(row)}}" data-title="{{action.get_title(row)}}">{{action.get_title(row)}}</button>
                         {% end %}
                     {% end %}
                 </td>
             {% end %}
         </tr>
     {% end %}
 </table>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 {% init xnote_table_var = "table" %} {% set _xnote_table = globals()
 [xnote_table_var] %}
-{{{{hheeaadd..ttiittllee}}}}          ?æ???ä?½?
-                                                {% for action in
-                                                _xnote_table.actions %} {% if
-                                                action.type == "link" %} _{
-                                                _{_a_c_t_i_o_n_._t_i_t_l_e_}_} {% end %} {% if
-                                                action.type == "button" %} {
-_{_{_r_o_w_._g_e_t_(_h_e_a_d_._f_i_e_l_d_)_}_} {{row.get(head.field)}} {action.get_title(row)}} {% end
-                                                %} {% if action.type ==
-                                                "confirm" %} {{action.get_title
-                                                (row)}} {% end %} {% if
-                                                action.type == "edit_form" %} {
-                                                {action.get_title(row)}} {% end
-                                                %} {% end %}
+{{{{hheeaadd..ttiittllee}}}}                        ?æ???ä?½?
+                                      {% for action in _xnote_table.actions %}
+                                      {% if action.type == "link" and
+                                      action.get_link(row) != None %} _{
+                                      _{_a_c_t_i_o_n_._t_i_t_l_e_}_} {% end %} {% if
+                                      action.type == "button" and
+                                      action.get_link(row) != None %} {
+{% if head.has_link(row) %} _{_{_r_o_w_._g_e_t {action.get_title(row)}} {% end %} {% if
+_(_h_e_a_d_._f_i_e_l_d_)_}_}                        action.type == "confirm" and
+                                      action.get_link(row) != None %} {
+                                      {action.get_title(row)}} {% end %} {% if
+                                      action.type == "edit_form" and
+                                      action.get_link(row) != None %} {
+                                      {action.get_title(row)}} {% end %} {% end
+                                      %}
```

### Comparing `xnote-web-0.0.9/handlers/common/theme/sidebar.html` & `xnote-web-0.1.0/handlers/common/theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/common/theme/sidebar_left.html` & `xnote-web-0.1.0/handlers/common/theme/sidebar_left.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/cron/cron_stats.py` & `xnote-web-0.1.0/handlers/cron/cron_stats.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/cron/diskclean.py` & `xnote-web-0.1.0/handlers/cron/diskclean.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/component/dict_sidebar.html` & `xnote-web-0.1.0/handlers/dict/component/dict_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/dao_relevant.py` & `xnote-web-0.1.0/handlers/dict/dao_relevant.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/dict.py` & `xnote-web-0.1.0/handlers/dict/dict.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/dict_dao.py` & `xnote-web-0.1.0/handlers/dict/dict_dao.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/dict_relevant.py` & `xnote-web-0.1.0/handlers/dict/dict_relevant.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/page/dict_add.html` & `xnote-web-0.1.0/handlers/dict/page/dict_add.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/page/dict_edit.html` & `xnote-web-0.1.0/handlers/dict/page/dict_edit.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/page/dict_list.html` & `xnote-web-0.1.0/handlers/dict/page/dict_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/page/dict_update.html` & `xnote-web-0.1.0/handlers/dict/page/dict_update.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/dict/page/relevant_list.html` & `xnote-web-0.1.0/handlers/dict/page/relevant_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/error.html` & `xnote-web-0.1.0/handlers/error.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/clipboard-dialog.html` & `xnote-web-0.1.0/handlers/fs/component/clipboard-dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/filelist_gallery.html` & `xnote-web-0.1.0/handlers/fs/component/filelist_gallery.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/filelist_simple.html` & `xnote-web-0.1.0/handlers/fs/component/filelist_simple.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 {% import os %}
 {% from xutils import fsutil %}
 {% init show_rename_file_link = True %}
 
 <table class="table row">
+    <tr>
+        <th>文件名</th>
+        <th>文件大小</th>
+        <th>操作</th>
+    </tr>
     {% for fpath in pathlist %}
         {% set fname = os.path.basename(fpath) %}
         {% set display_name = fsutil.get_display_name(fpath, dirname) %}
-        <tr>
+        <tr class="hover-tr">
             <td class="option-name"><a href="{{fsutil.get_webpath(fpath)}}">{{display_name}}</a></td>
             <td class="option-td">
                 {{xutils.format_file_size(fpath)}}
             </td>
             <td class="option-td">
                 <div class="float-right">
                     {% if show_rename_file_link %}
-                        <a class="rename-btn" data-name="{{display_name}}" 
+                        <a class="btn btn-default" data-name="{{display_name}}" 
                             onclick="xnote.action.fs.rename(this);">重命名</a>
                     {% end %}
-                    <a class="danger-link" data-path="{{fpath}}" data-name="{{display_name}}" 
+                    <a class="btn danger" data-path="{{fpath}}" data-name="{{display_name}}" 
                         onclick="xnote.action.fs.delete(this);">删除</a>
                 </div>
             </td>
         </tr>
     {% end %}
 </table>
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 {% import os %} {% from xutils import fsutil %} {% init show_rename_file_link =
 True %}
+?æ???ä?»?¶?å??        ?æ???ä?»?¶?å?¤?§?å?°?              ?æ???ä?½?
 _{_{_d_i_s_p_l_a_y___n_a_m_e_}_} {{xutils.format_file_size {% if show_rename_file_link %}
                  (fpath)}}                 éå½å {% end %} å é¤
```

### Comparing `xnote-web-0.0.9/handlers/fs/component/fs_sidebar.html` & `xnote-web-0.1.0/handlers/fs/component/fs_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/move_file_dialog.html` & `xnote-web-0.1.0/handlers/fs/component/move_file_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/options/fs_options.html` & `xnote-web-0.1.0/handlers/fs/component/options/fs_options.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/options/fs_options_buttons.html` & `xnote-web-0.1.0/handlers/fs/component/options/fs_options_buttons.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/options/fs_options_buttons.mobile.html` & `xnote-web-0.1.0/handlers/fs/component/options/fs_options_buttons.mobile.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/options_css.html` & `xnote-web-0.1.0/handlers/fs/component/options_css.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/plugins-dialog.html` & `xnote-web-0.1.0/handlers/fs/component/plugins-dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/component/script/file_op_script.html` & `xnote-web-0.1.0/handlers/fs/component/script/file_op_script.html`

 * *Files 5% similar despite different names*

```diff
@@ -5,52 +5,39 @@
 {% include fs/component/move_file_dialog.html %}
 
 <input type="hidden" id="currentPath" value="{{path}}">
 
 <script type="text/template" id="fileItemOptionDialog">
     <div class="card">
         <div class="align-center">
-            <button class="btn btn-default large" data-path="{{!filePath}}" 
+            <button class="btn btn-default huge" data-path="{{!filePath}}" 
                 onclick="xnote.action.fs.download(this);">下载</button>
-            <button class="btn btn-default large" 
+            <button class="btn btn-default huge" 
                 data-path="{{!filePath}}" 
                 data-name="{{!fileName}}"
+                data-realname="{{!fileRealName}}"
                 onclick="xnote.action.fs.rename(this);">重命名</button>
-            <button class="btn btn-default large" 
+            <button class="btn btn-default huge" 
                 data-path="{{!filePath}}"
                 data-name="{{!fileName}}"
+                data-realname="{{!fileRealName}}"
                 onclick="xnote.action.fs.delete(this);">删除</button>
-            <button class="btn btn-default large"
+            <button class="btn btn-default huge"
                 data-path="{{!filePath}}"
                 onclick="xnote.action.fs.move(this);">移动</button>
-            <button class="btn btn-default large"
+            <button class="btn btn-default huge"
                 onclick="xnote.action.fs.copy(this);">复制</button>
-            <button class="btn btn-default large"
+            <button class="btn btn-default huge"
                 onclick="xnote.action.fs.showDetail(this);">详细信息</button>
         </div>
     </div>
 </script>
 
 <script type="text/javascript">
 
-xnote.action.fs.openOptionDialog = function (target) {
-    console.log(window.event);
-    window.event.preventDefault();
-    window.event.stopPropagation();
-    console.log(target);
-    var filePath = $(target).attr("data-path");
-    var fileName = $(target).attr("data-name");
-    var html = $("#fileItemOptionDialog").render({
-        "filePath": filePath,
-        "fileName": fileName
-    });
-
-    xnote.openDialog("选项", html);
-};
-
 xnote.action.fs.download = function(target) {
     var path = $(target).attr("data-path");
     window.open("{{_server_home}}/fs/~" + path +"?type=blob", "_blank");
 };
 
 xnote.action.fs.move = function(target) {
     var path = $(target).attr("data-path");
```

### Comparing `xnote-web-0.0.9/handlers/fs/fs.py` & `xnote-web-0.1.0/handlers/fs/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 import sys
 import time
 import datetime
 
 import mimetypes
 import web
 import xutils
+import logging
+
 from xnote.core import xauth
 from xnote.core import xconfig
 from xnote.core import xtemplate
 from xnote.core import xmanager
-import logging
-import multiprocessing
 from xnote.core import xnote_event
 
 from xutils import FileItem, u, Storage, fsutil
 from xutils import dbutil
+from xutils import webutil
 from .fs_mode import get_fs_page_by_mode
 from .fs_helper import sort_files_by_size
 from . import fs_image
 from . import fs_helper
 
 def is_stared(path):
     return xconfig.has_config("STARED_DIRS", path)
@@ -123,14 +124,15 @@
         """Content-Type设置, 优先级从高到低依次是：参数配置、系统配置、默认配置"""
         type = xutils.get_argument_str("type")
         path = xutils.decode_name(path)
 
         if type == "text":
             web.header("Content-Type", 'text/plain; charset=utf-8')
             return
+        
         if type == "blob":
             web.header("Content-Type", self.mime_types[""])
             fname = os.path.basename(path)
             fname = xutils.quote_unicode(fname)
             web.header("Content-Disposition", "attachment; filename=\"%s\"" % fname)
             return
         
@@ -433,38 +435,38 @@
     def GET(self):
         return self.POST()
 
 class RenameAjaxHandler:
 
     @xauth.login_required("admin")
     def POST(self):
-        dirname  = xutils.get_argument("dirname")
-        old_name = xutils.get_argument("old_name", "")
-        new_name = xutils.get_argument("new_name", "")
+        dirname  = xutils.get_argument_str("dirname")
+        old_name = xutils.get_argument_str("old_name", "")
+        new_name = xutils.get_argument_str("new_name", "")
         user_info = xauth.current_user()
         assert user_info != None
 
         user_name = user_info.name
 
-        assert isinstance(old_name, str)
-        assert isinstance(new_name, str)
-        assert isinstance(dirname, str)
-
         if dirname is None or dirname == "":
             return dict(code="fail", message="dirname is blank")
+        
         if old_name is None or old_name == "":
             return dict(code="fail", message="old_name is blank")
 
         if ".." in new_name:
             return dict(code="fail", message="invalid new name")
+        
         if new_name == "":
-            new_name = os.path.basename(old_name)
+            return webutil.FailedResult(code="400", message="新的文件名称为空")
+        
+        logging.info("encode_name=%s, new_name=%s", xconfig.USE_URLENCODE, new_name)
+
         if xconfig.USE_URLENCODE:
-            old_name = xutils.quote_unicode(old_name)
-            new_name = xutils.quote_unicode(new_name)
+            new_name = fsutil.get_safe_file_name(new_name)
 
         old_path = os.path.join(dirname, old_name)
         new_path = os.path.join(dirname, new_name)
 
         # 获取真实的路径
         old_path = xutils.get_real_path(old_path)
 
@@ -529,15 +531,15 @@
     def GET(self):
         return self.POST()
 
 class ListAjaxHandler:
 
     @xauth.login_required("admin")
     def GET(self):
-        fpath = xutils.get_argument("fpath")
+        fpath = xutils.get_argument_str("fpath")
         show_parent = xutils.get_argument_str("show_parent")
 
         if fpath == "" or fpath == None:
             return dict(code = "400", message = u"fpath参数为空")
 
         if not os.path.exists(fpath):
             return dict(code = "404", message = u"文件不存在")
```

### Comparing `xnote-web-0.0.9/handlers/fs/fs_add.py` & `xnote-web-0.1.0/handlers/fs/fs_add.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_api.py` & `xnote-web-0.1.0/handlers/fs/fs_api.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_cache.py` & `xnote-web-0.1.0/handlers/fs/fs_cache.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_find.py` & `xnote-web-0.1.0/handlers/fs/fs_find.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_helper.py` & `xnote-web-0.1.0/handlers/fs/fs_helper.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_hex.py` & `xnote-web-0.1.0/handlers/fs/fs_hex.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_image.py` & `xnote-web-0.1.0/handlers/fs/fs_image.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_index.py` & `xnote-web-0.1.0/handlers/fs/fs_index.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_mode.py` & `xnote-web-0.1.0/handlers/fs/fs_mode.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_plugins.py` & `xnote-web-0.1.0/handlers/fs/fs_plugins.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_preview.py` & `xnote-web-0.1.0/handlers/fs/fs_preview.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_text.py` & `xnote-web-0.1.0/handlers/fs/fs_text.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/fs_upload.py` & `xnote-web-0.1.0/handlers/fs/fs_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 from xnote.core import xconfig
 import xutils
 from xnote.core import xtemplate
 from xnote.core import xmanager
 import time
 import math
 from xutils import fsutil, Storage, dateutil
+from xutils import webutil
 from xnote.core.xtemplate import T
 from xnote.core.xnote_event import FileUploadEvent
 from .fs_helper import FileInfoDao
+from xutils.fsutil import get_safe_file_name
 try:
     from PIL import Image
 except ImportError:
     Image = None
 
 
 # 完整的元信息参考文档 https://zhuanlan.zhihu.com/p/366726838
@@ -29,21 +31,14 @@
 def get_link(filename, webpath):
     """返回Markdown的链接"""
     if xutils.is_img_file(filename):
         return "![%s](%s)" % (filename, webpath)
     return "[%s](%s)" % (filename, webpath)
 
 
-def get_safe_file_name(filename):
-    """处理文件名中的特殊符号"""
-    for c in " @$:#\\|=&?":
-        filename = filename.replace(c, "_")
-    return filename
-
-
 def generate_filename(filename, prefix="", ext=None):
     if prefix:
         prefix = prefix + '_'
     else:
         prefix = ""
 
     if filename is None:
@@ -118,15 +113,19 @@
 def get_user_upload_dir(user):
     return os.path.join(xconfig.UPLOAD_DIR, user)
 
 def get_upload_file_path(user, filename, upload_dir="files", rename_conflict=False):
     """生成上传文件名"""
     from xnote.core import xconfig
     if xconfig.USE_URLENCODE:
+        origin_filename = filename
         filename = xutils.quote_unicode(filename)
+        if origin_filename != filename:
+            filename = xutils.encode_name(filename)
+
     basename, ext = os.path.splitext(filename)
     date = time.strftime("upload/%Y/%m")
     dirname = os.path.join(xconfig.DATA_PATH, upload_dir, user, date)
     fsutil.makedirs(dirname)
 
     origin_filename = os.path.join(dirname, filename)
     fileindex = 1
@@ -146,52 +145,80 @@
                                              user, date, temp_filename)
         fileindex += 1
     return os.path.abspath(newfilepath), webpath
 
 
 class UploadHandler:
 
+    def get_recovery_path(self, fpath=""):
+        fpath = fpath.replace("$data", xconfig.FileConfig.data_dir)
+        return fpath, fsutil.get_webpath(fpath)
+
     @xauth.login_required()
     def POST(self):
+        try:
+            return self.do_post()
+        except Exception as e:
+            err_stack = xutils.print_exc()
+            err_msg = str(e)
+            if xauth.is_admin():
+                err_msg = err_stack
+            return webutil.FailedResult(code="500", message=err_msg)
+        
+    def do_post(self):
         file = xutils.get_argument_field_storage("file")
         prefix = xutils.get_argument_str("prefix")
         name = xutils.get_argument_str("name")
         note_id = xutils.get_argument_str("note_id")
+        upload_type = xutils.get_argument_str("upload_type")
+
         user_info = xauth.current_user()
         assert user_info != None
         user_name = user_info.name
         webpath = ""
         filename = ""
 
-        if file.filename != None:            
-            filename = get_safe_file_name(file.filename)
-            if file.filename == "":
-                return dict(code="400", message="filename is empty")
-            
-            basename, ext = os.path.splitext(filename)
-            if name == "auto":
-                # iOS上传文件截图文件固定是image.png
-                filename = generate_filename(None, prefix, ext)
-
+        if file.file is None:
+            return webutil.FailedResult(code="400", message="file.file is None")
+        
+        if file.filename is None:
+            return webutil.FailedResult(code="400", message="file.filename is None")
+        
+        filename = get_safe_file_name(file.filename)
+        basename, ext = os.path.splitext(filename)
+        if name == "auto":
+            # iOS上传文件截图文件固定是image.png
+            filename = generate_filename(None, prefix, ext)
+
+        if upload_type == "recovery":
+            if not xauth.is_admin():
+                return webutil.FailedResult(code="403", message="recovery mode is only allowed by admin")
+            filepath, webpath = self.get_recovery_path(filename)
+            dirs = os.path.dirname(filepath)
+            fsutil.makedirs(dirs)
+        else:
             filepath, webpath = get_upload_file_path(user_name, filename)
 
-            with open(filepath, "wb") as fout:
-                for chunk in file.file:
-                    fout.write(chunk)
-            
-            event = FileUploadEvent()
-            event.fpath = filepath
-            event.user_name = user_info.name
-            event.user_id = user_info.id
-            xmanager.fire("fs.upload", event)
+        with open(filepath, "wb") as fout:
+            for chunk in file.file:
+                fout.write(chunk)
+        
+        event = FileUploadEvent()
+        event.fpath = filepath
+        event.user_name = user_info.name
+        event.user_id = user_info.id
+        xmanager.fire("fs.upload", event)
 
-            try_fix_orientation(filepath)
-            try_touch_note(note_id)
+        try_fix_orientation(filepath)
+        try_touch_note(note_id)
 
-        return dict(code="success", webpath=webpath, link=get_link(filename, webpath))
+        result = webutil.SuccessResult()
+        result.webpath = webpath
+        result.link = get_link(filename, webpath)
+        return result
 
     @xauth.login_required()
     def GET(self):
         return self.get_upload_page_v1()
         
     def get_upload_page_v1(self):
         user_info = xauth.current_user()
@@ -244,14 +271,15 @@
         dest_path = os.path.join(dirname, filename)
         user_info = xauth.current_user()
         assert user_info != None
         user_name = user_info.name
 
         with open(dest_path, "wb") as fp:
             for chunk in range(chunks):
+                filename = get_safe_file_name(filename)
                 tmp_path = os.path.join(dirname, filename)
                 tmp_path = "%s_%d.part" % (tmp_path, chunk)
                 if not os.path.exists(tmp_path):
                     raise Exception("upload file broken")
                 with open(tmp_path, "rb") as tmp_fp:
                     fp.write(tmp_fp.read())
                 xutils.remove(tmp_path, True)
@@ -284,71 +312,78 @@
         dirname = dirname.replace("$DATA", xconfig.DATA_DIR)
         note_id = xutils.get_argument("note_id")
 
         # 不能访问上级目录
         if ".." in dirname:
             return dict(code="fail", message="can not access parent directory")
 
+        if not hasattr(file, "filename"):
+            return webutil.FailedResult(code="400", message="请选择文件")
+        
+        if file.file is None:
+            return webutil.FailedResult(code="400", message="file.file is None")
+
         filename = None
         webpath = ""
         origin_name = ""
         filepath = ""
 
-        if hasattr(file, "filename"):
-            origin_name = file.filename
-            xutils.trace("UploadFile", file.filename)
-            filename = os.path.basename(file.filename)
-            filename = get_safe_file_name(filename)
-            filename = xutils.get_real_path(filename)
-            if dirname == "auto":
-                filename = generate_filename(None, prefix)
-                filepath, webpath = get_upload_file_path(
-                    user_name, filename, rename_conflict=True)
-                dirname = os.path.dirname(filepath)
-                filename = os.path.basename(filepath)
-            else:
-                # check permission.
-                if xauth.current_role() != "admin":
-                    # 普通用户操作
-                    user_upload_dir = get_user_upload_dir(user_name)
-                    if not fsutil.is_parent_dir(user_upload_dir, dirname):
-                        return dict(code="403", message="无权操作")
-
-                filepath = os.path.join(dirname, filename)
-            
-            if self.is_fixed_name(origin_name):
-                filename = self.find_available_path(origin_name)
-                filepath = os.path.join(dirname, filename)
-
-            if chunk == 0:
-                lock = try_lock_file(filepath)
-
-            if os.path.exists(filepath):
-                # return dict(code = "fail", message = "文件已存在")
-                web.ctx.status = "500 Server Error"
-                return dict(code="fail", message="文件已存在")
-
-            if part_file:
-                tmp_name = "%s_%d.part" % (filename, chunk)
-                seek = 0
-            else:
-                tmp_name = filename
-                seek = chunk * chunksize
-
-            xutils.makedirs(dirname)
-            tmp_path = os.path.join(dirname, tmp_name)
-
-            with open(tmp_path, "wb") as fp:
-                fp.seek(seek)
-                if seek != 0:
-                    logging.info("seek to %s", seek)
-                for file_chunk in file.file:
-                    fp.write(file_chunk)
+        origin_name = file.filename
+        xutils.trace("UploadFile", file.filename)
+        if origin_name is None:
+            return webutil.FailedResult(code="400", message="file.filename is None")
+        
+        filename = os.path.basename(origin_name)
+        filename = get_safe_file_name(filename)
+
+        if dirname == "auto":
+            filename = generate_filename(None, prefix)
+            filepath, webpath = get_upload_file_path(
+                user_name, filename, rename_conflict=True)
+            dirname = os.path.dirname(filepath)
+            filename = os.path.basename(filepath)
         else:
-            return dict(code="fail", message=u"请选择文件")
+            # check permission.
+            if xauth.current_role() != "admin":
+                # 普通用户操作
+                user_upload_dir = get_user_upload_dir(user_name)
+                if not fsutil.is_parent_dir(user_upload_dir, dirname):
+                    return dict(code="403", message="无权操作")
+
+            filepath = os.path.join(dirname, filename)
+        
+        if self.is_fixed_name(origin_name):
+            filename = self.find_available_path(origin_name)
+            filepath = os.path.join(dirname, filename)
+
+        if chunk == 0:
+            lock = try_lock_file(filepath)
+
+        if os.path.exists(filepath):
+            # return dict(code = "fail", message = "文件已存在")
+            web.ctx.status = "500 Server Error"
+            return dict(code="fail", message="文件已存在")
+
+        if part_file:
+            tmp_name = "%s_%d.part" % (filename, chunk)
+            seek = 0
+        else:
+            tmp_name = filename
+            seek = chunk * chunksize
+
+        xutils.makedirs(dirname)
+        tmp_path = os.path.join(dirname, tmp_name)
+
+        with open(tmp_path, "wb") as fp:
+            fp.seek(seek)
+            if seek != 0:
+                logging.info("seek to %s", seek)
+            for file_chunk in file.file:
+                fp.write(file_chunk)
+        
         if part_file and chunk+1 == chunks:
             self.merge_files(dirname, filename, chunks)
 
         try_fix_orientation(filepath)
         try_touch_note(note_id)
 
         if note_id != None and note_id != "":
```

### Comparing `xnote-web-0.0.9/handlers/fs/mod_aside.html` & `xnote-web-0.1.0/handlers/fs/mod_aside.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/mod_fs_upload.html` & `xnote-web-0.1.0/handlers/fs/mod_fs_upload.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs.html` & `xnote-web-0.1.0/handlers/fs/page/fs.html`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                 {% if _item.show_opt_btn %}
                 <div class="float-right">
                     <span class="fs-size-span">{{_item.size}}</span>
                     <span>&nbsp;</span>
                     <button class="btn btn-default" 
                         data-path="{{_item.path}}"
                         data-name="{{_item.name}}"
+                        data-realname="{{_item.realname}}"
                         onclick="xnote.action.fs.openOptionDialog(this)">{{T("操作")}}</button>
                 </div>
                 {% end %}
             </a>
         {% end %}
     </div>
 </div>
```

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_bookmark.html` & `xnote-web-0.1.0/handlers/fs/page/fs_bookmark.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_grid.html` & `xnote-web-0.1.0/handlers/fs/page/fs_grid.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_index.html` & `xnote-web-0.1.0/handlers/fs/page/fs_index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_plugins.html` & `xnote-web-0.1.0/handlers/fs/page/fs_plugins.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_shell.html` & `xnote-web-0.1.0/handlers/fs/page/fs_shell.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_sidebar.html` & `xnote-web-0.1.0/handlers/fs/page/fs_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_text.html` & `xnote-web-0.1.0/handlers/fs/page/fs_text.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_text_v1.html` & `xnote-web-0.1.0/handlers/fs/page/fs_text_v1.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/fs/page/fs_upload.html` & `xnote-web-0.1.0/handlers/fs/page/fs_upload.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/index.html` & `xnote-web-0.1.0/handlers/index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/index.py` & `xnote-web-0.1.0/handlers/index.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/ajax/message_ajax.html` & `xnote-web-0.1.0/handlers/message/ajax/message_ajax.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/ajax/message_tag_ajax.html` & `xnote-web-0.1.0/handlers/message/ajax/message_tag_ajax.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/card/deleted_msg_left.html` & `xnote-web-0.1.0/handlers/message/card/deleted_msg_left.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/card/deleted_msg_left_new.html` & `xnote-web-0.1.0/handlers/message/card/deleted_msg_left_new.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/card/deleted_msg_right.html` & `xnote-web-0.1.0/handlers/message/card/deleted_msg_right.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/card/message_system_tag.html` & `xnote-web-0.1.0/handlers/message/card/message_system_tag.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/card/msg_edit_card.html` & `xnote-web-0.1.0/handlers/message/card/msg_edit_card.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_date_right.html` & `xnote-web-0.1.0/handlers/message/component/message_date_right.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_edit.html` & `xnote-web-0.1.0/handlers/message/component/message_edit.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_event.html` & `xnote-web-0.1.0/handlers/message/component/message_event.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_input.html` & `xnote-web-0.1.0/handlers/message/component/message_input.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_keyword_info.html` & `xnote-web-0.1.0/handlers/message/component/message_keyword_info.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_list.html` & `xnote-web-0.1.0/handlers/message/component/message_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_sub_link.html` & `xnote-web-0.1.0/handlers/message/component/message_sub_link.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_tab.html` & `xnote-web-0.1.0/handlers/message/component/message_tab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_tab_log.html` & `xnote-web-0.1.0/handlers/message/component/message_tab_log.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_tab_task.html` & `xnote-web-0.1.0/handlers/message/component/message_tab_task.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_tag_list.html` & `xnote-web-0.1.0/handlers/message/component/message_tag_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_title.html` & `xnote-web-0.1.0/handlers/message/component/message_title.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/message_todo_inner.html` & `xnote-web-0.1.0/handlers/message/component/message_todo_inner.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/right/tags.html` & `xnote-web-0.1.0/handlers/message/component/right/tags.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/script/tab_script.html` & `xnote-web-0.1.0/handlers/message/component/script/tab_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/select_topic_dialog.html` & `xnote-web-0.1.0/handlers/message/component/select_topic_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/show_topic_dialog.html` & `xnote-web-0.1.0/handlers/message/component/show_topic_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/component/tag/orderby_tab.html` & `xnote-web-0.1.0/handlers/message/component/tag/orderby_tab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/dao.py` & `xnote-web-0.1.0/handlers/message/dao.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/message.py` & `xnote-web-0.1.0/handlers/message/message.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/message_model.py` & `xnote-web-0.1.0/handlers/message/message_model.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/message_search.py` & `xnote-web-0.1.0/handlers/message/message_search.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/message_tag.py` & `xnote-web-0.1.0/handlers/message/message_tag.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/message_task.py` & `xnote-web-0.1.0/handlers/message/message_task.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/message_utils.py` & `xnote-web-0.1.0/handlers/message/message_utils.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message.html` & `xnote-web-0.1.0/handlers/message/page/message.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message_calendar.html` & `xnote-web-0.1.0/handlers/message/page/message_calendar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message_list_by_day.html` & `xnote-web-0.1.0/handlers/message/page/message_list_by_day.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message_list_view.html` & `xnote-web-0.1.0/handlers/message/page/message_list_view.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message_search.html` & `xnote-web-0.1.0/handlers/message/page/message_search.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message_tag_select.html` & `xnote-web-0.1.0/handlers/message/page/message_tag_select.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/message_tag_view.html` & `xnote-web-0.1.0/handlers/message/page/message_tag_view.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/old/dairy.html` & `xnote-web-0.1.0/handlers/message/page/old/dairy.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/old/message_calendar_old.html` & `xnote-web-0.1.0/handlers/message/page/old/message_calendar_old.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/message/page/task_index.html` & `xnote-web-0.1.0/handlers/message/page/task_index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/mod_fs_path.html` & `xnote-web-0.1.0/handlers/mod_fs_path.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/ajax/comment_edit_dialog.html` & `xnote-web-0.1.0/handlers/note/ajax/comment_edit_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/ajax/comment_list.html` & `xnote-web-0.1.0/handlers/note/ajax/comment_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/ajax/edit_symbol_dialog.html` & `xnote-web-0.1.0/handlers/note/ajax/edit_symbol_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/ajax/group_option_dialog.html` & `xnote-web-0.1.0/handlers/note/ajax/group_option_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/ajax/share_group_dialog.html` & `xnote-web-0.1.0/handlers/note/ajax/share_group_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/ajax/share_note_dialog.html` & `xnote-web-0.1.0/handlers/note/ajax/share_note_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/hot_notes.html` & `xnote-web-0.1.0/handlers/note/card/hot_notes.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/note_contents_left.html` & `xnote-web-0.1.0/handlers/note/card/note_contents_left.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/note_date_picker.html` & `xnote-web-0.1.0/handlers/note/card/note_date_picker.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/note_groups.html` & `xnote-web-0.1.0/handlers/note/card/note_groups.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/note_types.html` & `xnote-web-0.1.0/handlers/note/card/note_types.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/plan_note_card.html` & `xnote-web-0.1.0/handlers/note/card/plan_note_card.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/plan_sidebar.html` & `xnote-web-0.1.0/handlers/note/card/plan_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/recent_created_notes.html` & `xnote-web-0.1.0/handlers/note/card/recent_created_notes.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/recent_update_groups.html` & `xnote-web-0.1.0/handlers/note/card/recent_update_groups.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/recent_update_notes.html` & `xnote-web-0.1.0/handlers/note/card/recent_update_notes.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/sticky_notes.html` & `xnote-web-0.1.0/handlers/note/card/sticky_notes.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/card/task_memo.html` & `xnote-web-0.1.0/handlers/note/card/task_memo.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/comment.py` & `xnote-web-0.1.0/handlers/note/comment.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/attribute/note_category.html` & `xnote-web-0.1.0/handlers/note/component/attribute/note_category.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/batch_move.html` & `xnote-web-0.1.0/handlers/note/component/batch_move.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/create_note_header.html` & `xnote-web-0.1.0/handlers/note/component/create_note_header.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/css/edit_css.html` & `xnote-web-0.1.0/handlers/note/component/css/edit_css.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/css/gallery_css.html` & `xnote-web-0.1.0/handlers/note/component/css/gallery_css.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/detail_left.html` & `xnote-web-0.1.0/handlers/note/component/detail_left.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/editor_default_vars.html` & `xnote-web-0.1.0/handlers/note/component/editor/editor_default_vars.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/gallery.html` & `xnote-web-0.1.0/handlers/note/component/editor/gallery.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/markdown.html` & `xnote-web-0.1.0/handlers/note/component/editor/markdown.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/markdown_edit.html` & `xnote-web-0.1.0/handlers/note/component/editor/markdown_edit.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/markdown_edit.mobile.html` & `xnote-web-0.1.0/handlers/note/component/editor/markdown_edit.mobile.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/post.html` & `xnote-web-0.1.0/handlers/note/component/editor/post.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/table_lang.html` & `xnote-web-0.1.0/handlers/note/component/editor/table_lang.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/editor/table_myexcel.html` & `xnote-web-0.1.0/handlers/note/component/editor/table_myexcel.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/filter/group_tag_filter.html` & `xnote-web-0.1.0/handlers/note/component/filter/group_tag_filter.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/filter/note_tag_filter.html` & `xnote-web-0.1.0/handlers/note/component/filter/note_tag_filter.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/filter/type_filter.html` & `xnote-web-0.1.0/handlers/note/component/filter/type_filter.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/group_select.html` & `xnote-web-0.1.0/handlers/note/component/group_select.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/group_select_tree.html` & `xnote-web-0.1.0/handlers/note/component/group_select_tree.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/header/common_header.html` & `xnote-web-0.1.0/handlers/note/component/header/common_header.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/header/group_detail_header.html` & `xnote-web-0.1.0/handlers/note/component/header/group_detail_header.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/mobile/group_category_switch.html` & `xnote-web-0.1.0/handlers/note/component/mobile/group_category_switch.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/mod_aside.html` & `xnote-web-0.1.0/handlers/note/component/mod_aside.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/note_list_component.html` & `xnote-web-0.1.0/handlers/note/component/note_list_component.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/note_orderby_select.html` & `xnote-web-0.1.0/handlers/note/component/note_orderby_select.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/note_path.html` & `xnote-web-0.1.0/handlers/note/component/note_path.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/option/create_option.html` & `xnote-web-0.1.0/handlers/note/component/option/create_option.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/option/group_option.html` & `xnote-web-0.1.0/handlers/note/component/option/group_option.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/option/group_option_dropdown.html` & `xnote-web-0.1.0/handlers/note/component/option/group_option_dropdown.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/option/note_dropdown.html` & `xnote-web-0.1.0/handlers/note/component/option/note_dropdown.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/root_dropdown.html` & `xnote-web-0.1.0/handlers/note/component/root_dropdown.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/create_script.html` & `xnote-web-0.1.0/handlers/note/component/script/create_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/delete_script.html` & `xnote-web-0.1.0/handlers/note/component/script/delete_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/group_select_script.html` & `xnote-web-0.1.0/handlers/note/component/script/group_select_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/note_copy_script.html` & `xnote-web-0.1.0/handlers/note/component/script/note_copy_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/note_option_script.html` & `xnote-web-0.1.0/handlers/note/component/script/note_option_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/rename_script.html` & `xnote-web-0.1.0/handlers/note/component/script/rename_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/share_script.html` & `xnote-web-0.1.0/handlers/note/component/script/share_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/status_script.html` & `xnote-web-0.1.0/handlers/note/component/script/status_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/tag_manage_script.html` & `xnote-web-0.1.0/handlers/note/component/script/tag_manage_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/script/tag_script.html` & `xnote-web-0.1.0/handlers/note/component/script/tag_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/share_dialog.html` & `xnote-web-0.1.0/handlers/note/component/share_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/sidebar/group_list_sidebar.html` & `xnote-web-0.1.0/handlers/note/component/sidebar/group_list_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/sidebar/group_manage_sidebar.html` & `xnote-web-0.1.0/handlers/note/component/sidebar/group_manage_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/sidebar/group_sidebar.html` & `xnote-web-0.1.0/handlers/note/component/sidebar/group_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/sidebar/markdown_edit_sidebar.html` & `xnote-web-0.1.0/handlers/note/component/sidebar/markdown_edit_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/sidebar/note_sidebar.html` & `xnote-web-0.1.0/handlers/note/component/sidebar/note_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/sort/note_sort_tab.html` & `xnote-web-0.1.0/handlers/note/component/sort/note_sort_tab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/timeline/timeline_body.html` & `xnote-web-0.1.0/handlers/note/component/timeline/timeline_body.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/timeline/timeline_create_option.html` & `xnote-web-0.1.0/handlers/note/component/timeline/timeline_create_option.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/view_css.html` & `xnote-web-0.1.0/handlers/note/component/view_css.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/view_footer.html` & `xnote-web-0.1.0/handlers/note/component/view_footer.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/view_header.html` & `xnote-web-0.1.0/handlers/note/component/view_header.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/component/view_header_tag.html` & `xnote-web-0.1.0/handlers/note/component/view_header_tag.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/constant.py` & `xnote-web-0.1.0/handlers/note/constant.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao.py` & `xnote-web-0.1.0/handlers/note/dao.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_api.py` & `xnote-web-0.1.0/handlers/note/dao_api.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_book.py` & `xnote-web-0.1.0/handlers/note/dao_book.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_category.py` & `xnote-web-0.1.0/handlers/note/dao_category.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_comment.py` & `xnote-web-0.1.0/handlers/note/dao_comment.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_delete.py` & `xnote-web-0.1.0/handlers/note/dao_delete.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_draft.py` & `xnote-web-0.1.0/handlers/note/dao_draft.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_edit.py` & `xnote-web-0.1.0/handlers/note/dao_edit.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_log.py` & `xnote-web-0.1.0/handlers/note/dao_log.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_read.py` & `xnote-web-0.1.0/handlers/note/dao_read.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_share.py` & `xnote-web-0.1.0/handlers/note/dao_share.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/dao_tag.py` & `xnote-web-0.1.0/handlers/note/dao_tag.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/html_importer.py` & `xnote-web-0.1.0/handlers/note/html_importer.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_api.py` & `xnote-web-0.1.0/handlers/note/note_api.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_category.py` & `xnote-web-0.1.0/handlers/note/note_category.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_checklist.py` & `xnote-web-0.1.0/handlers/note/note_checklist.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_edit.py` & `xnote-web-0.1.0/handlers/note/note_edit.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_group.py` & `xnote-web-0.1.0/handlers/note/note_group.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_helper.py` & `xnote-web-0.1.0/handlers/note/note_helper.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_stat.py` & `xnote-web-0.1.0/handlers/note/note_stat.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_tag.py` & `xnote-web-0.1.0/handlers/note/note_tag.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_timeline.py` & `xnote-web-0.1.0/handlers/note/note_timeline.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_view.py` & `xnote-web-0.1.0/handlers/note/note_view.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/note_workspace.py` & `xnote-web-0.1.0/handlers/note/note_workspace.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/batch/gallery_manage.html` & `xnote-web-0.1.0/handlers/note/page/batch/gallery_manage.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base %}
 
-{% block body %}
+{% block body_left %}
     <div class="card">
         <h3 class="card-title btn-line-height">
             <a href="{{note.url}}" class="link2">{{note.name}}</a> / 管理
             {% include common/back.html %}
         </h3>
     </div>
 
@@ -13,7 +13,11 @@
 
     <script type="text/javascript" src="/static/js/fs/fs.js"></script>
 
     <div class="card">    
         {% include fs/component/filelist_simple.html %}
     </div>
 {% end %}
+
+{% block body_right %}
+    {% include common/sidebar/default.html %}
+{% end %}
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
-{% extends base %} {% block body %}
+{% extends base %} {% block body_left %}
 ******** _{{_{{_nn_oo_tt_ee_.._nn_aa_mm_ee_}}_}} // ?ç?®?¡?ç?? {{%% iinncclluuddee ccoommmmoonn//bbaacckk..hhttmmll %%}} ********
 {% include fs/component/filelist_simple.html %}
-{% end %}
+{% end %} {% block body_right %} {% include common/sidebar/default.html %} {%
+end %}
```

### Comparing `xnote-web-0.0.9/handlers/note/page/batch/group_manage.html` & `xnote-web-0.1.0/handlers/note/page/batch/group_manage.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/batch/group_manage_category.html` & `xnote-web-0.1.0/handlers/note/page/batch/group_manage_category.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/batch/note_manage.html` & `xnote-web-0.1.0/handlers/note/page/batch/note_manage.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/category.html` & `xnote-web-0.1.0/handlers/note/page/category.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/comment.html` & `xnote-web-0.1.0/handlers/note/page/comment.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/create.html` & `xnote-web-0.1.0/handlers/note/page/create.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/detail/checklist_detail.html` & `xnote-web-0.1.0/handlers/note/page/detail/checklist_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/detail/form_detail.html` & `xnote-web-0.1.0/handlers/note/page/detail/form_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/detail/group_detail.html` & `xnote-web-0.1.0/handlers/note/page/detail/group_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/detail/group_detail_body.html` & `xnote-web-0.1.0/handlers/note/page/detail/group_detail_body.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/detail/note_detail.html` & `xnote-web-0.1.0/handlers/note/page/detail/note_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/detail/table_detail.html` & `xnote-web-0.1.0/handlers/note/page/detail/table_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/group_list.html` & `xnote-web-0.1.0/handlers/note/page/group_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/group_list_nav_desktop.html` & `xnote-web-0.1.0/handlers/note/page/group_list_nav_desktop.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/group_list_nav_mobile.html` & `xnote-web-0.1.0/handlers/note/page/group_list_nav_mobile.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/history_list.html` & `xnote-web-0.1.0/handlers/note/page/history_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/html_importer.html` & `xnote-web-0.1.0/handlers/note/page/html_importer.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/index/note_index.html` & `xnote-web-0.1.0/handlers/note/page/index/note_index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/index/note_workspace.html` & `xnote-web-0.1.0/handlers/note/page/index/note_workspace.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/index/note_workspace.mobile.html` & `xnote-web-0.1.0/handlers/note/page/index/note_workspace.mobile.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/index/note_workspace2.html` & `xnote-web-0.1.0/handlers/note/page/index/note_workspace2.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/list_by_date.html` & `xnote-web-0.1.0/handlers/note/page/list_by_date.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/note_calendar.html` & `xnote-web-0.1.0/handlers/note/page/note_calendar.html`

 * *Files 0% similar despite different names*

```diff
@@ -509,8 +509,12 @@
     showCalendarData();
   });
 
 })();
 
 </script>
 
-{% end %}
+{% end %}
+
+{% block body_right %}
+  {% include common/sidebar/default.html %}
+{% end %}
```

### Comparing `xnote-web-0.0.9/handlers/note/page/note_default.html` & `xnote-web-0.1.0/handlers/note/page/note_default.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/note_list.html` & `xnote-web-0.1.0/handlers/note/page/note_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/note_recent.html` & `xnote-web-0.1.0/handlers/note/page/note_recent.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/note_share.html` & `xnote-web-0.1.0/handlers/note/page/note_share.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/note_tools.html` & `xnote-web-0.1.0/handlers/note/page/note_tools.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/old/category_old.html` & `xnote-web-0.1.0/handlers/note/page/old/category_old.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/old/create_log.html` & `xnote-web-0.1.0/handlers/note/page/old/create_log.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/old/group_list_archived.html` & `xnote-web-0.1.0/handlers/note/page/old/group_list_archived.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/old/list_by_date_old.html` & `xnote-web-0.1.0/handlers/note/page/old/list_by_date_old.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/old/project_list_old.html` & `xnote-web-0.1.0/handlers/note/page/old/project_list_old.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/old/upload_file.html` & `xnote-web-0.1.0/handlers/note/page/old/upload_file.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/print.html` & `xnote-web-0.1.0/handlers/note/page/print.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/taglist.html` & `xnote-web-0.1.0/handlers/note/page/taglist.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/tagname.html` & `xnote-web-0.1.0/handlers/note/page/tagname.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/note/page/timeline/timeline.html` & `xnote-web-0.1.0/handlers/note/page/timeline/timeline.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plan/dao.py` & `xnote-web-0.1.0/handlers/plan/dao.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plan/page/month_plan.html` & `xnote-web-0.1.0/handlers/plan/page/month_plan.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plan/plan.py` & `xnote-web-0.1.0/handlers/plan/plan.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/base/base_form_plugin.html` & `xnote-web-0.1.0/handlers/plugin/base/base_form_plugin.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/base/base_plugin.html` & `xnote-web-0.1.0/handlers/plugin/base/base_plugin.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/base/base_plugin_title.html` & `xnote-web-0.1.0/handlers/plugin/base/base_plugin_title.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/dao.py` & `xnote-web-0.1.0/handlers/plugin/dao.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/header/plugin_category.html` & `xnote-web-0.1.0/handlers/plugin/header/plugin_category.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/header/plugin_header_normal.html` & `xnote-web-0.1.0/handlers/plugin/header/plugin_header_normal.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/page/grid.html` & `xnote-web-0.1.0/handlers/plugin/page/grid.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/page/plugins_v1.html` & `xnote-web-0.1.0/handlers/plugin/page/plugins_v1.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/page/plugins_v2.html` & `xnote-web-0.1.0/handlers/plugin/page/plugins_v2.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/page/plugins_v3.html` & `xnote-web-0.1.0/handlers/plugin/page/plugins_v3.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/plugin_create.py` & `xnote-web-0.1.0/handlers/plugin/plugin_create.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/plugin_page.py` & `xnote-web-0.1.0/handlers/plugin/plugin_page.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/plugin/plugin_upload.py` & `xnote-web-0.1.0/handlers/plugin/plugin_upload.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/ajax/search_dialog.html` & `xnote-web-0.1.0/handlers/search/ajax/search_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/ajax/search_dialog_detail.html` & `xnote-web-0.1.0/handlers/search/ajax/search_dialog_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/api.py` & `xnote-web-0.1.0/handlers/search/api.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/calc.py` & `xnote-web-0.1.0/handlers/search/calc.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/component/search_pagination.html` & `xnote-web-0.1.0/handlers/search/component/search_pagination.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/component/search_sidebar.html` & `xnote-web-0.1.0/handlers/search/component/search_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/component/search_tab.html` & `xnote-web-0.1.0/handlers/search/component/search_tab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/dictionary.py` & `xnote-web-0.1.0/handlers/search/dictionary.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/mute.py` & `xnote-web-0.1.0/handlers/search/mute.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/note.py` & `xnote-web-0.1.0/handlers/search/note.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/page/search_history.html` & `xnote-web-0.1.0/handlers/search/page/search_history.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/page/search_result.html` & `xnote-web-0.1.0/handlers/search/page/search_result.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/pydoc.py` & `xnote-web-0.1.0/handlers/search/pydoc.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/reminder.py` & `xnote-web-0.1.0/handlers/search/reminder.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/scripts.py` & `xnote-web-0.1.0/handlers/search/scripts.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/search.html` & `xnote-web-0.1.0/handlers/search/search.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/search.py` & `xnote-web-0.1.0/handlers/search/search.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/search_rules.html` & `xnote-web-0.1.0/handlers/search/search_rules.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/search/tools.py` & `xnote-web-0.1.0/handlers/search/tools.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/component/admin_settings.html` & `xnote-web-0.1.0/handlers/settings/component/admin_settings.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/component/note_settings.html` & `xnote-web-0.1.0/handlers/settings/component/note_settings.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/component/search_settings.html` & `xnote-web-0.1.0/handlers/settings/component/search_settings.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/component/settings_sidebar.html` & `xnote-web-0.1.0/handlers/settings/component/settings_sidebar.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/page/properties.html` & `xnote-web-0.1.0/handlers/settings/page/properties.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/page/settings.html` & `xnote-web-0.1.0/handlers/settings/page/settings.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/settings/settings.py` & `xnote-web-0.1.0/handlers/settings/settings.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/backup.py` & `xnote-web-0.1.0/handlers/system/backup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 import xutils
 from xnote.core import xconfig, xauth, xtemplate
 import web.db
 
 from xutils import Storage
 from xutils import dbutil
 from xutils import fsutil, logutil
+from xutils import dateutil
 from xutils.db.driver_sqlite import SqliteKV
 from xnote.core import xtables
-from xnote.service import JobService, SysJob, JobStatusEnum
+from xnote.service import JobService, SysJob, JobStatusEnum, DatabaseLockService
 
 config = xconfig
 
 _black_list = [".zip", ".pyc", ".pdf", "__pycache__", ".git"]
 _dirname = "./"
 _zipname = "xnote.zip"
 _dest_path = os.path.join(_dirname, "static", _zipname)
 
 # 删除备份在 cron/diskclean 任务里面
-# 备份的锁
-_backup_lock = threading.RLock()
 _import_logger = logutil.new_mem_logger("import_db", size = 20)
 
 def zip_xnote(nameblacklist = [_zipname]):
     dirname = "./"
     fp = open(_dest_path, "w")
     fp.close()
     zf = zipfile.ZipFile(_dest_path, "w")
@@ -69,14 +68,16 @@
 
 class DBBackup:
     """数据库备份"""
 
     _progress = 0.0
     _start_time = -1
     _total = 0
+    lock_key = "backup_job"
+    expire_seconds = 3600
 
     def __init__(self):
         self.db_backup_file = os.path.join(xconfig.TMP_DIR, "temp.db")
 
     @staticmethod
     def progress():
         return "%.2f%%" % (DBBackup._progress * 100.0)
@@ -216,25 +217,21 @@
             DBBackup._count = -1
             DBBackup._progress = 0.0
         return count
 
 
     def execute(self, backup_kv=True):
         logger = self.get_backup_logger()
-        got_lock = False
         try:
-            if _backup_lock.acquire(blocking = False):
-                got_lock = True
+            with DatabaseLockService.lock(self.lock_key, self.expire_seconds):
                 self.do_execute(backup_kv=backup_kv)
-            else:
-                logger.log("backup is busy")
-                return "backup is busy"
-        finally:
-            if got_lock:
-                _backup_lock.release()
+            return "backup success"
+        except:
+            logger.log("backup is busy")
+            return "backup is busy"
 
     def do_execute(self, backup_kv=True):
         
         job_info = SysJob()
         job_info.job_type = "db_backup"
         
         with JobService.run_with_job(job_info):
@@ -260,14 +257,15 @@
             fsutil.mvfile(self.db_backup_file, destfile)
 
             # 再次清理
             self.clean()
             
             job_info.job_status = JobStatusEnum.success
             job_info.job_result = "备份任务完成"
+            job_info.mtime = dateutil.format_datetime()
 
             return dict(count = count, cost_time = "%sms" % cost_time)
 
 def chk_db_backup():
     if not xconfig.get_system_config("db_backup"):
         return
     backup = DBBackup()
@@ -295,42 +293,42 @@
     if cost_time > 0:
         return count/cost_time
     return -1
 
 
 class DBImporter:
 
+    lock_key = "db_import"
+    expire_seconds = 3600
+
     def import_db(self, db_file):
         self.db_backup_file = db_file
-        got_lock = False
         try:
-            if _backup_lock.acquire(blocking = False):
-                got_lock = True
+            with DatabaseLockService.lock(self.lock_key, self.expire_seconds):
                 self.import_sql(db_file)
                 return self.import_kv(db_file)
-            else:
-                logging.warning("import_db is busy")
-                return "import_db is busy"
         except:
             exc_info = xutils.print_exc()
             _import_logger.info(exc_info)
-        finally:
-            if got_lock:
-                _backup_lock.release()
-
+            logging.warning("import_db is busy")
+            return "import_db is busy"
+    
     def get_logger(self):
         return _import_logger
 
     def import_sql(self, db_file):
         logger = self.get_logger()
         backup_db = xtables.MySqliteDB(db = db_file)
         batch_size = 100
 
         try:
             for table in xtables.get_all_tables():
+                if table.table_name == xconfig.DatabaseConfig.kv_store:
+                    logger.info(f"skip kv_store table: {table.table_name}")
+                    continue
                 backup_table = xtables.init_backup_table(table.tablename, backup_db)
                 total_count = backup_table.count()
                 logger.info("import table:(%s) count:(%d)", table.tablename, total_count)
                 start_time = time.time()
                 count = 0
                 assert isinstance(table, xtables.TableProxy)
                 for records in backup_table.iter_batch(batch_size=batch_size):
@@ -424,16 +422,15 @@
 
         if p == "import_db":
             path = xutils.get_argument("path", "")
             return import_db(path)
 
         if p == "backup_sql":
             backup = DBBackup()
-            backup.execute(backup_kv=False)
-            return "backup_sql"
+            return backup.execute(backup_kv=False)
 
         # 备份所有的
         chk_db_backup()
         chk_scripts_backup()
         return "OK"
     
 # chk_backup()
```

### Comparing `xnote-web-0.0.9/handlers/system/cache_admin.py` & `xnote-web-0.1.0/handlers/system/cache_admin.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/clipboard.py` & `xnote-web-0.1.0/handlers/system/clipboard.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/command.py` & `xnote-web-0.1.0/handlers/system/command.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/admin_nav.html` & `xnote-web-0.1.0/handlers/system/component/admin_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/db_kv_nav.html` & `xnote-web-0.1.0/handlers/system/component/db_kv_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/db_nav.html` & `xnote-web-0.1.0/handlers/system/component/db_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/system_log_tab.html` & `xnote-web-0.1.0/handlers/system/component/system_log_tab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/system_sync_cluster_info.html` & `xnote-web-0.1.0/handlers/system/component/system_sync_cluster_info.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/system_sync_follower_view.html` & `xnote-web-0.1.0/handlers/system/component/system_sync_follower_view.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/component/thread_nav.html` & `xnote-web-0.1.0/handlers/system/component/thread_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/db_admin.py` & `xnote-web-0.1.0/handlers/system/db_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         next_cursor = ""
         keywords = textutil.split_words(keyword)
 
         for key, value in dbutil.prefix_iter(
                 prefix, key_from=key_from, key_to=key_to, include_key=True, limit=limit+1,
                 parse_json=False, reverse=reverse, scan_db=True):
             if scanned < limit and (textutil.contains_all(key, keywords) or textutil.contains_all(value, keywords)):
-                item = Storage(key=key, key_encoded=xutils.quote(key), value=value)
+                item = Storage(key=key, key_encoded=xutils.quote(key), value=value, data_key=xutils.html_escape(key))
                 result.append(item)
             scanned += 1
             next_cursor = key
 
         has_next = False
         if scanned > limit:
             scanned = limit
```

### Comparing `xnote-web-0.0.9/handlers/system/db_index.py` & `xnote-web-0.1.0/handlers/system/db_index.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/db_migrate_tools.py` & `xnote-web-0.1.0/handlers/system/db_migrate_tools.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/db_refresh.py` & `xnote-web-0.1.0/handlers/system/db_refresh.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/db_shell.py` & `xnote-web-0.1.0/handlers/system/db_shell.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/db_upgrade.py` & `xnote-web-0.1.0/handlers/system/db_upgrade.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/develop_controller.py` & `xnote-web-0.1.0/handlers/system/develop_controller.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/mod_aside.html` & `xnote-web-0.1.0/handlers/system/mod_aside.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/network_profile.py` & `xnote-web-0.1.0/handlers/system/network_profile.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/cache_admin.html` & `xnote-web-0.1.0/handlers/system/page/cache_admin.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/crontab.html` & `xnote-web-0.1.0/handlers/system/page/crontab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/crontab_edit.html` & `xnote-web-0.1.0/handlers/system/page/crontab_edit.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/db_admin.html` & `xnote-web-0.1.0/handlers/system/page/db/db_admin.html`

 * *Files 3% similar despite different names*

```diff
@@ -83,38 +83,39 @@
                 <td style="width:20%">{{!item.key}}</td>
                 <td style="width:60%">{{!item.valueShort}}</td>
                 <td style="width:20%">
                     <div class="float-right">
                         <button class="btn btn-default view-btn" 
                             data-url="/system/sqldb_detail?method=get_kv_detail&key={{!item.key_encoded}}" 
                             onclick="xnote.admin.viewMainRecord(this)">查看</button>
-                        <button class="btn btn-danger delete-btn" data-key="{{!item.key_encoded}}">删除</button>
+                        <button class="btn btn-danger delete-btn" data-key="{{!item.data_key}}" 
+                            onclick="xnote.admin.deleteRecord(this)">删除</button>
                     </div>
                 </td>
             </tr>
         {{!/each }}
     </table>
 </div>
 </script>
 
 <script>
 $(function () {
     var globalVersion = 0;
 
-    $("body").on("click", ".delete-btn", function (e) {
-        var key = $(this).attr("data-key");
+    xnote.admin.deleteRecord = function (target) {
+        var key = $(target).attr("data-key");
         xnote.confirm("准备删除【" + key + "】，请确认", function (confirmed) {
             var params = {key: key};
             xnote.http.post("?action=delete", params, function (resp) {
                 search();
             }).fail(function () {
                 xnote.toast("删除失败，请稍后重试~");
             })
         });
-    }); 
+    }
 
     $(".do-search-btn").click(function (e) {
         search();    
     });
 
     // 搜索接口
     function search() {
```

### Comparing `xnote-web-0.0.9/handlers/system/page/db/db_backup.html` & `xnote-web-0.1.0/handlers/system/page/db/db_backup.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/db_index.html` & `xnote-web-0.1.0/handlers/system/page/db/db_index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/db_index_v2.html` & `xnote-web-0.1.0/handlers/system/page/db/db_index_v2.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/db_meta.html` & `xnote-web-0.1.0/handlers/system/page/db/db_meta.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/db_struct.html` & `xnote-web-0.1.0/handlers/system/page/db/db_struct.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/driver_info.html` & `xnote-web-0.1.0/handlers/system/page/db/driver_info.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/sqldb_detail.html` & `xnote-web-0.1.0/handlers/system/page/db/sqldb_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/db/sqldb_list.html` & `xnote-web-0.1.0/handlers/system/page/db/sqldb_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/develop/index.html` & `xnote-web-0.1.0/handlers/system/page/develop/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     </h3>
 </div>
 
 {% set data_list = [
     Storage(name = "浏览器信息", url = "/tools/browser_info"),
     Storage(name = "系统模块", url = "/system/module_list"),
     Storage(name = "前端组件", url = "/test/example"),
+    Storage(name = "性能分析", url = "/system/handler_profile"),
 ] %}
 
 <div class="card list">
 
     {% for item in data_list %}
         <a class="list-link" href="{{_server_home}}{{item.url}}">
             <span>{{item.name}}</span>
```

### Comparing `xnote-web-0.0.9/handlers/system/page/history.html` & `xnote-web-0.1.0/handlers/system/page/history.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/module_detail.html` & `xnote-web-0.1.0/handlers/system/page/module_detail.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/module_list.html` & `xnote-web-0.1.0/handlers/system/page/module_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/script.html` & `xnote-web-0.1.0/handlers/system/page/script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/sqlite.html` & `xnote-web-0.1.0/handlers/system/page/sqlite.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/system_admin.html` & `xnote-web-0.1.0/handlers/system/page/system_admin.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/system_index.html` & `xnote-web-0.1.0/handlers/system/page/system_index.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/system_info.html` & `xnote-web-0.1.0/handlers/system/page/system_info.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/system_info_text.html` & `xnote-web-0.1.0/handlers/system/page/system_info_text.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/system_sync.html` & `xnote-web-0.1.0/handlers/system/page/system_sync.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/template_cache.html` & `xnote-web-0.1.0/handlers/system/page/template_cache.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/page/thread_info.html` & `xnote-web-0.1.0/handlers/system/page/thread_info.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/script.py` & `xnote-web-0.1.0/handlers/system/script.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/stats.py` & `xnote-web-0.1.0/handlers/system/stats.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system.py` & `xnote-web-0.1.0/handlers/system/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,22 +94,23 @@
 SYS_TOOLS = [
     user_link("设置",   "/system/settings", "cog"),
     guest_link("登录", "/login", "sign-in"),
 
     admin_link("系统信息",   "/system/info", "info-circle"),
     admin_link("文件",       "/fs_list", "file-text-o"),
     admin_link("定时任务",   "/system/crontab", "clock-o"),
-    admin_link("任务列表", "/admin/jobs"),
+    admin_link("任务实例", "/admin/jobs"),
     admin_link("事件注册", "/system/event"),
     admin_link("线程管理", "/system/thread_info"),
     admin_link("Menu_User",   "/system/user/list", "users"),
     admin_link("Menu_Log",    "/system/log"),
     admin_link("Menu_Modules",  "/system/modules_info"),
     admin_link("Shell",    "/tools/shell", "terminal"),
     admin_link("集群管理", "/system/sync?p=home", "server"),
+    admin_link("开发者", "/system/develop"),
 
     user_link("Menu_Plugin",   "/plugin_category_list?category=index&show_back=true", "cogs"),
     # 关于链接，支持外链
     about_link(),
 ]
 
 NOTE_TOOLS = [
```

### Comparing `xnote-web-0.0.9/handlers/system/system_boot.py` & `xnote-web-0.1.0/handlers/system/system_boot.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_event.py` & `xnote-web-0.1.0/handlers/system/system_event.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_info.py` & `xnote-web-0.1.0/handlers/system/system_info.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_log.py` & `xnote-web-0.1.0/handlers/system/system_log.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_module.py` & `xnote-web-0.1.0/handlers/system/system_module.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/models.py` & `xnote-web-0.1.0/handlers/system/system_sync/models.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/node_base.py` & `xnote-web-0.1.0/handlers/system/system_sync/node_base.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/node_follower.py` & `xnote-web-0.1.0/handlers/system/system_sync/node_follower.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/node_leader.py` & `xnote-web-0.1.0/handlers/system/system_sync/node_leader.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/system_sync_controller.py` & `xnote-web-0.1.0/handlers/system/system_sync/system_sync_controller.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/system_sync_indexer.py` & `xnote-web-0.1.0/handlers/system/system_sync/system_sync_indexer.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/system_sync/system_sync_proxy.py` & `xnote-web-0.1.0/handlers/system/system_sync/system_sync_proxy.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/template_cache.py` & `xnote-web-0.1.0/handlers/system/template_cache.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/system/thread_info.py` & `xnote-web-0.1.0/handlers/system/thread_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # encoding=utf-8
 """
 展示系统使用的线程信息
 """
-import xauth
+from xnote.core import xauth, xtemplate, xmanager
 import threading
-import xtemplate
 import xutils
-import xmanager
 from xutils import MyStdout
 
 def get_thread_log(thread):
     records = MyStdout.get_records(thread)
     if records is None:
         return "[无]"
     return xutils.mark_text("".join(records))
```

### Comparing `xnote-web-0.0.9/handlers/test/component/example_nav.html` & `xnote-web-0.1.0/handlers/test/component/example_nav.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/page/example_btn.html` & `xnote-web-0.1.0/handlers/test/page/example_btn.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/page/example_dialog.html` & `xnote-web-0.1.0/handlers/test/page/example_dialog.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/page/example_dropdown.html` & `xnote-web-0.1.0/handlers/test/page/example_dropdown.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/page/example_hammer.html` & `xnote-web-0.1.0/handlers/test/page/example_hammer.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/page/example_tab.html` & `xnote-web-0.1.0/handlers/test/page/example_tab.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/page/example_tag.html` & `xnote-web-0.1.0/handlers/test/page/example_tag.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/test/test_dbutil_handler.py` & `xnote-web-0.1.0/handlers/test/test_dbutil_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 # @author xupingmao
 # @since 2021/12/18 17:37:52
 # @modified 2022/03/20 23:28:21
 # @filename test_dbutil_handler.py
 
-import xauth
+from xnote.core import xauth
 import xutils
 import random
 from xutils import Storage
 from xutils import dbutil
 
 dbutil.register_table("test", "测试数据库")
 dbutil.register_table_index("test", "age")
```

### Comparing `xnote-web-0.0.9/handlers/test/test_handler.py` & `xnote-web-0.1.0/handlers/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/barcode.html` & `xnote-web-0.1.0/handlers/tools/barcode.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/base64.html` & `xnote-web-0.1.0/handlers/tools/base64.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/browser_info.html` & `xnote-web-0.1.0/handlers/tools/browser_info.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/camera.html` & `xnote-web-0.1.0/handlers/tools/camera.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/chat_demo.html` & `xnote-web-0.1.0/handlers/tools/chat_demo.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/code_template.html` & `xnote-web-0.1.0/handlers/tools/code_template.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/color.html` & `xnote-web-0.1.0/handlers/tools/color.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/datetime.html` & `xnote-web-0.1.0/handlers/tools/datetime.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/hex.html` & `xnote-web-0.1.0/handlers/tools/hex.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/img2gray.html` & `xnote-web-0.1.0/handlers/tools/img2gray.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/img_merge.html` & `xnote-web-0.1.0/handlers/tools/img_merge.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/img_split.html` & `xnote-web-0.1.0/handlers/tools/img_split.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/md5.html` & `xnote-web-0.1.0/handlers/tools/md5.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/multi_win.html` & `xnote-web-0.1.0/handlers/tools/multi_win.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/notebook.html` & `xnote-web-0.1.0/handlers/tools/notebook.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/port_scanner.py` & `xnote-web-0.1.0/handlers/tools/port_scanner.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/qrcode.html` & `xnote-web-0.1.0/handlers/tools/qrcode.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/random_string.html` & `xnote-web-0.1.0/handlers/tools/random_string.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/responsive.html` & `xnote-web-0.1.0/handlers/tools/responsive.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/runjs.html` & `xnote-web-0.1.0/handlers/tools/runjs.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/search_compare.html` & `xnote-web-0.1.0/handlers/tools/search_compare.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/sha1.html` & `xnote-web-0.1.0/handlers/tools/sha1.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/shell.html` & `xnote-web-0.1.0/handlers/tools/shell.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/speech_recognition.html` & `xnote-web-0.1.0/handlers/tools/speech_recognition.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/tcc.html` & `xnote-web-0.1.0/handlers/tools/tcc.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/terminal.html` & `xnote-web-0.1.0/handlers/tools/terminal.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/text_convert.html` & `xnote-web-0.1.0/handlers/tools/text_convert.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/text_diff.html` & `xnote-web-0.1.0/handlers/tools/text_diff.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/text_set.html` & `xnote-web-0.1.0/handlers/tools/text_set.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/tools.py` & `xnote-web-0.1.0/handlers/tools/tools.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/urlcoder.html` & `xnote-web-0.1.0/handlers/tools/urlcoder.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/vue_test.html` & `xnote-web-0.1.0/handlers/tools/vue_test.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/tools/webuploader.html` & `xnote-web-0.1.0/handlers/tools/webuploader.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/component/user_script.html` & `xnote-web-0.1.0/handlers/user/component/user_script.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/login.py` & `xnote-web-0.1.0/handlers/user/login.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/change_password.html` & `xnote-web-0.1.0/handlers/user/page/change_password.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/login.html` & `xnote-web-0.1.0/handlers/user/page/login.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/user.html` & `xnote-web-0.1.0/handlers/user/page/user.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/user_list.html` & `xnote-web-0.1.0/handlers/user/page/user_list.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/user_manage.html` & `xnote-web-0.1.0/handlers/user/page/user_manage.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/user_op_log.html` & `xnote-web-0.1.0/handlers/user/page/user_op_log.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/page/userinfo.html` & `xnote-web-0.1.0/handlers/user/page/userinfo.html`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/user/user.py` & `xnote-web-0.1.0/handlers/user/user.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/handlers/webdav/webdav.py` & `xnote-web-0.1.0/handlers/webdav/webdav.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/html2text.py` & `xnote-web-0.1.0/lib/html2text.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/leveldb-x64.dll` & `xnote-web-0.1.0/lib/leveldb-x64.dll`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/leveldb.dll` & `xnote-web-0.1.0/lib/leveldb.dll`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/leveldbpy.py` & `xnote-web-0.1.0/lib/leveldbpy.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/smallseg.py` & `xnote-web-0.1.0/lib/smallseg.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/__init__.py` & `xnote-web-0.1.0/lib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/application.py` & `xnote-web-0.1.0/lib/web/application.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/browser.py` & `xnote-web-0.1.0/lib/web/browser.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/contrib/template.py` & `xnote-web-0.1.0/lib/web/contrib/template.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/db.py` & `xnote-web-0.1.0/lib/web/db.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/debugerror.py` & `xnote-web-0.1.0/lib/web/debugerror.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/form.py` & `xnote-web-0.1.0/lib/web/form.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/http.py` & `xnote-web-0.1.0/lib/web/http.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/httpserver.py` & `xnote-web-0.1.0/lib/web/httpserver.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/net.py` & `xnote-web-0.1.0/lib/web/net.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/py3helpers.py` & `xnote-web-0.1.0/lib/web/py3helpers.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/session.py` & `xnote-web-0.1.0/lib/web/session.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/template.py` & `xnote-web-0.1.0/lib/web/template.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/test.py` & `xnote-web-0.1.0/lib/web/test.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/utils.py` & `xnote-web-0.1.0/lib/web/utils.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/webapi.py` & `xnote-web-0.1.0/lib/web/webapi.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/webopenid.py` & `xnote-web-0.1.0/lib/web/webopenid.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgi.py` & `xnote-web-0.1.0/lib/web/wsgi.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgiserver/LICENSE.txt` & `xnote-web-0.1.0/lib/web/wsgiserver/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgiserver/__init__.py` & `xnote-web-0.1.0/lib/web/wsgiserver/__init__.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgiserver/ssl_builtin.py` & `xnote-web-0.1.0/lib/web/wsgiserver/ssl_builtin.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgiserver/ssl_pyopenssl.py` & `xnote-web-0.1.0/lib/web/wsgiserver/ssl_pyopenssl.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgiserver/wsgiserver2.py` & `xnote-web-0.1.0/lib/web/wsgiserver/wsgiserver2.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/web/wsgiserver/wsgiserver3.py` & `xnote-web-0.1.0/lib/web/wsgiserver/wsgiserver3.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/lib/wget.py` & `xnote-web-0.1.0/lib/wget.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/setup.py` & `xnote-web-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fp.read()
 
 
 data_ext_list =  ["*.txt", "*.json", "*.properties", "*.js", "*.html", "*.css"]
 
 setuptools.setup(
     name = "xnote-web",
-    version = "0.0.9",
+    version = "0.1.0",
     author = "mark",
     author_email = "578749341@qq.com",
     description = "xnote-web框架",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     # packages = ["config", "core", "docs", "handlers", "lib", "static", "tools", "xnote", "xutils"],
     packages=setuptools.find_packages(),
```

### Comparing `xnote-web-0.0.9/static/audio/todo_done.mp3` & `xnote-web-0.1.0/static/audio/todo_done.mp3`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/app.build.css` & `xnote-web-0.1.0/static/css/app.build.css`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     font-size: 14px;
 }
 
 textarea:focus, input:focus {
     border: 1px solid #8cc;
 }
 
+textarea:read-only, input[type=text]:read-only {
+    background-color: #eee;
+}
+
 select {
     padding: 5px;
     border: 1px solid #ccc;
 }
 
 /** 链接样式 **/
 a {
@@ -1831,14 +1835,19 @@
 .toolbar.homepage>.action:hover {
     opacity: 1.0;
 }
 
 .btn.large {
     width: 100px;
     height: 30px;
+}
+
+.btn.huge {
+    width: 100%;
+    height: 30px;
 }/**
  * markdown的样式扩展
  * @author xupingmao
  * @since 2021/08/01 14:25:17
  * @modified 2022/03/27 16:53:38
  * @filename common-markdown.css
  */
```

### Comparing `xnote-web-0.0.9/static/css/app.css` & `xnote-web-0.1.0/static/css/app.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-button.css` & `xnote-web-0.1.0/static/css/base/common-button.css`

 * *Files 11% similar despite different names*

```diff
@@ -160,8 +160,13 @@
 .toolbar.homepage>.action:hover {
     opacity: 1.0;
 }
 
 .btn.large {
     width: 100px;
     height: 30px;
+}
+
+.btn.huge {
+    width: 100%;
+    height: 30px;
 }
```

### Comparing `xnote-web-0.0.9/static/css/base/common-dropdown.css` & `xnote-web-0.1.0/static/css/base/common-dropdown.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-icon.css` & `xnote-web-0.1.0/static/css/base/common-icon.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-layout.css` & `xnote-web-0.1.0/static/css/base/common-layout.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-markdown.css` & `xnote-web-0.1.0/static/css/base/common-markdown.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-mobile.css` & `xnote-web-0.1.0/static/css/base/common-mobile.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-page.css` & `xnote-web-0.1.0/static/css/base/common-page.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-photo.css` & `xnote-web-0.1.0/static/css/base/common-photo.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-tab.css` & `xnote-web-0.1.0/static/css/base/common-tab.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common-tag.css` & `xnote-web-0.1.0/static/css/base/common-tag.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/common.css` & `xnote-web-0.1.0/static/css/base/common.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/base/reset.css` & `xnote-web-0.1.0/static/css/base/reset.css`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,18 @@
     font-size: 14px;
 }
 
 textarea:focus, input:focus {
     border: 1px solid #8cc;
 }
 
+textarea:read-only, input[type=text]:read-only {
+    background-color: #eee;
+}
+
 select {
     padding: 5px;
     border: 1px solid #ccc;
 }
 
 /** 链接样式 **/
 a {
```

### Comparing `xnote-web-0.0.9/static/css/common-card.css` & `xnote-web-0.1.0/static/css/common-card.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/common-left.css` & `xnote-web-0.1.0/static/css/common-left.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/common-react.css` & `xnote-web-0.1.0/static/css/common-react.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/font-awesome.min.css` & `xnote-web-0.1.0/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/message.css` & `xnote-web-0.1.0/static/css/message.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/note.css` & `xnote-web-0.1.0/static/css/note.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/plugins.css` & `xnote-web-0.1.0/static/css/plugins.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/timeline.css` & `xnote-web-0.1.0/static/css/timeline.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/css/todo.css` & `xnote-web-0.1.0/static/css/todo.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/favicon.ico` & `xnote-web-0.1.0/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/favicon.png` & `xnote-web-0.1.0/static/favicon.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/fonts/fontawesome-webfont.woff` & `xnote-web-0.1.0/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/fonts/fontawesome-webfont.woff2` & `xnote-web-0.1.0/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/checked.png` & `xnote-web-0.1.0/static/image/checked.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/file.png` & `xnote-web-0.1.0/static/image/file.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/file2.png` & `xnote-web-0.1.0/static/image/file2.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/folder3.png` & `xnote-web-0.1.0/static/image/folder3.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_application.svg` & `xnote-web-0.1.0/static/image/icon_application.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_dict.png` & `xnote-web-0.1.0/static/image/icon_dict.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_dict.svg` & `xnote-web-0.1.0/static/image/icon_dict.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_recent.png` & `xnote-web-0.1.0/static/image/icon_recent.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_recent.svg` & `xnote-web-0.1.0/static/image/icon_recent.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_right.png` & `xnote-web-0.1.0/static/image/icon_right.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_script.png` & `xnote-web-0.1.0/static/image/icon_script.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_script.svg` & `xnote-web-0.1.0/static/image/icon_script.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_search.png` & `xnote-web-0.1.0/static/image/icon_search.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_search.svg` & `xnote-web-0.1.0/static/image/icon_search.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_settings_applications.png` & `xnote-web-0.1.0/static/image/icon_settings_applications.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_settings_applications.svg` & `xnote-web-0.1.0/static/image/icon_settings_applications.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_shell.png` & `xnote-web-0.1.0/static/image/icon_shell.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_shell.svg` & `xnote-web-0.1.0/static/image/icon_shell.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icon_txt.png` & `xnote-web-0.1.0/static/image/icon_txt.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icons/icon_barcode.png` & `xnote-web-0.1.0/static/image/icons/icon_barcode.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icons/icon_game.png` & `xnote-web-0.1.0/static/image/icons/icon_game.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icons/icon_network.png` & `xnote-web-0.1.0/static/image/icons/icon_network.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/image/icons/icon_work.png` & `xnote-web-0.1.0/static/image/icons/icon_work.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/Lexer.js` & `xnote-web-0.1.0/static/js/Lexer.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/admin.js` & `xnote-web-0.1.0/static/js/admin.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/app.build.js` & `xnote-web-0.1.0/static/js/app.build.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -3742,14 +3742,15 @@
 };
 
 
 // 删除文件
 FileView.delete = function(target) {
     var path = $(target).attr("data-path");
     var name = $(target).attr("data-name");
+
     xnote.confirm("确定删除【" + name + "】?", function(value) {
         xnote.http.post("/fs_api/remove", {
             path: path
         }, function(resp) {
             if (resp.code == "success") {
                 window.location.reload();
             } else {
@@ -3759,14 +3760,37 @@
     });
 };
 
 // 重命名
 FileView.rename = function(target) {
     var filePath = $(target).attr("data-path");
     var oldName = $(target).attr("data-name");
+    var realname = $(target).attr("data-realname");
+    if (xnote.isEmpty(realname)) {
+        realname = oldName;
+    }
+
     var dirname = $("#currentDir").val();
     xnote.prompt("输入新的文件名", oldName, function(newName) {
-        FileAPI.rename(dirname, oldName, newName, function(resp) {
+        FileAPI.rename(dirname, realname, newName, function(resp) {
             window.location.reload();
         });
     });
+};
+
+// 打开选项对话框
+FileView.openOptionDialog = function(target) {
+    console.log(window.event);
+    window.event.preventDefault();
+    window.event.stopPropagation();
+    console.log(target);
+    var filePath = $(target).attr("data-path");
+    var fileName = $(target).attr("data-name");
+    var fileRealName = $(target).attr("data-realname");
+    var html = $("#fileItemOptionDialog").render({
+        "filePath": filePath,
+        "fileName": fileName,
+        "fileRealName": fileRealName
+    });
+
+    xnote.openDialog("选项", html);
 };
```

### Comparing `xnote-web-0.0.9/static/js/app.js` & `xnote-web-0.1.0/static/js/app.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/ajax.js` & `xnote-web-0.1.0/static/js/base/ajax.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/array.js` & `xnote-web-0.1.0/static/js/base/array.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/datetime.js` & `xnote-web-0.1.0/static/js/base/datetime.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/jq-ext.js` & `xnote-web-0.1.0/static/js/base/jq-ext.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/misc.js` & `xnote-web-0.1.0/static/js/base/misc.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/string.js` & `xnote-web-0.1.0/static/js/base/string.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/base/url.js` & `xnote-web-0.1.0/static/js/base/url.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/codemirror-addon/xnote-search.js` & `xnote-web-0.1.0/static/js/codemirror-addon/xnote-search.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/colors.js` & `xnote-web-0.1.0/static/js/colors.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/components/date-picker.js` & `xnote-web-0.1.0/static/js/components/date-picker.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/console.js` & `xnote-web-0.1.0/static/js/console.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/editor-csv.js` & `xnote-web-0.1.0/static/js/editor-csv.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/editor.js` & `xnote-web-0.1.0/static/js/editor.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/fs/fs.js` & `xnote-web-0.1.0/static/js/fs/fs.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -29,14 +29,15 @@
 };
 
 
 // 删除文件
 FileView.delete = function(target) {
     var path = $(target).attr("data-path");
     var name = $(target).attr("data-name");
+
     xnote.confirm("确定删除【" + name + "】?", function(value) {
         xnote.http.post("/fs_api/remove", {
             path: path
         }, function(resp) {
             if (resp.code == "success") {
                 window.location.reload();
             } else {
@@ -46,14 +47,37 @@
     });
 };
 
 // 重命名
 FileView.rename = function(target) {
     var filePath = $(target).attr("data-path");
     var oldName = $(target).attr("data-name");
+    var realname = $(target).attr("data-realname");
+    if (xnote.isEmpty(realname)) {
+        realname = oldName;
+    }
+
     var dirname = $("#currentDir").val();
     xnote.prompt("输入新的文件名", oldName, function(newName) {
-        FileAPI.rename(dirname, oldName, newName, function(resp) {
+        FileAPI.rename(dirname, realname, newName, function(resp) {
             window.location.reload();
         });
     });
+};
+
+// 打开选项对话框
+FileView.openOptionDialog = function(target) {
+    console.log(window.event);
+    window.event.preventDefault();
+    window.event.stopPropagation();
+    console.log(target);
+    var filePath = $(target).attr("data-path");
+    var fileName = $(target).attr("data-name");
+    var fileRealName = $(target).attr("data-realname");
+    var html = $("#fileItemOptionDialog").render({
+        "filePath": filePath,
+        "fileName": fileName,
+        "fileRealName": fileRealName
+    });
+
+    xnote.openDialog("选项", html);
 };
```

### Comparing `xnote-web-0.0.9/static/js/marked-ext.js` & `xnote-web-0.1.0/static/js/marked-ext.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/message/message.js` & `xnote-web-0.1.0/static/js/message/message.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/note.js` & `xnote-web-0.1.0/static/js/note.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/old/TagEditor.js` & `xnote-web-0.1.0/static/js/old/TagEditor.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/old/fileEditor.js` & `xnote-web-0.1.0/static/js/old/fileEditor.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/plan/plan.js` & `xnote-web-0.1.0/static/js/plan/plan.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/plugin/plugin.form.js` & `xnote-web-0.1.0/static/js/plugin/plugin.form.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/upload.js` & `xnote-web-0.1.0/static/js/upload.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/utils.build.js` & `xnote-web-0.1.0/static/js/utils.build.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/layer.photos.js` & `xnote-web-0.1.0/static/js/xnote-ui/layer.photos.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-audio.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-audio.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-device.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-device.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-dialog.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-dialog.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-dropdown.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-dropdown.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-event.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-event.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-init.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-init.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-layout.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-layout.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-photo.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-photo.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-tab.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-tab.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-template.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-template.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-upload.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-upload.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/js/xnote-ui/x-url.js` & `xnote-web-0.1.0/static/js/xnote-ui/x-url.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/JsBarcode/JsBarcode.all.min.js` & `xnote-web-0.1.0/static/lib/JsBarcode/JsBarcode.all.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/art-template/template-web-4.13.2.js` & `xnote-web-0.1.0/static/lib/art-template/template-web-4.13.2.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/base64.js/base64.js` & `xnote-web-0.1.0/static/lib/base64.js/base64.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/bootstrap/bootstrap-3.3.5.min.css` & `xnote-web-0.1.0/static/lib/bootstrap/bootstrap-3.3.5.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/clipboard/clipboard-2.0.4.min.js` & `xnote-web-0.1.0/static/lib/clipboard/clipboard-2.0.4.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/5.41.0/codemirror.min.css` & `xnote-web-0.1.0/static/lib/codemirror/5.41.0/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/5.41.0/codemirror.min.js` & `xnote-web-0.1.0/static/lib/codemirror/5.41.0/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/5.65.12/codemirror.css` & `xnote-web-0.1.0/static/lib/codemirror/5.65.12/codemirror.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/5.65.12/codemirror.js` & `xnote-web-0.1.0/static/lib/codemirror/5.65.12/codemirror.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/dialog/dialog.css` & `xnote-web-0.1.0/static/lib/codemirror/addon/dialog/dialog.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/dialog/dialog.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/dialog/dialog.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/anyword-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/anyword-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/css-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/css-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/html-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/html-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/javascript-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/javascript-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/show-hint.css` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/show-hint.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/show-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/show-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/sql-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/sql-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/hint/xml-hint.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/hint/xml-hint.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/search/jump-to-line.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/search/jump-to-line.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/search/search.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/search/search.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/addon/search/searchcursor.js` & `xnote-web-0.1.0/static/lib/codemirror/addon/search/searchcursor.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/codemirror.min.css` & `xnote-web-0.1.0/static/lib/codemirror/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/codemirror.min.js` & `xnote-web-0.1.0/static/lib/codemirror/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/keymap/sublime.js` & `xnote-web-0.1.0/static/lib/codemirror/keymap/sublime.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/clike/clike.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/clike/clike.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/css.min.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/css.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/javascript.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/javascript.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/markdown.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/markdown.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/php.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/php.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/properties.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/properties.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/python.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/python.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/shell.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/shell.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/mode/sql.min.js` & `xnote-web-0.1.0/static/lib/codemirror/mode/sql.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/theme/eclipse.css` & `xnote-web-0.1.0/static/lib/codemirror/theme/eclipse.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/theme/monokai.min.css` & `xnote-web-0.1.0/static/lib/codemirror/theme/monokai.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/codemirror/theme/xq-light.css` & `xnote-web-0.1.0/static/lib/codemirror/theme/xq-light.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/csv.js/csv.js` & `xnote-web-0.1.0/static/lib/csv.js/csv.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/d3/d3.js` & `xnote-web-0.1.0/static/lib/d3/d3.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/d3/d3.min.js` & `xnote-web-0.1.0/static/lib/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/exif-js/exif.js` & `xnote-web-0.1.0/static/lib/exif-js/exif.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/css/font-awesome.css` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/css/font-awesome.min.css` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/FontAwesome.otf` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.eot` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.svg` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.ttf` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff2` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/animated.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/animated.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/bordered-pulled.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/bordered-pulled.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/font-awesome.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/icons.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/icons.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/mixins.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/mixins.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/path.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/path.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/rotated-flipped.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/less/variables.less` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/less/variables.less`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_animated.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_animated.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_bordered-pulled.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_bordered-pulled.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_icons.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_mixins.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_path.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_rotated-flipped.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/font-awesome-4.7.0/scss/_variables.scss` & `xnote-web-0.1.0/static/lib/font-awesome-4.7.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/highlight.js/11.6.0/highlight.min.js` & `xnote-web-0.1.0/static/lib/highlight.js/11.6.0/highlight.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/highlight.js/11.6.0/styles/default.min.css` & `xnote-web-0.1.0/static/lib/highlight.js/11.6.0/styles/default.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/highlight.js/11.7.0/styles/a11y-dark.min.css` & `xnote-web-0.1.0/static/lib/highlight.js/11.7.0/styles/a11y-dark.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jexcel.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jexcel.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jexcel.min.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jexcel.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.css` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.min.css` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jcalendar.min.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jcalendar.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.css` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.min.css` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jdropdown.min.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jdropdown.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.css` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.min.css` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jexcel/2.0.2/jquery.jexcel.min.js` & `xnote-web-0.1.0/static/lib/jexcel/2.0.2/jquery.jexcel.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery/jquery-1.12.4.min.js` & `xnote-web-0.1.0/static/lib/jquery/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery-url-parser/purl.js` & `xnote-web-0.1.0/static/lib/jquery-url-parser/purl.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery-url-parser/purl.min.js` & `xnote-web-0.1.0/static/lib/jquery-url-parser/purl.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery.qrcode/jquery.qrcode.min.js` & `xnote-web-0.1.0/static/lib/jquery.qrcode/jquery.qrcode.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery.terminal/dterm.js` & `xnote-web-0.1.0/static/lib/jquery.terminal/dterm.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.css` & `xnote-web-0.1.0/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.js` & `xnote-web-0.1.0/static/lib/jquery.terminal/jquery.terminal-1.3.1.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jsdiff/diff.js` & `xnote-web-0.1.0/static/lib/jsdiff/diff.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/README.md` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/WEBCOMPONENT.md` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/WEBCOMPONENT.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.css` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.js` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/deps/jsuites.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.css` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.js` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.theme.css` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/dist/jexcel.theme.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/de_DE.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/de_DE.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/en_GB.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/en_GB.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/fr_FR.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/fr_FR.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/it_IT.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/it_IT.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/pt_BR.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/pt_BR.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/lang/zh_CN.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/lang/zh_CN.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/package.json` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/package.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/jspreadsheet-ce-4.6.0/webcomponent-spreadsheet.md` & `xnote-web-0.1.0/static/lib/jspreadsheet-ce-4.6.0/webcomponent-spreadsheet.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layDate-v5.0.9/laydate.js` & `xnote-web-0.1.0/static/lib/layDate-v5.0.9/laydate.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.eot` & `xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.eot`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.svg` & `xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.svg`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.ttf` & `xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/font/iconfont.woff` & `xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/font/iconfont.woff`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layDate-v5.0.9/theme/default/laydate.css` & `xnote-web-0.1.0/static/lib/layDate-v5.0.9/theme/default/laydate.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/layer.full.js` & `xnote-web-0.1.0/static/lib/layer/layer.full.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/layer.js` & `xnote-web-0.1.0/static/lib/layer/layer.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/mobile/layer.js` & `xnote-web-0.1.0/static/lib/layer/mobile/layer.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/mobile/need/layer.css` & `xnote-web-0.1.0/static/lib/layer/mobile/need/layer.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/theme/default/icon-ext.png` & `xnote-web-0.1.0/static/lib/layer/theme/default/icon-ext.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/theme/default/icon.png` & `xnote-web-0.1.0/static/lib/layer/theme/default/icon.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/theme/default/layer.css` & `xnote-web-0.1.0/static/lib/layer/theme/default/layer.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/theme/default/loading-0.gif` & `xnote-web-0.1.0/static/lib/layer/theme/default/loading-0.gif`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/theme/default/loading-1.gif` & `xnote-web-0.1.0/static/lib/layer/theme/default/loading-1.gif`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/layer/theme/default/loading-2.gif` & `xnote-web-0.1.0/static/lib/layer/theme/default/loading-2.gif`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/marked/marked.js` & `xnote-web-0.1.0/static/lib/marked/marked.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/md5.js` & `xnote-web-0.1.0/static/lib/md5.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/package-lock.json` & `xnote-web-0.1.0/static/lib/package-lock.json`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/quarkjs/quark.base-1.0.0.min.js` & `xnote-web-0.1.0/static/lib/quarkjs/quark.base-1.0.0.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/require-2.1.17.js` & `xnote-web-0.1.0/static/lib/require-2.1.17.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/requirejs/require-2.3.6.js` & `xnote-web-0.1.0/static/lib/requirejs/require-2.3.6.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/string-format/string-format.js` & `xnote-web-0.1.0/static/lib/string-format/string-format.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/string-format/string-format.min.js` & `xnote-web-0.1.0/static/lib/string-format/string-format.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/string.js/string-3.3.1.min.js` & `xnote-web-0.1.0/static/lib/string.js/string-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/string.js/string.js` & `xnote-web-0.1.0/static/lib/string.js/string.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/utf.js` & `xnote-web-0.1.0/static/lib/utf.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/vue/vue-2.2.6.min.js` & `xnote-web-0.1.0/static/lib/vue/vue-2.2.6.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/vue/vue-2.7.9.min.js` & `xnote-web-0.1.0/static/lib/vue/vue-2.7.9.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/wangEditor/wangEditor-3.1.1.min.js` & `xnote-web-0.1.0/static/lib/wangEditor/wangEditor-3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/webuploader/README.md` & `xnote-web-0.1.0/static/lib/webuploader/README.md`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/webuploader/Uploader.swf` & `xnote-web-0.1.0/static/lib/webuploader/Uploader.swf`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/webuploader/webuploader.css` & `xnote-web-0.1.0/static/lib/webuploader/webuploader.css`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/lib/webuploader/webuploader.nolog.min.js` & `xnote-web-0.1.0/static/lib/webuploader/webuploader.nolog.min.js`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/xnote.pdn` & `xnote-web-0.1.0/static/xnote.pdn`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/static/xnote.png` & `xnote-web-0.1.0/static/xnote.png`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_admin.py` & `xnote-web-0.1.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_app.py` & `xnote-web-0.1.0/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2017-05-23 00:30:19
 @LastEditors  : xupingmao
-@LastEditTime : 2023-10-29 17:02:22
+@LastEditTime : 2024-04-20 16:42:38
 @FilePath     : /xnote/tests/test_app.py
 @Description  : 描述
 """
 
 import os
 import xutils
 from xnote.core import xtemplate, xconfig, xtables, xauth, xmanager
@@ -293,26 +293,14 @@
 
     def test_code_wiki(self):
         self.check_200("/code/wiki/README.md")
 
     def test_cron_list(self):
         self.check_200("/system/crontab")
 
-    def test_cron_add_url(self):
-        result = json_request("/system/crontab/add", method="POST",
-                              data=dict(url="test", tm_wday="*", tm_hour="*", tm_min="*"))
-        sched_id = result["data"]["id"]
-        self.check_OK("/system/crontab/remove?id={}".format(sched_id))
-
-    def test_cron_add_script(self):
-        result = json_request("/system/crontab/add", method="POST",
-                              data=dict(script_url="script://test.py", tm_wday="1", tm_hour="*", tm_min="*"))
-        sched_id = result["data"]["id"]
-        self.check_OK("/system/crontab/remove?id={}".format(sched_id))
-
     def test_BaseTextPlugin(self):
         TextPage().render()
 
     def test_plugin(self):
         code = '''
 # @api-level 2.8
 # @title Unit-Test-Plugin
```

### Comparing `xnote-web-0.0.9/tests/test_base.py` & `xnote-web-0.1.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_dict.py` & `xnote-web-0.1.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_exif.py` & `xnote-web-0.1.0/tests/test_exif.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_fs.py` & `xnote-web-0.1.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_message.py` & `xnote-web-0.1.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_note.py` & `xnote-web-0.1.0/tests/test_note.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_search.py` & `xnote-web-0.1.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_system_sync.py` & `xnote-web-0.1.0/tests/test_system_sync.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_user.py` & `xnote-web-0.1.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_xauth.py` & `xnote-web-0.1.0/tests/test_xauth.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_xmanager.py` & `xnote-web-0.1.0/tests/test_xmanager.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_xutils.py` & `xnote-web-0.1.0/tests/test_xutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,20 @@
             path = "/root/test"
             pathlist = xutils.splitpath(path)
             self.assertEqual(2, len(pathlist))
 
     def test_decode_name(self):
         self.assertEqual("a.txt", xutils.decode_name("a.txt"))
         self.assertEqual("a.txt", xutils.decode_name("YS50eHQ=.x0"))
+        self.assertEqual("a.txt", xutils.decode_name("YS50eHQ.x0"))
         self.assertEqual("a.txt", xutils.decode_name("YS50eHQ=.xenc"))
 
     def test_encode_name(self):
-        self.assertEqual("YS50eHQ=.x0", xutils.encode_name("a.txt"))
-        self.assertEqual("YS50eHQ=.x0", xutils.encode_name("YS50eHQ=.x0"))
+        self.assertEqual("YS50eHQ.x0", xutils.encode_name("a.txt"))
+        self.assertEqual("YS50eHQ.x0", xutils.encode_name("YS50eHQ.x0"))
 
     def test_edit_distance(self):
         self.assertEqual(1, xutils.edit_distance("abcd","abc"))
         self.assertEqual(2, xutils.edit_distance("abcd", "ab"))
         self.assertEqual(6, xutils.edit_distance("abc", "def"))
         self.assertEqual(3, xutils.edit_distance("kkabcd", "abc"))
```

### Comparing `xnote-web-0.0.9/tests/test_xutils_cache.py` & `xnote-web-0.1.0/tests/test_xutils_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,14 @@
 
     def test_cache_set_delete(self):
         cacheutil.set("name", 123, expire = 600)
         self.assertEqual(123, cacheutil.get("name"))
         cacheutil.delete("name")
         self.assertEqual(None, cacheutil.get("name"))
 
-    def test_cache_load_dump(self):
-        cacheutil.load_dump()
-
     def test_cache_hash(self):
         cacheutil.hset("h01", "key", "value", expire = 600)
         value = cacheutil.hget("h01", "key")
         self.assertEqual("value", value)
         self.assertEqual(None, cacheutil.hget("h01", "key02"))
 
     def test_cache_call(self):
```

### Comparing `xnote-web-0.0.9/tests/test_xutils_db.py` & `xnote-web-0.1.0/tests/test_xutils_db.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_xutils_db_hash_table.py` & `xnote-web-0.1.0/tests/test_xutils_db_hash_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2023-04-29 18:57:21
 @LastEditors  : xupingmao
-@LastEditTime : 2023-05-20 22:45:02
+@LastEditTime : 2024-04-13 20:34:44
 @FilePath     : /xnote/tests/test_xutils_db_hash_table.py
 @Description  : 描述
 """
 
 from . import test_base
 from xutils import dbutil, Storage
 
 app = test_base.init()
 dbutil.register_table("hash_test", "测试数据库")
+dbutil.register_table("lk_hash_test", "测试数据库")
 
 class TestMain(test_base.BaseTestCase):
 
     def get_table(self):
         return dbutil.get_hash_table("hash_test")
     
     def drop_table(self):
@@ -59,7 +60,16 @@
         self.assertEqual("admin", found.name)
         self.assertEqual(20, found.age)
 
         key, first = table.first(where=dict(age=20))
         self.assertEqual("admin", first.name)
         self.assertEqual(20, first.age)
 
+
+    def test_large_key_hash(self):
+        db = dbutil.LargeKeyHashTable(table_name="lk_hash_test")
+        db.put("test", 1)
+        value = db.get("test")
+        assert value == 1
+        db.delete("test")
+        assert db.get("test") == None
+
```

### Comparing `xnote-web-0.0.9/tests/test_xutils_db_table.py` & `xnote-web-0.1.0/tests/test_xutils_db_table.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/tests/test_xutils_sqldb.py` & `xnote-web-0.1.0/tests/test_xutils_sqldb.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/__init__.py` & `xnote-web-0.1.0/xnote/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/autoreload.py` & `xnote-web-0.1.0/xnote/core/autoreload.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xauth.py` & `xnote-web-0.1.0/xnote/core/xauth.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xconfig.py` & `xnote-web-0.1.0/xnote/core/xconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2023-10-27 21:17:40
 @LastEditors  : xupingmao
-@LastEditTime : 2024-02-14 19:15:31
+@LastEditTime : 2024-05-02 22:05:57
 @FilePath     : /xnote/xnote/core/xconfig.py
 @Description  : 描述
 """
 # encoding=utf-8
 # @author xupingmao
 # @modified 2022/03/19 18:10:06
 # @filename xconfig.py
@@ -39,14 +39,15 @@
 # 菜单配置
 
 '''
 import os
 import time
 import json
 import xutils
+import logging
 from xutils import textutil
 from xutils import fsutil
 from xutils.base import Storage
 
 __version__ = "1.0"
 __author__ = "xupingmao (578749341@qq.com)"
 __copyright__ = "(C) 2016-2023 xupingmao. GNU GPL 3."
@@ -83,15 +84,15 @@
 # 线程数
 MIN_THREADS = 20
 # 打开浏览器
 OPEN_IN_BROWSER = False
 # 启用数据库的缓存搜索
 USE_CACHE_SEARCH = False
 # 文件系统使用urlencode方式,适用于只支持ASCII字符的系统
-USE_URLENCODE = False
+USE_URLENCODE = True
 # 初始化脚本
 INIT_SCRIPT = "init.py"
 
 # *** 样式设置 ***
 # BASE_TEMPLATE = "common/theme/sidebar.html"
 BASE_TEMPLATE = "common/base.html"
 # 主题样式
@@ -225,18 +226,20 @@
 
     data_dir = ""
     sqlite_dir = ""
     backup_dir = ""
     backup_db_dir = ""
     db_dir = ""
     files_dir = ""
+    tmp_dir = ""
 
     boot_lock_file = "" # 启动的锁文件
     record_db_name = "" # 默认的sqlite数据库名称
     record_db_file = "" # 默认的sqlite数据库路径
+    kv_db_name = "kv_store"
     kv_db_file = ""
 
     source_root_dir = "" # 源码根目录
     plugins_dir = "" # 插件目录
     ext_handlers_dir = "./ext_handlers"
 
     db_backup_expire_days = 5
@@ -264,29 +267,44 @@
 
         cls.backup_dir = os.path.join(data_dir, "backup")
         makedirs(cls.backup_dir)
 
         cls.backup_db_dir = os.path.join(cls.backup_dir, "db")
         makedirs(cls.backup_db_dir)
 
+        cls.tmp_dir = os.path.join(data_dir, "tmp")
+        makedirs(cls.tmp_dir)
+
         cls.record_db_name = SystemConfig.get_str("record_db_name", "record")
         cls.record_db_file = cls.get_db_path(cls.record_db_name)
-        cls.kv_db_file = cls.get_db_path("kv_store")
+
+        cls.kv_db_name = SystemConfig.get_str("kv_db_name", "kv_store")
+        cls.kv_db_file = cls.get_db_path(cls.kv_db_name)
+
         cls.db_backup_expire_days = SystemConfig.get_int("db_backup_expire_days", 5)
         cls.plugins_dir = os.path.join(cls.data_dir, "scripts", "plugins")
         cls.plugins_upload_dir = os.path.join(cls.plugins_dir, "upload")
 
         cls.template_base_nav_left = SystemConfig.get_str("template_base_nav_left", "common/nav/base_nav_left.html")
         cls.template_base_nav_top = SystemConfig.get_str("template_base_nav_top", "common/nav/base_nav_top.html")
 
         cls.boot_lock_file = SystemConfig.get_str("boot_lock_file", "pid.lock")
+        cls.enable_boot_lock = SystemConfig.get_bool("enable_boot_lock", True)
+
+        global USE_URLENCODE
+        USE_URLENCODE = SystemConfig.get_bool("fs_encode_name", True)
+        fsutil.FileUtilConfig.encode_name = USE_URLENCODE
 
     @classmethod
     def get_db_path(cls, dbname=""):
         """dbname: sqlite数据库的文件名称"""
+        if dbname in ("$temp", "$tmp"):
+            tmp_file_path = fsutil.get_tmp_path(ext=".db")
+            logging.info("tmp_file_path=%s", tmp_file_path)
+            return tmp_file_path
         if not dbname.endswith(".db"):
             dbname += ".db"
         return os.path.join(cls.sqlite_dir, dbname)
 
     @classmethod
     def get_backup_db_path(cls, dbname=""):
         if not dbname.endswith(".db"):
@@ -417,19 +435,21 @@
 
 class DatabaseConfig:
 
     db_driver = "" # sqlite/mysql/leveldb/ssdb
     db_driver_cache = "" # memory/redis
     db_driver_sql = "" # sqlite/mysql
     db_driver_kv = ""  # sqlite/mysql/leveldb/ssdb
+    kv_store = "kv_store" # SQL模拟KV的表名
 
     user_max_log_size = 500 # 用户日志保留的最大条数
     db_debug = False
     db_log_debug = False
     db_profile_table_proxy = False
+    db_auto_ddl = True # 自动执行DDL
 
     binlog = False
     binlog_max_size = 10000
     # leveldb配置
     block_cache_size = 16 * 1024**2
     write_buffer_size = 4 * 1024**2
     max_open_files = 1000
@@ -461,14 +481,15 @@
         cls.binlog = SystemConfig.get_bool("binlog")
         cls.binlog_max_size = SystemConfig.get_int("binlog_max_size")
         cls.block_cache_size = SystemConfig.get_int("block_cache_size")
         cls.write_buffer_size = SystemConfig.get_int("write_buffer_size")
         cls.max_open_files = SystemConfig.get_int("max_open_files")
         cls.db_profile_table_proxy = SystemConfig.get_int("db_profile_table_proxy")
         cls.db_sys_log_max_size = SystemConfig.get_int("db_sys_log_max_size", 100000)
+        cls.db_auto_ddl = SystemConfig.get_bool("db_auto_ddl", True)
 
         cls.sqlite_journal_mode = SystemConfig.get_str("sqlite_journal_mode", "delete")
         cls.sqlite_page_size = SystemConfig.get_int("sqlite_page_size", 0)
 
         cls.ssdb_host = SystemConfig.get_str("ssdb_host", "127.0.0.1")
         cls.ssdb_port = SystemConfig.get_int("ssdb_port", 8888)
```

### Comparing `xnote-web-0.0.9/xnote/core/xmanager.py` & `xnote-web-0.1.0/xnote/core/xmanager.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xnote_app.py` & `xnote-web-0.1.0/xnote/core/xnote_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import argparse
 import logging
 import time
 import sys
 import os
 from .autoreload import AutoReloadThread
 from xutils.db import dbutil_cache
-from xutils.lockutil import FileLock
+from xutils.lockutil import FileLockAdapter, DummyLock
 from xutils.mem_util import log_mem_info_deco
 from xutils import mem_util
 from xutils import Storage
 from xutils import dbutil
 from xutils import cacheutil, interfaces
 from xutils.sqldb import TableProxy
 from . import xnote_code_builder
@@ -286,14 +286,15 @@
 
 
 def init_xutils():
     xutils.init(xconfig)
     from xutils.fsutil import FileUtilConfig
     FileUtilConfig.data_dir = xconfig.FileConfig.data_dir
     FileUtilConfig.use_urlencode = xconfig.USE_URLENCODE
+    FileUtilConfig.tmp_dir = xconfig.FileConfig.tmp_dir
 
 def init_app_internal(boot_config_kw=None):
     """初始化APP内部方法"""
     global app
     print_env_info()
 
     # 构建静态文件
@@ -358,37 +359,44 @@
             return
 
 
 def run_init_hooks(app):
     for func in xnote_hooks.get_init_hooks():
         func(app)
 
+def get_file_lock():
+    if xconfig.FileConfig.enable_boot_lock:
+        return FileLockAdapter(xconfig.FileConfig.boot_lock_file)
+    return DummyLock()
 
 def main(boot_config_kw=None):
     global app
 
     # 处理初始化参数
     handle_args_and_init_config(boot_config_kw=boot_config_kw)
 
-    file_lock = FileLock(xconfig.FileConfig.boot_lock_file)
+    xnote_version = xconfig.SystemConfig.get_str("version")
+    logging.info("starting xnote, version: %s", xnote_version)
+
+    file_lock = get_file_lock()
 
     try:
-        if file_lock.acquire():
+        if file_lock.try_lock():
             # 初始化
             init_app_internal(boot_config_kw=boot_config_kw)
             # 执行钩子函数
             run_init_hooks(app)
             # 监听端口
             app.web_app.run()
             logging.info("服务器已关闭")
             wait_thread_exit()
             sys.exit(xconfig.EXIT_CODE)
         else:
             logging.error("get lock failed")
             logging.error("xnote进程已启动，请不要重复启动!")
             sys.exit(1)
     finally:
-        file_lock.release()
+        file_lock.unlock()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `xnote-web-0.0.9/xnote/core/xnote_code_builder.py` & `xnote-web-0.1.0/xnote/core/xnote_code_builder.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xnote_hooks.py` & `xnote-web-0.1.0/xnote/core/xnote_hooks.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xnote_trace.py` & `xnote-web-0.1.0/xnote/core/xnote_trace.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xnote_user_config.py` & `xnote-web-0.1.0/xnote/core/xnote_user_config.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xtables.py` & `xnote-web-0.1.0/xnote/core/xtables.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,29 +383,42 @@
         manager.add_column("args", "text", "")
         manager.add_index(["user_id", "url"])
     
     # 日志数据, 关闭profile
     TableConfig.disable_profile(table_name)
     TableConfig.disable_binlog(table_name)
 
-def init_sys_job():
+def init_job_table():
     """系统任务
     @since 2024/03/10
     """
-    table_name = "sys_job"
+    table_name = "t_job" # 避免关键字冲突
     comment = "系统任务"
     with create_default_table_manager(table_name, comment=comment) as manager:
         manager.add_column("ctime", "datetime", DEFAULT_DATETIME)
         manager.add_column("mtime", "datetime", DEFAULT_DATETIME)
         manager.add_column("job_type", "varchar(30)", "")
         manager.add_column("job_status", "tinyint", 0, comment="日志状态,0-初始化,1-执行中,2-执行成功,3-执行失败")
         manager.add_column("job_params", "text", "")
         manager.add_column("job_result", "text", "")
         manager.add_index(["job_type", "mtime"])
 
+def init_lock_table():
+    """分布式锁的表
+    @since 2024/04/03
+    """
+    table_name = "t_lock" # 避免和关键字冲突
+    comment = "系统任务"
+    with create_default_table_manager(table_name, comment=comment) as manager:
+        manager.add_column("ctime", "datetime", default_value=DEFAULT_DATETIME)
+        manager.add_column("mtime", "datetime", default_value=DEFAULT_DATETIME)
+        manager.add_column("lock_key", "varchar(128)", default_value="")
+        manager.add_column("lock_token", "varchar(36)", default_value="", comment="锁的token")
+        manager.add_column("timeout_time", "bigint", default_value=0, comment="锁超时时间,毫秒时间戳")
+        manager.add_index("lock_key", is_unique=True)
 
 def init_msg_index_table():
     """随手记索引"""
     table_name = "msg_index"
     comment = "随手记索引"
     with create_default_table_manager(table_name, comment=comment) as manager:
         # 展示创建时间
@@ -623,26 +636,30 @@
 
 @xutils.log_init_deco("xtables")
 def init():
     TableManager.clear_table_dict()
     web.db.config.debug_sql = xconfig.DatabaseConfig.db_debug
 
     TableConfig.enable_binlog = xconfig.DatabaseConfig.binlog
+    TableConfig.enable_auto_ddl = xconfig.DatabaseConfig.db_auto_ddl
+
     if xconfig.DatabaseConfig.db_profile_table_proxy:
         dbutil.register_table("sys_log", "系统日志")
         TableProxy.profile_logger = DBProfileLogger()
         TableProxy.log_profile = True
     
     init_dict_table()
     init_record_table()
     init_user_table()
     init_file_info()
     
-    # 系统任务
-    init_sys_job()
+    # 持久化任务表
+    init_job_table()
+    # 分布式锁表
+    init_lock_table()
     
     # 统计信息
     init_site_visit_log()
     init_page_visit_log()
     
     # 标签相关
     init_note_tag_rel_table() # 已删除, 占位防止冲突
@@ -665,9 +682,9 @@
     # 通用的分享记录
     init_share_info_table()
     
     if xconfig.DatabaseConfig.db_driver_sql == "mysql":
         init_kv_store_table()
         init_kv_zset_table(get_db_instance())
     
-    if xconfig.DatabaseConfig.db_driver == "sqlite":
+    if xconfig.DatabaseConfig.db_driver_sql == "sqlite":
         init_kv_store_table()
```

### Comparing `xnote-web-0.0.9/xnote/core/xtables_kv.py` & `xnote-web-0.1.0/xnote/core/xtables_kv.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/core/xtemplate.py` & `xnote-web-0.1.0/xnote/core/xtemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         for template_mapping in self.template_mapping_list:
             if name.startswith(template_mapping.prefix):
                 relative_path = name[len(template_mapping.prefix):]
                 return os.path.join(template_mapping.dirname, relative_path)
         
         if name.endswith(".str"):
-            # 字符串类型的模板,只在内存种存在
+            # 字符串类型的模板,只在内存中存在
             return name
 
         return os.path.join(xconfig.HANDLERS_DIR, name)
 
     def _create_template(self, name):
         if name.endswith(".str"):
             return Template(name, name=name, loader=self)
@@ -267,16 +267,18 @@
 def render_text(text, template_name="<string>", **kw):
     """使用模板引擎渲染文本信息,使用缓存
     TODO 控制缓存大小，使用FIFO或者LRU淘汰
     """
     nkw = do_render_kw(kw)
 
     # 使用hash不能保证唯一性
-    name = "template@%s.str" % id(text)
-    _loader.init_template(name, text)
+    text_md5 = xutils.md5_hex(text)
+    name = f"template@{template_name}_{text_md5}.str"
+    if name not in _loader.templates:
+        _loader.init_template(name, text)
     return _loader.load(name).generate(**nkw)
 
 
 def get_code(name):
     return _loader.load(name).code
 
 
@@ -403,16 +405,16 @@
         self.html_footer = render_text(html, **kw)
 
     def writehtml(self, html, **kw):
         """@deprecated 请使用 #writebody
         这个方法现在和 `writetemplate` 等价"""
         return self.writetemplate(html, **kw)
 
-    def writetemplate(self, template, **kw):
-        html = render_text(template, **kw)
+    def writetemplate(self, template_text, **kw):
+        html = render_text(template_text, template_name=self.title, **kw)
         self.html += u(html.decode("utf-8"))
         return self.html
 
     def write_aside(self, template, **kw):
         self.show_aside = True
         self.show_right = True
         self.aside_html = render_text(template, **kw)
@@ -443,23 +445,23 @@
         return TextResponse(html)
 
     def handle(self, input):
         """子类实现这个方法"""
         raise NotImplementedError()
 
     def get_input(self):
-        return xutils.get_argument("input", "")
+        return xutils.get_argument_str("input", "")
 
     def get_format(self):
         """返回当前请求的数据格式"""
         return xutils.get_argument_str("_format", "")
 
     def get_page(self):
         """返回当前页码"""
-        return xutils.get_argument("page", 1, type=int)
+        return xutils.get_argument_int("page", 1)
 
     def check_access(self):
         role = xauth.get_current_role()
         if role in self.permitted_role_list:
             return
 
         if self.require_admin:
```

### Comparing `xnote-web-0.0.9/xnote/plugin/component.py` & `xnote-web-0.1.0/xnote/plugin/component.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/plugin/form.py` & `xnote-web-0.1.0/xnote/plugin/form.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,42 +39,50 @@
         self.field = ""
         self.placeholder = ""
         self.value = ""
         self.type = FormRowType.input
         self.css_class = ""
         self.options = []
         self.date_type = FormRowDateType.date # 用于日期组件
+        self.readonly = False
     
     def add_option(self, title="", value=""):
         option = FormRowOption()
         option.title = title
         option.value = value
         self.options.append(option)
         return self
+
+    def get_readonly_attr(self):
+        if self.readonly:
+            return "readonly"
+        else:
+            return ""
     
 class DataForm:
     """数据表格"""
     
     def __init__(self):
         self.id = "0"
         self.row_id = 0
         self.rows = []
         self.save_action = "save"
         self.model_name = "default"
     
-    def add_row(self, title="", field="", placeholder="", value="", type="input", css_class=""):
+    def add_row(self, title="", field="", placeholder="", value="", type="input", css_class="", readonly=False):
         self.row_id += 1
         row = FormRow()
         row.id = f"row_{self.id}_{self.row_id}"
         row.title = title
         row.field = field
         row.placeholder = placeholder
         row.value = value
         row.type = type
         row.css_class = css_class
+        row.readonly = readonly
         
         self.rows.append(row)
         return row
 
     def count_type(self, type=""):
         count = 0
         for item in self.rows:
```

### Comparing `xnote-web-0.0.9/xnote/plugin/plugin.py` & `xnote-web-0.1.0/xnote/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/plugin/table.py` & `xnote-web-0.1.0/xnote/plugin/table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2024-03-10 16:20:05
 @LastEditors  : xupingmao
-@LastEditTime : 2024-03-16 17:21:32
-@FilePath     : /xnote/xnote/core/template/table.py
+@LastEditTime : 2024-04-21 19:15:41
+@FilePath     : /xnote/xnote/plugin/table.py
 @Description  : 描述
 """
 
 class TableActionType:
     """表格动作的类型"""
     link = "link"
     button = "button"
@@ -20,15 +20,28 @@
     """表格的标题单元"""
     def __init__(self):
         self.title = ""
         self.field = ""
         self.link_field = ""
         self.type = ""
         self.width = "auto"
-
+        self.css_class_field = ""
+    
+    def get_css_class(self, row):
+        return row.get(self.css_class_field, "")
+    
+    def get_link(self, row):
+        return row.get(self.link_field)
+    
+    def has_link(self, row):
+        if self.link_field == "":
+            return False
+        link = self.get_link(row)
+        return link not in (None, "")
+    
 class TableAction:
     """表格的操作单元"""
     def __init__(self):
         self.title = ""
         self.type = ""
         self.link_field = ""
         self.title_field = ""
@@ -44,29 +57,39 @@
     
     def get_msg(self, row):
         assert isinstance(row, dict)
         if self.msg_field == "":
             return self.default_msg
         return row.get(self.msg_field)
     
+    def get_link(self, row):
+        return row.get(self.link_field)
+    
+    def has_link(self, row):
+        if self.link_field == "":
+            return False
+        link = self.get_link(row)
+        return link not in (None, "")
+
 class DataTable:
     """数据表格"""
     
     def __init__(self):
         self.heads = []
         self.rows = []
         self.actions = []
     
-    def add_head(self, title="", field = "", type="", link_field="", width="auto"):
+    def add_head(self, title="", field = "", type="", link_field="", width="auto", css_class_field=""):
         head = TableHead()
         head.title = title
         head.field = field
         head.type = type
         head.width = width
         head.link_field = link_field
+        head.css_class_field = css_class_field
         self.heads.append(head)
         
     def add_row(self, obj):
         assert isinstance(obj, dict)
         self.rows.append(obj)
         
     def set_rows(self, rows):
```

### Comparing `xnote-web-0.0.9/xnote/plugin/table_plugin.py` & `xnote-web-0.1.0/xnote/plugin/table_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2024-03-31 11:17:36
 @LastEditors  : xupingmao
-@LastEditTime : 2024-03-31 12:01:04
+@LastEditTime : 2024-04-03 18:32:06
 @FilePath     : /xnote/xnote/plugin/table_plugin.py
 @Description  : 描述
 """
 
 import xutils
 from xnote.core.xtemplate import BasePlugin
 from xutils import Storage
@@ -64,41 +64,45 @@
             return self.handle_delete()
         return self.handle_page()
     
 
     def handle_edit(self):
         form = DataForm()
         form.add_row("id", "id", css_class="hide")
+        form.add_row("只读属性", "readonly_attr", value="test", readonly=True)
+
         row = form.add_row("类型", "type", type=FormRowType.select)
         row.add_option("类型1", "1")
         row.add_option("类型2", "2")
+        
         form.add_row("标题", "title")
         form.add_row("日期", "date", type=FormRowType.date)
         form.add_row("内容", "content", type=FormRowType.textarea)
         
         kw = Storage()
         kw.form = form
         return self.response_form(**kw)
     
     def handle_save(self):
         return webutil.FailedResult(code="500", message="Not Implemented")
     
     def handle_page(self):
         table = DataTable()
         table.add_head("类型", "type")
-        table.add_head("标题", "title")
+        table.add_head("标题", "title", css_class_field="title_class")
         table.add_head("日期", "date")
         table.add_head("内容", "content")
 
         table.add_action("编辑", link_field="edit_url", type=TableActionType.edit_form)
         table.add_action("删除", link_field="delete_url", type=TableActionType.confirm, msg_field="delete_msg", css_class="btn danger")
 
         row = {}
         row["type"] = "类型1"
         row["title"] = "测试"
+        row["title_class"] = "red"
         row["date"] = "2020-01-01"
         row["content"] = "测试内容"
         row["edit_url"] = "?action=edit"
         row["delete_url"] = "?action=delete"
         row["delete_msg"] = "确认删除记录吗?"
         table.add_row(row)
```

### Comparing `xnote-web-0.0.9/xnote/service/comment_service.py` & `xnote-web-0.1.0/xnote/service/comment_service.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote/service/job_service.py` & `xnote-web-0.1.0/xnote/service/job_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2024-03-10 15:34:47
 @LastEditors  : xupingmao
-@LastEditTime : 2024-03-10 16:01:25
-@FilePath     : /xnote/xnote/service/service_job.py
+@LastEditTime : 2024-04-03 23:59:03
+@FilePath     : /xnote/xnote/service/job_service.py
 @Description  : 描述
 """
 
 from xnote.core import xtables
 from xutils import dateutil
 
 class JobStatusEnum:
@@ -59,15 +59,15 @@
             self.job_info.job_status = JobStatusEnum.success
         
         JobService.update_job(self.job_info)
 
 
 class JobService:
     
-    db = xtables.get_table_by_name("sys_job")
+    db = xtables.get_table_by_name("t_job")
     
     @classmethod
     def create_job(cls, job_info):
         assert isinstance(job_info, SysJob)
         assert job_info.id == 0
         
         record = job_info.__dict__
```

### Comparing `xnote-web-0.0.9/xnote/service/tag_service.py` & `xnote-web-0.1.0/xnote/service/tag_service.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/__init__.py` & `xnote-web-0.1.0/xnote_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/base.py` & `xnote-web-0.1.0/xnote_migrate/base.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_001.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_001.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_002.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_002.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_003.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_003.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_004.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_004.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_005.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_005.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_007.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_007.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_009.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_009.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_010.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_010.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_011.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_011.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_012.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_012.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_013.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_013.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_014.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_014.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_015.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_015.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_016.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_016.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_017.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_017.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_migrate/upgrade_018.py` & `xnote-web-0.1.0/xnote_migrate/upgrade_018.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xnote_web.egg-info/PKG-INFO` & `xnote-web-0.1.0/xnote_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnote-web
-Version: 0.0.9
+Version: 0.1.0
 Summary: xnote-web框架
 Author: mark
 Author-email: 578749341@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `xnote-web-0.0.9/xnote_web.egg-info/SOURCES.txt` & `xnote-web-0.1.0/xnote_web.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 config/requirements.test.txt
 config/requirements.txt
 config/requirements.win.txt
 config/version.txt
 config/boot/boot.default.properties
 config/boot/boot.local.follower.properties
 config/boot/boot.local.leveldb.properties
+config/boot/boot.local.mem.properties
 config/boot/boot.local.properties
 config/boot/boot.min.properties
 config/boot/boot.sae.properties
 config/boot/boot.sqlite.properties
 config/boot/boot.test.properties
 config/cron/cron.json
 config/file/audio.properties
@@ -461,14 +462,15 @@
 handlers/settings/page/settings.html
 handlers/system/__init__.py
 handlers/system/backup.py
 handlers/system/cache_admin.py
 handlers/system/clipboard.py
 handlers/system/command.py
 handlers/system/crontab.py
+handlers/system/dao_cron.py
 handlers/system/db_admin.py
 handlers/system/db_index.py
 handlers/system/db_migrate_tools.py
 handlers/system/db_refresh.py
 handlers/system/db_shell.py
 handlers/system/db_upgrade.py
 handlers/system/develop_controller.py
@@ -892,14 +894,15 @@
 tests/test_base.py
 tests/test_dict.py
 tests/test_exif.py
 tests/test_fs.py
 tests/test_message.py
 tests/test_note.py
 tests/test_search.py
+tests/test_service.py
 tests/test_system_sync.py
 tests/test_user.py
 tests/test_xauth.py
 tests/test_xmanager.py
 tests/test_xutils.py
 tests/test_xutils_cache.py
 tests/test_xutils_db.py
@@ -927,14 +930,15 @@
 xnote/plugin/form.py
 xnote/plugin/plugin.py
 xnote/plugin/table.py
 xnote/plugin/table_plugin.py
 xnote/service/__init__.py
 xnote/service/comment_service.py
 xnote/service/job_service.py
+xnote/service/lock_service.py
 xnote/service/tag_service.py
 xnote_migrate/__init__.py
 xnote_migrate/base.py
 xnote_migrate/upgrade_000.py
 xnote_migrate/upgrade_001.py
 xnote_migrate/upgrade_002.py
 xnote_migrate/upgrade_003.py
@@ -1006,14 +1010,15 @@
 xutils/db/driver_sqlite.py
 xutils/db/driver_ssdb.py
 xutils/db/encode.py
 xutils/db/filters.py
 xutils/db/lock.py
 xutils/db/shard.py
 xutils/sqldb/__init__.py
+xutils/sqldb/table_config.py
 xutils/sqldb/table_manager.py
 xutils/sqldb/table_proxy.py
 xutils/sqldb/utils.py
 xutils/tornado/__init__.py
 xutils/tornado/escape.py
 xutils/tornado/log.py
 xutils/tornado/template.py
```

### Comparing `xnote-web-0.0.9/xutils/__init__.py` & `xnote-web-0.1.0/xutils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 建议通过xutils暴露统一接口，其他的utils由xutils导入
 
 """
 from __future__ import print_function
 from __future__ import absolute_import
 
 import shutil
+import subprocess
 import logging
 import logging.handlers
 from threading import current_thread
 
 from xutils.imports import *
 # xnote工具
 import xutils.textutil as textutil
@@ -187,22 +188,14 @@
 
 
 def obj2dict(obj):
     if obj == None:
         return None
     return dict(**obj.__dict__)
 
-
-def get_safe_file_name(filename):
-    """处理文件名中的特殊符号"""
-    for c in " @$:#\\|":
-        filename = filename.replace(c, "_")
-    return filename
-
-
 #################################################################
 ##   Platform/OS Utilities, Python 2 do not have this file
 #################################################################
 
 def system(cmd, cwd = None):
     p = subprocess.Popen(cmd, cwd=cwd, 
                                  shell=True,
```

### Comparing `xnote-web-0.0.9/xutils/base.py` & `xnote-web-0.1.0/xutils/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 # @author xupingmao <578749341@qq.com>
 # @since 2020/11/28 23:23:13
 # @modified 2022/04/16 22:47:23
 import copy
 import sys
 import traceback
 
+IS_PY2 = sys.version_info[0] == 2
+
+if IS_PY2:
+    string_types = (basestring,)
+else:
+    string_types = (str,)
+
+
 class Storage(dict):
     """
     A Storage object is like a dictionary except `obj.foo` can be used
     in addition to `obj['foo']`. (This class is modified from web.py)
     
         >>> o = storage(a=1)
         >>> o.a
@@ -64,7 +72,10 @@
     """打印系统异常堆栈"""
     exc_info = traceback.format_exc()
     print(exc_info)
     return exc_info
 
 def print_stacktrace():
     print_exc()
+
+def is_str(s):
+    return isinstance(s, string_types)
```

### Comparing `xnote-web-0.0.9/xutils/cacheutil.py` & `xnote-web-0.1.0/xutils/cacheutil.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,24 +30,35 @@
 
 * 参考redis的API
 * TODO: 可以使用 BitCask 存储模型实现
 """
 import threading
 import random
 import datetime
+import time
+import re
+import os
+import json
+import inspect
+import sys
+import traceback
+import base64
+
 from xutils import dateutil
 from collections import OrderedDict, deque
-from xutils.imports import *
-from xutils import interfaces
+from xutils import interfaces, Storage
 from xutils.db.dbutil_cache import DatabaseCache
+from xutils.base import is_str
 
 _cache_dict = dict()
 _cache_queue = deque()
-STORAGE_DIR = None
 
+class CacheConfig:
+    """缓存配置"""
+    storage_dir = ""
 
 def encode_key(text):
     """编码key为文件名"""
     return text + ".json"
     # return base64.urlsafe_b64encode(text.encode("utf-8")).decode("utf-8") + ".pk"
 
 
@@ -75,72 +86,81 @@
     # print(msg)
     pass
 
 
 def log_error(msg):
     print(msg)
 
+class JsonSerializer:
+    """缓存编码器"""
 
-class MemoryCache(interfaces.CacheInterface):
-    """缓存实现,一般情况下不要直接用它,优先使用 PrefixedCache, 这样便于迁移到Redis之类的分布式缓存"""
-
-    def __init__(self, max_size = -1):
-        self.dict = OrderedDict()
-        self.expire_dict = dict()
-        self.max_size = max_size
-        self.lock = threading.RLock()
-
+    def format_value(self, value):
+        if isinstance(value, dict):
+            result = dict()
+            for key in value:
+                item_value = value.get(key)
+                if isinstance(item_value, datetime.datetime):
+                    result[key] = dateutil.format_datetime(item_value)
+                else:
+                    result[key] = item_value
+            return result
+        return value
+    
     def _fix_storage(self, obj):
         if isinstance(obj, dict):
             return Storage(**obj)
         if isinstance(obj, list):
             for index, item in enumerate(obj):
                 if isinstance(item, dict):
                     obj[index] = Storage(**item)
             return obj
         return obj
 
+    def encode(self, value):
+        if isinstance(value, bytes):
+            return value
+        else:
+            formatted_value = self.format_value(value)
+            return json.dumps(formatted_value) # 转成json，要保证能够序列化
+
+    def decode(self, value):
+        if isinstance(value, bytes):
+            obj = value
+        else:
+            obj = json.loads(value)
+        return self._fix_storage(obj)
+
+class MemoryCache(interfaces.CacheInterface):
+    """缓存实现,一般情况下不要直接用它,优先使用 PrefixedCache, 这样便于迁移到Redis之类的分布式缓存"""
+
+    def __init__(self, max_size = -1, serializer=JsonSerializer()):
+        self.dict = OrderedDict()
+        self.expire_dict = dict()
+        self.max_size = max_size
+        self.lock = threading.RLock()
+        self.serializer = serializer
+
     def get(self, key, default_value=None):
         assert isinstance(key, str), key
         value = self.dict.get(key)
         if value != None:
             if self.is_alive(key):
                 self.dict[key] = value # 移到最后面
-                if isinstance(value, bytes):
-                    obj = value
-                else:
-                    obj = json.loads(value)
-                return self._fix_storage(obj)
+                return self.serializer.decode(value)
             else:
                 self.delete(key)
         return default_value
     
     def get_raw(self, key):
         return self.dict.get(key)
-    
-    def format_value(self, value):
-        if isinstance(value, dict):
-            result = dict()
-            for key in value:
-                item_value = value.get(key)
-                if isinstance(item_value, datetime.datetime):
-                    result[key] = dateutil.format_datetime(item_value)
-                else:
-                    result[key] = item_value
-            return result
-        return value
 
     def put(self, key, value, expire=60*5, random_range=60*5):
         assert expire > 0
         with self.lock:
-            if isinstance(value, bytes):
-                self.dict[key] = value
-            else:
-                value = self.format_value(value)
-                self.dict[key] = json.dumps(value) # 转成json，要保证能够序列化
+            self.dict[key] = self.serializer.encode(value)
             self.expire_dict[key] = time.time() + expire + random.randint(0, random_range)
             
             if self.max_size > 0:
                 self.check_size_and_clear()
 
     def is_alive(self, key):
         value = self.expire_dict.get(key, 60*5)
@@ -324,16 +344,16 @@
         if len(key) > 200:
             raise ValueError("invalid key: len(key)>200")
 
     def is_valid_key(self, key):
         return self.valid_key_pattern.match(key) != None
 
     def _get_path(self, key):
-        assert STORAGE_DIR != None
-        return os.path.join(STORAGE_DIR, key + ".json")
+        assert CacheConfig.storage_dir != ""
+        return os.path.join(CacheConfig.storage_dir, key + ".json")
 
     def get_dump_value(self):
         if self.type == "zset":
             return dict(**self.value)
         else:
             return self.value
 
@@ -749,45 +769,17 @@
     log_error(exc_info)
 
 
 def json_object_hook(dict_obj):
     return Storage(**dict_obj)
 
 
-def load_dump():
-    dirname = STORAGE_DIR
-    valid_ext_tuple = (".json")
-    for fname in os.listdir(dirname):
-        if not fname.endswith(valid_ext_tuple):
-            continue
-        try:
-            fpath = os.path.join(dirname, fname)
-            with open(fpath, "rb") as fp:
-                pickled = fp.read()
-                if pickled == b'':
-                    continue
-                if fname.endswith(".json"):
-                    dict_obj = json.loads(pickled.decode(
-                        "utf-8"), object_hook=json_object_hook)
-                else:
-                    dict_obj = pickle.loads(pickled)
-                # 持久化的都是不失效的数据
-                obj_type = dict_obj.get("type", "object")
-                obj = CacheObj(
-                    dict_obj["key"], dict_obj["value"], -1, type=obj_type, need_save=False)
-                if obj.is_temp():
-                    os.remove(fpath)
-        except:
-            log_error("failed to load cache %s" % fname)
-            print_exc()
-
-
 def clear_temp():
     for key in _cache_dict.copy():
         value = _cache_dict.get(key)
         if value != None and value.is_temp():
             value.clear()
 
 
-def init(storage_dir):
-    global STORAGE_DIR
-    STORAGE_DIR = storage_dir
+def init(storage_dir=""):
+    CacheConfig.storage_dir = storage_dir
+
```

### Comparing `xnote-web-0.0.9/xutils/dateutil.py` & `xnote-web-0.1.0/xutils/dateutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,27 +63,41 @@
         self.month = 0
         self.day = 0
         self.wday = 0 # week day
 
     def __repr__(self):
         return "(%r,%r,%r)" % (self.year, self.month, self.day)
 
+def to_py_date(date_info):
+    """转换成python内置的date类型"""
+    if isinstance(date_info, str):
+        return datetime.date.fromisoformat(date_info)
+    assert isinstance(date_info, datetime.date)
+    return date_info
+
+def to_py_datetime(datetime_info):
+    """转换成python内置的datetime类型"""
+    if isinstance(datetime_info, str):
+        return datetime.datetime.fromisoformat(datetime_info)
+    assert isinstance(datetime_info, datetime.datetime)
+    return datetime_info
 
 def is_str(s):
     return isinstance(s, str)
 
 def before(days=None, month=None, format=False):
     if days is not None:
         fasttime = time.time() - days * SECONDS_PER_DAY
         if format:
             return format_time(fasttime)
         return fasttime
     return None
 
 def days_before(days, format=False):
+    """获取N天前的日期"""
     seconds = time.time()
     seconds -= days * 3600 * 24
     if format:
         return format_time(seconds)
     return time.localtime(seconds)
 
 
@@ -299,18 +313,32 @@
         month = (month - 1) % 12 + 1
     if days != 0:
         date_obj = datetime.datetime(year=year, month=month, day=day)
         date_obj += datetime.timedelta(days=days)
         return date_obj.year, date_obj.month, date_obj.day
     return int(year), month, day
 
+def get_last_day_of_month(date_info: datetime.date):
+    """获取一个月的最后一天"""
+    new_day = get_days_of_month(date_info.year, date_info.month)
+    return datetime.date(date_info.year, date_info.month, new_day)
+
+def get_first_day_of_month(date_info: datetime.date):
+    """获取一个月的第一天"""
+    return datetime.date(date_info.year, date_info.month, 1)
+
+def get_last_day_of_year(date: datetime.date):
+    """获取一年的最后一天"""
+    return datetime.date(date.year, 12, 31)
+
 def is_leap_year(year):
+    """判断是否是闰年"""
     return ((year % 4 == 0) and (year % 100 != 0)) or (year % 400 == 0)
 
-def get_days_of_month(year, month):
+def get_days_of_month(year=2020, month=1):
     """获取指定月份的天数 (get days of a month)
         >>> get_days_of_month(2000, 2)
         29
         >>> get_days_of_month(2001, 2)
         28
         >>> get_days_of_month(2002, 1)
         31
@@ -321,43 +349,15 @@
     if 2 == month:
         if is_leap_year(year):
             d = 29
         else:
             d = 28
     else:
         d = days[month-1]
-    return d;
-
-class Timer:
-
-    def __init__(self, name = "[unknown]"):
-        self.name = name
-
-    def start(self):
-        self.start_time = time.time()
-
-    def stop(self):
-        self.stop_time = time.time()
-
-    def __enter__(self):
-        self.start()
-        return self
-
-    def __exit__(self, type, value, traceback):
-        import xutils
-        self.stop()
-        xutils.log("%s cost time: %s" % (self.name, self.cost()))
-
-
-    def cost(self):
-        return "%s ms" % int((self.stop_time - self.start_time) * 1000)
-
-    def cost_millis(self):
-        return int((self.stop_time - self.start_time) * 1000)
-
+    return d
 
 def match_time(year = None, month = None, day = None, wday = None, tm = None):
     if tm is None:
         tm = time.localtime()
     if year is not None and year != tm.tm_year:
         return False
     if month is not None and month != tm.tm_mon:
```

### Comparing `xnote-web-0.0.9/xutils/db/binlog.py` & `xnote-web-0.1.0/xutils/db/binlog.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_base.py` & `xnote-web-0.1.0/xutils/db/dbutil_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,14 +537,22 @@
         result = convert_bytes_to_object(value)
         if result is None:
             return default_value
         return result
     except KeyError:
         return default_value
     
+def db_get_object(key, default_value=None):
+    value = db_get(key)
+    if value is None:
+        return value
+    assert isinstance(value, xutils.Storage)
+    return value
+
+    
 def db_get_str(key, default_value=None, encoding="utf-8"):
     check_leveldb()
     try:
         if key == "" or key == None:
             return None
         
         if not isinstance(key, str):
```

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_cache.py` & `xnote-web-0.1.0/xutils/db/dbutil_cache.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_deque.py` & `xnote-web-0.1.0/xutils/db/dbutil_deque.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_hash.py` & `xnote-web-0.1.0/xutils/db/dbutil_hash.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding:utf-8 -*-
 # @author xupingmao
 # @since 2021/12/04 15:35:23
 # @modified 2022/04/05 21:15:18
 # @filename dbutil_hash.py
 
 from xutils import Storage
+from xutils import textutil
 from xutils.db import dbutil_base
 from xutils.db.dbutil_base import (
     db_get, db_put, db_delete, 
     check_table_name, 
     get_table_info, TableInfo, 
     count_table, prefix_iter
 )
@@ -150,7 +151,86 @@
         if len(records) > 0:
             return records[0]
         else:
             return None, None
 
 class LdbHashTable(KvHashTable):
     pass
+
+
+class LargeKeyHashTable:
+    """针对大key优化的hashtable,使用md5哈希后的值作为数据库的key"""
+    
+    def __init__(self, table_name=""):
+        check_table_name(table_name)
+        self.table_name = table_name
+        self.prefix = table_name + ":"
+
+    def build_key(self, key):
+        return self.prefix + textutil.md5_hex(key)
+    
+    def _check_key(self, key):
+        if not isinstance(key, str):
+            raise Exception("KvHashTableV2_param_error: expect str key")
+
+    def _check_value(self, value):
+        pass
+
+    def get(self, key, default_value = None):
+        """通过key来查询value，这个key是hash的key，不是ldb的key
+        @param {string} key hash的key
+        @param {object} default_value 如果值不存在，返回默认值
+        """
+        row_key = self.build_key(key)
+        item_dict = db_get(row_key)
+        if item_dict == None:
+            return default_value
+        assert isinstance(item_dict, dict)
+        return item_dict.get(key, default_value)
+    
+    def get_row_dict(self, row_key=""):
+        item_dict = db_get(row_key)
+        if item_dict == None:
+            return None
+        assert isinstance(item_dict, dict)
+        return item_dict
+
+    def put(self, key, value, batch = None):
+        """通过key来设置value，这个key是hash的key，不是ldb的key
+        @param {string} key hash的key
+        @param {object} value hash的value
+        """
+        self._check_key(key)
+        self._check_value(value)
+
+        row_key = self.build_key(key)
+        item_dict = self.get_row_dict(row_key)
+        if item_dict == None:
+            item_dict = {}
+        item_dict[key] = value
+
+        if batch != None:
+            batch.put(row_key, item_dict)
+        else:
+            db_put(row_key, item_dict)
+
+
+    def delete(self, key, batch = None):
+        row_key = self.build_key(key)
+        item_dict = self.get_row_dict(row_key)
+        if item_dict == None:
+            return
+        if len(item_dict) == 0:
+            return
+        
+        item_dict.pop(key, None)
+
+        if len(item_dict) > 0:
+            if batch != None:
+                batch.put(row_key, item_dict)
+            else:
+                db_put(row_key, item_dict)
+        else:
+            if batch != None:
+                batch.delete(row_key)
+            else:
+                db_delete(row_key)
```

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_helper.py` & `xnote-web-0.1.0/xutils/db/dbutil_helper.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_id_gen.py` & `xnote-web-0.1.0/xutils/db/dbutil_id_gen.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_set.py` & `xnote-web-0.1.0/xutils/db/dbutil_set.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_sortedset.py` & `xnote-web-0.1.0/xutils/db/dbutil_sortedset.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_table.py` & `xnote-web-0.1.0/xutils/db/dbutil_table.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_table_index.py` & `xnote-web-0.1.0/xutils/db/dbutil_table_index.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/dbutil_table_v2.py` & `xnote-web-0.1.0/xutils/db/dbutil_table_v2.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_leveldb.py` & `xnote-web-0.1.0/xutils/db/driver_leveldb.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_leveldbpy.py` & `xnote-web-0.1.0/xutils/db/driver_leveldbpy.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_lmdb.py` & `xnote-web-0.1.0/xutils/db/driver_lmdb.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_mysql.py` & `xnote-web-0.1.0/xutils/db/driver_mysql.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_mysql_enhance.py` & `xnote-web-0.1.0/xutils/db/driver_mysql_enhance.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_sqlite.py` & `xnote-web-0.1.0/xutils/db/driver_sqlite.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/driver_ssdb.py` & `xnote-web-0.1.0/xutils/db/driver_ssdb.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/encode.py` & `xnote-web-0.1.0/xutils/db/encode.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/filters.py` & `xnote-web-0.1.0/xutils/db/filters.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/lock.py` & `xnote-web-0.1.0/xutils/db/lock.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/db/shard.py` & `xnote-web-0.1.0/xutils/db/shard.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/dbutil.py` & `xnote-web-0.1.0/xutils/dbutil.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/exeutil.py` & `xnote-web-0.1.0/xutils/exeutil.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/fsutil.py` & `xnote-web-0.1.0/xutils/fsutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     import ctypes
 except ImportError:
     ctypes = None
 
 from xutils import six
 from xutils.imports import *
 from xutils.base import Storage
+from xutils import textutil
 from fnmatch import fnmatch
 from xutils.six.moves.configparser import ConfigParser
 from xutils import logutil
 
 # mbcs泛指通过2字节来编码的字符编码
 # https://zhuanlan.zhihu.com/p/453675608
 # GBK兼容GB2312
@@ -37,25 +38,27 @@
 CONFIG_FILE_MAX_SIZE = 1024 * 1024
 
 # Windows的文件名最大长度
 WIN_MAXPATH = 260
 
 
 class FileUtilConfig:
-    use_urlencode = False
+    """文件util配置"""
+    encode_name = False
     data_dir = ""
+    tmp_dir = "/tmp"
 
 def get_real_path(path):
     """获取真实的path信息，如果配置了urlencode，强制进行urlencode，否则先按原路径检查，如果文件不存在，再进行urlencode
     之所以要这样做，主要是为了兼容从不支持unicode文件名的服务器同步到本地的文件"""
     assert isinstance(path, str)
     if path == "":
         return path
 
-    if FileUtilConfig.use_urlencode:
+    if FileUtilConfig.encode_name:
         return get_real_path_encode_first(path)
 
     # 如果文件存在,直接返回
     if os.path.exists(path):
         return path
 
     # 兼容urlencode编码
@@ -199,15 +202,15 @@
     if size < 0 and format:
         return "-"
     if format:
         return format_size(size)
     return size
 
 def list_file_objects(dirname, webpath=False):
-    import xconfig
+    from xnote.core import xconfig
     filelist = [
         FileItem(os.path.join(dirname, child)) for child in os.listdir(dirname)
     ]
     if webpath:
         for item in filelist:
             item.path = get_relative_path(item.path, xconfig.UPLOAD_DIR)
     filelist.sort()
@@ -242,65 +245,72 @@
     return file_objects
 
 
 def splitpath(path):
     return split_path_to_objects(path)
 
 
-def decode_name(name):
+def decode_name(name: str):
     dirname = os.path.dirname(name)
     basename = os.path.basename(name)
     namepart, ext = os.path.splitext(basename)
     if ext in (".xenc", ".x0"):
         try:
+            pad_size = 4 - len(namepart)%4
+            namepart += '=' * pad_size
             basename = base64.urlsafe_b64decode(
                 namepart.encode("utf-8")).decode("utf-8")
             return os.path.join(dirname, basename)
         except:
-            return name
-    return name
+            pass
+    return xutils.unquote(name)
 
 
-def encode_name(name):
+def encode_name(name: str):
     namepart, ext = os.path.splitext(name)
     if ext in (".xenc", ".x0"):
         return name
-    return base64.urlsafe_b64encode(
-        name.encode("utf-8")).decode("utf-8") + ".x0"
+    result = base64.urlsafe_b64encode(name.encode("utf-8")).decode("utf-8")
+    result = result.strip("=")
+    return result + ".x0"
 
 
 def path_equals(source, target):
     """判断两个路径是否相同
 
     >>> path_equals('/home/a.txt', '/home/ccc/../a.txt')
     True
 
     """
     return os.path.abspath(source) == os.path.abspath(target)
 
 
-def tmp_path(fname="", prefix="", ext=""):
+def get_tmp_path(fname="", prefix="", ext=""):
     """生成临时文件路径
     TODO 多线程情况下加锁
     """
-    import xconfig
-    if fname != None:
-        return os.path.join(xconfig.TMP_DIR, fname)
+    if ext != "":
+        if ext[0] != ".":
+            raise Exception("expect ext like .xx")
+
+    if fname != "" and fname != None:
+        return os.path.join(FileUtilConfig.tmp_dir, fname)
 
     retry_times = 10
-    name = prefix + time.strftime("%Y_%m_%d_%H%M%S")
-    base_path = os.path.join(xconfig.TMP_DIR, name)
+    name = prefix + time.strftime("%Y_%m_%d_") + textutil.create_uuid()
+    base_path = os.path.join(FileUtilConfig.tmp_dir, name)
     path = base_path + ext
 
     for i in range(1, retry_times + 1):
         if not os.path.exists(path):
             return path
         path = "%s_%s" % (base_path, i) + ext
     raise Exception("创建临时文件失败, 请手动重试")
 
+tmp_path = get_tmp_path
 
 def data_path(fname):
     """获取data目录文件路径"""
     return os.path.join(FileUtilConfig.data_dir, fname)
 
 
 ### 文件操作部分
@@ -580,15 +590,17 @@
     def __init__(self,
                  path,
                  parent=None,
                  merge=False,
                  encode_path=True,
                  name=None):
         self.path = path
-        self.name = fixed_basename(path)
+        realname = fixed_basename(path)
+        self.name = realname
+        self.realname = realname
 
         self.size = '-'
         self.cdate = '-'
         self.icon = "fa-file-o"
         _, self.ext = os.path.splitext(path)
         self.ext = self.ext.lower()
 
@@ -845,8 +857,19 @@
                                                    ctypes.pointer(free_bytes))
         return free_bytes.value
     else:
         st = os.statvfs(folder)
         return st.f_bavail * st.f_frsize
 
 def is_same_file(path1, path2):
-    return os.path.abspath(path1) == os.path.abspath(path2)
+    return os.path.abspath(path1) == os.path.abspath(path2)
+
+
+def get_safe_file_name(filename: str):
+    """处理文件名中的特殊符号"""
+    for c in " @$:#\\|=&?":
+        filename = filename.replace(c, "_")
+    
+    quote_name = xutils.quote_unicode(filename)
+    if quote_name != filename:
+        return encode_name(filename)
+    return filename
```

### Comparing `xnote-web-0.0.9/xutils/func_util.py` & `xnote-web-0.1.0/xutils/func_util.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/functions.py` & `xnote-web-0.1.0/xutils/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding:utf-8 -*-
 # @author xupingmao <578749341@qq.com>
 # @since 2018/05/25 10:52:11
 # @modified 2022/04/11 23:05:34
+import time
 from collections import deque
 from xutils.dateutil import format_time
 
 class Counter:
 
     def __init__(self, sorted=False):
         self.dict = {}
@@ -194,15 +195,15 @@
 class History(MemTable):
 
     def __init__(self, type, maxsize):
         self.type = type
         MemTable.__init__(self, maxsize=maxsize)
 
     def add(self, key, rt=-1):
-        import xauth
+        from xnote.core import xauth
         self._insert(type = self.type,
             ctime = format_time(), 
             user = xauth.get_current_name(), 
             key = key, 
             rt = rt)
 
     def new_value(self, name, extinfo):
@@ -219,26 +220,14 @@
         if found == None:
             found = self.new_value(name, extinfo)
         found.count += 1
         found.time = format_time()
         self.data.append(found)
 
 
-class SortedSet:
-    """仿照redis的SortedSet，但是是基于内存的，不会持久化"""
-
-    def __init__(self):
-        raise NotImplementedError()
-    
-    def zadd(self, member, score):
-        pass
-
-    def zrange(self, start_index, stop_index):
-        pass
-
 def listremove(list: list, obj) -> None:
     return remove_list_item(list, obj)
 
 def remove_list_item(list: list, obj):
     """删除列表中的所有元素,list自带的remove方法只删除一个，而且如果不包含目标对象会抛出异常"""
     if list is None:
         return
@@ -321,10 +310,37 @@
     False
     """
     for item in iter_obj:
         if func(item):
             return True
     return False
 
+class Timer:
+    """计时器"""
+    def __init__(self, name = "[unknown]"):
+        self.name = name
+
+    def start(self):
+        self.start_time = time.time()
+
+    def stop(self):
+        self.stop_time = time.time()
+
+    def __enter__(self):
+        self.start()
+        return self
+
+    def __exit__(self, type, value, traceback):
+        import xutils
+        self.stop()
+        xutils.log("%s cost time: %s" % (self.name, self.cost()))
+
+
+    def cost(self):
+        return "%s ms" % int((self.stop_time - self.start_time) * 1000)
+
+    def cost_millis(self):
+        return int((self.stop_time - self.start_time) * 1000)
+
 if __name__ == '__main__':
     import doctest
     doctest.testmod()
```

### Comparing `xnote-web-0.0.9/xutils/htmlutil.py` & `xnote-web-0.1.0/xutils/htmlutil.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/imports.py` & `xnote-web-0.1.0/xutils/imports.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-# -*- coding:utf-8 -*-
-# 专门用来import各种依赖
-# @author xupingmao <578749341@qq.com>
-# @since 2018/06/07 22:12:44
-# @modified 2022/04/16 09:05:41
-from __future__ import print_function
-
-from . import six
-from .six.moves.configparser import ConfigParser
-from .six.moves.urllib.parse import quote, unquote
-from .six.moves.urllib.request import urlopen
-from .six import StringIO
-
-import sys
-import os
-import traceback
-import inspect
-import json
-import base64
-import time
-import platform
-import re
-import gc
-import shutil
-import profile as pf
-import subprocess
-import pickle
-import hashlib
-import codecs
-from xutils.base import Storage
-from collections import deque
-from fnmatch import fnmatch
-from xutils.tornado.escape import xhtml_escape
-
-import web
-from web.utils import safestr, safeunicode
-
-try:
-    import sqlite3
-except ImportError:
-    sqlite3 = None # sqlite3 is not available, may be jython
-
-try:
-    import bs4
-except ImportError:
-    bs4 = None
-
-PY2 = sys.version_info[0] == 2
-
-if PY2:
-    from Queue import Queue, PriorityQueue
-    # from commands import getstatusoutput
-
-    def u(s, encoding="utf-8"):
-        if isinstance(s, str):
-            return s.decode(encoding)
-        elif isinstance(s, unicode):
-            return s
-        elif isinstance(s, Exception):
-            return u(s.message)
-        return str(s)
-
-    def listdir(dirname):
-        names = list(os.listdir(dirname))
-        encoding = sys.getfilesystemencoding()
-        return [newname.decode(encoding) for newname in names]
-
-    def is_str(s):
-        return isinstance(s, (str, unicode))
-else:
-    # Py3 and later
-    from subprocess import getstatusoutput
-    from queue import Queue, PriorityQueue
-
-    u = str
-    listdir = os.listdir
-
-    def is_str(s):
-        return isinstance(s, str)
-
-# 关于Py2的getstatusoutput，实际上是对os.popen的封装
-# 而Py3中的getstatusoutput则是对subprocess.Popen的封装
-# Py2的getstatusoutput, 注意原来的windows下不能正确运行，但是下面改进版的可以运行
-
-if PY2:
-    def getstatusoutput(cmd):
-        """Return (status, output) of executing cmd in a shell."""
-        import os
-        # old
-        # pipe = os.popen('{ ' + cmd + '; } 2>&1', 'r')
-        # 这样修改有一个缺点就是执行多个命令的时候只能获取最后一个命令的输出
-        pipe = os.popen(cmd + ' 2>&1', 'r')
-        text = pipe.read()
-        sts = pipe.close()
-        if sts is None: sts = 0
-        if text[-1:] == '\n': text = text[:-1]
-        return sts, text
-
-
-def quote_unicode(url):
-    # python的quote会quote大部分字符，包括ASCII符号
-    # JavaScript的encodeURI
-    # encodeURI 会替换所有的字符，但不包括以下字符，即使它们具有适当的UTF-8转义序列：
-    #    类型  包含
-    #    保留字符    ; , / ? : @ & = + $
-    #    非转义的字符  字母 数字 - _ . ! ~ * ' ( )
-    #    数字符号    #
-    # 根据最新的RFC3986，方括号[]也是非转义字符
-    # JavaScript的encodeURIComponent会编码+,&,=等字符
-    def quote_char_by_code(c):
-        # ASCII 范围 [0-127]
-        # 32=空格
-        if c == 32: 
-            return '%20'
-        if c <= 127:
-            return chr(c)
-        return '%%%02X' % c
-
-    if six.PY2:
-        bytes = url
-        return ''.join([quote_char_by_code(ord(c)) for c in bytes])
-    else:
-        bytes = url.encode("utf-8")
-        return ''.join([quote_char_by_code(c) for c in bytes])
-
-    # def urlencode(matched):
-    #     text = matched.group()
-    #     return quote(text)
-    # return re.sub(r"[\u4e00-\u9fa5]+", urlencode, url)
-
-def try_decode(bytes):
-    exc = None
-    for charset in ("utf-8", "gbk", "mbcs", "latin_1"):
-        try:
-            return codecs.decode(bytes, charset)
-        except Exception as e:
-            exc = e
-    if exc != None:
-        raise exc
-
+# -*- coding:utf-8 -*-
+# 专门用来import各种依赖
+# @author xupingmao <578749341@qq.com>
+# @since 2018/06/07 22:12:44
+# @modified 2022/04/16 09:05:41
+from __future__ import print_function
+
+from . import six
+from .six.moves.configparser import ConfigParser
+from .six.moves.urllib.parse import quote, unquote
+from .six.moves.urllib.request import urlopen
+from .six import StringIO
+
+import sys
+import os
+import traceback
+import inspect
+import json
+import base64
+import time
+import platform
+import re
+import gc
+import shutil
+import profile as pf
+import subprocess
+import pickle
+import hashlib
+import codecs
+from xutils.base import Storage
+from collections import deque
+from fnmatch import fnmatch
+from xutils.tornado.escape import xhtml_escape
+
+import web
+from web.utils import safestr, safeunicode
+
+try:
+    import sqlite3
+except ImportError:
+    sqlite3 = None # sqlite3 is not available, may be jython
+
+try:
+    import bs4
+except ImportError:
+    bs4 = None
+
+PY2 = sys.version_info[0] == 2
+
+if PY2:
+    from Queue import Queue, PriorityQueue
+    # from commands import getstatusoutput
+
+    def u(s, encoding="utf-8"):
+        if isinstance(s, str):
+            return s.decode(encoding)
+        elif isinstance(s, unicode):
+            return s
+        elif isinstance(s, Exception):
+            return u(s.message)
+        return str(s)
+
+    def listdir(dirname):
+        names = list(os.listdir(dirname))
+        encoding = sys.getfilesystemencoding()
+        return [newname.decode(encoding) for newname in names]
+
+    def is_str(s):
+        return isinstance(s, (str, unicode))
+else:
+    # Py3 and later
+    from subprocess import getstatusoutput
+    from queue import Queue, PriorityQueue
+
+    u = str
+    listdir = os.listdir
+
+    def is_str(s):
+        return isinstance(s, str)
+
+# 关于Py2的getstatusoutput，实际上是对os.popen的封装
+# 而Py3中的getstatusoutput则是对subprocess.Popen的封装
+# Py2的getstatusoutput, 注意原来的windows下不能正确运行，但是下面改进版的可以运行
+
+if PY2:
+    def getstatusoutput(cmd):
+        """Return (status, output) of executing cmd in a shell."""
+        import os
+        # old
+        # pipe = os.popen('{ ' + cmd + '; } 2>&1', 'r')
+        # 这样修改有一个缺点就是执行多个命令的时候只能获取最后一个命令的输出
+        pipe = os.popen(cmd + ' 2>&1', 'r')
+        text = pipe.read()
+        sts = pipe.close()
+        if sts is None: sts = 0
+        if text[-1:] == '\n': text = text[:-1]
+        return sts, text
+
+
+def quote_unicode(url):
+    # python的quote会quote大部分字符，包括ASCII符号
+    # JavaScript的encodeURI
+    # encodeURI 会替换所有的字符，但不包括以下字符，即使它们具有适当的UTF-8转义序列：
+    #    类型  包含
+    #    保留字符    ; , / ? : @ & = + $
+    #    非转义的字符  字母 数字 - _ . ! ~ * ' ( )
+    #    数字符号    #
+    # 根据最新的RFC3986，方括号[]也是非转义字符
+    # JavaScript的encodeURIComponent会编码+,&,=等字符
+    def quote_char_by_code(c):
+        # ASCII 范围 [0-127]
+        # 32=空格
+        if c == 32: 
+            return '%20'
+        if c <= 127:
+            return chr(c)
+        return '%%%02X' % c
+
+    if six.PY2:
+        bytes = url
+        return ''.join([quote_char_by_code(ord(c)) for c in bytes])
+    else:
+        bytes = url.encode("utf-8")
+        return ''.join([quote_char_by_code(c) for c in bytes])
+
+    # def urlencode(matched):
+    #     text = matched.group()
+    #     return quote(text)
+    # return re.sub(r"[\u4e00-\u9fa5]+", urlencode, url)
+
+def try_decode(bytes):
+    exc = None
+    for charset in ("utf-8", "gbk", "mbcs", "latin_1"):
+        try:
+            return codecs.decode(bytes, charset)
+        except Exception as e:
+            exc = e
+    if exc != None:
+        raise exc
+
```

### Comparing `xnote-web-0.0.9/xutils/interfaces.py` & `xnote-web-0.1.0/xutils/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,28 +145,38 @@
                 value_int += increment
 
             value_bytes = str(value_int).encode("utf-8")
             self.Put(key, value_bytes)
             return value_int
 
 
-class DBLockInterface:
-    """基于数据库的锁的接口"""
+class LockInterface:
+    """分布式锁接口"""
 
-    def Acquire(self, resource_id, timeout):
-        """返回token
-        @return {str} token
+    def acquire(self, resource_key="", expires=60*1000):
+        """返回锁对象
         """
-        raise NotImplementedError("Acquire")
+        raise NotImplementedError("acquire")
     
-    def Release(self, resource_id, token):
-        raise NotImplementedError("Release")
+    def release(self, resource_id, token):
+        raise NotImplementedError("release")
     
-    def Refresh(self, resource_id, token, refresh_time):
-        raise NotImplementedError("Refresh")
+    def refresh(self, resource_id, token, refresh_time):
+        raise NotImplementedError("refresh")
+
+class FileLockInterface:
+    """文件锁接口"""
+    def lock(self):
+        return True
+
+    def try_lock(self):
+        return True
+    
+    def unlock(self):
+        pass
 
 class RecordInterface:
     """数据库记录的接口
     一般情况下推荐继承 xutils.Storage
     继承自Storage无法调用类的方法, 这种情况下可以继承当前的接口
     """
```

### Comparing `xnote-web-0.0.9/xutils/jsonutil.py` & `xnote-web-0.1.0/xutils/jsonutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : kylen66
 @email        : kylen66
 @Date         : 2023-06-27 23:19:07
 @LastEditors  : xupingmao
-@LastEditTime : 2023-06-29 23:19:54
+@LastEditTime : 2024-05-02 00:02:36
 @FilePath     : /xnote/xutils/jsonutil.py
 @Description  : 描述
 """
 
 import json
 import uuid
 from datetime import datetime
@@ -16,13 +16,19 @@
 
 class MyEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, datetime):
             return obj.strftime('%Y-%m-%d %H:%M:%S')
         elif isinstance(obj, date):
             return obj.strftime('%Y-%m-%d')
-        elif isinstance(obj, type(bytes)):
+        elif isinstance(obj, bytes):
             return str(obj, encoding='utf-8')
         elif isinstance(obj,uuid.UUID):
             return obj.hex
         else:
             return json.JSONEncoder.default(self, obj)
+
+
+def parse_json_to_dict(text=""):
+    result = json.loads(text)
+    assert isinstance(result, dict)
+    return result
```

### Comparing `xnote-web-0.0.9/xutils/lockutil.py` & `xnote-web-0.1.0/xutils/lockutil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding:utf-8 -*-
 # @author xupingmao
 # @since 2021/12/04 15:35:23
 # @modified 2022/01/23 23:57:56
 # @filename lockutil.py
 import os
 import xutils
+from xutils.interfaces import FileLockInterface
 
 try:
 	import fcntl
 except ImportError:
 	fcntl = None
 
-class UnixLock:
+class UnixLock(FileLockInterface):
 	"""Unix环境的锁实现"""
 
 	def __init__(self, fpath):
 		self.fpath = fpath
 		self.fp = open(fpath, "w+")
 		self.got_lock = False
 
@@ -40,24 +41,24 @@
 		if self.got_lock:
 			fcntl.flock(self.fp, fcntl.LOCK_UN)
 			# 不需要重置为空
 			self.fp.close()
 			self.got_lock = False
 		return True
 
-class WinLock:
+class WinLock(FileLockInterface):
 
 	def __init__(self, fpath):
 		self.fpath = fpath
 
 	def try_lock(self):
 		return True
 
 	def unlock(self):
-		pass
+		return
 
 class WinLockOld:
 	"""Windows环境的锁实现"""
 
 	def __init__(self, fpath):
 		self.fpath = fpath
 		self.got_lock = False
@@ -91,23 +92,25 @@
 			self.got_lock = False
 
 		if self.fp != None:
 			self.fp.close()
 			self.fp = None
 
 
-class FileLock:
+class FileLockAdapter(FileLockInterface):
 	"""文件锁，注意目前只支持posix系统"""
 
 	def __init__(self, fpath):
 		if fcntl != None:
 			self.impl = UnixLock(fpath)
 		else:
 			self.impl = WinLock(fpath)
 
-	def acquire(self):
+	def try_lock(self):
 		return self.impl.try_lock()
 
-	def release(self):
+	def unlock(self):
 		return self.impl.unlock()
 
 
+class DummyLock(FileLockInterface):
+	pass
```

### Comparing `xnote-web-0.0.9/xutils/logutil.py` & `xnote-web-0.1.0/xutils/logutil.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/mem_util.py` & `xnote-web-0.1.0/xutils/mem_util.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/netutil.py` & `xnote-web-0.1.0/xutils/netutil.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/six.py` & `xnote-web-0.1.0/xutils/six.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/sqldb/table_manager.py` & `xnote-web-0.1.0/xutils/sqldb/table_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2023-04-28 20:36:45
 @LastEditors  : xupingmao
-@LastEditTime : 2023-10-14 08:42:11
+@LastEditTime : 2024-04-05 11:58:25
 @FilePath     : /xnote/xutils/sqldb/table_manager.py
-@Description  : 描述
+@Description  : SQL表结构管理
 """
 
 import logging
 import xutils
 import web.db
+from .table_config import TableConfig
 
 empty_db = web.db.DB(None, {})
 
 class ColumnInfo:
 
     def __init__(self):
         self.name = ""
@@ -193,14 +194,16 @@
                     self.tablename, index_name, colname_str)
 
         if self.is_index_exists(index_name):
             logging.info("index %s already exists", index_name)
             return
         
         logging.info("%s", sql)
+        if not TableConfig.enable_auto_ddl:
+            raise Exception("db_auto_ddl is disabled")
         self.execute(sql)
         
     
     def is_index_exists(self, index_name=""):
         assert len(self.mysql_database) > 0
         sql = "SELECT COUNT(*) as amount FROM information_schema.statistics WHERE table_schema=$database AND table_name = $table_name AND index_name = $index_name"
         first = self.db.query(sql, vars=dict(database=self.mysql_database, table_name=self.tablename, index_name=index_name)).first()
@@ -361,14 +364,21 @@
                 raise Exception("table already defined: %s" % tablename)
         
         if not is_backup:
             self.table_dict[tablename] = self.table_info
     
     def add_column(self, colname, coltype,
                    default_value=None, not_null=True, comment=""):
+        coltype_lower = coltype.lower()
+
+        if "varchar" in coltype_lower:
+            assert default_value != None, f"varchar column {colname} default value cant be NULL"
+        if coltype_lower in ("int", "tinyint", "bigint"):
+            assert default_value != None, f"{coltype} column {colname} default value cant be NULL"
+        
         self.table_info.add_column(colname, coltype, default_value, not_null)
         self.manager.add_column(colname, coltype, default_value, not_null, comment=comment)
     
     def drop_column(self, colname, coltype,
                    default_value=None, not_null=True):
         pass
```

### Comparing `xnote-web-0.0.9/xutils/sqldb/table_proxy.py` & `xnote-web-0.1.0/xutils/sqldb/table_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2023-04-28 21:09:40
 @LastEditors  : xupingmao
-@LastEditTime : 2024-02-14 18:14:04
+@LastEditTime : 2024-04-05 12:47:10
 @FilePath     : /xnote/xutils/sqldb/table_proxy.py
-@Description  : 描述
+@Description  : SQL表查询代理
 """
 import time
 import xutils
 import web.db
 from web.db import SQLQuery, sqlparam
 from . import table_manager
+from .table_config import TableConfig
 from xutils.interfaces import ProfileLog, ProfileLogger, SQLDBInterface
 from xutils.db.binlog import BinLog, BinLogOpType
 
 
-class TableConfig:
-
-    log_profile = False
-    enable_binlog = False
-    
-    _disable_profile_tables = set()
-    _disable_binlog_tables = set()
-    
-    @classmethod
-    def disable_profile(cls, table_name=""):
-        cls._disable_profile_tables.add(table_name)
-        
-    @classmethod
-    def disable_binlog(cls, table_name=""):
-        cls._disable_binlog_tables.add(table_name)
-    
 
 class TableProxy(SQLDBInterface):
     """基于web.db的装饰器
     SqliteDB是全局唯一的, 它的底层使用了连接池技术, 每个线程都有独立的sqlite连接
     """
     log_profile = False
     enable_binlog = False
```

### Comparing `xnote-web-0.0.9/xutils/text_parser.py` & `xnote-web-0.1.0/xutils/text_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2021-01-10 14:36:09
 @LastEditors  : xupingmao
-@LastEditTime : 2023-08-19 11:48:48
+@LastEditTime : 2024-05-03 12:05:40
 @FilePath     : /xnote/xutils/text_parser.py
 @Description  : 描述
 """
 
 """标记文本解析
 
 类
@@ -36,15 +36,17 @@
                 print("exception occurs", prefix, args, kw)
                 raise e
         return handle
     return deco
 
 def is_img_file(filename):
     """根据文件后缀判断是否是图片"""
-    name, ext = os.path.splitext(filename)
+    from xutils import fsutil
+    realname = fsutil.decode_name(filename)
+    name, ext = os.path.splitext(realname)
     return ext.lower() in IMG_EXT_SET
 
 def set_img_file_ext(img_set):
     global IMG_EXT_SET
     IMG_EXT_SET = img_set
 
 def escape_html(text):
@@ -463,25 +465,26 @@
             if len(hrefs) > 1:
                 token = '<div class="msg-img-box multi"><img class="msg-img x-photo" alt="%s" src="%s"></div>' % (href, href)
             else:
                 token = '<div class="msg-img-box"><img class="msg-img x-photo" alt="%s" src="%s"></div>' % (href, href)
             self.tokens.append(token)
 
     def mark_file(self):
+        from xutils import fsutil
         self.profile("mark_file")
 
         self.save_str_token()
         href = self.read_before_blank()
         href = href[7:]
         if is_img_file(href):
             self.handle_img_list(href)
         else:
             name = href[href.rfind("/")+1:]
             # 尝试urldecode名称
-            name = unquote(name)
+            name = fsutil.decode_name(name)
             token = '<a href="%s">%s</a>' % (href, name)
             self.tokens.append(token)
 
     def parse(self, text):
         self.init(text)
         self.init_ext(text)
```

### Comparing `xnote-web-0.0.9/xutils/text_parser_properties.py` & `xnote-web-0.1.0/xutils/text_parser_properties.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/textutil.py` & `xnote-web-0.1.0/xutils/textutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @modified 2022/04/16 18:18:24
 
 """
 @Author       : xupingmao
 @email        : 578749341@qq.com
 @Date         : 2022-04-17 17:04:15
 @LastEditors  : xupingmao
-@LastEditTime : 2023-11-18 22:54:24
+@LastEditTime : 2024-04-04 11:39:23
 @FilePath     : /xnote/xutils/textutil.py
 @Description  : 文本处理工具
 """
 
 import re
 import random
 import json
@@ -759,17 +759,21 @@
     # quoted = quoted.replace("&", "%26")
     # quoted = quoted.replace(" ", "%20")
     # quoted = quoted.replace("=", "%3D")
     # quoted = quoted.replace("+", "%2B")
     # quoted = quoted.replace("#", "%23")
     return quote(text)
 
-def md5_hex(string):
+def md5_hex(string=""):
+    """生成MD5哈希校验码, 长度是32"""
     return hashlib.md5(string.encode("utf-8")).hexdigest()
 
+def sha1_hex(string=""):
+    """生产SHA-1哈希校验码, 长度是40"""
+    return hashlib.sha1(string.encode("utf-8")).hexdigest()
         
 class Properties(object): 
     
     """Properties 文件处理器"""
     def __init__(self, fileName, ordered = True): 
         self.ordered = ordered
         self.fileName = fileName
```

### Comparing `xnote-web-0.0.9/xutils/textutil_url.py` & `xnote-web-0.1.0/xutils/textutil_url.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/tokenizer.py` & `xnote-web-0.1.0/xutils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/tornado/escape.py` & `xnote-web-0.1.0/xutils/tornado/escape.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/tornado/log.py` & `xnote-web-0.1.0/xutils/tornado/log.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/tornado/template.py` & `xnote-web-0.1.0/xutils/tornado/template.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/tornado/util.py` & `xnote-web-0.1.0/xutils/tornado/util.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/webutil.py` & `xnote-web-0.1.0/xutils/webutil.py`

 * *Files identical despite different names*

### Comparing `xnote-web-0.0.9/xutils/ziputil.py` & `xnote-web-0.1.0/xutils/ziputil.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 压缩文件，对非ASCII码进行urlencode处理
 """
 import zipfile
 import os
 import sys
 
 def quote_unicode(url):
-    import xconfig
+    from xnote.core import xconfig
     if not xconfig.USE_URLENCODE:
         return url
     def quote_char(c):
         # ASCII 范围 [0-127]
         if c <= 127:
             return chr(c)
         return '%%%02X' % c
```

