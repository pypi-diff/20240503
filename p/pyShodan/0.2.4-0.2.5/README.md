# Comparing `tmp/pyShodan-0.2.4.tar.gz` & `tmp/pyShodan-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyShodan-0.2.4.tar", last modified: Wed Jun  2 16:53:09 2021, max compression
+gzip compressed data, was "dist/pyShodan-0.2.5.tar", last modified: Wed Jun  2 18:33:01 2021, max compression
```

## Comparing `pyShodan-0.2.4.tar` & `pyShodan-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 sscott    (1000) sscott    (1000)        0 2021-06-02 16:53:09.000000 pyShodan-0.2.4/
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)     7651 2019-05-06 00:26:16.000000 pyShodan-0.2.4/LICENSE
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)     1537 2021-06-02 16:53:09.000000 pyShodan-0.2.4/PKG-INFO
-drwxrwxrwx   0 sscott    (1000) sscott    (1000)        0 2021-06-02 16:53:09.000000 pyShodan-0.2.4/pyShodan/
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)     3968 2021-06-02 16:28:05.000000 pyShodan-0.2.4/pyShodan/test.py
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)     4646 2021-06-02 16:28:05.000000 pyShodan-0.2.4/pyShodan/__init__.py
-drwxrwxrwx   0 sscott    (1000) sscott    (1000)        0 2021-06-02 16:53:09.000000 pyShodan-0.2.4/pyShodan.egg-info/
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)        1 2021-06-02 16:53:08.000000 pyShodan-0.2.4/pyShodan.egg-info/dependency_links.txt
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)     1537 2021-06-02 16:53:08.000000 pyShodan-0.2.4/pyShodan.egg-info/PKG-INFO
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)       11 2021-06-02 16:53:08.000000 pyShodan-0.2.4/pyShodan.egg-info/requires.txt
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)      223 2021-06-02 16:53:09.000000 pyShodan-0.2.4/pyShodan.egg-info/SOURCES.txt
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)        9 2021-06-02 16:53:08.000000 pyShodan-0.2.4/pyShodan.egg-info/top_level.txt
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)      972 2021-06-02 16:52:46.000000 pyShodan-0.2.4/README.md
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)       38 2021-06-02 16:53:09.000000 pyShodan-0.2.4/setup.cfg
--rwxrwxrwx   0 sscott    (1000) sscott    (1000)      767 2021-06-02 16:49:13.000000 pyShodan-0.2.4/setup.py
+drwxrwxrwx   0 sscott    (1000) sscott    (1000)        0 2021-06-02 18:33:01.000000 pyShodan-0.2.5/
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)     7651 2019-05-06 00:26:16.000000 pyShodan-0.2.5/LICENSE
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)     1537 2021-06-02 18:33:01.000000 pyShodan-0.2.5/PKG-INFO
+drwxrwxrwx   0 sscott    (1000) sscott    (1000)        0 2021-06-02 18:33:01.000000 pyShodan-0.2.5/pyShodan/
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)     3968 2021-06-02 16:28:05.000000 pyShodan-0.2.5/pyShodan/test.py
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)     4646 2021-06-02 16:28:05.000000 pyShodan-0.2.5/pyShodan/__init__.py
+drwxrwxrwx   0 sscott    (1000) sscott    (1000)        0 2021-06-02 18:33:01.000000 pyShodan-0.2.5/pyShodan.egg-info/
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)        1 2021-06-02 18:33:00.000000 pyShodan-0.2.5/pyShodan.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)     1537 2021-06-02 18:33:00.000000 pyShodan-0.2.5/pyShodan.egg-info/PKG-INFO
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)       11 2021-06-02 18:33:00.000000 pyShodan-0.2.5/pyShodan.egg-info/requires.txt
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)      223 2021-06-02 18:33:00.000000 pyShodan-0.2.5/pyShodan.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)        9 2021-06-02 18:33:00.000000 pyShodan-0.2.5/pyShodan.egg-info/top_level.txt
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)      972 2021-06-02 16:52:46.000000 pyShodan-0.2.5/README.md
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)       38 2021-06-02 18:33:01.000000 pyShodan-0.2.5/setup.cfg
+-rwxrwxrwx   0 sscott    (1000) sscott    (1000)      767 2021-06-02 18:32:48.000000 pyShodan-0.2.5/setup.py
```

### Comparing `pyShodan-0.2.4/LICENSE` & `pyShodan-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyShodan-0.2.4/PKG-INFO` & `pyShodan-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyShodan
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library for querying the Shodan API
 Home-page: https://github.com/GoVanguard/pyShodan
 Author: Shane Scott
 Author-email: sscott@gvit.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyShodan-0.2.4/pyShodan/test.py` & `pyShodan-0.2.5/pyShodan/test.py`

 * *Files identical despite different names*

### Comparing `pyShodan-0.2.4/pyShodan/__init__.py` & `pyShodan-0.2.5/pyShodan/__init__.py`

 * *Files identical despite different names*

### Comparing `pyShodan-0.2.4/pyShodan.egg-info/PKG-INFO` & `pyShodan-0.2.5/pyShodan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyShodan
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library for querying the Shodan API
 Home-page: https://github.com/GoVanguard/pyShodan
 Author: Shane Scott
 Author-email: sscott@gvit.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyShodan-0.2.4/README.md` & `pyShodan-0.2.5/README.md`

 * *Files identical despite different names*

