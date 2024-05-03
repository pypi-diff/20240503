# Comparing `tmp/xmonkey_namonica-0.1.5.tar.gz` & `tmp/xmonkey_namonica-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.5.tar", last modified: Thu May  2 01:23:40 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.6.tar", last modified: Thu May  2 08:05:23 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.5.tar` & `xmonkey_namonica-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.678223 xmonkey_namonica-0.1.5/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.5/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-02 01:23:40.678062 xmonkey_namonica-0.1.5/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1966 2024-04-29 20:51:13.000000 xmonkey_namonica-0.1.5/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-02 01:23:40.678255 xmonkey_namonica-0.1.5/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      343 2024-05-02 01:22:54.000000 xmonkey_namonica-0.1.5/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.674326 xmonkey_namonica-0.1.5/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2265 2024-05-01 21:38:26.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3953 2024-05-02 01:18:35.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.677564 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4011 2024-04-29 20:48:00.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/gen_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3696 2024-04-28 18:23:26.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/github_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5113 2024-05-02 01:21:48.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/golang_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.5/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 01:23:40.677899 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      752 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-02 01:23:40.000000 xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 08:05:23.898533 xmonkey_namonica-0.1.6/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.6/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-02 08:05:23.898327 xmonkey_namonica-0.1.6/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2203 2024-05-02 08:01:20.000000 xmonkey_namonica-0.1.6/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-02 08:05:23.898571 xmonkey_namonica-0.1.6/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      343 2024-05-02 08:04:57.000000 xmonkey_namonica-0.1.6/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 08:05:23.896203 xmonkey_namonica-0.1.6/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2383 2024-05-02 07:11:50.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3953 2024-05-02 06:31:44.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 08:05:23.897997 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2159 2024-05-02 07:58:12.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5119 2024-05-02 08:04:00.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/gem_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4022 2024-05-02 07:58:07.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/gen_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3707 2024-05-02 07:58:03.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/github_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5124 2024-05-02 07:57:56.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/golang_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2211 2024-05-02 07:57:50.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2159 2024-05-02 07:57:46.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2229 2024-05-02 07:57:36.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.6/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-02 08:05:23.898147 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-05-02 08:05:23.000000 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      793 2024-05-02 08:05:23.000000 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-02 08:05:23.000000 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-02 08:05:23.000000 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-02 08:05:23.000000 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-02 08:05:23.000000 xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.5/LICENSE` & `xmonkey_namonica-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.5/README.md` & `xmonkey_namonica-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -50,19 +50,31 @@
 ### Cargo (RUST)
 Sample Cargo purl is provided below:
 
 ```
 xmonkey-namonica "pkg:cargo/grin@1.0.0?type=crate"
 ```
 
+### Golang (Go)
+Sample Golang purl is provided below:
+
+```
+xmonkey-namonica "pkg:golang/github.com/mailru/easyjson@v0.7.7"
+```
+
+### Gem (Ruby)
+Sample Ruby purl is provided below:
+
+```
+xmonkey-namonica "pkg:gem/jruby-launcher@1.1.18?platform=java"
+```
+
 ### Work in Progress:
 * Maven (*)
 * RPM
-* gem
-* Golang
 * Conan
 * Conda
 * Bower
 * Composer
 * Cran
 * Cocoapods
 * Swift
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .handlers.npm_handler import NpmHandler
 from .handlers.cargo_handler import CargoHandler
 from .handlers.pypi_handler import PypiHandler
 from .handlers.nuget_handler import NugetHandler
 from .handlers.gen_handler import GenericHandler
 from .handlers.github_handler import GithubHandler
 from .handlers.golang_handler import GolangHandler
