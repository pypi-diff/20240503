# Comparing `tmp/aws_ssm_juggle-24.5.1.tar.gz` & `tmp/aws_ssm_juggle-24.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_juggle-24.5.1.tar", max compression
+gzip compressed data, was "aws_ssm_juggle-24.5.2.tar", max compression
```

## Comparing `aws_ssm_juggle-24.5.1.tar` & `aws_ssm_juggle-24.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.5.1/LICENSE
--rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.5.1/README.md
--rw-r--r--   0        0        0     2117 2024-05-02 09:08:44.744453 aws_ssm_juggle-24.5.1/aws_ssm_juggle/__init__.py
--rw-r--r--   0        0        0     6910 2024-05-02 09:15:30.256428 aws_ssm_juggle-24.5.1/aws_ssm_juggle/ec2.py
--rw-r--r--   0        0        0    10744 2024-05-02 09:15:29.091399 aws_ssm_juggle-24.5.1/aws_ssm_juggle/ecs.py
--rw-r--r--   0        0        0      728 2024-05-02 09:15:38.369695 aws_ssm_juggle-24.5.1/pyproject.toml
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.1/setup.py
--rw-r--r--   0        0        0     3074 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.5.2/LICENSE
+-rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.5.2/README.md
+-rw-r--r--   0        0        0     2307 2024-05-03 12:36:18.759626 aws_ssm_juggle-24.5.2/aws_ssm_juggle/__init__.py
+-rw-r--r--   0        0        0     6936 2024-05-03 12:37:57.704544 aws_ssm_juggle-24.5.2/aws_ssm_juggle/ec2.py
+-rw-r--r--   0        0        0    10970 2024-05-03 12:38:14.119563 aws_ssm_juggle-24.5.2/aws_ssm_juggle/ecs.py
+-rw-r--r--   0        0        0      744 2024-05-03 12:38:49.585761 aws_ssm_juggle-24.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.2/setup.py
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.2/PKG-INFO
```

### Comparing `aws_ssm_juggle-24.5.1/LICENSE` & `aws_ssm_juggle-24.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.1/README.md` & `aws_ssm_juggle-24.5.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.1/aws_ssm_juggle/__init__.py` & `aws_ssm_juggle-24.5.2/aws_ssm_juggle/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import os
 
 from boto3 import session
 from botocore import exceptions
+from diskcache import Cache
 from simple_term_menu import TerminalMenu
 
