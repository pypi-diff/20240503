# Comparing `tmp/f2r-2.8.0.tar.gz` & `tmp/f2r-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f2r-2.8.0.tar", last modified: Fri May  3 06:53:49 2024, max compression
+gzip compressed data, was "f2r-2.8.1.tar", last modified: Fri May  3 07:19:43 2024, max compression
```

## Comparing `f2r-2.8.0.tar` & `f2r-2.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-05-03 06:53:49.244779 f2r-2.8.0/
--rw-r--r--   0 bvonhall   (502) staff       (20)    35141 2024-02-13 07:26:31.000000 f2r-2.8.0/COPYING
--rw-r--r--   0 bvonhall   (502) staff       (20)     3152 2024-05-03 06:53:49.244509 f2r-2.8.0/PKG-INFO
--rw-r--r--   0 bvonhall   (502) staff       (20)     2553 2024-05-03 06:50:43.000000 f2r-2.8.0/README.md
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     7469 2024-02-15 08:38:39.000000 f2r-2.8.0/f2r
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-05-03 06:53:49.235247 f2r-2.8.0/f2r.egg-info/
--rw-r--r--   0 bvonhall   (502) staff       (20)     3152 2024-05-03 06:53:49.000000 f2r-2.8.0/f2r.egg-info/PKG-INFO
--rw-r--r--   0 bvonhall   (502) staff       (20)      490 2024-05-03 06:53:49.000000 f2r-2.8.0/f2r.egg-info/SOURCES.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)        1 2024-05-03 06:53:49.000000 f2r-2.8.0/f2r.egg-info/dependency_links.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       34 2024-05-03 06:53:49.000000 f2r-2.8.0/f2r.egg-info/requires.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)        8 2024-05-03 06:53:49.000000 f2r-2.8.0/f2r.egg-info/top_level.txt
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-05-03 06:53:49.244071 f2r-2.8.0/flp2rpm/
--rw-r--r--   0 bvonhall   (502) staff       (20)      502 2024-04-30 09:46:54.000000 f2r-2.8.0/flp2rpm/Defaults.py
--rw-r--r--   0 bvonhall   (502) staff       (20)    10229 2024-04-30 10:08:08.000000 f2r-2.8.0/flp2rpm/Fpm.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1548 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/Module.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     3043 2024-04-30 09:46:54.000000 f2r-2.8.0/flp2rpm/Package.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      558 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/Repo.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1609 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/S3.py
--rw-r--r--   0 bvonhall   (502) staff       (20)       24 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1647 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/after_install_template.sh
--rw-r--r--   0 bvonhall   (502) staff       (20)      603 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/after_remove_template.sh
--rw-r--r--   0 bvonhall   (502) staff       (20)      314 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/config.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      731 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/devel.slc7.yaml
--rw-r--r--   0 bvonhall   (502) staff       (20)     1040 2024-05-03 06:46:09.000000 f2r-2.8.0/flp2rpm/devel.slc8.yaml
--rw-r--r--   0 bvonhall   (502) staff       (20)     1728 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/helpers.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      407 2024-02-13 07:26:31.000000 f2r-2.8.0/flp2rpm/runtime.slc7.yaml
--rw-r--r--   0 bvonhall   (502) staff       (20)      733 2024-05-03 06:46:09.000000 f2r-2.8.0/flp2rpm/runtime.slc8.yaml
--rw-r--r--   0 bvonhall   (502) staff       (20)       38 2024-05-03 06:53:49.244881 f2r-2.8.0/setup.cfg
--rw-r--r--   0 bvonhall   (502) staff       (20)     1124 2024-05-03 06:50:51.000000 f2r-2.8.0/setup.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-05-03 07:19:43.230113 f2r-2.8.1/
+-rw-r--r--   0 bvonhall   (502) staff       (20)    35141 2024-02-13 07:26:31.000000 f2r-2.8.1/COPYING
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3239 2024-05-03 07:19:43.229807 f2r-2.8.1/PKG-INFO
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2640 2024-05-03 07:18:30.000000 f2r-2.8.1/README.md
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     7469 2024-02-15 08:38:39.000000 f2r-2.8.1/f2r
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-05-03 07:19:43.222867 f2r-2.8.1/f2r.egg-info/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3239 2024-05-03 07:19:43.000000 f2r-2.8.1/f2r.egg-info/PKG-INFO
+-rw-r--r--   0 bvonhall   (502) staff       (20)      490 2024-05-03 07:19:43.000000 f2r-2.8.1/f2r.egg-info/SOURCES.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)        1 2024-05-03 07:19:43.000000 f2r-2.8.1/f2r.egg-info/dependency_links.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       34 2024-05-03 07:19:43.000000 f2r-2.8.1/f2r.egg-info/requires.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)        8 2024-05-03 07:19:43.000000 f2r-2.8.1/f2r.egg-info/top_level.txt
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-05-03 07:19:43.229241 f2r-2.8.1/flp2rpm/
+-rw-r--r--   0 bvonhall   (502) staff       (20)      547 2024-05-03 07:18:30.000000 f2r-2.8.1/flp2rpm/Defaults.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)    11209 2024-05-03 07:19:12.000000 f2r-2.8.1/flp2rpm/Fpm.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1548 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/Module.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3573 2024-05-03 07:18:30.000000 f2r-2.8.1/flp2rpm/Package.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      558 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/Repo.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1609 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/S3.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)       24 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1647 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/after_install_template.sh
+-rw-r--r--   0 bvonhall   (502) staff       (20)      603 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/after_remove_template.sh
+-rw-r--r--   0 bvonhall   (502) staff       (20)      314 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/config.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      731 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/devel.slc7.yaml
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1064 2024-05-03 07:18:30.000000 f2r-2.8.1/flp2rpm/devel.slc8.yaml
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1728 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/helpers.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      407 2024-02-13 07:26:31.000000 f2r-2.8.1/flp2rpm/runtime.slc7.yaml
+-rw-r--r--   0 bvonhall   (502) staff       (20)      751 2024-05-03 07:18:30.000000 f2r-2.8.1/flp2rpm/runtime.slc8.yaml
+-rw-r--r--   0 bvonhall   (502) staff       (20)       38 2024-05-03 07:19:43.230243 f2r-2.8.1/setup.cfg
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1124 2024-05-03 07:19:33.000000 f2r-2.8.1/setup.py
```

### Comparing `f2r-2.8.0/COPYING` & `f2r-2.8.1/COPYING`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/PKG-INFO` & `f2r-2.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f2r
-Version: 2.8.0
+Version: 2.8.1
 Summary: Produces RPMs for FLP packages out of aliBuild ouput
 Home-page: https://gitlab.cern.ch/AliceO2Group/flp-to-rpm
 Author: Adam Wegrzynek
 Author-email: adam.wegrzynek@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 Command line tool to create RPMs out of aliBuild output.
 
 ## Prerequisites
  - [aliBuild](https://alisw.github.io/alibuild/)
  - [environment Modules](https://modules.readthedocs.io/en/latest/) 4.3 or higher, RPM is available from [this S3 location](http://s3.cern.ch/swift/v1/system-configuration/RPMS/environment-modules-4.6.1-1.el7.cern.x86_64.rpm)
  - Optional: To enable S3 support you need to create a config file under `~/.s3cfg`, see [CERN IT instructions](https://clouddocs.web.cern.ch/object_store/s3cmd.html)
+ - gem + fpm: `yum install rubygems -y ; gem install fpm`
 
 ## Installation
 
 To just install the tool:
 `python3 -m pip install f2r`
 
 OR
@@ -39,14 +40,15 @@
 Build packages using `aliBuild`, eg:
 ```bash
 aliBuild build O2Suite --defaults o2-dataflow --always-prefer-system
 ```
 Then, run `alienv` as indicated by `aliBuild` in order to create modulefiles:
 ```bash
 alienv enter O2Suite/latest-o2-dataflow
