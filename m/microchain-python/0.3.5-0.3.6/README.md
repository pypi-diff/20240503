# Comparing `tmp/microchain-python-0.3.5.tar.gz` & `tmp/microchain_python-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microchain-python-0.3.5.tar", last modified: Mon Apr  8 09:34:07 2024, max compression
+gzip compressed data, was "microchain_python-0.3.6.tar", last modified: Fri May  3 14:33:06 2024, max compression
```

## Comparing `microchain-python-0.3.5.tar` & `microchain_python-0.3.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.260300 microchain-python-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-08 09:33:54.000000 microchain-python-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-08 09:34:07.260300 microchain-python-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-08 09:33:54.000000 microchain-python-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/engine/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-08 09:33:54.000000 microchain-python-0.3.5/microchain/models/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/microchain_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 09:34:07.000000 microchain-python-0.3.5/microchain_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:34:07.260300 microchain-python-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-08 09:33:54.000000 microchain-python-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:34:07.256300 microchain-python-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-08 09:33:54.000000 microchain-python-0.3.5/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-08 09:33:54.000000 microchain-python-0.3.5/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 09:33:54.000000 microchain-python-0.3.5/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.847809 microchain_python-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-03 14:32:58.000000 microchain_python-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-03 14:33:06.843809 microchain_python-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-03 14:32:58.000000 microchain_python-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:33:06.847809 microchain_python-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-03 14:32:58.000000 microchain_python-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-03 14:32:58.000000 microchain_python-0.3.6/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-03 14:32:58.000000 microchain_python-0.3.6/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 14:32:58.000000 microchain_python-0.3.6/tests/test_openai.py
```

### Comparing `microchain-python-0.3.5/LICENSE` & `microchain_python-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/PKG-INFO` & `microchain_python-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.5
+Version: 0.3.6
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain-python-0.3.5/README.md` & `microchain_python-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/microchain/engine/agent.py` & `microchain_python-0.3.6/microchain/engine/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,37 +14,40 @@
         self.engine.bind(self)
         self.reset()
 
     def reset(self):
         self.history = []
         self.do_stop = False
 
+    def execute_command(self, command: str):
+        result, output = self.engine.execute(command)
+        if result == FunctionResult.ERROR:
+            raise Exception(f"Your command ({command}) contains an error. output={output}")
+
+        print(colored(f">> {command}", "blue"))
+        print(colored(f"{output}", "green"))
+
+        self.history.append(dict(
+            role="assistant",
+            content=command
+        ))
+        self.history.append(dict(
+            role="user",
+            content=output
+        ))
+
     def build_initial_messages(self):
         self.history = [
             dict(
                 role="user",
                 content=self.prompt
             ),
         ]
         for command in self.bootstrap:
-            result, output = self.engine.execute(command)
-            if result == FunctionResult.ERROR:
-                raise Exception(f"Your bootstrap commands contain an error. output={output}")
-
-            print(colored(f">> {command}", "blue"))
-            print(colored(f"{output}", "green"))
-
-            self.history.append(dict(
-                role="assistant",
-                content=command
-            ))
-            self.history.append(dict(
-                role="user",
-                content=output
-            ))
+            self.execute_command(command)
             
     def clean_reply(self, reply):
         reply = reply.replace("\_", "_")
         reply = reply.strip()
         reply = reply[:reply.rfind(")")+1]
         return reply
 
@@ -98,24 +101,24 @@
         
         return dict(
             abort=abort,
             reply=reply,
             output=output,
         )
 
-    def run(self, iterations=10):
+    def run(self, iterations=10, resume=False):
         if self.prompt is None:
             raise ValueError("You must set a prompt before running the agent")
 
-        print(colored(f"prompt:\n{self.prompt}", "blue"))
-        print(colored(f"Running {iterations} iterations", "green"))
-
-        self.reset()
-        self.build_initial_messages()
+        if not resume:
+            print(colored(f"prompt:\n{self.prompt}", "blue"))
+            self.reset()
+            self.build_initial_messages()
 
+        print(colored(f"Running {iterations} iterations", "green"))
         for it in range(iterations):
             if self.do_stop:
                 break
 
             step_output = self.step()
             
             if step_output["abort"]:
```

### Comparing `microchain-python-0.3.5/microchain/engine/engine.py` & `microchain_python-0.3.6/microchain/engine/engine.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/microchain/engine/function.py` & `microchain_python-0.3.6/microchain/engine/function.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/microchain/functions.py` & `microchain_python-0.3.6/microchain/functions.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/microchain/models/templates.py` & `microchain_python-0.3.6/microchain/models/templates.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/microchain_python.egg-info/PKG-INFO` & `microchain_python-0.3.6/microchain_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.5
+Version: 0.3.6
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain-python-0.3.5/microchain_python.egg-info/SOURCES.txt` & `microchain_python-0.3.6/microchain_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/setup.py` & `microchain_python-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "README.md"), "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="microchain-python",
-    version="0.3.5",
+    version="0.3.6",
     author="Federico A. Galatolo",
     author_email="federico.galatolo@unipi.it",
     description="",
     url="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["microchain", "microchain.models", "microchain.engine"],
```

### Comparing `microchain-python-0.3.5/tests/test_agent.py` & `microchain_python-0.3.6/tests/test_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         llm = object()
         agent = Agent(llm=llm, engine=engine)
         
         agent.prompt=""
         agent.bootstrap = [
             'Sum(a=2*2, b=2)'
         ]
-        self.assertRaisesRegex(Exception, r".*Your bootstrap commands contain an error\. output=Error: the command Sum\(a=2\*2, b=2\) must be a function call, you cannot use variables\. Please try again\..*", agent.run, 1)
+        self.assertRaisesRegex(Exception, r".*Your command \(Sum\(a=2\*2, b=2\)\) contains an error. output=Error: the command Sum\(a=2\*2, b=2\) must be a function call, you cannot use variables\. Please try again\..*", agent.run, 1)
 
     def test_step_empty_reply(self):
         engine = Engine()
         engine.register(Sum())
         engine.agent=object()
         engine.help_called = True
         llm = LLM()
```

### Comparing `microchain-python-0.3.5/tests/test_engine.py` & `microchain_python-0.3.6/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `microchain-python-0.3.5/tests/test_openai.py` & `microchain_python-0.3.6/tests/test_openai.py`

 * *Files identical despite different names*

