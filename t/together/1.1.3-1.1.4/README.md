# Comparing `tmp/together-1.1.3.tar.gz` & `tmp/together-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-1.1.3.tar", max compression
+gzip compressed data, was "together-1.1.4.tar", max compression
```

## Comparing `together-1.1.3.tar` & `together-1.1.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-04-30 18:14:31.730405 together-1.1.3/LICENSE
--rw-r--r--   0        0        0    10365 2024-04-30 18:14:31.730405 together-1.1.3/README.md
--rw-r--r--   0        0        0     2590 2024-04-30 18:14:31.730405 together-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-04-30 18:14:31.734405 together-1.1.3/src/together/__init__.py
--rw-r--r--   0        0        0       57 2024-04-30 18:14:31.734405 together-1.1.3/src/together/abstract/__init__.py
--rw-r--r--   0        0        0    25103 2024-04-30 18:14:31.734405 together-1.1.3/src/together/abstract/api_requestor.py
--rw-r--r--   0        0        0        0 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/__init__.py
--rw-r--r--   0        0        0     7838 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/chat.py
--rw-r--r--   0        0        0     3691 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/completions.py
--rw-r--r--   0        0        0     3186 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/files.py
--rw-r--r--   0        0        0     4954 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/finetune.py
--rw-r--r--   0        0        0     2363 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/images.py
--rw-r--r--   0        0        0     1126 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/api/models.py
--rw-r--r--   0        0        0     1977 2024-04-30 18:14:31.734405 together-1.1.3/src/together/cli/cli.py
--rw-r--r--   0        0        0     4774 2024-04-30 18:14:31.734405 together-1.1.3/src/together/client.py
--rw-r--r--   0        0        0      908 2024-04-30 18:14:31.734405 together-1.1.3/src/together/constants.py
--rw-r--r--   0        0        0     5329 2024-04-30 18:14:31.734405 together-1.1.3/src/together/error.py
--rw-r--r--   0        0        0    11438 2024-04-30 18:14:31.734405 together-1.1.3/src/together/filemanager.py
--rw-r--r--   0        0        0        0 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/__init__.py
--rw-r--r--   0        0        0      727 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/base.py
--rw-r--r--   0        0        0     2343 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/complete.py
--rw-r--r--   0        0        0      591 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/embeddings.py
--rw-r--r--   0        0        0     3863 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/files.py
--rw-r--r--   0        0        0     4917 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/finetune.py
--rw-r--r--   0        0        0      582 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/images.py
--rw-r--r--   0        0        0     1053 2024-04-30 18:14:31.734405 together-1.1.3/src/together/legacy/models.py
--rw-r--r--   0        0        0      701 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/__init__.py
--rw-r--r--   0        0        0      617 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/chat/__init__.py
--rw-r--r--   0        0        0    11140 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/chat/completions.py
--rw-r--r--   0        0        0     8403 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/completions.py
--rw-r--r--   0        0        0     2546 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/embeddings.py
--rw-r--r--   0        0        0     4593 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/files.py
--rw-r--r--   0        0        0    12416 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/finetune.py
--rw-r--r--   0        0        0     4775 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/images.py
--rw-r--r--   0        0        0     1786 2024-04-30 18:14:31.734405 together-1.1.3/src/together/resources/models.py
--rw-r--r--   0        0        0     1319 2024-04-30 18:14:31.734405 together-1.1.3/src/together/together_response.py
--rw-r--r--   0        0        0     1432 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/__init__.py
--rw-r--r--   0        0        0      642 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/abstract.py
--rw-r--r--   0        0        0     3648 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/chat_completions.py
--rw-r--r--   0        0        0     1491 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/common.py
--rw-r--r--   0        0        0     2173 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/completions.py
--rw-r--r--   0        0        0      751 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/embeddings.py
--rw-r--r--   0        0        0      370 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/error.py
--rw-r--r--   0        0        0     1954 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/files.py
--rw-r--r--   0        0        0     5775 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/finetune.py
--rw-r--r--   0        0        0      915 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/images.py
--rw-r--r--   0        0        0     1013 2024-04-30 18:14:31.734405 together-1.1.3/src/together/types/models.py
--rw-r--r--   0        0        0      662 2024-04-30 18:14:31.734405 together-1.1.3/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/_log.py
--rw-r--r--   0        0        0     2407 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/api_helpers.py
--rw-r--r--   0        0        0     7165 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/files.py
--rw-r--r--   0        0        0     1788 2024-04-30 18:14:31.738405 together-1.1.3/src/together/utils/tools.py
--rw-r--r--   0        0        0      126 2024-04-30 18:14:31.738405 together-1.1.3/src/together/version.py
--rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 03:50:53.189128 together-1.1.4/LICENSE
+-rw-r--r--   0        0        0    10365 2024-05-03 03:50:53.189128 together-1.1.4/README.md
+-rw-r--r--   0        0        0     2590 2024-05-03 03:50:53.189128 together-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-05-03 03:50:53.189128 together-1.1.4/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-03 03:50:53.189128 together-1.1.4/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-05-03 03:50:53.189128 together-1.1.4/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     9170 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     4199 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3186 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     5417 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-05-03 03:50:53.189128 together-1.1.4/src/together/client.py
+-rw-r--r--   0        0        0      908 2024-05-03 03:50:53.189128 together-1.1.4/src/together/constants.py
+-rw-r--r--   0        0        0     5329 2024-05-03 03:50:53.189128 together-1.1.4/src/together/error.py
+-rw-r--r--   0        0        0    11438 2024-05-03 03:50:53.189128 together-1.1.4/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3863 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    14084 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0    11353 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4593 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/files.py
+-rw-r--r--   0        0        0    12416 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-05-03 03:50:53.189128 together-1.1.4/src/together/together_response.py
+-rw-r--r--   0        0        0     1432 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/abstract.py
+-rw-r--r--   0        0        0     4335 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/common.py
+-rw-r--r--   0        0        0     2887 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/error.py
+-rw-r--r--   0        0        0     1954 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/files.py
+-rw-r--r--   0        0        0     5775 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     7165 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-05-03 03:50:53.193128 together-1.1.4/src/together/version.py
+-rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.1.4/PKG-INFO
```

### Comparing `together-1.1.3/LICENSE` & `together-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `together-1.1.3/README.md` & `together-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `together-1.1.3/pyproject.toml` & `together-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "oldest-supported-numpy>=0.14; python_version<'3.9'",
     "numpy>=1.25; python_version>='3.9'",
 ]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `together-1.1.3/src/together/__init__.py` & `together-1.1.4/src/together/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/abstract/api_requestor.py` & `together-1.1.4/src/together/abstract/api_requestor.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/cli/api/chat.py` & `together-1.1.4/src/together/cli/api/chat.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,26 +24,32 @@
         model: str,
         max_tokens: int | None = None,
         stop: List[str] | None = None,
         temperature: float | None = None,
         top_p: float | None = None,
         top_k: int | None = None,
         repetition_penalty: float | None = None,
+        presence_penalty: float | None = None,
+        frequency_penalty: float | None = None,
+        min_p: float | None = None,
         safety_model: str | None = None,
         system_message: str | None = None,
     ) -> None:
         super().__init__()
         self.client = client
         self.model = model
         self.max_tokens = max_tokens
         self.stop = stop
         self.temperature = temperature
         self.top_p = top_p
         self.top_k = top_k
         self.repetition_penalty = repetition_penalty
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.min_p = min_p
         self.safety_model = safety_model
         self.system_message = system_message
 
         self.messages = (
             [{"role": "system", "content": self.system_message}]
             if self.system_message
             else []
@@ -65,28 +71,30 @@
             model=self.model,
             max_tokens=self.max_tokens,
             stop=self.stop,
             temperature=self.temperature,
             top_p=self.top_p,
             top_k=self.top_k,
             repetition_penalty=self.repetition_penalty,
+            presence_penalty=self.presence_penalty,
+            frequency_penalty=self.frequency_penalty,
+            min_p=self.min_p,
             safety_model=self.safety_model,
             stream=True,
         ):
             # assertions for type checking
             assert isinstance(chunk, ChatCompletionChunk)
             assert chunk.choices
             assert chunk.choices[0].delta
-            assert chunk.choices[0].delta.content
 
             token = chunk.choices[0].delta.content
 
             click.echo(token, nl=False)
 
-            output += token
+            output += token or ""
 
         click.echo("\n")
 
         self.messages.append({"role": "assistant", "content": output})
 
     def do_reset(self, arg: str) -> None:
         self.messages = (
@@ -105,25 +113,32 @@
 @click.option("--max-tokens", type=int, help="Max tokens to generate")
 @click.option(
     "--stop", type=str, multiple=True, help="List of strings to stop generation"
 )
 @click.option("--temperature", type=float, help="Sampling temperature")
 @click.option("--top-p", type=int, help="Top p sampling")
 @click.option("--top-k", type=float, help="Top k sampling")
+@click.option("--repetition-penalty", type=float, help="Repetition penalty")
+@click.option("--presence-penalty", type=float, help="Presence penalty")
+@click.option("--frequency-penalty", type=float, help="Frequency penalty")
+@click.option("--min-p", type=float, help="Minimum p")
 @click.option("--safety-model", type=str, help="Moderation model")
 @click.option("--system-message", type=str, help="System message to use for the chat")
 def interactive(
     ctx: click.Context,
     model: str,
     max_tokens: int | None = None,
     stop: List[str] | None = None,
     temperature: float | None = None,
     top_p: float | None = None,
     top_k: int | None = None,
     repetition_penalty: float | None = None,
+    presence_penalty: float | None = None,
+    frequency_penalty: float | None = None,
+    min_p: float | None = None,
     safety_model: str | None = None,
     system_message: str | None = None,
 ) -> None:
     """Interactive chat shell"""
     client: Together = ctx.obj
 
     ChatShell(
@@ -131,14 +146,17 @@
         model=model,
         max_tokens=max_tokens,
         stop=stop,
         temperature=temperature,
         top_p=top_p,
         top_k=top_k,
         repetition_penalty=repetition_penalty,
+        presence_penalty=presence_penalty,
+        frequency_penalty=frequency_penalty,
+        min_p=min_p,
         safety_model=safety_model,
         system_message=system_message,
     ).cmdloop()
 
 
 @click.command(name="chat.completions")
 @click.pass_context
@@ -154,14 +172,19 @@
 @click.option(
     "--stop", type=str, multiple=True, help="List of strings to stop generation"
 )
 @click.option("--temperature", type=float, help="Sampling temperature")
 @click.option("--top-p", type=int, help="Top p sampling")
 @click.option("--top-k", type=float, help="Top k sampling")
 @click.option("--repetition-penalty", type=float, help="Repetition penalty")
+@click.option("--presence-penalty", type=float, help="Presence penalty sampling method")
+@click.option(
+    "--frequency-penalty", type=float, help="Frequency penalty sampling method"
+)
+@click.option("--min-p", type=float, help="Min p sampling")
 @click.option("--no-stream", is_flag=True, help="Disable streaming")
 @click.option("--logprobs", type=int, help="Return logprobs. Only works with --raw.")
 @click.option("--echo", is_flag=True, help="Echo prompt. Only works with --raw.")
 @click.option("--n", type=int, help="Number of output generations")
 @click.option("--safety-model", type=str, help="Moderation model")
 @click.option("--raw", is_flag=True, help="Output raw JSON")
 def chat(
@@ -170,14 +193,17 @@
     model: str,
     max_tokens: int | None = None,
     stop: List[str] | None = None,
     temperature: float | None = None,
     top_p: float | None = None,
     top_k: int | None = None,
     repetition_penalty: float | None = None,
+    presence_penalty: float | None = None,
+    frequency_penalty: float | None = None,
+    min_p: float | None = None,
     no_stream: bool = False,
     logprobs: int | None = None,
     echo: bool | None = None,
     n: int | None = None,
     safety_model: str | None = None,
     raw: bool = False,
 ) -> None:
@@ -191,14 +217,17 @@
         messages=messages,
         top_p=top_p,
         top_k=top_k,
         temperature=temperature,
         max_tokens=max_tokens,
         stop=stop,
         repetition_penalty=repetition_penalty,
+        presence_penalty=presence_penalty,
+        frequency_penalty=frequency_penalty,
+        min_p=min_p,
         stream=not no_stream,
         logprobs=logprobs,
         echo=echo,
         n=n,
         safety_model=safety_model,
     )
```

