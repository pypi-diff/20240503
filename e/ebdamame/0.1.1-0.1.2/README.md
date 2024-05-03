# Comparing `tmp/ebdamame-0.1.1.tar.gz` & `tmp/ebdamame-0.1.2.tar.gz`

## Comparing `ebdamame-0.1.1.tar` & `ebdamame-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 ebdamame-0.1.1/README.md
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 ebdamame-0.1.1/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ebdamame-0.1.1/requirements.in
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ebdamame-0.1.1/requirements.txt
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 ebdamame-0.1.1/setup.cfg
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ebdamame-0.1.1/setup.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ebdamame-0.1.1/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/packaging.yml
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ebdamame-0.1.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ebdamame-0.1.1/src/_ebddocx2table_version.py
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 ebdamame-0.1.1/src/ebdamame/__init__.py
--rw-r--r--   0        0        0    17292 2020-02-02 00:00:00.000000 ebdamame-0.1.1/src/ebdamame/docxtableconverter.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ebdamame-0.1.1/src/ebdamame/py.typed
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 ebdamame-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ebdamame-0.1.1/LICENSE
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ebdamame-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 ebdamame-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 ebdamame-0.1.2/README.md
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 ebdamame-0.1.2/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ebdamame-0.1.2/requirements.in
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ebdamame-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 ebdamame-0.1.2/setup.cfg
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ebdamame-0.1.2/setup.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ebdamame-0.1.2/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/packaging.yml
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/_ebddocx2table_version.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/ebdamame/__init__.py
+-rw-r--r--   0        0        0    17292 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/ebdamame/docxtableconverter.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/ebdamame/py.typed
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ebdamame-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ebdamame-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ebdamame-0.1.2/PKG-INFO
```

### Comparing `ebdamame-0.1.1/.pre-commit-config.yaml` & `ebdamame-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/README.md` & `ebdamame-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 ![Coverage status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Black/badge.svg)
 ![PyPi Status Badge](https://img.shields.io/pypi/v/ebdamame)
 
 🇩🇪 Dieses Repository enthält ein Python-Paket namens [`ebdamame`](https://pypi.org/project/ebdamame) (früher: `ebddocx2table`), das genutzt werden kann, um aus .docx-Dateien maschinenlesbare Tabellen, die einen Entscheidungsbaum (EBD) modellieren, zu extrahieren (scrapen).
 Diese Entscheidungsbäume sind Teil eines regulatorischen Regelwerks für die deutsche Energiewirtschaft und kommen in der Eingangsprüfung der Marktkommunikation zum Einsatz.
-Die mit diesem Paket erstellten maschinenlesbaren Tabellen können mit [`ebdtable2graph`](https://pypi.org/project/ebdtable2graph) in echte Graphen und Diagramme umgewandelt werden.
+Die mit diesem Paket erstellten maschinenlesbaren Tabellen können mit [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (früher: `ebdtable2graph`) in echte Graphen und Diagramme umgewandelt werden.
 Exemplarische Ergebnisse des Scrapings finden sich als .json-Dateien im Repository [`machine-readable_entscheidungsbaumdiagramme`](https://github.com/Hochfrequenz/machine-readable_entscheidungsbaumdiagramme/).
 
 🇬🇧 This repository contains the source code of the Python package [`ebdamame`](https://pypi.org/project/ebdamame) (formerly published as `ebddocx2table`).
 
 ## Rationale
 
 Assume that you want to analyse or visualize the Entscheidungsbaumdiagramme (EBD) by EDI@Energy.
 The website edi-energy.de, as always, only provides you with PDF or Word files instead of _really_ digitized data.
 
-The package `ebdamame` scrapes the `.docx` files and returns data in a model defined in the "sister" package [`ebdtable2graph`](https://pypi.org/project/ebdtable2graph).
+The package `ebdamame` scrapes the `.docx` files and returns data in a model defined in the "sister" package [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (formerly known as `ebdtable2graph`).
 
-Once you scraped the data (using this package) you can plot it with [`ebdtable2graph`](https://pypi.org/project/ebdtable2graph).
+Once you scraped the data (using this package) you can plot it with [`rebdhuhn`](https://pypi.org/project/rebdhuhn).
 
 ## How to use the package
 
 In any case, install the repo from PyPI:
 
 ```bash
 pip install ebdamame
```

### Comparing `ebdamame-0.1.1/main.py` & `ebdamame-0.1.2/main.py`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/requirements.txt` & `ebdamame-0.1.2/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # via requests
 charset-normalizer==2.1.1
     # via requests
 click==8.1.7
     # via -r requirements.in
 ebdtable2graph==0.1.20
     # via -r requirements.in
-idna==3.4
+idna==3.7
     # via requests
 lxml==4.9.3
     # via
     #   ebdtable2graph
     #   python-docx
     #   svgutils
 more-itertools==10.2.0
```

### Comparing `ebdamame-0.1.1/setup.cfg` & `ebdamame-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/tox.ini` & `ebdamame-0.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/dependabot.yml` & `ebdamame-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/coverage.yml` & `ebdamame-0.1.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/dependabot_automerge.yml` & `ebdamame-0.1.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/formatting.yml` & `ebdamame-0.1.2/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/packaging.yml` & `ebdamame-0.1.2/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/python-publish.yml` & `ebdamame-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/pythonlint.yml` & `ebdamame-0.1.2/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.github/workflows/unittests.yml` & `ebdamame-0.1.2/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/dev_requirements/requirements-packaging.txt` & `ebdamame-0.1.2/dev_requirements/requirements-packaging.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
-#    pip-compile requirements-packaging.in
+#    pip-compile dev_requirements/requirements-packaging.in
 #
-bleach==6.0.0
-    # via readme-renderer
-build==1.1.1
+build==1.2.1
     # via -r dev_requirements/requirements-packaging.in
-certifi==2023.7.22
+certifi==2024.2.2
     # via requests
-cffi==1.15.1
+cffi==1.16.0
     # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
-cryptography==42.0.4
+cryptography==42.0.5
     # via secretstorage
 docutils==0.20.1
     # via readme-renderer
-idna==3.4
+idna==3.7
     # via requests
-importlib-metadata==6.7.0
+importlib-metadata==7.0.2
     # via
     #   keyring
     #   twine
-jaraco-classes==3.2.3
+jaraco-classes==3.3.1
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==24.2.0
+keyring==24.3.1
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
     # via jaraco-classes
-packaging==23.1
+nh3==0.2.15
+    # via readme-renderer
+packaging==24.0
     # via build
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-readme-renderer==40.0
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.4.2
+rich==13.7.1
     # via twine
 secretstorage==3.3.3
     # via keyring
-six==1.16.0
-    # via bleach
 twine==5.0.0
     # via -r dev_requirements/requirements-packaging.in
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-webencodings==0.5.1
-    # via bleach
-zipp==3.15.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `ebdamame-0.1.1/dev_requirements/requirements-tests.txt` & `ebdamame-0.1.2/dev_requirements/requirements-tests.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 attrs==23.2.0
     # via pytest-subtests
 iniconfig==2.0.0
     # via pytest
 packaging==23.0
     # via pytest
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
-pytest==8.1.1
+pytest==8.2.0
     # via
     #   -r dev_requirements/requirements-tests.in
     #   pytest-datafiles
     #   pytest-subtests
 pytest-datafiles==3.0.0
     # via -r dev_requirements/requirements-tests.in
 pytest-subtests==0.12.1
```

### Comparing `ebdamame-0.1.1/src/ebdamame/__init__.py` & `ebdamame-0.1.2/src/ebdamame/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     """
     parent_elements = document.element.body
     for item in parent_elements.iterchildren():
         if isinstance(item, CT_P):
             yield Paragraph(item, document)
         elif isinstance(item, CT_Tbl):
             yield Table(item, document)
+        else:
+            _logger.debug("Item %s is neither Paragraph nor Table", str(item))
 
 
 _ebd_key_pattern = re.compile(r"^E_\d{4}$")
 _ebd_key_with_heading_pattern = re.compile(r"^(?P<key>E_\d{4})_(?P<title>.*)\s*$")
 
 
 class TableNotFoundError(Exception):
@@ -134,15 +136,15 @@
         if (
             isinstance(table_or_paragraph, Table)
             and is_inside_subsection_of_requested_table
             and _table_is_an_ebd_table(table_or_paragraph)
         ):
             table: Table = table_or_paragraph
             tables.append(table)
-            # Now we have to check if the EBD table spans multiple pages and _maybe_ we have to collect more tables.
+            # Now we have to check if the EBD table spans multiple pages, and _maybe_ we have to collect more tables.
             # The funny thing is: Sometimes the authors create multiple tables split over multiple lines which belong
             # together, sometimes they create 1 proper table that spans multiple pages.
             # The latter case (1 docx table spanning >1 pages) is transparent to the extraction logic; i.e. python-docx
             # treats a single table that spans multiple pages just the same as a table on only 1 page.
             for next_item in tables_and_paragraphs:  # start iterating from where the outer loop paused
                 if isinstance(next_item, Table):
                     # this is the case that the authors created multiple single tables on single adjacent pages
```

### Comparing `ebdamame-0.1.1/src/ebdamame/docxtableconverter.py` & `ebdamame-0.1.2/src/ebdamame/docxtableconverter.py`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/.gitignore` & `ebdamame-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/LICENSE` & `ebdamame-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/pyproject.toml` & `ebdamame-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.1/PKG-INFO` & `ebdamame-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ebdamame
-Version: 0.1.1
+Version: 0.1.2
 Summary: A scraper to library to scrape .docx files with 'Entscheidungsbaumdiagramm' tables into a truely machine readable structure
 Project-URL: Changelog, https://github.com/Hochfrequenz/ebdamame/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/ebdamame
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: EBD,Energiewirtschaft,Marktkommunikation
@@ -31,27 +31,27 @@
 ![Coverage status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Black/badge.svg)
 ![PyPi Status Badge](https://img.shields.io/pypi/v/ebdamame)
 
 🇩🇪 Dieses Repository enthält ein Python-Paket namens [`ebdamame`](https://pypi.org/project/ebdamame) (früher: `ebddocx2table`), das genutzt werden kann, um aus .docx-Dateien maschinenlesbare Tabellen, die einen Entscheidungsbaum (EBD) modellieren, zu extrahieren (scrapen).
 Diese Entscheidungsbäume sind Teil eines regulatorischen Regelwerks für die deutsche Energiewirtschaft und kommen in der Eingangsprüfung der Marktkommunikation zum Einsatz.
-Die mit diesem Paket erstellten maschinenlesbaren Tabellen können mit [`ebdtable2graph`](https://pypi.org/project/ebdtable2graph) in echte Graphen und Diagramme umgewandelt werden.
+Die mit diesem Paket erstellten maschinenlesbaren Tabellen können mit [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (früher: `ebdtable2graph`) in echte Graphen und Diagramme umgewandelt werden.
 Exemplarische Ergebnisse des Scrapings finden sich als .json-Dateien im Repository [`machine-readable_entscheidungsbaumdiagramme`](https://github.com/Hochfrequenz/machine-readable_entscheidungsbaumdiagramme/).
 
 🇬🇧 This repository contains the source code of the Python package [`ebdamame`](https://pypi.org/project/ebdamame) (formerly published as `ebddocx2table`).
 
 ## Rationale
 
 Assume that you want to analyse or visualize the Entscheidungsbaumdiagramme (EBD) by EDI@Energy.
 The website edi-energy.de, as always, only provides you with PDF or Word files instead of _really_ digitized data.
 
-The package `ebdamame` scrapes the `.docx` files and returns data in a model defined in the "sister" package [`ebdtable2graph`](https://pypi.org/project/ebdtable2graph).
+The package `ebdamame` scrapes the `.docx` files and returns data in a model defined in the "sister" package [`rebdhuhn`](https://pypi.org/project/rebdhuhn) (formerly known as `ebdtable2graph`).
 
-Once you scraped the data (using this package) you can plot it with [`ebdtable2graph`](https://pypi.org/project/ebdtable2graph).
+Once you scraped the data (using this package) you can plot it with [`rebdhuhn`](https://pypi.org/project/rebdhuhn).
 
 ## How to use the package
 
 In any case, install the repo from PyPI:
 
 ```bash
 pip install ebdamame
```

