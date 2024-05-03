# Comparing `tmp/pytest-md-report-0.5.1.tar.gz` & `tmp/pytest_md_report-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-md-report-0.5.1.tar", last modified: Sun Feb  4 10:03:00 2024, max compression
+gzip compressed data, was "pytest_md_report-0.6.0.tar", last modified: Fri May  3 16:05:19 2024, max compression
```

## Comparing `pytest-md-report-0.5.1.tar` & `pytest_md_report-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,53 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-04 10:03:00.975761 pytest-md-report-0.5.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      204 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    15394 2024-02-04 10:03:00.975761 pytest-md-report-0.5.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    13563 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      894 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-04 10:03:00.965761 pytest-md-report-0.5.1/pytest_md_report/
--rw-r--r--   0 toor      (1000) toor      (1000)      300 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pytest_md_report/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pytest_md_report/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5071 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pytest_md_report/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4394 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pytest_md_report/_style_filter.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16477 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pytest_md_report/plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/pytest_md_report/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-04 10:03:00.975761 pytest-md-report-0.5.1/pytest_md_report.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    15394 2024-02-04 10:03:00.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      643 2024-02-04 10:03:00.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-02-04 10:03:00.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       54 2024-02-04 10:03:00.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-02-04 10:02:39.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       93 2024-02-04 10:03:00.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2024-02-04 10:03:00.000000 pytest-md-report-0.5.1/pytest_md_report.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-04 10:03:00.965761 pytest-md-report-0.5.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       85 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-02-04 10:03:00.975761 pytest-md-report-0.5.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2982 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-02-04 10:03:00.965761 pytest-md-report-0.5.1/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1034 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/tests/test_option.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8072 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      861 2024-02-04 10:02:23.000000 pytest-md-report-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.709804 pytest_md_report-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.713804 pytest_md_report-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.713804 pytest_md_report-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/gfm_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_xfailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_xpassed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.713804 pytest_md_report-0.6.0/pytest_md_report/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/_style_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/pytest_md_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:05:08.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/ss/
+-rw-r--r--   0 runner    (1001) docker     (127)    75738 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/md-report_exclude_outcomes_verbose_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61742 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/md-report_gha.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/pytest_md_report_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41954 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/pytest_md_report_example_verbose.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tests/test_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tox.ini
```

### Comparing `pytest-md-report-0.5.1/LICENSE` & `pytest_md_report-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.5.1/PKG-INFO` & `pytest_md_report-0.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,37 @@
-Metadata-Version: 2.1
-Name: pytest-md-report
-Version: 0.5.1
-Summary: A pytest plugin to make a test results report with Markdown table format.
-Home-page: https://github.com/thombashi/pytest-md-report
-Author: Tsuyoshi Hombashi
-Author-email: tsuyoshi.hombashi@gmail.com
-License: MIT License
-Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
-Project-URL: Source, https://github.com/thombashi/pytest-md-report
-Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
-Keywords: pytest,plugin,markdown
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Plugins
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: pytablewriter<2,>=1.2.0
-Requires-Dist: pytest!=6.0.0,<9,>=3.3.2
-Requires-Dist: tcolorpy<1,>=0.0.5
-Requires-Dist: typepy<2,>=1.1.1
-Provides-Extra: test
-
 .. contents:: **pytest-md-report**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
-.. image:: https://badge.fury.io/py/pytest-md-report.svg
+|PyPI pkg ver| |Supported Python ver| |Supported Python impl| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pytest-md-report.svg
     :target: https://badge.fury.io/py/pytest-md-report
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pytest-md-report.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pytest-md-report.svg
     :target: https://pypi.org/project/pytest-md-report
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pytest-md-report.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pytest-md-report.svg
     :target: https://pypi.org/project/pytest-md-report
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pytest-md-report/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pytest-md-report/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/pytest-md-report/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
+.. |CodeQL| image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
     :target: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
-A pytest plugin to make test results report with Markdown table format.
-
+A pytest plugin to generate test outcomes reports with markdown table format.
 
 Installation
 ============================================
 ::
 
     pip install pytest-md-report
 
@@ -149,66 +108,127 @@
         [tool:pytest]
         md_report = True
         md_report_verbose = 0
         md_report_color = auto
 
 
 Add report to pull requests
---------------------------------------------
+-----------------------------------------------
 You can add test reports to pull requests by GitHub actions workflow like the below:
 
 .. code-block:: yaml
 
     name: md-report
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
+        permissions:
+          contents: read
+          pull-requests: write
 
         steps:
           - uses: actions/checkout@v4
 
-          - uses: actions/setup-python@v4
+          - uses: actions/setup-python@v5
             with:
-              python-version: '3.11'
+              python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
-            run: pytest --md-report --md-report-flavor gfm --md-report-output md_report.md
+            run: |
+              report_file=md_report.md
+              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
+              pytest --md-report --md-report-flavor gfm --md-report-output "$report_file"
 
           - name: Render reports to the PR when tests fail
             if: failure()
             env:
               GH_TOKEN: ${{ github.token }}
               PR_NUMBER: ${{ github.event.number }}
-            run:
-              gh pr comment $PR_NUMBER --body-file md_report.md 
+            run: |
+              if [ -f "$REPORT_FILE" ]; then
+                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+              fi
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_gha.png
     :scale: 80%
     :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_gha.png
 
     Rendering result
 
 
+Add report to pull requests: only failed tests
+-----------------------------------------------
+You can exclude specific test outcomes from the report by using the ``--md-report-exclude-outcomes`` option.
+The below example excludes ``passed``, ``skipped``, and ``xpassed`` test outcomes from the report and posts the report to the pull request when tests fail with verbose output.
+
+.. code-block:: yaml
+
+    name: md-report
+
+    on:
+      pull_request:
+
+    jobs:
+      run-tests:
+        runs-on: ubuntu-latest
+        permissions:
+          contents: read
+          pull-requests: write
+
+        steps:
+          - uses: actions/checkout@v4
+
+          - uses: actions/setup-python@v5
+            with:
+              python-version: '3.12'
+              cache: pip
+
+          - name: Install dependencies
+            run: pip install --upgrade pytest-md-report
+
+          - name: Run tests
+            run: |
+              report_file=md_report.md
+              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$report_file"
+
+          - name: Render reports to the PR when tests fail
+            if: failure()
+            env:
+              GH_TOKEN: ${{ github.token }}
+              PR_NUMBER: ${{ github.event.number }}
+            run: |
+              if [ -f "$REPORT_FILE" ]; then
+                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+              fi
+
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+    :scale: 80%
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+
+    Rendering result
+
+
 Options
 ============================================
 
 Command options
 --------------------------------------------
 ::
 
