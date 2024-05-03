# Comparing `tmp/r2ai-0.6.1.tar.gz` & `tmp/r2ai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2ai-0.6.1.tar", last modified: Thu Apr 11 14:37:21 2024, max compression
+gzip compressed data, was "r2ai-0.7.0.tar", last modified: Fri May  3 09:20:19 2024, max compression
```

## Comparing `r2ai-0.6.1.tar` & `r2ai-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-11 14:37:21.937710 r2ai-0.6.1/
--rw-r--r--   0 pancake    (501) staff       (20)     4863 2024-04-11 14:37:21.933785 r2ai-0.6.1/PKG-INFO
--rw-r--r--   0 pancake    (501) staff       (20)     4330 2024-03-27 22:26:58.000000 r2ai-0.6.1/README.md
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-11 14:37:21.932430 r2ai-0.6.1/r2ai/
--rw-r--r--   0 pancake    (501) staff       (20)      148 2024-04-11 14:36:44.000000 r2ai-0.6.1/r2ai/__init__.py
--rw-r--r--   0 pancake    (501) staff       (20)     7040 2024-03-12 10:27:41.000000 r2ai-0.6.1/r2ai/anthropic.py
--rw-r--r--   0 pancake    (501) staff       (20)    14444 2024-04-11 14:17:36.000000 r2ai-0.6.1/r2ai/auto.py
--rw-r--r--   0 pancake    (501) staff       (20)     1197 2023-11-09 16:50:46.000000 r2ai-0.6.1/r2ai/bubble.py
--rw-r--r--   0 pancake    (501) staff       (20)     3170 2024-02-28 22:47:42.000000 r2ai-0.6.1/r2ai/code_block.py
--rw-r--r--   0 pancake    (501) staff       (20)      281 2023-11-20 12:54:35.000000 r2ai-0.6.1/r2ai/const.py
--rw-r--r--   0 pancake    (501) staff       (20)    13069 2024-01-23 19:25:53.000000 r2ai-0.6.1/r2ai/index.py
--rw-r--r--   0 pancake    (501) staff       (20)    34635 2024-04-09 23:05:56.000000 r2ai-0.6.1/r2ai/interpreter.py
--rwxr-xr-x   0 pancake    (501) staff       (20)     3205 2024-04-11 14:17:36.000000 r2ai-0.6.1/r2ai/main.py
--rw-r--r--   0 pancake    (501) staff       (20)     1826 2024-02-28 22:47:42.000000 r2ai-0.6.1/r2ai/message_block.py
--rw-r--r--   0 pancake    (501) staff       (20)    20962 2024-04-10 08:10:44.000000 r2ai-0.6.1/r2ai/models.py
--rw-r--r--   0 pancake    (501) staff       (20)    10935 2024-04-11 14:17:36.000000 r2ai-0.6.1/r2ai/repl.py
--rw-r--r--   0 pancake    (501) staff       (20)      942 2024-02-28 22:47:42.000000 r2ai-0.6.1/r2ai/utils.py
--rw-r--r--   0 pancake    (501) staff       (20)     2234 2023-12-11 00:06:37.000000 r2ai-0.6.1/r2ai/voice.py
-drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-11 14:37:21.933570 r2ai-0.6.1/r2ai.egg-info/
--rw-r--r--   0 pancake    (501) staff       (20)     4863 2024-04-11 14:37:21.000000 r2ai-0.6.1/r2ai.egg-info/PKG-INFO
--rw-r--r--   0 pancake    (501) staff       (20)      409 2024-04-11 14:37:21.000000 r2ai-0.6.1/r2ai.egg-info/SOURCES.txt
--rw-r--r--   0 pancake    (501) staff       (20)        1 2024-04-11 14:37:21.000000 r2ai-0.6.1/r2ai.egg-info/dependency_links.txt
--rw-r--r--   0 pancake    (501) staff       (20)       40 2024-04-11 14:37:21.000000 r2ai-0.6.1/r2ai.egg-info/entry_points.txt
--rw-r--r--   0 pancake    (501) staff       (20)      108 2024-04-11 14:37:21.000000 r2ai-0.6.1/r2ai.egg-info/requires.txt
--rw-r--r--   0 pancake    (501) staff       (20)        5 2024-04-11 14:37:21.000000 r2ai-0.6.1/r2ai.egg-info/top_level.txt
--rw-r--r--   0 pancake    (501) staff       (20)       38 2024-04-11 14:37:21.937896 r2ai-0.6.1/setup.cfg
--rw-r--r--   0 pancake    (501) staff       (20)      821 2024-04-11 14:36:32.000000 r2ai-0.6.1/setup.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-03 09:20:19.212585 r2ai-0.7.0/
+-rw-r--r--   0 pancake    (501) staff       (20)     5073 2024-05-03 09:20:19.212323 r2ai-0.7.0/PKG-INFO
+-rw-r--r--   0 pancake    (501) staff       (20)     4540 2024-05-03 00:16:33.000000 r2ai-0.7.0/README.md
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-03 09:20:19.208640 r2ai-0.7.0/r2ai/
+-rw-r--r--   0 pancake    (501) staff       (20)      148 2024-05-03 09:18:41.000000 r2ai-0.7.0/r2ai/__init__.py
+-rw-r--r--   0 pancake    (501) staff       (20)     7040 2024-05-02 23:22:30.000000 r2ai-0.7.0/r2ai/anthropic.py
+-rw-r--r--   0 pancake    (501) staff       (20)    14018 2024-05-02 23:25:00.000000 r2ai-0.7.0/r2ai/auto.py
+-rw-r--r--   0 pancake    (501) staff       (20)     1597 2024-05-03 00:16:33.000000 r2ai-0.7.0/r2ai/bubble.py
+-rw-r--r--   0 pancake    (501) staff       (20)     3820 2024-05-03 00:39:04.000000 r2ai-0.7.0/r2ai/code_block.py
+-rw-r--r--   0 pancake    (501) staff       (20)      367 2024-05-02 23:22:30.000000 r2ai-0.7.0/r2ai/const.py
+-rw-r--r--   0 pancake    (501) staff       (20)    13069 2024-01-23 19:25:53.000000 r2ai-0.7.0/r2ai/index.py
+-rw-r--r--   0 pancake    (501) staff       (20)    35912 2024-05-02 23:22:30.000000 r2ai-0.7.0/r2ai/interpreter.py
+-rwxr-xr-x   0 pancake    (501) staff       (20)     3222 2024-05-02 23:22:30.000000 r2ai-0.7.0/r2ai/main.py
+-rw-r--r--   0 pancake    (501) staff       (20)     1826 2024-02-28 22:47:42.000000 r2ai-0.7.0/r2ai/message_block.py
+-rw-r--r--   0 pancake    (501) staff       (20)    20268 2024-05-03 09:14:50.000000 r2ai-0.7.0/r2ai/models.py
+-rw-r--r--   0 pancake    (501) staff       (20)      500 2024-05-02 23:29:58.000000 r2ai-0.7.0/r2ai/pipe.py
+-rw-r--r--   0 pancake    (501) staff       (20)    12296 2024-05-02 23:29:48.000000 r2ai-0.7.0/r2ai/repl.py
+-rw-r--r--   0 pancake    (501) staff       (20)     4239 2024-05-03 00:34:09.000000 r2ai-0.7.0/r2ai/tab.py
+-rw-r--r--   0 pancake    (501) staff       (20)      942 2024-02-28 22:47:42.000000 r2ai-0.7.0/r2ai/utils.py
+-rw-r--r--   0 pancake    (501) staff       (20)     2236 2024-05-02 23:22:30.000000 r2ai-0.7.0/r2ai/voice.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-05-03 09:20:19.211975 r2ai-0.7.0/r2ai.egg-info/
+-rw-r--r--   0 pancake    (501) staff       (20)     5073 2024-05-03 09:20:19.000000 r2ai-0.7.0/r2ai.egg-info/PKG-INFO
+-rw-r--r--   0 pancake    (501) staff       (20)      434 2024-05-03 09:20:19.000000 r2ai-0.7.0/r2ai.egg-info/SOURCES.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        1 2024-05-03 09:20:19.000000 r2ai-0.7.0/r2ai.egg-info/dependency_links.txt
+-rw-r--r--   0 pancake    (501) staff       (20)       40 2024-05-03 09:20:19.000000 r2ai-0.7.0/r2ai.egg-info/entry_points.txt
+-rw-r--r--   0 pancake    (501) staff       (20)      108 2024-05-03 09:20:19.000000 r2ai-0.7.0/r2ai.egg-info/requires.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        5 2024-05-03 09:20:19.000000 r2ai-0.7.0/r2ai.egg-info/top_level.txt
+-rw-r--r--   0 pancake    (501) staff       (20)       38 2024-05-03 09:20:19.212637 r2ai-0.7.0/setup.cfg
+-rw-r--r--   0 pancake    (501) staff       (20)      902 2024-05-03 00:16:33.000000 r2ai-0.7.0/setup.py
```

### Comparing `r2ai-0.6.1/PKG-INFO` & `r2ai-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2ai
-Version: 0.6.1
+Version: 0.7.0
 Summary: Applying language models on radare2 for reverse engineering and fun purposes
 Home-page: https://www.radare.org/
 Author: pancake
 Author-email: pancake@nopcode.org
 Description-Content-Type: text/markdown
 Requires-Dist: rich
 Requires-Dist: r2pipe
