# Comparing `tmp/mpbroker-0.9.0.tar.gz` & `tmp/mpbroker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbroker-0.9.0.tar", max compression
+gzip compressed data, was "mpbroker-1.0.0.tar", max compression
```

## Comparing `mpbroker-0.9.0.tar` & `mpbroker-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    35067 2022-04-21 09:47:13.597689 mpbroker-0.9.0/LICENSE
--rw-r--r--   0        0        0     5315 2022-05-07 11:11:29.175437 mpbroker-0.9.0/README.md
--rw-r--r--   0        0        0       22 2022-04-29 18:06:03.791139 mpbroker-0.9.0/mpbroker/__init__.py
--rw-r--r--   0        0        0       44 2022-04-29 18:06:03.791139 mpbroker-0.9.0/mpbroker/__main__.py
--rw-r--r--   0        0        0        0 2022-04-26 10:06:01.180041 mpbroker-0.9.0/mpbroker/config/__init__.py
--rw-r--r--   0        0        0     2008 2022-05-03 10:04:47.659519 mpbroker-0.9.0/mpbroker/config/config.py
--rw-r--r--   0        0        0     1511 2022-05-05 21:47:20.154898 mpbroker-0.9.0/mpbroker/config/db_init_design_docs.py
--rw-r--r--   0        0        0      814 2022-05-07 11:07:35.023774 mpbroker-0.9.0/mpbroker/config/models.py
--rw-r--r--   0        0        0     1017 2022-05-07 11:06:44.183416 mpbroker-0.9.0/mpbroker/example/user_config.toml
--rw-r--r--   0        0        0    17031 2022-05-10 13:38:40.197327 mpbroker-0.9.0/mpbroker/main.py
--rw-r--r--   0        0        0        0 2022-04-21 11:50:22.897600 mpbroker-0.9.0/mpbroker/models/__init__.py
--rw-r--r--   0        0        0     1708 2022-05-04 10:57:19.337941 mpbroker-0.9.0/mpbroker/models/injest.py
--rw-r--r--   0        0        0     3429 2022-05-05 10:41:17.732115 mpbroker-0.9.0/mpbroker/models/media.py
--rw-r--r--   0        0        0     4662 2022-05-10 13:15:38.748487 mpbroker-0.9.0/mpbroker/tools.py
--rw-r--r--   0        0        0     5907 2022-05-10 13:37:53.920369 mpbroker-0.9.0/mpbroker/utils.py
--rw-r--r--   0        0        0     1124 2022-05-10 12:21:08.088333 mpbroker-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6435 2022-05-10 13:39:06.990675 mpbroker-0.9.0/setup.py
--rw-r--r--   0        0        0     6458 2022-05-10 13:39:06.991325 mpbroker-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35067 2022-04-21 09:47:13.597689 mpbroker-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6295 2024-05-03 13:30:15.755063 mpbroker-1.0.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-03 13:05:03.326898 mpbroker-1.0.0/mpbroker/__init__.py
+-rw-r--r--   0        0        0       44 2024-05-03 13:05:03.346898 mpbroker-1.0.0/mpbroker/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:05:03.343565 mpbroker-1.0.0/mpbroker/config/__init__.py
+-rw-r--r--   0        0        0     2014 2024-05-03 13:19:22.470920 mpbroker-1.0.0/mpbroker/config/config.py
+-rw-r--r--   0        0        0     2956 2024-05-03 13:05:03.336898 mpbroker-1.0.0/mpbroker/config/db_init_design_docs.py
+-rw-r--r--   0        0        0      820 2024-05-03 13:05:03.340232 mpbroker-1.0.0/mpbroker/config/models.py
+-rw-r--r--   0        0        0     1056 2023-01-30 18:14:23.756945 mpbroker-1.0.0/mpbroker/example/user_config.toml
+-rw-r--r--   0        0        0    24554 2024-05-03 13:05:03.343565 mpbroker-1.0.0/mpbroker/main.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:05:03.333565 mpbroker-1.0.0/mpbroker/models/__init__.py
+-rw-r--r--   0        0        0      673 2024-05-03 13:05:03.330231 mpbroker-1.0.0/mpbroker/models/ingest.py
+-rw-r--r--   0        0        0     3420 2024-05-03 13:05:03.333565 mpbroker-1.0.0/mpbroker/models/media.py
+-rw-r--r--   0        0        0     5048 2024-05-03 13:05:03.346898 mpbroker-1.0.0/mpbroker/tools.py
+-rw-r--r--   0        0        0    11577 2024-05-03 13:05:03.350232 mpbroker-1.0.0/mpbroker/utils.py
+-rw-r--r--   0        0        0      863 2024-05-03 13:30:00.291237 mpbroker-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7256 1970-01-01 00:00:00.000000 mpbroker-1.0.0/PKG-INFO
```

### Comparing `mpbroker-0.9.0/LICENSE` & `mpbroker-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpbroker-0.9.0/README.md` & `mpbroker-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,111 @@
 # README
 
 Media Player Broker (mpb) is an application that helps you play and track media you have watched over disparet locations. mpb keeps track of what you have played at Location A so when you are at Location B you can see what you have watched from either location to avoid digging through history command output over SSH.
 
 mpb is not a player itself but it can be configured to launch your player of choice to view media.
 
 
