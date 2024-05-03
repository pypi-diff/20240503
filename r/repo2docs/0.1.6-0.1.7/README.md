# Comparing `tmp/repo2docs-0.1.6.tar.gz` & `tmp/repo2docs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2docs-0.1.6.tar", max compression
+gzip compressed data, was "repo2docs-0.1.7.tar", max compression
```

## Comparing `repo2docs-0.1.6.tar` & `repo2docs-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.6/LICENSE
--rw-r--r--   0        0        0     2628 2024-05-03 03:02:40.392117 repo2docs-0.1.6/README.md
--rw-r--r--   0        0        0      506 2024-05-03 03:02:17.949745 repo2docs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.6/repo2docs/__init__.py
--rw-r--r--   0        0        0     2044 2024-05-03 03:01:00.838466 repo2docs-0.1.6/repo2docs/llm.py
--rw-r--r--   0        0        0     6565 2024-05-03 01:45:59.090148 repo2docs-0.1.6/repo2docs/prompts.py
--rw-r--r--   0        0        0     3283 2024-05-03 03:02:01.367859 repo2docs-0.1.6/repo2docs/repo2docs.py
--rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.6/repo2docs/repo_to_text.py
--rw-r--r--   0        0        0     2262 2024-05-03 03:01:35.532506 repo2docs-0.1.6/repo2docs/text_to_docs.py
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 repo2docs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-21 08:05:48.817339 repo2docs-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2628 2024-05-03 03:02:40.392117 repo2docs-0.1.7/README.md
+-rw-r--r--   0        0        0      506 2024-05-03 03:08:19.517405 repo2docs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-21 06:47:26.694676 repo2docs-0.1.7/repo2docs/__init__.py
+-rw-r--r--   0        0        0     2044 2024-05-03 03:01:00.838466 repo2docs-0.1.7/repo2docs/llm.py
+-rw-r--r--   0        0        0     6665 2024-05-03 03:08:11.468685 repo2docs-0.1.7/repo2docs/prompts.py
+-rw-r--r--   0        0        0     3283 2024-05-03 03:02:01.367859 repo2docs-0.1.7/repo2docs/repo2docs.py
+-rw-r--r--   0        0        0     8778 2024-03-21 20:13:27.632756 repo2docs-0.1.7/repo2docs/repo_to_text.py
+-rw-r--r--   0        0        0     2262 2024-05-03 03:01:35.532506 repo2docs-0.1.7/repo2docs/text_to_docs.py
+-rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 repo2docs-0.1.7/PKG-INFO
```

### Comparing `repo2docs-0.1.6/LICENSE` & `repo2docs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.6/README.md` & `repo2docs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.6/repo2docs/llm.py` & `repo2docs-0.1.7/repo2docs/llm.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.6/repo2docs/prompts.py` & `repo2docs-0.1.7/repo2docs/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 documentation_prompt = """
-You are an AI assistant helping to prepare information for a provisional patent application for a software system. Your task is to generate detailed documentation based on the provided code and system description.
+You are an AI assistant helping to prepare a detailed documentation for a software system. Your task is to generate detailed documentation based on the provided code and system description.
 
 Please follow these steps:
 
 1. Analyze the provided code and system description to understand the key components, functionalities, and interactions of the software system.
 
 2. Generate a detailed documentation in Markdown (.md) format, covering the following aspects:
    - Overview of the system
@@ -15,21 +15,21 @@
    - Integration with external services or APIs
    - Data storage and management
 
 3. Use appropriate Markdown syntax for headings, lists, code blocks, and other formatting elements.
 
 4. Where necessary, include diagrams to illustrate the system architecture, components, or workflows using mermaid syntax in Markdown.
 
-5. Be detailed, accurate, and clear in your explanations. Your output will be used to assist in preparing a provisional patent application, so it should be comprehensive and professionally written.
+5. Be detailed, accurate, and clear in your explanations. Your output should be comprehensive and professionally written.
 
-6. Your response will be saved as a markdown file, so ensure the formatting is correct and omit any extraneous information that does not pertain to the documentation.
+6. Your response will be saved as a markdown file, so ensure the formatting is correct and omit any extraneous information that does not pertain to the documentation (Do not wrap ```markdown in the output)
 """
 
 diagram_prompt = """
-You are an AI assistant helping to prepare diagrams for a provisional patent application for a software system. Your task is to create diagrams based on the documentation generated in the previous step.
+You are an AI assistant helping to prepare detailed diagrams for a software system. Your task is to create diagrams based on the documentation generated in the previous step.
 
 Please follow these steps:
 
 1. Review the documentation generated in the previous step to understand the system architecture, user interactions, and key processes.
 
 2. Create diagrams to visually represent the following aspects:
    - Overall system architecture
@@ -41,15 +41,18 @@
 
 3. Use a code-based diagramming syntax, such as Mermaid, to generate the diagrams. Provide the diagram code in the Markdown output.
 
 4. Provide a brief explanation or caption for each diagram to clarify its purpose and content.
 
 5. Generate the output in Markdown (.md) format, clearly separating the diagram code and explanations.
 
-6. Ensure that the diagrams are clear, accurate, and visually appealing. They should effectively communicate the system's architecture and processes to assist in preparing the provisional patent application.
+6. Ensure that the diagrams are clear, accurate, and visually appealing. They should effectively communicate the system's architecture and processes.
+
+7. Your response will be saved as a markdown file, so ensure the formatting is correct and omit any extraneous information that does not pertain to the documentation (Do not wrap ```markdown in the output)
+
 """
 
 database_prompt = """
 You are an AI assistant specialized in generating Entity-Relationship Diagrams (ERDs) from codebases that include database models and schemas. Your task is to analyze the provided codebase, identify the relevant database information, and create a clear and accurate ERD representation using Mermaid syntax.
 
 Please follow these steps:
 
@@ -97,9 +100,9 @@
    - Integration with device features (e.g., camera, GPS, sensors)
    - Data storage and management
    - Integration with backend services or APIs
    - Security and privacy considerations
 
 3. Use appropriate Markdown syntax for headings, lists, code blocks, and other formatting elements.
 
-4. Your response will be saved as a markdown file, so ensure the formatting is correct and omit any extraneous information that does not pertain to the documentation.
+4. Your response will be saved as a markdown file, so ensure the formatting is correct and omit any extraneous information that does not pertain to the documentation (Do not wrap ```markdown in the output)
 """
```

### Comparing `repo2docs-0.1.6/repo2docs/repo2docs.py` & `repo2docs-0.1.7/repo2docs/repo2docs.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.6/repo2docs/repo_to_text.py` & `repo2docs-0.1.7/repo2docs/repo_to_text.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.6/repo2docs/text_to_docs.py` & `repo2docs-0.1.7/repo2docs/text_to_docs.py`

 * *Files identical despite different names*

### Comparing `repo2docs-0.1.6/PKG-INFO` & `repo2docs-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2docs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Documentation from your codebase using LLMs
 License: MIT
 Author: Joe Petrantoni
 Author-email: 79169021+jpetrantoni@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