-    make test results report with markdown table format:
-      --md-report           Create Markdown report. you can also specify the value
+    generate test outcomes report with markdown table format:
+      --md-report           Create a Markdown report. you can also specify the value
                             with PYTEST_MD_REPORT environment variable.
       --md-report-verbose=VERBOSITY_LEVEL
                             Verbosity level for pytest-md-report.
                             If not set, use the verbosity level of pytest.
                             Defaults to 0.
                             you can also specify the value with
                             PYTEST_MD_REPORT_VERBOSE environment variable.
@@ -238,15 +258,15 @@
                             Defaults to 1.
                             you can also specify the value with
                             PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
                             Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
-                            Automatically set to 'number' when CI environment
+                            Automatically set to 'number' when the CI environment
                             variable is set to
                             TRUE (case insensitive) to display reports correctly at
                             CI services.
                             Defaults to 'number'.
                             you can also specify the value with
                             PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
@@ -277,23 +297,31 @@
                             you can also specify the value with
                             PYTEST_MD_REPORT_ERROR_COLOR environment variable.
       --md-report-flavor={common_mark,github,gfm,jekyll,kramdown}
                             Markdown flavor of the output report.
                             Defaults to 'common_mark'.
                             you can also specify the value with
                             PYTEST_MD_REPORT_FLAVOR environment variable.
