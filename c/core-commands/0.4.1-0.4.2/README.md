# Comparing `tmp/core_commands-0.4.1.tar.gz` & `tmp/core_commands-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_commands-0.4.1.tar", max compression
+gzip compressed data, was "core_commands-0.4.2.tar", max compression
```

## Comparing `core_commands-0.4.1.tar` & `core_commands-0.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       20 2023-11-24 10:50:39.212993 core_commands-0.4.1/core_commands/__init__.py
--rw-r--r--   0        0        0       18 2024-04-27 16:09:33.472746 core_commands-0.4.1/core_commands/cmd/__init__.py
--rw-r--r--   0        0        0      423 2024-04-14 12:32:15.243453 core_commands-0.4.1/core_commands/cmd/__pycache__/command_cmd.cpython-311.pyc
--rw-r--r--   0        0        0      339 2024-04-26 09:35:36.626791 core_commands-0.4.1/core_commands/cmd/attrib.py
--rw-r--r--   0        0        0      620 2023-11-26 14:53:35.801583 core_commands-0.4.1/core_commands/cmd/call.py
--rw-r--r--   0        0        0      192 2024-04-27 12:30:59.113021 core_commands-0.4.1/core_commands/cmd/cd.py
--rw-r--r--   0        0        0      162 2023-11-26 13:34:37.662604 core_commands-0.4.1/core_commands/cmd/chdir.py
--rw-r--r--   0        0        0       74 2023-11-26 13:40:27.657852 core_commands-0.4.1/core_commands/cmd/cls.py
--rw-r--r--   0        0        0      844 2024-04-27 16:06:39.947709 core_commands-0.4.1/core_commands/cmd/cmd.py
--rw-r--r--   0        0        0      682 2024-04-27 07:51:44.074159 core_commands-0.4.1/core_commands/cmd/color.py
--rw-r--r--   0        0        0      170 2024-04-26 23:21:15.988546 core_commands-0.4.1/core_commands/cmd/command_cmd.py
--rw-r--r--   0        0        0      236 2023-11-26 14:35:07.010104 core_commands-0.4.1/core_commands/cmd/copy.py
--rw-r--r--   0        0        0      305 2023-11-26 15:00:26.545414 core_commands-0.4.1/core_commands/cmd/curl.py
--rw-r--r--   0        0        0      298 2024-04-26 23:42:17.496887 core_commands-0.4.1/core_commands/cmd/date.py
--rw-r--r--   0        0        0      515 2024-04-26 23:50:17.588678 core_commands-0.4.1/core_commands/cmd/DEL.py
--rw-r--r--   0        0        0      172 2023-11-26 13:19:57.348400 core_commands-0.4.1/core_commands/cmd/dir.py
--rw-r--r--   0        0        0      295 2024-05-03 12:33:29.666710 core_commands-0.4.1/core_commands/cmd/echo.py
--rw-r--r--   0        0        0      183 2024-04-27 00:01:46.298923 core_commands-0.4.1/core_commands/cmd/hostname.py
--rw-r--r--   0        0        0      434 2023-11-26 13:45:26.083270 core_commands-0.4.1/core_commands/cmd/mkdir.py
--rw-r--r--   0        0        0       81 2024-04-26 23:34:26.835037 core_commands-0.4.1/core_commands/cmd/ver.py
--rw-r--r--   0        0        0      158 2024-04-26 23:57:32.523142 core_commands-0.4.1/core_commands/cmd/verify.py
--rw-r--r--   0        0        0      107 2024-04-26 10:41:32.743320 core_commands-0.4.1/core_commands/cmd/w32tm.py
--rw-r--r--   0        0        0       98 2024-04-26 11:00:05.864162 core_commands-0.4.1/core_commands/cmd/waitfor.py
--rw-r--r--   0        0        0      111 2024-04-26 23:26:24.217463 core_commands-0.4.1/core_commands/cmd/wbadmin.py
--rw-r--r--   0        0        0      149 2024-04-26 23:25:22.564346 core_commands-0.4.1/core_commands/cmd/wecutil.py
--rw-r--r--   0        0        0      113 2024-04-26 23:22:14.346255 core_commands-0.4.1/core_commands/cmd/wevtutil.py
--rw-r--r--   0        0        0      241 2024-04-26 10:02:55.946106 core_commands-0.4.1/core_commands/cmd/where.py
--rw-r--r--   0        0        0      217 2024-04-26 09:54:04.254430 core_commands-0.4.1/core_commands/cmd/whoami.py
--rw-r--r--   0        0        0      117 2024-04-26 23:27:44.659390 core_commands-0.4.1/core_commands/cmd/windiff.py
--rw-r--r--   0        0        0      198 2024-04-26 09:43:50.036526 core_commands-0.4.1/core_commands/cmd/winget.py
--rw-r--r--   0        0        0      103 2024-04-26 10:43:30.309215 core_commands-0.4.1/core_commands/cmd/wpr.py
--rw-r--r--   0        0        0      338 2024-04-26 10:40:42.176790 core_commands-0.4.1/core_commands/cmd/wt.py
--rw-r--r--   0        0        0      277 2024-04-26 23:32:19.197506 core_commands-0.4.1/core_commands/cmd/xcopy.py
--rw-r--r--   0        0        0        0 2023-08-15 15:36:53.392178 core_commands-0.4.1/core_commands/commands/winrar,py
--rw-r--r--   0        0        0      185 2024-04-26 09:24:52.311676 core_commands-0.4.1/core_commands/powershell/command_powershell.py
--rw-r--r--   0        0        0        0 2024-04-26 09:16:20.617692 core_commands-0.4.1/core_commands/powershell/powershell.py
--rw-r--r--   0        0        0      383 2024-05-03 12:34:15.340816 core_commands-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-21 14:03:17.437817 core_commands-0.4.1/README.md
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 core_commands-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-11-24 10:50:39.212993 core_commands-0.4.2/core_commands/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-27 16:09:33.472746 core_commands-0.4.2/core_commands/cmd/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-14 12:32:15.243453 core_commands-0.4.2/core_commands/cmd/__pycache__/command_cmd.cpython-311.pyc
+-rw-r--r--   0        0        0      339 2024-04-26 09:35:36.626791 core_commands-0.4.2/core_commands/cmd/attrib.py
+-rw-r--r--   0        0        0      620 2023-11-26 14:53:35.801583 core_commands-0.4.2/core_commands/cmd/call.py
+-rw-r--r--   0        0        0      192 2024-04-27 12:30:59.113021 core_commands-0.4.2/core_commands/cmd/cd.py
+-rw-r--r--   0        0        0      162 2023-11-26 13:34:37.662604 core_commands-0.4.2/core_commands/cmd/chdir.py
+-rw-r--r--   0        0        0       74 2023-11-26 13:40:27.657852 core_commands-0.4.2/core_commands/cmd/cls.py
+-rw-r--r--   0        0        0      844 2024-04-27 16:06:39.947709 core_commands-0.4.2/core_commands/cmd/cmd.py
+-rw-r--r--   0        0        0      682 2024-04-27 07:51:44.074159 core_commands-0.4.2/core_commands/cmd/color.py
+-rw-r--r--   0        0        0      170 2024-04-26 23:21:15.988546 core_commands-0.4.2/core_commands/cmd/command_cmd.py
+-rw-r--r--   0        0        0      236 2023-11-26 14:35:07.010104 core_commands-0.4.2/core_commands/cmd/copy.py
+-rw-r--r--   0        0        0      305 2023-11-26 15:00:26.545414 core_commands-0.4.2/core_commands/cmd/curl.py
+-rw-r--r--   0        0        0      298 2024-04-26 23:42:17.496887 core_commands-0.4.2/core_commands/cmd/date.py
+-rw-r--r--   0        0        0      515 2024-04-26 23:50:17.588678 core_commands-0.4.2/core_commands/cmd/DEL.py
+-rw-r--r--   0        0        0      172 2023-11-26 13:19:57.348400 core_commands-0.4.2/core_commands/cmd/dir.py
+-rw-r--r--   0        0        0      270 2024-05-03 12:38:26.310842 core_commands-0.4.2/core_commands/cmd/echo.py
+-rw-r--r--   0        0        0      183 2024-04-27 00:01:46.298923 core_commands-0.4.2/core_commands/cmd/hostname.py
+-rw-r--r--   0        0        0      434 2023-11-26 13:45:26.083270 core_commands-0.4.2/core_commands/cmd/mkdir.py
+-rw-r--r--   0        0        0       81 2024-04-26 23:34:26.835037 core_commands-0.4.2/core_commands/cmd/ver.py
+-rw-r--r--   0        0        0      158 2024-04-26 23:57:32.523142 core_commands-0.4.2/core_commands/cmd/verify.py
+-rw-r--r--   0        0        0      107 2024-04-26 10:41:32.743320 core_commands-0.4.2/core_commands/cmd/w32tm.py
+-rw-r--r--   0        0        0       98 2024-04-26 11:00:05.864162 core_commands-0.4.2/core_commands/cmd/waitfor.py
+-rw-r--r--   0        0        0      111 2024-04-26 23:26:24.217463 core_commands-0.4.2/core_commands/cmd/wbadmin.py
+-rw-r--r--   0        0        0      149 2024-04-26 23:25:22.564346 core_commands-0.4.2/core_commands/cmd/wecutil.py
+-rw-r--r--   0        0        0      113 2024-04-26 23:22:14.346255 core_commands-0.4.2/core_commands/cmd/wevtutil.py
+-rw-r--r--   0        0        0      241 2024-04-26 10:02:55.946106 core_commands-0.4.2/core_commands/cmd/where.py
+-rw-r--r--   0        0        0      217 2024-04-26 09:54:04.254430 core_commands-0.4.2/core_commands/cmd/whoami.py
+-rw-r--r--   0        0        0      117 2024-04-26 23:27:44.659390 core_commands-0.4.2/core_commands/cmd/windiff.py
+-rw-r--r--   0        0        0      198 2024-04-26 09:43:50.036526 core_commands-0.4.2/core_commands/cmd/winget.py
+-rw-r--r--   0        0        0      103 2024-04-26 10:43:30.309215 core_commands-0.4.2/core_commands/cmd/wpr.py
+-rw-r--r--   0        0        0      338 2024-04-26 10:40:42.176790 core_commands-0.4.2/core_commands/cmd/wt.py
+-rw-r--r--   0        0        0      277 2024-04-26 23:32:19.197506 core_commands-0.4.2/core_commands/cmd/xcopy.py
+-rw-r--r--   0        0        0        0 2023-08-15 15:36:53.392178 core_commands-0.4.2/core_commands/commands/winrar,py
+-rw-r--r--   0        0        0      185 2024-04-26 09:24:52.311676 core_commands-0.4.2/core_commands/powershell/command_powershell.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:16:20.617692 core_commands-0.4.2/core_commands/powershell/powershell.py
+-rw-r--r--   0        0        0      383 2024-05-03 12:41:36.855635 core_commands-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-21 14:03:17.437817 core_commands-0.4.2/README.md
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 core_commands-0.4.2/PKG-INFO
```

### Comparing `core_commands-0.4.1/core_commands/cmd/call.py` & `core_commands-0.4.2/core_commands/cmd/call.py`

 * *Files identical despite different names*

### Comparing `core_commands-0.4.1/core_commands/cmd/cmd.py` & `core_commands-0.4.2/core_commands/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `core_commands-0.4.1/core_commands/cmd/color.py` & `core_commands-0.4.2/core_commands/cmd/color.py`

 * *Files identical despite different names*

### Comparing `core_commands-0.4.1/core_commands/cmd/DEL.py` & `core_commands-0.4.2/core_commands/cmd/DEL.py`

 * *Files identical despite different names*

