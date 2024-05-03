# Comparing `tmp/cryptik-3.8.0.tar.gz` & `tmp/cryptik-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptik-3.8.0.tar", max compression
+gzip compressed data, was "cryptik-3.9.0.tar", max compression
```

## Comparing `cryptik-3.8.0.tar` & `cryptik-3.9.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    35067 2020-02-12 17:40:41.312178 cryptik-3.8.0/LICENSE
--rw-r--r--   0        0        0     2257 2021-12-19 15:39:31.658961 cryptik-3.8.0/README.md
--rw-r--r--   0        0        0        0 2022-04-29 20:51:18.926152 cryptik-3.8.0/cryptik/__init__.py
--rw-r--r--   0        0        0       48 2022-04-29 21:04:03.467878 cryptik-3.8.0/cryptik/__main__.py
--rw-r--r--   0        0        0        0 2022-04-29 21:19:41.567415 cryptik-3.8.0/cryptik/config/__init__.py
--rw-r--r--   0        0        0      502 2022-04-29 21:48:50.175629 cryptik-3.8.0/cryptik/config/config.py
--rw-r--r--   0        0        0     8804 2022-04-29 21:47:27.478417 cryptik-3.8.0/cryptik/main.py
--rw-r--r--   0        0        0      967 2022-04-29 21:47:04.218263 cryptik-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     3154 2022-04-29 21:51:24.716868 cryptik-3.8.0/setup.py
--rw-r--r--   0        0        0     3147 2022-04-29 21:51:24.717151 cryptik-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35067 2020-02-12 17:40:41.312178 cryptik-3.9.0/LICENSE
+-rw-r--r--   0        0        0     1748 2023-01-14 11:42:48.834371 cryptik-3.9.0/README.md
+-rw-r--r--   0        0        0        0 2022-09-18 10:36:32.707026 cryptik-3.9.0/cryptik/__init__.py
+-rw-r--r--   0        0        0       48 2022-09-18 10:36:32.707026 cryptik-3.9.0/cryptik/__main__.py
+-rw-r--r--   0        0        0        0 2022-09-18 10:36:32.710360 cryptik-3.9.0/cryptik/config/__init__.py
+-rw-r--r--   0        0        0      476 2022-09-18 10:36:32.710360 cryptik-3.9.0/cryptik/config/config.py
+-rw-r--r--   0        0        0     8778 2022-09-18 10:36:32.707026 cryptik-3.9.0/cryptik/main.py
+-rw-r--r--   0        0        0      960 2023-11-07 19:43:34.274470 cryptik-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 cryptik-3.9.0/PKG-INFO
```

### Comparing `cryptik-3.8.0/LICENSE` & `cryptik-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptik-3.8.0/cryptik/main.py` & `cryptik-3.9.0/cryptik/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #  SPDX-License-Identifier: GPL-3.0-only
-#  Copyright 2021 drad <drader@adercon.com>
+#  Copyright 2022 drad <sa@adercon.com>
+#
+# LOGGING: designed to run at INFO loglevel.
 
-import arrow
-import click
 import json
 import logging
 import os
 import sys
-import tomli
 from decimal import Decimal
 from urllib.request import urlopen
-from cryptik.config import config
+
+import arrow
+import click
+import tomli
+
 from cryptik.config.config import APP_NAME, APP_VERSION
 
 local_config = None
 logger_base = logging.getLogger(__name__)
 
 
 class Ticker(object):
@@ -81,17 +83,15 @@
             logging.error(
                 f"Unknown response data format: [{local_config['default']['response_data_format']}]"
             )
             return ""
 
 
 def show_version():
-    logging.critical(
-        f"{APP_NAME} {APP_VERSION}"
-    )
+    logging.critical(f"{APP_NAME} {APP_VERSION}")
     sys.exit()
 
 
 def list_all_exchanges():
     for exchg in local_config["exchanges"]:
         logging.critical(f"- {exchg['label']} ({exchg['id']}) - {exchg['type']}")
     sys.exit()
```

### Comparing `cryptik-3.8.0/pyproject.toml` & `cryptik-3.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 [internal]
 created = 2013-12-31
 
 [tool.poetry]
 name = "cryptik"
