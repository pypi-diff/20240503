# Comparing `tmp/nextline_alert-0.1.3.tar.gz` & `tmp/nextline_alert-0.1.4.tar.gz`

## Comparing `nextline_alert-0.1.3.tar` & `nextline_alert-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/setup.cfg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.github/release.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/default.toml
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/emitter.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/py.typed
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/schema/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/src/nextline_alert/schema/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/tests/test_emitter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/tests/test_version.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/README.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 nextline_alert-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/setup.cfg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/release.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/default.toml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/emitter.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/py.typed
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/schema/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/src/nextline_alert/schema/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/tests/test_emitter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/tests/test_version.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/README.md
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 nextline_alert-0.1.4/PKG-INFO
```

### Comparing `nextline_alert-0.1.3/.github/workflows/pypi.yml` & `nextline_alert-0.1.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/.github/workflows/release.yml` & `nextline_alert-0.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/.github/workflows/type-check.yml` & `nextline_alert-0.1.4/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/.github/workflows/unit-test.yml` & `nextline_alert-0.1.4/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/src/nextline_alert/emitter.py` & `nextline_alert-0.1.4/src/nextline_alert/emitter.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,37 @@
         self._platform = platform
         self._logger = getLogger(__name__)
         self._logger.info(f'Campana endpoint: {url}')
         self._logger.debug(f'Platform: {platform!r}')
 
     @hookimpl
     async def on_end_run(self, context: Context) -> None:
-        run_arg = context.run_arg
         nextline = context.nextline
-        if fmt_exc := nextline.format_exception():
-            run_no_str = 'unknown' if run_arg is None else f'{run_arg.run_no}'
-            alertname = f'Run {run_no_str} failed'
-            self._logger.info(f"Emitting alert: '{alertname}'")
-            labels = {'alertname': alertname, 'platform': self._platform}
-            try:
-                await emit(url=self._url, labels=labels, description=fmt_exc)
-            except BaseException:
-                self._logger.exception(f"Failed to emit alert: '{alertname}'")
-                self._logger.debug(f'Alert description: {fmt_exc!r}')
+
+        if not (fmt_exc := nextline.format_exception()):
+            return
+
+        # TODO: Quick implementation to ignore KeyboardInterrupt
+        #       Instead of parsing fmt_exc, store the exception type as string
+        #       in RunResult in the spawned process.
+        #       https://github.com/simonsobs/nextline/blob/v0.7.4/nextline/spawned/types.py#L35-L58
+        if fmt_exc.rstrip().endswith('KeyboardInterrupt'):
+            self._logger.info('Ignoring KeyboardInterrupt')
+            return
+
+        run_arg = context.run_arg
+        run_no_str = 'unknown' if run_arg is None else f'{run_arg.run_no}'
+        alertname = f'Run {run_no_str} failed'
+        self._logger.info(f"Emitting alert: '{alertname}'")
+        labels = {'alertname': alertname, 'platform': self._platform}
+        try:
+            await emit(url=self._url, labels=labels, description=fmt_exc)
+        except BaseException:
+            self._logger.exception(f"Failed to emit alert: '{alertname}'")
+            self._logger.debug(f'Alert description: {fmt_exc!r}')
 
 
 async def emit(url: str, labels: dict[str, str], description: str) -> None:
     data = {
         'status': 'firing',
         'alerts': [
             {
```

### Comparing `nextline_alert-0.1.3/src/nextline_alert/plugin.py` & `nextline_alert-0.1.4/src/nextline_alert/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/tests/test_emitter.py` & `nextline_alert-0.1.4/tests/test_emitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import asyncio
 import json
 import time
 
+import pytest
 import respx
 from nextline import Nextline
 
 from nextline_alert.emitter import Emitter
 
 
 def func_success():
     time.sleep(0.001)
 
 
-def func_rase():
+def func_raise_ignore():
+    time.sleep(0.001)
+    raise KeyboardInterrupt
+
+
+def func_raise():
     time.sleep(0.001)
     raise ValueError('test')
 
 
 @respx.mock
-async def test_emit_no_alert() -> None:
-    nextline = Nextline(func_success)
+@pytest.mark.parametrize('func', [func_success, func_raise_ignore])
+async def test_emit_no_alert(func) -> None:
+    nextline = Nextline(func)
 
     url = 'http://localhost:5000/alerts'
     platform = 'pytest'
     emitter = Emitter(url=url, platform=platform)
     assert nextline.register(emitter)
 
     # Mock the HTTP POST request
@@ -36,15 +43,15 @@
 
     # Assert the HTTP POST request
     assert not route.called
 
 
 @respx.mock
 async def test_emit_alert() -> None:
-    nextline = Nextline(func_rase)
+    nextline = Nextline(func_raise)
 
     url = 'http://localhost:5000/alerts'
     platform = 'pytest'
     emitter = Emitter(url=url, platform=platform)
     assert nextline.register(emitter)
 
     # Mock the HTTP POST request
```

### Comparing `nextline_alert-0.1.3/.gitignore` & `nextline_alert-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/LICENSE.txt` & `nextline_alert-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/README.md` & `nextline_alert-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/pyproject.toml` & `nextline_alert-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextline_alert-0.1.3/PKG-INFO` & `nextline_alert-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline-alert
-Version: 0.1.3
+Version: 0.1.4
 Summary: A plugin of nextline-graphql. Emit alerts to Campana
 Project-URL: Documentation, https://github.com/simonsobs/nextline-alert#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-alert/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-alert
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
```

