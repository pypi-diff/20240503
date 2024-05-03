# Comparing `tmp/repo2docs-0.1.8.tar.gz` & `tmp/repo2docs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2docs-0.1.8.tar", max compression
+gzip compressed data, was "repo2docs-0.1.9.tar", max compression
```

## Comparing `repo2docs-0.1.8.tar` & `repo2docs-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.8/LICENSE
--rw-r--r--   0        0        0     2680 2024-05-03 03:11:07.963220 repo2docs-0.1.8/README.md
--rw-r--r--   0        0        0      506 2024-05-03 03:11:14.324582 repo2docs-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.8/repo2docs/__init__.py
--rw-r--r--   0        0        0     2044 2024-05-03 03:01:00.838466 repo2docs-0.1.8/repo2docs/llm.py
--rw-r--r--   0        0        0     6665 2024-05-03 03:08:11.468685 repo2docs-0.1.8/repo2docs/prompts.py
--rw-r--r--   0        0        0     3283 2024-05-03 03:02:01.367859 repo2docs-0.1.8/repo2docs/repo2docs.py
--rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.8/repo2docs/repo_to_text.py
--rw-r--r--   0        0        0     2262 2024-05-03 03:01:35.532506 repo2docs-0.1.8/repo2docs/text_to_docs.py
--rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 repo2docs-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3262 2024-05-03 03:20:32.673129 repo2docs-0.1.9/README.md
+-rw-r--r--   0        0        0      506 2024-05-03 03:20:39.860174 repo2docs-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.9/repo2docs/__init__.py
+-rw-r--r--   0        0        0     2124 2024-05-03 03:17:16.427229 repo2docs-0.1.9/repo2docs/llm.py
+-rw-r--r--   0        0        0     6665 2024-05-03 03:08:11.468685 repo2docs-0.1.9/repo2docs/prompts.py
+-rw-r--r--   0        0        0     3381 2024-05-03 03:17:20.195701 repo2docs-0.1.9/repo2docs/repo2docs.py
+-rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.9/repo2docs/repo_to_text.py
+-rw-r--r--   0        0        0     2274 2024-05-03 03:16:00.587464 repo2docs-0.1.9/repo2docs/text_to_docs.py
+-rw-r--r--   0        0        0     3960 1970-01-01 00:00:00.000000 repo2docs-0.1.9/PKG-INFO
```

### Comparing `repo2docs-0.1.8/LICENSE` & `repo2docs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.8/README.md` & `repo2docs-0.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -49,21 +49,31 @@
 
    cd into the directory where the repo is located
    ```
    cd <path_to_repo>
    ```
    Run the following command to generate documentation:
    ```
-   repo2docs --dir_path . --output_file documentation.md --type documentation --llm openai
+   repo2docs --dir_path <path_to_repo> --output_file <output_file> --type <type> --llm <llm>
    ```
 
-   To generate mobile documentation, use `--type mobile`.
-   To generate diagrams instead of documentation, use `--type diagram`.
-   To generate database erd diagrams, use `--type database`.
-   To use a custom prompt, use `--prompt "<prompt>"`.
+   - Leaving `dir_path` empty will default to the current directory.
+   - Leaving `output_file` empty will default to `output.md`.
+   - Leaving `type` empty will default to `documentation`.
+     - To generate mobile documentation, use `--type mobile`.
+     - To generate diagrams instead of documentation, use `--type diagram`.
+     - To generate database erd diagrams, use `--type database`.
+     - To use a custom prompt,leave `type` empty and use `--prompt "<prompt>"`.
+   - Leaving `llm` empty will default to `openai`.
+     - To use Anthropic, use `--llm anthropic`.
+       - Defaults to `claude-3-haiku-20240307`.
+       - To use a specific model, use `--llm anthropic:<model>`.
+     - To use OpenAI, use `--llm openai`.
+       - Defaults to `gpt-4-turbo`.
+       - To use a specific model, use `--llm openai:<model>`.
 
 ## Supported File Types
 
 Repo2Docs currently supports processing files with the following extensions: `.py`, `.js`, `.jsx`, `.ts`, `.tsx`, `.c`, `.cpp`, `.h`, `.hpp`. It filters out files from directories like `docs`, `examples`, `tests`, and others that are unlikely to contain useful information for documentation.
 
 ## Contributing
