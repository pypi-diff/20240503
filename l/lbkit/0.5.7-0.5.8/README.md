# Comparing `tmp/lbkit-0.5.7.tar.gz` & `tmp/lbkit-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbkit-0.5.7.tar", last modified: Sun Apr 28 16:23:16 2024, max compression
+gzip compressed data, was "lbkit-0.5.8.tar", last modified: Fri May  3 18:33:06 2024, max compression
```

## Comparing `lbkit-0.5.7.tar` & `lbkit-0.5.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/
--rw-rw-r--   0 root         (0) root         (0)      122 2024-04-28 16:23:09.000000 lbkit-0.5.7/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)    11357 2024-04-28 16:23:09.000000 lbkit-0.5.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      149 2024-04-28 16:23:09.000000 lbkit-0.5.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-28 16:23:16.106330 lbkit-0.5.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      388 2024-04-28 16:23:09.000000 lbkit-0.5.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.102330 lbkit-0.5.7/lbkit/
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-28 16:23:10.000000 lbkit-0.5.7/lbkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/ci_robot/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/ci_robot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12840 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/ci_robot/gitee.py
--rw-rw-r--   0 root         (0) root         (0)     8483 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/codegen/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4241 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/codegen.py
--rw-rw-r--   0 root         (0) root         (0)    22507 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/ctype_defination.py
--rw-rw-r--   0 root         (0) root         (0)    33054 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/idf_interface.py
--rw-rw-r--   0 root         (0) root         (0)      287 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/codegen/template/
--rw-rw-r--   0 root         (0) root         (0)     5781 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/client.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2888 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/client.h.mako
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/interface.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2297 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/interface.introspect.xml.mako
--rw-rw-r--   0 root         (0) root         (0)    40159 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/public.c.mako
--rw-rw-r--   0 root         (0) root         (0)     9070 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/public.h.mako
--rw-rw-r--   0 root         (0) root         (0)    13180 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/server.c.mako
--rw-rw-r--   0 root         (0) root         (0)     1440 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/codegen/template/server.h.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/component/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2155 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/arg_parser.py
--rw-rw-r--   0 root         (0) root         (0)    13224 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/component/template/
--rw-rw-r--   0 root         (0) root         (0)     9157 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/template/conanbase.mako
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/template/deploy.mako
--rw-rw-r--   0 root         (0) root         (0)     5554 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/component/test.py
--rw-rw-r--   0 root         (0) root         (0)     2119 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/errors.py
--rw-rw-r--   0 root         (0) root         (0)      829 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2762 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/build_manifest.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/build_prepare.py
--rw-rw-r--   0 root         (0) root         (0)     8475 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/build_rootfs.py
--rw-rw-r--   0 root         (0) root         (0)     2890 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/config.py
--rw-rw-r--   0 root         (0) root         (0)     4637 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit/integration/template/
--rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/integration/template/conanfile.py.mako
--rw-rw-r--   0 root         (0) root         (0)      114 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/lbkit.py
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/log.py
--rw-rw-r--   0 root         (0) root         (0)     3551 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/misc.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-28 16:23:09.000000 lbkit-0.5.7/lbkit/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 16:23:16.106330 lbkit-0.5.7/lbkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1268 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-28 16:23:16.000000 lbkit-0.5.7/lbkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 16:23:16.106330 lbkit-0.5.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1295 2024-04-28 16:23:09.000000 lbkit-0.5.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-05-03 18:32:59.000000 lbkit-0.5.8/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)    11357 2024-05-03 18:32:59.000000 lbkit-0.5.8/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      149 2024-05-03 18:32:59.000000 lbkit-0.5.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-03 18:33:06.637037 lbkit-0.5.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-05-03 18:32:59.000000 lbkit-0.5.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-03 18:33:00.000000 lbkit-0.5.8/lbkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/ci_robot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/ci_robot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12840 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/ci_robot/gitee.py
+-rw-rw-r--   0 root         (0) root         (0)     8483 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/codegen/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4241 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/codegen.py
+-rw-rw-r--   0 root         (0) root         (0)    22507 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/ctype_defination.py
+-rw-rw-r--   0 root         (0) root         (0)    33054 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/idf_interface.py
+-rw-rw-r--   0 root         (0) root         (0)      287 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/codegen/template/
+-rw-rw-r--   0 root         (0) root         (0)     6172 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/client.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     3048 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/client.h.mako
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/interface.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2297 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/interface.introspect.xml.mako
+-rw-rw-r--   0 root         (0) root         (0)    40581 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/public.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     9230 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/public.h.mako
+-rw-rw-r--   0 root         (0) root         (0)    13342 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/server.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     1629 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/server.h.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/component/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2155 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/arg_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    13224 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit/component/template/
+-rw-rw-r--   0 root         (0) root         (0)     9157 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/template/conanbase.mako
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/template/deploy.mako
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/test.py
+-rw-rw-r--   0 root         (0) root         (0)     2119 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/errors.py
+-rw-rw-r--   0 root         (0) root         (0)      829 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit/integration/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2762 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/build_manifest.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/build_prepare.py
+-rw-rw-r--   0 root         (0) root         (0)     8475 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/build_rootfs.py
+-rw-rw-r--   0 root         (0) root         (0)     2890 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4637 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit/integration/template/
+-rw-rw-r--   0 root         (0) root         (0)     1276 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/template/conanfile.py.mako
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/lbkit.py
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/log.py
+-rw-rw-r--   0 root         (0) root         (0)     3551 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 18:33:06.637037 lbkit-0.5.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1295 2024-05-03 18:32:59.000000 lbkit-0.5.8/setup.py
```

### Comparing `lbkit-0.5.7/LICENSE` & `lbkit-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/PKG-INFO` & `lbkit-0.5.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.7/lbkit/ci_robot/gitee.py` & `lbkit-0.5.8/lbkit/ci_robot/gitee.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/cli.py` & `lbkit-0.5.8/lbkit/cli.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/codegen/codegen.py` & `lbkit-0.5.8/lbkit/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/codegen/ctype_defination.py` & `lbkit-0.5.8/lbkit/codegen/ctype_defination.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/codegen/idf_interface.py` & `lbkit-0.5.8/lbkit/codegen/idf_interface.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/codegen/template/client.c.mako` & `lbkit-0.5.8/lbkit/codegen/template/client.c.mako`

 * *Files 8% similar despite different names*

```diff
@@ -41,36 +41,51 @@
         g_variant_unref(out);
     }
     return ret;
 }
 % endfor
 
 % for method in intf.methods:
