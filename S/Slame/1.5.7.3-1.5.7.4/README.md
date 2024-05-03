# Comparing `tmp/Slame-1.5.7.3.tar.gz` & `tmp/Slame-1.5.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slame-1.5.7.3.tar", last modified: Thu May  2 18:26:19 2024, max compression
+gzip compressed data, was "Slame-1.5.7.4.tar", last modified: Thu May  2 18:30:44 2024, max compression
```

## Comparing `Slame-1.5.7.3.tar` & `Slame-1.5.7.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-02 18:26:19.939038 Slame-1.5.7.3/
--rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-02 18:26:19.939038 Slame-1.5.7.3/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.7.3/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-02 18:26:19.939038 Slame-1.5.7.3/Slame/
--rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.7.3/Slame/__init__.py
--rw-r--r--   0 dev       (1000) dev       (1000)    11589 2024-05-02 18:24:48.000000 Slame-1.5.7.3/Slame/slame.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-02 18:26:19.939038 Slame-1.5.7.3/Slame.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-02 18:26:19.000000 Slame-1.5.7.3/Slame.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-02 18:26:19.000000 Slame-1.5.7.3/Slame.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-02 18:26:19.000000 Slame-1.5.7.3/Slame.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-02 18:26:19.000000 Slame-1.5.7.3/Slame.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-02 18:26:19.000000 Slame-1.5.7.3/Slame.egg-info/top_level.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-02 18:26:19.939038 Slame-1.5.7.3/setup.cfg
--rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-02 18:25:29.000000 Slame-1.5.7.3/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-02 18:30:44.844152 Slame-1.5.7.4/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      897 2024-05-02 18:30:44.844152 Slame-1.5.7.4/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5.7.4/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-02 18:30:44.844152 Slame-1.5.7.4/Slame/
+-rw-r--r--   0 dev       (1000) dev       (1000)      233 2024-04-29 14:45:27.000000 Slame-1.5.7.4/Slame/__init__.py
+-rw-r--r--   0 dev       (1000) dev       (1000)    11525 2024-05-02 18:29:38.000000 Slame-1.5.7.4/Slame/slame.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-05-02 18:30:44.844152 Slame-1.5.7.4/Slame.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      897 2024-05-02 18:30:44.000000 Slame-1.5.7.4/Slame.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      205 2024-05-02 18:30:44.000000 Slame-1.5.7.4/Slame.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-05-02 18:30:44.000000 Slame-1.5.7.4/Slame.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       19 2024-05-02 18:30:44.000000 Slame-1.5.7.4/Slame.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-05-02 18:30:44.000000 Slame-1.5.7.4/Slame.egg-info/top_level.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-05-02 18:30:44.844152 Slame-1.5.7.4/setup.cfg
+-rw-r--r--   0 dev       (1000) dev       (1000)     1255 2024-05-02 18:30:33.000000 Slame-1.5.7.4/setup.py
```

### Comparing `Slame-1.5.7.3/PKG-INFO` & `Slame-1.5.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.7.3
+Version: 1.5.7.4
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.7.3/README.md` & `Slame-1.5.7.4/README.md`

 * *Files identical despite different names*

### Comparing `Slame-1.5.7.3/Slame/slame.py` & `Slame-1.5.7.4/Slame/slame.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                     content_length = self.get_content_length(request_data)
                     data = self.parse_post_data(request_data, content_length)
                     response = route['handler'](data)
                 else:
                     response = route['handler']()
 
                 response_headers = "HTTP/1.1 200 OK\n\n"
-                return response_headers.encode('utf-8') + response.encode('utf-8')
+                return response_headers + response
             else:
                 return "HTTP/1.1 405 Method Not Allowed\n\n405 Method Not Allowed"
         elif path.startswith('/static/'):
             return self.serve_static_file(path)
         else:
             return "HTTP/1.1 404 Not Found\n\n404 Not Found"
 
@@ -83,15 +83,15 @@
         script_dir = os.path.dirname(os.path.abspath(__file__))
         abs_file_path = os.path.join(script_dir, "static", path[1:])
 
         try:
             with open(abs_file_path, 'rb') as file:
                 content = file.read()
             response_headers = "HTTP/1.1 200 OK\n\n"
-            return response_headers.encode('utf-8') + content.encode('utf-8')
+            return response_headers + content
         except FileNotFoundError:
             return "HTTP/1.1 404 Not Found\n\n404 Not Found"
 
     def get_content_length(self, request_data):
         for line in request_data.split('\n'):
             if line.startswith('Content-Length:'):
                 return int(line.split(':')[1])
```

### Comparing `Slame-1.5.7.3/Slame.egg-info/PKG-INFO` & `Slame-1.5.7.4/Slame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.5.7.3
+Version: 1.5.7.4
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.5.7.3/setup.py` & `Slame-1.5.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 :authors: ZHRXXgroup
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 ZHRXXgroup
 """
 
-version = '1.5.7.3'
+version = '1.5.7.4'
 
 long_description  = "Slame is an Python Module for serving a webserver and in 1.2 we added Plugins you can use your own plugins in Slame or you can download plugins from other Peoples at https://zhrxxgroup.com/slame/spm/. SLAME DOCS: https://zhrxxgroup.com/slame or https://github.com/zhrexx/Slame, OUR WEBSITE: https://zhrxxgroup.com"
 
 
 
 setup(
     name="Slame",
```

