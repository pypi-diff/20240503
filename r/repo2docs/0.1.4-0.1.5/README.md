# Comparing `tmp/repo2docs-0.1.4.tar.gz` & `tmp/repo2docs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2docs-0.1.4.tar", max compression
+gzip compressed data, was "repo2docs-0.1.5.tar", max compression
```

## Comparing `repo2docs-0.1.4.tar` & `repo2docs-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.4/LICENSE
--rw-r--r--   0        0        0     2576 2024-05-03 02:03:32.612872 repo2docs-0.1.4/README.md
--rw-r--r--   0        0        0      507 2024-05-03 02:22:06.107200 repo2docs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.4/repo2docs/__init__.py
--rw-r--r--   0        0        0     2011 2024-05-03 02:12:41.755256 repo2docs-0.1.4/repo2docs/llm.py
--rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.4/repo2docs/prompts.py
--rw-r--r--   0        0        0     3268 2024-05-03 02:15:09.238936 repo2docs-0.1.4/repo2docs/repo2docs.py
--rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.4/repo2docs/repo_to_text.py
--rw-r--r--   0        0        0     2140 2024-05-03 02:19:11.424381 repo2docs-0.1.4/repo2docs/text_to_docs.py
--rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 repo2docs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2687 2024-05-03 02:31:53.127912 repo2docs-0.1.5/README.md
+-rw-r--r--   0        0        0      507 2024-05-03 02:52:24.229912 repo2docs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.5/repo2docs/__init__.py
+-rw-r--r--   0        0        0     2011 2024-05-03 02:12:41.755256 repo2docs-0.1.5/repo2docs/llm.py
+-rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.5/repo2docs/prompts.py
+-rw-r--r--   0        0        0     3576 2024-05-03 02:50:47.360967 repo2docs-0.1.5/repo2docs/repo2docs.py
+-rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.5/repo2docs/repo_to_text.py
+-rw-r--r--   0        0        0     2353 2024-05-03 02:40:00.488875 repo2docs-0.1.5/repo2docs/text_to_docs.py
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 repo2docs-0.1.5/PKG-INFO
```

### Comparing `repo2docs-0.1.4/LICENSE` & `repo2docs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.4/README.md` & `repo2docs-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
    ```
    repo2docs --dir_path . --output_file documentation.md --type documentation --llm openai
    ```
 
    To generate mobile documentation, use `--type mobile`.
    To generate diagrams instead of documentation, use `--type diagram`.
    To generate database erd diagrams, use `--type database`.
+   To generate custom documentation, use `--type custom` and provide a custom prompt with `--prompt <prompt>`.
 
 ## Supported File Types
 
 Repo2Docs currently supports processing files with the following extensions: `.py`, `.js`, `.jsx`, `.ts`, `.tsx`, `.c`, `.cpp`, `.h`, `.hpp`. It filters out files from directories like `docs`, `examples`, `tests`, and others that are unlikely to contain useful information for documentation.
 
 ## Contributing
```

### Comparing `repo2docs-0.1.4/repo2docs/llm.py` & `repo2docs-0.1.5/repo2docs/llm.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.4/repo2docs/prompts.py` & `repo2docs-0.1.5/repo2docs/prompts.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.4/repo2docs/repo2docs.py` & `repo2docs-0.1.5/repo2docs/repo2docs.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,17 +26,20 @@
     repo_processor = RepoProcessor(
         repo_zip_path, None, ignore_dirs
     )
     repo_text = repo_processor.process_repo()
 
     logging.info(f"Repository text has been successfully processed.")
     
+    print(f"LLM choice received: {llm}")
+    
     # Convert the repository text to documentation
     text_to_docs = TextToDocs(llm)
-    if prompt:
+    if doc_type == "custom":
+        print(f"Custom prompt provided: {prompt}")
         docs_content = text_to_docs.generate_custom(repo_text, prompt)
     elif doc_type == "diagram":
         docs_content = text_to_docs.generate_diagram(repo_text)
     elif doc_type == "database":
         docs_content = text_to_docs.generate_database(repo_text)
     elif doc_type == "mobile":
         docs_content = text_to_docs.generate_mobile(repo_text)
@@ -50,15 +53,20 @@
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     with open(output_file, "w", encoding="utf-8") as outfile:
         outfile.write(docs_content)
     logging.info(f"Documentation has been successfully saved to {output_file}.")
 
