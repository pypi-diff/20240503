# Comparing `tmp/repo2docs-0.1.5.tar.gz` & `tmp/repo2docs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2docs-0.1.5.tar", max compression
+gzip compressed data, was "repo2docs-0.1.6.tar", max compression
```

## Comparing `repo2docs-0.1.5.tar` & `repo2docs-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.5/LICENSE
--rw-r--r--   0        0        0     2687 2024-05-03 02:31:53.127912 repo2docs-0.1.5/README.md
--rw-r--r--   0        0        0      507 2024-05-03 02:52:24.229912 repo2docs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.5/repo2docs/__init__.py
--rw-r--r--   0        0        0     2011 2024-05-03 02:12:41.755256 repo2docs-0.1.5/repo2docs/llm.py
--rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.5/repo2docs/prompts.py
--rw-r--r--   0        0        0     3576 2024-05-03 02:50:47.360967 repo2docs-0.1.5/repo2docs/repo2docs.py
--rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.5/repo2docs/repo_to_text.py
--rw-r--r--   0        0        0     2353 2024-05-03 02:40:00.488875 repo2docs-0.1.5/repo2docs/text_to_docs.py
--rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 repo2docs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2628 2024-05-03 03:02:40.392117 repo2docs-0.1.6/README.md
+-rw-r--r--   0        0        0      506 2024-05-03 03:02:17.949745 repo2docs-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.6/repo2docs/__init__.py
+-rw-r--r--   0        0        0     2044 2024-05-03 03:01:00.838466 repo2docs-0.1.6/repo2docs/llm.py
+-rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.6/repo2docs/prompts.py
+-rw-r--r--   0        0        0     3283 2024-05-03 03:02:01.367859 repo2docs-0.1.6/repo2docs/repo2docs.py
+-rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.6/repo2docs/repo_to_text.py
+-rw-r--r--   0        0        0     2262 2024-05-03 03:01:35.532506 repo2docs-0.1.6/repo2docs/text_to_docs.py
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 repo2docs-0.1.6/PKG-INFO
```

### Comparing `repo2docs-0.1.5/LICENSE` & `repo2docs-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.5/README.md` & `repo2docs-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
    ```
    repo2docs --dir_path . --output_file documentation.md --type documentation --llm openai
    ```
 
    To generate mobile documentation, use `--type mobile`.
    To generate diagrams instead of documentation, use `--type diagram`.
    To generate database erd diagrams, use `--type database`.
-   To generate custom documentation, use `--type custom` and provide a custom prompt with `--prompt <prompt>`.
+   To use a custom prompt, use `--prompt <prompt>`.
 
 ## Supported File Types
 
 Repo2Docs currently supports processing files with the following extensions: `.py`, `.js`, `.jsx`, `.ts`, `.tsx`, `.c`, `.cpp`, `.h`, `.hpp`. It filters out files from directories like `docs`, `examples`, `tests`, and others that are unlikely to contain useful information for documentation.
 
 ## Contributing
```

### Comparing `repo2docs-0.1.5/repo2docs/llm.py` & `repo2docs-0.1.6/repo2docs/llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
 import os
 import openai
 import anthropic
 import sys
+import getpass
 
 class LLMClient(ABC):
     """
     Abstract base class for LLM clients.
     """
 
     @abstractmethod
@@ -17,18 +18,17 @@
     def get_api_key(env_var, client_name):
         """
         Retrieve API key from environment or prompt user if not found, specifying the client.
         """
         api_key = os.getenv(env_var)
         if not api_key:
             print(f"API key for {client_name} ({env_var}) not found. Please enter your API key:")
-            api_key = input()
+            api_key = getpass.getpass(prompt='')
         return api_key
 
