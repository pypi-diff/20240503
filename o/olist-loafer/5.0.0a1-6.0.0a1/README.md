# Comparing `tmp/olist_loafer-5.0.0a1.tar.gz` & `tmp/olist_loafer-6.0.0a1.tar.gz`

## Comparing `olist_loafer-5.0.0a1.tar` & `olist_loafer-6.0.0a1.tar`

### file list

```diff
@@ -1,72 +1,48 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/.editorconfig
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/CHANGES.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/CONTRIBUTORS.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/MANIFEST.in
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/env.local
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/Makefile
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/changelog.rst
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/conf.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/contributors.rst
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/error_handlers.rst
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/exceptions.rst
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/faq.rst
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/generic_handlers.rst
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/handlers.rst
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/index.rst
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/managers.rst
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/message_translators.rst
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/overview.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/providers.rst
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/routes.rst
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/settings.rst
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/tutorial.rst
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/_static/sequence_loafer.diag
--rw-r--r--   0        0        0    21698 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/_static/sequence_loafer.png
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/development/installation.rst
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/development/release.rst
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/docs/source/quickstart/installation.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/__init__.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/compat.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/dispatchers.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/exceptions.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/managers.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/message_translators.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/providers.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/routes.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/runners.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/sentry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/aws/__init__.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/aws/bases.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/aws/handlers.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/aws/message_translators.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/aws/providers.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/loafer/ext/aws/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/conftest.py
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/test_dispatchers.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/test_managers.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/test_message_translator.py
--rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/test_routes.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/test_runners.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/test_sentry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/__init__.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/conftest.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/test_bases.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/test_handlers.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/test_message_translators.py
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/test_providers.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/tests/ext/aws/test_routes.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/LICENSE
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/README.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/hatch.toml
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 olist_loafer-5.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/.editorconfig
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/CHANGES.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/CONTRIBUTORS.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/MANIFEST.in
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/Makefile
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/env.local
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/compat.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/dispatchers.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/exceptions.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/managers.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/message_translators.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/providers.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/routes.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/runners.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/sentry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/aws/__init__.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/aws/bases.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/aws/handlers.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/aws/message_translators.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/aws/providers.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/src/loafer/ext/aws/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/conftest.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/test_dispatchers.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/test_managers.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/test_message_translator.py
+-rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/test_routes.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/test_runners.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/test_sentry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/__init__.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/conftest.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/test_bases.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/test_handlers.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/test_message_translators.py
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/test_providers.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/tests/ext/aws/test_routes.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/README.md
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/hatch.toml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a1/PKG-INFO
```

### Comparing `olist_loafer-5.0.0a1/.pre-commit-config.yaml` & `olist_loafer-6.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/CHANGES.rst` & `olist_loafer-6.0.0a1/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,24 @@
-UNRELEASED
+5.0.0 (2023-12-12)
 ----------
