# Comparing `tmp/tutor-contrib-panorama-16.2.2.tar.gz` & `tmp/tutor_contrib_panorama-16.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/andres/Workspace/tutor-contrib-panorama/dist/.tmp-1hyp30cc/tutor-contrib-panorama-16.2.2.tar", last modified: Wed Mar  6 15:01:33 2024, max compression
+gzip compressed data, was "/Users/andres/Workspace/tutor-contrib-panorama/dist/.tmp-jyg3f1j0/tutor_contrib_panorama-16.2.3.tar", last modified: Fri May  3 12:57:04 2024, max compression
```

## Comparing `tutor-contrib-panorama-16.2.2.tar` & `tutor_contrib_panorama-16.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.826391 tutor-contrib-panorama-16.2.2/
--rw-r--r--   0 andres     (501) staff       (20)    11357 2022-06-16 13:37:21.000000 tutor-contrib-panorama-16.2.2/LICENSE
--rw-r--r--   0 andres     (501) staff       (20)       86 2023-11-29 11:52:52.000000 tutor-contrib-panorama-16.2.2/MANIFEST.in
--rw-r--r--   0 andres     (501) staff       (20)     8353 2024-03-06 15:01:33.799613 tutor-contrib-panorama-16.2.2/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)     7338 2023-12-19 18:38:42.000000 tutor-contrib-panorama-16.2.2/README.rst
--rw-r--r--   0 andres     (501) staff       (20)       38 2024-03-06 15:01:33.826599 tutor-contrib-panorama-16.2.2/setup.cfg
--rw-r--r--   0 andres     (501) staff       (20)     1840 2024-02-16 21:54:33.000000 tutor-contrib-panorama-16.2.2/setup.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.798817 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/
--rw-r--r--   0 andres     (501) staff       (20)     8353 2024-03-06 15:01:33.000000 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/PKG-INFO
--rw-r--r--   0 andres     (501) staff       (20)     1434 2024-03-06 15:01:33.000000 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 andres     (501) staff       (20)        1 2024-03-06 15:01:33.000000 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 andres     (501) staff       (20)       50 2024-03-06 15:01:33.000000 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/entry_points.txt
--rw-r--r--   0 andres     (501) staff       (20)       22 2024-03-06 15:01:33.000000 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/requires.txt
--rw-r--r--   0 andres     (501) staff       (20)       14 2024-03-06 15:01:33.000000 tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/top_level.txt
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.754803 tutor-contrib-panorama-16.2.2/tutorpanorama/
--rw-r--r--   0 andres     (501) staff       (20)       23 2024-03-04 20:02:01.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/__about__.py
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/__init__.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.782298 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/.gitignore
--rw-r--r--   0 andres     (501) staff       (20)     2327 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/k8s-deployments
--rw-r--r--   0 andres     (501) staff       (20)     1438 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/k8s-jobs
--rw-r--r--   0 andres     (501) staff       (20)     1064 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/kustomization
--rw-r--r--   0 andres     (501) staff       (20)      514 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/kustomization-configmapgenerator
--rw-r--r--   0 andres     (501) staff       (20)      983 2023-12-19 18:38:42.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/local-docker-compose-dev-services
--rw-r--r--   0 andres     (501) staff       (20)      187 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/local-docker-compose-jobs-services
--rw-r--r--   0 andres     (501) staff       (20)      927 2023-07-17 11:05:52.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/patches/local-docker-compose-services
--rw-r--r--   0 andres     (501) staff       (20)     4277 2024-02-19 20:11:23.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/plugin.py
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.747133 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.748526 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.783240 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/.gitignore
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.794798 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/
--rw-r--r--   0 andres     (501) staff       (20)      145 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/crontab
--rw-r--r--   0 andres     (501) staff       (20)     1585 2023-12-19 19:12:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf
--rw-r--r--   0 andres     (501) staff       (20)     2866 2023-07-17 08:20:19.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf
--rw-r--r--   0 andres     (501) staff       (20)    13120 2023-12-19 18:38:42.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml
--rw-r--r--   0 andres     (501) staff       (20)      267 2022-11-15 16:01:37.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/parsers.conf
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.795645 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/
--rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/.gitignore
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.796031 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/panorama-elt/
--rw-r--r--   0 andres     (501) staff       (20)      309 2024-03-04 20:00:52.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/panorama-elt/Dockerfile
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.796877 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/panorama-elt-logs/
--rw-r--r--   0 andres     (501) staff       (20)      561 2023-12-19 19:11:44.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.797521 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/tasks/
--rw-r--r--   0 andres     (501) staff       (20)        0 2023-12-19 18:38:42.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/tasks/.gitignore
-drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-03-06 15:01:33.797975 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/tasks/panorama-elt/
--rw-r--r--   0 andres     (501) staff       (20)      511 2023-12-19 18:38:42.000000 tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/tasks/panorama-elt/init
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.850060 tutor_contrib_panorama-16.2.3/
+-rw-r--r--   0 andres     (501) staff       (20)    11357 2022-06-16 13:37:21.000000 tutor_contrib_panorama-16.2.3/LICENSE
+-rw-r--r--   0 andres     (501) staff       (20)       86 2023-11-29 11:52:52.000000 tutor_contrib_panorama-16.2.3/MANIFEST.in
+-rw-r--r--   0 andres     (501) staff       (20)     8353 2024-05-03 12:57:04.849578 tutor_contrib_panorama-16.2.3/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)     7338 2023-12-19 18:38:42.000000 tutor_contrib_panorama-16.2.3/README.rst
+-rw-r--r--   0 andres     (501) staff       (20)       38 2024-05-03 12:57:04.850181 tutor_contrib_panorama-16.2.3/setup.cfg
+-rw-r--r--   0 andres     (501) staff       (20)     1840 2024-02-16 21:54:33.000000 tutor_contrib_panorama-16.2.3/setup.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.848889 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/
+-rw-r--r--   0 andres     (501) staff       (20)     8353 2024-05-03 12:57:04.000000 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 andres     (501) staff       (20)     1434 2024-05-03 12:57:04.000000 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 andres     (501) staff       (20)        1 2024-05-03 12:57:04.000000 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 andres     (501) staff       (20)       50 2024-05-03 12:57:04.000000 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/entry_points.txt
+-rw-r--r--   0 andres     (501) staff       (20)       22 2024-05-03 12:57:04.000000 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/requires.txt
+-rw-r--r--   0 andres     (501) staff       (20)       14 2024-05-03 12:57:04.000000 tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/top_level.txt
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.836251 tutor_contrib_panorama-16.2.3/tutorpanorama/
+-rw-r--r--   0 andres     (501) staff       (20)       23 2024-05-03 12:56:42.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/__about__.py
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/__init__.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.841755 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/.gitignore
+-rw-r--r--   0 andres     (501) staff       (20)     2327 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/k8s-deployments
+-rw-r--r--   0 andres     (501) staff       (20)     1438 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/k8s-jobs
+-rw-r--r--   0 andres     (501) staff       (20)     1064 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/kustomization
+-rw-r--r--   0 andres     (501) staff       (20)      514 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/kustomization-configmapgenerator
+-rw-r--r--   0 andres     (501) staff       (20)      983 2023-12-19 18:38:42.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/local-docker-compose-dev-services
+-rw-r--r--   0 andres     (501) staff       (20)      187 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 andres     (501) staff       (20)      927 2023-07-17 11:05:52.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/patches/local-docker-compose-services
+-rw-r--r--   0 andres     (501) staff       (20)     4277 2024-05-02 14:41:57.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/plugin.py
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.829299 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.830638 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.842494 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/.gitignore
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.845471 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/
+-rw-r--r--   0 andres     (501) staff       (20)      145 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/crontab
+-rw-r--r--   0 andres     (501) staff       (20)     1585 2023-12-19 19:12:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf
+-rw-r--r--   0 andres     (501) staff       (20)     2866 2023-07-17 08:20:19.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf
+-rw-r--r--   0 andres     (501) staff       (20)    13132 2024-05-03 12:53:56.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml
+-rw-r--r--   0 andres     (501) staff       (20)      267 2022-11-15 16:01:37.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/parsers.conf
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.846147 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2022-05-17 21:35:53.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/.gitignore
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.846453 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/panorama-elt/
+-rw-r--r--   0 andres     (501) staff       (20)      309 2024-05-02 14:41:57.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/panorama-elt/Dockerfile
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.847199 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/panorama-elt-logs/
+-rw-r--r--   0 andres     (501) staff       (20)      561 2024-05-02 14:41:57.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.847841 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/tasks/
+-rw-r--r--   0 andres     (501) staff       (20)        0 2023-12-19 18:38:42.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/tasks/.gitignore
+drwxr-xr-x   0 andres     (501) staff       (20)        0 2024-05-03 12:57:04.848153 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/tasks/panorama-elt/
+-rw-r--r--   0 andres     (501) staff       (20)      511 2023-12-19 18:38:42.000000 tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/tasks/panorama-elt/init
```

### Comparing `tutor-contrib-panorama-16.2.2/LICENSE` & `tutor_contrib_panorama-16.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/PKG-INFO` & `tutor_contrib_panorama-16.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-panorama
-Version: 16.2.2
+Version: 16.2.3
 Summary: Tutor plugin for Panorama Analytics
 Home-page: https://github.com/aulasneo/tutor-contrib-panorama
 Author: Aulsneo
 Author-email: andres@aulasneo.com
 Maintainer: Aulasneo
 License: AGPLv3
 Project-URL: Code, https://github.com/aulasneo/tutor-contrib-panorama
