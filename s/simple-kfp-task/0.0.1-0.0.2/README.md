# Comparing `tmp/simple_kfp_task-0.0.1.tar.gz` & `tmp/simple_kfp_task-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task-0.0.1.tar", last modified: Fri May  3 07:24:15 2024, max compression
+gzip compressed data, was "simple_kfp_task-0.0.2.tar", last modified: Fri May  3 07:48:58 2024, max compression
```

## Comparing `simple_kfp_task-0.0.1.tar` & `simple_kfp_task-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:24:15.099633 simple_kfp_task-0.0.1/
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     1077 2024-05-03 07:11:12.000000 simple_kfp_task-0.0.1/LICENSE
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      555 2024-05-03 07:24:15.098987 simple_kfp_task-0.0.1/PKG-INFO
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:10:43.000000 simple_kfp_task-0.0.1/README.md
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      689 2024-05-03 07:24:06.000000 simple_kfp_task-0.0.1/pyproject.toml
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       38 2024-05-03 07:24:15.099765 simple_kfp_task-0.0.1/setup.cfg
-drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:24:15.095755 simple_kfp_task-0.0.1/simple_kfp_task/
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       19 2024-05-02 17:02:34.000000 simple_kfp_task-0.0.1/simple_kfp_task/__init__.py
--rwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)     1607 2024-05-02 20:55:36.000000 simple_kfp_task-0.0.1/simple_kfp_task/cli.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)    10826 2024-05-02 20:55:39.000000 simple_kfp_task-0.0.1/simple_kfp_task/deploykf.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     3855 2024-05-02 20:55:47.000000 simple_kfp_task-0.0.1/simple_kfp_task/git.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)    10578 2024-05-03 06:32:44.000000 simple_kfp_task-0.0.1/simple_kfp_task/pipeline.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     3048 2024-05-03 06:33:10.000000 simple_kfp_task-0.0.1/simple_kfp_task/task.py
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      793 2024-05-03 06:30:52.000000 simple_kfp_task-0.0.1/simple_kfp_task/utils.py
-drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:24:15.098394 simple_kfp_task-0.0.1/simple_kfp_task.egg-info/
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      555 2024-05-03 07:24:15.000000 simple_kfp_task-0.0.1/simple_kfp_task.egg-info/PKG-INFO
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      409 2024-05-03 07:24:15.000000 simple_kfp_task-0.0.1/simple_kfp_task.egg-info/SOURCES.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)        1 2024-05-03 07:24:15.000000 simple_kfp_task-0.0.1/simple_kfp_task.egg-info/dependency_links.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       61 2024-05-03 07:24:15.000000 simple_kfp_task-0.0.1/simple_kfp_task.egg-info/entry_points.txt
--rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       16 2024-05-03 07:24:15.000000 simple_kfp_task-0.0.1/simple_kfp_task.egg-info/top_level.txt
+drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:48:58.518621 simple_kfp_task-0.0.2/
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     1077 2024-05-03 07:11:12.000000 simple_kfp_task-0.0.2/LICENSE
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      852 2024-05-03 07:48:58.518205 simple_kfp_task-0.0.2/PKG-INFO
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:10:43.000000 simple_kfp_task-0.0.2/README.md
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      788 2024-05-03 07:48:53.000000 simple_kfp_task-0.0.2/pyproject.toml
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      161 2024-05-03 07:19:04.000000 simple_kfp_task-0.0.2/requirements.txt
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       38 2024-05-03 07:48:58.518710 simple_kfp_task-0.0.2/setup.cfg
+drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:48:58.513951 simple_kfp_task-0.0.2/simple_kfp_task/
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       19 2024-05-02 17:02:34.000000 simple_kfp_task-0.0.2/simple_kfp_task/__init__.py
+-rwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)     1607 2024-05-02 20:55:36.000000 simple_kfp_task-0.0.2/simple_kfp_task/cli.py
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)    10826 2024-05-02 20:55:39.000000 simple_kfp_task-0.0.2/simple_kfp_task/deploykf.py
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     3855 2024-05-02 20:55:47.000000 simple_kfp_task-0.0.2/simple_kfp_task/git.py
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     9711 2024-05-03 07:38:07.000000 simple_kfp_task-0.0.2/simple_kfp_task/pipeline.py
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)     3217 2024-05-03 07:36:34.000000 simple_kfp_task-0.0.2/simple_kfp_task/task.py
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      793 2024-05-03 06:30:52.000000 simple_kfp_task-0.0.2/simple_kfp_task/utils.py
+drwxr-xr-x   0 SebastianAlberternst   (503) staff       (20)        0 2024-05-03 07:48:58.517536 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      852 2024-05-03 07:48:58.000000 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/PKG-INFO
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      464 2024-05-03 07:48:58.000000 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/SOURCES.txt
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)        1 2024-05-03 07:48:58.000000 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/dependency_links.txt
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       61 2024-05-03 07:48:58.000000 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/entry_points.txt
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)      162 2024-05-03 07:48:58.000000 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/requires.txt
+-rw-r--r--   0 SebastianAlberternst   (503) staff       (20)       16 2024-05-03 07:48:58.000000 simple_kfp_task-0.0.2/simple_kfp_task.egg-info/top_level.txt
```

### Comparing `simple_kfp_task-0.0.1/LICENSE` & `simple_kfp_task-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.1/pyproject.toml` & `simple_kfp_task-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-kfp-task"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dynamic = ["dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
 simple-kfp-task = "simple_kfp_task.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/salberternst/simple-kfp-task"
 Issues = "https://github.com/salberternst/simple-kfp-task/issues"
