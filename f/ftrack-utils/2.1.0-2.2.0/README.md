# Comparing `tmp/ftrack_utils-2.1.0.tar.gz` & `tmp/ftrack_utils-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_utils-2.1.0.tar", max compression
+gzip compressed data, was "ftrack_utils-2.2.0.tar", max compression
```

## Comparing `ftrack_utils-2.1.0.tar` & `ftrack_utils-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0    10176 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0      154 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/README.md
--rw-r--r--   0        0        0      783 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      353 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/__init__.py
--rw-r--r--   0        0        0      251 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/__init__.py
--rw-r--r--   0        0        0      992 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/asynchronous.py
--rw-r--r--   0        0        0     1133 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/session.py
--rw-r--r--   0        0        0     5652 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/track_usage.py
--rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/directories/__init__.py
--rw-r--r--   0        0        0      514 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/directories/scan_dir.py
--rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/__init__.py
--rw-r--r--   0        0        0      349 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/environment.py
--rw-r--r--   0        0        0     1708 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/overrides.py
--rw-r--r--   0        0        0     5712 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/registry.py
--rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/__init__.py
--rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/config/__init__.py
--rw-r--r--   0        0        0     4843 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/config/tool.py
--rw-r--r--   0        0        0      270 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/remote.py
--rw-r--r--   0        0        0      980 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/json/__init__.py
--rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/modules/__init__.py
--rw-r--r--   0        0        0      698 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/modules/scan_modules.py
--rw-r--r--   0        0        0     1624 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/paths/__init__.py
--rw-r--r--   0        0        0      191 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/server/__init__.py
--rw-r--r--   0        0        0      996 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/server/send_event.py
--rw-r--r--   0        0        0      633 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/server/track_usage.py
--rw-r--r--   0        0        0     1863 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/string/__init__.py
--rw-r--r--   0        0        0      661 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/threading/__init__.py
--rw-r--r--   0        0        0      111 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/usage/__init__.py
--rw-r--r--   0        0        0     2239 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/usage/track_usage.py
--rw-r--r--   0        0        0     1639 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/version/__init__.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 ftrack_utils-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/README.md
+-rw-r--r--   0        0        0      783 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      353 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/__init__.py
+-rw-r--r--   0        0        0      251 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/decorators/__init__.py
+-rw-r--r--   0        0        0      992 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/decorators/asynchronous.py
+-rw-r--r--   0        0        0     1133 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/decorators/session.py
+-rw-r--r--   0        0        0     5652 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/decorators/track_usage.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/directories/__init__.py
+-rw-r--r--   0        0        0      514 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/directories/scan_dir.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/extensions/__init__.py
+-rw-r--r--   0        0        0      349 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/extensions/environment.py
+-rw-r--r--   0        0        0     2544 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/extensions/overrides.py
+-rw-r--r--   0        0        0     5712 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/extensions/registry.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/framework/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/framework/config/__init__.py
+-rw-r--r--   0        0        0     4843 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/framework/config/tool.py
+-rw-r--r--   0        0        0      270 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/framework/remote.py
+-rw-r--r--   0        0        0      980 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/json/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/modules/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/modules/scan_modules.py
+-rw-r--r--   0        0        0     1624 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/paths/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/process/__init__.py
+-rw-r--r--   0        0        0     1875 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/process/monitor.py
+-rw-r--r--   0        0        0      108 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/rpc/__init__.py
+-rw-r--r--   0        0        0    10392 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/rpc/js_rpc.py
+-rw-r--r--   0        0        0      191 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/server/__init__.py
+-rw-r--r--   0        0        0      996 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/server/send_event.py
+-rw-r--r--   0        0        0      633 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/server/track_usage.py
+-rw-r--r--   0        0        0     1863 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/string/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/threading/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/usage/__init__.py
+-rw-r--r--   0        0        0     2239 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/usage/track_usage.py
+-rw-r--r--   0        0        0     1639 2024-05-02 08:05:11.806332 ftrack_utils-2.2.0/source/ftrack_utils/version/__init__.py
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 ftrack_utils-2.2.0/PKG-INFO
```

### Comparing `ftrack_utils-2.1.0/LICENSE.txt` & `ftrack_utils-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/pyproject.toml` & `ftrack_utils-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-utils"
-version = "2.1.0"
+version = "2.2.0"
 description='ftrack utils library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_utils", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/utils"