+<% RSP_PARA = f'' %>\
+<% REQ_PARA = f'' %>\
+    % if len(method.returns.parameters) > 0:
+<% RSP_PARA = f'{intf.alias}_{method.name}_Rsp **rsp, ' %>\
+    % endif
+    % if len(method.parameters.parameters) > 0:
+<% REQ_PARA = f'const {intf.alias}_{method.name}_Req *req, ' %>\
+    % endif
 /*
  * ${method.description}
  *
  * method name: ${method.name}
     % for arg in method.parameters.parameters:
  *   @in_${arg.name}: ${arg.description}, signature: ${arg.signature}
     % endfor
     % for arg in method.returns.parameters:
  *   @out_${arg.name}: ${arg.description}, signature: ${arg.signature}
     % endfor
  */
-int ${class_name}_Call_${method.name}(const ${class_name} *object, const ${intf.alias}_${method.name}_Req *req,
-    ${intf.alias}_${method.name}_Rsp **rsp, gint timeout, GError **error)
+int ${class_name}_Call_${method.name}(const ${class_name} *object,
+    ${REQ_PARA}${RSP_PARA}gint timeout,
+    GError **error)
 {
     if (error == NULL) {
         log_error("Emit method ${method.name} with parameter error, error is NULL");
         return -1;
     }
     if (object == NULL) {
         *error = g_error_new(G_DBUS_ERROR, G_DBUS_ERROR_FAILED, "Call method ${method.name} with parameter error, object is NULL");
         return -1;
     }
+    % if len(method.returns.parameters) == 0:
+    void **rsp = NULL;
+    % endif
+    % if len(method.parameters.parameters) == 0:
+    void *req = NULL;
+    % endif
     return gcl_impl.call_method((GclObject *)object, (const GclMethod *)&${method_processer}->${method.name},
                                  (void *)req, (void **)rsp, timeout, error);
 }
 % endfor
 
 static GclObject *_${class_name}_create(const gchar *obj_name, gpointer opaque);
 /*
```

### Comparing `lbkit-0.5.7/lbkit/codegen/template/client.h.mako` & `lbkit-0.5.8/lbkit/codegen/template/client.h.mako`

 * *Files 22% similar despite different names*

```diff
@@ -25,23 +25,31 @@
     GError **error);
     % endif
 gint ${class_name}_get_${prop.name}(const ${class_name} *object, GVariant **value,
     GError **error);
 % endfor
 
 % for method in intf.methods:
+<% RSP_PARA = f'' %>\
+<% REQ_PARA = f'' %>\
+    % if len(method.returns.parameters) > 0:
+<% RSP_PARA = f'{intf.alias}_{method.name}_Rsp **rsp, ' %>\
+    % endif
+    % if len(method.parameters.parameters) > 0:
+<% REQ_PARA = f'const {intf.alias}_{method.name}_Req *req, ' %>\
+    % endif
 /* method.description */
     % if method.deprecated:
 __attribute__((__deprecated__)) int ${class_name}_Call_${method.name}(const ${class_name} *object,
-    const ${intf.alias}_${method.name}_Req *req, ${intf.alias}_${method.name}_Rsp **rsp,
-    gint timeout, GError **error);
+    ${REQ_PARA}${RSP_PARA}gint timeout,
+    GError **error);
     % else:
 int ${class_name}_Call_${method.name}(const ${class_name} *object,
-    const ${intf.alias}_${method.name}_Req *req, ${intf.alias}_${method.name}_Rsp **rsp,
-    gint timeout, GError **error);
+    ${REQ_PARA}${RSP_PARA}gint timeout,
+    GError **error);
     % endif
 % endfor
 
 % for signal in intf.signals:
 /* ${signal.description} */
 typedef void (*${class_name}_${signal.name}_Signal)(const ${class_name} *object, const gchar *destination,
     const ${intf.alias}_${signal.name}_Msg *req, gpointer user_data);
