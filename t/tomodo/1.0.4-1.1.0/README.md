# Comparing `tmp/tomodo-1.0.4.tar.gz` & `tmp/tomodo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodo-1.0.4.tar", max compression
+gzip compressed data, was "tomodo-1.1.0.tar", max compression
```

## Comparing `tomodo-1.0.4.tar` & `tomodo-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1099 2024-03-25 06:13:25.429454 tomodo-1.0.4/LICENSE
--rw-r--r--   0        0        0     8977 2024-03-25 06:13:25.429454 tomodo-1.0.4/README.md
--rw-r--r--   0        0        0     1121 2024-03-25 06:13:25.429454 tomodo-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      381 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/cli/__init__.py
--rw-r--r--   0        0        0     8560 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/cli/provision.py
--rw-r--r--   0        0        0      828 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/cli/tags.py
--rw-r--r--   0        0        0     9896 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/cmd.py
--rw-r--r--   0        0        0        1 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/__init__.py
--rw-r--r--   0        0        0     5611 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/cleaner.py
--rw-r--r--   0        0        0     1849 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/config.py
--rw-r--r--   0        0        0      678 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/errors.py
--rw-r--r--   0        0        0    19045 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/models.py
--rw-r--r--   0        0        0    22442 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/provisioner.py
--rw-r--r--   0        0        0     5504 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/reader.py
--rw-r--r--   0        0        0     2269 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/starter.py
--rw-r--r--   0        0        0     4630 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/tag_manager.py
--rw-r--r--   0        0        0     6920 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/common/util.py
--rw-r--r--   0        0        0     8240 2024-03-25 06:13:25.433454 tomodo-1.0.4/tomodo/functional.py
--rw-r--r--   0        0        0     9954 1970-01-01 00:00:00.000000 tomodo-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-05-03 08:20:52.919956 tomodo-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9352 2024-05-03 08:20:52.919956 tomodo-1.1.0/README.md
+-rw-r--r--   0        0        0     1121 2024-05-03 08:20:52.919956 tomodo-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      381 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/cli/__init__.py
+-rw-r--r--   0        0        0     8964 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/cli/provision.py
+-rw-r--r--   0        0        0      828 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/cli/tags.py
+-rw-r--r--   0        0        0     9896 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/cmd.py
+-rw-r--r--   0        0        0        1 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/__init__.py
+-rw-r--r--   0        0        0     5611 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/cleaner.py
+-rw-r--r--   0        0        0     1909 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/config.py
+-rw-r--r--   0        0        0      678 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/errors.py
+-rw-r--r--   0        0        0    19045 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/models.py
+-rw-r--r--   0        0        0    22658 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/provisioner.py
+-rw-r--r--   0        0        0     5504 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/reader.py
+-rw-r--r--   0        0        0     2269 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/starter.py
+-rw-r--r--   0        0        0     4630 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/tag_manager.py
+-rw-r--r--   0        0        0     6920 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/common/util.py
+-rw-r--r--   0        0        0     8954 2024-05-03 08:20:52.923956 tomodo-1.1.0/tomodo/functional.py
+-rw-r--r--   0        0        0    10329 1970-01-01 00:00:00.000000 tomodo-1.1.0/PKG-INFO
```

### Comparing `tomodo-1.0.4/LICENSE` & `tomodo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/README.md` & `tomodo-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 # tomodo
 
 **tomodo** is a Toolbox for MongoDB on Docker.
 
 -------
 
