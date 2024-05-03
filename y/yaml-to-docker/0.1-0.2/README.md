# Comparing `tmp/yaml_to_docker-0.1.tar.gz` & `tmp/yaml_to_docker-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_to_docker-0.1.tar", last modified: Thu May  2 22:00:01 2024, max compression
+gzip compressed data, was "yaml_to_docker-0.2.tar", last modified: Thu May  2 22:36:25 2024, max compression
```

## Comparing `yaml_to_docker-0.1.tar` & `yaml_to_docker-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-02 22:00:01.960307 yaml_to_docker-0.1/
--rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      471 2024-05-02 22:00:01.960307 yaml_to_docker-0.1/PKG-INFO
--rw-------   0 u0_a192  (10192) u0_a192  (10192)       90 2024-05-02 21:58:52.000000 yaml_to_docker-0.1/README.rst
--rw-------   0 u0_a192  (10192) u0_a192  (10192)       38 2024-05-02 22:00:01.963640 yaml_to_docker-0.1/setup.cfg
--rw-------   0 u0_a192  (10192) u0_a192  (10192)      593 2024-05-02 21:57:57.000000 yaml_to_docker-0.1/setup.py
--rwx------   0 u0_a192  (10192) u0_a192  (10192)      531 2024-05-02 21:40:23.000000 yaml_to_docker-0.1/yaml-to-docker
-drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-02 22:00:01.956974 yaml_to_docker-0.1/yaml_to_docker.egg-info/
--rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      471 2024-05-02 22:00:01.000000 yaml_to_docker-0.1/yaml_to_docker.egg-info/PKG-INFO
--rw-------   0 u0_a192  (10192) u0_a192  (10192)      186 2024-05-02 22:00:01.000000 yaml_to_docker-0.1/yaml_to_docker.egg-info/SOURCES.txt
--rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-02 22:00:01.000000 yaml_to_docker-0.1/yaml_to_docker.egg-info/dependency_links.txt
--rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-02 22:00:01.000000 yaml_to_docker-0.1/yaml_to_docker.egg-info/top_level.txt
+drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-02 22:36:25.961421 yaml_to_docker-0.2/
+-rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      518 2024-05-02 22:36:25.958088 yaml_to_docker-0.2/PKG-INFO
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)      137 2024-05-02 22:10:12.000000 yaml_to_docker-0.2/README.rst
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)       38 2024-05-02 22:36:25.961421 yaml_to_docker-0.2/setup.cfg
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)      593 2024-05-02 22:35:06.000000 yaml_to_docker-0.2/setup.py
+-rwx------   0 u0_a192  (10192) u0_a192  (10192)      991 2024-05-02 22:34:36.000000 yaml_to_docker-0.2/yaml-to-docker
+drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-02 22:36:25.954754 yaml_to_docker-0.2/yaml_to_docker.egg-info/
+-rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      518 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/PKG-INFO
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)      186 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/SOURCES.txt
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/dependency_links.txt
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/top_level.txt
```

### Comparing `yaml_to_docker-0.1/setup.py` & `yaml_to_docker-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='yaml-to-docker',
-    version='0.1',
+    version='0.2',
     license='MIT',
     description='Script to Convert YAML to Docker',
     long_description=readme(),
     author='Alexander Krefting',
     author_email='linuxdevalex@outlook.de',
     url='https://github.com/androlinuxs/termux-music',
     scripts=['yaml-to-docker'],
```

