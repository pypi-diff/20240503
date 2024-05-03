# Comparing `tmp/orion_nais-0.1.2.tar.gz` & `tmp/orion_nais-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orion_nais-0.1.2.tar", max compression
+gzip compressed data, was "orion_nais-0.2.0.tar", max compression
```

## Comparing `orion_nais-0.1.2.tar` & `orion_nais-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-02-10 13:07:27.340638 orion_nais-0.1.2/LICENSE
--rw-r--r--   0        0        0     6590 2023-04-15 09:26:36.509871 orion_nais-0.1.2/README.md
--rw-r--r--   0        0        0       39 2023-01-26 14:12:33.833384 orion_nais-0.1.2/orion/__init__.py
--rw-r--r--   0        0        0    16061 2023-04-15 13:15:33.647801 orion_nais-0.1.2/orion/client.py
--rw-r--r--   0        0        0    17635 2023-04-15 13:20:41.818455 orion_nais-0.1.2/orion/mmsi.py
--rw-r--r--   0        0        0        0 2023-02-03 22:04:07.481203 orion_nais-0.1.2/orion/types/__init__.py
--rw-r--r--   0        0        0      296 2023-02-03 09:47:58.249080 orion_nais-0.1.2/orion/types/ais.py
--rw-r--r--   0        0        0      136 2023-01-27 13:52:51.653087 orion_nais-0.1.2/orion/urls.py
--rw-r--r--   0        0        0        0 2023-02-04 00:21:05.300372 orion_nais-0.1.2/orion/utils/__init__.py
--rw-r--r--   0        0        0     1100 2023-02-10 10:06:30.752969 orion_nais-0.1.2/orion/utils/get_data.py
--rw-r--r--   0        0        0    16652 2023-04-15 13:25:46.276172 orion_nais-0.1.2/orion/vessel_codes.py
--rw-r--r--   0        0        0     1654 2023-04-15 13:53:48.863111 orion_nais-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7713 1970-01-01 00:00:00.000000 orion_nais-0.1.2/setup.py
--rw-r--r--   0        0        0     7451 1970-01-01 00:00:00.000000 orion_nais-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-10 13:07:27.340638 orion_nais-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6590 2023-04-15 09:26:36.509871 orion_nais-0.2.0/README.md
+-rw-r--r--   0        0        0       88 2024-05-03 08:34:59.857897 orion_nais-0.2.0/orion/__init__.py
+-rw-r--r--   0        0        0    16183 2024-05-03 08:46:29.887008 orion_nais-0.2.0/orion/client.py
+-rw-r--r--   0        0        0     7464 2024-05-03 11:51:30.704100 orion_nais-0.2.0/orion/historic.py
+-rw-r--r--   0        0        0    17637 2024-05-03 08:40:45.963093 orion_nais-0.2.0/orion/mmsi.py
+-rw-r--r--   0        0        0        0 2023-02-03 22:04:07.481203 orion_nais-0.2.0/orion/types/__init__.py
+-rw-r--r--   0        0        0      296 2023-02-03 09:47:58.249080 orion_nais-0.2.0/orion/types/ais.py
+-rw-r--r--   0        0        0      192 2024-05-03 08:34:59.859990 orion_nais-0.2.0/orion/urls.py
+-rw-r--r--   0        0        0        0 2023-02-04 00:21:05.300372 orion_nais-0.2.0/orion/utils/__init__.py
+-rw-r--r--   0        0        0     1100 2023-02-10 10:06:30.752969 orion_nais-0.2.0/orion/utils/get_data.py
+-rw-r--r--   0        0        0    16652 2023-04-15 13:25:46.276172 orion_nais-0.2.0/orion/vessel_codes.py
+-rw-r--r--   0        0        0     1654 2024-05-03 11:54:24.743342 orion_nais-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7713 1970-01-01 00:00:00.000000 orion_nais-0.2.0/setup.py
+-rw-r--r--   0        0        0     7451 1970-01-01 00:00:00.000000 orion_nais-0.2.0/PKG-INFO
```

### Comparing `orion_nais-0.1.2/LICENSE` & `orion_nais-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.2/README.md` & `orion_nais-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.2/orion/client.py` & `orion_nais-0.2.0/orion/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Documentation of available API's and how to use them
 https://wiki.barentswatch.net/display/BO/API-Documentation
 
 Example:
 
 
 """
+
 import json
 import logging
 import math
 import os
 import urllib.parse
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional, Union
@@ -39,15 +40,14 @@
 logger = logging.getLogger(__name__)
 
 CLIENT_ID = os.getenv("CLIENT_ID", None)
 CLIENT_SECRET = os.getenv("CLIENT_SECRET", None)
 
 
 class Orion(MmsiMixin, VesselCodeMixin):
-
     """Interface to Barentswatch API
 
     The CLIENT_ID and CLIENT_SECRET should be exposed as environment variables called
     `CLIENT_ID` and `CLIENT_SECRET` or passed as parameters
     when creating an instance of the class.
 
     orion = Orion(client_id="myclientid", client_secret="myclientsecret")
