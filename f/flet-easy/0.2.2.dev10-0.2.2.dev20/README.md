# Comparing `tmp/flet_easy-0.2.2.dev10.tar.gz` & `tmp/flet_easy-0.2.2.dev20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy-0.2.2.dev10.tar", last modified: Thu Apr 25 02:33:54 2024, max compression
+gzip compressed data, was "flet_easy-0.2.2.dev20.tar", last modified: Fri May  3 15:54:31 2024, max compression
```

## Comparing `flet_easy-0.2.2.dev10.tar` & `flet_easy-0.2.2.dev20.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11541 2024-04-25 01:11:21.131137 flet_easy-0.2.2.dev10/LICENSE
--rw-r--r--   0        0        0    11541 2024-04-25 01:11:21.131137 flet_easy-0.2.2.dev10/LICENSE
--rw-r--r--   0        0        0     5794 2024-04-25 01:11:21.131137 flet_easy-0.2.2.dev10/README.md
--rw-r--r--   0        0        0     5794 2024-04-25 01:11:21.131137 flet_easy-0.2.2.dev10/README.md
--rw-r--r--   0        0        0     1909 2024-04-25 02:33:54.877892 flet_easy-0.2.2.dev10/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-25 01:11:21.244553 flet_easy-0.2.2.dev10/src/flet_easy/__init__.py
--rw-r--r--   0        0        0     1282 2024-04-25 01:11:21.244553 flet_easy-0.2.2.dev10/src/flet_easy/auto_route.py
--rw-r--r--   0        0        0     2356 2024-04-25 01:11:21.245552 flet_easy-0.2.2.dev10/src/flet_easy/cli/copy.py
--rw-r--r--   0        0        0     2105 2024-04-25 02:33:04.190065 flet_easy-0.2.2.dev10/src/flet_easy/cli/main.py
--rw-r--r--   0        0        0     3266 2024-04-25 01:11:21.247574 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/.gitignore
--rw-r--r--   0        0        0      213 2024-04-25 01:11:21.247574 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/README.md
--rw-r--r--   0        0        0     1020 2024-04-25 01:11:21.248581 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/favicon.png
--rw-r--r--   0        0        0    30189 2024-04-25 01:11:21.249571 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icon.png
--rw-r--r--   0        0        0     7610 2024-04-25 01:11:21.250567 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-192.png
--rw-r--r--   0        0        0    33055 2024-04-25 01:11:21.250567 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-512.png
--rw-r--r--   0        0        0     7610 2024-04-25 01:11:21.251570 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    33055 2024-04-25 01:11:21.252569 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    56474 2024-04-25 01:11:21.253573 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/loading-animation.png
--rw-r--r--   0        0        0     3626 2024-04-25 01:11:21.254090 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/index.html
--rw-r--r--   0        0        0      932 2024-04-25 01:11:21.255114 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/manifest.json
--rw-r--r--   0        0        0       84 2024-04-25 01:11:21.255114 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/components/__init__.py
--rw-r--r--   0        0        0     2422 2024-04-25 01:11:21.256137 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/components/counter.py
--rw-r--r--   0        0        0      543 2024-04-25 01:11:21.257134 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/components/swoDrawer.py
--rw-r--r--   0        0        0       45 2024-04-25 01:11:21.257134 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/controllers/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-25 01:11:21.258140 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/controllers/counter.py
--rw-r--r--   0        0        0        0 2024-04-25 01:11:21.258140 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/core/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-25 01:11:21.259136 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/core/config.py
--rw-r--r--   0        0        0      246 2024-04-25 01:11:21.259136 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/main.py
--rw-r--r--   0        0        0        0 2024-04-25 01:11:21.260137 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-25 01:11:21.261140 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/views/counter.py
--rw-r--r--   0        0        0      615 2024-04-25 01:11:21.261140 flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/views/index.py
--rw-r--r--   0        0        0    12208 2024-04-25 01:11:21.262139 flet_easy-0.2.2.dev10/src/flet_easy/datasy.py
--rw-r--r--   0        0        0      187 2024-04-25 01:11:21.262139 flet_easy-0.2.2.dev10/src/flet_easy/extra.py
--rw-r--r--   0        0        0     2483 2024-04-25 01:11:21.262139 flet_easy-0.2.2.dev10/src/flet_easy/extrasJwt.py
--rw-r--r--   0        0        0    18351 2024-04-25 01:11:21.263715 flet_easy-0.2.2.dev10/src/flet_easy/fletEasy.py
--rw-r--r--   0        0        0     9856 2024-04-25 01:11:21.264681 flet_easy-0.2.2.dev10/src/flet_easy/inheritance.py
--rw-r--r--   0        0        0     1191 2024-04-25 01:11:21.264681 flet_easy-0.2.2.dev10/src/flet_easy/job.py
--rw-r--r--   0        0        0     4024 2024-04-25 01:11:21.265679 flet_easy-0.2.2.dev10/src/flet_easy/jwt.py
--rw-r--r--   0        0        0     7512 2024-04-25 01:11:21.265679 flet_easy-0.2.2.dev10/src/flet_easy/pagesy.py
--rw-r--r--   0        0        0    11101 2024-04-25 02:32:56.957883 flet_easy-0.2.2.dev10/src/flet_easy/route.py
--rw-r--r--   0        0        0     1540 2024-04-25 01:11:21.266698 flet_easy-0.2.2.dev10/src/flet_easy/view_404.py
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 flet_easy-0.2.2.dev10/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-05-03 13:42:27.173525 flet_easy-0.2.2.dev20/LICENSE
+-rw-r--r--   0        0        0    11541 2024-05-03 13:42:27.173525 flet_easy-0.2.2.dev20/LICENSE
+-rw-r--r--   0        0        0     5794 2024-05-03 13:42:27.173525 flet_easy-0.2.2.dev20/README.md
+-rw-r--r--   0        0        0     5794 2024-05-03 13:42:27.173525 flet_easy-0.2.2.dev20/README.md
+-rw-r--r--   0        0        0     1909 2024-05-03 15:54:31.532514 flet_easy-0.2.2.dev20/pyproject.toml
+-rw-r--r--   0        0        0      432 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/__init__.py
+-rw-r--r--   0        0        0     1282 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/auto_route.py
+-rw-r--r--   0        0        0     2356 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/cli/copy.py
+-rw-r--r--   0        0        0     2105 2024-05-03 15:54:04.763357 flet_easy-0.2.2.dev20/src/flet_easy/cli/main.py
+-rw-r--r--   0        0        0     3266 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/.gitignore
+-rw-r--r--   0        0        0      213 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/README.md
+-rw-r--r--   0        0        0     1020 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/favicon.png
+-rw-r--r--   0        0        0    30189 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icon.png
+-rw-r--r--   0        0        0     7610 2024-05-03 13:42:27.284593 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-192.png
+-rw-r--r--   0        0        0    33055 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-512.png
+-rw-r--r--   0        0        0     7610 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    33055 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    56474 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/loading-animation.png
+-rw-r--r--   0        0        0     3626 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/index.html
+-rw-r--r--   0        0        0      932 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/manifest.json
+-rw-r--r--   0        0        0       84 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/components/__init__.py
+-rw-r--r--   0        0        0     2422 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/components/counter.py
+-rw-r--r--   0        0        0      543 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/components/swoDrawer.py
+-rw-r--r--   0        0        0       45 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/controllers/__init__.py
+-rw-r--r--   0        0        0     1258 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/controllers/counter.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:42:27.300249 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/core/__init__.py
+-rw-r--r--   0        0        0     1662 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/core/config.py
+-rw-r--r--   0        0        0      246 2024-05-03 15:51:57.553417 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/main.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/views/counter.py
+-rw-r--r--   0        0        0      615 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/views/index.py
+-rw-r--r--   0        0        0    12239 2024-05-03 15:53:51.404737 flet_easy-0.2.2.dev20/src/flet_easy/datasy.py
+-rw-r--r--   0        0        0      187 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/extra.py
+-rw-r--r--   0        0        0     2483 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/extrasJwt.py
+-rw-r--r--   0        0        0    18351 2024-05-03 13:42:27.308268 flet_easy-0.2.2.dev20/src/flet_easy/fletEasy.py
+-rw-r--r--   0        0        0     9856 2024-05-03 13:42:27.313818 flet_easy-0.2.2.dev20/src/flet_easy/inheritance.py
+-rw-r--r--   0        0        0     1191 2024-05-03 13:42:27.313818 flet_easy-0.2.2.dev20/src/flet_easy/job.py
+-rw-r--r--   0        0        0     4024 2024-05-03 13:42:27.313818 flet_easy-0.2.2.dev20/src/flet_easy/jwt.py
+-rw-r--r--   0        0        0     7512 2024-05-03 13:42:27.313818 flet_easy-0.2.2.dev20/src/flet_easy/pagesy.py
+-rw-r--r--   0        0        0    11178 2024-05-03 15:53:39.442826 flet_easy-0.2.2.dev20/src/flet_easy/route.py
+-rw-r--r--   0        0        0     1540 2024-05-03 13:42:27.316337 flet_easy-0.2.2.dev20/src/flet_easy/view_404.py
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 flet_easy-0.2.2.dev20/PKG-INFO
```

### Comparing `flet_easy-0.2.2.dev10/LICENSE` & `flet_easy-0.2.2.dev20/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/README.md` & `flet_easy-0.2.2.dev20/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/pyproject.toml` & `flet_easy-0.2.2.dev20/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flet-easy"
-version = "0.2.2.dev10"
+version = "0.2.2.dev20"
 description = "⚡Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features."
 authors = [
     { name = "Daxexs", email = "Daxexsdev@gmail.com" },
 ]
 dependencies = [
     "parse>=1.20.1",
     "pyJWT>=2.8.0",
```

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/auto_route.py` & `flet_easy-0.2.2.dev20/src/flet_easy/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/copy.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/copy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/main.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from rich.prompt import Prompt
 from rich_argparse import RichHelpFormatter
 from tomlkit import dump
 
 from .copy import _copy_template
 
-VERSION = "0.2.2.dev10"
+VERSION = "0.2.2.dev20"
 
 RichHelpFormatter.styles["argparse.text"] = "italic"
 RichHelpFormatter.styles["argparse.help"] = "light_sky_blue3"
 RichHelpFormatter.styles["argparse.prog"] = "blue"
 
 
 def init_app():
```

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/.gitignore` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/favicon.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icon.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-192.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-512.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/icons/loading-animation.png` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/index.html` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/index.html`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/assets/manifest.json` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/components/counter.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/components/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/components/swoDrawer.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/components/swoDrawer.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/controllers/counter.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/controllers/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/core/config.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/core/config.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/views/counter.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/views/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/cli/templates/views/index.py` & `flet_easy-0.2.2.dev20/src/flet_easy/cli/templates/views/index.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/datasy.py` & `flet_easy-0.2.2.dev20/src/flet_easy/datasy.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,16 @@
                 )
             )
         else:
             raise ValueError("Method not implemented in logout_init method.")
 
     def _create_login(self):
         """Create the connection between sessions."""
-        self.page.pubsub.subscribe_topic(self.page.client_ip, self.__logaut_init)
+        if self.page.web:
+            self.page.pubsub.subscribe_topic(self.page.client_ip, self.__logaut_init)
 
     def _create_tasks(self, time_expiry: timedelta, key: str, sleep: int) -> None:
         """Creates the logout task when logging in."""
         if time_expiry is not None:
             Job(
                 func=self.logout,
                 key=key,
```

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/extrasJwt.py` & `flet_easy-0.2.2.dev20/src/flet_easy/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/fletEasy.py` & `flet_easy-0.2.2.dev20/src/flet_easy/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/inheritance.py` & `flet_easy-0.2.2.dev20/src/flet_easy/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/job.py` & `flet_easy-0.2.2.dev20/src/flet_easy/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/jwt.py` & `flet_easy-0.2.2.dev20/src/flet_easy/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/pagesy.py` & `flet_easy-0.2.2.dev20/src/flet_easy/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/route.py` & `flet_easy-0.2.2.dev20/src/flet_easy/route.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,19 +57,15 @@
             secret_key=secret_key,
             auto_logout=auto_logout,
             page_on_keyboard=self.__page_on_keyboard,
             page_on_resize=self.__page_on_resize,
             login_async=iscoroutinefunction(self.__config_login),
             go=self._go,
         )
