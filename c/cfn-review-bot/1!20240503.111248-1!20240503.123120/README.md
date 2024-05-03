# Comparing `tmp/cfn-review-bot-1!20240503.111248.tar.gz` & `tmp/cfn-review-bot-1!20240503.123120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-review-bot-1!20240503.111248.tar", last modified: Fri May  3 11:13:47 2024, max compression
+gzip compressed data, was "cfn-review-bot-1!20240503.123120.tar", last modified: Fri May  3 12:32:07 2024, max compression
```

## Comparing `cfn-review-bot-1!20240503.111248.tar` & `cfn-review-bot-1!20240503.123120.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3708 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/cfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/dirloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/package-version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/templates/summary.md
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:32:07.494011 cfn-review-bot-1!20240503.123120/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 12:32:07.494011 cfn-review-bot-1!20240503.123120/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:32:07.490012 cfn-review-bot-1!20240503.123120/cfn_review_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3842 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/cfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/dirloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/package-version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:32:07.490012 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:32:07.494011 cfn-review-bot-1!20240503.123120/cfn_review_bot/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/templates/summary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:32:07.490012 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 12:32:07.000000 cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:32:07.494011 cfn-review-bot-1!20240503.123120/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 12:31:58.000000 cfn-review-bot-1!20240503.123120/setup.py
```

### Comparing `cfn-review-bot-1!20240503.111248/LICENSE` & `cfn-review-bot-1!20240503.123120/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/PKG-INFO` & `cfn-review-bot-1!20240503.123120/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-review-bot
-Version: 1!20240503.111248
+Version: 1!20240503.123120
 Summary: CLI to manage CloudFormation stacks
 Home-page: https://github.com/biochimia/cfn-review-bot
 Author: João Abecasis
 Author-email: joao@abecasis.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/_version.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return git_output.strip().decode()
 
 
 def _get_git_timestamp():
     git_output = subprocess.check_output(
         'git log -1 --date=unix --format=format:%cd'.split(),
         stderr=subprocess.DEVNULL, stdin=subprocess.DEVNULL)
-    return datetime.datetime.utcfromtimestamp(int(git_output))
+    return datetime.datetime.fromtimestamp(int(git_output), datetime.timezone.utc)
 
 
 def get_version_info():
     try:
         return _get_version_info_from_package()
     except FileNotFoundError:
         pass
@@ -102,13 +102,16 @@
     with open(PACKAGE_VERSION_FILE, mode='w') as f:
         json.dump(vi._asdict(), f, ensure_ascii=True, indent=2, sort_keys=True)
     return vi
 
 
 if __name__ == '__main__':
     version = get_version_info()
+
     print(f'cfn-review-bot version {version.package_version} (git: {version.git_revision})')
+
     if 'github-action' in sys.argv:
-        print(
-            '\n'
-            f'::set-output name=package_version::{version.package_version}\n'
-            f'::set-output name=git_revision::{version.git_revision}')
+        outfile = os.environ.get('GITHUB_OUTPUT', sys.stdout.fileno())
+        with open(outfile, 'a', closefd=not isinstance(outfile, int)) as out:
+            out.write(
+                f'package_version={version.package_version}\n'
+                f'git_revision={version.git_revision}\n')
```

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/aws.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/aws.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/canonical.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/canonical.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/cfn.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/cfn.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/dirloader.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/dirloader.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/loader.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/loader.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/main.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/main.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/markdown.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/markdown.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/merge.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/merge.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/model.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/model.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/stack.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/stack.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/target.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/target.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/template.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/template.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/test_stack.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/schema/test_stack.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/templates/summary.md` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/templates/summary.md`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot/test_merge.py` & `cfn-review-bot-1!20240503.123120/cfn_review_bot/test_merge.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/PKG-INFO` & `cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-review-bot
-Version: 1!20240503.111248
+Version: 1!20240503.123120
 Summary: CLI to manage CloudFormation stacks
 Home-page: https://github.com/biochimia/cfn-review-bot
 Author: João Abecasis
 Author-email: joao@abecasis.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/SOURCES.txt` & `cfn-review-bot-1!20240503.123120/cfn_review_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240503.111248/setup.py` & `cfn-review-bot-1!20240503.123120/setup.py`

 * *Files identical despite different names*

