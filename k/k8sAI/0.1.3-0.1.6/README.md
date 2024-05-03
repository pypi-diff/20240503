# Comparing `tmp/k8sai-0.1.3.tar.gz` & `tmp/k8sai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8sai-0.1.3.tar", last modified: Fri May  3 02:16:36 2024, max compression
+gzip compressed data, was "k8sai-0.1.6.tar", last modified: Fri May  3 08:33:51 2024, max compression
```

## Comparing `k8sai-0.1.3.tar` & `k8sai-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.233478 k8sai-0.1.3/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.3/LICENSE
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.3/MANIFEST.in
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3723 2024-05-03 02:16:36.233252 k8sai-0.1.3/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.3/README.md
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.214641 k8sai-0.1.3/k8sAI/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.3/k8sAI/__init__.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.216912 k8sai-0.1.3/k8sAI/kuberag/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.3/k8sAI/kuberag/__init__.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     2599 2024-05-02 00:01:57.000000 k8sai-0.1.3/k8sAI/kuberag/chat.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.217279 k8sai-0.1.3/k8sAI/kuberag/embeddings/
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.232789 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/chroma.sqlite3
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3501 2024-05-03 01:47:59.000000 k8sai-0.1.3/k8sAI/kuberag/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.3/k8sAI/kuberag/retriever.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.3/k8sAI/kuberag/tool_handler.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     6695 2024-05-03 01:51:44.000000 k8sai-0.1.3/k8sAI/kuberag/tools.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4185 2024-05-03 01:41:36.000000 k8sai-0.1.3/k8sAI/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       87 2024-05-01 22:29:29.000000 k8sai-0.1.3/k8sAI/util.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.232976 k8sai-0.1.3/k8sAI.egg-info/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3723 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/entry_points.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       65 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/requires.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/top_level.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-03 02:16:36.233515 k8sai-0.1.3/setup.cfg
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      670 2024-05-03 01:52:57.000000 k8sai-0.1.3/setup.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.162188 k8sai-0.1.6/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.6/LICENSE
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.6/MANIFEST.in
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3766 2024-05-03 08:33:51.161916 k8sai-0.1.6/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.6/README.md
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.139921 k8sai-0.1.6/k8sAI/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.6/k8sAI/__init__.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.142363 k8sai-0.1.6/k8sAI/kuberag/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.6/k8sAI/kuberag/__init__.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     2680 2024-05-03 03:56:55.000000 k8sai-0.1.6/k8sAI/kuberag/chat.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.142597 k8sai-0.1.6/k8sAI/kuberag/embeddings/
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.157220 k8sai-0.1.6/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.6/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.6/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.6/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.6/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.6/k8sAI/kuberag/embeddings/chroma.sqlite3
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3501 2024-05-03 01:47:59.000000 k8sai-0.1.6/k8sAI/kuberag/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.6/k8sAI/kuberag/retriever.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.6/k8sAI/kuberag/tool_handler.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     6926 2024-05-03 06:45:53.000000 k8sai-0.1.6/k8sAI/kuberag/tools.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4345 2024-05-03 06:43:38.000000 k8sai-0.1.6/k8sAI/main.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.157436 k8sai-0.1.6/k8sAI/usage/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 06:31:05.000000 k8sai-0.1.6/k8sAI/usage/__init__.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     2905 2024-05-03 08:17:49.000000 k8sai-0.1.6/k8sAI/usage/usage.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      139 2024-05-03 06:42:49.000000 k8sai-0.1.6/k8sAI/util.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:33:51.161645 k8sai-0.1.6/k8sAI.egg-info/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3766 2024-05-03 08:33:51.000000 k8sai-0.1.6/k8sAI.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      796 2024-05-03 08:33:51.000000 k8sai-0.1.6/k8sAI.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-03 08:33:51.000000 k8sai-0.1.6/k8sAI.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-03 08:33:51.000000 k8sai-0.1.6/k8sAI.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       78 2024-05-03 08:33:51.000000 k8sai-0.1.6/k8sAI.egg-info/requires.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-03 08:33:51.000000 k8sai-0.1.6/k8sAI.egg-info/top_level.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-03 08:33:51.162233 k8sai-0.1.6/setup.cfg
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      752 2024-05-03 08:33:47.000000 k8sai-0.1.6/setup.py
```

### Comparing `k8sai-0.1.3/LICENSE` & `k8sai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.3/PKG-INFO` & `k8sai-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.3
+Version: 0.1.6
 Summary: A conversational AI for Kubernetes users.
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: langchain
 Requires-Dist: langchain-chroma
 Requires-Dist: langchain_openai
 Requires-Dist: prompt_toolkit
