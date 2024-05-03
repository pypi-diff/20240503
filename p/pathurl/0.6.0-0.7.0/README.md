# Comparing `tmp/pathurl-0.6.0.tar.gz` & `tmp/pathurl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathurl-0.6.0.tar", max compression
+gzip compressed data, was "pathurl-0.7.0.tar", max compression
```

## Comparing `pathurl-0.6.0.tar` & `pathurl-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7652 2023-01-28 23:28:28.010464 pathurl-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1730 2023-06-29 14:56:38.858233 pathurl-0.6.0/README.rst
--rw-r--r--   0        0        0     2572 2023-06-29 14:56:38.839108 pathurl-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      126 2023-01-28 23:28:28.011188 pathurl-0.6.0/src/pathurl/__init__.py
--rw-r--r--   0        0        0      458 2023-03-05 22:42:54.891380 pathurl-0.6.0/src/pathurl/_constants.py
--rw-r--r--   0        0        0     1250 2023-06-29 13:56:06.801723 pathurl-0.6.0/src/pathurl/path.py
--rw-r--r--   0        0        0        0 2023-01-28 23:28:28.011349 pathurl-0.6.0/src/pathurl/py.typed
--rw-r--r--   0        0        0     3042 2023-06-29 14:23:43.799591 pathurl-0.6.0/src/pathurl/query.py
--rw-r--r--   0        0        0     3878 2023-06-29 13:58:47.111208 pathurl-0.6.0/src/pathurl/url.py
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 pathurl-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-02 20:57:25.591775 pathurl-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     1467 2024-05-03 10:22:04.659219 pathurl-0.7.0/docs/README.md
+-rw-r--r--   0        0        0     2927 2024-05-03 11:00:42.727304 pathurl-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/__init__.py
+-rw-r--r--   0        0        0      458 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/_constants.py
+-rw-r--r--   0        0        0     1250 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/path.py
+-rw-r--r--   0        0        0        0 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/py.typed
+-rw-r--r--   0        0        0     3028 2024-05-02 20:57:25.595108 pathurl-0.7.0/src/pathurl/query.py
+-rw-r--r--   0        0        0     3960 2024-05-02 20:57:25.595108 pathurl-0.7.0/src/pathurl/url.py
+-rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 pathurl-0.7.0/PKG-INFO
```

### Comparing `pathurl-0.6.0/LICENSE.txt` & `pathurl-0.7.0/LICENSE.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,165 +1,159 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+# GNU LESSER GENERAL PUBLIC LICENSE
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
+Version 3, 29 June 2007
 
+Copyright &copy; 2007 Free Software Foundation, Inc.
+[https://fsf.org/][FSF]
 
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
 
-  0. Additional Definitions.
+This version of the GNU Lesser General Public License incorporates the
+terms and conditions of version 3 of the GNU General Public License,
+supplemented by the additional permissions listed below.
 
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
+## 0. Additional Definitions.
 
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
+As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the
+GNU General Public License.
 
-  An "Application" is any work that makes use of an interface provided
+"The Library" refers to a covered work governed by this License, other
+than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided
 by the Library, but which is not otherwise based on the Library.
 Defining a subclass of a class defined by the Library is deemed a mode
 of using an interface provided by the Library.
 
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
+A "Combined Work" is a work produced by combining or linking an
+Application with the Library. The particular version of the Library
 with which the Combined Work was made is also called the "Linked
 Version".
 
-  The "Minimal Corresponding Source" for a Combined Work means the
+The "Minimal Corresponding Source" for a Combined Work means the
 Corresponding Source for the Combined Work, excluding any source code
 for portions of the Combined Work that, considered in isolation, are
 based on the Application, and not on the Linked Version.
 
-  The "Corresponding Application Code" for a Combined Work means the
+The "Corresponding Application Code" for a Combined Work means the
 object code and/or source code for the Application, including any data
 and utility programs needed for reproducing the Combined Work from the
 Application, but excluding the System Libraries of the Combined Work.
 
-  1. Exception to Section 3 of the GNU GPL.
+## 1. Exception to Section 3 of the GNU GPL.
 
-  You may convey a covered work under sections 3 and 4 of this License
+You may convey a covered work under sections 3 and 4 of this License
 without being bound by section 3 of the GNU GPL.
 
-  2. Conveying Modified Versions.
+## 2. Conveying Modified Versions.
 
-  If you modify a copy of the Library, and, in your modifications, a
+If you modify a copy of the Library, and, in your modifications, a
 facility refers to a function or data to be supplied by an Application
 that uses the facility (other than as an argument passed when the
 facility is invoked), then you may convey a copy of the modified
 version:
 
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
+-   a) under this License, provided that you make a good faith effort
+    to ensure that, in the event an Application does not supply the
+    function or data, the facility still operates, and performs
+    whatever part of its purpose remains meaningful, or
+-   b) under the GNU GPL, with none of the additional permissions of
+    this License applicable to that copy.
 