### Comparing `together-1.1.3/src/together/cli/api/completions.py` & `together-1.1.4/src/together/cli/api/completions.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 from together.types.completions import CompletionChoicesChunk, CompletionResponse
 
 
 @click.command()
 @click.pass_context
 @click.argument("prompt", type=str, required=True)
 @click.option("--model", type=str, required=True, help="Model name")
-@click.option("--no-stream", is_flag=True, help="Disable streaming")
 @click.option("--max-tokens", type=int, help="Max tokens to generate")
 @click.option(
     "--stop", type=str, multiple=True, help="List of strings to stop generation"
 )
 @click.option("--temperature", type=float, help="Sampling temperature")
 @click.option("--top-p", type=int, help="Top p sampling")
 @click.option("--top-k", type=float, help="Top k sampling")
+@click.option("--repetition-penalty", type=float, help="Repetition penalty")
+@click.option("--presence-penalty", type=float, help="Presence penalty")
+@click.option("--frequency-penalty", type=float, help="Frequency penalty")
+@click.option("--min-p", type=float, help="Minimum p")
+@click.option("--no-stream", is_flag=True, help="Disable streaming")
 @click.option("--logprobs", type=int, help="Return logprobs. Only works with --raw.")
 @click.option("--echo", is_flag=True, help="Echo prompt. Only works with --raw.")
 @click.option("--n", type=int, help="Number of output generations")
 @click.option("--safety-model", type=str, help="Moderation model")
 @click.option("--raw", is_flag=True, help="Return raw JSON response")
 def completions(
     ctx: click.Context,
@@ -33,14 +37,17 @@
     model: str,
     max_tokens: int | None = 512,
     stop: List[str] | None = None,
     temperature: float | None = None,
     top_p: float | None = None,
     top_k: int | None = None,
     repetition_penalty: float | None = None,
+    presence_penalty: float | None = None,
+    frequency_penalty: float | None = None,
+    min_p: float | None = None,
     no_stream: bool = False,
     logprobs: int | None = None,
     echo: bool | None = None,
     n: int | None = None,
     safety_model: str | None = None,
     raw: bool = False,
 ) -> None:
