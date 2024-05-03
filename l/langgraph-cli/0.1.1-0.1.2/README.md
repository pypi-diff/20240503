# Comparing `tmp/langgraph_cli-0.1.1.tar.gz` & `tmp/langgraph_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_cli-0.1.1.tar", max compression
+gzip compressed data, was "langgraph_cli-0.1.2.tar", max compression
```

## Comparing `langgraph_cli-0.1.1.tar` & `langgraph_cli-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.1/langgraph_cli/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-02 17:41:43.798531 langgraph_cli-0.1.1/langgraph_cli/cli.py
--rw-r--r--   0        0        0     2738 2024-05-02 00:35:49.773352 langgraph_cli-0.1.1/langgraph_cli/config.py
--rw-r--r--   0        0        0     1609 2024-05-02 20:46:38.017185 langgraph_cli-0.1.1/langgraph_cli/docker.py
--rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.1/langgraph_cli/initdb/init.sql
--rw-r--r--   0        0        0     1024 2024-05-02 20:47:24.787936 langgraph_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.772511 langgraph_cli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:35:49.772849 langgraph_cli-0.1.2/langgraph_cli/__init__.py
+-rw-r--r--   0        0        0     6293 2024-05-02 22:28:25.526691 langgraph_cli-0.1.2/langgraph_cli/cli.py
+-rw-r--r--   0        0        0     4266 2024-05-02 22:22:39.743107 langgraph_cli-0.1.2/langgraph_cli/config.py
+-rw-r--r--   0        0        0     1609 2024-05-02 20:46:38.017185 langgraph_cli-0.1.2/langgraph_cli/docker.py
+-rw-r--r--   0        0        0       39 2024-05-02 00:35:49.772817 langgraph_cli-0.1.2/langgraph_cli/initdb/init.sql
+-rw-r--r--   0        0        0     1024 2024-05-02 22:28:50.231701 langgraph_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 langgraph_cli-0.1.2/PKG-INFO
```

### Comparing `langgraph_cli-0.1.1/langgraph_cli/cli.py` & `langgraph_cli-0.1.2/langgraph_cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,58 +63,83 @@
             t.cancel()
         for d in done:
             if exc := d.exception():
                 exceptions.append(exc)
 
 
 OPT_O = click.option(
-    "--override",
-    "-o",
+    "--docker-compose",
+    "-d",
+    help="Advanced: Path to docker-compose.yml file with additional services to launch",
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=False,
         resolve_path=True,
         path_type=pathlib.Path,
     ),
 )
 OPT_C = click.option(
     "--config",
     "-c",
+    help="""Path to configuration file declaring dependencies, graphs and environment variables.
+    
+    \b
+    Example:
+    {
+        "dependencies": [
+            "langchain_openai",
+            "./your_package"
+        ],
+        "graphs": {
+            "my_graph_id": "./your_package/your_file.py:variable"
+        },
+        "env": "./.env"
+    }
+
+    Defaults to looking for langgraph.json in the current directory.""",
+    default="langgraph.json",
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=False,
         resolve_path=True,
         path_type=pathlib.Path,
     ),
 )
-OPT_PORT = click.option("--port", "-p", type=int, default=8123)
+OPT_PORT = click.option(
+    "--port", "-p", type=int, default=8123, show_default=True, help="Port to expose"
+)
 
 
 @click.group()
 def cli():
     pass
 
 
+@click.option(
+    "--recreate/--no-recreate",
+    default=False,
+    show_default=True,
+    help="Clear previous data",
+)
+@click.option(
+    "--pull/--no-pull", default=True, show_default=True, help="Pull latest images"
+)
+@OPT_PORT
 @OPT_O
 @OPT_C
-@OPT_PORT
-@click.option("--recreate", is_flag=True, default=False)
-@click.option("--pull", is_flag=True, default=False)
-@cli.command()
+@cli.command(help="Start langgraph API server")
 def up(
-    override: Optional[pathlib.Path],
-    config: Optional[pathlib.Path],
+    config: pathlib.Path,
+    docker_compose: Optional[pathlib.Path],
     port: int,
     recreate: bool,
     pull: bool,
 ):
-    if not override and not config:
-        raise click.UsageError("Must provide either --override or --config")
     with asyncio.Runner() as runner:
         # check docker available
         try:
             runner.run(exec("docker", "--version"))
             runner.run(exec("docker", "compose", "version"))
         except click.exceptions.Exit:
             click.echo("Docker not installed or not running")
@@ -122,21 +147,21 @@
         # pull latest images
         if pull:
             runner.run(exec("docker", "pull", "langchain/langserve"))
         # prepare args
         stdin = langgraph_cli.docker.compose(port=port)
         args = [
             "--project-directory",
-            override.parent if override else config.parent,
+            config.parent,
             "-f",
             "-",  # stdin
         ]
         # apply options
-        if override:
-            args.extend(["-f", str(override)])
+        if docker_compose:
+            args.extend(["-f", str(docker_compose)])
         args.append("up")
         if config:
             with open(config) as f:
                 stdin += langgraph_cli.config.config_to_compose(config, json.load(f))
         if recreate:
             args.extend(["--force-recreate", "--remove-orphans"])
             shutil.rmtree(".langserve-data", ignore_errors=True)
