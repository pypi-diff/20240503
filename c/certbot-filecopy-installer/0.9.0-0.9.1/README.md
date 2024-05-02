# Comparing `tmp/certbot_filecopy_installer-0.9.0.tar.gz` & `tmp/certbot_filecopy_installer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_filecopy_installer-0.9.0.tar", last modified: Wed May  1 23:09:12 2024, max compression
+gzip compressed data, was "certbot_filecopy_installer-0.9.1.tar", last modified: Wed May  1 23:12:54 2024, max compression
```

## Comparing `certbot_filecopy_installer-0.9.0.tar` & `certbot_filecopy_installer-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:09:12.713451 certbot_filecopy_installer-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 23:09:08.000000 certbot_filecopy_installer-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 23:09:12.713451 certbot_filecopy_installer-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 23:09:08.000000 certbot_filecopy_installer-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:09:12.713451 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 23:09:12.000000 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-01 23:09:12.000000 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:09:12.000000 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 23:09:12.000000 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 23:09:12.000000 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 23:09:12.000000 certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:09:12.713451 certbot_filecopy_installer-0.9.0/filecopy_installer/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 23:09:08.000000 certbot_filecopy_installer-0.9.0/filecopy_installer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-01 23:09:08.000000 certbot_filecopy_installer-0.9.0/filecopy_installer/filecopy_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:09:12.713451 certbot_filecopy_installer-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-01 23:09:08.000000 certbot_filecopy_installer-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:12:54.160167 certbot_filecopy_installer-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 23:12:49.000000 certbot_filecopy_installer-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-01 23:12:54.160167 certbot_filecopy_installer-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 23:12:49.000000 certbot_filecopy_installer-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:12:54.160167 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-01 23:12:54.000000 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-01 23:12:54.000000 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:12:54.000000 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 23:12:54.000000 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 23:12:54.000000 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 23:12:54.000000 certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:12:54.160167 certbot_filecopy_installer-0.9.1/filecopy_installer/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 23:12:49.000000 certbot_filecopy_installer-0.9.1/filecopy_installer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-01 23:12:49.000000 certbot_filecopy_installer-0.9.1/filecopy_installer/filecopy_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:12:54.160167 certbot_filecopy_installer-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-01 23:12:49.000000 certbot_filecopy_installer-0.9.1/setup.py
```

### Comparing `certbot_filecopy_installer-0.9.0/LICENSE` & `certbot_filecopy_installer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot_filecopy_installer-0.9.0/PKG-INFO` & `certbot_filecopy_installer-0.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-filecopy-installer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simple file copy installer for certbot
 Home-page: https://github.com/NotBobTheBuilder/certbot-filecopy-installer
 Maintainer: Jack Wearden
 Maintainer-email: jack@jackwearden.co.uk
 License: MIT License
 Keywords: letsencrypt certbot installer
 Requires-Python: >=3.6
@@ -12,8 +12,13 @@
 License-File: LICENSE
 Requires-Dist: acme
 Requires-Dist: certbot
 Requires-Dist: setuptools
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
-README.md
+Certbot Filecopy Installer
+===
+
+This is a certbot plugin designed to install certificates by copying the file contents rather than just symlinks.
+
+Useful for systems that create or deploy certbot certificates across execution boundaries like containers.
```

### Comparing `certbot_filecopy_installer-0.9.0/certbot_filecopy_installer.egg-info/PKG-INFO` & `certbot_filecopy_installer-0.9.1/certbot_filecopy_installer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-filecopy-installer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simple file copy installer for certbot
 Home-page: https://github.com/NotBobTheBuilder/certbot-filecopy-installer
 Maintainer: Jack Wearden
 Maintainer-email: jack@jackwearden.co.uk
 License: MIT License
 Keywords: letsencrypt certbot installer
 Requires-Python: >=3.6
@@ -12,8 +12,13 @@
 License-File: LICENSE
 Requires-Dist: acme
 Requires-Dist: certbot
 Requires-Dist: setuptools
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
-README.md
+Certbot Filecopy Installer
+===
+
+This is a certbot plugin designed to install certificates by copying the file contents rather than just symlinks.
+
+Useful for systems that create or deploy certbot certificates across execution boundaries like containers.
```

### Comparing `certbot_filecopy_installer-0.9.0/filecopy_installer/filecopy_installer.py` & `certbot_filecopy_installer-0.9.1/filecopy_installer/filecopy_installer.py`

 * *Files identical despite different names*

### Comparing `certbot_filecopy_installer-0.9.0/setup.py` & `certbot_filecopy_installer-0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from setuptools import find_packages, setup
+from pathlib import Path
 
-version='0.9.0'
+version='0.9.1'
+this_directory = Path(__file__).parent
+long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='certbot-filecopy-installer',
     version=version,
     maintainer='Jack Wearden',
     maintainer_email='jack@jackwearden.co.uk',
     description='Simple file copy installer for certbot',
-    long_description='README.md',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='letsencrypt certbot installer',
     url='https://github.com/NotBobTheBuilder/certbot-filecopy-installer',
     license='MIT License',
     python_requires='>=3.6',
     packages=find_packages(),
     include_package_data=True,
```

