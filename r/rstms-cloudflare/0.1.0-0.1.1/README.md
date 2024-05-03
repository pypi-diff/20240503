# Comparing `tmp/rstms_cloudflare-0.1.0.tar.gz` & `tmp/rstms_cloudflare-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_cloudflare-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_cloudflare-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_cloudflare-0.1.0.tar` & `rstms_cloudflare-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      383 2024-04-16 03:27:18.236141 rstms_cloudflare-0.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1338 2024-04-16 03:08:46.809802 rstms_cloudflare-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-0.1.0/LICENSE
--rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-0.1.0/Makefile
--rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-0.1.0/README.md
--rw-r--r--   0        0        0        6 2024-04-16 03:27:18.236141 rstms_cloudflare-0.1.0/VERSION
--rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.0/docs/Makefile
--rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.0/docs/cli.rst
--rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.0/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.0/docs/contributing.rst
--rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.0/docs/index.rst
--rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.0/docs/installation.rst
--rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-0.1.0/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.0/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-0.1.0/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-0.1.0/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.0/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.0/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-0.1.0/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-16 03:08:46.821802 rstms_cloudflare-0.1.0/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-0.1.0/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.0/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.0/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-0.1.0/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.0/make/version.mk
--rw-r--r--   0        0        0     1159 2024-04-16 03:27:18.236141 rstms_cloudflare-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-0.1.0/pytest.ini
--rw-r--r--   0        0        0       97 2024-04-16 03:27:18.076143 rstms_cloudflare-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-04-16 03:27:18.140142 rstms_cloudflare-0.1.0/requirements-docs.txt
--rw-r--r--   0        0        0       19 2024-04-16 03:27:18.004144 rstms_cloudflare-0.1.0/requirements.txt
--rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-0.1.0/rstms_cloudflare/__init__.py
--rw-r--r--   0        0        0     5526 2024-04-16 03:19:45.677822 rstms_cloudflare-0.1.0/rstms_cloudflare/cli.py
--rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-0.1.0/rstms_cloudflare/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-0.1.0/rstms_cloudflare/shell.py
--rw-r--r--   0        0        0      127 2024-04-16 03:27:18.236141 rstms_cloudflare-0.1.0/rstms_cloudflare/version.py
--rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-0.1.0/tests/test_cli.py
--rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-0.1.0/tox.ini
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      383 2024-05-03 02:00:28.943188 rstms_cloudflare-0.1.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1338 2024-04-16 03:08:46.809802 rstms_cloudflare-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-16 03:08:46.805802 rstms_cloudflare-0.1.1/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-16 03:08:46.809802 rstms_cloudflare-0.1.1/Makefile
+-rw-r--r--   0        0        0      689 2024-04-16 03:08:46.817802 rstms_cloudflare-0.1.1/README.md
+-rw-r--r--   0        0        0        6 2024-05-03 02:00:28.943188 rstms_cloudflare-0.1.1/VERSION
+-rw-r--r--   0        0        0      617 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0       97 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.1/docs/cli.rst
+-rwxr-xr-x   0        0        0     4960 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-16 03:08:46.889801 rstms_cloudflare-0.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0      300 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0     1174 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.1/docs/installation.rst
+-rw-r--r--   0        0        0      778 2024-04-16 03:08:46.877802 rstms_cloudflare-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-16 03:08:46.873802 rstms_cloudflare-0.1.1/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.1/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-16 03:08:46.845802 rstms_cloudflare-0.1.1/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-16 03:08:46.837802 rstms_cloudflare-0.1.1/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.1/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.1/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-16 03:08:46.825802 rstms_cloudflare-0.1.1/make/docs.mk
+-rw-r--r--   0        0        0      610 2024-04-16 03:08:46.821802 rstms_cloudflare-0.1.1/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-16 03:08:46.825802 rstms_cloudflare-0.1.1/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.1/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-16 03:08:46.829802 rstms_cloudflare-0.1.1/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-16 03:08:46.821802 rstms_cloudflare-0.1.1/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-16 03:08:46.833802 rstms_cloudflare-0.1.1/make/version.mk
+-rw-r--r--   0        0        0     1159 2024-05-03 02:00:28.943188 rstms_cloudflare-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-16 03:08:46.789803 rstms_cloudflare-0.1.1/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-03 02:00:28.671191 rstms_cloudflare-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-03 02:00:28.755190 rstms_cloudflare-0.1.1/requirements-docs.txt
+-rw-r--r--   0        0        0       19 2024-05-03 02:00:28.591192 rstms_cloudflare-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      217 2024-04-16 03:18:17.194893 rstms_cloudflare-0.1.1/rstms_cloudflare/__init__.py
+-rw-r--r--   0        0        0     5633 2024-05-03 02:00:33.767135 rstms_cloudflare-0.1.1/rstms_cloudflare/cli.py
+-rw-r--r--   0        0        0     1065 2024-04-16 03:11:31.499807 rstms_cloudflare-0.1.1/rstms_cloudflare/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-16 03:11:31.507807 rstms_cloudflare-0.1.1/rstms_cloudflare/shell.py
+-rw-r--r--   0        0        0      127 2024-05-03 02:00:28.943188 rstms_cloudflare-0.1.1/rstms_cloudflare/version.py
+-rw-r--r--   0        0        0       46 2024-04-16 03:08:46.849802 rstms_cloudflare-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-16 03:11:31.547806 rstms_cloudflare-0.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0      432 2024-04-16 03:08:46.789803 rstms_cloudflare-0.1.1/tox.ini
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rstms_cloudflare-0.1.1/PKG-INFO
```

### Comparing `rstms_cloudflare-0.1.0/.gitignore` & `rstms_cloudflare-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/LICENSE` & `rstms_cloudflare-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/Makefile` & `rstms_cloudflare-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/README.md` & `rstms_cloudflare-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/docs/Makefile` & `rstms_cloudflare-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/docs/conf.py` & `rstms_cloudflare-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/docs/installation.rst` & `rstms_cloudflare-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/docs/make.bat` & `rstms_cloudflare-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/clean.mk` & `rstms_cloudflare-0.1.1/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/common.mk` & `rstms_cloudflare-0.1.1/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/docs.mk` & `rstms_cloudflare-0.1.1/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/lint.mk` & `rstms_cloudflare-0.1.1/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/publish.mk` & `rstms_cloudflare-0.1.1/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/release.mk` & `rstms_cloudflare-0.1.1/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/test.mk` & `rstms_cloudflare-0.1.1/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/make/version.mk` & `rstms_cloudflare-0.1.1/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/pyproject.toml` & `rstms_cloudflare-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-cloudflare"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_cloudflare"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_cloudflare-0.1.0/rstms_cloudflare/cli.py` & `rstms_cloudflare-0.1.1/rstms_cloudflare/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,34 +177,41 @@
         if not context.quiet:
             click.echo(ret["id"])
 
 
 @cli.command
 @click.option("-p", "--priority")
 @click.argument("domain")
