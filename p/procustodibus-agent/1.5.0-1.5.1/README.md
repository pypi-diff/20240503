# Comparing `tmp/procustodibus_agent-1.5.0.tar.gz` & `tmp/procustodibus_agent-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procustodibus_agent-1.5.0.tar", last modified: Fri Apr  5 20:29:39 2024, max compression
+gzip compressed data, was "procustodibus_agent-1.5.1.tar", last modified: Fri May  3 18:59:11 2024, max compression
```

## Comparing `procustodibus_agent-1.5.0.tar` & `procustodibus_agent-1.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.370915 procustodibus_agent-1.5.0/
--rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.0/LICENSE
--rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.5.0/MANIFEST.in
--rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-04-05 20:29:39.370915 procustodibus_agent-1.5.0/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     4732 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.0/README.md
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.354905 procustodibus_agent-1.5.0/procustodibus_agent/
--rw-rw-r--   0 justin    (1000) justin    (1000)      208 2024-04-05 18:04:51.000000 procustodibus_agent-1.5.0/procustodibus_agent/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2898 2023-10-08 21:10:01.000000 procustodibus_agent-1.5.0/procustodibus_agent/agent.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    10970 2023-12-10 23:12:39.000000 procustodibus_agent-1.5.0/procustodibus_agent/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1889 2023-12-10 23:12:39.000000 procustodibus_agent-1.5.0/procustodibus_agent/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    17905 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     5464 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.0/procustodibus_agent/connectivity.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.5.0/procustodibus_agent/credentials.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.358908 procustodibus_agent-1.5.0/procustodibus_agent/executor/
--rw-rw-r--   0 justin    (1000) justin    (1000)      122 2024-04-05 18:04:48.000000 procustodibus_agent-1.5.0/procustodibus_agent/executor/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    34310 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/executor/execution.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    20632 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/executor/sys_cmd.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     7432 2024-04-05 18:04:47.000000 procustodibus_agent-1.5.0/procustodibus_agent/ip_route.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/procustodibus_agent/mfa/
--rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.0/procustodibus_agent/mfa/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.0/procustodibus_agent/mfa/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.0/procustodibus_agent/mfa/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.5.0/procustodibus_agent/resolve_hostname.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.5.0/procustodibus_agent/wg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    13359 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/wg_cnf.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/procustodibus_agent/windows/
--rw-rw-r--   0 justin    (1000) justin    (1000)     5763 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.0/procustodibus_agent/windows/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2132 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.0/procustodibus_agent/windows/service.py
--rw-rw-r--   0 justin    (1000) justin    (1000)      344 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/procustodibus_agent/windows/service_config.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/
--rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     1130 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      187 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      714 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/requires.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       20 2024-04-05 20:29:39.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.5.0/procustodibus_agent.egg-info/zip-safe
--rw-rw-r--   0 justin    (1000) justin    (1000)       92 2024-03-17 03:21:19.000000 procustodibus_agent-1.5.0/pyproject.toml
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-04-05 20:29:39.362910 procustodibus_agent-1.5.0/requirements/
--rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.5.0/requirements/dev.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.0/requirements/lint.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      124 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/requirements/prod.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.5.0/requirements/test.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      591 2024-04-05 20:29:39.370915 procustodibus_agent-1.5.0/setup.cfg
--rw-rw-r--   0 justin    (1000) justin    (1000)     2273 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.0/setup.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.124505 procustodibus_agent-1.5.1/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.1/LICENSE
+-rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.5.1/MANIFEST.in
+-rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-05-03 18:59:11.124505 procustodibus_agent-1.5.1/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4732 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.1/README.md
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.104457 procustodibus_agent-1.5.1/procustodibus_agent/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      208 2024-05-03 18:21:41.000000 procustodibus_agent-1.5.1/procustodibus_agent/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3153 2024-05-03 18:21:40.000000 procustodibus_agent-1.5.1/procustodibus_agent/agent.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    10970 2023-12-10 23:12:39.000000 procustodibus_agent-1.5.1/procustodibus_agent/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1895 2024-05-03 18:21:40.000000 procustodibus_agent-1.5.1/procustodibus_agent/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    18953 2024-05-03 18:21:40.000000 procustodibus_agent-1.5.1/procustodibus_agent/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5464 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.1/procustodibus_agent/connectivity.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.5.1/procustodibus_agent/credentials.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.108467 procustodibus_agent-1.5.1/procustodibus_agent/executor/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      122 2024-04-05 18:04:48.000000 procustodibus_agent-1.5.1/procustodibus_agent/executor/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    34310 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/executor/execution.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    20632 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/executor/sys_cmd.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7432 2024-04-05 18:04:47.000000 procustodibus_agent-1.5.1/procustodibus_agent/ip_route.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.112476 procustodibus_agent-1.5.1/procustodibus_agent/mfa/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.1/procustodibus_agent/mfa/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.1/procustodibus_agent/mfa/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.1/procustodibus_agent/mfa/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.5.1/procustodibus_agent/resolve_hostname.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.5.1/procustodibus_agent/wg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    13359 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/wg_cnf.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.112476 procustodibus_agent-1.5.1/procustodibus_agent/windows/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5763 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.1/procustodibus_agent/windows/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2132 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.1/procustodibus_agent/windows/service.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)      344 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/windows/service_config.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.116486 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/
+-rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1130 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      187 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      714 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       20 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/zip-safe
+-rw-rw-r--   0 justin    (1000) justin    (1000)       92 2024-03-17 03:21:19.000000 procustodibus_agent-1.5.1/pyproject.toml
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.116486 procustodibus_agent-1.5.1/requirements/
+-rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.5.1/requirements/dev.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.1/requirements/lint.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      124 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/requirements/prod.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.5.1/requirements/test.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      591 2024-05-03 18:59:11.124505 procustodibus_agent-1.5.1/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2273 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/setup.py
```

### Comparing `procustodibus_agent-1.5.0/LICENSE` & `procustodibus_agent-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/PKG-INFO` & `procustodibus_agent-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.5.0
+Version: 1.5.1
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
```

### Comparing `procustodibus_agent-1.5.0/README.md` & `procustodibus_agent-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/agent.py` & `procustodibus_agent-1.5.1/procustodibus_agent/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """Agent logic."""
 from io import StringIO
 from logging import getLogger
 from time import sleep
 
 from procustodibus_agent import __version__ as version
 from procustodibus_agent.api import ping_api