```

### Comparing `lbkit-0.5.7/lbkit/codegen/template/interface.introspect.xml.mako` & `lbkit-0.5.8/lbkit/codegen/template/interface.introspect.xml.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/codegen/template/public.c.mako` & `lbkit-0.5.8/lbkit/codegen/template/public.c.mako`

 * *Files 2% similar despite different names*

```diff
@@ -1024,24 +1024,38 @@
             break;
         }
         old_handler = NULL;
     }
     g_mutex_unlock(&_${class_name}_${action.name}_lock);
 }
 
-int ${class_name}_${action.name}_run(const ${class_name} *object, const ${class_name}_${action.name}_Req *req, ${class_name}_${action.name}_Rsp **rsp)
+<% RSP_PARA = f'' %>\
+<% REQ_PARA = f'' %>\
+<% REQ_NAME = f'' %>\
+    % if len(action.returns.parameters) > 0:
+<% RSP_PARA = f', {class_name}_{action.name}_Rsp **rsp' %>\
+    % endif
+    % if len(action.parameters.parameters) > 0:
+<% REQ_PARA = f', const {class_name}_{action.name}_Req *req' %>\
+<% REQ_NAME = f', req' %>\
+    % endif
+int ${class_name}_${action.name}_run(const ${class_name} *object${REQ_PARA}${RSP_PARA})
 {
     gint result = 0;
     g_mutex_lock(&_${class_name}_${action.name}_lock);
     for (GSList *item = _${class_name}_${action.name}_actions; item; item = item->next) {
+        _${class_name}_${action.name}_PluginAction *handler = (_${class_name}_${action.name}_PluginAction *)item->data;
+    % if len(action.returns.parameters) > 0:
         if (rsp && *rsp) {
             ${class_name}_${action.name}_Rsp_free(rsp);
         }
-        _${class_name}_${action.name}_PluginAction *handler = (_${class_name}_${action.name}_PluginAction *)item->data;
-        gint ret = handler->action(object, req, rsp, handler->user_data);
+        gint ret = handler->action(object${REQ_NAME}, rsp, handler->user_data);
+    % else:
+        gint ret = handler->action(object${REQ_NAME}, handler->user_data);
+    % endif
         if (ret != 0)
             result = ret;
         % if action.policy == "return_any_success":
         /* return when any action success(ret == 0) */
         if (ret == 0)
             break;
         % elif action.policy == "return_any_fail":
```

### Comparing `lbkit-0.5.7/lbkit/codegen/template/public.h.mako` & `lbkit-0.5.8/lbkit/codegen/template/public.h.mako`

 * *Files 4% similar despite different names*

```diff
@@ -172,21 +172,29 @@
     } ${method.name};
 % endfor
     GclMethod __reserved__;
 } ${class_name}_Methods;
 
 % if len(intf.plugin.actions) > 0:
 % for action in intf.plugin.actions:
