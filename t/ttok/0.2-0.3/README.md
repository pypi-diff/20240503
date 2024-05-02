# Comparing `tmp/ttok-0.2.tar.gz` & `tmp/ttok-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttok-0.2.tar", last modified: Mon Jul 10 23:38:22 2023, max compression
+gzip compressed data, was "ttok-0.3.tar", last modified: Thu May  2 23:39:00 2024, max compression
```

## Comparing `ttok-0.2.tar` & `ttok-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.424844 ttok-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 23:38:08.000000 ttok-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-10 23:38:22.420844 ttok-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-10 23:38:08.000000 ttok-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:38:22.424844 ttok-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-10 23:38:08.000000 ttok-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.420844 ttok-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-10 23:38:08.000000 ttok-0.2/tests/test_ttok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.420844 ttok-0.2/ttok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:08.000000 ttok-0.2/ttok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:38:08.000000 ttok-0.2/ttok/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-10 23:38:08.000000 ttok-0.2/ttok/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.420844 ttok-0.2/ttok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:39:00.682115 ttok-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 23:38:55.000000 ttok-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-02 23:39:00.682115 ttok-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-02 23:38:55.000000 ttok-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:39:00.682115 ttok-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-02 23:38:55.000000 ttok-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:39:00.678115 ttok-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-02 23:38:55.000000 ttok-0.3/tests/test_ttok.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:39:00.682115 ttok-0.3/ttok/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:38:55.000000 ttok-0.3/ttok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 23:38:55.000000 ttok-0.3/ttok/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-02 23:38:55.000000 ttok-0.3/ttok/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:39:00.682115 ttok-0.3/ttok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-02 23:39:00.000000 ttok-0.3/ttok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 23:39:00.000000 ttok-0.3/ttok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:39:00.000000 ttok-0.3/ttok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 23:39:00.000000 ttok-0.3/ttok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 23:39:00.000000 ttok-0.3/ttok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 23:39:00.000000 ttok-0.3/ttok.egg-info/top_level.txt
```

### Comparing `ttok-0.2/LICENSE` & `ttok-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttok-0.2/setup.py` & `ttok-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.2"
+VERSION = "0.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `ttok-0.2/tests/test_ttok.py` & `ttok-0.3/tests/test_ttok.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,7 +90,20 @@
     runner = CliRunner()
     with runner.isolated_filesystem():
         with open("input.txt", "w") as f:
             f.write(file_input)
         result = runner.invoke(cli, args, **kwargs)
         assert result.exit_code == 0
         assert result.output.strip() == str(expected_count)
+
+
+def test_ttok_special_tokens():
+    # https://github.com/simonw/ttok/issues/13
+    runner = CliRunner()
+    # Without --allow-special raises an error
+    result = runner.invoke(cli, ["<|endoftext|>", "--encode"])
+    assert result.exit_code != 0
+    assert "Use --allow-special to allow special tokens" in result.output
+    # With --allow-special it works
+    result = runner.invoke(cli, ["<|endoftext|>", "--encode", "--allow-special"])
+    assert result.exit_code == 0
+    assert result.output.strip() == "100257"
```

### Comparing `ttok-0.2/ttok/cli.py` & `ttok-0.3/ttok/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,25 @@
 @click.option(
     "encode_tokens", "--encode", "--tokens", is_flag=True, help="Output token integers"
 )
 @click.option(
     "decode_tokens", "--decode", is_flag=True, help="Convert token integers to text"
 )
 @click.option("as_tokens", "--tokens", is_flag=True, help="Output full tokens")
-def cli(prompt, input, truncate, model, encode_tokens, decode_tokens, as_tokens):
+@click.option("--allow-special", is_flag=True, help="Do not error on special tokens")
+def cli(
+    prompt,
+    input,
+    truncate,
+    model,
+    encode_tokens,
+    decode_tokens,
+    as_tokens,
+    allow_special,
+):
     """
     Count and truncate text based on tokens
 
     To count tokens for text passed as arguments:
 
         ttok one two three
 
@@ -53,14 +63,18 @@
 
     Outputs:
 
         [b'hello', b' world']
     """
     if decode_tokens and encode_tokens:
         raise click.ClickException("Cannot use --decode with --encode")
+    if allow_special and not (encode_tokens or as_tokens):
+        raise click.ClickException(
+            "Cannot use --allow-special without --encode or --tokens"
+        )
     if as_tokens and not decode_tokens and not encode_tokens:
         encode_tokens = True
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError as e:
         raise click.ClickException(f"Invalid model: {model}") from e
     if not prompt and input is None:
@@ -78,15 +92,28 @@
         if as_tokens:
             click.echo(encoding.decode_tokens_bytes(tokens))
         else:
             click.echo(encoding.decode(tokens))
         return
 
     # Tokenize it
-    tokens = encoding.encode(text)
+    kwargs = {}
+    if allow_special:
+        kwargs["allowed_special"] = "all"
+    try:
+        tokens = encoding.encode(text, **kwargs)
+    except ValueError as ex:
+        ex_str = str(ex)
+        if "disallowed special token" in ex_str and not allow_special:
+            # Just the first line, then add a hint
+            ex_str = (
+                ex_str.split("\n")[0]
+                + "\n\nUse --allow-special to allow special tokens"
+            )
+        raise click.ClickException(ex_str)
     if truncate:
         tokens = tokens[:truncate]
 
     if encode_tokens:
         if as_tokens:
             click.echo(encoding.decode_tokens_bytes(tokens))
         else:
```