@@ -24,14 +24,16 @@
 |  \____|/  ____||  _,_  || : |
 |   :  \ \   .  ||   :   ||   |
 |   |___\ \__:__||___|   ||   |
 |___|        :       |___||___|
              *       --pancake
 ```
 
+[![ci](https://github.com/radareorg/r2ai/actions/workflows/ci.yml/badge.svg)](https://github.com/radareorg/r2ai/actions/workflows/ci.yml)
+
 Run a language model in local, without internet, to entertain you or help answering questions about radare2 or reverse engineering in general. Note that models used by r2ai are pulled from external sources which may behave different or respond unrealible information. That's why there's an ongoing effort into improving the post-finetuning using memgpt-like techniques which can't get better without your help!
 
 <p align="center">
   <img src="doc/r2clippy.jpg">
 </p>
 
 ## Features
@@ -102,14 +104,15 @@
 
 ## Usage
 
 There are 4 different ways to run `r2ai`:
 
 * Standalone and interactive: `r2pm -r r2ai` or `python main.py`
 * Batch mode: `r2ai '-r act as a calculator' '3+3=?'`
+* As an r2 plugin: `r2 -i main.py /bin/ls`
 * From radare2 (requires `r2pm -ci rlang-python`): `r2 -c 'r2ai -h'`
 * Using r2pipe: `#!pipe python main.py`
   * Define a macro command: `'$r2ai=#!pipe python main.py`
 
 ## Auto mode
 
 When using OpenAI, Claude or any of the Functionary local models you can use the auto mode which permits the language model to execute r2 commands, analyze the output in loop and in a loop until it is resolved. Here's a sample session to achieve that:
@@ -122,26 +125,26 @@
 [0x00000000]> '$r2ai=#!pipe python main.py
 [0x00000000]> $r2ai '-m openai:gpt-4'
 [0x00000000]> $r2ai "' list the imports for this program"
 [0x00000000]> $r2ai "' draw me a donut"
 [0x00000000]> $r2ai "' decompile current function and explain it"
 ```
 
-
 ## Examples
 
 You can interact with r2ai from standalone python, from r2pipe via r2 keeping a global state or using the javascript intrepreter embedded inside `radare2`.
 
 * [conversation.r2.js](examples/conversation.r2.js) - load two models and make them talk to each other
 
 ### Development/Testing
 
 Just run `make` .. or well `python main.py`
 
 ### TODO
 
 * add "undo" command to drop the last message
 * dump / restore conversational states (see -L command)
+* Implement `~`, `|` and `>`
 
 ### Kudos
 
 The original code of r2ai is based on OpenInterpreter. I want to thanks all the contributors to this project as they made it possible to build r2ai taking their code as source for this.  Kudos to Killian and all the contributors.
```

### Comparing `r2ai-0.6.1/README.md` & `r2ai-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 |  \____|/  ____||  _,_  || : |
 |   :  \ \   .  ||   :   ||   |
 |   |___\ \__:__||___|   ||   |
 |___|        :       |___||___|
              *       --pancake
 ```
 
+[![ci](https://github.com/radareorg/r2ai/actions/workflows/ci.yml/badge.svg)](https://github.com/radareorg/r2ai/actions/workflows/ci.yml)
+
 Run a language model in local, without internet, to entertain you or help answering questions about radare2 or reverse engineering in general. Note that models used by r2ai are pulled from external sources which may behave different or respond unrealible information. That's why there's an ongoing effort into improving the post-finetuning using memgpt-like techniques which can't get better without your help!
 
 <p align="center">
   <img src="doc/r2clippy.jpg">
 </p>
 
 ## Features
@@ -82,14 +84,15 @@
 
 ## Usage
 
 There are 4 different ways to run `r2ai`:
 
 * Standalone and interactive: `r2pm -r r2ai` or `python main.py`
 * Batch mode: `r2ai '-r act as a calculator' '3+3=?'`
+* As an r2 plugin: `r2 -i main.py /bin/ls`
 * From radare2 (requires `r2pm -ci rlang-python`): `r2 -c 'r2ai -h'`
 * Using r2pipe: `#!pipe python main.py`
   * Define a macro command: `'$r2ai=#!pipe python main.py`
 
 ## Auto mode
 
 When using OpenAI, Claude or any of the Functionary local models you can use the auto mode which permits the language model to execute r2 commands, analyze the output in loop and in a loop until it is resolved. Here's a sample session to achieve that:
