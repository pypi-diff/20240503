# Comparing `tmp/k8sai-0.1.2.tar.gz` & `tmp/k8sai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8sai-0.1.2.tar", last modified: Thu May  2 05:50:25 2024, max compression
+gzip compressed data, was "k8sai-0.1.3.tar", last modified: Fri May  3 02:16:36 2024, max compression
```

## Comparing `k8sai-0.1.2.tar` & `k8sai-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.441635 k8sai-0.1.2/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.2/LICENSE
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.2/MANIFEST.in
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3706 2024-05-02 05:50:25.441377 k8sai-0.1.2/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.2/README.md
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.426312 k8sai-0.1.2/k8sAI/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.2/k8sAI/__init__.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.428259 k8sai-0.1.2/k8sAI/kuberag/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.2/k8sAI/kuberag/__init__.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     2599 2024-05-02 00:01:57.000000 k8sai-0.1.2/k8sAI/kuberag/chat.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.428505 k8sai-0.1.2/k8sAI/kuberag/embeddings/
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.440862 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.2/k8sAI/kuberag/embeddings/chroma.sqlite3
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3415 2024-05-02 05:42:12.000000 k8sai-0.1.2/k8sAI/kuberag/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.2/k8sAI/kuberag/retriever.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.2/k8sAI/kuberag/tool_handler.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     6276 2024-05-02 05:42:12.000000 k8sai-0.1.2/k8sAI/kuberag/tools.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4144 2024-05-02 05:47:26.000000 k8sai-0.1.2/k8sAI/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       87 2024-05-01 22:29:29.000000 k8sai-0.1.2/k8sAI/util.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-02 05:50:25.441067 k8sai-0.1.2/k8sAI.egg-info/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3706 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/entry_points.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       65 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/requires.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-02 05:50:25.000000 k8sai-0.1.2/k8sAI.egg-info/top_level.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-02 05:50:25.441684 k8sai-0.1.2/setup.cfg
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      653 2024-05-02 05:42:12.000000 k8sai-0.1.2/setup.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.233478 k8sai-0.1.3/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.3/LICENSE
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.3/MANIFEST.in
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3723 2024-05-03 02:16:36.233252 k8sai-0.1.3/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.3/README.md
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.214641 k8sai-0.1.3/k8sAI/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.3/k8sAI/__init__.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.216912 k8sai-0.1.3/k8sAI/kuberag/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.3/k8sAI/kuberag/__init__.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     2599 2024-05-02 00:01:57.000000 k8sai-0.1.3/k8sAI/kuberag/chat.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.217279 k8sai-0.1.3/k8sAI/kuberag/embeddings/
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.232789 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.3/k8sAI/kuberag/embeddings/chroma.sqlite3
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3501 2024-05-03 01:47:59.000000 k8sai-0.1.3/k8sAI/kuberag/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.3/k8sAI/kuberag/retriever.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.3/k8sAI/kuberag/tool_handler.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     6695 2024-05-03 01:51:44.000000 k8sai-0.1.3/k8sAI/kuberag/tools.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4185 2024-05-03 01:41:36.000000 k8sai-0.1.3/k8sAI/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       87 2024-05-01 22:29:29.000000 k8sai-0.1.3/k8sAI/util.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 02:16:36.232976 k8sai-0.1.3/k8sAI.egg-info/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3723 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       65 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/requires.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-03 02:16:36.000000 k8sai-0.1.3/k8sAI.egg-info/top_level.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-03 02:16:36.233515 k8sai-0.1.3/setup.cfg
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      670 2024-05-03 01:52:57.000000 k8sai-0.1.3/setup.py
```

### Comparing `k8sai-0.1.2/LICENSE` & `k8sai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/PKG-INFO` & `k8sai-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.2
-Summary: A simple example package
+Version: 0.1.3
+Summary: A conversational AI for Kubernetes users.
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: langchain
```

### Comparing `k8sai-0.1.2/README.md` & `k8sai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/k8sAI/kuberag/chat.py` & `k8sai-0.1.3/k8sAI/kuberag/chat.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/k8sAI/kuberag/embeddings/chroma.sqlite3` & `k8sai-0.1.3/k8sAI/kuberag/embeddings/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/k8sAI/kuberag/main.py` & `k8sai-0.1.3/k8sAI/kuberag/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,30 +63,32 @@
                 config={"configurable": {"session_id": "<foo>"}},
             ):
                 # Agent Action
                 if "actions" in chunk:
                     for action in chunk["actions"]:
                         console.print(
                             Padding(
-                                f":hammer: Calling Tool: `{action.tool}` with input `\
-                                              {action.tool_input}`",
+                                f":hammer: Calling Tool: `{action.tool}` with input `{action.tool_input}`",
                                 pad=(0, 0, 0, 2),
-                            )
+                            ),
+                            style="italic bright_black",
                         )
                 # Observation
                 elif "steps" in chunk:
                     continue
                 # Final result
                 elif "output" in chunk:
                     if registry.has_tool_handler(chunk["output"]):