-        self.__data.view = (
-            self.__page.run_task(self.__view_data_config).result()
-            if self.__view_data is not None
-            else None
-        )
+        self.__data.view = self.__view_data_config() if self.__view_data is not None else None
         if self.__route_login is not None:
             self.__data._create_login()
 
     # ----------- Supports async
     def __route_change(self, e: RouteChangeEvent):
         if not self.__data._check_event_router:
             route = (
@@ -78,42 +74,42 @@
                 else e.route
             )
             self._go(route)
         self.__data._check_event_router = False
 
     def __view_pop(self, e):
         self.__page.views.pop()
-        top_view = self.__page.views[-1]
-        self._go(top_view.route)
+        route = self.__page.views[-1].route
         self.__page.views.pop()
+        self._go(route)
 
     async def __on_keyboard(self, e: KeyboardEvent):
         self.__page_on_keyboard.call = e
         if self.__page_on_keyboard._controls():
             await self.__page_on_keyboard._run_controls()
 
     def __page_resize(self, e: ControlEvent):
         self.__page_on_resize.e = e
 
-    async def __add_configuration_start(self):
+    def __add_configuration_start(self):
         """Add general settings to the pages."""
         if self.__view_config:
             if iscoroutinefunction(self.__view_config):
-                await self.__view_config(self.__page)
+                self.__page.run_task(self.__view_config, self.__page).result()
             else:
                 self.__view_config(self.__page)
 
         if self.__config_event:
             if iscoroutinefunction(self.__config_event):