```

### Comparing `repo2docs-0.1.8/repo2docs/llm.py` & `repo2docs-0.1.9/repo2docs/llm.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,51 +22,53 @@
         api_key = os.getenv(env_var)
         if not api_key:
             print(f"API key for {client_name} ({env_var}) not found. Please enter your API key:")
             api_key = getpass.getpass(prompt='')
         return api_key
 
 class OpenAIClient(LLMClient):
-    def __init__(self, api_key=None):
+    def __init__(self, api_key=None, model=None):
         if not api_key:
             api_key = self.get_api_key('OPENAI_API_KEY', 'OpenAI')
+        if not model:
+            model = 'gpt-4-turbo'
         self.client = openai.OpenAI(api_key=api_key)
 
     def generate_response(
         self,
         prompt,
-        model="gpt-4-turbo-preview",
         max_tokens=4000,
         temperature=0.5,
         messages=[],
     ):
         response = self.client.chat.completions.create(
-            model=model,
+            model=self.model,
             max_tokens=max_tokens,
             temperature=temperature,
             messages=[{"role": "system", "content": prompt}, *messages],
         )
         return response.choices[0].message.content
 
 
 class AnthropicClient(LLMClient):
-    def __init__(self, api_key=None):
+    def __init__(self, api_key=None, model=None):
         if not api_key:
             api_key = self.get_api_key('ANTHROPIC_API_KEY', 'Anthropic')
+        if not model:
+            model = 'claude-3-haiku-20240307'
         self.client = anthropic.Anthropic(api_key=api_key)
 
     def generate_response(
         self,
         prompt,
-        model="claude-3-haiku-20240307",
         max_tokens=4000,
         temperature=0.5,
         messages=[],
     ):
         response = self.client.messages.create(
-            model=model,
+            model=self.model,
             max_tokens=max_tokens,
             temperature=temperature,
             system=prompt,
             messages=messages,
         )
         return response.content[0].text
```

### Comparing `repo2docs-0.1.8/repo2docs/prompts.py` & `repo2docs-0.1.9/repo2docs/prompts.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.8/repo2docs/repo2docs.py` & `repo2docs-0.1.9/repo2docs/repo2docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,21 @@
     repo_processor = RepoProcessor(
         repo_zip_path, None, ignore_dirs
     )
     repo_text = repo_processor.process_repo()
 
     logging.info(f"Repository text has been successfully processed.")
     
+    if ":" in llm:
+        llm, model = llm.split(":")
+    else:
+        model = None
+    
     # Convert the repository text to documentation
-    text_to_docs = TextToDocs(llm)
+    text_to_docs = TextToDocs(llm, model)
     if prompt:
         docs_content = text_to_docs.generate_custom(repo_text, prompt)
     elif doc_type == "diagram":
         docs_content = text_to_docs.generate_diagram(repo_text)
     elif doc_type == "database":
         docs_content = text_to_docs.generate_database(repo_text)
     elif doc_type == "mobile":
```

### Comparing `repo2docs-0.1.8/repo2docs/repo_to_text.py` & `repo2docs-0.1.9/repo2docs/repo_to_text.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.8/repo2docs/text_to_docs.py` & `repo2docs-0.1.9/repo2docs/text_to_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dotenv import load_dotenv
 from repo2docs.llm import OpenAIClient, AnthropicClient, LLMClient
 from repo2docs.prompts import documentation_prompt, diagram_prompt, mobile_prompt, database_prompt
 
 load_dotenv()
 
 class TextToDocs:
-    def __init__(self, api_choice):
+    def __init__(self, api_choice, model=None):
         if api_choice == "anthropic":
             api_key = os.getenv("ANTHROPIC_API_KEY")
             if not api_key:
                 api_key = LLMClient.get_api_key('ANTHROPIC_API_KEY', 'Anthropic')
             self.client = AnthropicClient(api_key=api_key)
         elif api_choice == "openai":
             api_key = os.getenv("OPENAI_API_KEY")
```

