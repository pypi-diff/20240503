# Comparing `tmp/rebdhuhn-0.0.0.tar.gz` & `tmp/rebdhuhn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebdhuhn-0.0.0.tar", last modified: Wed Mar 13 17:35:51 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `rebdhuhn-0.0.0.tar` & `rebdhuhn-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:35:51.694793 rebdhuhn-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-03-13 17:35:51.694793 rebdhuhn-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-13 17:35:51.694793 rebdhuhn-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:35:51.690793 rebdhuhn-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:35:51.690793 rebdhuhn-0.0.0/src/rebdhuhn/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/add_watermark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/graph_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/graphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/hochfrequenz-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/kroki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:35:51.694793 rebdhuhn-0.0.0/src/rebdhuhn/models/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/models/ebd_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/models/ebd_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:35:51.694793 rebdhuhn-0.0.0/src/rebdhuhn/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-13 17:35:43.000000 rebdhuhn-0.0.0/src/rebdhuhn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:35:51.694793 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-03-13 17:35:51.000000 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-13 17:35:51.000000 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:35:51.000000 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:35:51.000000 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-13 17:35:51.000000 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 17:35:51.000000 rebdhuhn-0.0.0/src/rebdhuhn.egg-info/top_level.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.gitattributes
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/README.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/create_env_file.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/docker-compose.yaml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/env.example
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/mwe_e0003.svg
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/requirements.txt
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0    24708 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/last_common_ancestor.drawio.svg
+-rw-r--r--   0        0        0    17251 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/plantuml_not_convertable.drawio.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/__init__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/add_watermark.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/graph_conversion.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/graph_utils.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/graphviz.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/hochfrequenz-logo.svg
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/kroki.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/plantuml.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/version.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/models/__init__.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/models/ebd_graph.py
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/models/ebd_table.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/src/rebdhuhn/models/errors/__init__.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 rebdhuhn-0.2.3/PKG-INFO
```

### Comparing `rebdhuhn-0.0.0/LICENSE` & `rebdhuhn-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/PKG-INFO` & `rebdhuhn-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rebdhuhn
-Version: 0.0.0
+Version: 0.2.3
 Summary: Converts (already scraped) Entscheidungsbaumdiagramm tables to real graphs
-Home-page: https://github.com/Hochfrequenz/rebdhuhn
-Author: Hochfrequenz Unternehmensberatung GmbH
-Author-email: info@hochfrequenz.de
-License: mit
-Project-URL: Documentation, https://github.com/Hochfrequenz/rebdhuhn
-Project-URL: Code, https://github.com/Hochfrequenz/rebdhuhn
-Project-URL: Bug tracker, https://github.com/Hochfrequenz/rebdhuhn/issues
-Platform: any
+Project-URL: Homepage, https://github.com/Hochfrequenz/rebdhuhn
+Project-URL: Changelog, https://github.com/Hochfrequenz/rebdhuhn/releases
+Project-URL: Repository, https://github.com/Hochfrequenz/rebdhuhn
+Project-URL: Issue Tracker, https://github.com/Hochfrequenz/rebdhuhn/issues
+Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
+License: GPL
+License-File: LICENSE
+Keywords: ahb,automation,bdew,edi@energy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
 Requires-Dist: attrs
-Requires-Dist: networkx
-Requires-Dist: requests
 Requires-Dist: cattrs
 Requires-Dist: lxml>=4.9.3
+Requires-Dist: networkx
+Requires-Dist: requests
 Requires-Dist: svgutils
