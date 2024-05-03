# Comparing `tmp/repo2docs-0.1.0.tar.gz` & `tmp/repo2docs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2docs-0.1.0.tar", max compression
+gzip compressed data, was "repo2docs-0.1.1.tar", max compression
```

## Comparing `repo2docs-0.1.0.tar` & `repo2docs-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.0/LICENSE
--rw-r--r--   0        0        0     3234 2024-05-02 23:59:49.152932 repo2docs-0.1.0/README.md
--rw-r--r--   0        0        0      507 2024-05-03 01:39:22.832744 repo2docs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.0/repo2docs/__init__.py
--rw-r--r--   0        0        0     1456 2024-05-02 23:52:41.042589 repo2docs-0.1.0/repo2docs/llm.py
--rw-r--r--   0        0        0      677 2024-03-21 06:47:21.128940 repo2docs-0.1.0/repo2docs/prompt_loader.py
--rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.0/repo2docs/prompts.py
--rw-r--r--   0        0        0     3307 2024-05-03 01:54:52.888384 repo2docs-0.1.0/repo2docs/repo2docs.py
--rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.0/repo2docs/repo_to_text.py
--rw-r--r--   0        0        0     2098 2024-05-03 01:52:50.826712 repo2docs-0.1.0/repo2docs/text_to_docs.py
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 repo2docs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2576 2024-05-03 02:03:32.612872 repo2docs-0.1.1/README.md
+-rw-r--r--   0        0        0      507 2024-05-03 02:03:51.229643 repo2docs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.1/repo2docs/__init__.py
+-rw-r--r--   0        0        0     1456 2024-05-03 01:56:39.798050 repo2docs-0.1.1/repo2docs/llm.py
+-rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.1/repo2docs/prompts.py
+-rw-r--r--   0        0        0     3268 2024-05-03 01:56:53.227931 repo2docs-0.1.1/repo2docs/repo2docs.py
+-rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.1/repo2docs/repo_to_text.py
+-rw-r--r--   0        0        0     2098 2024-05-03 01:52:50.826712 repo2docs-0.1.1/repo2docs/text_to_docs.py
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 repo2docs-0.1.1/PKG-INFO
```

### Comparing `repo2docs-0.1.0/LICENSE` & `repo2docs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.0/README.md` & `repo2docs-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: repo2docs
+Version: 0.1.1
+Summary: Documentation from your codebase using LLMs
+License: MIT
+Author: Joe Petrantoni
+Author-email: 79169021+jpetrantoni@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anthropic (>=0.25.7,<0.26.0)
+Requires-Dist: instructor (>=1.2.5,<2.0.0)
+Requires-Dist: openai (>=1.25.1,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Description-Content-Type: text/markdown
+
 # Repo2Docs: Convert GitHub Repositories to Documentation
 
 Inspired by [github2file](https://github.com/cognitivecomputations/github2file)
 
 Repo2Docs is a Python-based tool designed to convert the contents of a GitHub repository into comprehensive documentation or diagrams. This tool leverages language model APIs such as OpenAI or Anthropic to process and generate documentation, making it easier for developers to create documentation for their projects.
 
 ## How It Works
@@ -21,59 +40,40 @@
     LLM->>TD: Return generated content
     TD->>Main: Return documentation
     Main->>U: Save documentation to file
 ```
 *Caption: This sequence diagram illustrates the flow of interactions from the user executing the script to the generation and saving of documentation.*
 
 
-## Running Repo2Docs Locally
+## Using Repo2Docs
 
 To run Repo2Docs on your local machine, follow these steps:
 
-1. **Clone the Repository**:
+1. **Install Repo2Docs**:
    ```
-   git clone https://github.com/earlybird-labs/repo2docs.git
-   cd repo2docs
+   pip install repo2docs
    ```
 
-2. **Create and Activate Virtual Environment**:
 
-   First, ensure you have Python installed on your system. Then, create a virtual environment and activate it:
-   
-   For macOS/Linux:
-   ```
-   python3 -m venv venv
-   source venv/bin/activate
+2. **Set Up Environment Variables**:
+   Export your OpenAI and Anthropic API keys as environment variables:
    ```
-   
-   For Windows:
-   ```
-   python -m venv venv
-   .\venv\Scripts\activate
+   export OPENAI_API_KEY=your_openai_api_key_here
+   export ANTHROPIC_API_KEY=your_anthropic_api_key_here
    ```
 
-   **Install Dependencies**:
-   
-   After activating the virtual environment, install the required dependencies by running:
-   ```
-   pip install -r requirements.txt
-   ```
+3. **Run the Tool**:
 
-3. **Set Up Environment Variables**:
-   Create a `.env` file in the root directory and add your language model API keys:
+   cd into the directory where the repo is located
    ```
-   OPENAI_API_KEY=your_openai_api_key_here
-   ANTHROPIC_API_KEY=your_anthropic_api_key_here
+   cd <path_to_repo>
    ```
-
-4. **Run the Tool**:
-   Use the following command to convert a repository to documentation. Replace `path_to_repo.zip` and `output_file.md` with your repository's `.zip` file path and your desired output file path, respectively.
+   Run the following command to generate documentation:
    ```
-   cd src
-   python repo2docs.py input/path_to_repo.zip output/output_file.md --type documentation --llm openai
+   repo2docs --dir_path . --output_file documentation.md --type documentation --llm openai
    ```
 
    To generate mobile documentation, use `--type mobile`.
    To generate diagrams instead of documentation, use `--type diagram`.
    To generate database erd diagrams, use `--type database`.
 
 ## Supported File Types
@@ -86,7 +86,8 @@
 
 ## License
 
 Repo2Docs is released under the MIT License. See the LICENSE file for more details.
 
 
 
+
```

### Comparing `repo2docs-0.1.0/repo2docs/llm.py` & `repo2docs-0.1.1/repo2docs/llm.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.0/repo2docs/prompts.py` & `repo2docs-0.1.1/repo2docs/prompts.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.0/repo2docs/repo2docs.py` & `repo2docs-0.1.1/repo2docs/repo2docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
                 zipf.write(os.path.join(root, file), os.path.relpath(os.path.join(root, file), os.path.join(dir_path, '..')))
 
     # Process the .zip file to get repository text
     repo_processor = RepoProcessor(
         repo_zip_path, None, ignore_dirs
     )
     repo_text = repo_processor.process_repo()
-    print(repo_text)
-    print("Test")
 
     logging.info(f"Repository text has been successfully processed.")
     
     # Convert the repository text to documentation
     text_to_docs = TextToDocs(llm)
     if doc_type == "diagram":
         docs_content = text_to_docs.generate_diagram(repo_text)
```

### Comparing `repo2docs-0.1.0/repo2docs/repo_to_text.py` & `repo2docs-0.1.1/repo2docs/repo_to_text.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.0/repo2docs/text_to_docs.py` & `repo2docs-0.1.1/repo2docs/text_to_docs.py`

 * *Files identical despite different names*