+* chore: move to a PEP 621 compliant build system (hatch) (#44)
+* chore: add every supported version to black settings (#46)
+* chore: add toml extension to devcontainer
+* fix: hatch environment definitions were wrong
+* build: make github actions run only the tests for the right python version
+* chore: add github actions extension to dev container
+* fix: lint check-fixtures command wasn't working
+* style: use black isort profile
+* chore: remove boto3 dependency
+* chore: bump minimum aiobotocore version to 2.0.0
 * refactor: remove ConfigurationError exception
 * refactor: remove concurrency limit param
 * refactor: remove max threads param
-* chore: add support for Python 3.12
+* perf: instantiate a single aiobotocore session
+* chore: leave max python version open
 
 4.0.0 (2023-07-10)
 ------------------
 
 * chore: drop support for Python 3.7
 * chore: drop add_current_dir_to_syspath decorator
 * chore: remove import_callable function
```

### Comparing `olist_loafer-5.0.0a1/Makefile` & `olist_loafer-6.0.0a1/Makefile`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/managers.py` & `olist_loafer-6.0.0a1/src/loafer/managers.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from .dispatchers import LoaferDispatcher
 from .runners import LoaferRunner
 
 logger = logging.getLogger(__name__)
 
 
 class LoaferManager:
-    def __init__(self, routes, runner=None):
+    def __init__(self, routes, runner=None, max_concurrency=None):
         if runner is None:
             self.runner = LoaferRunner(on_stop_callback=self.on_loop__stop)
         else:
             self.runner = runner
 
         self.routes = routes
-        self.dispatcher = LoaferDispatcher(self.routes)
+        self.dispatcher = LoaferDispatcher(self.routes, max_concurrency)
 
     def run(self, forever=True, debug=False):
         loop = self.runner.loop
         self._future = asyncio.ensure_future(
             self.dispatcher.dispatch_providers(forever=forever),
             loop=loop,
         )
```

### Comparing `olist_loafer-5.0.0a1/loafer/message_translators.py` & `olist_loafer-6.0.0a1/src/loafer/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/providers.py` & `olist_loafer-6.0.0a1/src/loafer/providers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/routes.py` & `olist_loafer-6.0.0a1/src/loafer/routes.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/runners.py` & `olist_loafer-6.0.0a1/src/loafer/runners.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/utils.py` & `olist_loafer-6.0.0a1/src/loafer/utils.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/ext/aws/bases.py` & `olist_loafer-6.0.0a1/src/loafer/ext/aws/bases.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/ext/aws/handlers.py` & `olist_loafer-6.0.0a1/src/loafer/ext/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/ext/aws/message_translators.py` & `olist_loafer-6.0.0a1/src/loafer/ext/aws/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/ext/aws/providers.py` & `olist_loafer-6.0.0a1/src/loafer/ext/aws/providers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/loafer/ext/aws/routes.py` & `olist_loafer-6.0.0a1/src/loafer/ext/aws/routes.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/conftest.py` & `olist_loafer-6.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/test_dispatchers.py` & `olist_loafer-6.0.0a1/tests/test_dispatchers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,148 @@
 import asyncio
 from unittest import mock
 
 import pytest
 
+from loafer.compat import PY311
 from loafer.dispatchers import LoaferDispatcher
 from loafer.exceptions import DeleteMessage
 from loafer.routes import Route
 
+if not PY311:
+    from exceptiongroup import ExceptionGroup
 
-@pytest.fixture
-def provider():
-    return mock.AsyncMock(
-        fetch_messages=mock.AsyncMock(return_value=["message"]),
+
+def create_mock_route(messages):
+    provider = mock.AsyncMock(
+        fetch_messages=mock.AsyncMock(side_effect=[messages]),
         confirm_message=mock.AsyncMock(),
         message_not_processed=mock.AsyncMock(),
     )
 
-
-@pytest.fixture
-def route(provider):
-    message_translator = mock.Mock(translate=mock.Mock(return_value={"content": "message"}))
+    message_translator = mock.Mock(
+        translate=mock.Mock(side_effect=[{"content": message} for message in messages])
+    )
     route = mock.AsyncMock(
         provider=provider,
-        handler=mock.Mock(),
+        handler=mock.AsyncMock(),
         message_translator=message_translator,
         spec=Route,
     )
     return route
 
 
+@pytest.fixture
+def route():
+    return create_mock_route(["message"])
+
+
 @pytest.mark.asyncio
 async def test_dispatch_message(route):
     route.deliver = mock.AsyncMock(return_value="confirmation")
     dispatcher = LoaferDispatcher([route])
 
     message = "foobar"
     confirmation = await dispatcher.dispatch_message(message, route)
     assert confirmation == "confirmation"
 
-    assert route.deliver.called
-    route.deliver.assert_called_once_with(message)
+    route.deliver.assert_awaited_once_with(message)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("message", [None, ""])
 async def test_dispatch_invalid_message(route, message):
     route.deliver = mock.AsyncMock()
     dispatcher = LoaferDispatcher([route])
 
     confirmation = await dispatcher.dispatch_message(message, route)
     assert confirmation is False
-    assert route.deliver.called is False
+    route.deliver.assert_not_awaited()
 
 
 @pytest.mark.asyncio
 async def test_dispatch_message_task_delete_message(route):
     route.deliver = mock.AsyncMock(side_effect=DeleteMessage)
     dispatcher = LoaferDispatcher([route])
-
     message = "rejected-message"
+
     confirmation = await dispatcher.dispatch_message(message, route)
-    assert confirmation is True
 
+    assert confirmation is True
     assert route.deliver.called
-    route.deliver.assert_called_once_with(message)
+    route.deliver.assert_awaited_once_with(message)
 
 
 @pytest.mark.asyncio
 async def test_dispatch_message_task_error(route):
     exc = Exception()
     route.deliver = mock.AsyncMock(side_effect=exc)
     route.error_handler = mock.AsyncMock(return_value="confirmation")
     dispatcher = LoaferDispatcher([route])
-
     message = "message"
+
     confirmation = await dispatcher.dispatch_message(message, route)
-    assert confirmation == "confirmation"
 
-    assert route.deliver.called is True
-    route.deliver.assert_called_once_with(message)
-    assert route.error_handler.called is True
+    assert confirmation == "confirmation"
+    route.deliver.assert_awaited_once_with(message)
+    route.error_handler.assert_awaited_once_with((Exception, exc, mock.ANY), message)
 
 
 @pytest.mark.asyncio
 async def test_dispatch_message_task_cancel(route):
     route.deliver = mock.AsyncMock(side_effect=asyncio.CancelledError)
     dispatcher = LoaferDispatcher([route])
-
     message = "message"
+
     confirmation = await dispatcher.dispatch_message(message, route)
-    assert confirmation is False
 
-    assert route.deliver.called
-    route.deliver.assert_called_once_with(message)
+    assert confirmation is False
+    route.deliver.assert_awaited_once_with(message)
 
 
 @pytest.mark.asyncio
-async def test_message_processing(route):
+async def test_dispatch_providers(route):
     dispatcher = LoaferDispatcher([route])
     dispatcher.dispatch_message = mock.AsyncMock()
-    await dispatcher._process_message("message", route)
 
-    assert dispatcher.dispatch_message.called
-    dispatcher.dispatch_message.assert_called_once_with("message", route)
-    assert route.provider.confirm_message.called
-    assert route.provider.message_not_processed.called is False
-    route.provider.confirm_message.assert_called_once_with("message")
-
-
-@pytest.mark.asyncio
-async def test_message_processing_unsuccessfully(route):
-    dispatcher = LoaferDispatcher([route])
-    dispatcher.dispatch_message = mock.AsyncMock(return_value=False)
-    await dispatcher._process_message("message", route)
-
-    assert dispatcher.dispatch_message.called
-    dispatcher.dispatch_message.assert_called_once_with("message", route)
-
-    assert route.provider.message_not_processed.called
-    assert route.provider.confirm_message.called is False
-    route.provider.message_not_processed.assert_called_once_with("message")
-
-
-@pytest.mark.asyncio
-async def test_dispatch_provider(route):
-    route.provider.fetch_messages = mock.AsyncMock(return_value=["message"])
-    dispatcher = LoaferDispatcher([route])
-    await dispatcher._dispatch_provider(route, forever=False)
+    await dispatcher.dispatch_providers(forever=False)
 
-    assert route.provider.fetch_messages.called
-    assert route.provider.confirm_message.called
-    assert route.provider.message_not_processed.called is False
+    dispatcher.dispatch_message.assert_awaited_once_with("message", route)
 
 
 @pytest.mark.asyncio
-async def test_dispatch_without_tasks(route, event_loop):
-    route.provider.fetch_messages = mock.AsyncMock(return_value=[])
-    dispatcher = LoaferDispatcher([route])
-    await dispatcher._dispatch_provider(route, forever=False)
-
-    assert route.provider.fetch_messages.called
-    assert route.provider.confirm_message.called is False
-    assert route.provider.message_not_processed.called is False
-
+async def test_dispatch_providers_multiple_routes():
+    route1 = create_mock_route(["message1", "message2"])
+    route2 = create_mock_route(["message3"])
+    dispatcher = LoaferDispatcher([route1, route2])
+    dispatcher.dispatch_message = mock.AsyncMock()
 
-@pytest.mark.asyncio
-async def test_dispatch_providers(route, event_loop):
-    dispatcher = LoaferDispatcher([route])
-    dispatcher._dispatch_provider = mock.AsyncMock()
     await dispatcher.dispatch_providers(forever=False)
 
-    dispatcher._dispatch_provider.assert_called_once_with(route, False)
+    dispatcher.dispatch_message.assert_has_awaits(
+        [
+            mock.call("message1", route1),
+            mock.call("message2", route1),
+            mock.call("message3", route2),
+        ],
+        any_order=True,
+    )
 
 
 @pytest.mark.asyncio
-async def test_dispatch_providers_with_error(route, event_loop):
+async def test_dispatch_providers_with_error(route):
     route.provider.fetch_messages.side_effect = ValueError
     dispatcher = LoaferDispatcher([route])
-    with pytest.raises(ValueError):
+
+    with pytest.raises(ExceptionGroup) as exc_info:
         await dispatcher.dispatch_providers(forever=False)
 
+    assert exc_info.value.subgroup(ValueError) is not None
+
 
 def test_dispatcher_stop(route):
     route.stop = mock.Mock()
     dispatcher = LoaferDispatcher([route])
+
     dispatcher.stop()
+
     assert route.stop.called
```

### Comparing `olist_loafer-5.0.0a1/tests/test_managers.py` & `olist_loafer-6.0.0a1/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/test_routes.py` & `olist_loafer-6.0.0a1/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/test_runners.py` & `olist_loafer-6.0.0a1/tests/test_runners.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/test_sentry.py` & `olist_loafer-6.0.0a1/tests/ext/test_sentry.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/aws/conftest.py` & `olist_loafer-6.0.0a1/tests/ext/aws/conftest.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/aws/test_bases.py` & `olist_loafer-6.0.0a1/tests/ext/aws/test_bases.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/aws/test_handlers.py` & `olist_loafer-6.0.0a1/tests/ext/aws/test_handlers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/aws/test_message_translators.py` & `olist_loafer-6.0.0a1/tests/ext/aws/test_message_translators.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/aws/test_providers.py` & `olist_loafer-6.0.0a1/tests/ext/aws/test_providers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/tests/ext/aws/test_routes.py` & `olist_loafer-6.0.0a1/tests/ext/aws/test_routes.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/.gitignore` & `olist_loafer-6.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/LICENSE` & `olist_loafer-6.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/README.md` & `olist_loafer-6.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `olist_loafer-5.0.0a1/pyproject.toml` & `olist_loafer-6.0.0a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "olist-loafer"
-version = "5.0.0a1"
+dynamic = ["version"]
 description = "Asynchronous message dispatcher for concurrent tasks processing"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Olist", email = "developers@olist.com" }]
 keywords = ["asyncio", "message", "dispatcher", "tasks", "microservices"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Distributed Computing",
 ]
 requires-python = ">=3.8"
-dependencies = ["aiobotocore>=2.0.0,<3.0.0"]
+dependencies = ["aiobotocore>=2.0.0,<3.0.0", "taskgroup ; python_version < '3.11'"]
 
 [project.urls]
 Download = "https://github.com/olist/olist-loafer/releases"
 Repository = "https://github.com/olist/olist-loafer/"
 
 [tool.black]
 line-length = 110
@@ -39,10 +39,19 @@
 [tool.isort]
 profile = "black"
 line_length = 110
 known_localfolder = ["loafer", "tests"]
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "LOCALFOLDER"]
 default_section = "THIRDPARTY"
 
+[tool.hatch.build.targets.sdist]
+exclude = ["/.devcontainer", "/.github", "/docs"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/loafer"]
+
+[tool.hatch.version]
+source = "vcs"
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 asyncio_mode = "strict"
```

### Comparing `olist_loafer-5.0.0a1/PKG-INFO` & `olist_loafer-6.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: olist-loafer
-Version: 5.0.0a1
+Version: 6.0.0a1
 Summary: Asynchronous message dispatcher for concurrent tasks processing
 Project-URL: Download, https://github.com/olist/olist-loafer/releases
 Project-URL: Repository, https://github.com/olist/olist-loafer/
 Author-email: Olist <developers@olist.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 George Kussumoto
@@ -39,14 +39,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Requires-Dist: aiobotocore<3.0.0,>=2.0.0
+Requires-Dist: taskgroup; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 [![PyPI latest](https://img.shields.io/pypi/v/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)
 [![Python versions](https://img.shields.io/pypi/pyversions/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)
 [![License](https://img.shields.io/pypi/l/loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/olist-loafer)
 [![CircleCI](https://circleci.com/gh/olist/olist-loafer/tree/main.svg?style=svg)](https://circleci.com/gh/olist/olist-loafer/tree/main)
 [![Olist Sponsor](https://img.shields.io/badge/sponsor-olist-53b5f6.svg?style=flat-square)](http://opensource.olist.com/)
```