-                await self.__config_event(self.__data)
+                self.__page.run_task(self.__config_event, self.__data).result()
             else:
                 self.__config_event(self.__data)
 
     def __disconnect(self, e):
-        if self.__data._login_done:
+        if self.__data._login_done and self.__page.web:
             self.__page.pubsub.send_others_on_topic(
                 self.__page.client_ip,
                 Msg("updateLoginSessions", value=self.__data._login_done),
             )
 
     # -- initialization
 
@@ -121,15 +117,15 @@
         if self.__route_init != "/" and self.__page.route == "/":
             self.__page.route = self.__route_init
 
         if len(self.__page.views) == 1:
             self.__page.views.clear()
 
         """ Add custom events """
-        self.__page.run_task(self.__add_configuration_start)
+        self.__add_configuration_start()
 
         """ Executing charter events """
         self.__page.on_route_change = self.__route_change
         self.__page.on_view_pop = self.__view_pop
         self.__page.on_error = lambda e: print("Page error:", e.data)
         self.__page.on_disconnect = self.__disconnect
 
@@ -138,25 +134,25 @@
             self.__page.on_resize = self.__page_resize
         if self.__on_Keyboard:
             self.__page.on_keyboard_event = self.__on_keyboard
 
         self._go(self.__page.route)
 
     # ---------------------------[Route controller]-------------------------------------