-                        additional_context, terminate = registry.use_handler(chunk["output"])
+                        additional_context, terminate = registry.use_handler(
+                            chunk["output"]
+                        )
                         if terminate:
                             break
                     else:
-                        console.print("k8sAI:")
+                        console.print("k8sAI:\n", style="bold green")
                         console.print(Markdown(chunk["output"]))
 
                 else:
                     raise ValueError()
                 console.print("---")
 
             if terminal:
```

### Comparing `k8sai-0.1.2/k8sAI/kuberag/retriever.py` & `k8sai-0.1.3/k8sAI/kuberag/retriever.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/k8sAI/kuberag/tool_handler.py` & `k8sai-0.1.3/k8sAI/kuberag/tool_handler.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/k8sAI/kuberag/tools.py` & `k8sai-0.1.3/k8sAI/kuberag/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from langchain.tools.retriever import create_retriever_tool
 from langchain.pydantic_v1 import BaseModel, Field
 from langchain.tools import BaseTool
 from rich.padding import Padding
 from k8sAI.util import console
 from prompt_toolkit import prompt
-
+from prompt_toolkit.styles import Style
 
 
 def retriever_tool(retriever):
     """
     Create the retriever tool.
     """
     return create_retriever_tool(
@@ -62,19 +62,16 @@
 
     def _run(
         self,
         notes: str,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
-        # return this as a jsonified string so that we can parse and return it in the frontend
-        data_dict = {"notes": notes, "query": query}
         if notes:
-            console.print("\n")
-            console.print(notes)
+            console.print("\nNote: " + notes + "\n", style="italic")
         if query:
             cmd = prompt(
                 "Edit the cmd and press (enter) to run, leave empty to return to GPT\n\n",
                 default=query,
             )
         args = cmd.split()
 
@@ -136,14 +133,26 @@
             r"^kubectl version",
             r"^kubectl config view",
             r"^kubectl logs ",
         ]
         if not any(re.match(pattern, command) for pattern in allowed_patterns):
             return "Error: Command is not permitted, must be a read-only operation"
 
+        console.print(
+            Padding(
+                "k8sAI is requesting to run the following command:", pad=(0, 0, 0, 2)
+            )
+        )
+        console.print(Padding(command + "\n", pad=(0, 0, 0, 4)), style="yellow")
+        user_response = ""
+        while user_response.lower() not in ["y", "n"]:
+            user_response = input("  Enter y/n to approve/deny: ")
+        if user_response.lower() == "n":
+            return "User did not approve command execution. You can suggest the command instead."
+
         try:
             console.print(
                 Padding(f":gear: running command: {command}", pad=(0, 0, 0, 2))
             )
             output = subprocess.check_output(command, shell=True).decode("utf-8")
             console.print(Padding(":green_circle: command complete", pad=(0, 0, 0, 2)))
             return output
```

### Comparing `k8sai-0.1.2/k8sAI/main.py` & `k8sai-0.1.3/k8sAI/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 )
 def chat(prompt, terminal, disable_execution):
     """
     Start a conversation with the k8sAI model.
     k8sAI can suggest commands that can then be executed.
     """
     kube_ai = k8sAI(disable_execution)
-    console.print(":robot: starting conversation with k8sAI...")
+    console.print("\n:robot: starting conversation with k8sAI...", style="bold green")
     if not terminal:
-        console.print("Type 'exit' to end the conversation.")
+        console.print("   type 'exit' to end the conversation.", style="italic")
 
     kube_ai.start_chat(prompt, terminal=terminal)
 
 
 @chat_group.command()
 @click.option("--cmd", help="Kubectl command that k8sAI will explain the results of")
 @click.option(
```

### Comparing `k8sai-0.1.2/k8sAI.egg-info/PKG-INFO` & `k8sai-0.1.3/k8sAI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.2
-Summary: A simple example package
+Version: 0.1.3
+Summary: A conversational AI for Kubernetes users.
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: langchain
```

### Comparing `k8sai-0.1.2/k8sAI.egg-info/SOURCES.txt` & `k8sai-0.1.3/k8sAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.2/setup.py` & `k8sai-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="k8sAI",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
-    description="A simple example package",
+    description="A conversational AI for Kubernetes users.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Wilson Spearman",
     author_email="wilsonspearman@gmail.com",
     url="https://github.com/wilson090/k8sAI",
     include_package_data=True,
     install_requires=[
```