-@click.argument("type", type=click.Choice(RECORD_TYPES))
+@click.argument("type", type=click.Choice(RECORD_TYPES + ["ID"]))
 @click.argument("name")
 @click.pass_obj
 def delete(context, domain, type, name, priority):
     records = get_zone_records(context, domain)
-    name = parse_name(name, domain)
+    hostname = parse_name(name, domain)
 
     for record in records:
-        if record["type"] == type and record["name"] == name:
+        if type == "ID":
+            if name != record["id"]:
+                continue
+        elif type == record["type"] and hostname == record["name"]:
             if priority and (priority != record.get("priority", None)):
                 continue
-            zone_id = record["zone_id"]
-            record_id = record["id"]
-            ret = context.client.zones.dns_records.delete(zone_id, record_id)
-            if context.json:
-                click.echo(json.dumps(ret))
-            else:
-                if not context.quiet:
-                    click.echo(ret["id"])
-            sys.exit(0)
+        else:
+            continue
+        record_id = record["id"]
+        zone_id = record["zone_id"]
+        ret = context.client.zones.dns_records.delete(zone_id, record_id)
+        if context.json:
+            click.echo(json.dumps(ret))
+        else:
+            if not context.quiet:
+                click.echo(ret["id"])
+        sys.exit(0)
+
     if not context.quiet:
         fail("record not found")
+
     sys.exit(-1)
 
 
 if __name__ == "__main__":
     sys.exit(cli())
```

### Comparing `rstms_cloudflare-0.1.0/rstms_cloudflare/exception_handler.py` & `rstms_cloudflare-0.1.1/rstms_cloudflare/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/rstms_cloudflare/shell.py` & `rstms_cloudflare-0.1.1/rstms_cloudflare/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/tests/test_cli.py` & `rstms_cloudflare-0.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_cloudflare-0.1.0/PKG-INFO` & `rstms_cloudflare-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-cloudflare
-Version: 0.1.0
+Version: 0.1.1
 Summary: Top-level package for rstms-cloudflare.
 Keywords: rstms_cloudflare
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