-    async def __view_data_config(self):
+    def __view_data_config(self):
         """Add the `View` configuration, to reuse on every page."""
         if iscoroutinefunction(self.__view_data):
-            return await self.__view_data(self.__data)
+            return self.__page.run_task(self.__view_data, self.__data).result()
         else:
             return self.__view_data(self.__data)
 
-    async def _view_append(self, route: str):
+    def _view_append(self, route: str):
         """Add a new page and update it."""
         view = (
-            await self.__pagesy.view(self.__data, **self.__data.url_params)
+            self.__page.run_task(self.__pagesy.view, self.__data, **self.__data.url_params).result()
             if iscoroutinefunction(self.__pagesy.view)
             else self.__pagesy.view(self.__data, **self.__data.url_params)
         )
 
         view.route = route
         self.__page.views.append(view)
         self.__page.route = route
@@ -198,15 +194,15 @@
 
                     if not res_middleware:
                         raise Exception(
                             "A middleware function has occurred, use the methods to return (data.redirect) or not return False."
                         )
             if self.__pagesy.middleware is None or _middlewares_two:
                 self.__reload_datasy(url_params)
-                self.__page.run_task(self._view_append, route)
+                self._view_append(route)
                 return False
             else:
                 _middlewares = self.__pagesy.middleware
                 _middlewares_two = True
 
     def __process_route(self, custom_params: Dict[str, Callable[[], bool]], path: str, route: str):
         if custom_params is None:
@@ -240,38 +236,40 @@
         for page in self.__pages:
             route_math, route_check = self.__process_route(page.custom_params, path, page.route)
             if route_check:
                 pg_404 = False
                 self.__pagesy = page
                 try:
                     if page.protected_route:
+                        assert (
+                            self.__route_login is not None
+                        ), "Configure the route of the login page, in the Flet-Easy class in the parameter (route_login)"
+
                         if iscoroutinefunction(self.__config_login):
                             try:
                                 auth = self.__page.run_task(
                                     self.__config_login, self.__data
                                 ).result()
                             except Exception as e:
                                 raise Exception(
                                     "Use async methods in the function decorated by 'login', to avoid conflicts.",
                                     e,
                                 )
                         else:
                             auth = self.__config_login(self.__data)
                         if auth:
                             self.__reload_datasy(route_math.named)
-                            self.__page.run_task(self._view_append, route).result()
-                            break
+                            self._view_append(route)
                         else:
                             self._go(self.__route_login)
                             break
                     else:
-                        response = self.__run_middlewares(
+                        if self.__run_middlewares(
                             route=route, middleware=self.__middlewares, url_params=route_math.named
-                        )
-                        if not response:
+                        ):
                             break
                 except Exception as e:
                     raise Exception(e)
         if pg_404:
             if self.__page_404:
                 self.__pagesy = self.__page_404
                 self.__page.route = self.__page_404
```

### Comparing `flet_easy-0.2.2.dev10/src/flet_easy/view_404.py` & `flet_easy-0.2.2.dev20/src/flet_easy/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.2.dev10/PKG-INFO` & `flet_easy-0.2.2.dev20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-easy
-Version: 0.2.2.dev10
+Version: 0.2.2.dev20
 Summary: ⚡Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
 Keywords: flet easy,flet,python,flet easy route,python web template,app python,flet mvc,flet easy mvc,flet easy fastapi,flutter python,web application,fast flet
 Author-Email: Daxexs <Daxexsdev@gmail.com>
 License: apache-2.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