@@ -52,14 +59,17 @@
         prompt=prompt,
         top_p=top_p,
         top_k=top_k,
         temperature=temperature,
         max_tokens=max_tokens,
         stop=stop,
         repetition_penalty=repetition_penalty,
+        presence_penalty=presence_penalty,
+        frequency_penalty=frequency_penalty,
+        min_p=min_p,
         stream=not no_stream,
         logprobs=logprobs,
         echo=echo,
         n=n,
         safety_model=safety_model,
     )
```

### Comparing `together-1.1.3/src/together/cli/api/files.py` & `together-1.1.4/src/together/cli/api/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/cli/api/finetune.py` & `together-1.1.4/src/together/cli/api/finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,18 +103,28 @@
 
     click.echo(json.dumps(response.model_dump(), indent=4))
 
 
 @fine_tuning.command()
 @click.pass_context
 @click.argument("fine_tune_id", type=str, required=True)
-def cancel(ctx: click.Context, fine_tune_id: str) -> None:
+@click.option(
+    "--quiet", is_flag=True, help="Do not prompt for confirmation before cancelling job"
+)
+def cancel(ctx: click.Context, fine_tune_id: str, quiet: bool = False) -> None:
     """Cancel fine-tuning job"""
     client: Together = ctx.obj
-
+    if not quiet:
+        confirm_response = input(
+            "You will be billed for any completed training steps upon cancellation. "
+            f"Do you want to cancel job {fine_tune_id}? [y/N]"
+        )
+        if "y" not in confirm_response.lower():
+            click.echo({"status": "Cancel not submitted"})
+            return
     response = client.fine_tuning.cancel(fine_tune_id)
 
     click.echo(json.dumps(response.model_dump(), indent=4))
 
 
 @fine_tuning.command()
 @click.pass_context