+from procustodibus_agent.cnf import reload_cnf_if_modified
 from procustodibus_agent.connectivity import check_connectivity
 from procustodibus_agent.executor import execute_desired
 from procustodibus_agent.ip_route import annotate_wg_show_with_ip_address_show
 from procustodibus_agent.resolve_hostname import apply_endpoint_hostnames
 from procustodibus_agent.wg import filter_wg_show, parse_wg_show, run_wg_show
 from procustodibus_agent.wg_cnf import annotate_wg_show_with_wg_cnf
 
@@ -35,33 +36,37 @@
             getLogger(__name__).error(buffer.getvalue())
         return False
 
     getLogger(__name__).info(buffer.getvalue())
     return True
 
 
-def ping_loop(cnf):
+def ping_loop(cnf, cli_args=None):
     """Pings continuously as specified by looping configuration.
 
     Arguments:
         cnf (Config): Config object.
+        cli_args (list): List of arguments to pass to Cnf constructor when reloading.
     """
     good = is_connection_good(cnf, message=f"Starting agent {version}")
+    hide_error = True
 
     while cnf.loop:
         if good:
             try:
                 ping(cnf)
             except Exception:
                 getLogger(__name__).exception("ping failed")
-                good = is_connection_good(cnf)
-            sleep(cnf.loop)
+                good = False
+                hide_error = False
         else:
-            sleep(cnf.loop)
-            good = is_connection_good(cnf, expect_error=True)
+            good = is_connection_good(cnf, expect_error=hide_error)
+            hide_error = True
+        sleep(cnf.loop)
+        cnf = reload_cnf_if_modified(cnf, cli_args)
 
 
 def ping(cnf):
     """Gathers wg info and pings api, executing desired changes from response.
 
     Arguments:
         cnf (Config): Config object.
```

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/api.py` & `procustodibus_agent-1.5.1/procustodibus_agent/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/cli.py` & `procustodibus_agent-1.5.1/procustodibus_agent/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
     Arguments:
         *args (list): List of arguments to pass to Cnf constructor.
     """
     cnf = Cnf(*args)
 
     if cnf.loop:
