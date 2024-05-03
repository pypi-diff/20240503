# Comparing `tmp/llmdocgen-0.1.0.tar.gz` & `tmp/llmdocgen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmdocgen-0.1.0.tar", last modified: Fri May  3 16:42:42 2024, max compression
+gzip compressed data, was "llmdocgen-0.1.1.tar", last modified: Fri May  3 17:05:44 2024, max compression
```

## Comparing `llmdocgen-0.1.0.tar` & `llmdocgen-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-03 16:42:42.618842 llmdocgen-0.1.0/
--rw-r--r--   0 gdoermann   (501) staff       (20)     1070 2024-05-03 14:18:10.000000 llmdocgen-0.1.0/LICENSE
--rw-r--r--   0 gdoermann   (501) staff       (20)       43 2024-05-03 15:48:05.000000 llmdocgen-0.1.0/MANIFEST.in
--rw-r--r--   0 gdoermann   (501) staff       (20)     5133 2024-05-03 16:42:42.618774 llmdocgen-0.1.0/PKG-INFO
--rw-r--r--   0 gdoermann   (501) staff       (20)     3931 2024-05-03 16:37:43.000000 llmdocgen-0.1.0/README.md
--rw-r--r--   0 gdoermann   (501) staff       (20)      440 2024-05-03 15:48:05.000000 llmdocgen-0.1.0/pyproject.toml
--rw-r--r--   0 gdoermann   (501) staff       (20)     1289 2024-05-03 16:42:42.619129 llmdocgen-0.1.0/setup.cfg
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-03 16:42:42.615750 llmdocgen-0.1.0/src/
--rw-r--r--   0 gdoermann   (501) staff       (20)     6148 2024-05-03 16:02:34.000000 llmdocgen-0.1.0/src/.DS_Store
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-03 16:42:42.617014 llmdocgen-0.1.0/src/llmdocgen/
--rw-r--r--   0 gdoermann   (501) staff       (20)      314 2024-05-03 15:36:35.000000 llmdocgen-0.1.0/src/llmdocgen/__init__.py
--rw-r--r--   0 gdoermann   (501) staff       (20)     2328 2024-05-03 16:27:45.000000 llmdocgen-0.1.0/src/llmdocgen/enrich.py
--rw-r--r--   0 gdoermann   (501) staff       (20)     1881 2024-05-03 16:33:47.000000 llmdocgen-0.1.0/src/llmdocgen/executor.py
--rw-r--r--   0 gdoermann   (501) staff       (20)     4279 2024-05-03 16:36:15.000000 llmdocgen-0.1.0/src/llmdocgen/settings.py
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-03 16:42:42.618297 llmdocgen-0.1.0/src/llmdocgen.egg-info/
--rw-r--r--   0 gdoermann   (501) staff       (20)     5133 2024-05-03 16:42:42.000000 llmdocgen-0.1.0/src/llmdocgen.egg-info/PKG-INFO
--rw-r--r--   0 gdoermann   (501) staff       (20)      390 2024-05-03 16:42:42.000000 llmdocgen-0.1.0/src/llmdocgen.egg-info/SOURCES.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-03 16:42:42.000000 llmdocgen-0.1.0/src/llmdocgen.egg-info/dependency_links.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-03 15:59:01.000000 llmdocgen-0.1.0/src/llmdocgen.egg-info/not-zip-safe
--rw-r--r--   0 gdoermann   (501) staff       (20)       92 2024-05-03 16:42:42.000000 llmdocgen-0.1.0/src/llmdocgen.egg-info/requires.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)       10 2024-05-03 16:42:42.000000 llmdocgen-0.1.0/src/llmdocgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:05:44.168539 llmdocgen-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-03 17:05:44.168539 llmdocgen-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-03 17:05:44.168539 llmdocgen-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:05:44.164539 llmdocgen-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:05:44.164539 llmdocgen-0.1.1/src/llmdocgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/src/llmdocgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/src/llmdocgen/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/src/llmdocgen/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-03 17:05:39.000000 llmdocgen-0.1.1/src/llmdocgen/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:05:44.168539 llmdocgen-0.1.1/src/llmdocgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-03 17:05:44.000000 llmdocgen-0.1.1/src/llmdocgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-03 17:05:44.000000 llmdocgen-0.1.1/src/llmdocgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:05:44.000000 llmdocgen-0.1.1/src/llmdocgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:05:43.000000 llmdocgen-0.1.1/src/llmdocgen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 17:05:44.000000 llmdocgen-0.1.1/src/llmdocgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 17:05:44.000000 llmdocgen-0.1.1/src/llmdocgen.egg-info/top_level.txt
```

### Comparing `llmdocgen-0.1.0/LICENSE` & `llmdocgen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmdocgen-0.1.0/PKG-INFO` & `llmdocgen-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: llmdocgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automate documentation generation using the LLM of your choice!
 Home-page: https://github.com/gdoermann/llmdocgen
 Author: Greg Doermann
 Author-email: gdoermann+llmdocgen@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff
 Requires-Dist: attrdict3
