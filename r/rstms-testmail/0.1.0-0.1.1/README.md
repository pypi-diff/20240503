# Comparing `tmp/rstms_testmail-0.1.0.tar.gz` & `tmp/rstms_testmail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_testmail-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_testmail-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_testmail-0.1.0.tar` & `rstms_testmail-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      381 2024-04-30 06:16:13.068440 rstms_testmail-0.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.1.0/LICENSE
--rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.1.0/Makefile
--rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.1.0/README.md
--rw-r--r--   0        0        0        6 2024-04-30 06:16:13.064440 rstms_testmail-0.1.0/VERSION
--rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.1.0/docs/Makefile
--rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.1.0/docs/cli.rst
--rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.1.0/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.1.0/docs/contributing.rst
--rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.1.0/docs/index.rst
--rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.1.0/docs/installation.rst
--rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.1.0/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.1.0/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.1.0/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.1.0/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.1.0/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.1.0/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.1.0/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.1.0/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.1.0/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.1.0/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.1.0/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.1.0/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.1.0/make/version.mk
--rw-r--r--   0        0        0     1232 2024-04-30 06:16:13.068440 rstms_testmail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.1.0/pytest.ini
--rw-r--r--   0        0        0       97 2024-04-30 06:16:12.732443 rstms_testmail-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-04-30 06:16:12.832442 rstms_testmail-0.1.0/requirements-docs.txt
--rw-r--r--   0        0        0       89 2024-04-30 06:16:12.636444 rstms_testmail-0.1.0/requirements.txt
--rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.1.0/rstms_testmail/__init__.py
--rw-r--r--   0        0        0     3576 2024-04-30 06:11:07.687811 rstms_testmail-0.1.0/rstms_testmail/cli.py
--rw-r--r--   0        0        0      957 2024-04-28 02:18:58.990987 rstms_testmail-0.1.0/rstms_testmail/counter.py
--rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.1.0/rstms_testmail/exception_handler.py
--rw-r--r--   0        0        0     2418 2024-04-28 12:23:41.455715 rstms_testmail-0.1.0/rstms_testmail/gmail.py
--rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.1.0/rstms_testmail/netstat.py
--rw-r--r--   0        0        0      594 2024-04-30 04:50:24.597373 rstms_testmail-0.1.0/rstms_testmail/sendgrid_server.py
--rw-r--r--   0        0        0      901 2024-04-30 05:56:32.621345 rstms_testmail-0.1.0/rstms_testmail/settings.py
--rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.1.0/rstms_testmail/shell.py
--rw-r--r--   0        0        0     1244 2024-04-30 05:00:13.658436 rstms_testmail-0.1.0/rstms_testmail/smtp_server.py
--rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.1.0/rstms_testmail/timer.py
--rw-r--r--   0        0        0      127 2024-04-30 06:16:13.064440 rstms_testmail-0.1.0/rstms_testmail/version.py
--rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.1.0/rstms_testmail/watcher.py
--rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2259 2024-04-28 01:57:04.271457 rstms_testmail-0.1.0/tests/test_cli.py
--rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.1.0/tests/test_counter.py
--rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.1.0/tests/test_gmail.py
--rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.1.0/tests/test_netstat.py
--rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.1.0/tests/test_sendgrid.py
--rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.1.0/tests/test_watcher.py
--rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.1.0/tox.ini
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-05-03 20:16:33.430798 rstms_testmail-0.1.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.1.1/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.1.1/Makefile
+-rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.1.1/README.md
+-rw-r--r--   0        0        0        6 2024-05-03 20:16:33.426798 rstms_testmail-0.1.1/VERSION
+-rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.1.1/docs/cli.rst
+-rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.1.1/docs/installation.rst
+-rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.1.1/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.1.1/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.1.1/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.1.1/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.1.1/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.1.1/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.1.1/make/docs.mk
+-rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.1.1/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.1.1/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.1.1/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.1.1/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.1.1/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.1.1/make/version.mk
+-rw-r--r--   0        0        0     1232 2024-05-03 20:16:33.426798 rstms_testmail-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.1.1/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-03 20:16:33.258800 rstms_testmail-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-03 20:16:33.318800 rstms_testmail-0.1.1/requirements-docs.txt
+-rw-r--r--   0        0        0       89 2024-05-03 20:16:33.198801 rstms_testmail-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.1.1/rstms_testmail/__init__.py
+-rw-r--r--   0        0        0     3594 2024-05-03 20:07:08.741073 rstms_testmail-0.1.1/rstms_testmail/cli.py
+-rw-r--r--   0        0        0      957 2024-04-28 02:18:58.990987 rstms_testmail-0.1.1/rstms_testmail/counter.py
+-rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.1.1/rstms_testmail/exception_handler.py
+-rw-r--r--   0        0        0     2418 2024-04-28 12:23:41.455715 rstms_testmail-0.1.1/rstms_testmail/gmail.py
+-rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.1.1/rstms_testmail/netstat.py
+-rw-r--r--   0        0        0      594 2024-05-03 19:33:45.846287 rstms_testmail-0.1.1/rstms_testmail/sendgrid_server.py
+-rw-r--r--   0        0        0      901 2024-04-30 05:56:32.621345 rstms_testmail-0.1.1/rstms_testmail/settings.py
+-rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.1.1/rstms_testmail/shell.py
+-rw-r--r--   0        0        0     1244 2024-04-30 05:00:13.658436 rstms_testmail-0.1.1/rstms_testmail/smtp_server.py
+-rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.1.1/rstms_testmail/timer.py
+-rw-r--r--   0        0        0      127 2024-05-03 20:16:33.426798 rstms_testmail-0.1.1/rstms_testmail/version.py
+-rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.1.1/rstms_testmail/watcher.py
+-rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2259 2024-04-28 01:57:04.271457 rstms_testmail-0.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.1.1/tests/test_counter.py
+-rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.1.1/tests/test_gmail.py
+-rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.1.1/tests/test_netstat.py
+-rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.1.1/tests/test_sendgrid.py
+-rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.1.1/tests/test_watcher.py
+-rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.1.1/tox.ini
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.1.1/PKG-INFO
```

### Comparing `rstms_testmail-0.1.0/.gitignore` & `rstms_testmail-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/LICENSE` & `rstms_testmail-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/Makefile` & `rstms_testmail-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/README.md` & `rstms_testmail-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/docs/Makefile` & `rstms_testmail-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/docs/conf.py` & `rstms_testmail-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/docs/installation.rst` & `rstms_testmail-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/docs/make.bat` & `rstms_testmail-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/clean.mk` & `rstms_testmail-0.1.1/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/common.mk` & `rstms_testmail-0.1.1/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/docs.mk` & `rstms_testmail-0.1.1/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/lint.mk` & `rstms_testmail-0.1.1/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/publish.mk` & `rstms_testmail-0.1.1/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/release.mk` & `rstms_testmail-0.1.1/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/test.mk` & `rstms_testmail-0.1.1/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/make/version.mk` & `rstms_testmail-0.1.1/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/pyproject.toml` & `rstms_testmail-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-testmail"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_testmail"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_testmail-0.1.0/rstms_testmail/cli.py` & `rstms_testmail-0.1.1/rstms_testmail/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 @click.option("-c", "--set-counter", type=int)
 @click.option("-s", "--system", envvar="TESTMAIL_SYSTEM")
 @click.option("-e", "--exec", "exec_command", envvar="TESTMAIL_EXEC")
 @click.option("-k", "--api-key", envvar="TESTMAIL_API_KEY")
 @click.option("-u", "--username", envvar="TESTMAIL_USERNAME")
 @click.option("-p", "--password", envvar="TESTMAIL_PASSWORD")
 @click.option("-P", "--port", default=465, envvar="TESTMAIL_PORT")