+## Latest Changes
+
+- cleaned up version and config's usage of importlib.metadata and/or pkg_resources (removed pkg_resources)
+- cleaned up `info` to be more concise and to show more 'about' info
+- update copyright date
+- package updates: idna, pydantic, typer, package
+- change python version requirement from 3.8+ to 3.11+ (for speed and to leverage internal tomllib)
+
+
+### NOTICE
+
+- version 1.0.0 requires python 3.11+ (for internal toml processing capabilities and its fast)
+- version 0.14.0 corrected the spelling error (injest ─⏵ ingest) which requires a change to your `user_config.toml` file (change `[injest]` to `[ingest]`)
+
+
 ### The Need
 
 Rather than living in the cloud I have my videos duplicated at various locations. I needed something that remembers what episode of MacGyver I had watched in one location so when I was in another location I could continue watching the next episode without digging through `history` output or keeping track of what was played where.
 
-mpb consists of a CLI application (the client) and a database (couchdb). From the client you `injest` your media metadata. This extracts the file names from file paths and stores the data in the database. After injesting, you can `list` your media which shows you the media Item, whether it has been watched or not along with a Rating, Notes, and the Sources the item is available at. You can then use the `play` command along with the Item to watch the Item. After playback is completed you are prompted to mark the item as played/watched, Rate it and add Notes - all of which are used in the `list` command to show what you have already watched and what is new.
+mpb consists of a CLI application (the client) and a database (couchdb). From the client you `ingest` your media metadata. This extracts the file names from file paths and stores the data in the database. After ingesting, you can `list` your media which shows you the media Item, whether it has been watched or not along with a Rating, Notes, and the Sources the item is available at. You can then use the `play` command along with the Item to watch the Item. After playback is completed you are prompted to mark the item as played/watched, Rate it and add Notes - all of which are used in the `list` command to show what you have already watched and what is new.
 
 mpb can also be used by multiple 'users' - you can share a 'user' so your wife can see what you have watched or you can keep separate users so your wife sees what she has watched and you know what you have watched.
 
 
 ### Install
 
 We recommend using [pipx](https://github.com/pypa/pipx) to install mpbroker: `pipx install mpbroker`. You can also install via pip: `pip install --user mpbroker`.
 
-mpbroker uses a config file to store your setup. This file contains information such as your media player, the database url, and types of data to injest. You can grab the sample config file from  [mpbroker/example/user_config.toml](https://gitlab.com/drad/mpbroker/-/blob/master/mpbroker/example/user_config.toml) and place it in a config location. mpbroker searches the following locations for the config file (in order of precedence):
+mpbroker uses a config file to store your setup. This file contains information such as your media player, the database url, and types of data to ingest. You can grab the sample config file from  [mpbroker/example/user_config.toml](https://gitlab.com/drad/mpbroker/-/blob/master/mpbroker/example/user_config.toml) and place it in a config location. mpbroker searches the following locations for the config file (in order of precedence):
 
 - $MPB_CONFIG_HOME: set this environment variable to any path you like and place the mpbroker `user_config.toml` file in this location
 - $XDG_CONFIG_HOME/mpbroker
 - $APPDATA/mpbroker
 - $HOME/.config/mpbroker
 
 
 ### Configure
 
 #### Notices
+
 - an example `user_config.toml` file can be found in the [project example directory](https://gitlab.com/drad/mpbroker/-/tree/master/mpbroker/example)
 - if you do not want to use the standard locations and do not want to set a `MPB_CONFIG_HOME` envvar you can set `MPB_CONFIG_HOME` on the command line before calling mpb such as `MPB_CONFIG_HOME=/opt/tmp mpb list 'The_Matrix'`
 
 To set up MPB you need to:
 - create your `user_config.toml` file (see above for locations of this file)
 - configure your user_config.toml file (at a minimum you will need to set/change the `database.db_uri` value)
 - ensure your mpb database is available
   + use the `db-init` command to initialize your db if it is a new instance!
 
-If you are testing mpb or do not have a database you can use docker-compose to start a local database with `docker-compose up` from the [project's docker-compose.yml file](https://gitlab.com/drad/mpbroker). If you use the local database your `database.db_uri` would be: `http://admin:couchdb@localhost:5984`
+If you are testing mpb or do not have a database you can use docker-compose to start a local database with `docker-compose up` from the [project's docker-compose.yml file](https://gitlab.com/drad/mpbroker). If you use the local database your `database.db_uri` would be: `http://localhost:5984` (add your username and password if needed).
 
 
 ### Using MPB
 
 mpb has built in help (`mpb --help`) which should give you enough info to get going.
 
 A Quick Start:
 
-- you will likely want to `injest` some media
+- you will likely want to `ingest` some media
 - next you can use `list` to view/find an item to play
 - finally you can `play` an item
 
 #### Paging Output
 
 mpb has pager support, to enable it set the 'use_pager' config option in the user_config.toml file. By default this is not enabled as most pagers drop color support. If you would like pager support and want color to remain in the output you can set the following in your `~/.bashrc` (or equivalent) file:
 
 ```
-export LESS='--RAW-CONTROL-CHARS'
+export LESS='--quit-if-one-screen --ignore-case --status-column --LONG-PROMPT --RAW-CONTROL-CHARS --HILITE-UNREAD --tabs=4 --no-init --window=-4'
 ```
 
 Tip: using a pager allows showing one 'page' (screen) of results at a time; however, most pagers (less) also allow searching within the results easily and quickly. We recommend setting the `--RAW-CONTROL-CHARS` and using `less` with mpbroker.
 
 
-### Injestion
+### Ingestion
 
-Injestion is the process of loading media metadata into your mpbroker database.
+Ingestion is the process of loading media metadata into your mpbroker database.
 
 #### Extract Metadata
 
-Extracting metadata on injestion increases the injestion time but adds the following data to each injested media item:
+Extracting metadata on ingestion increases the ingestion time but adds the following data to each ingested media item:
 
     file_size: # filesize in human readable format (569 MiB, 1.1 GiB)
     file_type: # file type (video/H265)
     file_format: # file format (Matroska)
     encoding: # encoding (x265)
     duration: # duration in human readable format (1 h 52 min, 2 h 48 min)
     resolution: # resulution in width x height format (720 x 480)
     aspect_ratio: # display aspect ratio (16:9)
     audio_format:  audio format (AAC)
     audio_sampling: audio sample rate (48000)
 
-#### Injestion Time Details
+To extract metadata you will need to install [MediaInfo](https://mediaarea.net/en/MediaInfo) which should be available in the repo of most distributions:
+
+- arch: `mediainfo`
+- debian: `mediainfo`
+
+#### Ingestion Time Details
 
 - ~500 videos
     + with metadata extraction: 6.05s
     + without metadata extraction: 99.05s
 - 2785 videos
     + with metadata extraction: 596.53s
     + without metadata extraction: 72.75s
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mpbroker-0.9.0/mpbroker/config/config.py` & `mpbroker-1.0.0/mpbroker/config/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2022 drad <drader@adercon.com>
+#  Copyright 2024 dradux.com
 
 import logging
 from os import environ, getenv, path
 
-import pkg_resources
-import tomli
+import importlib.metadata as md
+import tomllib
 
 from mpbroker.config.models import UserConfigBase
 
-logger = logging.getLogger("default")
-
 user_config_file_name = "user_config.toml"
-
+logger = logging.getLogger("default")
 
 def env_strtobool(val: str) -> bool:
     if val in ["true", "'true'"]:
         return True
     return False
 
 
 def csv_to_set(in_str: str) -> set:
-
     return set(map(int, in_str.split(",")))
 
 
 def load_config(cfg_file: str = None) -> dict:
     """
     Load config data from toml config file
     """
 
     conf = {}
     try:
         with open(cfg_file, "rb") as f:
-            conf = tomli.load(f)
+            conf = tomllib.load(f)
     except FileNotFoundError as e:
         print(f"File not found: {e}")
     except Exception as e:
         print(f"Other Exception: {e}")
     return conf
 
 
-APP_VERSION = pkg_resources.get_distribution("mpbroker").version
-APP_NAME = pkg_resources.get_distribution("mpbroker").project_name
+APP_NAME = md.metadata("mpbroker")["Name"]
+APP_VERSION = md.metadata("mpbroker")["Version"]
+APP_AUTHORS = md.metadata("mpbroker")["Authors"]
 
 # get user config file (e.g. ~/.config/{APP_NAME}/{user_config_file_name)
 _user_config_file = None
 if environ.get("MPB_CONFIG_HOME"):
     _user_config_file = path.join(environ.get("MPB_CONFIG_HOME"), user_config_file_name)
 elif environ.get("XDG_CONFIG_HOME"):
     _user_config_file = path.join(
```

### Comparing `mpbroker-0.9.0/mpbroker/config/models.py` & `mpbroker-1.0.0/mpbroker/config/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2022 drad <drader@adercon.com>
+#  Copyright 2024 dradux.com
 
 from typing import List
 
 from pydantic import BaseModel
 
 
 class UserConfigDefaults(BaseModel):
     """
     Defaults for UserConfig.
     """
 
     source: str = None
     user: str = None
+    base: str = None
 
 
-class UserConfigInjest(BaseModel):
+class UserConfigIngest(BaseModel):
     """
-    User Config Injest.
+    User Config Ingest.
     """
 
     file_types: List[str] = None
 
 
 class UserConfigDatabase(BaseModel):
     """
@@ -39,9 +40,9 @@
     """
 
     player: str = None
     use_pager: bool = False
 
     database: UserConfigDatabase = None
     defaults: UserConfigDefaults = None
-    injest: UserConfigInjest = None
+    ingest: UserConfigIngest = None
     source_mappings: dict = None
```

### Comparing `mpbroker-0.9.0/mpbroker/example/user_config.toml` & `mpbroker-1.0.0/mpbroker/example/user_config.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # MPB User Configuration file.
 
 player = "/usr/sbin/smplayer"                                                  # the player to use.
 
 use_pager = false                                                              # use pager (see README.md for more info)
 
 [database]
-    db_uri = "http://user:password@localhost:5984"                             # Database URI.
+    db_uri = "http://localhost:5984"                                           # Database URI (add username and password if needed)
 
 
 [defaults]
-    user = "drad"                                                              # default user (so you dont need to supply the --user param
-    source = "gaz"                                                             # default source (so you dont need to supply the --source param
+    user = "drad"                                                              # default user
+    source = "gaz"                                                             # default source
+    base = "/opt/media"                                                        # default base
 
 
-[injest]
-    # file types to injest
+[ingest]
+    # file types to ingest
     file_types = ['*.3g2', '*.3gp', '*.AVI', '*.MOV', '*.MP4', '*.asf', '*.avi', '*.m4v', '*.mkv', '*.mp4', '*.mpg', '*.ogv', '*.webm']
 
 
 [source_mappings]                                                              # source mappings map a source to a base path.
   gaz-opt = "/opt/media"
   gaz-festus = "/mnt/media/video"
```

### Comparing `mpbroker-0.9.0/mpbroker/models/media.py` & `mpbroker-1.0.0/mpbroker/models/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2022 drad <drader@adercon.com>
+#  Copyright 2024 dradux.com
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import BaseModel
 
@@ -49,35 +49,35 @@
 
 
 class MediaPlay(BaseModel):
     """
     Media item Play info.
     """
 
-    status: MediaPlayStatus = MediaPlayStatus.new  # the play status of the item.
+    status: MediaPlayStatus = MediaPlayStatus.new.value  # the play status of the item.
     rating: Optional[MediaPlayRating] = None  # play rating.
     rating_notes: Optional[str] = None  # notes about rating.
     notes: Optional[str] = None  # notes about the play (e.g. watched 1, 2, 3).
     history: Optional[List[MediaPlayHistory]] = None  # play history info.
 
 
 class MediaMetadata(BaseModel):
     """
     Media Metadata.
     """
 
-    file_size: str = None  # filesize in human readable format (569 MiB, 1.1 GiB)
-    file_type: str = None  # file type (video/H265)
-    file_format: str = None  # file format (Matroska)
-    encoding: str = None  # encoding (x265)
-    duration: str = None  # duration in human readable format (1 h 52 min, 2 h 48 min)
-    resolution: str = None  # resulution in width x height format (720 x 480)
-    aspect_ratio: str = None  # display aspect ratio (16:9)
-    audio_format: str = None  # audio format (AAC)
-    audio_sampling: str = None  # audio sample rate (48000)
+    file_size: str | None  # filesize in human readable format (569 MiB, 1.1 GiB)
+    file_type: str | None  # file type (video/H265)
+    file_format: str | None  # file format (Matroska)
+    encoding: str | None  # encoding (x265)
+    duration: str | None  # duration in human readable format (1 h 52 min, 2 h 48 min)
+    resolution: str | None  # resulution in width x height format (720 x 480)
+    aspect_ratio: str | None  # display aspect ratio (16:9)
+    audio_format: str | None  # audio format (AAC)
+    audio_sampling: int | None  # audio sample rate (48000)
 
 
 class MediaBase(BaseModel):
     """
     A media item.
     """
```

### Comparing `mpbroker-0.9.0/mpbroker/tools.py` & `mpbroker-1.0.0/mpbroker/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2022 drad <drader@adercon.com>
+#  Copyright 2024 dradux.com
 #
 
 import pycouchdb
 import requests
 import typer
 
 from mpbroker.config.config import DATABASES, user_cfg
@@ -15,14 +15,15 @@
 app = typer.Typer(help="[Somewhat] useful tools!")
 
 
 @app.command()
 def db_init():
     """
     Perform DB setup tasks: create databases, views, etc.
+    NOTICE: this command is safe to use on a database that already has data.
     """
     from mpbroker.config.db_init_design_docs import views
 
     typer.echo("Creating Databases:")
     for db in DATABASES:
         try:
             server.create(db)
@@ -39,15 +40,22 @@
                 err=True,
             )
             raise typer.Exit()
 
     typer.echo("Creating Views:")
     try:
         for view in views:
+            # NOTE: we take the approach of deleting all views first and then create all to ensure views are updated.
             db = server.database(view[0])
+            # drop view
+            db.delete(view[1])
+            typer.secho(
+                f" ✓ {view[0]}/{view[1]['_id']} - deleted", fg=typer.colors.GREEN
+            )
+            # create view
             db.save(view[1])
             typer.secho(
                 f" ✓ {view[0]}/{view[1]['_id']} - created", fg=typer.colors.GREEN
             )
 
     except requests.exceptions.ConnectionError:
         db_not_available()
@@ -117,15 +125,15 @@
             fg=typer.colors.RED,
             bold=True,
         )
     typer.confirm("\nDo you want to continue?", abort=True)
 
     db = server.database("media")
     results = db.query(
-        "filters/names",
+        "filters/by-name",
         # group='true',
         # keys=[name],
         startkey=f"{from_user}",
         endkey=f"{from_user}\ufff0",
         as_list=True,
         # flat="key"
     )
```

### Comparing `mpbroker-0.9.0/pyproject.toml` & `mpbroker-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 [internal]
 created = 2022-04-21
+modified = 2024-05-03
 
 [tool.poetry]
 name = "mpbroker"
-version = "0.9.0"
+version = "1.0.0"
 description = "Media Player Broker"
 license = "GPL-3.0-only"
-authors = ["David Rader <sa@adercon.com>"]
-maintainers = ["David Rader <sa@adercon.com>"]
+authors = ["drad <sa@adercon.com>"]
+maintainers = ["drad <sa@adercon.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/drad/mpbroker"
 repository = "https://gitlab.com/drad/mpbroker"
-keywords = ["media player", "broker", "player", "video", "smplayer", "vlc", "couchdb", "cli"]
+keywords = ["media player", "broker", "player", "video", "smplayer", "vlc", "couchdb", "cli", "mpv"]
 
 [tool.poetry.scripts]
 mpb = "mpbroker.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typer = {extras = ["all"], version = "^0.4.1"}
-arrow = "^1.2.2"
-pycouchdb = "^1.14.1"
-pydantic = "^1.9.0"
-requests = "^2.27.1"
-rich = "^12.3.0"
-tomli = "^2.0.1"
-pymediainfo = "^5.1.0"
-natsort = "^8.1.0"
+python = "^3.11"
+typer = {extras = ["all"], version = "^0.12.1"}
+pycouchdb = "^1.14.2"
+pydantic = "^2.6.4"
+requests = "^2.31.0"
+rich = "^13.7.1"
+pymediainfo = "^6.1.0"
+natsort = "^8.4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+#pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.black]
-line-length = 88
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
```

### Comparing `mpbroker-0.9.0/setup.py` & `mpbroker-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mpbroker
+Version: 1.0.0
+Summary: Media Player Broker
+Home-page: https://gitlab.com/drad/mpbroker
+License: GPL-3.0-only
+Keywords: media player,broker,player,video,smplayer,vlc,couchdb,cli,mpv
+Author: drad
+Author-email: sa@adercon.com
+Maintainer: drad
+Maintainer-email: sa@adercon.com
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: natsort (>=8.4.0,<9.0.0)
+Requires-Dist: pycouchdb (>=1.14.2,<2.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pymediainfo (>=6.1.0,<7.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: typer[all] (>=0.12.1,<0.13.0)
+Project-URL: Repository, https://gitlab.com/drad/mpbroker
+Description-Content-Type: text/markdown
 
-packages = \
-['mpbroker', 'mpbroker.config', 'mpbroker.models']
+# README
 
-package_data = \
-{'': ['*'], 'mpbroker': ['example/*']}
+Media Player Broker (mpb) is an application that helps you play and track media you have watched over disparet locations. mpb keeps track of what you have played at Location A so when you are at Location B you can see what you have watched from either location to avoid digging through history command output over SSH.
 
-install_requires = \
-['arrow>=1.2.2,<2.0.0',
- 'natsort>=8.1.0,<9.0.0',
- 'pycouchdb>=1.14.1,<2.0.0',
- 'pydantic>=1.9.0,<2.0.0',
- 'pymediainfo>=5.1.0,<6.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'rich>=12.3.0,<13.0.0',
- 'tomli>=2.0.1,<3.0.0',
- 'typer[all]>=0.4.1,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['mpb = mpbroker.main:app']}
-
-setup_kwargs = {
-    'name': 'mpbroker',
-    'version': '0.9.0',
-    'description': 'Media Player Broker',
-    'long_description': "# README\n\nMedia Player Broker (mpb) is an application that helps you play and track media you have watched over disparet locations. mpb keeps track of what you have played at Location A so when you are at Location B you can see what you have watched from either location to avoid digging through history command output over SSH.\n\nmpb is not a player itself but it can be configured to launch your player of choice to view media.\n\n\n### The Need\n\nRather than living in the cloud I have my videos duplicated at various locations. I needed something that remembers what episode of MacGyver I had watched in one location so when I was in another location I could continue watching the next episode without digging through `history` output or keeping track of what was played where.\n\nmpb consists of a CLI application (the client) and a database (couchdb). From the client you `injest` your media metadata. This extracts the file names from file paths and stores the data in the database. After injesting, you can `list` your media which shows you the media Item, whether it has been watched or not along with a Rating, Notes, and the Sources the item is available at. You can then use the `play` command along with the Item to watch the Item. After playback is completed you are prompted to mark the item as played/watched, Rate it and add Notes - all of which are used in the `list` command to show what you have already watched and what is new.\n\nmpb can also be used by multiple 'users' - you can share a 'user' so your wife can see what you have watched or you can keep separate users so your wife sees what she has watched and you know what you have watched.\n\n\n### Install\n\nWe recommend using [pipx](https://github.com/pypa/pipx) to install mpbroker: `pipx install mpbroker`. You can also install via pip: `pip install --user mpbroker`.\n\nmpbroker uses a config file to store your setup. This file contains information such as your media player, the database url, and types of data to injest. You can grab the sample config file from  [mpbroker/example/user_config.toml](https://gitlab.com/drad/mpbroker/-/blob/master/mpbroker/example/user_config.toml) and place it in a config location. mpbroker searches the following locations for the config file (in order of precedence):\n\n- $MPB_CONFIG_HOME: set this environment variable to any path you like and place the mpbroker `user_config.toml` file in this location\n- $XDG_CONFIG_HOME/mpbroker\n- $APPDATA/mpbroker\n- $HOME/.config/mpbroker\n\n\n### Configure\n\n#### Notices\n- an example `user_config.toml` file can be found in the [project example directory](https://gitlab.com/drad/mpbroker/-/tree/master/mpbroker/example)\n- if you do not want to use the standard locations and do not want to set a `MPB_CONFIG_HOME` envvar you can set `MPB_CONFIG_HOME` on the command line before calling mpb such as `MPB_CONFIG_HOME=/opt/tmp mpb list 'The_Matrix'`\n\nTo set up MPB you need to:\n- create your `user_config.toml` file (see above for locations of this file)\n- configure your user_config.toml file (at a minimum you will need to set/change the `database.db_uri` value)\n- ensure your mpb database is available\n  + use the `db-init` command to initialize your db if it is a new instance!\n\nIf you are testing mpb or do not have a database you can use docker-compose to start a local database with `docker-compose up` from the [project's docker-compose.yml file](https://gitlab.com/drad/mpbroker). If you use the local database your `database.db_uri` would be: `http://admin:couchdb@localhost:5984`\n\n\n### Using MPB\n\nmpb has built in help (`mpb --help`) which should give you enough info to get going.\n\nA Quick Start:\n\n- you will likely want to `injest` some media\n- next you can use `list` to view/find an item to play\n- finally you can `play` an item\n\n#### Paging Output\n\nmpb has pager support, to enable it set the 'use_pager' config option in the user_config.toml file. By default this is not enabled as most pagers drop color support. If you would like pager support and want color to remain in the output you can set the following in your `~/.bashrc` (or equivalent) file:\n\n```\nexport LESS='--RAW-CONTROL-CHARS'\n```\n\nTip: using a pager allows showing one 'page' (screen) of results at a time; however, most pagers (less) also allow searching within the results easily and quickly. We recommend setting the `--RAW-CONTROL-CHARS` and using `less` with mpbroker.\n\n\n### Injestion\n\nInjestion is the process of loading media metadata into your mpbroker database.\n\n#### Extract Metadata\n\nExtracting metadata on injestion increases the injestion time but adds the following data to each injested media item:\n\n    file_size: # filesize in human readable format (569 MiB, 1.1 GiB)\n    file_type: # file type (video/H265)\n    file_format: # file format (Matroska)\n    encoding: # encoding (x265)\n    duration: # duration in human readable format (1 h 52 min, 2 h 48 min)\n    resolution: # resulution in width x height format (720 x 480)\n    aspect_ratio: # display aspect ratio (16:9)\n    audio_format:  audio format (AAC)\n    audio_sampling: audio sample rate (48000)\n\n#### Injestion Time Details\n\n- ~500 videos\n    + with metadata extraction: 6.05s\n    + without metadata extraction: 99.05s\n- 2785 videos\n    + with metadata extraction: 596.53s\n    + without metadata extraction: 72.75s\n",
-    'author': 'David Rader',
-    'author_email': 'sa@adercon.com',
-    'maintainer': 'David Rader',
-    'maintainer_email': 'sa@adercon.com',
-    'url': 'https://gitlab.com/drad/mpbroker',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+mpb is not a player itself but it can be configured to launch your player of choice to view media.
 
 
-setup(**setup_kwargs)
+## Latest Changes
+
+- cleaned up version and config's usage of importlib.metadata and/or pkg_resources (removed pkg_resources)
+- cleaned up `info` to be more concise and to show more 'about' info
+- update copyright date
+- package updates: idna, pydantic, typer, package
+- change python version requirement from 3.8+ to 3.11+ (for speed and to leverage internal tomllib)
+
+
+### NOTICE
+
+- version 1.0.0 requires python 3.11+ (for internal toml processing capabilities and its fast)
+- version 0.14.0 corrected the spelling error (injest ─⏵ ingest) which requires a change to your `user_config.toml` file (change `[injest]` to `[ingest]`)
+
+
+### The Need
+
+Rather than living in the cloud I have my videos duplicated at various locations. I needed something that remembers what episode of MacGyver I had watched in one location so when I was in another location I could continue watching the next episode without digging through `history` output or keeping track of what was played where.
+
+mpb consists of a CLI application (the client) and a database (couchdb). From the client you `ingest` your media metadata. This extracts the file names from file paths and stores the data in the database. After ingesting, you can `list` your media which shows you the media Item, whether it has been watched or not along with a Rating, Notes, and the Sources the item is available at. You can then use the `play` command along with the Item to watch the Item. After playback is completed you are prompted to mark the item as played/watched, Rate it and add Notes - all of which are used in the `list` command to show what you have already watched and what is new.
+
+mpb can also be used by multiple 'users' - you can share a 'user' so your wife can see what you have watched or you can keep separate users so your wife sees what she has watched and you know what you have watched.
+
+
+### Install
+
+We recommend using [pipx](https://github.com/pypa/pipx) to install mpbroker: `pipx install mpbroker`. You can also install via pip: `pip install --user mpbroker`.
+
+mpbroker uses a config file to store your setup. This file contains information such as your media player, the database url, and types of data to ingest. You can grab the sample config file from  [mpbroker/example/user_config.toml](https://gitlab.com/drad/mpbroker/-/blob/master/mpbroker/example/user_config.toml) and place it in a config location. mpbroker searches the following locations for the config file (in order of precedence):
+
+- $MPB_CONFIG_HOME: set this environment variable to any path you like and place the mpbroker `user_config.toml` file in this location
+- $XDG_CONFIG_HOME/mpbroker
+- $APPDATA/mpbroker
+- $HOME/.config/mpbroker
+
+
+### Configure
+
+#### Notices
+
+- an example `user_config.toml` file can be found in the [project example directory](https://gitlab.com/drad/mpbroker/-/tree/master/mpbroker/example)
+- if you do not want to use the standard locations and do not want to set a `MPB_CONFIG_HOME` envvar you can set `MPB_CONFIG_HOME` on the command line before calling mpb such as `MPB_CONFIG_HOME=/opt/tmp mpb list 'The_Matrix'`
+
+To set up MPB you need to:
+- create your `user_config.toml` file (see above for locations of this file)
+- configure your user_config.toml file (at a minimum you will need to set/change the `database.db_uri` value)
+- ensure your mpb database is available
+  + use the `db-init` command to initialize your db if it is a new instance!
+
+If you are testing mpb or do not have a database you can use docker-compose to start a local database with `docker-compose up` from the [project's docker-compose.yml file](https://gitlab.com/drad/mpbroker). If you use the local database your `database.db_uri` would be: `http://localhost:5984` (add your username and password if needed).
+
+
+### Using MPB
+
+mpb has built in help (`mpb --help`) which should give you enough info to get going.
+
+A Quick Start:
+
+- you will likely want to `ingest` some media
+- next you can use `list` to view/find an item to play
+- finally you can `play` an item
+
+#### Paging Output
+
+mpb has pager support, to enable it set the 'use_pager' config option in the user_config.toml file. By default this is not enabled as most pagers drop color support. If you would like pager support and want color to remain in the output you can set the following in your `~/.bashrc` (or equivalent) file:
+
+```
+export LESS='--quit-if-one-screen --ignore-case --status-column --LONG-PROMPT --RAW-CONTROL-CHARS --HILITE-UNREAD --tabs=4 --no-init --window=-4'
+```
+
+Tip: using a pager allows showing one 'page' (screen) of results at a time; however, most pagers (less) also allow searching within the results easily and quickly. We recommend setting the `--RAW-CONTROL-CHARS` and using `less` with mpbroker.
+
+
+### Ingestion
+
+Ingestion is the process of loading media metadata into your mpbroker database.
+
+#### Extract Metadata
+
+Extracting metadata on ingestion increases the ingestion time but adds the following data to each ingested media item:
+
+    file_size: # filesize in human readable format (569 MiB, 1.1 GiB)
+    file_type: # file type (video/H265)
+    file_format: # file format (Matroska)
+    encoding: # encoding (x265)
+    duration: # duration in human readable format (1 h 52 min, 2 h 48 min)
+    resolution: # resulution in width x height format (720 x 480)
+    aspect_ratio: # display aspect ratio (16:9)
+    audio_format:  audio format (AAC)
+    audio_sampling: audio sample rate (48000)
+
+To extract metadata you will need to install [MediaInfo](https://mediaarea.net/en/MediaInfo) which should be available in the repo of most distributions:
+
+- arch: `mediainfo`
+- debian: `mediainfo`
+
+#### Ingestion Time Details
+
+- ~500 videos
+    + with metadata extraction: 6.05s
+    + without metadata extraction: 99.05s
+- 2785 videos
+    + with metadata extraction: 596.53s
+    + without metadata extraction: 72.75s
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