+from .handlers.gem_handler import GemHandler
 
 
 def main():
     parser = argparse.ArgumentParser(description="Package Analyzer Tool")
     parser.add_argument("purl", type=str, help="Package URL to process")
     parser.add_argument(
         "--export", type=str,
@@ -29,14 +30,16 @@
         handler = CargoHandler(args.purl)
     elif "pkg:pypi" in args.purl:
         handler = PypiHandler(args.purl)
     elif "pkg:nuget" in args.purl:
         handler = NugetHandler(args.purl)
     elif "pkg:golang" in args.purl:
         handler = GolangHandler(args.purl)
+    elif "pkg:gem" in args.purl:
+        handler = GemHandler(args.purl)
     elif "pkg:generic" in args.purl:
         handler = GenericHandler(args.purl)
     elif "pkg:github" in args.purl:
         handler = GithubHandler(args.purl)
     else:
         raise ValueError("Unsupported PURL type")
     handler.fetch()
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/common.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/cargo_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/npm_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
 from ..utils import download_file, temp_directory, extract_tar
 
 
-class CargoHandler(BaseHandler):
+class NpmHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
                 f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
-            logging.info(f"Downloaded package in {self.temp_dir}")
+            logging.info(f"Downloaded package to {package_file_path}")
             self.temp_dir = temp_dir
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
@@ -36,29 +36,30 @@
             extract_tar(package_file_path, self.temp_dir)
             logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
     def construct_download_url(self):
         namespace = (
-            self.purl_details['namespace'].replace('%40', '@')
+            self.purl_details['namespace'].replace('%40', '@') + '/' +
+            self.purl_details['name']
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
         return (
-            f"https://crates.io/api/v1/crates/"
-            f"{self.purl_details['name']}/"
-            f"{self.purl_details['version']}/download"
+            f"https://registry.npmjs.org/"
+            f"{namespace}/-/"
+            f"{self.purl_details['name']}-{self.purl_details['version']}.tgz"
         )
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/gen_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/gen_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 logging.error(f"Error unpacking file in {self.temp_dir}")
                 exit()
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/github_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/github_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 logging.error(f"Error unpacking file in {self.temp_dir}")
                 exit()
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/golang_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/golang_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 logging.error(f"Error unpacking file in {self.temp_dir}")
                 exit()
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/cargo_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
 from ..utils import download_file, temp_directory, extract_tar
 
 
-class NpmHandler(BaseHandler):
+class CargoHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
                 f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
-            logging.info(f"Downloaded package to {package_file_path}")
+            logging.info(f"Downloaded package in {self.temp_dir}")
             self.temp_dir = temp_dir
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
@@ -36,30 +36,29 @@
             extract_tar(package_file_path, self.temp_dir)
             logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
         logging.info("Generating report based on the scanned data...")
         return self.results
 
     def construct_download_url(self):
         namespace = (
-            self.purl_details['namespace'].replace('%40', '@') + '/' +
-            self.purl_details['name']
+            self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
         return (
-            f"https://registry.npmjs.org/"
-            f"{namespace}/-/"
-            f"{self.purl_details['name']}-{self.purl_details['version']}.tgz"
+            f"https://crates.io/api/v1/crates/"
+            f"{self.purl_details['name']}/"
+            f"{self.purl_details['version']}/download"
         )
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-from ..utils import download_file, temp_directory, extract_zip
+from ..utils import download_file, temp_directory, extract_tar
 
 
-class NugetHandler(BaseHandler):
+class PypiHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.zip"
+                f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
             logging.info(f"Downloaded package to {package_file_path}")
@@ -23,28 +23,28 @@
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.zip"
+                f"{self.purl_details['version']}.tgz"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
-            extract_zip(package_file_path, self.temp_dir)
+            extract_tar(package_file_path, self.temp_dir)
             logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
@@ -53,12 +53,13 @@
 
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
+        iniName = namespace[0].lower()
         return (
-            f"https://www.nuget.org/api/v2/package/"
-            f"{self.purl_details['name']}/"
-            f"{self.purl_details['version']}"
+            f"https://pypi.python.org/packages/source/{iniName}/{namespace}/"
+            f"{self.purl_details['name']}-"
+            f"{self.purl_details['version']}.tar.gz"
         )
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import logging
 from .base_handler import BaseHandler
 from ..common import PackageManager, temp_directory
-from ..utils import download_file, temp_directory, extract_tar
+from ..utils import download_file, temp_directory, extract_zip
 
 
-class PypiHandler(BaseHandler):
+class NugetHandler(BaseHandler):
     def fetch(self):
         download_url = self.construct_download_url()
         with temp_directory() as temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.tgz"
+                f"{self.purl_details['version']}.zip"
             )
             package_file_path = os.path.join(
                 temp_dir,
                 filename
             )
             download_file(download_url, package_file_path)
             logging.info(f"Downloaded package to {package_file_path}")
@@ -23,28 +23,28 @@
             self.unpack()
             self.scan()
 
     def unpack(self):
         if self.temp_dir:
             filename = (
                 f"{self.purl_details['name']}-"
-                f"{self.purl_details['version']}.tgz"
+                f"{self.purl_details['version']}.zip"
             )
             package_file_path = os.path.join(
                 self.temp_dir,
                 filename
             )
-            extract_tar(package_file_path, self.temp_dir)
+            extract_zip(package_file_path, self.temp_dir)
             logging.info(f"Unpacked package in {self.temp_dir}")
 
     def scan(self):
         results = {}
         logging.info("Scanning package contents...")
         files = PackageManager.scan_for_files(
-            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE']
+            self.temp_dir, ['COPYRIGHT', 'NOTICES', 'LICENSE', 'COPYING']
         )
         results['license_files'] = files
         copyhits = PackageManager.scan_for_copyright(self.temp_dir)
         results['copyrights'] = copyhits
         self.results = results
 
     def generate_report(self):
@@ -53,13 +53,12 @@
 
     def construct_download_url(self):
         namespace = (
             self.purl_details['namespace'].replace('%40', '@')
             if self.purl_details['namespace']
             else self.purl_details['name']
         )
-        iniName = namespace[0].lower()
         return (
-            f"https://pypi.python.org/packages/source/{iniName}/{namespace}/"
-            f"{self.purl_details['name']}-"
-            f"{self.purl_details['version']}.tar.gz"
+            f"https://www.nuget.org/api/v2/package/"
+            f"{self.purl_details['name']}/"
+            f"{self.purl_details['version']}"
         )
```

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.6/xmonkey_namonica/utils.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.5/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.6/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 xmonkey_namonica.egg-info/dependency_links.txt
 xmonkey_namonica.egg-info/entry_points.txt
 xmonkey_namonica.egg-info/requires.txt
 xmonkey_namonica.egg-info/top_level.txt
 xmonkey_namonica/handlers/__init__.py
 xmonkey_namonica/handlers/base_handler.py
 xmonkey_namonica/handlers/cargo_handler.py
+xmonkey_namonica/handlers/gem_handler.py
 xmonkey_namonica/handlers/gen_handler.py
 xmonkey_namonica/handlers/github_handler.py
 xmonkey_namonica/handlers/golang_handler.py
 xmonkey_namonica/handlers/npm_handler.py
 xmonkey_namonica/handlers/nuget_handler.py
 xmonkey_namonica/handlers/pypi_handler.py
```