-@click.option('--profile', default='default', envvar='TESTMAIL_PROFILE')
+@click.option('--profile', default='default', show_envvar=True, envvar='TESTMAIL_PROFILE')
 @click.option("--dryrun", is_flag=True)
 @click.argument("message", required=False)
 @click.pass_context
 def cli(ctx, debug, shell_completion, quiet, verbose, dryrun, to_addr, from_addr, set_counter, subject, message, system, exec_command, username, password, port, api_key, profile):
     """send a test email"""
 
     if "{}" in subject:
```

### Comparing `rstms_testmail-0.1.0/rstms_testmail/counter.py` & `rstms_testmail-0.1.1/rstms_testmail/counter.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/exception_handler.py` & `rstms_testmail-0.1.1/rstms_testmail/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/gmail.py` & `rstms_testmail-0.1.1/rstms_testmail/gmail.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/sendgrid_server.py` & `rstms_testmail-0.1.1/rstms_testmail/sendgrid_server.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/settings.py` & `rstms_testmail-0.1.1/rstms_testmail/settings.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/shell.py` & `rstms_testmail-0.1.1/rstms_testmail/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/smtp_server.py` & `rstms_testmail-0.1.1/rstms_testmail/smtp_server.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/timer.py` & `rstms_testmail-0.1.1/rstms_testmail/timer.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/rstms_testmail/watcher.py` & `rstms_testmail-0.1.1/rstms_testmail/watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/tests/test_cli.py` & `rstms_testmail-0.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/tests/test_sendgrid.py` & `rstms_testmail-0.1.1/tests/test_sendgrid.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/tests/test_watcher.py` & `rstms_testmail-0.1.1/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.1.0/PKG-INFO` & `rstms_testmail-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-testmail
-Version: 0.1.0
+Version: 0.1.1
 Summary: Top-level package for rstms-testmail.
 Keywords: rstms_testmail
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