-
 class OpenAIClient(LLMClient):
     def __init__(self, api_key=None):
         if not api_key:
             api_key = self.get_api_key('OPENAI_API_KEY', 'OpenAI')
         self.client = openai.OpenAI(api_key=api_key)
 
     def generate_response(
```

### Comparing `repo2docs-0.1.5/repo2docs/prompts.py` & `repo2docs-0.1.6/repo2docs/prompts.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.5/repo2docs/repo2docs.py` & `repo2docs-0.1.6/repo2docs/repo2docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,17 @@
     repo_processor = RepoProcessor(
         repo_zip_path, None, ignore_dirs
     )
     repo_text = repo_processor.process_repo()
 
     logging.info(f"Repository text has been successfully processed.")
     
-    print(f"LLM choice received: {llm}")
-    
     # Convert the repository text to documentation
     text_to_docs = TextToDocs(llm)
-    if doc_type == "custom":
-        print(f"Custom prompt provided: {prompt}")
+    if prompt:
         docs_content = text_to_docs.generate_custom(repo_text, prompt)
     elif doc_type == "diagram":
         docs_content = text_to_docs.generate_diagram(repo_text)
     elif doc_type == "database":
         docs_content = text_to_docs.generate_database(repo_text)
     elif doc_type == "mobile":
         docs_content = text_to_docs.generate_mobile(repo_text)
@@ -56,18 +53,15 @@
     with open(output_file, "w", encoding="utf-8") as outfile:
         outfile.write(docs_content)
     logging.info(f"Documentation has been successfully saved to {output_file}.")
 
 
 
 
-if __name__ == "__main__":
-    print("Running repo2docs")
-    
-    logging.basicConfig(level=logging.INFO)
+def run():
 
     parser = argparse.ArgumentParser(
         description="Convert a directory into documentation."
     )
     parser.add_argument(
         "--dir_path", 
         help="The directory path to process, defaults to current directory if not provided.",
@@ -82,26 +76,25 @@
         "--prompt",
         help="The prompt to use for generating the documentation.",
         default=None
     )
     parser.add_argument(
         "--type",
         dest="doc_type",  # Ensure this matches the parameter name in main
-        choices=["documentation", "diagram", "database", "mobile", "custom"],
+        choices=["documentation", "diagram", "database", "mobile"],
         default="documentation",
         help="Specify the type of documentation to generate.",
     )
     parser.add_argument(
         "--llm",
         choices=["openai", "anthropic"],
         default="anthropic",
         help="Specify the language model API to use for generating documentation.",
     )
     parser.add_argument(
         "--ignore_dirs", nargs="*", default=[], help="List of directories to ignore."
     )
 
     args = parser.parse_args()
-    print(args)  # Debug: Print all parsed arguments to verify their values
 
     main(args.dir_path, args.output_file, args.prompt, args.doc_type, args.llm, args.ignore_dirs)
```

### Comparing `repo2docs-0.1.5/repo2docs/repo_to_text.py` & `repo2docs-0.1.6/repo2docs/repo_to_text.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.5/repo2docs/text_to_docs.py` & `repo2docs-0.1.6/repo2docs/text_to_docs.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from repo2docs.llm import OpenAIClient, AnthropicClient, LLMClient
 from repo2docs.prompts import documentation_prompt, diagram_prompt, mobile_prompt, database_prompt
 
 load_dotenv()
 
 class TextToDocs:
     def __init__(self, api_choice):
-        print(f"Initializing TextToDocs with API choice: {api_choice}")  # Debug statement
         if api_choice == "anthropic":
             api_key = os.getenv("ANTHROPIC_API_KEY")
             if not api_key:
                 api_key = LLMClient.get_api_key('ANTHROPIC_API_KEY', 'Anthropic')
             self.client = AnthropicClient(api_key=api_key)
         elif api_choice == "openai":
             api_key = os.getenv("OPENAI_API_KEY")
```

### Comparing `repo2docs-0.1.5/PKG-INFO` & `repo2docs-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2docs
-Version: 0.1.5
+Version: 0.1.6
 Summary: Documentation from your codebase using LLMs
 License: MIT
 Author: Joe Petrantoni
 Author-email: 79169021+jpetrantoni@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
    ```
    repo2docs --dir_path . --output_file documentation.md --type documentation --llm openai
    ```
 
    To generate mobile documentation, use `--type mobile`.
    To generate diagrams instead of documentation, use `--type diagram`.
    To generate database erd diagrams, use `--type database`.
-   To generate custom documentation, use `--type custom` and provide a custom prompt with `--prompt <prompt>`.
+   To use a custom prompt, use `--prompt <prompt>`.
 
 ## Supported File Types
 
 Repo2Docs currently supports processing files with the following extensions: `.py`, `.js`, `.jsx`, `.ts`, `.tsx`, `.c`, `.cpp`, `.h`, `.hpp`. It filters out files from directories like `docs`, `examples`, `tests`, and others that are unlikely to contain useful information for documentation.
 
 ## Contributing
```

