# Comparing `tmp/chartfactor_jlab_ext-5.0.6.tar.gz` & `tmp/chartfactor_jlab_ext-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartfactor_jlab_ext-5.0.6.tar", last modified: Mon Apr 29 22:51:53 2024, max compression
+gzip compressed data, was "chartfactor_jlab_ext-5.0.7.tar", last modified: Thu May  2 22:27:37 2024, max compression
```

## Comparing `chartfactor_jlab_ext-5.0.6.tar` & `chartfactor_jlab_ext-5.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.251039 chartfactor_jlab_ext-5.0.6/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1506 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/LICENSE
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      379 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.0.6/MANIFEST.in
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-04-29 22:51:53.250802 chartfactor_jlab_ext-5.0.6/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1861 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/README.md
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.246781 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     6148 2023-04-06 16:48:24.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/.DS_Store
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      318 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/__init__.py
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      441 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/_version.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.246965 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2342 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/package.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.248610 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    15480 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2669 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      852 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    70526 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      336 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     7251 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     3373 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    85623 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      219 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     7858 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/remoteEntry.1944209dd73a93dcabf8.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      163 2024-04-29 22:51:51.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/style.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)    20796 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.250613 chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/PKG-INFO
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1436 2024-04-29 22:51:53.000000 chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/SOURCES.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/dependency_links.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-04-29 22:51:43.000000 chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/not-zip-safe
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       56 2024-04-29 22:51:52.000000 chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/top_level.txt
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      201 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/install.json
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.249993 chartfactor_jlab_ext-5.0.6/lib/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     9591 2022-06-24 19:57:03.000000 chartfactor_jlab_ext-5.0.6/lib/cfs.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1675 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.0.6/lib/commons.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      877 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.0.6/lib/index.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     1969 2022-06-17 17:26:57.000000 chartfactor_jlab_ext-5.0.6/lib/model.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      828 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.0.6/lib/runner.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2642 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.0.6/lib/storage-utils.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2198 2024-04-29 22:51:31.000000 chartfactor_jlab_ext-5.0.6/package.json
--rw-r--r--   0 jorgealarcon   (501) staff       (20)      145 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/pyproject.toml
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-04-29 22:51:53.251081 chartfactor_jlab_ext-5.0.6/setup.cfg
--rw-r--r--   0 jorgealarcon   (501) staff       (20)     2636 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.0.6/setup.py
-drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-04-29 22:51:53.250448 chartfactor_jlab_ext-5.0.6/style/
--rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/style/base.css
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       25 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/style/index.css
--rw-r--r--   0 jorgealarcon   (501) staff       (20)       21 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.6/style/index.js
--rw-r--r--   0 jorgealarcon   (501) staff       (20)   259094 2022-06-07 13:33:05.000000 chartfactor_jlab_ext-5.0.6/yarn.lock
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.160215 chartfactor_jlab_ext-5.0.7/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1506 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/LICENSE
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      379 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.0.7/MANIFEST.in
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-05-02 22:27:37.159987 chartfactor_jlab_ext-5.0.7/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1861 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/README.md
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.156155 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     6148 2023-04-06 16:48:24.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/.DS_Store
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      318 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/__init__.py
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      441 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/_version.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.156378 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2342 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/package.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.157904 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    15480 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2669 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      852 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    70526 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      336 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     7251 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     3373 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    85623 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      219 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     7858 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/remoteEntry.4e5718c5a6dbf6be84ba.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      163 2024-05-02 22:27:35.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/style.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)    20796 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.159803 chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2905 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/PKG-INFO
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1436 2024-05-02 22:27:37.000000 chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        1 2024-05-02 22:27:28.000000 chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/not-zip-safe
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       56 2024-05-02 22:27:36.000000 chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/top_level.txt
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      201 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/install.json
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.159278 chartfactor_jlab_ext-5.0.7/lib/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     9591 2022-06-24 19:57:03.000000 chartfactor_jlab_ext-5.0.7/lib/cfs.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1675 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.0.7/lib/commons.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      877 2022-06-15 14:46:17.000000 chartfactor_jlab_ext-5.0.7/lib/index.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     1969 2022-06-17 17:26:57.000000 chartfactor_jlab_ext-5.0.7/lib/model.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      828 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.0.7/lib/runner.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2642 2022-05-26 22:15:14.000000 chartfactor_jlab_ext-5.0.7/lib/storage-utils.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2198 2024-05-02 22:27:16.000000 chartfactor_jlab_ext-5.0.7/package.json
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)      145 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/pyproject.toml
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       38 2024-05-02 22:27:37.160254 chartfactor_jlab_ext-5.0.7/setup.cfg
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)     2636 2022-09-08 23:50:12.000000 chartfactor_jlab_ext-5.0.7/setup.py
+drwxr-xr-x   0 jorgealarcon   (501) staff       (20)        0 2024-05-02 22:27:37.159653 chartfactor_jlab_ext-5.0.7/style/
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)        0 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/style/base.css
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       25 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/style/index.css
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)       21 2022-02-15 22:26:32.000000 chartfactor_jlab_ext-5.0.7/style/index.js
+-rw-r--r--   0 jorgealarcon   (501) staff       (20)   259094 2022-06-07 13:33:05.000000 chartfactor_jlab_ext-5.0.7/yarn.lock
```

### Comparing `chartfactor_jlab_ext-5.0.6/LICENSE` & `chartfactor_jlab_ext-5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/PKG-INFO` & `chartfactor_jlab_ext-5.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor-jlab-ext
-Version: 5.0.6
+Version: 5.0.7
 Summary: Run chartfactor-py python commands in Jupyter Lab Kernels
 Home-page: https://github.com/Aktiun/chartfactor-jlab-ext
 Author: Aktiun
 Author-email: info@aktiun.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `chartfactor_jlab_ext-5.0.6/README.md` & `chartfactor_jlab_ext-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/.DS_Store` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/.DS_Store`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/package.json` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.972953216374269%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4e5718c5a6dbf6be84ba.js'}}",*

 * * "'version'": "'5.0.7'"}*