@@ -33,14 +32,18 @@
 
 # LLM Code Documentation Generator
 
 `llmdocgen` is a library for automatically documenting code using large language models (LLMs). It takes code files as
 input, sends them to an LLM to generate documentation comments, and returns the code with the generated documentation
 added.
 
+LLMDocGen will not just document python files but also other languages like JavaScript, Java, C++, etc. 
+It can be used as a library or run as a command line tool.
+
+
 ## Features
 
 - Automatically documents code using LLMs
 - Supports a wide variety of programming languages out of the box
 - Easily configurable to add support for additional file types
 - Can be used as a library or run as a command line tool
 - Integrates with [LiteLLM](https://docs.litellm.ai) to work with OpenAI, Anthropic, and other LLM providers
@@ -149,14 +152,31 @@
 ### Authenticating with LLMs
 
 As mentioned above, `llmdocgen` uses LiteLLM to integrate with LLM providers. All authentication happens through LiteLLM
 by setting the appropriate environment variables.
 See settings.LITELLM for the full list of supported settings. These map directly to arguments to LiteLLM's
 litellm.completion() function.
 
+
+### File Types
+
+`llmdocgen` supports a wide variety of file types out of the box. The supported file types are defined in the
+`settings.DEFAULT_EXTENSIONS` dictionary. Each key is a file extension, and each value is a list of languages that
+llmdocgen will use to generate documentation for that file type.
+
+If you would like to include additional file types, you can set the `LLMDOCGEN_EXTRA_EXTENSIONS` environment variable to a
+comma-separated list of file extensions. 
+
+If you want to override the default list entirely, you can set the `LLMDOCGEN_EXTENSIONS` environment variable to a
+comma-separated list of file extensions.  This would allow you to only document specific file types.
+
+All of these can be set in your environment file (see the Setup section above) so you do not have to set them every time
+you run `llmdocgen`.
+
+
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 `llmdocgen` is released under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `llmdocgen-0.1.0/README.md` & `llmdocgen-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # LLM Code Documentation Generator
 
 `llmdocgen` is a library for automatically documenting code using large language models (LLMs). It takes code files as
 input, sends them to an LLM to generate documentation comments, and returns the code with the generated documentation
 added.
 
+LLMDocGen will not just document python files but also other languages like JavaScript, Java, C++, etc. 
+It can be used as a library or run as a command line tool.
+
+
 ## Features
 
 - Automatically documents code using LLMs
 - Supports a wide variety of programming languages out of the box
 - Easily configurable to add support for additional file types
 - Can be used as a library or run as a command line tool
 - Integrates with [LiteLLM](https://docs.litellm.ai) to work with OpenAI, Anthropic, and other LLM providers
@@ -116,14 +120,31 @@
 ### Authenticating with LLMs
 
 As mentioned above, `llmdocgen` uses LiteLLM to integrate with LLM providers. All authentication happens through LiteLLM
 by setting the appropriate environment variables.
 See settings.LITELLM for the full list of supported settings. These map directly to arguments to LiteLLM's
 litellm.completion() function.
 
+
+### File Types
+
+`llmdocgen` supports a wide variety of file types out of the box. The supported file types are defined in the
+`settings.DEFAULT_EXTENSIONS` dictionary. Each key is a file extension, and each value is a list of languages that
+llmdocgen will use to generate documentation for that file type.
+
+If you would like to include additional file types, you can set the `LLMDOCGEN_EXTRA_EXTENSIONS` environment variable to a
+comma-separated list of file extensions. 
+
+If you want to override the default list entirely, you can set the `LLMDOCGEN_EXTENSIONS` environment variable to a
+comma-separated list of file extensions.  This would allow you to only document specific file types.
+
+All of these can be set in your environment file (see the Setup section above) so you do not have to set them every time
+you run `llmdocgen`.
+
+
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 `llmdocgen` is released under the MIT License. See [LICENSE](LICENSE) for more information.
```

### Comparing `llmdocgen-0.1.0/setup.cfg` & `llmdocgen-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
-	Programming Language :: Python :: 3.13
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 
 [options]
 python_requires = >=3.9
 include_package_data = true
 zip_safe = false
```

### Comparing `llmdocgen-0.1.0/src/llmdocgen/enrich.py` & `llmdocgen-0.1.1/src/llmdocgen/enrich.py`

 * *Files identical despite different names*

### Comparing `llmdocgen-0.1.0/src/llmdocgen/executor.py` & `llmdocgen-0.1.1/src/llmdocgen/executor.py`

 * *Files identical despite different names*

### Comparing `llmdocgen-0.1.0/src/llmdocgen/settings.py` & `llmdocgen-0.1.1/src/llmdocgen/settings.py`

 * *Files identical despite different names*

### Comparing `llmdocgen-0.1.0/src/llmdocgen.egg-info/PKG-INFO` & `llmdocgen-0.1.1/src/llmdocgen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: llmdocgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automate documentation generation using the LLM of your choice!
 Home-page: https://github.com/gdoermann/llmdocgen
 Author: Greg Doermann
 Author-email: gdoermann+llmdocgen@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff
 Requires-Dist: attrdict3
@@ -33,14 +32,18 @@
 
 # LLM Code Documentation Generator
 
 `llmdocgen` is a library for automatically documenting code using large language models (LLMs). It takes code files as
 input, sends them to an LLM to generate documentation comments, and returns the code with the generated documentation
 added.
 
+LLMDocGen will not just document python files but also other languages like JavaScript, Java, C++, etc. 
+It can be used as a library or run as a command line tool.
+
+
 ## Features
 
 - Automatically documents code using LLMs
 - Supports a wide variety of programming languages out of the box
 - Easily configurable to add support for additional file types
 - Can be used as a library or run as a command line tool
 - Integrates with [LiteLLM](https://docs.litellm.ai) to work with OpenAI, Anthropic, and other LLM providers
@@ -149,14 +152,31 @@
 ### Authenticating with LLMs
 
 As mentioned above, `llmdocgen` uses LiteLLM to integrate with LLM providers. All authentication happens through LiteLLM
 by setting the appropriate environment variables.
 See settings.LITELLM for the full list of supported settings. These map directly to arguments to LiteLLM's
 litellm.completion() function.
 
+
+### File Types
+
+`llmdocgen` supports a wide variety of file types out of the box. The supported file types are defined in the
+`settings.DEFAULT_EXTENSIONS` dictionary. Each key is a file extension, and each value is a list of languages that
+llmdocgen will use to generate documentation for that file type.
+
+If you would like to include additional file types, you can set the `LLMDOCGEN_EXTRA_EXTENSIONS` environment variable to a
+comma-separated list of file extensions. 
+
+If you want to override the default list entirely, you can set the `LLMDOCGEN_EXTENSIONS` environment variable to a
+comma-separated list of file extensions.  This would allow you to only document specific file types.
+
+All of these can be set in your environment file (see the Setup section above) so you do not have to set them every time
+you run `llmdocgen`.
+
+
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 `llmdocgen` is released under the MIT License. See [LICENSE](LICENSE) for more information.
```