@@ -102,26 +105,26 @@
 [0x00000000]> '$r2ai=#!pipe python main.py
 [0x00000000]> $r2ai '-m openai:gpt-4'
 [0x00000000]> $r2ai "' list the imports for this program"
 [0x00000000]> $r2ai "' draw me a donut"
 [0x00000000]> $r2ai "' decompile current function and explain it"
 ```
 
-
 ## Examples
 
 You can interact with r2ai from standalone python, from r2pipe via r2 keeping a global state or using the javascript intrepreter embedded inside `radare2`.
 
 * [conversation.r2.js](examples/conversation.r2.js) - load two models and make them talk to each other
 
 ### Development/Testing
 
 Just run `make` .. or well `python main.py`
 
 ### TODO
 
 * add "undo" command to drop the last message
 * dump / restore conversational states (see -L command)
+* Implement `~`, `|` and `>`
 
 ### Kudos
 
 The original code of r2ai is based on OpenInterpreter. I want to thanks all the contributors to this project as they made it possible to build r2ai taking their code as source for this.  Kudos to Killian and all the contributors.
```

### Comparing `r2ai-0.6.1/r2ai/anthropic.py` & `r2ai-0.7.0/r2ai/anthropic.py`

 * *Files identical despite different names*

### Comparing `r2ai-0.6.1/r2ai/auto.py` & `r2ai-0.7.0/r2ai/auto.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,35 +9,15 @@
 from .anthropic import construct_tool_use_system_prompt, extract_claude_tool_calls
 
 import os
 file_dir = os.path.dirname(__file__)
 sys.path.append(file_dir)
 import index
 