```diff
@@ -26,15 +26,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Aktiun/chartfactor-jlab-ext",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1944209dd73a93dcabf8.js",
+            "load": "static/remoteEntry.4e5718c5a6dbf6be84ba.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "chartfactor-jlab-ext/labextension"
     },
     "keywords": [
         "jupyter",
@@ -69,9 +69,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "5.0.6"
+    "version": "5.0.7"
 }
```

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/100.7e3a5f4a20c0f69ea729.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/remoteEntry.1944209dd73a93dcabf8.js` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/remoteEntry.4e5718c5a6dbf6be84ba.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -120,15 +120,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => w.e(223).then((() => () => w(223))))), l("chartfactor_jlab_ext", "5.0.6", (() => w.e(568).then((() => () => w(568))))), l("jupyterlab_toastify", "4.2.1", (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))), l("lodash", "4.17.21", (() => w.e(486).then((() => () => w(486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@phosphor/disposable", "1.10.1", (() => w.e(223).then((() => () => w(223))))), l("chartfactor_jlab_ext", "5.0.7", (() => w.e(568).then((() => () => w(568))))), l("jupyterlab_toastify", "4.2.1", (() => Promise.all([w.e(813), w.e(271)]).then((() => () => w(813))))), l("lodash", "4.17.21", (() => w.e(486).then((() => () => w(486)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor-jlab-ext/labextension/static/third-party-licenses.json` & `chartfactor_jlab_ext-5.0.7/chartfactor-jlab-ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/PKG-INFO` & `chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartfactor-jlab-ext
-Version: 5.0.6
+Version: 5.0.7
 Summary: Run chartfactor-py python commands in Jupyter Lab Kernels
 Home-page: https://github.com/Aktiun/chartfactor-jlab-ext
 Author: Aktiun
 Author-email: info@aktiun.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `chartfactor_jlab_ext-5.0.6/chartfactor_jlab_ext.egg-info/SOURCES.txt` & `chartfactor_jlab_ext-5.0.7/chartfactor_jlab_ext.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 chartfactor-jlab-ext/labextension/static/223.a93208f6436a19e928eb.js.LICENSE.txt
 chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js
 chartfactor-jlab-ext/labextension/static/486.ea74e810f4cf66ad8b28.js.LICENSE.txt
 chartfactor-jlab-ext/labextension/static/568.cb540ea7001c8dafbb5a.js
 chartfactor-jlab-ext/labextension/static/747.b46981187fdb90cccf38.js
 chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js
 chartfactor-jlab-ext/labextension/static/813.05d4b12c6f2c4f7d9c5b.js.LICENSE.txt
-chartfactor-jlab-ext/labextension/static/remoteEntry.1944209dd73a93dcabf8.js
+chartfactor-jlab-ext/labextension/static/remoteEntry.4e5718c5a6dbf6be84ba.js
 chartfactor-jlab-ext/labextension/static/style.js
 chartfactor-jlab-ext/labextension/static/third-party-licenses.json
 chartfactor_jlab_ext.egg-info/PKG-INFO
 chartfactor_jlab_ext.egg-info/SOURCES.txt
 chartfactor_jlab_ext.egg-info/dependency_links.txt
 chartfactor_jlab_ext.egg-info/not-zip-safe
 chartfactor_jlab_ext.egg-info/top_level.txt
```

### Comparing `chartfactor_jlab_ext-5.0.6/lib/cfs.js` & `chartfactor_jlab_ext-5.0.7/lib/cfs.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/lib/commons.js` & `chartfactor_jlab_ext-5.0.7/lib/commons.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/lib/index.js` & `chartfactor_jlab_ext-5.0.7/lib/index.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/lib/model.js` & `chartfactor_jlab_ext-5.0.7/lib/model.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/lib/runner.js` & `chartfactor_jlab_ext-5.0.7/lib/runner.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/lib/storage-utils.js` & `chartfactor_jlab_ext-5.0.7/lib/storage-utils.js`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/package.json` & `chartfactor_jlab_ext-5.0.7/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'5.0.7'"}*

```diff
@@ -64,9 +64,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
-    "version": "5.0.6"
+    "version": "5.0.7"
 }
```

### Comparing `chartfactor_jlab_ext-5.0.6/setup.py` & `chartfactor_jlab_ext-5.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `chartfactor_jlab_ext-5.0.6/yarn.lock` & `chartfactor_jlab_ext-5.0.7/yarn.lock`

 * *Files identical despite different names*