```

### Comparing `langgraph_cli-0.1.1/langgraph_cli/config.py` & `langgraph_cli-0.1.2/langgraph_cli/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,57 +8,86 @@
     dependencies: list[str]
     graphs: dict[str, str]
     env: Union[dict[str, str], str]
 
 
 def config_to_compose(config_path: pathlib.Path, config: Config):
     pypi_deps = [dep for dep in config["dependencies"] if not dep.startswith(".")]
-    local_pkgs = []
-    faux_pkgs = {}
-    locals_set = set()
+    local_pkgs: dict[pathlib.Path, str] = {}
+    faux_pkgs: dict[pathlib.Path, str] = {}
+    pkg_names = set()
 
     for local_dep in config["dependencies"]:
         if local_dep.startswith("."):
             resolved = config_path.parent / local_dep
 
             # validate local dependency
             if not resolved.exists():
                 raise FileNotFoundError(f"Could not find local dependency: {resolved}")
             elif not resolved.is_dir():
                 raise NotADirectoryError(
                     f"Local dependency must be a directory: {resolved}"
                 )
-            elif resolved.name in locals_set:
+            elif resolved.name in pkg_names:
                 raise ValueError(f"Duplicate local dependency: {resolved}")
             else:
-                locals_set.add(resolved.name)
+                pkg_names.add(resolved.name)
 
             # if it's installable, add it to local_pkgs
             # otherwise, add it to faux_pkgs, and create a pyproject.toml
             files = os.listdir(resolved)
             if "pyproject.toml" in files:
-                local_pkgs.append(local_dep)
+                local_pkgs[resolved] = local_dep
             elif "setup.py" in files:
-                local_pkgs.append(local_dep)
+                local_pkgs[resolved] = local_dep
             else:
-                faux_pkgs[resolved.name] = local_dep
+                faux_pkgs[resolved] = local_dep
 
-    for _, import_str in config["graphs"].items():
-        module_str, _, attrs_str = import_str.partition(":")
-        if not module_str or not attrs_str:
+    for graph_id, import_str in config["graphs"].items():
+        module_str, _, attr_str = import_str.partition(":")
+        if not module_str or not attr_str:
             message = (
                 'Import string "{import_str}" must be in format "<module>:<attribute>".'
             )
             raise ValueError(message.format(import_str=import_str))
+        if module_str.startswith("."):
+            resolved = config_path.parent / module_str
+            if not resolved.exists():
+                raise FileNotFoundError(f"Could not find local module: {resolved}")
+            elif not resolved.is_file():
+                raise IsADirectoryError(f"Local module must be a file: {resolved}")
+            else:
+                for local_pkg in local_pkgs:
+                    if resolved.is_relative_to(local_pkg):
+                        resolved = resolved.relative_to(local_pkg)
+                        break
+                else:
+                    for faux_pkg in faux_pkgs:
+                        if resolved.is_relative_to(faux_pkg):
+                            resolved = resolved.relative_to(faux_pkg.parent)
+                            break
+                    else:
+                        raise ValueError(
+                            f"Module '{import_str}' not found in 'dependencies' list"
+                            "Add its containing package to 'dependencies' list."
+                        )
+            # rewrite module_str to be a python import path
+            module_str = f"{'.'.join(resolved.parts[:-1])}"
+            if resolved.stem == "__init__":
+                pass
+            else:
+                module_str = f"{module_str}.{resolved.stem}"
+            # update the config
+            config["graphs"][graph_id] = f"{module_str}:{attr_str}"
 
     faux_pkgs_str = "\n\n".join(
-        f"ADD {path} /tmp/{name}/{name}\n                RUN touch /tmp/{name}/pyproject.toml"
-        for name, path in faux_pkgs.items()
+        f"ADD {relpath} /tmp/{fullpath.name}/{fullpath.name}\n                RUN touch /tmp/{fullpath.name}/pyproject.toml"
+        for fullpath, relpath in faux_pkgs.items()
     )
-    local_pkgs_str = f"ADD {' '.join(local_pkgs)} /tmp/" if local_pkgs else ""
+    local_pkgs_str = f"ADD {' '.join(local_pkgs.values())} /tmp/" if local_pkgs else ""
     env_vars_str = (
         "\n".join(f"            {k}: {v}" for k, v in config["env"].items())
         if isinstance(config["env"], dict)
         else ""
     )
     env_file_str = (
         f"env_file: {config['env']}" if isinstance(config["env"], str) else ""
```

### Comparing `langgraph_cli-0.1.1/langgraph_cli/docker.py` & `langgraph_cli-0.1.2/langgraph_cli/docker.py`

 * *Files identical despite different names*

### Comparing `langgraph_cli-0.1.1/pyproject.toml` & `langgraph_cli-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_cli"}]
 
 [tool.poetry.scripts]
 langgraph = "langgraph_cli.cli:cli"
```