+      --md-report-exclude-outcomes=MD_REPORT_EXCLUDE_OUTCOMES [MD_REPORT_EXCLUDE_OUTCOMES ...]
+                            List of test outcomes to exclude from the report.
+                            When specifying as an environment variable, pass a
+                            comma-separated string
+                            (e.g. 'passed,skipped').
+                            Defaults to '[]'.
+                            you can also specify the value with
+                            PYTEST_MD_REPORT_EXCLUDE_OUTCOMES environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
-  md_report (bool):     Create Markdown report.
+  md_report (bool):     Create a Markdown report.
   md_report_verbose (string):
                         Verbosity level for pytest-md-report. If not set, use
                         the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
                         How coloring output reports. auto: detect the output
                         destination and colorize reports appropriately with the
                         output. for terminal output, render colored (text and
@@ -307,15 +335,15 @@
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
                         Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
                         Rendering method for results of zero values. number:
                         render as a digit number (0). empty: not rendering.
-                        Automatically set to 'number' when CI environment
+                        Automatically set to 'number' when the CI environment
                         variable is set to TRUE (case insensitive) to display
                         reports correctly at CI services. Defaults to 'number'.
   md_report_success_color (string):
                         Text color of succeeded results. Specify a color name
                         (one of the black/red/green/yellow/blue/magenta/cyan/whi
                         te/lightblack/lightred/lightgreen/lightyellow/lightblue/
                         lightmagenta/lightcyan/lightwhite) or a color code (e.g.
@@ -331,13 +359,18 @@
                         of the black/red/green/yellow/blue/magenta/cyan/white/li
                         ghtblack/lightred/lightgreen/lightyellow/lightblue/light
                         magenta/lightcyan/lightwhite) or a color code (e.g.
                         #ff1020). Defaults to 'light_red'.
   md_report_flavor (string):
                         Markdown flavor of the output report. Defaults to
                         'common_mark'.
+  md_report_exclude_outcomes (args):
+                        List of test outcomes to exclude from the report. When
+                        specifying as an environment variable, pass a
+                        comma-separated string (e.g. 'passed,skipped'). Defaults
+                        to '[]'.
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.5.1/README.rst` & `pytest_md_report-0.6.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,79 @@
+Metadata-Version: 2.1
+Name: pytest-md-report
+Version: 0.6.0
+Summary: A pytest plugin to generate test outcomes reports with markdown table format.
+Home-page: https://github.com/thombashi/pytest-md-report
+Author: Tsuyoshi Hombashi
+Author-email: tsuyoshi.hombashi@gmail.com
+License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
+Project-URL: Source, https://github.com/thombashi/pytest-md-report
+Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
+Keywords: pytest,plugin,markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: pytablewriter<2,>=1.2.0
+Requires-Dist: pytest!=6.0.0,<9,>=3.3.2
+Requires-Dist: tcolorpy<1,>=0.0.5
+Requires-Dist: typepy<2,>=1.1.1
+Provides-Extra: test
+
 .. contents:: **pytest-md-report**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
-.. image:: https://badge.fury.io/py/pytest-md-report.svg
+|PyPI pkg ver| |Supported Python ver| |Supported Python impl| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pytest-md-report.svg
     :target: https://badge.fury.io/py/pytest-md-report
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pytest-md-report.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pytest-md-report.svg
     :target: https://pypi.org/project/pytest-md-report
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pytest-md-report.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pytest-md-report.svg
     :target: https://pypi.org/project/pytest-md-report
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pytest-md-report/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pytest-md-report/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/pytest-md-report/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
+.. |CodeQL| image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
     :target: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
-A pytest plugin to make test results report with Markdown table format.
-
+A pytest plugin to generate test outcomes reports with markdown table format.
 
 Installation
 ============================================
 ::
 
     pip install pytest-md-report
 
@@ -107,66 +150,127 @@
         [tool:pytest]
         md_report = True
         md_report_verbose = 0
         md_report_color = auto
 
 
 Add report to pull requests
---------------------------------------------
+-----------------------------------------------
 You can add test reports to pull requests by GitHub actions workflow like the below:
 
 .. code-block:: yaml
 
     name: md-report
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
+        permissions:
+          contents: read
+          pull-requests: write
 
         steps:
           - uses: actions/checkout@v4
 
-          - uses: actions/setup-python@v4
+          - uses: actions/setup-python@v5
             with:
-              python-version: '3.11'
+              python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
-            run: pytest --md-report --md-report-flavor gfm --md-report-output md_report.md
+            run: |
+              report_file=md_report.md
+              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
+              pytest --md-report --md-report-flavor gfm --md-report-output "$report_file"
 
           - name: Render reports to the PR when tests fail
             if: failure()
             env:
               GH_TOKEN: ${{ github.token }}
               PR_NUMBER: ${{ github.event.number }}
-            run:
-              gh pr comment $PR_NUMBER --body-file md_report.md 
+            run: |
+              if [ -f "$REPORT_FILE" ]; then
+                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+              fi
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_gha.png
     :scale: 80%
     :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_gha.png
 
     Rendering result
 
 
+Add report to pull requests: only failed tests
+-----------------------------------------------
+You can exclude specific test outcomes from the report by using the ``--md-report-exclude-outcomes`` option.
+The below example excludes ``passed``, ``skipped``, and ``xpassed`` test outcomes from the report and posts the report to the pull request when tests fail with verbose output.
+
+.. code-block:: yaml
+
+    name: md-report
+
+    on:
+      pull_request:
+
+    jobs:
+      run-tests:
+        runs-on: ubuntu-latest
+        permissions:
+          contents: read
+          pull-requests: write
+
+        steps:
+          - uses: actions/checkout@v4
+
+          - uses: actions/setup-python@v5
+            with:
+              python-version: '3.12'
+              cache: pip
+
+          - name: Install dependencies
+            run: pip install --upgrade pytest-md-report
+
+          - name: Run tests
+            run: |
+              report_file=md_report.md
+              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$report_file"
+
+          - name: Render reports to the PR when tests fail
+            if: failure()
+            env:
+              GH_TOKEN: ${{ github.token }}
+              PR_NUMBER: ${{ github.event.number }}
+            run: |
+              if [ -f "$REPORT_FILE" ]; then
+                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+              fi
+
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+    :scale: 80%
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+
+    Rendering result
+
+
 Options
 ============================================
 
 Command options
 --------------------------------------------
 ::
 
-    make test results report with markdown table format:
-      --md-report           Create Markdown report. you can also specify the value
+    generate test outcomes report with markdown table format:
+      --md-report           Create a Markdown report. you can also specify the value
                             with PYTEST_MD_REPORT environment variable.
       --md-report-verbose=VERBOSITY_LEVEL
                             Verbosity level for pytest-md-report.
                             If not set, use the verbosity level of pytest.
                             Defaults to 0.
                             you can also specify the value with
                             PYTEST_MD_REPORT_VERBOSE environment variable.
@@ -196,15 +300,15 @@
                             Defaults to 1.
                             you can also specify the value with
                             PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
                             Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
-                            Automatically set to 'number' when CI environment
+                            Automatically set to 'number' when the CI environment
                             variable is set to
                             TRUE (case insensitive) to display reports correctly at
                             CI services.
                             Defaults to 'number'.
                             you can also specify the value with
                             PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
@@ -235,23 +339,31 @@
                             you can also specify the value with
                             PYTEST_MD_REPORT_ERROR_COLOR environment variable.
       --md-report-flavor={common_mark,github,gfm,jekyll,kramdown}
                             Markdown flavor of the output report.
                             Defaults to 'common_mark'.
                             you can also specify the value with
                             PYTEST_MD_REPORT_FLAVOR environment variable.
+      --md-report-exclude-outcomes=MD_REPORT_EXCLUDE_OUTCOMES [MD_REPORT_EXCLUDE_OUTCOMES ...]
+                            List of test outcomes to exclude from the report.
+                            When specifying as an environment variable, pass a
+                            comma-separated string
+                            (e.g. 'passed,skipped').
+                            Defaults to '[]'.
+                            you can also specify the value with
+                            PYTEST_MD_REPORT_EXCLUDE_OUTCOMES environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
-  md_report (bool):     Create Markdown report.
+  md_report (bool):     Create a Markdown report.
   md_report_verbose (string):
                         Verbosity level for pytest-md-report. If not set, use
                         the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
                         How coloring output reports. auto: detect the output
                         destination and colorize reports appropriately with the
                         output. for terminal output, render colored (text and
@@ -265,15 +377,15 @@
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
                         Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
                         Rendering method for results of zero values. number:
                         render as a digit number (0). empty: not rendering.
-                        Automatically set to 'number' when CI environment
+                        Automatically set to 'number' when the CI environment
                         variable is set to TRUE (case insensitive) to display
                         reports correctly at CI services. Defaults to 'number'.
   md_report_success_color (string):
                         Text color of succeeded results. Specify a color name
                         (one of the black/red/green/yellow/blue/magenta/cyan/whi
                         te/lightblack/lightred/lightgreen/lightyellow/lightblue/
                         lightmagenta/lightcyan/lightwhite) or a color code (e.g.
@@ -289,13 +401,18 @@
                         of the black/red/green/yellow/blue/magenta/cyan/white/li
                         ghtblack/lightred/lightgreen/lightyellow/lightblue/light
                         magenta/lightcyan/lightwhite) or a color code (e.g.
                         #ff1020). Defaults to 'light_red'.
   md_report_flavor (string):
                         Markdown flavor of the output report. Defaults to
                         'common_mark'.
+  md_report_exclude_outcomes (args):
+                        List of test outcomes to exclude from the report. When
+                        specifying as an environment variable, pass a
+                        comma-separated string (e.g. 'passed,skipped'). Defaults
+                        to '[]'.
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.5.1/pyproject.toml` & `pytest_md_report-0.6.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+requires = [
+  "setuptools>=64",
+  "setuptools_scm>=7,<8; python_version<'3.8'",
+  "setuptools_scm>=8; python_version>='3.8'",
+]
+
+[tool.setuptools_scm]
+version_scheme = "guess-next-dev"
+local_scheme = "no-local-version"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -45,11 +53,35 @@
 show_error_codes = true
 show_error_context = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    ".tox",
+    ".venv",
+    "_build",
+    "_sandbox",
+    "build",
+    "dist"
+]
+pythonVersion = "3.7"
+
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
+
+[tool.ruff]
+line-length = 100
+target-version = "py37"
+exclude = [
+    ".eggs/",
+    ".tox/",
+    "_sandbox/*",
+    "build/",
+    "docs/conf.py",
+]
```

### Comparing `pytest-md-report-0.5.1/pytest_md_report/_const.py` & `pytest_md_report-0.6.0/pytest_md_report/_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum, unique
 from textwrap import dedent
+from typing import List
 
 from pytablewriter.writer.text import MarkdownFlavor
 from tcolorpy import AnsiFGColor
 
 
 COLOR_NAMES = "/".join([style.name.lower() for style in list(AnsiFGColor)])
 
@@ -40,28 +41,29 @@
 
 
 class Default:
     COLOR_POLICY = ColorPolicy.AUTO
     MARGIN = 1
     MARKDOWN_FLAVOR = MarkdownFlavor.COMMON_MARK
     ZEROS = ZerosRender.NUMBER
+    EXCLUDE_RESULTS: List[str] = []
 
     class FGColor:
         SUCCESS = "light_green"
         ERROR = "light_red"
         SKIP = "light_yellow"
         GRAYOUT = "light_black"
 
 
 OPTION_PREFIX = "md-report"
 
 
 @unique
 class Option(Enum):
-    MD_REPORT = (OPTION_PREFIX, "Create Markdown report.")
+    MD_REPORT = (OPTION_PREFIX, "Create a Markdown report.")
     MD_REPORT_VERBOSE = (
         f"{OPTION_PREFIX}-verbose",
         dedent(
             """\
             Verbosity level for pytest-md-report.
             If not set, use the verbosity level of pytest.
             Defaults to 0.
@@ -107,15 +109,15 @@
     MD_REPORT_ZEROS = (
         f"{OPTION_PREFIX}-zeros",
         dedent(
             """\
             Rendering method for results of zero values.
             number: render as a digit number (0).
             empty: not rendering.
-            Automatically set to 'number' when CI environment variable is set to
+            Automatically set to 'number' when the CI environment variable is set to
             TRUE (case insensitive) to display reports correctly at CI services.
             Defaults to '{default}'.
             """
         ).format(default=Default.ZEROS),
     )
     MD_REPORT_SUCCESS_COLOR = (
         f"{OPTION_PREFIX}-success-color",
@@ -154,14 +156,27 @@
             Markdown flavor of the output report.
             Defaults to '{default}'.
             """
         ).format(
             default=Default.MARKDOWN_FLAVOR.value,
         ),
     )
+    MD_EXCLUDE_OUTCOMES = (
+        f"{OPTION_PREFIX}-exclude-outcomes",
+        dedent(
+            """\
+            List of test outcomes to exclude from the report.
+            When specifying as an environment variable, pass a comma-separated string
+            (e.g. 'passed,skipped').
+            Defaults to '{default}'.
+            """
+        ).format(
+            default=Default.EXCLUDE_RESULTS,
+        ),
+    )
 
     @property
     def cmdoption_str(self) -> str:
         return "--" + self.__name.lower()
 
     @property
     def envvar_str(self) -> str:
```

### Comparing `pytest-md-report-0.5.1/pytest_md_report/_style_filter.py` & `pytest_md_report-0.6.0/pytest_md_report/_style_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from pytablewriter.writer import AbstractTableWriter
 
 from ._const import BGColor, ColorPolicy, FGColor, Header
 
 
 class ColorRetriever:
     def __init__(
-        self, row: int, is_grayout: bool, color_polilcy: ColorPolicy, color_map: Dict[str, str]
+        self,
+        row: int,
+        is_grayout: bool,
+        color_polilcy: ColorPolicy,
+        color_map: Dict[str, str],
     ) -> None:
         self.__row = row
         self.__is_grayout = is_grayout
         self.__color_polilcy = color_polilcy
         self.__color_map = color_map
 
     def retrieve_fg_bg_color(self, base_color: str) -> Tuple[str, Optional[str]]:
```

### Comparing `pytest-md-report-0.5.1/pytest_md_report/plugin.py` & `pytest_md_report-0.6.0/pytest_md_report/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from collections import defaultdict
-from typing import Any, Dict, Mapping, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple
 
 from _pytest.config import Config
 from _pytest.config.argparsing import Parser
 from _pytest.terminal import TerminalReporter
 from pytablewriter import TableWriterFactory
 from pytablewriter.writer.text import MarkdownFlavor, normalize_md_flavor
 from typepy import Bool, Integer, StrictLevel, is_not_null_string
@@ -18,15 +18,15 @@
     if value == 0:
         return ""
 
     return value
 
 
 def pytest_addoption(parser: Parser) -> None:
-    group = parser.getgroup("md report", "make test results report with markdown table format")
+    group = parser.getgroup("md report", "generate test outcomes report with markdown table format")
 
     group.addoption(
         Option.MD_REPORT.cmdoption_str,
         action="store_true",
         default=None,
         help=Option.MD_REPORT.help_msg
         + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.MD_REPORT.envvar_str),
@@ -96,35 +96,57 @@
     group.addoption(
         Option.MD_REPORT_FLAVOR.cmdoption_str,
         choices=[flavor.value for flavor in MarkdownFlavor],
         default=None,
         help=Option.MD_REPORT_FLAVOR.help_msg
         + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.MD_REPORT_FLAVOR.envvar_str),
     )
+    group.addoption(
+        Option.MD_EXCLUDE_OUTCOMES.cmdoption_str,
+        nargs="+",
+        default=[],
+        help=Option.MD_EXCLUDE_OUTCOMES.help_msg
+        + HelpMsg.EXTRA_MSG_TEMPLATE.format(Option.MD_EXCLUDE_OUTCOMES.envvar_str),
+    )
 
     parser.addini(
-        Option.MD_REPORT.inioption_str, type="bool", default=False, help=Option.MD_REPORT.help_msg
+        Option.MD_REPORT.inioption_str,
+        type="bool",
+        default=False,
+        help=Option.MD_REPORT.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_VERBOSE.inioption_str, default=None, help=Option.MD_REPORT_VERBOSE.help_msg
+        Option.MD_REPORT_VERBOSE.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_VERBOSE.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_COLOR.inioption_str, default=None, help=Option.MD_REPORT_COLOR.help_msg
+        Option.MD_REPORT_COLOR.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_COLOR.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_OUTPUT.inioption_str, default=None, help=Option.MD_REPORT_OUTPUT.help_msg
+        Option.MD_REPORT_OUTPUT.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_OUTPUT.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_TEE.inioption_str, default=None, help=Option.MD_REPORT_TEE.help_msg
+        Option.MD_REPORT_TEE.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_TEE.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_MARGIN.inioption_str, default=None, help=Option.MD_REPORT_MARGIN.help_msg
+        Option.MD_REPORT_MARGIN.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_MARGIN.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_ZEROS.inioption_str, default=None, help=Option.MD_REPORT_ZEROS.help_msg
+        Option.MD_REPORT_ZEROS.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_ZEROS.help_msg,
     )
     parser.addini(
         Option.MD_REPORT_SUCCESS_COLOR.inioption_str,
         default=None,
         help=Option.MD_REPORT_SUCCESS_COLOR.help_msg,
     )
     parser.addini(
@@ -134,34 +156,37 @@
     )
     parser.addini(
         Option.MD_REPORT_ERROR_COLOR.inioption_str,
         default=None,
         help=Option.MD_REPORT_ERROR_COLOR.help_msg,
     )
     parser.addini(
-        Option.MD_REPORT_FLAVOR.inioption_str, default=None, help=Option.MD_REPORT_FLAVOR.help_msg
+        Option.MD_REPORT_FLAVOR.inioption_str,
+        default=None,
+        help=Option.MD_REPORT_FLAVOR.help_msg,
+    )
+    parser.addini(
+        Option.MD_EXCLUDE_OUTCOMES.inioption_str,
+        type="args",
+        default=[],
+        help=Option.MD_EXCLUDE_OUTCOMES.help_msg,
     )
 
 
 def is_make_md_report(config: Config) -> bool:
     if config.option.help:
         return False
 
     make_report: Optional[bool] = config.option.md_report
 
     if make_report is None:
-        try:
-            make_report = Bool(
-                os.environ.get(Option.MD_REPORT.envvar_str), strict_level=StrictLevel.MIN
-            ).convert()
-        except TypeConversionError:
-            make_report = None
+        make_report = _to_bool(os.environ.get(Option.MD_REPORT.envvar_str))
 
     if make_report is None:
-        make_report = config.getini(Option.MD_REPORT.inioption_str)
+        make_report = _to_bool(config.getini(Option.MD_REPORT.inioption_str))
 
     if make_report is None:
         return False
 
     return make_report
 
 
@@ -202,15 +227,26 @@
     return APPVEYOR.lower() == "true"
 
 
 def _to_int(value: Any) -> Optional[int]:
     try:
         return Integer(value, strict_level=StrictLevel.MIN).convert()
     except TypeConversionError:
-        return None
+        pass
+
+    return None
+
+
+def _to_bool(value: Any) -> Optional[bool]:
+    try:
+        return Bool(value, strict_level=StrictLevel.MIN).convert()
+    except TypeConversionError:
+        pass
+
+    return None
 
 
 def retrieve_verbosity_level(config: Config) -> int:
     verbosity_level: Optional[int] = config.option.md_report_verbose
 
     if verbosity_level is not None and verbosity_level < 0:
         verbosity_level = None
@@ -218,27 +254,32 @@
     if verbosity_level is None:
         verbosity_level = _to_int(os.environ.get(Option.MD_REPORT_VERBOSE.envvar_str))
 
     if verbosity_level is None:
         verbosity_level = _to_int(config.getini(Option.MD_REPORT_VERBOSE.inioption_str))
 
     if verbosity_level is None:
-        verbosity_level = config.option.verbose
+        # use the verbosity level of the pytest if not set
+        return config.option.verbose
 
     return verbosity_level
 
 
 def retrieve_output_filepath(config: Config) -> Optional[str]:
     output_filepath: Optional[str] = config.option.md_report_output
 
     if not output_filepath:
         output_filepath = os.environ.get(Option.MD_REPORT_OUTPUT.envvar_str)
 
     if not output_filepath:
-        output_filepath = config.getini(Option.MD_REPORT_OUTPUT.inioption_str)
+        value = config.getini(Option.MD_REPORT_OUTPUT.inioption_str)
+        if value is None:
+            return None
+        else:
+            return str(value)
 
     return output_filepath
 
 
 def retrieve_tee(config: Config) -> bool:
     tee: Optional[bool] = config.option.md_report_tee
 
@@ -263,30 +304,57 @@
 
     if not md_flavor:
         md_flavor = config.getini(Option.MD_REPORT_FLAVOR.inioption_str)
 
     if not md_flavor:
         return Default.MARKDOWN_FLAVOR
 
-    return normalize_md_flavor(md_flavor)
+    return normalize_md_flavor(str(md_flavor))
+
+
+def retrieve_exclude_outcomes(config: Config) -> List[str]:
+    def norm_names(names: Sequence[Any]) -> List[str]:
+        return [str(name).lower().strip() for name in names]
+
+    exclude_outcomes = config.option.md_report_exclude_outcomes
+
+    if not exclude_outcomes:
+        exclude_outcomes = os.environ.get(Option.MD_EXCLUDE_OUTCOMES.envvar_str)
+        if exclude_outcomes:
+            return norm_names(exclude_outcomes.split(","))
+
+    if not exclude_outcomes:
+        exclude_outcomes = config.getini(Option.MD_EXCLUDE_OUTCOMES.inioption_str)
+
+    if not exclude_outcomes:
+        return Default.EXCLUDE_RESULTS
+
+    if isinstance(exclude_outcomes, list):
+        # list will be passed via pytest config file
+        return norm_names(exclude_outcomes)
+    elif isinstance(exclude_outcomes, str):
+        # comma-separated string (e.g. passed,skipped) will be passed via the command line option
+        return norm_names(exclude_outcomes.split(","))
+
+    raise TypeError(f"Unexpected type {type(exclude_outcomes)} for exclude_outcomes")
 
 
 def retrieve_color_policy(config: Config) -> ColorPolicy:
     color_policy = config.option.md_report_color
 
     if not color_policy:
         color_policy = os.environ.get(Option.MD_REPORT_COLOR.envvar_str)
 
     if not color_policy:
         color_policy = config.getini(Option.MD_REPORT_COLOR.inioption_str)
 
     if not color_policy:
         return Default.COLOR_POLICY
 
-    return ColorPolicy[color_policy.upper()]
+    return ColorPolicy[str(color_policy).upper()]
 
 
 def retrieve_report_margin(config: Config) -> int:
     margin = config.option.md_report_margin
 
     if margin is None:
         margin = _to_int(os.environ.get(Option.MD_REPORT_MARGIN.envvar_str))
@@ -311,30 +379,30 @@
 
     if _is_ci():
         report_zeros = ZerosRender.NUMBER
 
     if not report_zeros:
         report_zeros = Default.ZEROS
 
-    return report_zeros
+    return str(report_zeros)
 
 
 def retrieve_report_results_color(config: Config, color_option: Option, default: str) -> str:
     results_color = getattr(config.option, color_option.inioption_str)
 
     if not results_color:
         results_color = os.environ.get(color_option.envvar_str)
 
     if not results_color:
         results_color = config.getini(color_option.inioption_str)
 
     if not results_color:
         results_color = default
 
-    return results_color
+    return str(results_color)
 
 
 def _normalize_stat_name(name: str) -> str:
     if name == "error":
         return "errors"
 
     return name
@@ -367,34 +435,43 @@
 
             testfunc = value.head_line.split("[")[0]
 
             if verbosity_level == 0:
                 key: Tuple = (filesystempath,)
             elif verbosity_level >= 1:
                 key = (filesystempath, testfunc)
+            else:
+                continue
 
             if key not in results_per_testfunc:
                 results_per_testfunc[key] = defaultdict(int)
+
             results_per_testfunc[key][stat_key] += 1
 
     return results_per_testfunc
 
 
 def make_md_report(
     config: Config,
     reporter: TerminalReporter,
     total_stats: Mapping[str, int],
     color_policy: ColorPolicy,
     apply_ansi_escape: bool,
     md_flavor: MarkdownFlavor,
+    exclude_outcomes: List[str],
 ) -> str:
     verbosity_level = retrieve_verbosity_level(config)
 
     outcomes = ["passed", "failed", "error", "skipped", "xfailed", "xpassed"]
+    outcomes = [key for key in outcomes if key not in exclude_outcomes]
     outcomes = [key for key in outcomes if total_stats.get(key, 0) > 0]
+
+    if not outcomes:
+        return ""
+
     results_per_testfunc = extract_pytest_stats(
         reporter=reporter, outcomes=outcomes, verbosity_level=verbosity_level
     )
 
     writer = TableWriterFactory.create_from_format_name(
         "md", flavor=md_flavor.value, colorize_terminal=apply_ansi_escape
     )
@@ -462,19 +539,23 @@
 
 
 def pytest_unconfigure(config: Config) -> None:
     if not is_make_md_report(config):
         return
 
     reporter = config.pluginmanager.get_plugin("terminalreporter")
+    if reporter is None:
+        return
+
     stat_count_map = retrieve_stat_count_map(reporter)
     is_tee = retrieve_tee(config)
     output_filepath = retrieve_output_filepath(config)
     color_policy = retrieve_color_policy(config)
     md_flavor = retrieve_md_flavor(config)
+    exclude_outcomes = retrieve_exclude_outcomes(config)
 
     is_output_term = is_tee or not output_filepath
     is_output_file = is_not_null_string(output_filepath)
     term_color_policy = color_policy
     file_color_policy = extract_file_color_policy(color_policy, is_output_file, md_flavor)
 
     apply_ansi_escape_to_file = is_apply_ansi_escape_to_file(color_policy, is_output_file)
@@ -484,14 +565,15 @@
         term_report = make_md_report(
             config,
             reporter,
             stat_count_map,
             color_policy=term_color_policy,
             apply_ansi_escape=apply_ansi_escape_to_term,
             md_flavor=md_flavor,
+            exclude_outcomes=exclude_outcomes,
         )
         reporter._tw.write(term_report)
 
     if not is_output_file:
         return
 
     file_report = term_report
@@ -506,13 +588,14 @@
         file_report = make_md_report(
             config,
             reporter,
             stat_count_map,
             color_policy=file_color_policy,
             apply_ansi_escape=apply_ansi_escape_to_file,
             md_flavor=md_flavor,
+            exclude_outcomes=exclude_outcomes,
         )
 
     if file_report:
         assert output_filepath
         with open(output_filepath, "w") as f:
             f.write(file_report)
```

### Comparing `pytest-md-report-0.5.1/pytest_md_report.egg-info/PKG-INFO` & `pytest_md_report-0.6.0/pytest_md_report.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.5.1
-Summary: A pytest plugin to make a test results report with Markdown table format.
+Version: 0.6.0
+Summary: A pytest plugin to generate test outcomes reports with markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
 Project-URL: Tracker, https://github.com/thombashi/pytest-md-report/issues
@@ -43,36 +43,37 @@
 .. contents:: **pytest-md-report**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
-.. image:: https://badge.fury.io/py/pytest-md-report.svg
+|PyPI pkg ver| |Supported Python ver| |Supported Python impl| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pytest-md-report.svg
     :target: https://badge.fury.io/py/pytest-md-report
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pytest-md-report.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pytest-md-report.svg
     :target: https://pypi.org/project/pytest-md-report
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pytest-md-report.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pytest-md-report.svg
     :target: https://pypi.org/project/pytest-md-report
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pytest-md-report/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/pytest-md-report/actions?query=workflow%3ATests
-    :alt: Linux/macOS/Windows CI status
+.. |CI status| image:: https://github.com/thombashi/pytest-md-report/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pytest-md-report/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
+.. |CodeQL| image:: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql/badge.svg
     :target: https://github.com/thombashi/pytest-md-report/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
-A pytest plugin to make test results report with Markdown table format.
-
+A pytest plugin to generate test outcomes reports with markdown table format.
 
 Installation
 ============================================
 ::
 
     pip install pytest-md-report
 
@@ -149,66 +150,127 @@
         [tool:pytest]
         md_report = True
         md_report_verbose = 0
         md_report_color = auto
 
 
 Add report to pull requests
---------------------------------------------
+-----------------------------------------------
 You can add test reports to pull requests by GitHub actions workflow like the below:
 
 .. code-block:: yaml
 
     name: md-report
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
+        permissions:
+          contents: read
+          pull-requests: write
 
         steps:
           - uses: actions/checkout@v4
 
-          - uses: actions/setup-python@v4
+          - uses: actions/setup-python@v5
             with:
-              python-version: '3.11'
+              python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
-            run: pytest --md-report --md-report-flavor gfm --md-report-output md_report.md
+            run: |
+              report_file=md_report.md
+              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
+              pytest --md-report --md-report-flavor gfm --md-report-output "$report_file"
 
           - name: Render reports to the PR when tests fail
             if: failure()
             env:
               GH_TOKEN: ${{ github.token }}
               PR_NUMBER: ${{ github.event.number }}
-            run:
-              gh pr comment $PR_NUMBER --body-file md_report.md 
+            run: |
+              if [ -f "$REPORT_FILE" ]; then
+                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+              fi
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_gha.png
     :scale: 80%
     :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_gha.png
 
     Rendering result
 
 
+Add report to pull requests: only failed tests
+-----------------------------------------------
+You can exclude specific test outcomes from the report by using the ``--md-report-exclude-outcomes`` option.
+The below example excludes ``passed``, ``skipped``, and ``xpassed`` test outcomes from the report and posts the report to the pull request when tests fail with verbose output.
+
+.. code-block:: yaml
+
+    name: md-report
+
+    on:
+      pull_request:
+
+    jobs:
+      run-tests:
+        runs-on: ubuntu-latest
+        permissions:
+          contents: read
+          pull-requests: write
+
+        steps:
+          - uses: actions/checkout@v4
+
+          - uses: actions/setup-python@v5
+            with:
+              python-version: '3.12'
+              cache: pip
+
+          - name: Install dependencies
+            run: pip install --upgrade pytest-md-report
+
+          - name: Run tests
+            run: |
+              report_file=md_report.md
+              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$report_file"
+
+          - name: Render reports to the PR when tests fail
+            if: failure()
+            env:
+              GH_TOKEN: ${{ github.token }}
+              PR_NUMBER: ${{ github.event.number }}
+            run: |
+              if [ -f "$REPORT_FILE" ]; then
+                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+              fi
+
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+    :scale: 80%
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+
+    Rendering result
+
+
 Options
 ============================================
 
 Command options
 --------------------------------------------
 ::
 
-    make test results report with markdown table format:
-      --md-report           Create Markdown report. you can also specify the value
+    generate test outcomes report with markdown table format:
+      --md-report           Create a Markdown report. you can also specify the value
                             with PYTEST_MD_REPORT environment variable.
       --md-report-verbose=VERBOSITY_LEVEL
                             Verbosity level for pytest-md-report.
                             If not set, use the verbosity level of pytest.
                             Defaults to 0.
                             you can also specify the value with
                             PYTEST_MD_REPORT_VERBOSE environment variable.
@@ -238,15 +300,15 @@
                             Defaults to 1.
                             you can also specify the value with
                             PYTEST_MD_REPORT_MARGIN environment variable.
       --md-report-zeros={number,empty}
                             Rendering method for results of zero values.
                             number: render as a digit number (0).
                             empty: not rendering.
-                            Automatically set to 'number' when CI environment
+                            Automatically set to 'number' when the CI environment
                             variable is set to
                             TRUE (case insensitive) to display reports correctly at
                             CI services.
                             Defaults to 'number'.
                             you can also specify the value with
                             PYTEST_MD_REPORT_ZEROS environment variable.
       --md-report-success-color=MD_REPORT_SUCCESS_COLOR
@@ -277,23 +339,31 @@
                             you can also specify the value with
                             PYTEST_MD_REPORT_ERROR_COLOR environment variable.
       --md-report-flavor={common_mark,github,gfm,jekyll,kramdown}
                             Markdown flavor of the output report.
                             Defaults to 'common_mark'.
                             you can also specify the value with
                             PYTEST_MD_REPORT_FLAVOR environment variable.
+      --md-report-exclude-outcomes=MD_REPORT_EXCLUDE_OUTCOMES [MD_REPORT_EXCLUDE_OUTCOMES ...]
+                            List of test outcomes to exclude from the report.
+                            When specifying as an environment variable, pass a
+                            comma-separated string
+                            (e.g. 'passed,skipped').
+                            Defaults to '[]'.
+                            you can also specify the value with
+                            PYTEST_MD_REPORT_EXCLUDE_OUTCOMES environment variable.
 
 
 ini-options
 --------------------------------------------
 [pytest] ini-options in the first ``pytest.ini``/``tox.ini``/``setup.cfg``/``pyproject.toml (pytest 6.0.0 or later)`` file found:
 
 ::
 
-  md_report (bool):     Create Markdown report.
+  md_report (bool):     Create a Markdown report.
   md_report_verbose (string):
                         Verbosity level for pytest-md-report. If not set, use
                         the verbosity level of pytest. Defaults to 0.
   md_report_color (string):
                         How coloring output reports. auto: detect the output
                         destination and colorize reports appropriately with the
                         output. for terminal output, render colored (text and
@@ -307,15 +377,15 @@
   md_report_tee (string):
                         output test report for both standard output and a file.
   md_report_margin (string):
                         Margin size for each cell. Defaults to 1.
   md_report_zeros (string):
                         Rendering method for results of zero values. number:
                         render as a digit number (0). empty: not rendering.
-                        Automatically set to 'number' when CI environment
+                        Automatically set to 'number' when the CI environment
                         variable is set to TRUE (case insensitive) to display
                         reports correctly at CI services. Defaults to 'number'.
   md_report_success_color (string):
                         Text color of succeeded results. Specify a color name
                         (one of the black/red/green/yellow/blue/magenta/cyan/whi
                         te/lightblack/lightred/lightgreen/lightyellow/lightblue/
                         lightmagenta/lightcyan/lightwhite) or a color code (e.g.
@@ -331,13 +401,18 @@
                         of the black/red/green/yellow/blue/magenta/cyan/white/li
                         ghtblack/lightred/lightgreen/lightyellow/lightblue/light
                         magenta/lightcyan/lightwhite) or a color code (e.g.
                         #ff1020). Defaults to 'light_red'.
   md_report_flavor (string):
                         Markdown flavor of the output report. Defaults to
                         'common_mark'.
+  md_report_exclude_outcomes (args):
+                        List of test outcomes to exclude from the report. When
+                        specifying as an environment variable, pass a
+                        comma-separated string (e.g. 'passed,skipped'). Defaults
+                        to '[]'.
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-md-report/network/dependencies>`__
```

### Comparing `pytest-md-report-0.5.1/setup.py` & `pytest_md_report-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,18 @@
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
-    description="A pytest plugin to make a test results report with Markdown table format.",
+    description="A pytest plugin to generate test outcomes reports with markdown table format.",
     include_package_data=True,
     keywords=["pytest", "plugin", "markdown"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(),
     package_data={MODULE_NAME: ["py.typed"]},
```

### Comparing `pytest-md-report-0.5.1/tests/test_option.py` & `pytest_md_report-0.6.0/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pytest-md-report-0.5.1/tests/test_plugin.py` & `pytest_md_report-0.6.0/tests/test_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,15 +137,19 @@
         |            filepath             | passed | failed | error | skipped | xfailed | xpassed | SUBTOTAL |
         | ------------------------------- | -----: | -----: | ----: | ------: | ------: | ------: | -------: |
         | test_pytest_md_report_output.py |      1 |      1 |     1 |       1 |       1 |       1 |        6 |
         | TOTAL                           |      1 |      1 |     1 |       1 |       1 |       1 |        6 |"""
     )
     output_filepath = testdir.tmpdir.join("report.md")
     result = testdir.runpytest(
-        "--md-report", "--md-report-color", "never", "--md-report-output", output_filepath
+        "--md-report",
+        "--md-report-color",
+        "never",
+        "--md-report-output",
+        output_filepath,
     )
     out = "\n".join(result.outlines[-4:])
     assert out != expected
     with open(output_filepath) as f:
         assert f.read().strip() == expected
 
     result = testdir.runpytest(
@@ -234,7 +238,33 @@
             == r"""|    filepath     | $$\textcolor{#23d18b}{\tt{passed}}$$ | $$\textcolor{#f5f543}{\tt{skipped}}$$ | SUBTOTAL |
 | --------------- | --------------------------------: | --------------------------------: | -------: |
 | $$\textcolor{#23d18b}{\tt{test\\_passed.py}}$$ |   $$\textcolor{#23d18b}{\tt{1}}$$ |   $$\textcolor{#666666}{\tt{0}}$$ | $$\textcolor{#23d18b}{\tt{1}}$$ |
 | $$\textcolor{#f5f543}{\tt{test\\_skipped.py}}$$ |   $$\textcolor{#666666}{\tt{0}}$$ |   $$\textcolor{#f5f543}{\tt{1}}$$ | $$\textcolor{#f5f543}{\tt{1}}$$ |
 | $$\textcolor{#f5f543}{\tt{TOTAL}}$$ |   $$\textcolor{#23d18b}{\tt{1}}$$ |   $$\textcolor{#f5f543}{\tt{1}}$$ | $$\textcolor{#f5f543}{\tt{2}}$$ |
 """
         )
+
+
+def test_pytest_md_report_exclude_outcomes(testdir):
+    testdir.makepyfile(PYFILE_MIX_TESTS)
+    expected = dedent(
+        """\
+        |                 filepath                  | failed | error | xfailed | SUBTOTAL |
+        | ----------------------------------------- | -----: | ----: | ------: | -------: |
+        | test_pytest_md_report_exclude_outcomes.py |      1 |     1 |       1 |        3 |
+        | TOTAL                                     |      1 |     1 |       1 |        6 |
+        """
+    )
+    output_filepath = testdir.tmpdir.join("report.md")
+    testdir.runpytest(
+        "--md-report",
+        "--md-report-exclude-outcomes",
+        "passed",
+        "skipped",
+        "xpassed",
+        "--md-report-output",
+        output_filepath,
+    )
+    with open(output_filepath) as f:
+        report = f.read()
+        print(report)
+        assert report == expected
```

### Comparing `pytest-md-report-0.5.1/tox.ini` & `pytest_md_report-0.6.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -11,41 +11,63 @@
     test
 commands =
     pytest tests {posargs}
 
 [testenv:build]
 deps =
     build>=1
-    twine
+    ; twine
     wheel
 commands =
     python -m build
-    twine check dist/*.whl dist/*.tar.gz
+    ; twine check dist/*.whl dist/*.tar.gz
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
-[testenv:fmt]
+[testenv:fmt-black]
 skip_install = true
 deps =
     autoflake>=2
-    black>=23.1
+    black>=24.1
     isort>=5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
     black setup.py examples tests pytest_md_report
 
-[testenv:lint]
+[testenv:fmt]
 skip_install = true
 deps =
+    autoflake>=2
+    isort>=5
+    ruff>=0.3.5
+commands =
+    autoflake --in-place --recursive --remove-all-unused-imports .
+    isort .
+    ruff format
+
+[testenv:lint]
+extras =
+    test
+deps =
     codespell>=2
     mypy>=1
-    pylama>=8.4.1
+    pyright>=1.1
+    releasecmd
+    ruff>=0.3.5
 commands =
     mypy pytest_md_report setup.py
-    pylama
+    pyright
     - codespell pytest_md_report examples tests -q 2 --check-filenames
+    ruff format --check
+    ruff check
+
+[testenv:release]
+deps =
+    releasecmd
+commands =
+    python setup.py release --sign --skip-uploading --verbose --search-dir pytest_md_report
```

