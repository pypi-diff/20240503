# Comparing `tmp/seviper-0.0.3.tar.gz` & `tmp/seviper-0.0.4.tar.gz`

## Comparing `seviper-0.0.3.tar` & `seviper-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 seviper-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 seviper-0.0.3/README.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 seviper-0.0.3/domain-specific-terms.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 seviper-0.0.3/requirements.txt
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 seviper-0.0.3/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 seviper-0.0.3/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-extra-aiostream.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 seviper-0.0.3/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 seviper-0.0.3/src/_error_handler_version.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/_extra.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/callback.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/context_manager.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/core.py
--rw-r--r--   0        0        0    15539 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/decorator.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/pipe.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/py.typed
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/result.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/stream.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 seviper-0.0.3/src/error_handler/types.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 seviper-0.0.3/.gitignore
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 seviper-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 seviper-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 seviper-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 seviper-0.0.4/README.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 seviper-0.0.4/domain-specific-terms.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 seviper-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 seviper-0.0.4/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 seviper-0.0.4/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-extra-aiostream.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 seviper-0.0.4/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 seviper-0.0.4/src/_error_handler_version.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/_extra.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/callback.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/context_manager.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/core.py
+-rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/decorator.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/pipe.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/py.typed
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/result.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/stream.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 seviper-0.0.4/src/error_handler/types.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 seviper-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 seviper-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 seviper-0.0.4/PKG-INFO
```

### Comparing `seviper-0.0.3/.pre-commit-config.yaml` & `seviper-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/README.md` & `seviper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/tox.ini` & `seviper-0.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/dependabot.yml` & `seviper-0.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/codeql-analysis.yml` & `seviper-0.0.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/coverage.yml` & `seviper-0.0.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/dependabot_automerge.yml` & `seviper-0.0.4/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/dev_test.yml` & `seviper-0.0.4/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/formatting.yml` & `seviper-0.0.4/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/packaging_test.yml` & `seviper-0.0.4/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/python-publish.yml` & `seviper-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/pythonlint.yml` & `seviper-0.0.4/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.github/workflows/unittests.yml` & `seviper-0.0.4/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/dev_requirements/requirements-packaging.txt` & `seviper-0.0.4/dev_requirements/requirements-packaging.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,78 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.12
+# by the following command:
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
+idna==3.6
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
-keyring==23.13.1
+keyring==24.3.1
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.1.0
+more-itertools==10.2.0
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
-readme-renderer==37.3
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
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
 twine==5.0.0
     # via -r dev_requirements/requirements-packaging.in
-urllib3==2.0.7
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

### Comparing `seviper-0.0.3/src/error_handler/__init__.py` & `seviper-0.0.4/src/error_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/src/error_handler/_extra.py` & `seviper-0.0.4/src/error_handler/_extra.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/src/error_handler/callback.py` & `seviper-0.0.4/src/error_handler/callback.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/src/error_handler/context_manager.py` & `seviper-0.0.4/src/error_handler/context_manager.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/src/error_handler/core.py` & `seviper-0.0.4/src/error_handler/core.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/src/error_handler/decorator.py` & `seviper-0.0.4/src/error_handler/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,22 +288,25 @@
         return_func.__catcher__ = catcher_retrier  # type: ignore[union-attr]
         return_func.__original_callable__ = callable_to_secure  # type: ignore[union-attr]
         return return_func
 
     return decorator_inner  # type: ignore[return-value]
 
 
+_C = TypeVar("_C", bound=Callable)
+
+
 def decorator(
     *,
     on_success: Callable[Concatenate[_T, _P], Any] | None = None,
     on_error: Callable[Concatenate[BaseException, _P], Any] | None = None,
     on_finalize: Callable[_P, Any] | None = None,
     suppress_recalling_on_error: bool = True,
     on_error_return_always: _T | UnsetType = UNSET,
-) -> Decorator[_P, _T]:
+) -> Callable[[_C], _C]:
     """
     Returns a callback that converts the result of a secured function back to the original return type.
     To make this work, you need to define which value should be returned in error cases.
     Otherwise, if the secured function returns an error result, the error will be raised.
     """
 
     def decorator_inner(
```

### Comparing `seviper-0.0.3/src/error_handler/result.py` & `seviper-0.0.4/src/error_handler/result.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/src/error_handler/types.py` & `seviper-0.0.4/src/error_handler/types.py`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/.gitignore` & `seviper-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/pyproject.toml` & `seviper-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seviper-0.0.3/PKG-INFO` & `seviper-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: seviper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple and easy to use library to catch and handle exceptions.
 Project-URL: Changelog, https://github.com/Hochfrequenz/seviper/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/seviper
 Author-email: Leon Haffmans <leon.haffmans@hochfrequenz.de>
 License: MIT
 Keywords: aiostream,error-handling
 Classifier: Development Status :: 4 - Beta
```