-        ping_loop(cnf)
+        ping_loop(cnf, args)
     else:
         ping(cnf)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/cnf.py` & `procustodibus_agent-1.5.1/procustodibus_agent/cnf.py`

 * *Files 3% similar despite different names*

```diff
@@ -521,14 +521,45 @@
     if key in ["loop"]:
         if isinstance(value, str):
             return int(value)
 
     return value
 
 
+def get_file_last_modified(cnf_file):
+    """Returns the last modified time of the specified procustodibus config file.
+
+    Arguments:
+        cnf_file (str): Path to config file.
+
+    Returns:
+        float: Last modified time in seconds.
+    """
+    f = Path(cnf_file)
+    return f.stat().st_mtime if f.is_file() else 0
+
+
+def reload_cnf_if_modified(cnf, cli_args=None):
+    """Reloads the cnf file if modified.
+
+    Arguments:
+        cnf (Cnf): Config object.
+        cli_args (list): List of arguments to pass to Cnf constructor when reloading.
+
+    Returns:
+        Cnf: Config object (existing or reloaded).
+    """
+    if cnf.watch_cnf:
+        f = cnf.cnf_file or find_default_cnf()
+        if cnf.cnf_file_last_modified != get_file_last_modified(f):
+            logging.getLogger(__name__).info("Reloading configuration")
+            return Cnf(*cli_args) if cli_args else Cnf()
+    return cnf
+
+
 class Cnf(dict):
     """Configuration object."""
 
     # simpler to keep logic in same function even if it makes cognitive-complexity high
     def __init__(self, cnf_file="", verbosity=None, loop=0):  # noqa: CCR001
         """Creates new configuration object.
 
@@ -556,14 +587,16 @@
         self.resolve_hostnames = "auto"
         self.unmanaged_interfaces = []
 
         if not cnf_file:
             cnf_file = find_default_cnf()
         self.cnf_file = cnf_file
         apply_cnf(self, load_cnf(cnf_file))
+        self.cnf_file_last_modified = get_file_last_modified(cnf_file)
+        self.watch_cnf = bool(environ.get("PROCUSTODIBUS_WATCH_CONF"))
 
         if verbosity == 1:
             verbosity = "INFO"
         if verbosity == 2:
             verbosity = "DEBUG"
         if not self.logging:
             self.logging = _locate_extra_cnf_file(cnf_file, "logging")
```

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/connectivity.py` & `procustodibus_agent-1.5.1/procustodibus_agent/connectivity.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/credentials.py` & `procustodibus_agent-1.5.1/procustodibus_agent/credentials.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/executor/execution.py` & `procustodibus_agent-1.5.1/procustodibus_agent/executor/execution.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/executor/sys_cmd.py` & `procustodibus_agent-1.5.1/procustodibus_agent/executor/sys_cmd.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/ip_route.py` & `procustodibus_agent-1.5.1/procustodibus_agent/ip_route.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/mfa/__init__.py` & `procustodibus_agent-1.5.1/procustodibus_agent/mfa/__init__.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/mfa/api.py` & `procustodibus_agent-1.5.1/procustodibus_agent/mfa/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/mfa/cli.py` & `procustodibus_agent-1.5.1/procustodibus_agent/mfa/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/resolve_hostname.py` & `procustodibus_agent-1.5.1/procustodibus_agent/resolve_hostname.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/wg.py` & `procustodibus_agent-1.5.1/procustodibus_agent/wg.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/wg_cnf.py` & `procustodibus_agent-1.5.1/procustodibus_agent/wg_cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/windows/cnf.py` & `procustodibus_agent-1.5.1/procustodibus_agent/windows/cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent/windows/service.py` & `procustodibus_agent-1.5.1/procustodibus_agent/windows/service.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent.egg-info/PKG-INFO` & `procustodibus_agent-1.5.1/procustodibus_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.5.0
+Version: 1.5.1
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
```

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent.egg-info/SOURCES.txt` & `procustodibus_agent-1.5.1/procustodibus_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/procustodibus_agent.egg-info/requires.txt` & `procustodibus_agent-1.5.1/procustodibus_agent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/requirements/lint.txt` & `procustodibus_agent-1.5.1/requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/setup.cfg` & `procustodibus_agent-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.0/setup.py` & `procustodibus_agent-1.5.1/setup.py`

 * *Files identical despite different names*