+Requires-Dist: rich
+Requires-Dist: posthog
 
 # k8sAI
 
 k8sAI is a RAG-enabled GPT that uses a vector store with the embeddings of the [Kubernetes documentation](https://kubernetes.io/docs/).
 It can answer general questions about Kubernetes, explain output of provided kubectl commands, and suggested commands for you to then easily execute.
 Given an issue, it can also use kubectl commands to understand the issue and suggest a fix.
```

### Comparing `k8sai-0.1.3/README.md` & `k8sai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.3/k8sAI/kuberag/chat.py` & `k8sai-0.1.6/k8sAI/kuberag/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 llm = ChatOpenAI(model="gpt-4")
 
 chat_prompt = ChatPromptTemplate.from_messages(
     [
         (
             "system",
-            "You are a helpful, concise chatbot and kubernetes expert. Use the tools you have at your disposal to \
-                get information about kubernetes or to suggest a command to the user. \
-                When possible and if provided, use the execute tool to gather more information about the cluster before answering. \
-                If you use the execute tool, be sure to use the results in future answers and to fill in information and arguments. \
-                If the user is providing a task to you, consider using the execute tool to solve it. \
-                Refer to the chat history to check for relevant previous conversations and information. \
-                Users can't see your tool call results, so be sure to state all findings at the end clearly. \
-                If the user is requesting you to investigate a problem, use your knowledge as best you can to \
-                follow the best practices for troubleshooting k8s. If you find an issue, suggest a fix! \
-                If nothing is wrong, and the user asks for a fix, concisely let them know everything looks healthy.\
-                Answer the user's questions based on your general knowledge of kubernetes, with your tools, \
-                and the following logs (if provided):\n\n{logs}\n\
-                Kubectl command output (optional):\n\n{command_output}",
+            "You are a helpful, concise chatbot and kubernetes expert. You are also a fully functioning SRE with a toolset at your disposal. Use the tools you have to \
+get information about kubernetes or to suggest a command to the user. \
+When possible and if provided, use the execute tool to gather more information about the cluster before answering. \
+If you use the execute tool, be sure to use the results in future answers and to fill in information and arguments. \
+If the user is providing a task to you, consider using the execute tool to solve it. \
+Refer to the chat history to check for relevant previous conversations and information. \
+Users can't see your tool call results, so be sure to state all findings at the end clearly. \
+If the user is requesting you to investigate a problem, use your knowledge as best you can to \
+follow the best practices for troubleshooting k8s. When investigating a problem for a fix, make sure you utilize the your execute tool. \
+If you find an issue, suggest a fix! If the user prompts you asking for a fix without a prompt, then take a wholistic look at the cluster health to try to find an issue. \
+If nothing is wrong, and the user asks for a fix, concisely let them know everything looks healthy.\
+Answer the user's questions based on your general knowledge of kubernetes, with your tools, \
+and the following logs (if provided):\n\n{logs}\n\
+Kubectl command output (optional):\n\n{command_output}",
         ),
         ("placeholder", "{chat_history}"),
         ("human", "{input}"),
         ("ai", "{agent_scratchpad}"),
     ]
 )
```

### Comparing `k8sai-0.1.3/k8sAI/kuberag/embeddings/chroma.sqlite3` & `k8sai-0.1.6/k8sAI/kuberag/embeddings/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.3/k8sAI/kuberag/main.py` & `k8sai-0.1.6/k8sAI/kuberag/main.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.3/k8sAI/kuberag/retriever.py` & `k8sai-0.1.6/k8sAI/kuberag/retriever.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.3/k8sAI/kuberag/tool_handler.py` & `k8sai-0.1.6/k8sAI/kuberag/tool_handler.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.3/k8sAI/kuberag/tools.py` & `k8sai-0.1.6/k8sAI/kuberag/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     AsyncCallbackManagerForToolRun,
     CallbackManagerForToolRun,
 )
 from langchain.tools.retriever import create_retriever_tool
 from langchain.pydantic_v1 import BaseModel, Field
 from langchain.tools import BaseTool
 from rich.padding import Padding
-from k8sAI.util import console
+from k8sAI.util import console, usage
 from prompt_toolkit import prompt
 from prompt_toolkit.styles import Style
 
 
 def retriever_tool(retriever):
     """
     Create the retriever tool.
@@ -62,14 +62,15 @@
 
     def _run(
         self,
         notes: str,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        usage.log_event("suggest_kubectl_command")
         if notes:
             console.print("\nNote: " + notes + "\n", style="italic")
         if query:
             cmd = prompt(
                 "Edit the cmd and press (enter) to run, leave empty to return to GPT\n\n",
                 default=query,
             )
@@ -115,14 +116,15 @@
     Under no circumstances should you modify underlying resources with this tool!!!"
     args_schema: Type[BaseModel] = ExecuteKubectlCommandInput
     return_direct: bool = False
 
     def _run(
         self, command: str, run_manager: Optional[CallbackManagerForToolRun] = None
     ) -> str:
+        usage.log_event("execute_kubectl_command")
         # execute command
         if not command.startswith("kubectl"):
             return "Error: Command must be kubectl command"
 
         allowed_patterns = [
             r"^kubectl get ",
             r"^kubectl describe ",
@@ -143,15 +145,17 @@
             )
         )
         console.print(Padding(command + "\n", pad=(0, 0, 0, 4)), style="yellow")
         user_response = ""
         while user_response.lower() not in ["y", "n"]:
             user_response = input("  Enter y/n to approve/deny: ")
         if user_response.lower() == "n":
+            usage.log_event("execute_kubectl_command_denied")
             return "User did not approve command execution. You can suggest the command instead."
+        usage.log_event("execute_kubectl_command_approved")
 
         try:
             console.print(
                 Padding(f":gear: running command: {command}", pad=(0, 0, 0, 2))
             )
             output = subprocess.check_output(command, shell=True).decode("utf-8")
             console.print(Padding(":green_circle: command complete", pad=(0, 0, 0, 2)))
```

### Comparing `k8sai-0.1.3/k8sAI/main.py` & `k8sai-0.1.6/k8sAI/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # file: k8sAI/main.py
 """
 This module contains the commands for the CLI.
 """
 
+from mimetypes import init
 import subprocess
 import click
 
 from k8sAI.kuberag.main import k8sAI
-from k8sAI.util import console
+from k8sAI.util import console, usage
 
 
 @click.group()
 def chat_group():
     """
     This tool uses OpenAI's ChatGPT to chat about Kubernetes.
     It is enhanced with a retriever storing k8s documentation to improve results.