+exit # do not forget to exit
 ```
 And create RPMs providing same package and version as to `alienv`:
 ```bash
 f2r generate --package O2Suite --version latest-o2-dataflow
 ```
 Validate created RPMs (this requires `sudo`):
 ```
```

### Comparing `f2r-2.8.0/README.md` & `f2r-2.8.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Command line tool to create RPMs out of aliBuild output.
 
 ## Prerequisites
  - [aliBuild](https://alisw.github.io/alibuild/)
  - [environment Modules](https://modules.readthedocs.io/en/latest/) 4.3 or higher, RPM is available from [this S3 location](http://s3.cern.ch/swift/v1/system-configuration/RPMS/environment-modules-4.6.1-1.el7.cern.x86_64.rpm)
  - Optional: To enable S3 support you need to create a config file under `~/.s3cfg`, see [CERN IT instructions](https://clouddocs.web.cern.ch/object_store/s3cmd.html)
+ - gem + fpm: `yum install rubygems -y ; gem install fpm`
 
 ## Installation
 
 To just install the tool:
 `python3 -m pip install f2r`
 
 OR
@@ -21,14 +22,15 @@
 Build packages using `aliBuild`, eg:
 ```bash
 aliBuild build O2Suite --defaults o2-dataflow --always-prefer-system
 ```
 Then, run `alienv` as indicated by `aliBuild` in order to create modulefiles:
 ```bash
 alienv enter O2Suite/latest-o2-dataflow
+exit # do not forget to exit
 ```
 And create RPMs providing same package and version as to `alienv`:
 ```bash
 f2r generate --package O2Suite --version latest-o2-dataflow
 ```
 Validate created RPMs (this requires `sudo`):
 ```
```

### Comparing `f2r-2.8.0/f2r` & `f2r-2.8.1/f2r`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/f2r.egg-info/PKG-INFO` & `f2r-2.8.1/f2r.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f2r
-Version: 2.8.0
+Version: 2.8.1
 Summary: Produces RPMs for FLP packages out of aliBuild ouput
 Home-page: https://gitlab.cern.ch/AliceO2Group/flp-to-rpm
 Author: Adam Wegrzynek
 Author-email: adam.wegrzynek@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 Command line tool to create RPMs out of aliBuild output.
 
 ## Prerequisites
  - [aliBuild](https://alisw.github.io/alibuild/)
  - [environment Modules](https://modules.readthedocs.io/en/latest/) 4.3 or higher, RPM is available from [this S3 location](http://s3.cern.ch/swift/v1/system-configuration/RPMS/environment-modules-4.6.1-1.el7.cern.x86_64.rpm)
  - Optional: To enable S3 support you need to create a config file under `~/.s3cfg`, see [CERN IT instructions](https://clouddocs.web.cern.ch/object_store/s3cmd.html)
+ - gem + fpm: `yum install rubygems -y ; gem install fpm`
 
 ## Installation
 
 To just install the tool:
 `python3 -m pip install f2r`
 
 OR
@@ -39,14 +40,15 @@
 Build packages using `aliBuild`, eg:
 ```bash
 aliBuild build O2Suite --defaults o2-dataflow --always-prefer-system
 ```
 Then, run `alienv` as indicated by `aliBuild` in order to create modulefiles:
 ```bash
 alienv enter O2Suite/latest-o2-dataflow
+exit # do not forget to exit
 ```
 And create RPMs providing same package and version as to `alienv`:
 ```bash
 f2r generate --package O2Suite --version latest-o2-dataflow
 ```
 Validate created RPMs (this requires `sudo`):
 ```
```

### Comparing `f2r-2.8.0/flp2rpm/Fpm.py` & `f2r-2.8.1/flp2rpm/Fpm.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,31 @@
 
         self.runtimeDepsDict = parseYamlDict(os.path.join(config.work_dir, 'runtime.' + self.release_suffix + '.yaml'))
         self.develDepsDict = parseYamlDict(os.path.join(config.work_dir, 'devel.' + self.release_suffix + '.yaml'))
 
         if config.tag_version:
             self.release_suffix += '_' + config.release_tag.replace('/', '_')
 
+    rpmType = 'dir'
+    # prep dir arguments
+    # `=.` is necessary so that the complete source dir path
+    # is not replicated and the target dir consists of only
+    # prefix + package name + dir
+    package_dir = self.buildDir + "/" + name + "/" + fullVersion + "/"
+    subdirs = ['bin', 'lib', 'lib64', 'etc', 'include', 'bin-safe', 'libexec', 'WebDID', 'share', 'plugins', 'cmake', 'sbin', 'icons', 'fonts', 'response']
+    paths = []
+    for subdir in subdirs:
+        if os.path.exists(package_dir + subdir):
+            if subdir == 'etc' and os.listdir(package_dir + subdir) == ['modulefiles', 'profile.d']:
+                continue
+            # This is an ugly fix to a temporary problem. (OCONF-799)
+            # The lib64 symlink to lib in the Python-modules causes issues with fpm.
+            if name == 'Python-modules' and subdir == 'lib64' and os.path.islink(package_dir+subdir):
+                continue
+            paths.append(package_dir + subdir + '=.')
     def run(self, name, version, deps, devel_deps, extra_deps, RPMS_GENERATED=[]):
         """ Prepares arguments and executes fpm """
         fullVersion = version
         version = version.replace('local', '', 1)
         # Handle not standard versions, nightly, latest-o2-dataflow
         if 'latest' in version:
             iterationArg = ['--iteration', self.release_suffix]
```

### Comparing `f2r-2.8.0/flp2rpm/Module.py` & `f2r-2.8.1/flp2rpm/Module.py`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/Package.py` & `f2r-2.8.1/flp2rpm/Package.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,34 +2,44 @@
 import os
 
 from . import config
 from .helpers import parseRecipeHeader
 from .helpers import parseYamlDict
 from .Module import Module
 from .Defaults import Defaults
+import logging
 
 
 class Package:
 
     def __init__(self, name, version = None):
         self.name = name
         self.path = os.path.join(config.ali_prefix, 'alidist', name.lower() + '.sh')
 
         parsed = parseRecipeHeader(self.path)
         self.requires = parsed['requires'] if 'requires' in parsed.keys() else []
+
+        self.defaults = Defaults()
+        if self.defaults is not None and self.defaults.overrides is not None and self.name in self.defaults.overrides.keys() and 'requires' in self.defaults.overrides[self.name].keys(): # todo what is the proper way of expressing this ?
+            defaults_deps = self.defaults.overrides[self.name]['requires']
+            self.requires = defaults_deps
+
         self.devel = parsed['build_requires'] if 'build_requires' in parsed.keys() else []
         self.version = parsed['version'] 
         self.tag = parsed['tag'] if 'tag' in parsed else parsed['version']
-        if version != None:
+        if version is not None:
             self.module_version = version
             self.module_dep_versions = Module(name).deps_as_dict(version)
         else:
-            self.module_version = None;
+            self.module_version = None
             self.module_dep_versions = {}    
-        self.defaults = Defaults()
+
+
+    def __str__(self):
+        return f"package {self.name}: \nRequires: {self.requires}\nDevel: {self.devel}\nTag: {self.tag}\nVersion: {self.version}"
 
     def filter_deps(self, deps):
         """ List of deps with already applied arch and defaults filters """
         filtered = []
         # Filter on arch
         for dep in deps:
             filter = dep.split(':')
@@ -44,14 +54,15 @@
             return [x for x in filtered if x not in self.defaults.disable]
         return filtered
 
     def deps_with_versions(self):
         """ In addition to list of dependencies it provides correct versions from modulefile """
         dict = {}
         deps = self.filter_deps(self.requires)
+
         for dep in deps:
             if dep in self.module_dep_versions.keys():
                 dict[dep] = self.module_dep_versions[dep]
             else:
                 dict[dep] = 'from_system'  # TODO: rename dep into system RPM name
         return dict
```

### Comparing `f2r-2.8.0/flp2rpm/Repo.py` & `f2r-2.8.1/flp2rpm/Repo.py`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/S3.py` & `f2r-2.8.1/flp2rpm/S3.py`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/after_install_template.sh` & `f2r-2.8.1/flp2rpm/after_install_template.sh`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/after_remove_template.sh` & `f2r-2.8.1/flp2rpm/after_remove_template.sh`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/devel.slc7.yaml` & `f2r-2.8.1/flp2rpm/devel.slc7.yaml`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/devel.slc8.yaml` & `f2r-2.8.1/flp2rpm/devel.slc8.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,9 @@
 system-subversion:
   - subversion
   - subversion-devel
 golang:
   - golang
 MySQL:
   - mysql-devel
+sqlite:
+  - sqlite-devel
```

### Comparing `f2r-2.8.0/flp2rpm/helpers.py` & `f2r-2.8.1/flp2rpm/helpers.py`

 * *Files identical despite different names*

### Comparing `f2r-2.8.0/flp2rpm/runtime.slc8.yaml` & `f2r-2.8.1/flp2rpm/runtime.slc8.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -50,7 +50,9 @@
   - cyrus-sasl-devel
   - cyrus-sasl-md5
 system-subversion:
   - subversion
   - subversion-devel
 MySQL:
   - mysql-libs
+sqlite:
+  - sqlite
```

### Comparing `f2r-2.8.0/setup.py` & `f2r-2.8.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='f2r',
-    version='2.8.0',
+    version='2.8.1',
     author='Adam Wegrzynek',
     author_email='adam.wegrzynek@cern.ch',
     url='https://gitlab.cern.ch/AliceO2Group/flp-to-rpm',
     license='GPLv3',
     description='Produces RPMs for FLP packages out of aliBuild ouput',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