+cache = Cache("/tmp/_aws-ssm-juggle_cache")
+
 
 def show_menu(
     items: list,
     title: str,
     source: list = None,
     back: bool = True,
     clear_screen: bool = False,
@@ -30,15 +33,17 @@
     if index is None:
         exit(0)
     if items[index] == "Back":
         return None, index
     return source[index], index
 
 
-def port_forward(boto3_session: session.Session, remote_port: int, local_port: int, target: str) -> None:
+def port_forward(
+    boto3_session: session.Session, remote_port: int, local_port: int, target: str
+) -> None:
     """
     forward port
     """
     parameters = {
         "portNumber": [str(remote_port)],
         "localPortNumber": [str(local_port)],
     }
@@ -79,7 +84,12 @@
     try:
         os.execvp(
             "session-manager-plugin",
             args,
         )
     except FileNotFoundError:
         print("session-manager-plugin missing!")
+
+
+@cache.memoize(expire=600)
+def get_boto3_profiles() -> list:
+    return session.Session().available_profiles
```

### Comparing `aws_ssm_juggle-24.5.1/aws_ssm_juggle/ec2.py` & `aws_ssm_juggle-24.5.2/aws_ssm_juggle/ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 import configargparse
 import shtab
 from boto3 import session
 from botocore import exceptions
 
-from aws_ssm_juggle import port_forward, show_menu
+from aws_ssm_juggle import get_boto3_profiles, port_forward, show_menu
 
 
 class EC2Session:
     """
     EC2Session
     """
 
@@ -114,15 +114,15 @@
         ["--print-completion"],
         help="Print shell-completion. Run '. <(ec2-juggle --print-completion bash)' to load.",
     )
     parser.add_argument(
         "--profile",
         help="AWS Profile",
         default="default",
-        choices=session.Session().available_profiles,
+        choices=get_boto3_profiles(),
     )
     parser.add_argument(
         "--region",
         help="AWS region name",
         default="eu-central-1",
     )
     parser.add_argument(
@@ -215,15 +215,17 @@
     if "ssh_args" in arguments:
         ssh_args = arguments.ssh_args
     if "remote_port" in arguments:
         remote_port = arguments.remote_port
     if "local_port" in arguments:
         local_port = arguments.local_port
     while not instance_id:
-        instance_id, _ = get_instance_id(boto3_session=boto3_session, instance_id=instance_id)
+        instance_id, _ = get_instance_id(
+            boto3_session=boto3_session, instance_id=instance_id
+        )
         instance_id = instance_id.split(" - ")[0]
     ec2_session = EC2Session(
         boto3_session=boto3_session,
         instance_id=instance_id,
         local_port=local_port,
         remote_port=remote_port,
         ssh_args=ssh_args,
```

### Comparing `aws_ssm_juggle-24.5.1/aws_ssm_juggle/ecs.py` & `aws_ssm_juggle-24.5.2/aws_ssm_juggle/ecs.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 import configargparse
 import shtab
 from boto3 import session
 from botocore import exceptions
 
-from aws_ssm_juggle import port_forward, show_menu
+from aws_ssm_juggle import get_boto3_profiles, port_forward, show_menu
 
 
 class ECSSession:
     """
     ECSSession
     """
 
@@ -41,18 +41,26 @@
         self.container_index = container_index
         self.ecs = self.boto3_session.client("ecs")
         self.local_port = local_port
         self.remote_port = remote_port
         self.ssm = self.boto3_session.client("ssm")
         self.task = task
         self.task_details = task_details
-        self.runtime_id = task_details.get("tasks")[0].get("containers")[container_index].get("runtimeId")
+        self.runtime_id = (
+            task_details.get("tasks")[0]
+            .get("containers")[container_index]
+            .get("runtimeId")
+        )
         if not self.runtime_id:
-            raise RuntimeError("unable to get runtimeId from container, looks like it's not running.")
-        self.target = f"ecs:{self.cluster}_{self.runtime_id.split('-')[0]}_{self.runtime_id}"
+            raise RuntimeError(
+                "unable to get runtimeId from container, looks like it's not running."
+            )
+        self.target = (
+            f"ecs:{self.cluster}_{self.runtime_id.split('-')[0]}_{self.runtime_id}"
+        )
 
     def port_forward(self):
         port_forward(
             boto3_session=self.boto3_session,
             remote_port=self.remote_port,
             local_port=self.local_port,
             target=self.target,
@@ -103,15 +111,15 @@
         ["--print-completion"],
         help="Print shell-completion. Run '. <(ecs-juggle --print-completion bash)' to load.",
     )
     parser.add_argument(
         "--profile",
         help="AWS Profile",
         default="default",
-        choices=session.Session().available_profiles,
+        choices=get_boto3_profiles(),
     )
     parser.add_argument(
         "--region",
         help="AWS region name",
         default="eu-central-1",
     )
     parser.add_argument(
@@ -238,15 +246,17 @@
         clear_screen=True,
     )
     if ret[0] is None:
         return (cluster, None, *ret)
     return (cluster, service, *ret)
 
 
-def get_container(cluster: str, service: str, task: str, containers: list, container: str):
+def get_container(
+    cluster: str, service: str, task: str, containers: list, container: str
+):
     """
     get container
     """
     if container:
         return task, container, containers.index(container)
     ret = show_menu(
         items=containers,
@@ -278,15 +288,17 @@
         clear_screen=True,
     )
     if ret[0] is None:
         return (None, *ret)
     return (container, *ret)
 
 
-def menu_loop_condition(cluster: str, service: str, task: str, container: str, remote_port: int, action: str):
+def menu_loop_condition(
+    cluster: str, service: str, task: str, container: str, remote_port: int, action: str
+):
     menu_loop_condition = cluster and service and task and container
     if action == "forward":
         menu_loop_condition = menu_loop_condition and remote_port
     return menu_loop_condition
 
 
 def run():
@@ -320,34 +332,41 @@
         task=task,
         container=container,
         remote_port=remote_port,
         action=arguments.action,
     ):
         cluster, _ = get_cluster(ecs=ecs, cluster=cluster)
         cluster, service, _ = get_service(ecs=ecs, cluster=cluster, service=service)
-        cluster, service, task, _ = get_task(ecs=ecs, cluster=cluster, service=service, task=task)
+        cluster, service, task, _ = get_task(
+            ecs=ecs, cluster=cluster, service=service, task=task
+        )
         if cluster and task:
             task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
-            containers = [container.get("name") for container in task_details.get("tasks")[0].get("containers")]
+            containers = [
+                container.get("name")
+                for container in task_details.get("tasks")[0].get("containers")
+            ]
             ret = get_container(
                 cluster=cluster,
                 service=service,
                 task=task,
                 containers=containers,
                 container=container,
             )
             task, container, container_index = ret
         if (arguments.action == "forward" and container) and not remote_port:
             task_definition_arn = task_details.get("tasks")[0].get("taskDefinitionArn")
-            task_definition = task_definition or ecs.describe_task_definition(taskDefinition=task_definition_arn).get(
-                "taskDefinition"
-            )
+            task_definition = task_definition or ecs.describe_task_definition(
+                taskDefinition=task_definition_arn
+            ).get("taskDefinition")
             ports = [
                 str(container.get("containerPort"))
-                for container in task_definition.get("containerDefinitions")[container_index].get("portMappings")
+                for container in task_definition.get("containerDefinitions")[
+                    container_index
+                ].get("portMappings")
             ]
             container, remote_port, _ = get_port(
                 cluster=cluster,
                 service=service,
                 task=task,
                 container=container,
                 containers=containers,
```

### Comparing `aws_ssm_juggle-24.5.1/pyproject.toml` & `aws_ssm_juggle-24.5.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "aws-ssm-juggle"
-version = "24.5.1"
+version = "24.5.2"
 description = "AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/aws-ssm-juggle"
 
 [tool.poetry.dependencies]
 configargparse = "*"
 boto3 = "*"
 shtab = "*"
 simple_term_menu = "*"
+diskcache = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ecs-juggle = 'aws_ssm_juggle.ecs:run'
```

### Comparing `aws_ssm_juggle-24.5.1/setup.py` & `aws_ssm_juggle-24.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['aws_ssm_juggle']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3', 'configargparse', 'shtab', 'simple_term_menu']
+['boto3', 'configargparse', 'diskcache', 'shtab', 'simple_term_menu']
 
 entry_points = \
 {'console_scripts': ['ec2-juggle = aws_ssm_juggle.ec2:run',
                      'ecs-juggle = aws_ssm_juggle.ecs:run']}
 
 setup_kwargs = {
     'name': 'aws-ssm-juggle',
-    'version': '24.5.1',
+    'version': '24.5.2',
     'description': 'AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)',
     'long_description': '# aws-ssm-juggle\n\n## Installation\n\n```\npip install aws-ssm-juggle\n```\n\n## Pre-requisites\n\n### [session-manager-plugin](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html)\n\n#### Linux\n\n```bash\ncurl https://s3.amazonaws.com/session-manager-downloads/plugin/latest/ubuntu_64bit/session-manager-plugin.deb -o "/tmp/session-manager-plugin.deb"\nmkdir -p ~/bin\ndpkg-deb --fsys-tarfile /tmp/session-manager-plugin.deb | tar --strip-components=4 -C ~/bin/ -xvf - usr/local/sessionmanagerplugin/bin/session-manager-plugin\n```\n\n#### MacOS\n\n`brew install --cask session-manager-plugin`\n\n### Infrastructure\n\nUse [ecs-exec-checker](https://github.com/aws-containers/amazon-ecs-exec-checker) to check for the pre-requisites to use ECS exec.\n\n## ecs-juggle\n\nInspired by [ecsgo](https://github.com/tedsmitt/ecsgo).\n\nProvides a tool to interact with AWS ECS tasks.\n\nCurrently provides:\n\n* interactive execute-command (e.g. shell)\n* port-forwarding\n\nYou can supply command-line arguments to specify which cluster/service/task/... to use or will be prompted with a nice menu.\n\n\n### Usage\n\nSee `ecs-juggle --help` for all features.\n\n#### Execute command\n\nSelect all from menu:\n\n```bash\necs-juggle command\n```\n\n#### Port forwarding\n\nSelect all from menu:\n\n```bash\necs-juggle forward\n```\n\nSpecify port and select the rest from menu:\n\n```bash\necs-juggle forward --remote-port 8080\n```\n\n## ec2-juggle\n\nInspired by [gossm](https://github.com/gjbae1212/gossm/).\n\nProvides a tool to interact with AWS EC2 instances.\n\nCurrently provides:\n\n* interactive shell (e.g. shell)\n* ssh shell\n* port-forwarding\n\n### Usage\n\nSee `ec2-juggle --help` for all features.\n\n#### Start session\n\n```bash\nec2-juggle start\n```\n\n#### Start ssh session\n\nDefault:\n\n```bash\nec2-juggle ssh\n```\n\nWith extra arguments:\n\n```bash\nec2-juggle ssh --ssh-args="-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null -l ubuntu"\n```\n\n#### Port forwarding\n\n```bash\necs-juggle forward --remote-port 80\n```\n',
     'author': 'Stefan Heitmüller',
     'author_email': 'stefan.heitmueller@gmx.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/morph027/aws-ssm-juggle',
```

### Comparing `aws_ssm_juggle-24.5.1/PKG-INFO` & `aws_ssm_juggle-24.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-juggle
-Version: 24.5.1
+Version: 24.5.2
 Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)
 Home-page: https://github.com/morph027/aws-ssm-juggle
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3
 Requires-Dist: configargparse
+Requires-Dist: diskcache
 Requires-Dist: shtab
 Requires-Dist: simple_term_menu
 Project-URL: Repository, https://github.com/morph027/aws-ssm-juggle
 Description-Content-Type: text/markdown
 
 # aws-ssm-juggle
```