@@ -62,15 +62,14 @@
 
     def __init__(
         self,
         client_id: Optional[str] = None,
         client_secret: Optional[str] = None,
         skip_auth: Optional[bool] = False,
     ) -> None:
-
         if skip_auth:
             return
         self.client_id = client_id or CLIENT_ID
         self.client_secret = client_secret or CLIENT_SECRET
 
         if (not self.client_id) | (not self.client_secret):  # pragma: no cover # noqa
             raise ValueError(
@@ -200,15 +199,17 @@
             response = self.session.get(
                 f"{URLS['HISTORIC_AIS']}/historic/tracks/{mmsi}/{fromDate}/{toDate}"
             )
             return self.decorate_ais_response(response)
         except requests.exceptions.HTTPError as err:  # pragma: no cover
             raise err
 
-    def decorate_ais_response(self, response: requests.models.Response) -> List[Ais]:
+    def decorate_ais_response(  # type: ignore[no-any-unimported]
+        self, response: requests.models.Response
+    ) -> List[Ais]:
         response.raise_for_status()
         ais = response.json()
 
         ais = self.add_jurisdiction_and_ship_type(ais)
         return ais
 
     def get_multiple_ais(
@@ -481,11 +482,14 @@
         Adds the jurisdiction and ship type to the dataframe
 
         Args:
             ais (List[Ais]): the ais track from NAIS
         """
 
         for a in ais:
-            a["shipTypeTxt"] = self.ais_vessel_codes.get_vessel_type_name(a["shipType"])
+            if "shipType" in a:
+                a["shipTypeTxt"] = self.ais_vessel_codes.get_vessel_type_name(
+                    a["shipType"]
+                )
             a["jurisdiction"] = self.mmsi.get_jurisdiction_name(a["mmsi"])
 
         return ais
```

### Comparing `orion_nais-0.1.2/orion/mmsi.py` & `orion_nais-0.2.0/orion/mmsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,27 +304,29 @@
 
 
 @dataclass
 class Jurisdiction:
     """
     Represents a jurisdiction. A jurisdiction is a country or a group of countries
     """
+
     name: str
     midcode: str
     full_name: str
 
 
 @dataclass
 class Mmsi:
     """
     Used for working with MMSI numbers. MMSI numbers are used to identify ships.
     Has utility methods for checking if a MMSI is a ship and
     getting the MID code for a ship. Also for filtering on country codes.
 
     """
+
     jurisdictions: List[Jurisdiction] = field(default_factory=make_jurisdictions)
 
     def is_valid_ship_mmsi(self, mmsi: int) -> bool:
         """check if mmsi is a ship.
 
         Args:
             mmsi (int): mmsi number
```

### Comparing `orion_nais-0.1.2/orion/utils/get_data.py` & `orion_nais-0.2.0/orion/utils/get_data.py`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.2/orion/vessel_codes.py` & `orion_nais-0.2.0/orion/vessel_codes.py`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.2/pyproject.toml` & `orion_nais-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orion-nais"
-version = "0.1.2"
+version = "0.2.0"
 description = "A client for the NAIS API from FThe Norwegian Coastal Administration"
 authors = ["Lasse Lambrechts <lasse.lambrechts@bt.no>"]
 license = "MIT"
 repository = "https://github.com/BergensTidende/orion-nais"
 readme = "README.md"
 packages = [{include = "orion"}]
```

### Comparing `orion_nais-0.1.2/setup.py` & `orion_nais-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'python-dotenv>=0.21.0,<0.22.0',
  'pytz>=2022.7.1,<2023.0.0',
  'requests>=2.28.0,<3.0.0',
  'shapely>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'orion-nais',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'A client for the NAIS API from FThe Norwegian Coastal Administration',
     'long_description': '# Orion-NAIS\n\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#requirements">Why the nanme Orion?</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#installation">Installation</a>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#local-development">Local development</a>\n      <ul>\n        <li><a href="#requirements">Requirements</a></li>\n        <li><a href="#makefile-commands">Makefile commands</a></li>\n        <li><a href="#structure">Structure</a></li>\n      </ul>\n    </li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOrion-NAIS is a client to work with the NAIS API. It helps with authentication and provides a simple interface to work with the API.\n\nWhen working with the API you need to have a valid token. The token is valid for a set period of time. The client will automatically refresh the token when it expires.\n\n### Why the name Orion?\n\nThe NAIS Api is provided through BarentsWatch. BarentsWatch is a Norwegian information portal that provides overview of activity and knowledge in coastal and sea areas. The Norwegian movie "Orion\'s Belt" from 1985 is an action movie set in the Barents region. About three men, a bulldozer, a Russian helicopter and a ship. Thus the name Orion.\n\n## Installation\n\nRequires Python 3.10 or later.\n\n```bash\n\npip install orion-nais\n\n```\n\nor using pipenv:\n\n```bash\n\npipenv install orion-nais\n\n```\n\nor using poetry:\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nTo install the package in your project run\n\n```bash\n\npoetry add orion-nais\n```\n\nthen add an .env file to your project with the following variables:\n\n```bash\nCLIENT_ID=\nCLIENT_SECRET=\n```\n\nIf you don\'t have a client id and secret you can get one from your [BarentsWatch account](https://www.barentswatch.no/minside/).\n\nThen you can use the client like this:\n\n```python\nfrom orion import Orion\n\norion = Orion()\n# Get the last 24 hours of AIS data for a ship with MMSI XXXXXXXXXX\nais = orion.get_ais_last_24H(SHIP_MMSI)\n# Convert the AIS data to a line\nline = orion.ais_to_line(ais)\n\n```\n\n## Local development\n\n### Requirements\n- pyenv - manage python versions\n- poetry - manage python dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew or the way described in the [documentation](https://python-poetry.org/docs/#installation)\n\n\n### Makefile commands\n\n- `make lint`\n  - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.\n- `make format`\n  - format the code in the src folder with black and isort.\n- `make test`\n  - run the tests in the tests folder.\n- `make bump-patch`\n  - bump the patch version of the package. Example: 0.1.0 -> 0.1.1\n- `make bump-minor`\n  - bump the minor version of the package. Example: 0.1.0 -> 0.2.0\n- `make bump-major`\n  - bump the major version of the package. Example: 0.1.0 -> 1.0.0 \n- `make release`\n  - publish the package to pypi. You need to have an account and be logged in to pypi.\n\n\n### Structure\n\n```\n.\n├── .bumpversion.cfg\n├── .editorconfig\n├── .flake8\n├── .gitignore\n├── Makefile\n├── README.md\n├── orion\n│   ├── client.py\n│   ├── mmsi.py\n│   ├── types\n│   │   └── ais.py\n│   ├── urls.py\n│   ├── utils\n│   │   └── get_data.py\n│   └── vessel_codes.py\n├── poetry.lock\n├── pyproject.toml\n└── tests\n    ├── make_mock_data.py\n    ├── mocks\n    └── test_orion.py\n    \n```\n\n- `.bumpversion.cfg`\n  - Configuration file for bumpversion.\n- `.editorconfig`\n  - Configuration file for editorconfig.\n- `.flake8`\n  - Configuration file for flake8.\n- `.gitignore`\n  - Configuration file for git.\n- `pyproject.toml`\n  - Configuration file for poetry. Mypy and isort is configured here.\n- `poetry.lock`\n  - Lock file for poetry.\n- `Makefile`\n  - Makefile for the project. Here you can find commands for linting and formatting.\n- `README.md`\n  - This file.\n- `orion`\n  - The source code for the package.\n  - `client.py`\n    - The client class.\n  - `mmsi.py`\n    - A dataclass for handling MMSI numbers and MID-codes (jurisdiction).\n  - `types`\n    - A folder for types.\n    - `ais.py`\n      - A class for handling AIS messages.\n  - `urls.py`\n    - A file with urls for the API.\n  - `utils`\n    - A folder for utility functions.\n    - `get_data.py`\n      - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.\n  - `vessel_codes.py`\n    - A dataclass for looking up vessel codes.\n- `tests`\n  - Tests for the package.\n\n## Contributing\n\nDo you have write permissions to the repo? Then you can clone this project to a folder on your computer.\n\n```bash\ngit clone https://github.com/BergensTidende/orion-nais.git\n```\n\nIf not do the following:\n\n- Create a personal fork of the project on Github.\n- Clone the fork on your local machine. Your remote repo on Github is called `origin`.\n- Add the original repository as a remote called `upstream`.\n- If you created your fork a while ago be sure to pull upstream changes into your local repository.\n\nThis will clone the repo into `orion-nais`. \n\nCreate a branch for your changes\n\n```bash\ngit checkout -b name-of-branch\n```\n\nMake your changes, rememeber to commit. And always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.\n\nIf you\'re working on a clone push the branch to github and make PR.\n\nIf your\'re working a fork:\n\n- Squash your commits into a single commit with git\'s [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.\n- Push your branch to your fork on Github, the remote `origin`.\n- From your fork open a pull request in the correct branch. Target the project\'s `develop` branch if there is one, else go for `master`.\n- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.\n- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete\n  your extra branch(es).\n\n <!-- CONTACT -->\n\n## Contact\n\nBord4 - bord4@bt.no\n',
     'author': 'Lasse Lambrechts',
     'author_email': 'lasse.lambrechts@bt.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/BergensTidende/orion-nais',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['orion',
 'orion.types', 'orion.utils'] package_data = \ {'': ['*']} install_requires = \
 ['geopandas>=0.12.2,<0.13.0', 'pandas>=1.5.2,<2.0.0', 'python-
 dotenv>=0.21.0,<0.22.0', 'pytz>=2022.7.1,<2023.0.0', 'requests>=2.28.0,<3.0.0',
 'shapely>=2.0.0,<3.0.0'] setup_kwargs = { 'name': 'orion-nais', 'version':
-'0.1.2', 'description': 'A client for the NAIS API from FThe Norwegian Coastal
+'0.2.0', 'description': 'A client for the NAIS API from FThe Norwegian Coastal
 Administration', 'long_description': '# Orion-NAIS\n\n\n\n\n
 ********** TTaabbllee ooff CCoonntteennttss **********
 \n
    1. \n
    2. \n _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t\n
           o \n
           o _W_h_y_ _t_h_e_ _n_a_n_m_e_ _O_r_i_o_n_?
```

### Comparing `orion_nais-0.1.2/PKG-INFO` & `orion_nais-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orion-nais
-Version: 0.1.2
+Version: 0.2.0
 Summary: A client for the NAIS API from FThe Norwegian Coastal Administration
 Home-page: https://github.com/BergensTidende/orion-nais
 License: MIT
 Author: Lasse Lambrechts
 Author-email: lasse.lambrechts@bt.no
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: orion-nais Version: 0.1.2 Summary: A client for the
+Metadata-Version: 2.1 Name: orion-nais Version: 0.2.0 Summary: A client for the
 NAIS API from FThe Norwegian Coastal Administration Home-page: https://
 github.com/BergensTidende/orion-nais License: MIT Author: Lasse Lambrechts
 Author-email: lasse.lambrechts@bt.no Requires-Python: >=3.10,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: geopandas
 (>=0.12.2,<0.13.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-Dist:
```