-  3. Object Code Incorporating Material from Library Header Files.
+## 3. Object Code Incorporating Material from Library Header Files.
 
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
+The object code form of an Application may incorporate material from a
+header file that is part of the Library. You may convey such object
 code under terms of your choice, provided that, if the incorporated
 material is not limited to numerical parameters, data structure
 layouts and accessors, or small macros, inline functions and templates
 (ten or fewer lines in length), you do both of the following:
 
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
+-   a) Give prominent notice with each copy of the object code that
+    the Library is used in it and that the Library and its use are
+    covered by this License.
+-   b) Accompany the object code with a copy of the GNU GPL and this
+    license document.
+
+## 4. Combined Works.
+
+You may convey a Combined Work under terms of your choice that, taken
+together, effectively do not restrict modification of the portions of
+the Library contained in the Combined Work and reverse engineering for
+debugging such modifications, if you also do each of the following:
+
+-   a) Give prominent notice with each copy of the Combined Work that
+    the Library is used in it and that the Library and its use are
+    covered by this License.
+-   b) Accompany the Combined Work with a copy of the GNU GPL and this
+    license document.
+-   c) For a Combined Work that displays copyright notices during
+    execution, include the copyright notice for the Library among
+    these notices, as well as a reference directing the user to the
+    copies of the GNU GPL and this license document.
+-   d) Do one of the following:
+    -   0. Convey the Minimal Corresponding Source under the terms of
+           this License, and the Corresponding Application Code in a form
+           suitable for, and under terms that permit, the user to
+           recombine or relink the Application with a modified version of
+           the Linked Version to produce a modified Combined Work, in the
+           manner specified by section 6 of the GNU GPL for conveying
+           Corresponding Source.
+    -   1. Use a suitable shared library mechanism for linking with
+           the Library. A suitable mechanism is one that (a) uses at run
+           time a copy of the Library already present on the user's
+           computer system, and (b) will operate properly with a modified
+           version of the Library that is interface-compatible with the
+           Linked Version.
+-   e) Provide Installation Information, but only if you would
+    otherwise be required to provide such information under section 6
+    of the GNU GPL, and only to the extent that such information is
+    necessary to install and execute a modified version of the
+    Combined Work produced by recombining or relinking the Application
+    with a modified version of the Linked Version. (If you use option
+    4d0, the Installation Information must accompany the Minimal
+    Corresponding Source and Corresponding Application Code. If you
+    use option 4d1, you must provide the Installation Information in
+    the manner specified by section 6 of the GNU GPL for conveying
+    Corresponding Source.)
 
-  5. Combined Libraries.
+## 5. Combined Libraries.
 
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
+You may place library facilities that are a work based on the Library
+side by side in a single library together with other library
 facilities that are not Applications and are not covered by this
 License, and convey such a combined library under terms of your
 choice, if you do both of the following:
 
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
+-   a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities, conveyed under the terms of this License.
+-   b) Give prominent notice with the combined library that part of it
+    is a work based on the Library, and explaining where to find the
+    accompanying uncombined form of the same work.
 
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
+## 6. Revised Versions of the GNU Lesser General Public License.
 
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
+The Free Software Foundation may publish revised and/or new versions
 of the GNU Lesser General Public License from time to time. Such new
 versions will be similar in spirit to the present version, but may
 differ in detail to address new problems or concerns.
 
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
+Each version is given a distinguishing version number. If the Library
+as you received it specifies that a certain numbered version of the
+GNU Lesser General Public License "or any later version" applies to
+it, you have the option of following the terms and conditions either
+of that published version or of any later version published by the
+Free Software Foundation. If the Library as you received it does not
+specify a version number of the GNU Lesser General Public License, you
+may choose any version of the GNU Lesser General Public License ever
+published by the Free Software Foundation.
 
-  If the Library as you received it specifies that a proxy can decide
+If the Library as you received it specifies that a proxy can decide
 whether future versions of the GNU Lesser General Public License shall
 apply, that proxy's public statement of acceptance of any version is
 permanent authorization for you to choose that version for the
 Library.