-Use it to create and manage Docker-based MongoDB community deployments - standalone instances, replica sets,
-and sharded clusters.
+Use it to create and manage Docker-based MongoDB community deployments - standalone instances, replica sets, sharded clusters, and local Atlas deployments.
 
 * [Installation](#installation)
     + [Install with Homebrew](#install-with-homebrew)
     + [Install with pip](#install-with-pip)
     + [Install from Source](#install-from-source)
         - [Install with Poetry Package Manager for Python](#install-with-poetry-package-manager-for-python)
         - [Install from source with pip](#install-from-source-with-pip)
@@ -29,14 +28,15 @@
     + [Describe Deployments](#describe-deployments)
     + [List Deployments](#list-deployments)
     + [Stop Deployments](#stop-deployments)
     + [Start Deployments](#start-deployments)
     + [Remove Deployments](#remove-deployments)
     + [List Image Tags](#list-tags)
 * [Programmatic Usage](#programmatic-usage)
+* [Disclaimer](#disclaimer)
 
 --- 
 
 ## Installation
 
 ### Install with Homebrew
 
@@ -316,7 +316,13 @@
 
 # List all deployments:
 deployments: Dict = tfunc.list_deployments(include_stopped=True)
 for name in deployments.keys():
     deployment: Deployment = deployments[name]
     print(f"Deployment {name} is {deployment.last_known_state}")
 ```
+
+##  Disclaimer
+This software is not supported by MongoDB, Inc. under any of their commercial support subscriptions or otherwise.
+Any usage of tomodo is at your own risk. Bug reports, feature requests, and questions can be posted in the
+[Issues section](https://github.com/yuviherziger/tomodo/issues) of this repository.
+
```

### Comparing `tomodo-1.0.4/pyproject.toml` & `tomodo-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodo"
-version = "1.0.4"
+version = "1.1.0"
 description = "A CLI for managing MongoDB deployments on Docker"
 authors = ["MongoDB PS <yuvi.herziger@mongodb.com>"]
 readme = "README.md"
 homepage = "https://github.com/yuviherziger/tomodo"
 repository = "https://github.com/yuviherziger/tomodo"
 packages = [{ include = "tomodo" }]
 license = "MIT"
```

### Comparing `tomodo-1.0.4/tomodo/cli/provision.py` & `tomodo-1.1.0/tomodo/cli/provision.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 def _name() -> str:
     return typer.Option(
         default=None,
         help="The deployment's name; auto-generated if not provided"
     )
 
 
+def _ephemeral() -> bool:
+    return typer.Option(
+        default=False,
+        help="Whether the deployment should be ephemeral and not persist data. All data is lost when the "
+             "deployment stops"
+    )
+
+
 def _port() -> int:
     return typer.Option(
         default=27017,
         min=0,
         max=65535,
         help="The deployment's start port"
     )
@@ -98,23 +106,24 @@
         auth_roles: str = typer.Option(
             default="dbAdminAnyDatabase readWriteAnyDatabase userAdminAnyDatabase clusterAdmin",
             help="Default authentication roles (currently ignored)"
         ),
         image_repo: str = _image_repo(),
         image_tag: str = _image_tag(),
         port: int = _port(),
+        ephemeral: bool = _ephemeral(),
         network_name: str = _network_name()
 
 ):
     check_docker()
     config = ProvisionerConfig(
         standalone=True, name=name, port=port,
         auth=auth, username=username, password=password, auth_db=auth_db,
         auth_roles=auth_roles.split(" "), image_repo=image_repo, image_tag=image_tag,
-        network_name=network_name
+        network_name=network_name, ephemeral=ephemeral
     )
     _provision(config=config)
 
 
 @cli.command(
     help="Provision a MongoDB replica set deployment"
 )
@@ -151,23 +160,24 @@
         ),
         auth_roles: str = typer.Option(
             default="dbAdminAnyDatabase readWriteAnyDatabase userAdminAnyDatabase clusterAdmin",
             help="Default authentication roles (currently ignored)"
         ),
         image_repo: str = _image_repo(),
         image_tag: str = _image_tag(),
+        ephemeral: bool = _ephemeral(),
         network_name: str = _network_name()
 ):
     check_docker()
     config = ProvisionerConfig(
         replica_set=True, replicas=int(replicas.value),
         arbiter=arbiter, name=name, priority=priority, port=port,
         auth=auth, username=username, password=password, auth_db=auth_db,
         auth_roles=auth_roles.split(" "), image_repo=image_repo, image_tag=image_tag,
-        network_name=network_name
+        network_name=network_name, ephemeral=ephemeral
     )
     _provision(config=config)
 
 
 @cli.command(
     help="Provision a MongoDB sharded cluster"
 )
@@ -217,24 +227,25 @@
         ),
         auth_roles: str = typer.Option(
             default="dbAdminAnyDatabase readWriteAnyDatabase userAdminAnyDatabase clusterAdmin",
             help="Default authentication roles (currently ignored)"
         ),
         image_repo: str = _image_repo(),
         image_tag: str = _image_tag(),
+        ephemeral: bool = _ephemeral(),
         network_name: str = _network_name()
 ):
     check_docker()
     config = ProvisionerConfig(
         replicas=int(replicas.value), shards=shards,
         arbiter=arbiter, name=name, priority=priority,
         sharded=True, port=port, config_servers=config_servers, mongos=mongos,
         auth=auth, username=username, password=password, auth_db=auth_db,
         auth_roles=auth_roles.split(" "), image_repo=image_repo, image_tag=image_tag,
-        network_name=network_name
+        network_name=network_name, ephemeral=ephemeral
     )
     _provision(config=config)
 
 
 @cli.command(
     help="Provision a local MongoDB Atlas deployment"
 )
```

### Comparing `tomodo-1.0.4/tomodo/cli/tags.py` & `tomodo-1.1.0/tomodo/cli/tags.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/cmd.py` & `tomodo-1.1.0/tomodo/cmd.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/cleaner.py` & `tomodo-1.1.0/tomodo/common/cleaner.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/config.py` & `tomodo-1.1.0/tomodo/common/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class ProvisionerConfig:
 
     def __init__(self, standalone: bool = False, replica_set: bool = False, replicas: int = 3, shards: int = 2,
                  arbiter: bool = False, name: str = None, priority: bool = False, atlas: bool = False,
                  sharded: bool = False, port: int = 27017, config_servers: int = 1, mongos: int = 1,
                  auth: bool = False, username: str = None, password: str = None, auth_db: str = "admin",
                  auth_roles: List[str] = None, image_repo: str = "mongo", image_tag: str = "latest",
-                 network_name: str = "mongo_network", atlas_version: str = None):
+                 network_name: str = "mongo_network", atlas_version: str = None, ephemeral: bool = False):
         self.standalone = standalone
         self.replica_set = replica_set
         self.replicas = replicas
         self.atlas = atlas
         self.shards = shards
         self.arbiter = arbiter
         self.name = name or get_random_name(combo=[ADJECTIVES, ANIMALS], separator="-", style="lowercase")
@@ -33,11 +33,12 @@
         self.auth_db = auth_db
         self.auth_roles = auth_roles or ["dbAdminAnyDatabase", "readWriteAnyDatabase", "userAdminAnyDatabase",
                                          "clusterAdmin"]
         self.image_repo = image_repo
         self.image_tag = image_tag
         self.network_name = network_name
         self.atlas_version = atlas_version
+        self.ephemeral = ephemeral
 
     @property
     def is_auth_enabled(self) -> bool:
         return self.username is not None and self.password is not None
```

### Comparing `tomodo-1.0.4/tomodo/common/errors.py` & `tomodo-1.1.0/tomodo/common/errors.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/models.py` & `tomodo-1.1.0/tomodo/common/models.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/provisioner.py` & `tomodo-1.1.0/tomodo/common/provisioner.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,34 +421,37 @@
                 "tomodo-shard-count": str(self.config.shards or 0),
             }
         )
 
     def create_mongod_container(self, port: int, name: str, replset_name: str = None,
                                 config_svr: bool = False, sh_cluster: bool = False, shard_id: int = 0,
                                 arbiter: bool = False) -> Container:
-        data_dir_name = f"data/{name}-db"
-        data_dir_path = os.path.join(DATA_FOLDER, data_dir_name)
-        os.makedirs(data_dir_path, exist_ok=True)
-        host_path = os.path.abspath(data_dir_path)
-        container_path = f"/{data_dir_name}"
-        mounts = [Mount(
-            target=container_path, source=host_path, type="bind"
-        )]
-
         repo = self.config.image_repo
         tag = self.config.image_tag
         image = f"{repo}:{tag}"
         logger.info("Creating container from '%s'. Port %d will be exposed to your host", image, port)
+        host_path = ""
+        container_path = ""
+        mounts = []
         command = [
             "mongod",
             "--bind_ip_all",
             "--port", str(port),
-            "--dbpath", container_path,
-            "--logpath", f"{container_path}/mongod.log"
         ]
+        if not self.config.ephemeral:
+            data_dir_name = f"data/{name}-db"
+            data_dir_path = os.path.join(DATA_FOLDER, data_dir_name)
+            os.makedirs(data_dir_path, exist_ok=True)
+            host_path = os.path.abspath(data_dir_path)
+            container_path = f"/{data_dir_name}"
+            mounts = [Mount(
+                target=container_path, source=host_path, type="bind"
+            )]
+            command.extend(["--dbpath", container_path, "--logpath", f"{container_path}/mongod.log"])
+
         environment = []
         if self.config.username and self.config.password:
             keyfile_path = os.path.abspath(f"{DATA_FOLDER}/mongo_keyfile")
             environment = [f"MONGO_INITDB_ROOT_USERNAME={self.config.username}",
                            f"MONGO_INITDB_ROOT_PASSWORD={self.config.password}"]
 
             if not os.path.isfile(keyfile_path):
@@ -496,15 +499,16 @@
                 "tomodo-port": str(port),
                 "tomodo-role": "cfg-svr" if config_svr else "rs-member" if replset_name else "standalone",
                 "tomodo-type": deployment_type,
                 "tomodo-data-dir": host_path,
                 "tomodo-container-data-dir": container_path,
                 "tomodo-shard-id": str(shard_id),
                 "tomodo-shard-count": str(self.config.shards or 0),
-                "tomodo-arbiter": str(int(arbiter))
+                "tomodo-arbiter": str(int(arbiter)),
+                "tomodo-ephemeral": str(int(self.config.ephemeral))
             }
         ), host_path, container_path
 
     def get_network(self) -> Network:
         networks = self.docker_client.networks.list(filters={"name": self.config.network_name})
         if len(networks) > 0:
             network = networks[0]
```

### Comparing `tomodo-1.0.4/tomodo/common/reader.py` & `tomodo-1.1.0/tomodo/common/reader.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/starter.py` & `tomodo-1.1.0/tomodo/common/starter.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/tag_manager.py` & `tomodo-1.1.0/tomodo/common/tag_manager.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/common/util.py` & `tomodo-1.1.0/tomodo/common/util.py`

 * *Files identical despite different names*

### Comparing `tomodo-1.0.4/tomodo/functional.py` & `tomodo-1.1.0/tomodo/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,43 +6,47 @@
 
 def provision_standalone_instance(name: str = None,
                                   port: int = 27017,
                                   auth: bool = False, username: str = None, password: str = None,
                                   auth_db: str = "admin",
                                   auth_roles: List[str] = None, image_repo: str = "mongo",
                                   image_tag: str = "latest",
-                                  network_name: str = "mongo_network") -> Mongod:
+                                  network_name: str = "mongo_network",
+                                  ephemeral: bool = False) -> Mongod:
     """
     Provisions and returns a standalone instance of MongoDB
 
     :param name:            The deployment's name; auto-generated if not provided
     :param port:            The deployment port
     :param auth:            Whether to enable authentication
     :param username:        Optional authentication username
     :param password:        Optional authentication password
     :param auth_db:         Authorization DB (currently ignored)
     :param auth_roles:      Default authentication roles (currently ignored)
     :param image_repo:      The MongoDB image name/repo
     :param image_tag:       The MongoDB image tag, which determines the MongoDB version to install
     :param network_name:    The Docker network to provision the deployment in; will create a new one or use an existing
                             one with the same name if such network exists
+    :param ephemeral:       Whether the deployment should be ephemeral and not persist data. All data is lost when the
+                            deployment stops
     :return:                Mongod instance
     """
     config = ProvisionerConfig(
         standalone=True,
         name=name,
         port=port,
         auth=auth,
         username=username,
         password=password,
         auth_db=auth_db,
         auth_roles=auth_roles,
         image_repo=image_repo,
         image_tag=image_tag,
-        network_name=network_name
+        network_name=network_name,
+        ephemeral=ephemeral
     )
     provisioner = Provisioner(config=config)
     reader = Reader()
     return provisioner.provision(deployment_getter=reader.get_deployment_by_name)
 
 
 def provision_atlas_instance(name: str = None,
@@ -80,15 +84,16 @@
     reader = Reader()
     return provisioner.provision(deployment_getter=reader.get_deployment_by_name)
 
 
 def provision_replica_set(replicas: int = 3, arbiter: bool = False, name: str = None, priority: bool = False,
                           port: int = 27017, auth: bool = False, username: str = None, password: str = None,
                           auth_db: str = "admin", auth_roles: List[str] = None, image_repo: str = "mongo",
-                          image_tag: str = "latest", network_name: str = "mongo_network") -> ReplicaSet:
+                          image_tag: str = "latest", network_name: str = "mongo_network",
+                          ephemeral: bool = False) -> ReplicaSet:
     """
     Provisions and returns a replica set instance of MongoDB
 
     :param replicas:        The number of replica set nodes to provision
     :param arbiter:         Add an arbiter node to a replica set
     :param name:            The deployment's name; auto-generated if not provided
     :param priority:        Priority (currently ignored)
@@ -98,14 +103,16 @@
     :param password:        Admin password
     :param auth_db:         Authorization DB (currently ignored)
     :param auth_roles:      Default authentication roles (currently ignored)
     :param image_repo:      The MongoDB image name/repo
     :param image_tag:       The MongoDB image tag, which determines the MongoDB version to install
     :param network_name:    The Docker network to provision the deployment in; will create a new one or use an existing
                             one with the same name if such network exists
+    :param ephemeral:       Whether the deployment should be ephemeral and not persist data. All data is lost when the
+                            deployment stops
     :return:                ReplicaSet instance
     """
     config = ProvisionerConfig(
         replica_set=True,
         replicas=replicas,
         arbiter=arbiter,
         name=name,
@@ -114,27 +121,28 @@
         auth=auth,
         username=username,
         password=password,
         auth_db=auth_db,
         auth_roles=auth_roles,
         image_repo=image_repo,
         image_tag=image_tag,
-        network_name=network_name
+        network_name=network_name,
+        ephemeral=ephemeral
     )
     provisioner = Provisioner(config=config)
     reader = Reader()
     return provisioner.provision(deployment_getter=reader.get_deployment_by_name)
 
 
 def provision_sharded_cluster(replicas: int = 3, shards: int = 2,
                               arbiter: bool = False, name: str = None, priority: bool = False,
                               port: int = 27017, config_servers: int = 1, mongos: int = 1,
                               auth: bool = False, username: str = None, password: str = None, auth_db: str = "admin",
                               auth_roles: List[str] = None, image_repo: str = "mongo", image_tag: str = "latest",
-                              network_name: str = "mongo_network") -> ShardedCluster:
+                              network_name: str = "mongo_network", ephemeral: bool = False) -> ShardedCluster:
     """
     Provisions and returns a sharded cluster instance of MongoDB
 
     :param replicas:
     :param shards:
     :param arbiter:
     :param name:
@@ -146,14 +154,16 @@
     :param username:
     :param password:
     :param auth_db:
     :param auth_roles:
     :param image_repo:
     :param image_tag:
     :param network_name:
+    :param ephemeral:       Whether the deployment should be ephemeral and not persist data. All data is lost when the
+                            deployment stops
     :return:
     """
     config = ProvisionerConfig(
         sharded=True,
         replicas=replicas,
         shards=shards,
         config_servers=config_servers,
@@ -165,15 +175,16 @@
         auth=auth,
         username=username,
         password=password,
         auth_db=auth_db,
         auth_roles=auth_roles,
         image_repo=image_repo,
         image_tag=image_tag,
-        network_name=network_name
+        network_name=network_name,
+        ephemeral=ephemeral
     )
     provisioner = Provisioner(config=config)
     reader = Reader()
     return provisioner.provision(deployment_getter=reader.get_deployment_by_name)
 
 
 def get_deployment(name: str, include_stopped: bool = True) -> Union[Mongod, ReplicaSet, ShardedCluster]:
```

### Comparing `tomodo-1.0.4/PKG-INFO` & `tomodo-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodo
-Version: 1.0.4
+Version: 1.1.0
 Summary: A CLI for managing MongoDB deployments on Docker
 Home-page: https://github.com/yuviherziger/tomodo
 License: MIT
 Keywords: mongodb,docker,upgrade,python,cli
 Author: MongoDB PS
 Author-email: yuvi.herziger@mongodb.com
 Requires-Python: >=3.8,<3.13
@@ -36,16 +36,15 @@
 
 # tomodo
 
 **tomodo** is a Toolbox for MongoDB on Docker.
 
 -------
 
-Use it to create and manage Docker-based MongoDB community deployments - standalone instances, replica sets,
-and sharded clusters.
+Use it to create and manage Docker-based MongoDB community deployments - standalone instances, replica sets, sharded clusters, and local Atlas deployments.
 
 * [Installation](#installation)
     + [Install with Homebrew](#install-with-homebrew)
     + [Install with pip](#install-with-pip)
     + [Install from Source](#install-from-source)
         - [Install with Poetry Package Manager for Python](#install-with-poetry-package-manager-for-python)
         - [Install from source with pip](#install-from-source-with-pip)
@@ -54,14 +53,15 @@
     + [Describe Deployments](#describe-deployments)
     + [List Deployments](#list-deployments)
     + [Stop Deployments](#stop-deployments)
     + [Start Deployments](#start-deployments)
     + [Remove Deployments](#remove-deployments)
     + [List Image Tags](#list-tags)
 * [Programmatic Usage](#programmatic-usage)
+* [Disclaimer](#disclaimer)
 
 --- 
 
 ## Installation
 
 ### Install with Homebrew
 
@@ -342,7 +342,13 @@
 # List all deployments:
 deployments: Dict = tfunc.list_deployments(include_stopped=True)
 for name in deployments.keys():
     deployment: Deployment = deployments[name]
     print(f"Deployment {name} is {deployment.last_known_state}")
 ```
 
+##  Disclaimer
+This software is not supported by MongoDB, Inc. under any of their commercial support subscriptions or otherwise.
+Any usage of tomodo is at your own risk. Bug reports, feature requests, and questions can be posted in the
+[Issues section](https://github.com/yuviherziger/tomodo/issues) of this repository.
+
+
```