```

### Comparing `together-1.1.3/src/together/cli/api/images.py` & `together-1.1.4/src/together/cli/api/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/cli/api/models.py` & `together-1.1.4/src/together/cli/api/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/cli/cli.py` & `together-1.1.4/src/together/cli/cli.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/client.py` & `together-1.1.4/src/together/client.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/constants.py` & `together-1.1.4/src/together/constants.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/error.py` & `together-1.1.4/src/together/error.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/filemanager.py` & `together-1.1.4/src/together/filemanager.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/base.py` & `together-1.1.4/src/together/legacy/base.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/complete.py` & `together-1.1.4/src/together/legacy/complete.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/embeddings.py` & `together-1.1.4/src/together/legacy/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/files.py` & `together-1.1.4/src/together/legacy/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/finetune.py` & `together-1.1.4/src/together/legacy/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/images.py` & `together-1.1.4/src/together/legacy/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/legacy/models.py` & `together-1.1.4/src/together/legacy/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/__init__.py` & `together-1.1.4/src/together/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/chat/__init__.py` & `together-1.1.4/src/together/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/chat/completions.py` & `together-1.1.4/src/together/resources/completions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 from __future__ import annotations
 
-from typing import Any, AsyncGenerator, Dict, Iterator, List
+from typing import AsyncGenerator, Dict, Iterator, List
 
 from together.abstract import api_requestor
 from together.together_response import TogetherResponse
 from together.types import (
-    ChatCompletionChunk,
-    ChatCompletionRequest,
-    ChatCompletionResponse,
+    CompletionChunk,
+    CompletionRequest,
+    CompletionResponse,
     TogetherClient,
     TogetherRequest,
 )
 
 
