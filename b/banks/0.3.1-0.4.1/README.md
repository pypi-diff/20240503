# Comparing `tmp/banks-0.3.1.tar.gz` & `tmp/banks-0.4.1.tar.gz`

## Comparing `banks-0.3.1.tar` & `banks-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 banks-0.3.1/mkdocs.yml
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 banks-0.3.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.3.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 banks-0.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 banks-0.3.1/docs/async.md
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 banks-0.3.1/docs/index.md
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 banks-0.3.1/docs/prompt.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 banks-0.3.1/docs/python.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/__about__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/__init__.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/env.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/errors.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/loader.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/prompt.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/extensions/__init__.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/extensions/generate.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/extensions/inference_endpoint.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/filters/__init__.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/filters/lemmatize.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/banks_macros.jinja
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/blog.jinja
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/generate_tweet.jinja
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/run_prompt.jinja
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/run_prompt_process.jinja
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/summarize.jinja
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.3.1/src/banks/templates/summarize_lemma.jinja
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 banks-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_default_templates.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_env.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_loader.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_run_prompt.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_default_templates/blog.jinja.out
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_default_templates/generate_tweet.jinja.out
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_default_templates/summarize.jinja.out
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.3.1/tests/test_default_templates/summarize_lemma.jinja.out
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.3.1/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 banks-0.3.1/README.md
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 banks-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 banks-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 banks-0.4.1/MANIFEST.in
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 banks-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 banks-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 banks-0.4.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 banks-0.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 banks-0.4.1/docs/index.md
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 banks-0.4.1/docs/prompt.md
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 banks-0.4.1/docs/python.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/__about__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/config.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/env.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/errors.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/loader.py
+-rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/prompt.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/utils.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/extensions/__init__.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/extensions/generate.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/extensions/inference_endpoint.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/filters/__init__.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/filters/lemmatize.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/banks_macros.jinja
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/blog.jinja
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/generate_tweet.jinja
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/run_prompt.jinja
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/run_prompt_process.jinja
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/summarize.jinja
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 banks-0.4.1/src/banks/templates/summarize_lemma.jinja
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 banks-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_default_templates.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_env.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_loader.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_prompt.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_run_prompt.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_default_templates/blog.jinja.out
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_default_templates/generate_tweet.jinja.out
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_default_templates/summarize.jinja.out
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 banks-0.4.1/tests/test_default_templates/summarize_lemma.jinja.out
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 banks-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 banks-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 banks-0.4.1/README.md
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 banks-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 banks-0.4.1/PKG-INFO
```

### Comparing `banks-0.3.1/mkdocs.yml` & `banks-0.4.1/mkdocs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,26 @@
     primary: amber
     scheme: slate
 
 nav:
   - Home: 'index.md'
   - Python API: 'python.md'
   - Prompt API: 'prompt.md'
-  - asyncio support: 'async.md'
 
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
           paths: [src]
           options:
+              docstring_style: google
               show_root_heading: true
-              show_root_full_path: false
+              show_root_full_path: true
+              show_symbol_type_heading: true
               show_source: false
               show_signature_annotations: true
               show_bases: false
 
 markdown_extensions:
   - pymdownx.highlight:
       anchor_linenums: true
```

### Comparing `banks-0.3.1/.github/workflows/test.yml` & `banks-0.4.1/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
+        python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
```

### Comparing `banks-0.3.1/docs/index.md` & `banks-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/src/banks/env.py` & `banks-0.4.1/src/banks/env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
-import os
-
 from jinja2 import Environment, select_autoescape
 
-from banks.extensions import GenerateExtension, HFInferenceEndpointsExtension
-from banks.filters import lemmatize
-from banks.loader import MultiLoader
+from .config import async_enabled
+from .filters import lemmatize
+from .loader import MultiLoader
 
 
-def strtobool(val: str) -> bool:
-    """Convert a string representation of truth to True or False.
+def _add_extensions(env):
+    """
+    We lazily add extensions so that we can use the env in the extensions themselves if needed.
 
