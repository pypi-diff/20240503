# Comparing `tmp/cfn-review-bot-1!20240202.133301.tar.gz` & `tmp/cfn-review-bot-1!20240503.111248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-review-bot-1!20240202.133301.tar", last modified: Fri Feb  2 13:33:42 2024, max compression
+gzip compressed data, was "cfn-review-bot-1!20240503.111248.tar", last modified: Fri May  3 11:13:47 2024, max compression
```

## Comparing `cfn-review-bot-1!20240202.133301.tar` & `cfn-review-bot-1!20240503.111248.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/cfn_review_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3708 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/cfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/dirloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/package-version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/target.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/cfn_review_bot/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/templates/summary.md
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-02 13:33:42.000000 cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 13:33:42.146628 cfn-review-bot-1!20240202.133301/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-02 13:33:32.000000 cfn-review-bot-1!20240202.133301/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3708 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/cfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/dirloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/package-version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/templates/summary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 11:13:47.000000 cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:13:47.492259 cfn-review-bot-1!20240503.111248/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 11:13:37.000000 cfn-review-bot-1!20240503.111248/setup.py
```

### Comparing `cfn-review-bot-1!20240202.133301/LICENSE` & `cfn-review-bot-1!20240503.111248/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/PKG-INFO` & `cfn-review-bot-1!20240503.111248/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-review-bot
-Version: 1!20240202.133301
+Version: 1!20240503.111248
 Summary: CLI to manage CloudFormation stacks
 Home-page: https://github.com/biochimia/cfn-review-bot
 Author: João Abecasis
 Author-email: joao@abecasis.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/_version.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/_version.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/aws.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/aws.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/canonical.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/canonical.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/cfn.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/cfn.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,12 +213,12 @@
         start = datetime.datetime.now()
         while True:
             detail = self.cfn.describe_change_set(ChangeSetName=change_set.id)
             if detail['Status'] not in ['CREATE_PENDING', 'CREATE_IN_PROGRESS']:
                 change_set.detail = detail
                 return
 
-            if (datetime.datetime.now() - start).total_seconds() > 60:
+            if (datetime.datetime.now() - start).total_seconds() > 180:
                 raise TimeoutError(
                     f'Timeout waiting for change set {change_set.id} to become ready')
 
-            time.sleep(5)
+            time.sleep(15)
```

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/dirloader.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/dirloader.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/loader.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/loader.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/main.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/main.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/markdown.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/markdown.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/merge.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/merge.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/model.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/model.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/stack.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/stack.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/target.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/target.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/template.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/template.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/schema/test_stack.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/schema/test_stack.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/templates/summary.md` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/templates/summary.md`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot/test_merge.py` & `cfn-review-bot-1!20240503.111248/cfn_review_bot/test_merge.py`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/PKG-INFO` & `cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-review-bot
-Version: 1!20240202.133301
+Version: 1!20240503.111248
 Summary: CLI to manage CloudFormation stacks
 Home-page: https://github.com/biochimia/cfn-review-bot
 Author: João Abecasis
 Author-email: joao@abecasis.name
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfn-review-bot-1!20240202.133301/cfn_review_bot.egg-info/SOURCES.txt` & `cfn-review-bot-1!20240503.111248/cfn_review_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfn-review-bot-1!20240202.133301/setup.py` & `cfn-review-bot-1!20240503.111248/setup.py`

 * *Files identical despite different names*