-class ChatCompletions:
+class Completions:
     def __init__(self, client: TogetherClient) -> None:
         self._client = client
 
     def create(
         self,
         *,
-        messages: List[Dict[str, str]],
+        prompt: str,
         model: str,
-        max_tokens: int | None = None,
+        max_tokens: int | None = 512,
         stop: List[str] | None = None,
         temperature: float | None = None,
         top_p: float | None = None,
         top_k: int | None = None,
         repetition_penalty: float | None = None,
+        presence_penalty: float | None = None,
+        frequency_penalty: float | None = None,
+        min_p: float | None = None,
+        logit_bias: Dict[str, float] | None = None,
         stream: bool = False,
         logprobs: int | None = None,
         echo: bool | None = None,
         n: int | None = None,
         safety_model: str | None = None,
-        response_format: Dict[str, str | Dict[str, Any]] | None = None,
-        tools: Dict[str, str | Dict[str, Any]] | None = None,
-        tool_choice: str | Dict[str, str | Dict[str, str]] | None = None,
-    ) -> ChatCompletionResponse | Iterator[ChatCompletionChunk]:
+    ) -> CompletionResponse | Iterator[CompletionChunk]:
         """
         Method to generate completions based on a given prompt using a specified model.
 
         Args:
-            messages (List[Dict[str, str]]): A list of messages in the format
-                `[{"role": together.types.chat_completions.MessageRole, "content": TEXT}, ...]`
+            prompt (str): A string providing context for the model to complete.
             model (str): The name of the model to query.
             max_tokens (int, optional): The maximum number of tokens to generate.
                 Defaults to 512.
             stop (List[str], optional): List of strings at which to stop generation.
                 Defaults to None.
             temperature (float, optional): A decimal number that determines the degree of randomness in the response.
                 Defaults to None.
@@ -55,112 +55,117 @@
                 Defaults to None.
             top_k (int, optional): The top_k parameter is used to limit the number of choices for the
                     next predicted word or token.
                 Defaults to None.
             repetition_penalty (float, optional): A number that controls the diversity of generated text
                     by reducing the likelihood of repeated sequences. Higher values decrease repetition.
                 Defaults to None.
+            presence_penalty (float, optional): A number that controls the likelihood of tokens based on if they have
+                    appeared in the text. Positive values decrease the likelihood of repeated tokens or phrases.
+                    Must be in the range [-2, 2].
+                Defaults to None.
+            frequency_penalty (float, optional): A number that controls the likelihood of tokens based on the frequency
+                    of their appearance in the text. Positive decrease the likelihood of repeated tokens or phrases.
+                    Must be in the range [-2, 2].
+                Defaults to None.
+            min_p (float, optional): A number that controls the minimum percentage value that a token must reach to
+                be considered during sampling.
+                Must be in the range [0, 1].
+                Defaults to None.
+            logit_bias (Dict[str, float], optional): A dictionary of tokens and their bias values that modify the
+                likelihood of specific tokens being sampled. Bias values must be in the range [-100, 100].
+                Defaults to None.
             stream (bool, optional): Flag indicating whether to stream the generated completions.
                 Defaults to False.
             logprobs (int, optional): Number of top-k logprobs to return
                 Defaults to None.
             echo (bool, optional): Echo prompt in output. Can be used with logprobs to return prompt logprobs.
                 Defaults to None.
             n (int, optional): Number of completions to generate. Setting to None will return a single generation.
                 Defaults to None.
             safety_model (str, optional): A moderation model to validate tokens. Choice between available moderation
                     models found [here](https://docs.together.ai/docs/inference-models#moderation-models).
                 Defaults to None.
-            response_format (Dict[str, Any], optional): An object specifying the format that the model must output.
-                Defaults to None.
-            tools (Dict[str, str | Dict[str, str | Dict[str, Any]]], optional): A list of tools the model may call.
-                    Currently, only functions are supported as a tool.
-                    Use this to provide a list of functions the model may generate JSON inputs for.
-                Defaults to None
-            tool_choice: Controls which (if any) function is called by the model. auto means the model can pick
-                    between generating a message or calling a function. Specifying a particular function
-                    via {"type": "function", "function": {"name": "my_function"}} forces the model to call that function.
-                    Sets to `auto` if None.
-                Defaults to None.
 
         Returns:
-            ChatCompletionResponse | Iterator[ChatCompletionChunk]: Object containing the completions
+            CompletionResponse | Iterator[CompletionChunk]: Object containing the completions
             or an iterator over completion chunks.
         """
 
         requestor = api_requestor.APIRequestor(
             client=self._client,
         )
 
