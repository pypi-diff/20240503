# Comparing `tmp/xontrib-pipeliner-0.4.3.tar.gz` & `tmp/xontrib_pipeliner-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-pipeliner-0.4.3.tar", last modified: Wed Apr  3 11:30:04 2024, max compression
+gzip compressed data, was "xontrib_pipeliner-0.4.4.tar", last modified: Thu May  2 22:15:08 2024, max compression
```

## Comparing `xontrib-pipeliner-0.4.3.tar` & `xontrib_pipeliner-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.256156 xontrib-pipeliner-0.4.3/xontrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/xontrib/pipeliner/
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib/pipeliner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib/pipeliner/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/asttokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/line_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/mark_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:15:08.286041 xontrib_pipeliner-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-02 22:15:08.286041 xontrib_pipeliner-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:15:08.286041 xontrib_pipeliner-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:15:08.282041 xontrib_pipeliner-0.4.4/xontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:15:08.286041 xontrib_pipeliner-0.4.4/xontrib/pipeliner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib/pipeliner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib/pipeliner/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:15:08.286041 xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-02 22:15:08.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-02 22:15:08.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:15:08.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 22:15:08.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 22:15:08.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:15:08.286041 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/asttokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/line_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/mark_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 22:14:55.000000 xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/version.py
```

### Comparing `xontrib-pipeliner-0.4.3/LICENSE` & `xontrib_pipeliner-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/PKG-INFO` & `xontrib_pipeliner-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-pipeliner
-Version: 0.4.3
+Version: 0.4.4
 Summary: Easily process the lines using pipes in xonsh.
 Home-page: https://github.com/anki-code/xontrib-pipeliner
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-pipeliner/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-pipeliner
```

### Comparing `xontrib-pipeliner-0.4.3/README.md` & `xontrib_pipeliner-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/setup.py` & `xontrib_pipeliner-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setup(
     name='xontrib-pipeliner',
-    version='0.4.3',
+    version='0.4.4',
     license='BSD',
     author='anki',
     author_email='author@example.com',
     description="Easily process the lines using pipes in xonsh.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xontrib-pipeliner-0.4.3/xontrib/pipeliner/__init__.py` & `xontrib_pipeliner-0.4.4/xontrib/pipeliner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return
 
     num = 0
     for line in stdin.readlines():
         try:
             res = fn(line.rstrip(os.linesep), num)
         except:
-            print_color('{YELLOW}' + f'Error line {num+1}: {line}', file=sys.stderr)
+            print_color('{YELLOW}' + f'Error line {num+1}: {line!r}', file=sys.stderr)
             print_color('{YELLOW}' + str(traceback.format_exc()), file=sys.stderr)
             return
         num += 1
         if res is not None:
             print(res, file=stdout, flush=True)
```

### Comparing `xontrib-pipeliner-0.4.3/xontrib/pipeliner/parallel.py` & `xontrib_pipeliner-0.4.4/xontrib/pipeliner/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
        except:
            pass
        ctx['line'] = args[0]
        ctx['num'] = args[1]
        try:
            return eval(self.code, ctx)
        except:
-           print_color('{YELLOW}' + f'Error line {args[1]+1}: {args[0]}', file=sys.stderr)
+           print_color('{YELLOW}' + f'Error line {args[1]+1}: {args[0]!r}', file=sys.stderr)
            print_color('{YELLOW}' + str(traceback.format_exc()), file=sys.stderr)           
            return None
 
    def go(self, func_args, stdout):
        with Pool(cpu_count()) as p:
            parallel_tasks = p.imap_unordered(self, func_args)
            for result in parallel_tasks:
```

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/PKG-INFO` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-pipeliner
-Version: 0.4.3
+Version: 0.4.4
 Summary: Easily process the lines using pipes in xonsh.
 Home-page: https://github.com/anki-code/xontrib-pipeliner
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-pipeliner/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-pipeliner
```

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/SOURCES.txt` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/__init__.py` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/__init__.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/asttokens.py` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/asttokens.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/line_numbers.py` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/line_numbers.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/mark_tokens.py` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/mark_tokens.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/util.py` & `xontrib_pipeliner-0.4.4/xontrib_pipeliner_asttokens/util.py`

 * *Files identical despite different names*