```

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/decorators/asynchronous.py` & `ftrack_utils-2.2.0/source/ftrack_utils/decorators/asynchronous.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/decorators/session.py` & `ftrack_utils-2.2.0/source/ftrack_utils/decorators/session.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/decorators/track_usage.py` & `ftrack_utils-2.2.0/source/ftrack_utils/decorators/track_usage.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/directories/scan_dir.py` & `ftrack_utils-2.2.0/source/ftrack_utils/directories/scan_dir.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/extensions/overrides.py` & `ftrack_utils-2.2.0/source/ftrack_utils/extensions/overrides.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,22 +11,35 @@
     return root_extension_dict.update(override_dict)
 
 
 def set_overrides(current_extensions, new_extensions):
     '''If new extension from *new_extensions* found in *current_extensions* do a first level merge'''
     for new_extension in new_extensions:
         existing_extension = None
-        for discovered_extension in current_extensions:
+        idx = None
+        for idx, discovered_extension in enumerate(current_extensions):
             if (
                 discovered_extension['extension_type']
                 == new_extension['extension_type']
                 and discovered_extension['name'] == new_extension['name']
             ):
                 existing_extension = discovered_extension
                 break
+            elif not new_extension['extension_type'].endswith('_config'):
+                # Handle corner cases of dialogs plugins and widgets when name
+                # is not the same but class name is the same, then we need to
+                # override as well.
+                if (
+                    discovered_extension['extension_type']
+                    == new_extension['extension_type']
+                    and discovered_extension['extension'].__name__
+                    == new_extension['extension'].__name__
+                ):
+                    existing_extension = discovered_extension
+                    break
         if not existing_extension:
             # Add to discovered extensions
             current_extensions.append(new_extension)
         else:
             # Can we merge?
             if new_extension['extension_type'].endswith('_config'):
                 logging.info(
@@ -34,8 +47,11 @@
                     f' {existing_extension["path"]}) on top of {new_extension["name"]}({new_extension["extension_type"]}'
                     f' @ {new_extension["path"]}).'
                 )
                 # Have the latter extension be overridden by the former
                 first_level_merge(
                     existing_extension['extension'], new_extension['extension']
                 )
+            else:
+                # Make sure we replace the previous discovered extensions with the new one.
+                current_extensions[idx] = new_extension
     return current_extensions
```

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/extensions/registry.py` & `ftrack_utils-2.2.0/source/ftrack_utils/extensions/registry.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/framework/config/tool.py` & `ftrack_utils-2.2.0/source/ftrack_utils/framework/config/tool.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/json/__init__.py` & `ftrack_utils-2.2.0/source/ftrack_utils/json/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/modules/scan_modules.py` & `ftrack_utils-2.2.0/source/ftrack_utils/modules/scan_modules.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/paths/__init__.py` & `ftrack_utils-2.2.0/source/ftrack_utils/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/server/send_event.py` & `ftrack_utils-2.2.0/source/ftrack_utils/server/send_event.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/server/track_usage.py` & `ftrack_utils-2.2.0/source/ftrack_utils/server/track_usage.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/string/__init__.py` & `ftrack_utils-2.2.0/source/ftrack_utils/string/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/threading/__init__.py` & `ftrack_utils-2.2.0/source/ftrack_utils/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/usage/track_usage.py` & `ftrack_utils-2.2.0/source/ftrack_utils/usage/track_usage.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/source/ftrack_utils/version/__init__.py` & `ftrack_utils-2.2.0/source/ftrack_utils/version/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.1.0/PKG-INFO` & `ftrack_utils-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-utils
-Version: 2.1.0
+Version: 2.2.0
 Summary: ftrack utils library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