+
+[FSF]: https://www.fsf.org/
```

### Comparing `pathurl-0.6.0/pyproject.toml` & `pathurl-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,144 +1,174 @@
 [build-system]
-requires = ["poetry_core>=1.0.0"]
+requires = [
+    "poetry_core>=1.0.0",
+]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ["py38"]
+target-version = [
+    "py38",
+]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
 disallow_untyped_defs = true
+extra_checks = true
 ignore_missing_imports = true
 no_implicit_reexport = true
 show_error_codes = true
-strict_concatenate = true
 strict_equality = true
 warn_return_any = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 warn_unused_configs = true
 
 [tool.ruff]
+src = [
+    "src",
+]
+target-version = "py38"
+
+[tool.ruff.lint]
 select = [
     "A",
     "ARG",
+    "ASYNC",
     "B",
     "BLE",
     "C4",
+    "COM",
     "DTZ",
     "E",
+    "EM",
     "ERA",
     "EXE",
     "F",
+    "FA",
     "FBT",
+    "FLY",
     "G",
     "I",
+    "ICN",
     "INP",
     "ISC",
+    "LOG",
     "N",
     "PGH",
+    "PERF",
     "PIE",
     "PLC",
     "PLE",
     "PLW",
     "PT",
     "PTH",
+    "Q",
     "RET",
     "RSE",
     "RUF",
     "S",
     "SIM",
     "SLF",
+    "SLOT",
     "T10",
     "TID",
     "TRY",
     "UP",
     "W",
+    "YTT",
 ]
 ignore = [
+    "COM812",
     "E501",
     "TRY003",
 ]
-src = ["src"]
-target-version = "py38"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**" = [
     "FBT001",
     "PT011",
     "S101",
 ]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.flake8-tidy-imports.banned-api]
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
 "mock".msg = "Use unittest.mock"
 "pytz".msg = "Use zoneinfo"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
-forced-separate = ["tests"]
+forced-separate = [
+    "tests",
+]
 split-on-trailing-comma = false
 
 [tool.pytest.ini_options]
 addopts = "-vv"
 testpaths = "tests"
 
 [tool.coverage.run]
-source = ["src/"]
+source = [
+    "src/",
+]
 data_file = ".cov_cache/coverage.dat"
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "pathurl"
-version = "0.6.0"
+version = "0.7.0"
 description = "url manipulation"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
-readme = "README.rst"
+readme = "docs/README.md"
 
 homepage = "https://pathurl.readthedocs.io/en/stable/"
 repository = "https://github.com/spapanik/pathurl"
 documentation = "https://pathurl.readthedocs.io/en/stable/"
 
-keywords = ["url"]
+keywords = [
+    "url",
+]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 # python version
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
-ipdb = {version = "^0.13", python = "^3.9"}
-ipython = {version = "^8.12", python = "^3.9"}
-pipdeptree = "^2.7"
+ipdb = { version = "^0.13", python = "^3.10" }
+ipython = { version = "^8.21", python = "^3.10" }
+pickleshare = { version = "^0.7", python = "^3.10" }
+pipdeptree = "^2.13"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.3"
-mypy = "^1.4"
-ruff = "^0.0"
+black = "^24.1"
+mypy = "^1.8"
+ruff = "^0.4"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4"
-pytest-cov = "^4.0"
+pytest = "^8.0"
+pytest-cov = "^5.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.2"
-sphinx-rtd-theme = "^1.2"
+mkdocs = "^1.6"
+mkdocs-material = "^9.5"
+mkdocs-material-extensions = "^1.3"
+Pygments = "^2.17"
+pymdown-extensions = "^10.8"
```

### Comparing `pathurl-0.6.0/src/pathurl/path.py` & `pathurl-0.7.0/src/pathurl/path.py`

 * *Files identical despite different names*

### Comparing `pathurl-0.6.0/src/pathurl/query.py` & `pathurl-0.7.0/src/pathurl/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             data.setdefault(key, [])
             if isinstance(value, list):
                 data[key].extend(value)
             else:
                 data[key].append(value)
         return self.__class__(self._dict_to_str(data))
 
-    def set(  # noqa: A003
+    def set(
         self, dict_: dict[str, qs_value] | None = None, **kwargs: qs_value
     ) -> Query:
         data = deepcopy(self._data)
         dict_ = dict(dict_ or {}, **kwargs)
         for key, value in dict_.items():
             data.setdefault(key, [])
             if isinstance(value, list):
```

### Comparing `pathurl-0.6.0/src/pathurl/url.py` & `pathurl-0.7.0/src/pathurl/url.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,9 +148,13 @@
             "query",
             "fragment",
         }
         for part in parts:
             kwargs.setdefault(part, getattr(self, part))
         return self.from_parts(**kwargs)
 