-    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
-    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
-    'val' is anything else.
+    For example, we use banks to manage the system prompt in `GenerateExtension`
     """
-    val = val.lower()
-    if val in ("y", "yes", "t", "true", "on", "1"):
-        return True
-    elif val in ("n", "no", "f", "false", "off", "0"):
-        return False
-    else:
-        msg = f"invalid truth value {val}"
-        raise ValueError(msg)
+    from .extensions import GenerateExtension, HFInferenceEndpointsExtension
 
+    env.add_extension(GenerateExtension)
+    env.add_extension(HFInferenceEndpointsExtension)
 
-async_enabled = strtobool(os.environ.get("BANKS_ASYNC_ENABLED", "false"))
 
 # Init the Jinja env
 env = Environment(
     loader=MultiLoader(),
-    extensions=[GenerateExtension, HFInferenceEndpointsExtension],
     autoescape=select_autoescape(
         enabled_extensions=("html", "xml"),
         default_for_string=False,
     ),
     trim_blocks=True,
     lstrip_blocks=True,
     enable_async=bool(async_enabled),
 )
 
-# Setup custom filters
+# Setup custom filters and default extensions
 env.filters["lemmatize"] = lemmatize
+_add_extensions(env)
 
 
 def with_env(cls):
     """
     A decorator that adds an `env` attribute to the decorated class
     """
     cls.env = env
```

### Comparing `banks-0.3.1/src/banks/loader.py` & `banks-0.4.1/src/banks/loader.py`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/src/banks/extensions/generate.py` & `banks-0.4.1/src/banks/extensions/generate.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 # SPDX-License-Identifier: MIT
 from typing import cast
 
 from jinja2 import nodes
 from jinja2.ext import Extension
 from litellm import ModelResponse, acompletion, completion
 
+from banks.errors import CanaryWordError
+from banks.prompt import Prompt
+
 DEFAULT_MODEL = "gpt-3.5-turbo"
+SYSTEM_PROMPT = Prompt("{{canary_word}} You are a helpful assistant.")
 
 
-class GenerateExtension(Extension):
+def generate(model_name: str):  # noqa
     """
     `generate` can be used to call the LiteLLM API passing the tag text as a prompt and get back some content.
 
     Example:
         ```
         {% generate "write a tweet with positive sentiment" "gpt-3.5-turbo" %}
         Feeling grateful for all the opportunities that come my way! #positivity #productivity
         ```
     """
 
+
+class GenerateExtension(Extension):
     # a set of names that trigger the extension.
     tags = {"generate"}  # noqa
 
     def parse(self, parser):
         # We get the line number of the first token so that we can give
         # that line number to the nodes we create by hand.
         lineno = next(parser.stream).lineno
@@ -48,25 +54,32 @@
     def _generate(self, text, model_name=DEFAULT_MODEL):
         """
         Helper callback.
 
         To tweak the prompt used to generate content, change the variable `messages` .
         """
         messages = [
-            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "system", "content": SYSTEM_PROMPT.text()},
             {"role": "user", "content": text},
         ]
         response: ModelResponse = cast(ModelResponse, completion(model=model_name, messages=messages))
-        return response["choices"][0]["message"]["content"]
+        return self._get_content(response)
 
     async def _agenerate(self, text, model_name=DEFAULT_MODEL):
         """
         Helper callback.
 
         To tweak the prompt used to generate content, change the variable `messages` .
         """
         messages = [
-            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "system", "content": SYSTEM_PROMPT.text()},
             {"role": "user", "content": text},
         ]
         response: ModelResponse = cast(ModelResponse, await acompletion(model=model_name, messages=messages))
-        return response["choices"][0]["message"]["content"]
+        return self._get_content(response)
+
+    def _get_content(self, response: ModelResponse) -> str:
+        content = response["choices"][0]["message"]["content"]
+        if SYSTEM_PROMPT.canary_leaked(content):
+            msg = "The system prompt has leaked into the response, possible prompt injection!"
+            raise CanaryWordError(msg)
+        return content
```

### Comparing `banks-0.3.1/src/banks/extensions/inference_endpoint.py` & `banks-0.4.1/src/banks/extensions/inference_endpoint.py`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/src/banks/filters/lemmatize.py` & `banks-0.4.1/src/banks/filters/lemmatize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 from banks.errors import MissingDependencyError
 
 try:
-    from simplemma import text_lemmatizer
+    from simplemma.simplemma import text_lemmatizer
 
     simplemma_avail = True
 except ImportError:
     simplemma_avail = False
 
 
 def lemmatize(text: str) -> str:
     """
     Compute and return the lemmatization of the input. Language is hardcoded
     to English.
 
     Example:
-        ```
-        {{ 'The dog is running' | lemmatize }}
-        'the dog be run'
-        ```
+    ```
+    {{ 'The dog is running' | lemmatize }}
+    'the dog be run'
+    ```
 
     Note:
         Simplemma must be manually installed to use this filter
     """
     if not simplemma_avail:
         err_msg = "simplemma is not available, please install it with 'pip install simplemma'"
         raise MissingDependencyError(err_msg)
```

### Comparing `banks-0.3.1/tests/test_default_templates.py` & `banks-0.4.1/tests/test_default_templates.py`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/tests/test_loader.py` & `banks-0.4.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/tests/test_run_prompt.py` & `banks-0.4.1/tests/test_run_prompt.py`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/.gitignore` & `banks-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/LICENSE.txt` & `banks-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/README.md` & `banks-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `banks-0.3.1/pyproject.toml` & `banks-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "banks"
 dynamic = ["version"]
 description = 'A prompt programming language'
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Massimiliano Pippi", email = "mpippi@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -37,30 +36,33 @@
 [tool.hatch.version]
 path = "src/banks/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "mkdocs-material",
+  "mkdocstrings[python]",
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
+docs = "mkdocs build"
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+python = ["3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.lint]
 detached = false  # Normally the linting env can be detached, but mypy doesn't install all the stubs we need
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `banks-0.3.1/PKG-INFO` & `banks-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.3
 Name: banks
-Version: 0.3.1
+Version: 0.4.1
 Summary: A prompt programming language
 Project-URL: Documentation, https://github.com/unknown/banks#readme
 Project-URL: Issues, https://github.com/unknown/banks/issues
 Project-URL: Source, https://github.com/unknown/banks
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: jinja2
 Requires-Dist: litellm
 Description-Content-Type: text/markdown
 
 # banks
 
 [![PyPI - Version](https://img.shields.io/pypi/v/banks.svg)](https://pypi.org/project/banks)
```