-        parameter_payload = ChatCompletionRequest(
+        parameter_payload = CompletionRequest(
             model=model,
-            messages=messages,
+            prompt=prompt,
             top_p=top_p,
             top_k=top_k,
             temperature=temperature,
             max_tokens=max_tokens,
             stop=stop,
             repetition_penalty=repetition_penalty,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            min_p=min_p,
+            logit_bias=logit_bias,
             stream=stream,
             logprobs=logprobs,
             echo=echo,
             n=n,
             safety_model=safety_model,
-            response_format=response_format,
-            tools=tools,
-            tool_choice=tool_choice,
         ).model_dump()
 
         response, _, _ = requestor.request(
             options=TogetherRequest(
                 method="POST",
-                url="chat/completions",
+                url="completions",
                 params=parameter_payload,
             ),
             stream=stream,
         )
 
         if stream:
             # must be an iterator
             assert not isinstance(response, TogetherResponse)
-            return (ChatCompletionChunk(**line.data) for line in response)
+            return (CompletionChunk(**line.data) for line in response)
         assert isinstance(response, TogetherResponse)
-        return ChatCompletionResponse(**response.data)
+        return CompletionResponse(**response.data)
 
 
-class AsyncChatCompletions:
+class AsyncCompletions:
     def __init__(self, client: TogetherClient) -> None:
         self._client = client
 
     async def create(
         self,
         *,
-        messages: List[Dict[str, str]],
+        prompt: str,
         model: str,
-        max_tokens: int | None = None,
+        max_tokens: int | None = 512,
         stop: List[str] | None = None,
         temperature: float | None = None,
         top_p: float | None = None,
         top_k: int | None = None,
         repetition_penalty: float | None = None,
+        presence_penalty: float | None = None,
+        frequency_penalty: float | None = None,
+        min_p: float | None = None,
+        logit_bias: Dict[str, float] | None = None,
         stream: bool = False,
         logprobs: int | None = None,
         echo: bool | None = None,
         n: int | None = None,
         safety_model: str | None = None,
-        response_format: Dict[str, Any] | None = None,
-        tools: Dict[str, str | Dict[str, str | Dict[str, Any]]] | None = None,
-        tool_choice: str | Dict[str, str | Dict[str, str]] | None = None,
-    ) -> AsyncGenerator[ChatCompletionChunk, None] | ChatCompletionResponse:
+    ) -> AsyncGenerator[CompletionChunk, None] | CompletionResponse:
         """
         Async method to generate completions based on a given prompt using a specified model.
 
         Args:
-            messages (List[Dict[str, str]]): A list of messages in the format
-                `[{"role": together.types.chat_completions.MessageRole, "content": TEXT}, ...]`
+            prompt (str): A string providing context for the model to complete.
             model (str): The name of the model to query.
             max_tokens (int, optional): The maximum number of tokens to generate.
                 Defaults to 512.
             stop (List[str], optional): List of strings at which to stop generation.
                 Defaults to None.
             temperature (float, optional): A decimal number that determines the degree of randomness in the response.
                 Defaults to None.
@@ -169,73 +174,78 @@
                 Defaults to None.
             top_k (int, optional): The top_k parameter is used to limit the number of choices for the
                     next predicted word or token.
                 Defaults to None.
             repetition_penalty (float, optional): A number that controls the diversity of generated text
                     by reducing the likelihood of repeated sequences. Higher values decrease repetition.
                 Defaults to None.
+            presence_penalty (float, optional): A number that controls the likelihood of tokens based on if they have
+                    appeared in the text. Positive values decrease the likelihood of repeated tokens or phrases.
+                    Must be in the range [-2, 2].
+                Defaults to None.
+            frequency_penalty (float, optional): A number that controls the likelihood of tokens based on the frequency
+                    of their appearance in the text. Positive decrease the likelihood of repeated tokens or phrases.
+                    Must be in the range [-2, 2].
+                Defaults to None.
+            min_p (float, optional): A number that controls the minimum percentage value that a token must reach to
+                be considered during sampling.
+                Must be in the range [0, 1].
+                Defaults to None.
+            logit_bias (Dict[str, float], optional): A dictionary of tokens and their bias values that modify the
+                likelihood of specific tokens being sampled. Bias values must be in the range [-100, 100].
+                Defaults to None.
             stream (bool, optional): Flag indicating whether to stream the generated completions.
                 Defaults to False.
             logprobs (int, optional): Number of top-k logprobs to return
                 Defaults to None.
             echo (bool, optional): Echo prompt in output. Can be used with logprobs to return prompt logprobs.
                 Defaults to None.
             n (int, optional): Number of completions to generate. Setting to None will return a single generation.
                 Defaults to None.
             safety_model (str, optional): A moderation model to validate tokens. Choice between available moderation
                     models found [here](https://docs.together.ai/docs/inference-models#moderation-models).
                 Defaults to None.
-            response_format (Dict[str, Any], optional): An object specifying the format that the model must output.
-                Defaults to None.
-            tools (Dict[str, str | Dict[str, str | Dict[str, Any]]], optional): A list of tools the model may call.
-                    Currently, only functions are supported as a tool.
-                    Use this to provide a list of functions the model may generate JSON inputs for.
-                Defaults to None
-            tool_choice: Controls which (if any) function is called by the model. auto means the model can pick
-                    between generating a message or calling a function. Specifying a particular function
-                    via {"type": "function", "function": {"name": "my_function"}} forces the model to call that function.
-                    Sets to `auto` if None.
-                Defaults to None.
 
         Returns:
-            AsyncGenerator[ChatCompletionChunk, None] | ChatCompletionResponse: Object containing the completions
+            AsyncGenerator[CompletionChunk, None] | CompletionResponse: Object containing the completions
             or an iterator over completion chunks.
         """
 
         requestor = api_requestor.APIRequestor(
             client=self._client,
         )
 