+Description-Content-Type: text/markdown
 
 # rebdhuhn
 
 ![Unittests status badge](https://github.com/Hochfrequenz/rebdhuhn/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/rebdhuhn/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/rebdhuhn/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/rebdhuhn/workflows/Black/badge.svg)
@@ -37,15 +38,15 @@
 🇩🇪 Dieses Repository enthält ein Python-Paket namens [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (früher: `ebdtable2graph`), das genutzt werden kann, um aus .docx-Dateien extrahierte maschinenlesbare Tabellen, die einen Entscheidungsbaum (EBD) modellieren, in echte Graphen zu konvertieren. Diese Entscheidungsbäume sind Teil eines regulatorischen Regelwerks für die deutsche Energiewirtschaft und kommen in der Eingangsprüfung der Marktkommunikation zum Einsatz.
 
 🇬🇧 This repository contains the source code of the Python package [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (formerly known as `ebdtable2graph`).
 
 ## Rationale
 
 Assume, that you scraped the Entscheidungsbaumdiagramm tables by EDI@Energy from their somewhat "digitized" PDF/DOCX files.
-(To do so, you can use the package [`ebdameme`](https://github.com/Hochfrequenz/ebdamame) (was: 'ebddocx2table').)
+(To do so, you can use the package [`ebdamame`](https://github.com/Hochfrequenz/ebdamame) (was: 'ebddocx2table`).)
 Also assume, that the result of your scraping is a [`rebdhuhn.models.EbdTable`](src/rebdhuhn/models/ebd_table.py).
 
 The package `rebdhuhn` contains logic to convert your scraped data into a graph.
 This graph can then be exported e.g. as SVG and/or UML.
 
 ## How to use `rebdhuhn`?
 
@@ -146,18 +147,32 @@
         Gewählter Zeitpunkt nicht zulässig
     endnote
     kill;
 endif
 @enduml
 ```
 
-#### Export as SVG
+#### Export the graph as SVG
 
-You can also export the graph as SVG
+First, make sure to have a local instance of [kroki](https://kroki.io) up and running via docker (localhost:8125):
+
+Add the required `.env` file to the repository root by opening a new terminal session, changing the directory to
+```bash
+cd path\to\rebdhuhn\repository\root
+```
+and executing the `create_env_file.py` script via
+```bash
+python create_env_file.py
+```
+Run the `docker-desktop` app on your local maschine and host the local kroki instance on PORT `8125` via
+```bash
+docker-compose up -d
+```
 
+To export the graph as SVG, use
 ```python
 from rebdhuhn import convert_plantuml_to_svg_kroki
 
 svg_code = convert_plantuml_to_svg_kroki(plantuml_code)
 with open("e_0003.svg", "w+", encoding="utf-8") as svg_file:
     svg_file.write(svg_code)
 ```
```

### Comparing `rebdhuhn-0.0.0/README.md` & `rebdhuhn-0.2.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 🇩🇪 Dieses Repository enthält ein Python-Paket namens [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (früher: `ebdtable2graph`), das genutzt werden kann, um aus .docx-Dateien extrahierte maschinenlesbare Tabellen, die einen Entscheidungsbaum (EBD) modellieren, in echte Graphen zu konvertieren. Diese Entscheidungsbäume sind Teil eines regulatorischen Regelwerks für die deutsche Energiewirtschaft und kommen in der Eingangsprüfung der Marktkommunikation zum Einsatz.
 
 🇬🇧 This repository contains the source code of the Python package [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (formerly known as `ebdtable2graph`).
 
 ## Rationale
 
 Assume, that you scraped the Entscheidungsbaumdiagramm tables by EDI@Energy from their somewhat "digitized" PDF/DOCX files.
-(To do so, you can use the package [`ebdameme`](https://github.com/Hochfrequenz/ebdamame) (was: 'ebddocx2table').)
+(To do so, you can use the package [`ebdamame`](https://github.com/Hochfrequenz/ebdamame) (was: 'ebddocx2table`).)
 Also assume, that the result of your scraping is a [`rebdhuhn.models.EbdTable`](src/rebdhuhn/models/ebd_table.py).
 
 The package `rebdhuhn` contains logic to convert your scraped data into a graph.
 This graph can then be exported e.g. as SVG and/or UML.
 
 ## How to use `rebdhuhn`?
 
@@ -118,18 +118,32 @@
         Gewählter Zeitpunkt nicht zulässig
     endnote
     kill;
 endif
 @enduml
 ```
 
-#### Export as SVG
+#### Export the graph as SVG
 
-You can also export the graph as SVG
+First, make sure to have a local instance of [kroki](https://kroki.io) up and running via docker (localhost:8125):
 
+Add the required `.env` file to the repository root by opening a new terminal session, changing the directory to
+```bash
+cd path\to\rebdhuhn\repository\root
+```
+and executing the `create_env_file.py` script via
+```bash
+python create_env_file.py
+```
+Run the `docker-desktop` app on your local maschine and host the local kroki instance on PORT `8125` via
+```bash
+docker-compose up -d
+```
+
+To export the graph as SVG, use
 ```python
 from rebdhuhn import convert_plantuml_to_svg_kroki
 
 svg_code = convert_plantuml_to_svg_kroki(plantuml_code)
 with open("e_0003.svg", "w+", encoding="utf-8") as svg_file:
     svg_file.write(svg_code)
 ```
```

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/add_watermark.py` & `rebdhuhn-0.2.3/src/rebdhuhn/add_watermark.py`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/graph_conversion.py` & `rebdhuhn-0.2.3/src/rebdhuhn/graph_conversion.py`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/graph_utils.py` & `rebdhuhn-0.2.3/src/rebdhuhn/graph_utils.py`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/graphviz.py` & `rebdhuhn-0.2.3/src/rebdhuhn/graphviz.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,13 +178,13 @@
     Converts dot code to svg (code) and returns the result as string. It uses kroki.io.
     Optionally add the HF watermark to the svg code, controlled by the argument 'add_watermark'
     Optionally add a background with the color 'HF white', controlled by the argument 'add_background'
     If 'add_background' is False, the background is transparent.
     """
     if dot_to_svg_converter is None:
         dot_to_svg_converter = Kroki()
-    svg_out = dot_to_svg_converter.convert_to_svg(dot_code)
+    svg_out = dot_to_svg_converter.convert_dot_to_svg(dot_code)
     if add_watermark:
         svg_out = add_watermark_function(svg_out)
     if add_background:
         svg_out = add_background_function(svg_out)
     return svg_out
```

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/hochfrequenz-logo.svg` & `rebdhuhn-0.2.3/src/rebdhuhn/hochfrequenz-logo.svg`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/models/ebd_graph.py` & `rebdhuhn-0.2.3/src/rebdhuhn/models/ebd_graph.py`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/models/ebd_table.py` & `rebdhuhn-0.2.3/src/rebdhuhn/models/ebd_table.py`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/models/errors/__init__.py` & `rebdhuhn-0.2.3/src/rebdhuhn/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `rebdhuhn-0.0.0/src/rebdhuhn/plantuml.py` & `rebdhuhn-0.2.3/src/rebdhuhn/plantuml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 This module contains logic to convert EbdGraph data to plantuml code and further to parse this code to SVG images.
 """
 
 from collections import namedtuple
 
-import requests  # pylint: disable=import-error
 from networkx import DiGraph  # type:ignore[import]
 
 from rebdhuhn.graph_utils import COMMON_ANCESTOR_FIELD, _get_yes_no_edges, _mark_last_common_ancestors
+from rebdhuhn.kroki import Kroki, PlantUmlToSvgConverter
 from rebdhuhn.models import DecisionNode, EbdGraph, EndNode, OutcomeNode
 from rebdhuhn.models.errors import GraphTooComplexForPlantumlError, NotExactlyTwoOutgoingEdgesError
 
 ADD_INDENT = "    "  #: This is just for style purposes to make the plantuml files human-readable.
 
 
 def _escape_for_plantuml(input_str: str) -> str:
     """
-    Plantuml has sometimes problems with the character ')'. Therefore, we escape it with the respective HTML code since
+    Plantuml sometimes has problems with the character ')'. Therefore, we escape it with the respective HTML code since
     Plantuml supports HTML.
     """
     return input_str.replace(")", "&#41;")
 
 
 def _draw_node1_below_node2(graph: DiGraph, node1: str, node2: str) -> bool:
     """
@@ -185,23 +185,14 @@
     else:
         key_of_first_node = list(nx_graph["Start"].keys())[0]
     plantuml_code += _convert_node_to_plantuml(nx_graph, key_of_first_node, "")
 
     return plantuml_code + "\n@enduml\n"
 
 
-def convert_plantuml_to_svg_kroki(plantuml_code: str) -> str:
+def convert_plantuml_to_svg_kroki(plantuml_code: str, converter: PlantUmlToSvgConverter | None = None) -> str:
     """
-    Converts plantuml code to svg (code) and returns the result as string. It uses kroki.io.
+    Converts plantuml code to svg code using kroki
     """
-    url = "https://kroki.io"
-    answer = requests.post(
-        url,
-        json={"diagram_source": plantuml_code, "diagram_type": "plantuml", "output_format": "svg"},
-        timeout=5,
-    )
-    if answer.status_code != 200:
-        raise ValueError(
-            f"Error while converting plantuml to svg: {answer.status_code}: {requests.codes[answer.status_code]}. "
-            f"{answer.text}"
-        )
-    return answer.text
+    if converter is None:
+        converter = Kroki()  # with its default address (e.g. localhost:8125)
+    return converter.convert_plantuml_to_svg(plantuml_code)
```

