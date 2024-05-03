# Comparing `tmp/ibuilder-3.6.1.tar.gz` & `tmp/ibuilder-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibuilder-3.6.1.tar", max compression
+gzip compressed data, was "ibuilder-3.7.0.tar", max compression
```

## Comparing `ibuilder-3.6.1.tar` & `ibuilder-3.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.6.1/LICENSE
--rw-r--r--   0        0        0     5130 2024-04-05 09:24:54.705266 ibuilder-3.6.1/README.md
--rw-r--r--   0        0        0        0 2024-01-06 11:55:51.913157 ibuilder-3.6.1/ibuilder/__init__.py
--rw-r--r--   0        0        0       43 2024-01-06 11:55:51.916490 ibuilder-3.6.1/ibuilder/__main__.py
--rw-r--r--   0        0        0     4231 2024-01-06 11:55:51.919824 ibuilder-3.6.1/ibuilder/config/config.py
--rw-r--r--   0        0        0     2146 2024-04-09 15:47:47.718510 ibuilder-3.6.1/ibuilder/config/models.py
--rwxr-xr-x   0        0        0     6005 2024-04-05 09:31:38.769033 ibuilder-3.6.1/ibuilder/history.py
--rwxr-xr-x   0        0        0     3748 2024-01-06 12:03:11.386576 ibuilder-3.6.1/ibuilder/images.py
--rwxr-xr-x   0        0        0    13936 2024-04-05 09:40:19.536378 ibuilder-3.6.1/ibuilder/main.py
--rw-r--r--   0        0        0     1564 2024-04-05 09:15:56.066470 ibuilder-3.6.1/ibuilder/models.py
--rw-r--r--   0        0        0    15058 2024-01-06 11:55:51.909823 ibuilder-3.6.1/ibuilder/utils.py
--rw-r--r--   0        0        0      890 2024-04-09 15:39:16.076014 ibuilder-3.6.1/pyproject.toml
--rw-r--r--   0        0        0     6365 1970-01-01 00:00:00.000000 ibuilder-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.7.0/LICENSE
+-rw-r--r--   0        0        0     4939 2024-05-03 15:34:22.461724 ibuilder-3.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 15:21:59.571402 ibuilder-3.7.0/ibuilder/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-03 15:21:59.578069 ibuilder-3.7.0/ibuilder/__main__.py
+-rw-r--r--   0        0        0     4241 2024-05-03 15:21:59.581403 ibuilder-3.7.0/ibuilder/config/config.py
+-rw-r--r--   0        0        0     2135 2024-05-03 15:21:59.581403 ibuilder-3.7.0/ibuilder/config/models.py
+-rwxr-xr-x   0        0        0     5994 2024-05-03 15:21:59.584736 ibuilder-3.7.0/ibuilder/history.py
+-rwxr-xr-x   0        0        0     3737 2024-05-03 15:21:59.574736 ibuilder-3.7.0/ibuilder/images.py
+-rwxr-xr-x   0        0        0    13855 2024-05-03 15:35:06.469792 ibuilder-3.7.0/ibuilder/main.py
+-rw-r--r--   0        0        0     1553 2024-05-03 15:21:59.578069 ibuilder-3.7.0/ibuilder/models.py
+-rw-r--r--   0        0        0    15047 2024-05-03 15:21:59.568069 ibuilder-3.7.0/ibuilder/utils.py
+-rw-r--r--   0        0        0      863 2024-05-03 15:27:23.955065 ibuilder-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5954 1970-01-01 00:00:00.000000 ibuilder-3.7.0/PKG-INFO
```

### Comparing `ibuilder-3.6.1/LICENSE` & `ibuilder-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibuilder-3.6.1/README.md` & `ibuilder-3.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # README
 
 ibuilder is a [cli](https://en.wikipedia.org/wiki/Command-line_interface) based builder of [docker](https://hub.docker.com/) images. It provides an interface for building and pushing the image, signing images, as well as for tagging source code after build with a build version and other common image tasks.
 
 
 ### Latest Changes
 
-- upgrade to pydantic 2x
-- upgraded packages: docker, packaging, pydantic, rich, typer
-- changed --version to use importlib.metadata
-- removed capturing of sign_logs
-- turned off pretty_exceptions (typer/rich)
+- cleaned up version and config's usage of importlib.metadata and/or pkg_resources (removed pkg_resources)
+- change python version requirement from 3.8+ to 3.11+ (for speed and to leverage internal tomllib)
+- update copyright date
+- package updates: idna, pydantic, typer, typing-extensions
 
 
 ### NOTICES
 
-- __Next Release Will Require Python 3.11 or Newer__ as we would like to move away from tomllib to address the following:
-  + this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
+- version 1.0.0 requires python 3.11+ (for internal toml processing capabilities and its fast)
 
 
 ### Features
 
 - build: build docker images
 - push: push images to any container registry
 - sign: sign images for container signing and verification
 - source control: tag and push when you build an image
 - history: retain build history for quick/easy access to past build info
 - quick/easy: create an `ibuilder.toml` file and run `ib build -i minor` to build, push, commit to source control and sign a new image
 
+
 ### Requirements
 
 - python 3
 - docker: docker must be set up as it is used to build and push the image
 - git: (optional) if you use the source-tag feature you will need git installed and your code setup in git (it simply performs a git tag && git push from the working directory)
 - image signor: (optional) if you choose to sign images a signor (such as cosign) is needed
 
+
 ### Overview
 
 - setup (see #setup)
 - configure (see #configure): place a copy of the `example/.ibuilder.toml` in the same directory as your Dockerfile of the app you want to build and adjust it as needed
 - run (see #run): execute ibuilder to build/push/tag a version of your app, its as simple as `ib build`
 
 
@@ -73,14 +73,15 @@
 
 ### Recommendations
 
 We recommend using docker's configuration storage for reg_auth-* related configuration items as it encrypts sensitive information and is likely already configured (if you have already used `docker login`). If you leave the remaining items empty the default values will be used. This will then try `$HOME/.docker/config.json` and `$HOME/.dockercfg` for your docker config settings. If you do not already have a docker config run `docker login` and it should be created for you. After a successful login you should not need to do anything else for the application as the needed info will be stored in your dockercfg and the app will use it when needed.
 
 If you are signing your images you may want to set the `COSIGN_PASSWORD` environment variable in your `~/.bashrc` or equivalent shell config file to avoid being prompted for your signing password after build and push. It should be noted that you will be prompted twice (if you are pushing both the build version and the `latest` tag of this version) as ib signs both tags of the built image. To avoid this we recommend setting the `COSIGN_PASSWORD` environment variable but please ensure you understand the security implications of doing so.
 
+
 ### Legacy
 
 This project originally started under the name boi - builder of images and as such you may find references to boi and even backward support for boi (e.g. local history database, user config file, etc.).
 
 
 ### Links
```

### Comparing `ibuilder-3.6.1/ibuilder/config/config.py` & `ibuilder-3.7.0/ibuilder/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 import logging
 import sys
 from pathlib import Path
 
 import arrow
 import docker
-import pkg_resources
-import tomli
+import importlib.metadata as md
+import tomllib
 import typer
 from tinydb import TinyDB
 
 from ibuilder.config.models import Application, Project
 
 logger = logging.getLogger("default")
 
@@ -38,15 +38,15 @@
 def load_config(conf_file, ctype) -> dict:
     """
     Load config data from toml config file.
     """
 
     try:
         with open(conf_file, "rb") as f:
-            return ctype(**tomli.load(f))
+            return ctype(**tomllib.load(f))
 
     except FileNotFoundError as e:
         typer.secho(f"File [{conf_file}] not found: {e}", fg=typer.colors.RED, err=True)
         return None
     except Exception as e:
         typer.secho(
             f"Exception handling file [{conf_file}]: {e}", fg=typer.colors.RED, err=True
@@ -134,15 +134,17 @@
 
     else:
         typer.echo(f"- no project db, creating: {PRJ.config.dbpath}")
         open(PRJ.config.dbpath, "a").close()
         DB = TinyDB(PRJ.config.dbpath)
 
 
+APP_NAME = md.metadata("ibuilder")["Name"]
+APP_VERSION = md.metadata("ibuilder")["Version"]
 APP = Application(
-    name=pkg_resources.get_distribution("ibuilder").project_name,
-    version=pkg_resources.get_distribution("ibuilder").version,
+    name=APP_NAME,
+    version=APP_VERSION,
 )
 CALLING_PARAMS = " ".join(sys.argv[1:])
 DB = None
 PRJ = None
 RUNDTS = arrow.now("local").format("YYYY-MM-DD HH:mm:ss")
```

### Comparing `ibuilder-3.6.1/ibuilder/config/models.py` & `ibuilder-3.7.0/ibuilder/config/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 
 class Application(BaseModel):
```

### Comparing `ibuilder-3.6.1/ibuilder/history.py` & `ibuilder-3.7.0/ibuilder/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 from pprint import pformat
 
 import arrow
 import logging
 import typer
 from rich import box
```

### Comparing `ibuilder-3.6.1/ibuilder/images.py` & `ibuilder-3.7.0/ibuilder/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 import json
 import logging
 from base64 import b64decode
 from os import path
 
 import arrow
```

### Comparing `ibuilder-3.6.1/ibuilder/main.py` & `ibuilder-3.7.0/ibuilder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 import logging
 from datetime import datetime
 from os import getenv
 from typing import List, Optional
 
 import typer
@@ -13,14 +13,16 @@
 from rich.console import Console
 from tinydb import where
 
 import ibuilder.history
 import ibuilder.images
 from ibuilder.config.config import (
     APP,
+    APP_NAME,
+    APP_VERSION,
     CALLING_PARAMS,
     RUNDTS,
     get_db,
     get_docker_client,
     get_prj_conf,
     load_prj_conf,
 )
@@ -333,26 +335,25 @@
             f"Repushing from history created on [magenta]{r['created']}[/magenta] which was build version [magenta]{r['run_params']['build']['version']}[/magenta]"
         )
         _sign = False if no_sign else True
         logger.debug(f"- sign image flag is: {_sign}")
         image_repush(r, _sign)
 
 
+def get_version():
+    return f"{APP_NAME} {APP_VERSION}"
+
+
 def version_callback(value: bool):
     """
     Show version.
     """
 
-    import importlib.metadata
-
     if value:
-        _meta = importlib.metadata.metadata("ibuilder")
-        _name = _meta["Name"]
-        _version = _meta["Version"]
-        typer.echo(f"{_name} {_version}")
+        typer.echo(get_version())
         raise typer.Exit()
 
 
 @app.callback()
 def main(
     version: Optional[bool] = typer.Option(
         None,
```

### Comparing `ibuilder-3.6.1/ibuilder/models.py` & `ibuilder-3.7.0/ibuilder/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 from enum import Enum
 from typing import List
 
 from pydantic import BaseModel
 
 UNITS = {1000: ["KB", "MB", "GB"], 1024: ["KiB", "MiB", "GiB"]}
```

### Comparing `ibuilder-3.6.1/ibuilder/utils.py` & `ibuilder-3.7.0/ibuilder/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2023 drad <sa@adercon.com>
+#  Copyright 2024 dradux.com
 
 import logging
 import shutil
 import subprocess  # nosec
 from datetime import datetime
 from typing import List
```

### Comparing `ibuilder-3.6.1/pyproject.toml` & `ibuilder-3.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [internal]
 created = 2019-06-15
-modified = 2024-01-06
+modified = 2024-05-03
+
 
 [tool.poetry]
 name = "ibuilder"
-version = "3.6.1"
+version = "3.7.0"
 description = "build, tag, push, and sign docker images"
 authors = ["drad <sa@adercon.com>"]
 maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/ibuilder"
 repository = "https://gitlab.com/drad/ibuilder"
 keywords = ["cli", "docker", "containers", "build", "ci", "cd", "image", "tag", "git", "push", "sign", "cosign"]
 
+
 [tool.poetry.scripts]
 ib = "ibuilder.main:app"
 
+
 [tool.poetry.dependencies]
-python = "^3.8"
-arrow = "^1.3.0"
-click = "^8.1.7"
-docker = "^7.0.0"
+python = "^3.11"
+arrow = "^1.3"
+click = "^8.1"
+docker = "^7.0"
 packaging = "^24.0"
-pydantic = "^2.6.4"
-requests = "^2.31.0"
-rich = "^13.7.1"
-tinydb = "^4.8.0"
-tomli = "^2.0.1"
-typer = "^0.12.0"
+pydantic = "^2.6"
+requests = "^2.31"
+rich = "^13.7"
+tinydb = "^4.8"
+typer = "^0.12"
+
 
 [tool.poetry.dev-dependencies]
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ibuilder-3.6.1/PKG-INFO` & `ibuilder-3.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 Metadata-Version: 2.1
 Name: ibuilder
-Version: 3.6.1
+Version: 3.7.0
 Summary: build, tag, push, and sign docker images
 Home-page: https://gitlab.com/drad/ibuilder
 License: GPL-3.0-only
 Keywords: cli,docker,containers,build,ci,cd,image,tag,git,push,sign,cosign
 Author: drad
 Author-email: sa@adercon.com
 Maintainer: drad
 Maintainer-email: sa@adercon.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: arrow (>=1.3.0,<2.0.0)
-Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: docker (>=7.0.0,<8.0.0)
+Requires-Dist: arrow (>=1.3,<2.0)
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: docker (>=7.0,<8.0)
 Requires-Dist: packaging (>=24.0,<25.0)
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: tinydb (>=4.8.0,<5.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typer (>=0.12.0,<0.13.0)
+Requires-Dist: pydantic (>=2.6,<3.0)
+Requires-Dist: requests (>=2.31,<3.0)
+Requires-Dist: rich (>=13.7,<14.0)
+Requires-Dist: tinydb (>=4.8,<5.0)
+Requires-Dist: typer (>=0.12,<0.13)
 Project-URL: Repository, https://gitlab.com/drad/ibuilder
 Description-Content-Type: text/markdown
 
 # README
 
 ibuilder is a [cli](https://en.wikipedia.org/wiki/Command-line_interface) based builder of [docker](https://hub.docker.com/) images. It provides an interface for building and pushing the image, signing images, as well as for tagging source code after build with a build version and other common image tasks.
 
 
 ### Latest Changes
 
-- upgrade to pydantic 2x
-- upgraded packages: docker, packaging, pydantic, rich, typer
-- changed --version to use importlib.metadata
-- removed capturing of sign_logs
-- turned off pretty_exceptions (typer/rich)
+- cleaned up version and config's usage of importlib.metadata and/or pkg_resources (removed pkg_resources)
+- change python version requirement from 3.8+ to 3.11+ (for speed and to leverage internal tomllib)
+- update copyright date
+- package updates: idna, pydantic, typer, typing-extensions
 
 
 ### NOTICES
 
-- __Next Release Will Require Python 3.11 or Newer__ as we would like to move away from tomllib to address the following:
-  + this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
+- version 1.0.0 requires python 3.11+ (for internal toml processing capabilities and its fast)
 
 
 ### Features
 
 - build: build docker images
 - push: push images to any container registry
 - sign: sign images for container signing and verification
 - source control: tag and push when you build an image
 - history: retain build history for quick/easy access to past build info
 - quick/easy: create an `ibuilder.toml` file and run `ib build -i minor` to build, push, commit to source control and sign a new image
 
+
 ### Requirements
 
 - python 3
 - docker: docker must be set up as it is used to build and push the image
 - git: (optional) if you use the source-tag feature you will need git installed and your code setup in git (it simply performs a git tag && git push from the working directory)
 - image signor: (optional) if you choose to sign images a signor (such as cosign) is needed
 
+
 ### Overview
 
 - setup (see #setup)
 - configure (see #configure): place a copy of the `example/.ibuilder.toml` in the same directory as your Dockerfile of the app you want to build and adjust it as needed
 - run (see #run): execute ibuilder to build/push/tag a version of your app, its as simple as `ib build`
 
 
@@ -105,14 +101,15 @@
 
 ### Recommendations
 
 We recommend using docker's configuration storage for reg_auth-* related configuration items as it encrypts sensitive information and is likely already configured (if you have already used `docker login`). If you leave the remaining items empty the default values will be used. This will then try `$HOME/.docker/config.json` and `$HOME/.dockercfg` for your docker config settings. If you do not already have a docker config run `docker login` and it should be created for you. After a successful login you should not need to do anything else for the application as the needed info will be stored in your dockercfg and the app will use it when needed.
 
 If you are signing your images you may want to set the `COSIGN_PASSWORD` environment variable in your `~/.bashrc` or equivalent shell config file to avoid being prompted for your signing password after build and push. It should be noted that you will be prompted twice (if you are pushing both the build version and the `latest` tag of this version) as ib signs both tags of the built image. To avoid this we recommend setting the `COSIGN_PASSWORD` environment variable but please ensure you understand the security implications of doing so.
 
+
 ### Legacy
 
 This project originally started under the name boi - builder of images and as such you may find references to boi and even backward support for boi (e.g. local history database, user config file, etc.).
 
 
 ### Links
```