-        parameter_payload = ChatCompletionRequest(
+        parameter_payload = CompletionRequest(
             model=model,
-            messages=messages,
+            prompt=prompt,
             top_p=top_p,
             top_k=top_k,
             temperature=temperature,
             max_tokens=max_tokens,
             stop=stop,
             repetition_penalty=repetition_penalty,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            min_p=min_p,
+            logit_bias=logit_bias,
             stream=stream,
             logprobs=logprobs,
             echo=echo,
             n=n,
             safety_model=safety_model,
-            response_format=response_format,
-            tools=tools,
-            tool_choice=tool_choice,
         ).model_dump()
 
         response, _, _ = await requestor.arequest(
             options=TogetherRequest(
                 method="POST",
-                url="chat/completions",
+                url="completions",
                 params=parameter_payload,
             ),
             stream=stream,
         )
 
         if stream:
             # must be an iterator
             assert not isinstance(response, TogetherResponse)
-            return (ChatCompletionChunk(**line.data) async for line in response)
+            return (CompletionChunk(**line.data) async for line in response)
         assert isinstance(response, TogetherResponse)
-        return ChatCompletionResponse(**response.data)
+        return CompletionResponse(**response.data)
```

### Comparing `together-1.1.3/src/together/resources/embeddings.py` & `together-1.1.4/src/together/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/files.py` & `together-1.1.4/src/together/resources/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/finetune.py` & `together-1.1.4/src/together/resources/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/images.py` & `together-1.1.4/src/together/resources/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/resources/models.py` & `together-1.1.4/src/together/resources/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/together_response.py` & `together-1.1.4/src/together/together_response.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/__init__.py` & `together-1.1.4/src/together/types/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/abstract.py` & `together-1.1.4/src/together/types/abstract.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/chat_completions.py` & `together-1.1.4/src/together/types/chat_completions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
+import warnings
 from enum import Enum
 from typing import Any, Dict, List
 
-from pydantic import Field
+from pydantic import Field, model_validator
+from typing_extensions import Self
 
 from together.types.abstract import BaseModel
 from together.types.common import (
     DeltaContent,
     FinishReason,
     LogprobsPart,
     ObjectType,
@@ -83,14 +85,18 @@
     # stopping criteria: list of strings to stop generation
     stop: List[str] | None = None
     # sampling hyperparameters
     temperature: float | None = None
     top_p: float | None = None
     top_k: int | None = None
     repetition_penalty: float | None = None
+    presence_penalty: float | None = None
+    frequency_penalty: float | None = None
+    min_p: float | None = None
+    logit_bias: Dict[str, float] | None = None
     # stream SSE token chunks
     stream: bool = False
     # return logprobs
     logprobs: int | None = None
     # echo prompt.
     # can be used with logprobs to return prompt logprobs
     echo: bool | None = None
@@ -99,14 +105,24 @@
     # moderation model
     safety_model: str | None = None
     # constraints
     response_format: ResponseFormat | None = None
     tools: List[Tools] | None = None
     tool_choice: ToolChoice | ToolChoiceEnum | None = None
 
+    # Raise warning if repetition_penalty is used with presence_penalty or frequency_penalty
+    @model_validator(mode="after")
+    def verify_parameters(self) -> Self:
+        if self.repetition_penalty:
+            if self.presence_penalty or self.frequency_penalty:
+                warnings.warn(
+                    "repetition_penalty is not advisable to be used alongside presence_penalty or frequency_penalty"
+                )
+        return self
+
 
 class ChatCompletionChoicesData(BaseModel):
     index: int | None = None
     logprobs: LogprobsPart | None = None
     finish_reason: FinishReason | None = None
     message: ChatCompletionMessage | None = None
```

### Comparing `together-1.1.3/src/together/types/common.py` & `together-1.1.4/src/together/types/common.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/completions.py` & `together-1.1.4/src/together/types/images.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,42 @@
 from __future__ import annotations
 
-from typing import List
+from typing import List, Literal
 
 from together.types.abstract import BaseModel
-from together.types.common import (
-    DeltaContent,
-    FinishReason,
-    LogprobsPart,
-    ObjectType,
-    PromptPart,
-    UsageData,
-)
 
 
-class CompletionRequest(BaseModel):
-    # prompt to complete
+class ImageRequest(BaseModel):
+    # input or list of inputs
     prompt: str
-    # query model
+    # model to query
     model: str
-    # stopping criteria: max tokens to generate
-    max_tokens: int | None = None
-    # stopping criteria: list of strings to stop generation
-    stop: List[str] | None = None
-    # sampling hyperparameters
-    temperature: float | None = None
-    top_p: float | None = None
-    top_k: int | None = None
-    repetition_penalty: float | None = None
-    # stream SSE token chunks
-    stream: bool = False
-    # return logprobs
-    logprobs: int | None = None
-    # echo prompt.
-    # can be used with logprobs to return prompt logprobs
-    echo: bool | None = None
-    # number of output generations
-    n: int | None = None
-    # moderation model
-    safety_model: str | None = None
+    # num generation steps
+    steps: int | None = 20
+    # seed
+    seed: int | None = None
+    # number of results to return
+    n: int | None = 1
+    # pixel height
+    height: int | None = 1024
+    # pixel width
+    width: int | None = 1024
+    # negative prompt
+    negative_prompt: str | None = None
 
 
-class CompletionChoicesData(BaseModel):
+class ImageChoicesData(BaseModel):
+    # response index
     index: int
-    logprobs: LogprobsPart | None = None
-    finish_reason: FinishReason
-    text: str
-
-
-class CompletionChoicesChunk(BaseModel):
-    index: int | None = None
-    logprobs: float | None = None
-    finish_reason: FinishReason | None = None
-    delta: DeltaContent | None = None
+    # base64 image response
+    b64_json: str
 
 
-class CompletionResponse(BaseModel):
-    # request id
+class ImageResponse(BaseModel):
+    # job id
     id: str | None = None
-    # object type
-    object: ObjectType | None = None
-    # created timestamp
-    created: int | None = None
-    # model name
+    # query model
     model: str | None = None
-    # choices list
-    choices: List[CompletionChoicesData] | None = None
-    # prompt list
-    prompt: List[PromptPart] | None = None
-    # token usage data
-    usage: UsageData | None = None
-
-
-class CompletionChunk(BaseModel):
-    # request id
-    id: str | None = None
     # object type
-    object: ObjectType | None = None
-    # created timestamp
-    created: int | None = None
-    # model name
-    model: str | None = None
-    # choices list
-    choices: List[CompletionChoicesChunk] | None = None
-    # token usage data
-    usage: UsageData | None = None
+    object: Literal["list"] | None = None
+    # list of embedding choices
+    data: List[ImageChoicesData] | None = None
```

### Comparing `together-1.1.3/src/together/types/embeddings.py` & `together-1.1.4/src/together/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/files.py` & `together-1.1.4/src/together/types/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/finetune.py` & `together-1.1.4/src/together/types/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/types/models.py` & `together-1.1.4/src/together/types/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/utils/__init__.py` & `together-1.1.4/src/together/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/utils/_log.py` & `together-1.1.4/src/together/utils/_log.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/utils/api_helpers.py` & `together-1.1.4/src/together/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/utils/files.py` & `together-1.1.4/src/together/utils/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/src/together/utils/tools.py` & `together-1.1.4/src/together/utils/tools.py`

 * *Files identical despite different names*

### Comparing `together-1.1.3/PKG-INFO` & `together-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python client for Together's Cloud Platform!
 Home-page: https://github.com/togethercomputer/together-python
 License: Apache-2.0
 Author: Together AI
 Author-email: support@together.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: together Version: 1.1.3 Summary: Python client for
+Metadata-Version: 2.1 Name: together Version: 1.1.4 Summary: Python client for
 Together's Cloud Platform! Home-page: https://github.com/togethercomputer/
 together-python License: Apache-2.0 Author: Together AI Author-email:
 support@together.ai Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