-typedef int (*${class_name}_${action.name}_action)(const ${class_name} *object, const ${class_name}_${action.name}_Req *req, ${class_name}_${action.name}_Rsp **rsp, gpointer user_data);
+<% RSP_PARA = f'' %>\
+<% REQ_PARA = f'' %>\
+    % if len(action.returns.parameters) > 0:
+<% RSP_PARA = f', {class_name}_{action.name}_Rsq **rsp' %>\
+    % endif
+    % if len(action.parameters.parameters) > 0:
+<% REQ_PARA = f', const {class_name}_{action.name}_Req *req' %>\
+    % endif
+typedef int (*${class_name}_${action.name}_action)(const ${class_name} *object${REQ_PARA}${RSP_PARA}, gpointer user_data);
 
 /* Register a new plugin action, can't register repeated with same action and user_data */
 int ${class_name}_${action.name}_register(const gchar *req_signature, const gchar *rsp_signature,
     ${class_name}_${action.name}_action action, gpointer user_data);
 void ${class_name}_${action.name}_unregister(${class_name}_${action.name}_action action);
-int ${class_name}_${action.name}_run(const ${class_name} *object, const ${class_name}_${action.name}_Req *req, ${class_name}_${action.name}_Rsp **rsp);
+int ${class_name}_${action.name}_run(const ${class_name} *object${REQ_PARA}${RSP_PARA});
 
 % endfor
 % endif
 ### 开始生成方法的请求体、响应体和处理函数
 % for signal in intf.signals:
 /* ${signal.name}信号的消息体 */
 typedef struct {
```

### Comparing `lbkit-0.5.7/lbkit/codegen/template/server.c.mako` & `lbkit-0.5.8/lbkit/codegen/template/server.c.mako`

 * *Files 4% similar despite different names*

```diff
@@ -209,30 +209,37 @@
 
 % endfor
 % for signal in intf.signals:
 /*
  * Signal: ${signal.name}
  * ${signal.description}
  */
+<% REQ_PARA = f'' %>\
+    % if len(signal.properties.parameters) > 0:
+<% REQ_PARA = f'const {class_name}_{signal.name}_Msg *msg, ' %>\
+    % endif
     % if signal.deprecated:
 __attribute__((__deprecated__)) gboolean ${class_name}_${signal.name}_Signal(const ${class_name} *object,
-    const gchar *destination, const ${class_name}_${signal.name}_Msg *msg, GError **error)
+    const gchar *destination, ${REQ_PARA}GError **error)
     % else:
 gboolean ${class_name}_${signal.name}_Signal(const ${class_name} *object, const gchar *destination,
-    const ${class_name}_${signal.name}_Msg *msg, GError **error)
+    ${REQ_PARA}GError **error)
     % endif
 {
     if (error == NULL) {
         log_error("Emit ${signal.name} with parameter error, error is NULL");
         return FALSE;
     }
     if (object == NULL) {
         *error = g_error_new(G_DBUS_ERROR, G_DBUS_ERROR_FAILED, "Emit ${signal.name} with parameter error, object is NULL");
         return FALSE;
     }
+    % if len(signal.properties.parameters) == 0:
+    void *msg = NULL;
+    % endif
     return gcl_impl.emit_signal((GclObject *)object, destination,
         (const GclSignal *)&${signal_processer}->${signal.name}, msg, error);
 }
 
 % endfor
 static GclObject *_${class_name}_create(const gchar *obj_name, gpointer opaque);
 static void _load_from_odf(yaml_document_t *doc, yaml_node_t *node, GclObject *gcl_obj,
```

### Comparing `lbkit-0.5.7/lbkit/codegen/template/server.h.mako` & `lbkit-0.5.8/lbkit/codegen/template/server.h.mako`

 * *Files 22% similar despite different names*

```diff
@@ -22,15 +22,19 @@
     % endif
 % endfor
 
 % for signal in intf.signals:
 /*
  * ${signal.description}
  */
-gboolean ${class_name}_${signal.name}_Signal(const ${class_name} *object, const gchar *destination, const ${class_name}_${signal.name}_Msg *req, GError **error);
+    % if len(signal.properties.parameters) > 0:
+gboolean ${class_name}_${signal.name}_Signal(const ${class_name} *object, const gchar *destination, const ${class_name}_${signal.name}_Msg *msg, GError **error);
+    % else:
+gboolean ${class_name}_${signal.name}_Signal(const ${class_name} *object, const gchar *destination, GError **error);
+    % endif
 % endfor
 
 #define ${class_name.upper()}_NAME    "${intf.name}"
 % for prop in intf.properties:
 #define ${class_name.upper()}_${prop.name}_NAME    "${prop.name}"
 % endfor
```

### Comparing `lbkit-0.5.7/lbkit/component/arg_parser.py` & `lbkit-0.5.8/lbkit/component/arg_parser.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/component/build.py` & `lbkit-0.5.8/lbkit/component/build.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/component/template/conanbase.mako` & `lbkit-0.5.8/lbkit/component/template/conanbase.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/component/template/deploy.mako` & `lbkit-0.5.8/lbkit/component/template/deploy.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/component/test.py` & `lbkit-0.5.8/lbkit/component/test.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/errors.py` & `lbkit-0.5.8/lbkit/errors.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/helper.py` & `lbkit-0.5.8/lbkit/helper.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/integration/build_manifest.py` & `lbkit-0.5.8/lbkit/integration/build_manifest.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/integration/build_prepare.py` & `lbkit-0.5.8/lbkit/integration/build_prepare.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/integration/build_rootfs.py` & `lbkit-0.5.8/lbkit/integration/build_rootfs.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/integration/config.py` & `lbkit-0.5.8/lbkit/integration/config.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/integration/task.py` & `lbkit-0.5.8/lbkit/integration/task.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/integration/template/conanfile.py.mako` & `lbkit-0.5.8/lbkit/integration/template/conanfile.py.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/log.py` & `lbkit-0.5.8/lbkit/log.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/misc.py` & `lbkit-0.5.8/lbkit/misc.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit/tools.py` & `lbkit-0.5.8/lbkit/tools.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/lbkit.egg-info/PKG-INFO` & `lbkit-0.5.8/lbkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.7/lbkit.egg-info/SOURCES.txt` & `lbkit-0.5.8/lbkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.7/setup.py` & `lbkit-0.5.8/setup.py`

 * *Files identical despite different names*

