# Comparing `tmp/fourdigits-cli-1.8.1.tar.gz` & `tmp/fourdigits-cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fourdigits-cli-1.8.1.tar", last modified: Mon Nov 20 08:04:47 2023, max compression
+gzip compressed data, was "fourdigits-cli-1.9.0.tar", last modified: Thu Nov 23 09:51:44 2023, max compression
```

## Comparing `fourdigits-cli-1.8.1.tar` & `fourdigits-cli-1.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-20 08:04:47.942689 fourdigits-cli-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2086 2023-11-20 08:04:47.942689 fourdigits-cli-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1617 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-20 08:04:47.937686 fourdigits-cli-1.8.1/fourdigits_cli/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-20 08:04:47.940688 fourdigits-cli-1.8.1/fourdigits_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5786 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/commands/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/commands/exonet.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/commands/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-20 08:04:47.940688 fourdigits-cli-1.8.1/fourdigits_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3483 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/utils/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/fourdigits_cli/utils/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-20 08:04:47.939687 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2086 2023-11-20 08:04:47.000000 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      659 2023-11-20 08:04:47.000000 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-20 08:04:47.000000 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-11-20 08:04:47.000000 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-11-20 08:04:47.000000 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-11-20 08:04:47.000000 fourdigits-cli-1.8.1/fourdigits_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-11-20 08:04:47.942689 fourdigits-cli-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-20 08:04:47.941688 fourdigits-cli-1.8.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-11-20 08:03:48.000000 fourdigits-cli-1.8.1/tests/test_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 09:51:44.985765 fourdigits-cli-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-11-23 09:51:44.985765 fourdigits-cli-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 09:51:44.981765 fourdigits-cli-1.9.0/fourdigits_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 09:51:44.983765 fourdigits-cli-1.9.0/fourdigits_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5786 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/commands/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/commands/exonet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/commands/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 09:51:44.984765 fourdigits-cli-1.9.0/fourdigits_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/utils/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/fourdigits_cli/utils/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 09:51:44.984765 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-11-23 09:51:44.000000 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      659 2023-11-23 09:51:44.000000 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-23 09:51:44.000000 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-11-23 09:51:44.000000 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-11-23 09:51:44.000000 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-11-23 09:51:44.000000 fourdigits-cli-1.9.0/fourdigits_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-11-23 09:51:44.986765 fourdigits-cli-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-23 09:51:44.984765 fourdigits-cli-1.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-11-23 09:50:48.000000 fourdigits-cli-1.9.0/tests/test_settings.py
```

### Comparing `fourdigits-cli-1.8.1/PKG-INFO` & `fourdigits-cli-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.8.1
+Version: 1.9.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.3
 Requires-Dist: tomli~=2.0.1
 Requires-Dist: packaging
 Requires-Dist: requests
```

### Comparing `fourdigits-cli-1.8.1/README.md` & `fourdigits-cli-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/cli.py` & `fourdigits-cli-1.9.0/fourdigits_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/commands/docker.py` & `fourdigits-cli-1.9.0/fourdigits_cli/commands/docker.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/commands/exonet.py` & `fourdigits-cli-1.9.0/fourdigits_cli/commands/exonet.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,37 +16,41 @@
     pass
 
 
 @group.command()
 @click.argument("environment")
 @click.argument("docker_tag")
 @click.option("--message", default="", show_default=True)
-def deploy(environment, docker_tag, message=""):
+@click.option("--name", default="", show_default=True)
+def deploy(environment, docker_tag, message="", name=""):
     drone_token = os.getenv("DRONE_TOKEN", "")
+    name = name or DEFAULT_CONFIG.exonet_project_name
+
     if not drone_token:
         raise click.ClickException("Environment variable DRONE_TOKEN is not set")
 
     if environment not in DEFAULT_CONFIG.environments:
         raise click.ClickException("Environment doesn't exists in the pyproject.toml")
 
-    if not DEFAULT_CONFIG.exonet_project_name:
+    if not name:
         raise click.ClickException(
-            "The option exonet_project_name doesn't exists in the pyproject.toml"
+            "No name found. You can supply this by settings the exonet_project_name "
+            "in pyproject.toml. Alternatively, you can pass it as the --name argument."
         )
 
     if not message:
-        message = f"[{DEFAULT_CONFIG.exonet_project_name}] Deploying {docker_tag} to {environment} environment"  # noqa: E501
+        message = f"[{name}] Deploying {docker_tag} to {environment} environment"
 
     response = requests.post(
         url=DRONE_BUILD_URL,
         headers={
             "Authorization": f"Bearer {drone_token}",
         },
         params={
-            "name": DEFAULT_CONFIG.exonet_project_name,
+            "name": name,
             "target": environment,
             "tag": docker_tag,
             "channel": DEFAULT_CONFIG.slack_channel,
             "message": message,
         },
     )
```

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/commands/gitlab.py` & `fourdigits-cli-1.9.0/fourdigits_cli/commands/gitlab.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/settings.py` & `fourdigits-cli-1.9.0/fourdigits_cli/settings.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/utils/docker.py` & `fourdigits-cli-1.9.0/fourdigits_cli/utils/docker.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli/utils/git.py` & `fourdigits-cli-1.9.0/fourdigits_cli/utils/git.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli.egg-info/PKG-INFO` & `fourdigits-cli-1.9.0/fourdigits_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.8.1
+Version: 1.9.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.3
 Requires-Dist: tomli~=2.0.1
 Requires-Dist: packaging
 Requires-Dist: requests
```

### Comparing `fourdigits-cli-1.8.1/fourdigits_cli.egg-info/SOURCES.txt` & `fourdigits-cli-1.9.0/fourdigits_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/setup.py` & `fourdigits-cli-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.8.1/tests/test_settings.py` & `fourdigits-cli-1.9.0/tests/test_settings.py`

 * *Files identical despite different names*