```

### Comparing `tutor-contrib-panorama-16.2.2/README.rst` & `tutor_contrib_panorama-16.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/setup.py` & `tutor_contrib_panorama-16.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/PKG-INFO` & `tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-panorama
-Version: 16.2.2
+Version: 16.2.3
 Summary: Tutor plugin for Panorama Analytics
 Home-page: https://github.com/aulasneo/tutor-contrib-panorama
 Author: Aulsneo
 Author-email: andres@aulasneo.com
 Maintainer: Aulasneo
 License: AGPLv3
 Project-URL: Code, https://github.com/aulasneo/tutor-contrib-panorama
```

### Comparing `tutor-contrib-panorama-16.2.2/tutor_contrib_panorama.egg-info/SOURCES.txt` & `tutor_contrib_panorama-16.2.3/tutor_contrib_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/patches/k8s-deployments` & `tutor_contrib_panorama-16.2.3/tutorpanorama/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/patches/k8s-jobs` & `tutor_contrib_panorama-16.2.3/tutorpanorama/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/patches/kustomization` & `tutor_contrib_panorama-16.2.3/tutorpanorama/patches/kustomization`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/patches/kustomization-configmapgenerator` & `tutor_contrib_panorama-16.2.3/tutorpanorama/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/patches/local-docker-compose-dev-services` & `tutor_contrib_panorama-16.2.3/tutorpanorama/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/patches/local-docker-compose-services` & `tutor_contrib_panorama-16.2.3/tutorpanorama/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/plugin.py` & `tutor_contrib_panorama-16.2.3/tutorpanorama/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf` & `tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit-local.conf`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf` & `tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/fluent-bit.conf`

 * *Files identical despite different names*

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml` & `tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/apps/panorama-elt/panorama_openedx_settings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   - name: lms
     type: varchar
     value: {{ LMS_HOST }}
 datasources:
 - type: openedx_course_structures
   name: openedx_course_structures
   mongodb_host: {{ MONGODB_HOST }}
-  mongodb_username: {{ MONGODB_USERNAME }}
-  mongodb_password: {{ MONGODB_PASSWORD }}
+  mongodb_username: "{{ MONGODB_USERNAME }}"
+  mongodb_password: "{{ MONGODB_PASSWORD }}"
   mongodb_database: {{ MONGODB_DATABASE }}
   {% if PANORAMA_USE_SPLIT_MONGO %}
-  mysql_username: {{ OPENEDX_MYSQL_USERNAME }}
-  mysql_password: {{ OPENEDX_MYSQL_PASSWORD }}
+  mysql_username: "{{ OPENEDX_MYSQL_USERNAME }}"
+  mysql_password: "{{ OPENEDX_MYSQL_PASSWORD }}"
   mysql_host: {{ MYSQL_HOST }}
   mysql_database: {{ OPENEDX_MYSQL_DATABASE }}
   {% endif %}
   tables:
   - name: course_structures
     fields:
     - name: module_location
@@ -57,16 +57,16 @@
       type: varchar
     - name: component
       type: varchar
     - name: weight
       type: double
 - type: mysql
   name: openedx_mysql
-  mysql_username: {{ OPENEDX_MYSQL_USERNAME }}
-  mysql_password: {{ OPENEDX_MYSQL_PASSWORD }}
+  mysql_username: "{{ OPENEDX_MYSQL_USERNAME }}"
+  mysql_password: "{{ OPENEDX_MYSQL_PASSWORD }}"
   mysql_host: {{ MYSQL_HOST }}
   mysql_database: {{ OPENEDX_MYSQL_DATABASE }}
   tables:
   - name: student_anonymoususerid
     fields:
     - name: id
       type: int
```

### Comparing `tutor-contrib-panorama-16.2.2/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile` & `tutor_contrib_panorama-16.2.3/tutorpanorama/templates/panorama/build/panorama-elt-logs/Dockerfile`

 * *Files identical despite different names*