-r2lang = None
-try:
-  import r2lang
-  have_rlang = True
-except:
-  try:
-    import r2pipe
-    class FakeLang:
-      def __init__(self, r2):
-        self.r2 = r2
-      def cmd(self,x):
-        return self.r2.cmd(x)
-    try:
-      r2lang = FakeLang(r2pipe.open())
-      r2lang.cmd("?V") # r2pipe throws only here
-    except:
-      r2lang = FakeLang(r2pipe.open("/bin/ls"))
-      pass
-  except:
-    print("Cannot instantiate this FakeLang class with r2pipe")
-    pass
+from .pipe import have_rlang, r2lang
 
 ANSI_REGEX = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
 
 tools = [{
   "type": "function",
   "function": {
     "name": "r2cmd",
```

### Comparing `r2ai-0.6.1/r2ai/code_block.py` & `r2ai-0.7.0/r2ai/code_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,101 +1,104 @@
+"""Module providing a class to display code snippets"""
+
 import re
 from rich.live import Live
 from rich.panel import Panel
 from rich.box import MINIMAL
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.console import Group
 from rich.console import Console
 
 
 class CodeBlock:
-  """
-  Code Blocks display code and outputs in different languages.
-  """
-
-  def __init__(self):
-    # Define these for IDE auto-completion
-    self.language = ""
-    self.output = ""
-    self.code = ""
-    self.active_line = None
-    self.live = Live(auto_refresh=False, console=Console(), vertical_overflow="visible")
-#    self.live = Live(auto_refresh=False, console=Console())
-    self.live.start()
-
-  def update_from_message(self, message):
-    if "content" in message:
-      message = message["content"]
-    if type(message) is str:
-      lang = "python"
-      pos = message.find("```")
-      if pos != -1:
-        pre = message[0:pos]
-        cod = message[pos:]
-        lines = cod.split("\n")
-        lang = lines[0][3:]
-        message = "\n".join(lines[1:]).replace("```", "")
-      message = re.sub(r"`+$", '', message)
-      self.language = lang
-      self.code = message
-    elif "function_call" in message and "parsed_arguments" in message["function_call"]:
-      # never happens
-      parsed_arguments = message["function_call"]["parsed_arguments"]
-      if parsed_arguments is not None:
-        self.language = parsed_arguments.get("language")
-        self.code = parsed_arguments.get("code")
-    self.refresh()
-
-  def end(self):
-    self.refresh(cursor=False)
-    # Destroys live display
-    self.live.stop()
-    self.output = ""
-    self.code = ""
-    self.active_line = None
-
-  def refresh(self, cursor=True):
-    # Get code, return if there is none
-    code = self.code
-    if not code:
-      return
-    
-    # Create a table for the code
-    code_table = Table(show_header=False,
-                       show_footer=False,
-                       box=None,
-                       padding=0,
-                       expand=True)
-    code_table.add_column()
-
-    # Add cursor    
-    if cursor:
-      code += "█"
-
-    # Add each line of code to the table
-    code_lines = code.strip().split('\n')
-    for i, line in enumerate(code_lines, start=1):
-      if i == self.active_line:
-        # This is the active line, print it with a white background
-        syntax = Syntax(line, self.language, theme="bw", line_numbers=False, word_wrap=True)
-        code_table.add_row(syntax, style="black on white")
-      else:
-        # This is not the active line, print it normally
-        syntax = Syntax(line, self.language, theme="monokai", line_numbers=False, word_wrap=True)
-        code_table.add_row(syntax)
-
-    # Create a panel for the code
-    code_panel = Panel(code_table, box=MINIMAL, style="on #272727")
-
-    # Create a panel for the output (if there is any)
-    if self.output == "" or self.output == "None":
-      output_panel = ""
-    else:
-      output_panel = Panel(self.output, box=MINIMAL, style="#FFFFFF on #3b3b37")
-
-    # Create a group with the code table and output panel
-    group = Group(code_panel, output_panel)
-
-    # Update the live display
-    self.live.update(group)
-    self.live.refresh()
+    """
+    Code Blocks display code and outputs in different languages.
+    """
+
+    def __init__(self):
+        # Define these for IDE auto-completion
+        self.language = ""
+        self.output = ""
+        self.code = ""
+        self.active_line = None
+        self.live = Live(auto_refresh=False, console=Console(), vertical_overflow="visible")
+        # self.live = Live(auto_refresh=False, console=Console())
+        self.live.start()
+
+    def update_from_message(self, message):
+        """Update code block contents with given text
+        """
+        if "content" in message:
+            message = message["content"]
+        if isinstance(message, str):
+            lang = "python"
+            pos = message.find("```")
+            if pos != -1:
+                # pre = message[0:pos]
+                cod = message[pos:]
+                lines = cod.split("\n")
+                lang = lines[0][3:]
+                message = "\n".join(lines[1:]).replace("```", "")
+            message = re.sub(r"`+$", '', message)
+            self.language = lang
+            self.code = message
+        elif "function_call" in message and "parsed_arguments" in message["function_call"]:
+            # never happens
+            parsed_arguments = message["function_call"]["parsed_arguments"]
+            if parsed_arguments is not None:
+                self.language = parsed_arguments.get("language")
+                self.code = parsed_arguments.get("code")
+        self.refresh()
+
+    def end(self):
+        """Close the codeblock
+        """
+        self.refresh(cursor=False)
+        # Destroys live display
+        self.live.stop()
+        self.output = ""
+        self.code = ""
+        self.active_line = None
+
+    def refresh(self, cursor=True):
+        """Display this code on the terminal
+        """
+        # Get code, return if there is none
+        code = self.code
+        if not code:
+            return
+        # Create a table for the code
+        code_table = Table(show_header=False,
+                           show_footer=False,
+                           box=None,
+                           padding=0,
+                           expand=True)
+        code_table.add_column()
+        # Add cursor
+        if cursor:
+            code += "█"
+        # Add each line of code to the table
+        code_lines = code.strip().split('\n')
+        for i, line in enumerate(code_lines, start=1):
+            if i == self.active_line:
+                # This is the active line, print it with a white background
+                syntax = Syntax(line, self.language, theme="bw",
+                                line_numbers=False, word_wrap=True)
+                code_table.add_row(syntax, style="black on white")
+            else:
+                # This is not the active line, print it normally
+                syntax = Syntax(line, self.language, theme="monokai",
+                                line_numbers=False, word_wrap=True)
+                code_table.add_row(syntax)
+        # Create a panel for the code
+        code_panel = Panel(code_table, box=MINIMAL, style="on #272727")
+        # Create a panel for the output (if there is any)
+        if self.output in ["", "None"]:
+            output_panel = ""
+        else:
+            output_panel = Panel(self.output, box=MINIMAL, style="#FFFFFF on #3b3b37")
+        # Create a group with the code table and output panel
+        group = Group(code_panel, output_panel)
+        # Update the live display
+        self.live.update(group)
+        self.live.refresh()
```

### Comparing `r2ai-0.6.1/r2ai/index.py` & `r2ai-0.7.0/r2ai/index.py`

 * *Files identical despite different names*

### Comparing `r2ai-0.6.1/r2ai/interpreter.py` & `r2ai-0.7.0/r2ai/interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
 Ginterrupted = False
 def signal_handler(sig, frame):
 	global Ginterrupted
 	if Ginterrupted:
 	    sys.exit(0) # throws exception
 	Ginterrupted = True
-	print("^C")
+	print("^C", file=sys.stderr)
 signal(SIGINT, signal_handler)
 
 def exception_handler(self, sig, frame):
 	global Ginterrupted
 	if Ginterrupted:
 	    sys.exit(0) # throws exception
 	Ginterrupted = True
-	print("^C")
+	print("^C", file=sys.stderr)
 sys.excepthook = exception_handler
 
 def incodeblock(msg):
   return "content" in msg and msg["content"].count("```") % 2 == 1
 
 def r2eval(m):
   if "$(" in m and have_rlang:
@@ -121,18 +121,20 @@
   elif "falcon" in lowermodel:
     formatted_messages = template_falcon(self, messages)
   elif "utopia" in lowermodel:
     formatted_messages = template_alpaca(self, messages)
   elif "mistral" in lowermodel:
     formatted_messages = template_mistral(self, messages)
   elif "python" in lowermodel:
-    print("codellama-python model is not working well yet")
+    print("codellama-python model is not working well yet", file=sys.stderr)
     formatted_messages = template_llamapython(self, messages)
   elif "tinyllama" in lowermodel:
     formatted_messages = template_tinyllama(self, messages)
+  elif "llama-3" in lowermodel:
+    formatted_messages = template_llama3(self, messages)
   else:
     formatted_messages = template_llama(self, messages)
 
   if self.env["debug"] == "true":
     builtins.print(formatted_messages)
   return formatted_messages
 
@@ -433,14 +435,40 @@
       if role == 'user':
           formatted_messages += f"### User: {content}\n"
       elif self.env["chat.reply"] == "true":
           formatted_messages += f"### System: {content}\n"
   formatted_messages += f"### System: "
   return formatted_messages
 
+def template_llama3(self,messages):
+  formatted_messages = f"<|begin_of_text|>"
+  if self.system_message != "":
+      formatted_messages += f"<|start_header_id|>{self.system_message}<|end_header_id|>"
+  self.terminator = "<|end_header_id|>"
+  self.terminator = "<|eot_id|>"
+  self.terminator = "assistant"
+  for index, item in enumerate(messages):
+      if "role" in item:
+          role = item['role']
+      else:
+          role = 'user'
+      if "content" not in item:
+          continue
+      content = item['content']
+      if role == 'user':
+          formatted_messages += f"{content}<|eot_id|>"
+      elif role == 'hint':
+          formatted_messages += f"Hint: {content}<|eot_id|> "
+      elif role == 'function':
+          formatted_messages += f"Output: {content}<|eot_id|> "
+      elif role == 'assistant' and self.env["chat.reply"] == "true":
+          formatted_messages += f"{content}<|eot_id|>"
+  formatted_messages += f"<|start_header_id|>assistant<|end_header_id|>"
+  return formatted_messages
+
 def template_llama(self,messages):
   formatted_messages = f"<s>[INST]"
   if self.system_message != "":
       formatted_messages += f"<<SYS>>{self.system_message}<</SYS>>"
   self.terminator = "</s>"
   for index, item in enumerate(messages):
       if "role" in item:
@@ -482,14 +510,15 @@
     self.env["llm.maxtokens"] = "4096" # "1750"
     self.env["llm.maxmsglen"] = "8096" # "1750"
     self.env["llm.temperature"] = "0.002"
     self.env["user.name"] = "" # TODO auto fill?
     self.env["user.os"] = ""
     self.env["user.arch"] = ""
     self.env["user.cwd"] = ""
+    self.env["user.plugins"] = f"{R2AI_HOMEDIR}/plugins"
     self.env["voice.lang"] = "en"
     self.env["voice.model"] = "base"
     self.env["data.use"] = "false"
     self.env["data.path"] = f"{R2AI_HOMEDIR}/doc/data"
     self.env["data.local"] = "false"
     self.env["data.wikit"] = "false"
     self.env["data.mastodon"] = "false"
@@ -841,16 +870,16 @@
         if "content" in self.messages[-1]:
           last_message = self.messages[-1]["content"]
         if self.env["chat.reply"] == "true":
           self.messages.append({"role": "assistant", "content": response})
         print(response)
         return
       else:
-        print("pip install -U openai")
-        print("export OPENAI_API_KEY=...")
+        print("pip install -U openai", file=sys.stderr)
+        print("export OPENAI_API_KEY=...", file=sys.stderr)
         return
     elif self.model.startswith('anthropic:'):
       anthropic_model = self.model[10:]
       messages = []
       for m in self.messages:
         if m["role"] == "system":
           system_message = m["content"]
@@ -867,16 +896,16 @@
           messages=messages
         )
 
         if self.env["chat.reply"] == "true":
           self.messages.append({"role": "assistant", "content": completion.content})
           print(completion.content)
       else:
-        print("pip install -U anthropic")
-        print("export ANTHROPIC_API_KEY=...")
+        print("pip install -U anthropic", file=sys.stderr)
+        print("export ANTHROPIC_API_KEY=...", file=sys.stderr)
         return
     elif self.model.startswith('groq:'):
       if have_groq:
         self.groq_client = Groq()
         completion = self.groq_client.completions.create(
           model=self.model[5:],
           max_tokens=maxtokens,
```

### Comparing `r2ai-0.6.1/r2ai/main.py` & `r2ai-0.7.0/r2ai/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 OPENAI_KEY = ""
 try:
 	if "HOME" in os.environ:
 		from r2ai.utils import slurp
 		apikey = slurp(os.environ["HOME"] + "/.r2ai.openai-key").strip()
 		os.environ["OPENAI_API_KEY"] = apikey
-		print("[R2AI] OpenAI key loaded from ~/.r2ai.openai-key")
+		print("[R2AI] OpenAI key loaded from ~/.r2ai.openai-key", file=sys.stderr)
 except:
 	pass
 
 r2 = None
 r2_file = None
 have_rlang = False
 have_r2pipe = False
```

### Comparing `r2ai-0.6.1/r2ai/message_block.py` & `r2ai-0.7.0/r2ai/message_block.py`

 * *Files identical despite different names*

### Comparing `r2ai-0.6.1/r2ai/models.py` & `r2ai-0.7.0/r2ai/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 import llama_cpp
 import os
 import shutil
 import subprocess
 import sys
 import traceback
 
-#DEFAULT_MODEL = "TheBloke/CodeLlama-34B-Instruct-GGUF"
+# DEFAULT_MODEL = "TheBloke/CodeLlama-34B-Instruct-GGUF"
 # DEFAULT_MODEL = "TheBloke/llama2-7b-chat-codeCherryPop-qLoRA-GGUF"
-DEFAULT_MODEL = "-m TheBloke/dolphin-2_6-phi-2-GGUF"
+# DEFAULT_MODEL = "-m TheBloke/dolphin-2_6-phi-2-GGUF"
+DEFAULT_MODEL = "-m FaradayDotDev/llama-3-8b-Instruct-GGUF"
 r2ai_model_json = "r2ai.model.json" # windows path
 if "HOME" in os.environ:
 	r2ai_model_json = os.environ["HOME"] + "/.r2ai.model"
 
 def get_default_model():
     try:
         fd = open(r2ai_model_json)
@@ -87,14 +88,15 @@
 -m dagbs/dolphin-2.8-mistral-7b-v02-GGUF
 -m TheBloke/zephyr-7B-alpha-GGUF
 -m TheBloke/OpenOrca-Zephyr-7B-GGUF
 -m TheBloke/zephyr-7B-beta-GGUF
 -m maddes8cht/nomic-ai-gpt4all-falcon-7b-gguf
 -m KoboldAI/LLaMA2-13B-Tiefighter-GGUF
 Coding:
+-m FaradayDotDev/llama-3-8b-Instruct-GGUF
 -m bartowski/stable-code-instruct-3b-GGUF
 -m TheBloke/CodeBooga-34B-v0.1-GGUF
 -m TheBloke/llama2-7b-chat-codeCherryPop-qLoRA-GGUF
 -m TheBloke/deepseek-coder-6.7B-instruct-GGUF
 -m TheBloke/deepseek-coder-33B-instruct-GGUF
 -m TheBloke/CodeLlama-7B-Instruct-GGUF
 -m TheBloke/CodeLlama-34B-Instruct-GGUF
@@ -128,18 +130,18 @@
             repo_id = get_default_model()
         if usermodels is not None and repo_id in usermodels:
             model_path = usermodels[repo_id]
 #            print(f"[r2ai] Using {r2ai_model_json} {model_path}")
             return llama_cpp.Llama(model_path=model_path, n_gpu_layers=n_gpu_layers, verbose=debug_mode, n_ctx=context_window)
     except:
         traceback.print_exc()
-    print(f"Select {repo_id} model. See -M and -m flags")
+    print(f"Select {repo_id} model. See -M and -m flags", file=sys.stderr)
     raw_models = list_gguf_files(repo_id)
     if not raw_models:
-        print(f"Failed. Are you sure there are GGUF files in `{repo_id}`?")
+        print(f"Failed. Are you sure there are GGUF files in `{repo_id}`?", file=sys.stderr)
         return None
 #    print(raw_models)
     combined_models = group_and_combine_splits(raw_models)
     selected_model = None #"Medium"
 
     # First we give them a simple small medium large option. If they want to see more, they can.
     if selected_model is None and len(combined_models) > 3:
@@ -214,15 +216,15 @@
         if confirm_action(f"Download to {default_path}?"):
             for model_details in combined_models:
                 if model_details["filename"] == selected_model:
                     selected_model_details = model_details
 
                     # Check disk space and exit if not enough
                     if not enough_disk_space(selected_model_details['Size'], default_path):
-                        print(f"Not enough disk space available to download this model.")
+                        print(f"Not enough disk space available to download this model.", file=sys.stderr)
                         return None
 
             # Check if model was originally split
             split_files = [model["filename"] for model in raw_models if selected_model in model["filename"]]
             
             if len(split_files) > 1:
                 # Download splits
@@ -248,15 +250,15 @@
                     local_dir=default_path,
                     local_dir_use_symlinks=False,
                     resume_download=True)
 
             model_path = download_path
         
         else:
-            print('\n', "Download cancelled. Exiting.", '\n')
+            print('\nDownload cancelled. Exiting\n', file=sys.stderr)
             return None
     try:
         from llama_cpp import Llama
     except:
         if debug_mode:
             traceback.print_exc()
         # Ask for confirmation to install the required pip package
@@ -288,15 +290,15 @@
                     env_vars["CMAKE_ARGS"] = "-DLLAMA_METAL=on"
                 else:  # Default to OpenBLAS
                     env_vars["CMAKE_ARGS"] = "-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS"
                 
                 try:
                     subprocess.run([sys.executable, "-m", "pip", "install", "llama-cpp-python"], env={**os.environ, **env_vars}, check=True)
                 except subprocess.CalledProcessError as e:
-                    print(f"Error during installation with {backend}: {e}")
+                    print(f"Error during installation with {backend}: {e}", file=sys.stderr)
             
             def supports_metal():
                 # Check for macOS version
                 if platform.system() == "Darwin":
                     mac_version = tuple(map(int, platform.mac_ver()[0].split('.')))
                     # Metal requires macOS 10.11 or later
                     if mac_version >= (10, 11):
@@ -315,15 +317,15 @@
           
             print('', Markdown("Finished downloading `Code-Llama` interface."), '')
 
             # Check if on macOS
             if platform.system() == "Darwin":
                 # Check if it's Apple Silicon
                 if platform.machine() != "arm64":
-                    print("Warning: Running python-x86 on arm64, which is 10x slower than native m1")
+                    print("Warning: Running python-x86 on arm64, which is 10x slower than native m1", file=sys.stderr)
         else:
             print('', "Installation cancelled. Exiting.", '')
             return None
 
     set_default_model(repo_id)
     # Initialize and return Code-Llama
     assert os.path.isfile(model_path)
@@ -514,15 +516,15 @@
                     env_vars["CMAKE_ARGS"] = "-DLLAMA_METAL=on"
                 else:  # Default to OpenBLAS
                     env_vars["CMAKE_ARGS"] = "-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS"
                 
                 try:
                     subprocess.run([sys.executable, "-m", "pip", "install", "llama-cpp-python"], env={**os.environ, **env_vars}, check=True)
                 except subprocess.CalledProcessError as e:
-                    print(f"Error during installation with {backend}: {e}")
+                    print(f"Error during installation with {backend}: {e}", file=sys.stderr)
             
             def supports_metal():
                 # Check for macOS version
                 if platform.system() == "Darwin":
                     mac_version = tuple(map(int, platform.mac_ver()[0].split('.')))
                     # Metal requires macOS 10.11 or later
                     if mac_version >= (10, 11):
@@ -534,33 +536,16 @@
                 install_llama("cuBLAS")
             elif check_command(["rocminfo"]):
                 install_llama("hipBLAS")
             elif supports_metal():
                 install_llama("Metal")
             else:
                 install_llama("OpenBLAS")
-          
             print('', Markdown("Finished downloading `Code-Llama` interface."), '')
-
-            # Tell them if their architecture won't work well
-
-            # Check if on macOS
-            if platform.system() == "Darwin":
-                # Check if it's Apple Silicon
-                if platform.machine() != "arm64":
-                    print("Warning: You are using Apple Silicon (M1/M2) Mac but your Python is not of 'arm64' architecture.")
-                    print("The llama.ccp x86 version will be 10x slower on Apple Silicon (M1/M2) Mac.")
-                    print("\nTo install the correct version of Python that supports 'arm64' architecture:")
-                    print("1. Download Miniforge for M1/M2:")
-                    print("wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh")
-                    print("2. Install it:")
-                    print("bash Miniforge3-MacOSX-arm64.sh")
-                    print("")
-      
         else:
-            print('', "Installation cancelled. Exiting.", '')
+            print("Installation cancelled. Exiting.", file=sys.stderr)
             return None
 
     # Initialize and return Code-Llama
     if not os.path.isfile(model_path):
         print("Model is not a file")
     return llama_cpp.Llama(model_path=model_path, n_gpu_layers=n_gpu_layers, verbose=debug_mode, n_ctx=context_window)
```

### Comparing `r2ai-0.6.1/r2ai/repl.py` & `r2ai-0.7.0/r2ai/repl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,30 @@
 import builtins
 from r2ai.models import set_default_model
 from .utils import slurp
 import traceback
 have_readline = False
-from .const import R2AI_HISTFILE, R2AI_HOMEDIR, R2AI_RCFILE
+from .const import R2AI_HISTFILE, R2AI_HOMEDIR, R2AI_RCFILE, R2AI_USERDIR
 import r2ai
 import sys
 import os
 
-try:
-  import readline
-  readline.read_history_file(R2AI_HISTFILE)
-  have_readline = True
-except:
-  pass #readline not available
+from .tab import tab_init, tab_hist, tab_write, tab_evals
+
+tab_init()
 
 print_buffer = ""
-r2 = None
 ais = {}
 autoai = None
-have_rlang = False
-try:
-  import r2lang
-  have_rlang = True
-except:
-  try:
-    import r2pipe
-    class FakeLang:
-      def __init__(self, r):
-        global r2
-        self.r2 = r
-        r2 = r
-      def cmd(self, x):
-        return self.r2.cmd(x)
-    try:
-      r2lang = FakeLang(r2pipe.open())
-      r2lang.cmd("?V") # r2pipe throws only here
-    except:
-      r2lang = FakeLang(r2pipe.open("/bin/ls"))
-      pass
-  except:
-    print("Cannot find r2lang or r2pipe")
-    pass
+from .pipe import have_rlang, r2lang, r2singleton
+r2 = r2singleton()
 
 def r2_cmd(x):
-  have_rlang=True
-  global ai, r2, r2_file
+  global have_rlang, ai, r2, r2_file
+  have_rlang = True
   res = x
   if have_rlang:
     oc = r2lang.cmd('e scr.color').strip()
     r2lang.cmd('e scr.color=0')
     res = r2lang.cmd(x)
     r2lang.cmd('e scr.color=' + oc)
   elif r2 is not None:
@@ -90,27 +65,28 @@
   Handler.protocol_version = "HTTP/1.0"
   server = socketserver.TCPServer(("", PORT), SimpleHTTPRequestHandler)
   server.allow_reuse_address = True
   server.allow_reuse_port = True
   print("Serving at port", PORT)
   server.serve_forever()
 
-
 help_message = """Usage: r2ai [-option] ([query] | [script.py])
  r2ai . [file]          interpret r2ai script with access to globals
+ r2ai ..([script])      list or run r2ai user script
  r2ai :aa               run a r2 command
  r2ai ' [prompt]        auto mode; query LLM that can interact with r2
  r2ai !ls               run a system command
  r2ai -a                query with audio voice
  r2ai -A                enter the voice chat loop
  r2ai -k                clear the screen
  r2ai -c [cmd] [query]  run the given r2 command with the given query
  r2ai -e [k[=v]]        set environment variable
  r2ai -f [file]         load file and paste the output
  r2ai -h                show this help (same as ?)
+ r2ai -H ([var])        show path variables like it's done in r2 -H
  r2ai -i [file] ([q])   load the file contents and prompt it with the given optional query
  r2ai -m [file/repo]    select model from huggingface repository or local file
  r2ai -M                list supported and most common models from hf
  r2ai -MM               shorter list of models
  r2ai -n [num]          select the nth language model
  r2ai -q                quit/exit/^C
  r2ai -L                show chat logs (See -Lj for json)
@@ -119,15 +95,14 @@
  r2ai -r2               enter the r2clippy assistant mode
  r2ai -rf [doc/role/.f] load contents of a file to define the role
  r2ai -R                reset the chat conversation context
  r2ai -t [temp]         from 0.0001 to 10 your scale to randomness in my replies
  r2ai -v                show r2ai version (same as ?V)
  r2ai -w                toggle including LLM responses into the query (False is faster)"""
 
-
 def myprint(msg):
   global print_buffer
   builtins.print(msg)
   print_buffer += msg
 
 def runline2(usertext):
   global ai
@@ -139,29 +114,73 @@
   print = myprint
   runline(ai, usertext)
   ai.env["chat.live"] = chat_live
   res = print_buffer
   print_buffer = ""
   return f"{res}\n"
 
+def runplugin(ai, arg):
+  r2ai_plugdir = ai.env["user.plugins"]
+  if arg != "":
+    for plugdir in [R2AI_USERDIR, r2ai_plugdir]:
+      script_path = f"{plugdir}/{arg}.py"
+      if os.path.isfile(script_path):
+        runline(ai, f". {script_path}")
+        return
+    print("Script not found", file=sys.stderr)
+    return
+  try:
+    # print("-e user.plugins = " + r2ai_plugdir)
+    for plugdir in [R2AI_USERDIR, r2ai_plugdir]:
+      files = os.listdir(plugdir)
+      for file in files:
+        if file.endswith(".py"):
+          print(file.replace(".py", ""))
+  except:
+    pass
 
 def r2ai_version():
   import sys
   import llama_cpp
   print("python: " + sys.version)
   print("llama: " + llama_cpp.__version__)
   print("r2ai: " + r2ai.VERSION)
 
+def r2ai_vars(ai, arg):
+  vs = {
+    "R2AI_USERDIR": R2AI_USERDIR,
+    "R2AI_PLUGDIR": ai.env["user.plugins"],
+    "R2AI_HOMEDIR": R2AI_HOMEDIR,
+    "R2AI_RCFILE": R2AI_RCFILE,
+    "R2AI_HISTFILE": R2AI_HISTFILE
+  }
+  if arg != "":
+    if arg in vs.keys():
+      print(vs[arg])
+    else:
+      print("Unknown key", file=sys.stderr)
+  else:
+    for k in vs.keys():
+      print(k)
+
 def runline(ai, usertext):
-#  builtins.print(f"runline {usertext}")
   global print
   global autoai
+  if ai == None:
+    ai = ais[0];
   usertext = usertext.strip()
   if usertext == "" or usertext.startswith("#"):
     return
+  if usertext == "q":
+    return "q"
+  if usertext.startswith("-H"):
+    try:
+      return r2ai_vars(ai, usertext[2:].strip())
+    except:
+      traceback.print_exc()
   if usertext.startswith("?V") or usertext.startswith("-v"):
     print(r2ai.VERSION)
     r2ai_version()
   elif usertext.startswith("?") or usertext.startswith("-h"):
     print(help_message)
   elif usertext.startswith("clear") or usertext.startswith("-k"):
     print("\x1b[2J\x1b[0;0H\r")
@@ -205,54 +224,63 @@
     print(usertext)
     ai.chat(usertext)
     ai.env["chat.live"] = old_live
     ai.env["chat.voice"] = "false"
   elif usertext == "-q" or usertext == "exit":
     return "q"
   elif usertext == "-repl":
-    print("Nothing to do")
+    if have_rlang:
+      r2ai_repl(ai)
+    else:
+      print("r2ai -repl # only works when running as an radare2 plugin")
   elif usertext == "-r2":
     ai.env["data.use"] = "true"
     ai.env["data.hist"] = "true"
     ai.env["data.path"] = f"{R2AI_HOMEDIR}/doc/"
     ai.env["chat.bubble"] = "true"
     runline(ai, f"-rf {R2AI_HOMEDIR}/doc/role/r2clippy.txt")
   elif usertext.startswith("-e"):
     if len(usertext) == 2:
       for k in ai.env.keys():
         v = ai.env[k]
         print(f"-e {k}={v}")
+    elif usertext.endswith("."):
+      kp = usertext[2:].strip()
+      for k in ai.env.keys():
+        if k.startswith(kp):
+          v = ai.env[k]
+          print(f"-e {k}={v}")
     else:
       line = usertext[2:].strip().split("=")
       k = line[0]
       if len(line) > 1:
         v = line[1]
         if v == "":
           ai.env[k] = ""
         elif k in ai.env:
           ai.env[k] = v
         else:
-          print("Invalid config key")
+          print("Invalid config key", file=sys.stderr)
       else:
         try:
           print(ai.env[k])
         except:
-          print("Invalid config key")
+          print("Invalid config key", file=sys.stderr)
           pass
   elif usertext.startswith("-w"):
     start_http_server()
   elif usertext.startswith("-s"):
     r2ai_repl(ai)
   elif usertext.startswith("-rf"):
     if len(usertext) > 2:
       fname = usertext[3:].strip()
       try:
         ai.system_message = slurp(fname)
       except:
-        print(f"Cannot open file {fname}")
+        print(f"Cannot open file {fname}", file=sys.stderr)
     else:
       print(ai.system_message)
   elif usertext.startswith("-r"):
     if len(usertext) > 2:
       ai.system_message = usertext[2:].strip()
     else:
       print(ai.system_message)
@@ -278,15 +306,14 @@
       # tag = "CODE" # INPUT , TEXT, ..
       # r2ai.chat("Q: " + que + ":\n["+tag+"]\n"+ res+"\n[/"+tag+"]\n")
       ai.chat(f"{que}:\n```\n{res}\n```\n")
     else:
       que = input("[Query]> ")
       ai.chat(res)
   elif usertext.startswith("-n"):
-    global ais
     if len(ais.keys()) == 0:
       ais[0] = ai
     if usertext == "-n":
       for a in ais.keys():
         model = ais[a].model
         print(f"{a}  - {model}")
     else:
@@ -294,51 +321,61 @@
       if index not in ais:
         ais[index] = r2ai.Interpreter()
         ais[index].model = ai.model
       ai = ais[index]
   elif usertext.startswith("-c"):
     words = usertext[2:].strip().split(" ", 1)
     res = r2_cmd(words[0])
-    if len(words) > 1:
-      que = words[1]
-    else:
-      que = input("[Query]> ")
+    que = ""
+    try:
+      if len(words) > 1:
+        que = words[1]
+      else:
+        que = input("[Query]> ")
+    except:
+      print("")
+      return
     tag = "```\n" # TEXT, INPUT ..
     ai.chat(f"{que}:\n{tag}\n{res}\n{tag}\n")
   elif usertext[0] == "!":
     os.system(usertext[1:])
   elif usertext[0] == ".":
+    if len(usertext) > 1 and usertext[1] == ".": # ".." - run user plugins
+      runplugin(ai, usertext[2:].strip())
+      return
     try:
       filename = usertext[1:].strip()
       file = slurp(filename)
       if filename.endswith(".py"):
         exec(file, globals())
       else:
         for line in file.split("\n"):
           runline(ai, line)
-    except:
-      traceback.print_exc()
+    except Exception as e:
+      # traceback.print_exc()
+      print(e)
       pass
   elif usertext.startswith("' "):
     if not autoai:
       autoai = r2ai.interpreter.Interpreter()
       autoai.auto_run = True
     autoai.chat(usertext[2:])
   elif usertext[0] == ":":
     if r2 is None:
-      print("r2 is not available")
+      print("r2 is not available", file=sys.stderr)
     else:
       print(r2_cmd(usertext[1:]))
   elif usertext.startswith("-"):
-    print("Unknown flag. See 'r2ai -h' for help")
+    print("Unknown flag. See 'r2ai -h' for help", file=sys.stderr)
   else:
     ai.chat(usertext)
 
 def r2ai_repl(ai):
   from r2ai import bubble
+  tab_evals(ai.env.keys())
   oldoff = "0x00000000"
   olivemode = ai.env["chat.live"]
   ai.env["chat.live"] = "true"
   while True:
     prompt = "[r2ai:" + oldoff + "]> "
     if r2 is not None:
       off = r2_cmd("s").strip()
@@ -366,9 +403,9 @@
           bubble.response_end()
       else:
         if runline(ai, usertext) == "q":
           break
     except:
       traceback.print_exc()
       continue
-    readline.write_history_file(R2AI_HISTFILE)
+    tab_write()
   ai.env["chat.live"] = olivemode
```

### Comparing `r2ai-0.6.1/r2ai/utils.py` & `r2ai-0.7.0/r2ai/utils.py`

 * *Files identical despite different names*

### Comparing `r2ai-0.6.1/r2ai/voice.py` & `r2ai-0.7.0/r2ai/voice.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 except:
 	pass
 
 have_festival = os.path.isfile("/usr/bin/festival")
 
 def run(models):
 	for model in models:
-		cmd=f"ffmpeg -f avfoundation -list_devices true -i '' 2>&1 | grep '{model}'|cut -d '[' -f 3"
+		cmd = f"ffmpeg -f avfoundation -list_devices true -i '' 2>&1 | grep '{model}'|cut -d '[' -f 3"
 		output = syscmdstr(cmd)
 		if output != "":
 			return ":" + output[0]
 	return None
 
 def get_microphone(lang):
 	global DEVICE
```

### Comparing `r2ai-0.6.1/r2ai.egg-info/PKG-INFO` & `r2ai-0.7.0/r2ai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2ai
-Version: 0.6.1
+Version: 0.7.0
 Summary: Applying language models on radare2 for reverse engineering and fun purposes
 Home-page: https://www.radare.org/
 Author: pancake
 Author-email: pancake@nopcode.org
 Description-Content-Type: text/markdown
 Requires-Dist: rich
 Requires-Dist: r2pipe
@@ -24,14 +24,16 @@
 |  \____|/  ____||  _,_  || : |
 |   :  \ \   .  ||   :   ||   |
 |   |___\ \__:__||___|   ||   |
 |___|        :       |___||___|
              *       --pancake
 ```
 
+[![ci](https://github.com/radareorg/r2ai/actions/workflows/ci.yml/badge.svg)](https://github.com/radareorg/r2ai/actions/workflows/ci.yml)
+
 Run a language model in local, without internet, to entertain you or help answering questions about radare2 or reverse engineering in general. Note that models used by r2ai are pulled from external sources which may behave different or respond unrealible information. That's why there's an ongoing effort into improving the post-finetuning using memgpt-like techniques which can't get better without your help!
 
 <p align="center">
   <img src="doc/r2clippy.jpg">
 </p>
 
 ## Features
@@ -102,14 +104,15 @@
 
 ## Usage
 
 There are 4 different ways to run `r2ai`:
 
 * Standalone and interactive: `r2pm -r r2ai` or `python main.py`
 * Batch mode: `r2ai '-r act as a calculator' '3+3=?'`
+* As an r2 plugin: `r2 -i main.py /bin/ls`
 * From radare2 (requires `r2pm -ci rlang-python`): `r2 -c 'r2ai -h'`
 * Using r2pipe: `#!pipe python main.py`
   * Define a macro command: `'$r2ai=#!pipe python main.py`
 
 ## Auto mode
 
 When using OpenAI, Claude or any of the Functionary local models you can use the auto mode which permits the language model to execute r2 commands, analyze the output in loop and in a loop until it is resolved. Here's a sample session to achieve that:
@@ -122,26 +125,26 @@
 [0x00000000]> '$r2ai=#!pipe python main.py
 [0x00000000]> $r2ai '-m openai:gpt-4'
 [0x00000000]> $r2ai "' list the imports for this program"
 [0x00000000]> $r2ai "' draw me a donut"
 [0x00000000]> $r2ai "' decompile current function and explain it"
 ```
 
-
 ## Examples
 
 You can interact with r2ai from standalone python, from r2pipe via r2 keeping a global state or using the javascript intrepreter embedded inside `radare2`.
 
 * [conversation.r2.js](examples/conversation.r2.js) - load two models and make them talk to each other
 
 ### Development/Testing
 
 Just run `make` .. or well `python main.py`
 
 ### TODO
 
 * add "undo" command to drop the last message
 * dump / restore conversational states (see -L command)
+* Implement `~`, `|` and `>`
 
 ### Kudos
 
 The original code of r2ai is based on OpenInterpreter. I want to thanks all the contributors to this project as they made it possible to build r2ai taking their code as source for this.  Kudos to Killian and all the contributors.
```

### Comparing `r2ai-0.6.1/setup.py` & `r2ai-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+"""The classic setuptools python file."""
+
 from setuptools import setup
 import r2ai
 
-with open("README.md") as fd:
+with open("README.md", encoding = "utf-8") as fd:
     readme = fd.read()
 
 setup(
-    name='r2ai',
-    version=r2ai.VERSION,
-    description="Applying language models on radare2 for reverse engineering and fun purposes",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author="pancake",
-    author_email="pancake@nopcode.org",
-    url="https://www.radare.org/",
-    packages=[
+    name ='r2ai',
+    version = r2ai.VERSION,
+    description = "Applying language models on radare2 for reverse engineering and fun purposes",
+    long_description = readme,
+    long_description_content_type = "text/markdown",
+    author = "pancake",
+    author_email = "pancake@nopcode.org",
+    url = "https://www.radare.org/",
+    packages = [
         'r2ai',
     ],
-    install_requires=[
+    install_requires = [
         'rich',
         'r2pipe',
         'inquirer',
         'llama-cpp-python',
         'huggingface_hub',
         'appdirs',
         'unidecode',
@@ -29,9 +31,9 @@
         'pydantic',
         'torch',
     ],
     entry_points = {
         'console_scripts': [
             'r2ai = r2ai.main:main'
         ]
-    },
+    }
 )
```