-    def join(self, path: str | Path) -> URL:
-        return self.__class__(urljoin(str(self), str(path)))
+    def join(self, *paths: str | Path) -> URL:
+        result = str(self)
+        for path in paths:
+            result = urljoin(result, str(path))
+
+        return self.__class__(result)
```

### Comparing `pathurl-0.6.0/PKG-INFO` & `pathurl-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,57 @@
 Metadata-Version: 2.1
 Name: pathurl
-Version: 0.6.0
+Version: 0.7.0
 Summary: url manipulation
 Home-page: https://pathurl.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: url
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://pathurl.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/pathurl
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-=============================
-pathurl: object-oriented URLs
-=============================
-
-.. image:: https://github.com/spapanik/pathurl/actions/workflows/tests.yml/badge.svg
-  :alt: Tests
-  :target: https://github.com/spapanik/pathurl/actions/workflows/tests.yml
-.. image:: https://img.shields.io/github/license/spapanik/pathurl
-  :alt: License
-  :target: https://github.com/spapanik/pathurl/blob/main/LICENSE.txt
-.. image:: https://img.shields.io/pypi/v/pathurl
-  :alt: PyPI
-  :target: https://pypi.org/project/pathurl
-.. image:: https://pepy.tech/badge/pathurl
-  :alt: Downloads
-  :target: https://pepy.tech/project/pathurl
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-  :alt: code style: black
-  :target: https://github.com/psf/black
-.. image:: https://img.shields.io/badge/build%20automation-yamk-success
-  :alt: build automation: yam
-  :target: https://github.com/spapanik/yamk
-.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
-  :alt: Lint: ruff
-  :target: https://github.com/charliermarsh/ruff
-
-``pathurl`` is an objected-oriented way of manipulating URLs.
-
-In a nutshell
--------------
-
-Installation
-^^^^^^^^^^^^
-
-The easiest way is to use `poetry`_ to manage your dependencies and add *pathurl* to them.
-
-.. code-block:: toml
-
-    [tool.poetry.dependencies]
-    pathurl = "^0.6.0"
-
-Usage
-^^^^^
-
-``pathurl`` offers classes to manipulate URLs, paths and query strings. All objects are immutable.
-
-Links
------
-
-- `Documentation`_
-- `Changelog`_
-
-
-.. _poetry: https://python-poetry.org/
-.. _Changelog: https://github.com/spapanik/pathurl/blob/main/CHANGELOG.rst
-.. _Documentation: https://pathurl.readthedocs.io/en/latest/
+# pathurl: object-oriented URLs
+
+[![tests][test_badge]][test_url]
+[![license][licence_badge]][licence_url]
+[![pypi][pypi_badge]][pypi_url]
+[![downloads][pepy_badge]][pepy_url]
+[![code style: black][black_badge]][black_url]
+[![build automation: yam][yam_badge]][yam_url]
+[![Lint: ruff][ruff_badge]][ruff_url]
+
+`pathurl` is an objected-oriented way of manipulating URLs.
+
+## Links
+
+-   [Documentation]
+-   [Changelog]
+
+[test_badge]: https://github.com/spapanik/pathurl/actions/workflows/tests.yml/badge.svg
+[test_url]: https://github.com/spapanik/pathurl/actions/workflows/tests.yml
+[licence_badge]: https://img.shields.io/badge/License-LGPL_v3-blue.svg
+[licence_url]: https://github.com/spapanik/pathurl/blob/main/docs/LICENSE.md
+[pypi_badge]: https://img.shields.io/pypi/v/pathurl
+[pypi_url]: https://pypi.org/project/pathurl
+[pepy_badge]: https://pepy.tech/badge/pathurl
+[pepy_url]: https://pepy.tech/project/pathurl
+[black_badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black_url]: https://github.com/psf/black
+[yam_badge]: https://img.shields.io/badge/build%20automation-yamk-success
+[yam_url]: https://github.com/spapanik/yamk
+[ruff_badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+[ruff_url]: https://github.com/charliermarsh/ruff
+[Documentation]: https://pathurl.readthedocs.io/en/stable/
+[Changelog]: https://github.com/spapanik/pathurl/blob/main/docs/CHANGELOG.md
```

