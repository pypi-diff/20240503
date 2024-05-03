# Comparing `tmp/bambot-0.4.1.tar.gz` & `tmp/bambot-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.4.1.tar", last modified: Wed May  1 05:30:51 2024, max compression
+gzip compressed data, was "bambot-0.4.2.tar", last modified: Fri May  3 00:32:05 2024, max compression
```

## Comparing `bambot-0.4.1.tar` & `bambot-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:30:51.177772 bambot-0.4.1/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2148 2024-05-01 05:30:51.177564 bambot-0.4.1/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1217 2024-05-01 05:21:22.000000 bambot-0.4.1/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:30:51.174261 bambot-0.4.1/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3593 2024-05-01 05:29:44.000000 bambot-0.4.1/bambot/cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     3326 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/container.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1241 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/docker_utils.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      196 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/logging.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      254 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/metrics.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      446 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/prometheus.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1125 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/streamlit_dashboard.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:30:51.175732 bambot-0.4.1/bambot/templates/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      319 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/templates/Dockerfile
--rw-r--r--   0 spencerkinney   (501) staff       (20)      485 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/templates/agent_template.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      525 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/templates/langchain_template.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      150 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/templates/main.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)       55 2024-05-01 04:48:56.000000 bambot-0.4.1/bambot/templates/requirements.txt
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:30:51.177341 bambot-0.4.1/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     2148 2024-05-01 05:30:51.000000 bambot-0.4.1/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      690 2024-05-01 05:30:51.000000 bambot-0.4.1/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-01 05:30:51.000000 bambot-0.4.1/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-01 05:30:51.000000 bambot-0.4.1/bambot.egg-info/entry_points.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       60 2024-05-01 05:30:51.000000 bambot-0.4.1/bambot.egg-info/requires.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-01 05:30:51.000000 bambot-0.4.1/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-01 05:30:51.177805 bambot-0.4.1/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1248 2024-05-01 05:30:32.000000 bambot-0.4.1/setup.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-01 05:30:51.176970 bambot-0.4.1/tests/
--rw-r--r--   0 spencerkinney   (501) staff       (20)      394 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_cli.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      389 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_container.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      381 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_docker.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      232 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_logging.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      232 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_metrics.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      258 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_prometheus.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      307 2024-05-01 04:49:02.000000 bambot-0.4.1/tests/test_streamlit_dashboard.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 00:32:05.852456 bambot-0.4.2/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2096 2024-05-03 00:32:05.852218 bambot-0.4.2/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1223 2024-05-03 00:27:08.000000 bambot-0.4.2/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 00:32:05.848472 bambot-0.4.2/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        0 2024-05-01 04:48:56.000000 bambot-0.4.2/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2842 2024-05-03 00:22:16.000000 bambot-0.4.2/bambot/app.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2871 2024-05-03 00:27:43.000000 bambot-0.4.2/bambot/cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1583 2024-05-03 00:23:44.000000 bambot-0.4.2/bambot/docker_utils.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 00:32:05.850661 bambot-0.4.2/bambot/templates/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      361 2024-05-02 22:36:19.000000 bambot-0.4.2/bambot/templates/Dockerfile
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      171 2024-05-02 22:06:34.000000 bambot-0.4.2/bambot/templates/agent_runner.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      488 2024-05-02 21:29:46.000000 bambot-0.4.2/bambot/templates/agent_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      528 2024-05-02 21:29:55.000000 bambot-0.4.2/bambot/templates/langchain_template.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       44 2024-05-03 00:15:02.000000 bambot-0.4.2/bambot/templates/requirements.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2561 2024-05-03 00:19:09.000000 bambot-0.4.2/bambot/templates/server.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 00:32:05.851994 bambot-0.4.2/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2096 2024-05-03 00:32:05.000000 bambot-0.4.2/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      632 2024-05-03 00:32:05.000000 bambot-0.4.2/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-05-03 00:32:05.000000 bambot-0.4.2/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       40 2024-05-03 00:32:05.000000 bambot-0.4.2/bambot.egg-info/entry_points.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       32 2024-05-03 00:32:05.000000 bambot-0.4.2/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-05-03 00:32:05.000000 bambot-0.4.2/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-05-03 00:32:05.852496 bambot-0.4.2/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1214 2024-05-03 00:29:24.000000 bambot-0.4.2/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-05-03 00:32:05.851808 bambot-0.4.2/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      394 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_cli.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      389 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_container.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      381 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_docker.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      232 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_logging.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      232 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_metrics.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      258 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_prometheus.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      307 2024-05-01 04:49:02.000000 bambot-0.4.2/tests/test_streamlit_dashboard.py
```

### Comparing `bambot-0.4.1/PKG-INFO` & `bambot-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Containers for AI agents
 Home-page: https://github.com/Bam-Corp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: docker