-version = "3.8.0"
+version = "3.9.0"
 description = "display cryptocurrency prices"
 authors = ["David Rader <sa@adercon.com>"]
 maintainers = ["David Rader <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/cryptik"
 repository = "https://gitlab.com/drad/cryptik"
 keywords = ["cli", "crypto", "currency", "bitcoin", "ticker"]
 
 [tool.poetry.scripts]
 cryptik = "cryptik.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-arrow = "1.2.2"
-click = "8.1.3"
-toml = "0.10.2"
+python = "^3.8"
+arrow = "1.3.0"
+click = "8.1.7"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
+target-version = ['py36', 'py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `cryptik-3.8.0/PKG-INFO` & `cryptik-3.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,70 @@
 Metadata-Version: 2.1
 Name: cryptik
-Version: 3.8.0
+Version: 3.9.0
 Summary: display cryptocurrency prices
 Home-page: https://gitlab.com/drad/cryptik
 License: GPL-3.0-only
 Keywords: cli,crypto,currency,bitcoin,ticker
 Author: David Rader
 Author-email: sa@adercon.com
 Maintainer: David Rader
 Maintainer-email: sa@adercon.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: arrow (==1.2.2)
-Requires-Dist: click (==8.1.3)
-Requires-Dist: toml (==0.10.2)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: arrow (==1.3.0)
+Requires-Dist: click (==8.1.7)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://gitlab.com/drad/cryptik
 Description-Content-Type: text/markdown
 
-## About ##
+## About
 
-a [cli](https://en.wikipedia.org/wiki/Command-line_interface)-based application for displaying the current price of a cryptocurrency. cryptik supports multiple exchanges and multiple currencies.
+a [cli](https://en.wikipedia.org/wiki/Command-line_interface) application for displaying the current price of a cryptocurrency, designed (but not limited) to be ran in conky. cryptik supports multiple exchanges and multiple currencies.
 
 Please see the project wiki for supported currencies and supported exchanges or to request new currencies/exchanges.
 
 
-## Requirements ##
-
-- python3
-
+## NOTICES
 
-## Install
+- this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
 
-- download cryptik: 
+## Requirements
 
-```
-# set release tag as desired.
-release=3.1.1
-wget https://gitlab.com/drad/cryptik/-/archive/${release}/cryptik-${release}.tar.bz2 \
-  && tar -xjf cryptik-${release}.tar.bz2 \
-  && rm cryptik-${release}.tar.bz2 \
-  && chmod u+x cryptik-${release}/cryptik.py
-```
+- python3
 
 
-## Setup ##
+## Install
 
-Although a virtual environment is not required, we strongly recommend it to keep cryptic's requirements separated from other python apps you may have. You can create a virtual environment with the following: 
+We recommend using [pipx](https://github.com/pypa/pipx) to install cryptik: `pipx install cryptik`. You can also install via pip: `pip install --user cryptik`.
 
-- install virtualenv: `pacman -S virtualenv`
-- setup virtualenv for cryptic (in cryptic root): `python3 -m virtualenv .venv`
-- activate virtualenv: `source .venv/bin/activate`
-- install requirements: `pip install -r requirements.txt`
+cryptik uses a config file to store your setup. This file contains information such as the exchange(s) to use. You can grab the sample config file from  [cryptik/example/config.toml](https://gitlab.com/drad/cryptik/-/blob/master/example/config.toml) and place it in `~/.config/cryptik` as this is where cryptik looks for the file by default or you can place it anywhere you like and use the `--config-file` parameter to specify the location.
 
-We recommend copying the config file to `~/.config/cryptik`:
-```
-mkdir ~/.config/cryptik \
-  && cp cryptik-${release}/example/config.toml ~/.config/cryptik/
-```
-> ignore this step if you already have a `config.toml` file setup
 
-- modify the config file as needed
-	- note: no changes are required; however, the app can be customized to your taste.
-- create app symlink (optional): `ln -sf -t ~/bin/ "$HOME/apps/cryptik/cryptik-${release}/cryptik.py"`
-  - note: replace ${release} with the version you downloaded
-  - note: the above symlink assumes you perform the download step (above) in the ~/apps/cryptik directory and that ~/bin is in your $PATH
+## Usage
 
-
-## Usage ##
-- call cryptik from command line: `cryptik.py -e BITSTAMP -t BTC`
-	- show full response: `cryptik.py -d full`
+- call cryptik from command line: `cryptik -e BITSTAMP -t BTC`
+  + show full response: `cryptik.py -d full`
 - list all available exchanges: `cryptik.py -l`
 - get help on cryptik: `cryptik.py -h`
 - example conky usage (note: this will show prices from two exchanges):
+
 ```
 CRYPTIK
-  ${texeci 600 cryptik.py -e KRAKEN -t BTC}
-  ${texeci 600 cryptik.py -e BITSTAMP -t BTC}
+  ${texeci 600 cryptik -e KRAKEN -t BTC}
+  ${texeci 600 cryptik -e BITSTAMP -t BTC}
 ```
 
 ## Example Response
-* direct call:
+
+- direct call:
 ```
-$ cryptik.py -e BITSTAMP -t BTC
+$ cryptik -e BITSTAMP -t BTC
 BTMP:BTC $9711.24 @12:33
 ```
```