```

### Comparing `simple_kfp_task-0.0.1/simple_kfp_task/cli.py` & `simple_kfp_task-0.0.2/simple_kfp_task/cli.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.1/simple_kfp_task/deploykf.py` & `simple_kfp_task-0.0.2/simple_kfp_task/deploykf.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.1/simple_kfp_task/git.py` & `simple_kfp_task-0.0.2/simple_kfp_task/git.py`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.1/simple_kfp_task/pipeline.py` & `simple_kfp_task-0.0.2/simple_kfp_task/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,38 +41,14 @@
         name="Create Git Diff ConfigMap",
         k8s_resource=configmap,
         action="create",
         attribute_outputs={"name": "{.metadata.name}"}
     )
 
 
-def create_func_configmap_op(func: str):
-    """
-    Create a ConfigMap operation.
-
-    Returns:
-        dsl.ContainerOp: The ConfigMap operation.
-    """
-
-    configmap = kubernetes_client.V1ConfigMap(
-        kind="ConfigMap",
-        api_version="v1",
-        metadata=kubernetes_client.V1ObjectMeta(
-            name="{{workflow.name}}-func-config"),
-        data={"func": func}
-    )
-
-    return dsl.ResourceOp(
-        name="Create Func ConfigMap",
-        k8s_resource=configmap,
-        action="create",
-        attribute_outputs={"name": "{.metadata.name}"}
-    )
-
-
 def git_clone_op(
     remote_url: str,
     branch: str,
     volume_path: str,
     commit='HEAD'
 ):
     """
@@ -211,22 +187,14 @@
         name='Run Command',
         image=container_image,
         command=['bash', '-c', 'source venv/bin/activate && python %s %s' %
                  (command, command_args)],
         container_kwargs={'working_dir': '/app'}
     )
 
-def run_func_op(container_image: str):
-    return dsl.ContainerOp(
-        name='Run Function',
-        image=container_image,
-        command=['bash', '-c', 'source venv/bin/activate && cat /tmp/func | base64 -d | gunzip | python -'],
-        container_kwargs={'working_dir': '/app'}
-    )
-
 @dsl.pipeline(
     name='Simple Task Pipeline',
     description='A simple pipeline that clones a Git repository, creates a virtual environment, runs pip, and executes a script.'
 )
 def simple_task_pipeline(
     remote_url='https://github.com/your/repo.git',
     branch='main',
```

### Comparing `simple_kfp_task-0.0.1/simple_kfp_task/task.py` & `simple_kfp_task-0.0.2/simple_kfp_task/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from simple_kfp_task.git import build_git_diff, get_current_branch, get_current_commit, get_git_root, get_remote_url, is_branch_available_on_remote, is_commit_available_on_remote, is_git_dirty
 from typing import Callable
 from simple_kfp_task.pipeline import simple_task_pipeline
 from simple_kfp_task.utils import encode_string_to_base64, generate_function_code, get_caller_filename
 import os
 
 GIT_DIFF_MAX_LENGTH = 10000
+PIP_PACKAGE_NAME = "simple-kfp-task"
 
 def run(
         # kfp
         namespace=None,
         run_name=None,
         experiment_name=None,
         # command
@@ -34,14 +35,18 @@
         dry_run=False):
 
     if os.environ.get('INSIDE_KFP_FUNC_CONTAINER') and not func:
         return func()
     
     if func:
         command = get_caller_filename()
+        if packages is None:
+            packages = [ PIP_PACKAGE_NAME]
+        else:
+            packages.append(PIP_PACKAGE_NAME)
 
     if command:
         command = get_git_root(command)
 
     if remote_url is None:
         raise ValueError("Could not determine remote origin")
```

### Comparing `simple_kfp_task-0.0.1/simple_kfp_task/utils.py` & `simple_kfp_task-0.0.2/simple_kfp_task/utils.py`

 * *Files identical despite different names*