+
+
+
 if __name__ == "__main__":
+    print("Running repo2docs")
+    
     logging.basicConfig(level=logging.INFO)
 
     parser = argparse.ArgumentParser(
         description="Convert a directory into documentation."
     )
     parser.add_argument(
         "--dir_path", 
@@ -66,34 +74,34 @@
         default="."
     )
     parser.add_argument(
         "--output_file",
         help="The output file path where the documentation will be saved.",
         default="output.md",
     )
-    
     parser.add_argument(
         "--prompt",
         help="The prompt to use for generating the documentation.",
         default=None
     )
-    
     parser.add_argument(
         "--type",
-        choices=["documentation", "diagram", "database", "mobile"],
+        dest="doc_type",  # Ensure this matches the parameter name in main
+        choices=["documentation", "diagram", "database", "mobile", "custom"],
         default="documentation",
         help="Specify the type of documentation to generate.",
     )
     parser.add_argument(
         "--llm",
         choices=["openai", "anthropic"],
-        default="openai",
+        default="anthropic",
         help="Specify the language model API to use for generating documentation.",
     )
     parser.add_argument(
         "--ignore_dirs", nargs="*", default=[], help="List of directories to ignore."
     )
 
     args = parser.parse_args()
+    print(args)  # Debug: Print all parsed arguments to verify their values
 
-    main(args.dir_path, args.output_file, args.prompt, args.type, args.llm, args.ignore_dirs)
+    main(args.dir_path, args.output_file, args.prompt, args.doc_type, args.llm, args.ignore_dirs)
```

### Comparing `repo2docs-0.1.4/repo2docs/repo_to_text.py` & `repo2docs-0.1.5/repo2docs/repo_to_text.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.4/repo2docs/text_to_docs.py` & `repo2docs-0.1.5/repo2docs/text_to_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 from dotenv import load_dotenv
-from repo2docs.llm import OpenAIClient, AnthropicClient
+from repo2docs.llm import OpenAIClient, AnthropicClient, LLMClient
 from repo2docs.prompts import documentation_prompt, diagram_prompt, mobile_prompt, database_prompt
 
 load_dotenv()
 
-
 class TextToDocs:
-    """A class to convert text to documentation using a language model API."""
-
     def __init__(self, api_choice):
+        print(f"Initializing TextToDocs with API choice: {api_choice}")  # Debug statement
         if api_choice == "anthropic":
             api_key = os.getenv("ANTHROPIC_API_KEY")
+            if not api_key:
+                api_key = LLMClient.get_api_key('ANTHROPIC_API_KEY', 'Anthropic')
             self.client = AnthropicClient(api_key=api_key)
         elif api_choice == "openai":
             api_key = os.getenv("OPENAI_API_KEY")
+            if not api_key:
+                api_key = LLMClient.get_api_key('OPENAI_API_KEY', 'OpenAI')
             self.client = OpenAIClient(api_key=api_key)
         else:
-            raise ValueError(
-                "Invalid API choice. Please choose either 'anthropic' or 'openai'."
-            )
-
+            raise ValueError("Invalid API choice. Please choose either 'anthropic' or 'openai'.")
+        
     def generate_docs(self, repo_txt):
         """Generate documentation from the text."""
         response = self.client.generate_response(
             prompt=documentation_prompt,
             messages=[{"role": "user", "content": repo_txt}],
         )
         return response
```

### Comparing `repo2docs-0.1.4/PKG-INFO` & `repo2docs-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2docs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Documentation from your codebase using LLMs
 License: MIT
 Author: Joe Petrantoni
 Author-email: 79169021+jpetrantoni@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -71,14 +71,15 @@
    ```
    repo2docs --dir_path . --output_file documentation.md --type documentation --llm openai
    ```
 
    To generate mobile documentation, use `--type mobile`.
    To generate diagrams instead of documentation, use `--type diagram`.
    To generate database erd diagrams, use `--type database`.
+   To generate custom documentation, use `--type custom` and provide a custom prompt with `--prompt <prompt>`.
 
 ## Supported File Types
 
 Repo2Docs currently supports processing files with the following extensions: `.py`, `.js`, `.jsx`, `.ts`, `.tsx`, `.c`, `.cpp`, `.h`, `.hpp`. It filters out files from directories like `docs`, `examples`, `tests`, and others that are unlikely to contain useful information for documentation.
 
 ## Contributing
```