-Requires-Dist: prometheus-client
-Requires-Dist: streamlit
 Requires-Dist: tqdm
 Requires-Dist: python-dotenv
 
 # Bam
 
 [![PyPI version](https://badge.fury.io/py/bambot.svg)](https://badge.fury.io/py/bambot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -45,19 +43,19 @@
 
 1. Install bambot using pip:
 ```bash
 pip install bambot
 ```
 2. Create a new AI agent container:
 ```bash
-bam create container
+bam app create
 ```
-3. Run the AI agent container:
+3. Run the AI agent container locally:
 ```bash
-bam run
+bam app run
 ```
 
 That's it! You're now ready to start using Bam to create and run AI agent containers.
 
 ## Documentation
 
 For detailed documentation and additional features, please visit our website at [bam.bot](https://bam.bot) (coming soon).
```

### Comparing `bambot-0.4.1/README.md` & `bambot-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 1. Install bambot using pip:
 ```bash
 pip install bambot
 ```
 2. Create a new AI agent container:
 ```bash
-bam create container
+bam app create
 ```
-3. Run the AI agent container:
+3. Run the AI agent container locally:
 ```bash
-bam run
+bam app run
 ```
 
 That's it! You're now ready to start using Bam to create and run AI agent containers.
 
 ## Documentation
 
 For detailed documentation and additional features, please visit our website at [bam.bot](https://bam.bot) (coming soon).
```

### Comparing `bambot-0.4.1/bambot/container.py` & `bambot-0.4.2/bambot/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,75 @@
-# bam/container.py
+# container.py
 import os
 import click
 import pkg_resources
 from dotenv import load_dotenv
 from .docker_utils import build_image, create_docker_container
 import docker
+import signal
+import sys
 
+TEMPLATE_FILES = [
+    "agent_template.py", "Dockerfile", "agent_runner.py", "requirements.txt", "server.py"
+]
 
-def create_container(container_name, agent_type, env_file=".env"):
-    """Create a new container for an AI agent"""
+def create_app(container_name, agent_type, env_file=".env"):
+    """Create a new app for an AI agent"""
     # Create a new directory for the container
     container_dir = os.path.join(os.getcwd(), container_name)
     os.makedirs(container_dir, exist_ok=True)
 
-    # Generate template project structure
+    # Copy template files to the container directory
     click.echo(click.style("Generating project structure...", fg="yellow"))
     templates_dir = pkg_resources.resource_filename(__name__, 'templates')
-    template_path = os.path.join(templates_dir, "agent_template.py")
-    with open(template_path, "r") as f:
-        template = f.read()
-    template = template.replace("{{AGENT_TYPE}}", agent_type)
-    
-    # Create the agent file
-    agent_file_path = os.path.join(container_dir, f"{agent_type}_agent.py")
-    with open(agent_file_path, "w") as f:
-        f.write(template)
-    
-    # Generate requirements.txt based on the agent type
-    click.echo(click.style("Generating requirements.txt...", fg="yellow"))
-    requirements_template = pkg_resources.resource_string(__name__, "templates/requirements.txt").decode()
-    requirements_template = requirements_template.replace("{{AGENT_TYPE}}", agent_type)
-    requirements_path = os.path.join(container_dir, "requirements.txt")
-    with open(requirements_path, "w") as f:
-        f.write(requirements_template)
-    
-    # Generate Dockerfile
-    click.echo(click.style("Generating Dockerfile...", fg="yellow"))
-    dockerfile_path = os.path.join(container_dir, "Dockerfile")
-    dockerfile_template = pkg_resources.resource_string(__name__, "templates/Dockerfile").decode()
-    with open(dockerfile_path, "w") as f:
-        f.write(dockerfile_template)
-    
-    # Copy main.py file
-    main_file_path = os.path.join(container_dir, "main.py")
-    main_template = pkg_resources.resource_string(__name__, "templates/main.py").decode()
-    main_template = main_template.replace("{{AGENT_TYPE}}", agent_type)
-    with open(main_file_path, "w") as f:
-        f.write(main_template)
-    
+    for filename in TEMPLATE_FILES:
+        template_path = os.path.join(templates_dir, filename)
+        with open(template_path, "r") as f:
+            template = f.read()
+        template = template.replace("{{AGENT_TYPE}}", agent_type)
+        file_path = os.path.join(container_dir, filename.replace("agent_template.py", f"{agent_type}_agent.py"))
+        with open(file_path, "w") as f:
+            f.write(template)
+
     # Load environment variables from .env file
     env_file_path = os.path.join(container_dir, env_file)
     load_dotenv(env_file_path)
     env_vars = {key: value for key, value in os.environ.items()}
-    
+
     # Build Docker image
     click.echo(click.style("Building Docker image...", fg="yellow"))
     build_image(container_dir)
     click.echo(click.style("Docker image built successfully!", fg="green"))
-    
+
     # Create Docker container
     click.echo(click.style("Creating Docker container...", fg="yellow"))
     create_docker_container(container_name, env_vars)
-    click.echo(click.style(f"Container '{container_name}' created successfully!", fg="green"))
 
-def run_container(container_name):
-    """Run a container for an AI agent"""
+def run_app(container_name):
+    """Run an app for an AI agent"""
     docker_client = docker.from_env()
     container = docker_client.containers.get(container_name)
-    
     click.echo(click.style(f"Starting container: {container_name}", fg="yellow"))
     container.start()
-    
+
     # Stream container logs
     click.echo(click.style("Container logs:", fg="yellow"))
-    for log in container.logs(stream=True):
-        click.echo(log.decode(), nl=False)
-    
-    container.wait()
+
+    # Set up signal handler for SIGINT (Ctrl+C)
+    def signal_handler(sig, frame):
+        click.echo(click.style("\nStopping container...", fg="yellow"))
+        container.stop()
+        click.echo(click.style("Container stopped.", fg="green"))
+        sys.exit(0)
+
+    signal.signal(signal.SIGINT, signal_handler)
+
+    try:
+        for log in container.logs(stream=True, follow=True):
+            try:
+                log_str = log.decode('utf-8')
+                click.echo(log_str, nl=False)
+            except UnicodeDecodeError:
+                click.echo(f"Error decoding log line: {log}", nl=False)
+    except KeyboardInterrupt:
+        # Handle KeyboardInterrupt separately
+        signal_handler(signal.SIGINT, None)
```

### Comparing `bambot-0.4.1/bambot/docker_utils.py` & `bambot-0.4.2/bambot/docker_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bam/docker_utils.py
+# docker_utils.py
 import os
 import docker
 from tqdm import tqdm
 
 def build_image(container_dir):
     """Build a Docker image for an AI agent"""
     docker_client = docker.from_env()
@@ -10,30 +10,42 @@
     return image
 
 def create_docker_container(container_name, env_vars=None):
     """Create a Docker container for an AI agent"""
     docker_client = docker.from_env()
     container = docker_client.containers.create(
         f"{container_name}:latest",
-        detach=True,
         name=container_name,
-        environment=env_vars
+        environment=env_vars,
+        detach=True,
+        tty=True,
+        stdin_open=True,
+        ports={'1337/tcp': ('127.0.0.1', 1337)},
     )
     return container
 
-def prune_system():
+def prune_system(progress_bar=None):
     """Prune Docker system resources"""
     docker_client = docker.from_env()
-    with tqdm(total=4, desc="Pruning system resources") as pbar:
-        docker_client.containers.prune()
-        pbar.update(1)
-        docker_client.images.prune()
-        pbar.update(1)
-        docker_client.networks.prune()
-        pbar.update(1)
-        docker_client.volumes.prune()
-        pbar.update(1)
+    tasks = [
+        docker_client.containers.prune,
+        docker_client.images.prune,
+        docker_client.networks.prune,
+        docker_client.volumes.prune,
+    ]
+    if progress_bar:
+        for task in tasks:
+            task()
+            progress_bar.update(1)
+    else:
+        with tqdm(total=4, desc="Pruning system resources") as pbar:
+            for task in tasks:
+                task()
+                pbar.update(1)
 
-def list_containers():
-    """List all Docker containers"""
+def list_apps(prefix=""):
+    """List all Bam apps"""
     docker_client = docker.from_env()
-    return docker_client.containers.list(all=True)
+    containers = docker_client.containers.list(all=True)
+    if prefix:
+        containers = [c for c in containers if c.name.startswith(prefix)]
+    return containers
```

### Comparing `bambot-0.4.1/bambot/templates/langchain_template.py` & `bambot-0.4.2/bambot/templates/langchain_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bam/templates/langchain_template.py
+# bambot/templates/langchain_template.py
 from langchain import OpenAI, ConversationChain
 
 class Agent:
     def __init__(self):
         self.llm = OpenAI(temperature=0)
         self.conversation = ConversationChain(llm=self.llm)
```

### Comparing `bambot-0.4.1/bambot.egg-info/PKG-INFO` & `bambot-0.4.2/bambot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Containers for AI agents
 Home-page: https://github.com/Bam-Corp/bambot
 Author: Bam Corp
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: docker
-Requires-Dist: prometheus-client
-Requires-Dist: streamlit
 Requires-Dist: tqdm
 Requires-Dist: python-dotenv
 
 # Bam
 
 [![PyPI version](https://badge.fury.io/py/bambot.svg)](https://badge.fury.io/py/bambot)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -45,19 +43,19 @@
 
 1. Install bambot using pip:
 ```bash
 pip install bambot
 ```
 2. Create a new AI agent container:
 ```bash
-bam create container
+bam app create
 ```
-3. Run the AI agent container:
+3. Run the AI agent container locally:
 ```bash
-bam run
+bam app run
 ```
 
 That's it! You're now ready to start using Bam to create and run AI agent containers.
 
 ## Documentation
 
 For detailed documentation and additional features, please visit our website at [bam.bot](https://bam.bot) (coming soon).
```

### Comparing `bambot-0.4.1/bambot.egg-info/SOURCES.txt` & `bambot-0.4.2/bambot.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 README.md
 setup.py
 bambot/__init__.py
+bambot/app.py
 bambot/cli.py
-bambot/container.py
 bambot/docker_utils.py
-bambot/logging.py
-bambot/metrics.py
-bambot/prometheus.py
-bambot/streamlit_dashboard.py
 bambot.egg-info/PKG-INFO
 bambot.egg-info/SOURCES.txt
 bambot.egg-info/dependency_links.txt
 bambot.egg-info/entry_points.txt
 bambot.egg-info/requires.txt
 bambot.egg-info/top_level.txt
 bambot/templates/Dockerfile
+bambot/templates/agent_runner.py
 bambot/templates/agent_template.py
 bambot/templates/langchain_template.py
-bambot/templates/main.py
 bambot/templates/requirements.txt
+bambot/templates/server.py
 tests/test_cli.py
 tests/test_container.py
 tests/test_docker.py
 tests/test_logging.py
 tests/test_metrics.py
 tests/test_prometheus.py
 tests/test_streamlit_dashboard.py
```

### Comparing `bambot-0.4.1/setup.py` & `bambot-0.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bambot",
-    version="0.4.1",
+    version="0.4.2",
     author="Bam Corp",
     author_email="spencer@bam.bot",
     description="Containers for AI agents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bam-Corp/bambot",
     packages=find_packages(),
     package_data={'bambot': ['templates/*']},
-    install_requires=["click", "docker", "prometheus-client", "streamlit", "tqdm", "python-dotenv"],
+    install_requires=["click", "docker", "tqdm", "python-dotenv"],
     entry_points={
         "console_scripts": ["bam=bambot.cli:main"]
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

