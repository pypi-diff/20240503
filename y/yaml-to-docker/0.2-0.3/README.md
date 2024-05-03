# Comparing `tmp/yaml_to_docker-0.2.tar.gz` & `tmp/yaml_to_docker-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_to_docker-0.2.tar", last modified: Thu May  2 22:36:25 2024, max compression
+gzip compressed data, was "yaml_to_docker-0.3.tar", last modified: Fri May  3 10:20:37 2024, max compression
```

## Comparing `yaml_to_docker-0.2.tar` & `yaml_to_docker-0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-02 22:36:25.961421 yaml_to_docker-0.2/
--rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      518 2024-05-02 22:36:25.958088 yaml_to_docker-0.2/PKG-INFO
--rw-------   0 u0_a192  (10192) u0_a192  (10192)      137 2024-05-02 22:10:12.000000 yaml_to_docker-0.2/README.rst
--rw-------   0 u0_a192  (10192) u0_a192  (10192)       38 2024-05-02 22:36:25.961421 yaml_to_docker-0.2/setup.cfg
--rw-------   0 u0_a192  (10192) u0_a192  (10192)      593 2024-05-02 22:35:06.000000 yaml_to_docker-0.2/setup.py
--rwx------   0 u0_a192  (10192) u0_a192  (10192)      991 2024-05-02 22:34:36.000000 yaml_to_docker-0.2/yaml-to-docker
-drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-02 22:36:25.954754 yaml_to_docker-0.2/yaml_to_docker.egg-info/
--rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      518 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/PKG-INFO
--rw-------   0 u0_a192  (10192) u0_a192  (10192)      186 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/SOURCES.txt
--rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/dependency_links.txt
--rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-02 22:36:25.000000 yaml_to_docker-0.2/yaml_to_docker.egg-info/top_level.txt
+drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-03 10:20:37.508770 yaml_to_docker-0.3/
+-rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      649 2024-05-03 10:20:37.505437 yaml_to_docker-0.3/PKG-INFO
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)      233 2024-05-03 09:23:40.000000 yaml_to_docker-0.3/README.rst
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)       38 2024-05-03 10:20:37.508770 yaml_to_docker-0.3/setup.cfg
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)      663 2024-05-03 10:20:14.000000 yaml_to_docker-0.3/setup.py
+-rwx------   0 u0_a192  (10192) u0_a192  (10192)     1159 2024-05-03 10:16:34.000000 yaml_to_docker-0.3/yaml-to-docker-py
+-rwx------   0 u0_a192  (10192) u0_a192  (10192)      991 2024-05-02 22:34:36.000000 yaml_to_docker-0.3/yaml-to-docker-sh
+drwx------   0 u0_a192  (10192) u0_a192  (10192)        0 2024-05-03 10:20:37.502104 yaml_to_docker-0.3/yaml_to_docker.egg-info/
+-rw-r--r--   0 u0_a192  (10192) u0_a192  (10192)      649 2024-05-03 10:20:37.000000 yaml_to_docker-0.3/yaml_to_docker.egg-info/PKG-INFO
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)      244 2024-05-03 10:20:37.000000 yaml_to_docker-0.3/yaml_to_docker.egg-info/SOURCES.txt
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-03 10:20:37.000000 yaml_to_docker-0.3/yaml_to_docker.egg-info/dependency_links.txt
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)       20 2024-05-03 10:20:37.000000 yaml_to_docker-0.3/yaml_to_docker.egg-info/requires.txt
+-rw-------   0 u0_a192  (10192) u0_a192  (10192)        1 2024-05-03 10:20:37.000000 yaml_to_docker-0.3/yaml_to_docker.egg-info/top_level.txt
```

### Comparing `yaml_to_docker-0.2/yaml-to-docker` & `yaml_to_docker-0.3/yaml-to-docker-sh`

 * *Files identical despite different names*