@@ -40,14 +41,15 @@
                 be capable of executing kubectl commands (optional)",
 )
 def chat(prompt, terminal, disable_execution):
     """
     Start a conversation with the k8sAI model.
     k8sAI can suggest commands that can then be executed.
     """
+    usage.log_event("chat_command")
     kube_ai = k8sAI(disable_execution)
     console.print("\n:robot: starting conversation with k8sAI...", style="bold green")
     if not terminal:
         console.print("   type 'exit' to end the conversation.", style="italic")
 
     kube_ai.start_chat(prompt, terminal=terminal)
 
@@ -74,15 +76,15 @@
     help="If execution is disabled, k8sAI wil not be \
                 capable of executing kubectl commands (optional)",
 )
 def explain(cmd, prompt, terminal, disable_execution):
     """
     kubectl command will be executed and k8sAI will explain the result
     """
-
+    usage.log_event("explain_command")
     if not cmd.startswith("kubectl"):
         console.print("Error: Command must be kubectl command")
         return
 
     console.print(f":gear: running command: {cmd}")
     output = subprocess.check_output(cmd, shell=True).decode("utf-8")
     console.print(f":green_circle: command complete:\n{output}")
@@ -115,15 +117,15 @@
                 executing kubectl commands (optional)",
 )
 def fix(prompt, terminal, disable_execution):
     """
     k8sAI will suggest a fix based on a description of the problem
     (or try to find a problem if none is provided)
     """
-
+    usage.log_event("fix_command")
     enhanced_prompt = "Look for the root cause of the problem and suggest a fix."
     if prompt:
         enhanced_prompt += "The problem is:\n" + prompt
     else:
         enhanced_prompt += "Try to find the problem with your tools, \
             follow your best instincts for troubleshooting."
 
@@ -135,8 +137,9 @@
     kube_ai.start_chat(enhanced_prompt, terminal=terminal)
 
 
 def main():
     """
     Main function for the CLI.
     """
+    usage.setup()
     chat_group()
```

### Comparing `k8sai-0.1.3/k8sAI.egg-info/PKG-INFO` & `k8sai-0.1.6/k8sAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.3
+Version: 0.1.6
 Summary: A conversational AI for Kubernetes users.
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: langchain
 Requires-Dist: langchain-chroma
 Requires-Dist: langchain_openai
 Requires-Dist: prompt_toolkit
+Requires-Dist: rich
+Requires-Dist: posthog
 
 # k8sAI
 
 k8sAI is a RAG-enabled GPT that uses a vector store with the embeddings of the [Kubernetes documentation](https://kubernetes.io/docs/).
 It can answer general questions about Kubernetes, explain output of provided kubectl commands, and suggested commands for you to then easily execute.
 Given an issue, it can also use kubectl commands to understand the issue and suggest a fix.
```

### Comparing `k8sai-0.1.3/k8sAI.egg-info/SOURCES.txt` & `k8sai-0.1.6/k8sAI.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 k8sAI/kuberag/retriever.py
 k8sAI/kuberag/tool_handler.py
 k8sAI/kuberag/tools.py
 k8sAI/kuberag/embeddings/chroma.sqlite3
 k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
 k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
 k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
-k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
+k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
+k8sAI/usage/__init__.py
+k8sAI/usage/usage.py
```

### Comparing `k8sai-0.1.3/setup.py` & `k8sai-0.1.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from setuptools import setup, find_packages
+from setuptools.command.install import install
 
 setup(
     name="k8sAI",
-    version="0.1.3",
+    version="0.1.6",
     packages=find_packages(),
     description="A conversational AI for Kubernetes users.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Wilson Spearman",
     author_email="wilsonspearman@gmail.com",
     url="https://github.com/wilson090/k8sAI",
     include_package_data=True,
     install_requires=[
         "click",
         "langchain",
         "langchain-chroma",
         "langchain_openai",
         "prompt_toolkit",
+        "rich",
+        "posthog",
     ],
     entry_points="""
         [console_scripts]
         k8sAI=k8sAI.main:main
     """,
 )
```

