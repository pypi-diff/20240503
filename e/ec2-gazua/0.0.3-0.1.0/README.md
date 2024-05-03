# Comparing `tmp/ec2-gazua-0.0.3.tar.gz` & `tmp/ec2-gazua-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ec2-gazua-0.0.3.tar", last modified: Sat May 15 07:25:28 2021, max compression
+gzip compressed data, was "ec2-gazua-0.1.0.tar", last modified: Fri May  3 02:07:26 2024, max compression
```

## Comparing `ec2-gazua-0.0.3.tar` & `ec2-gazua-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hodolman   (501) staff       (20)        0 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/
--rw-r--r--   0 hodolman   (501) staff       (20)     1067 2020-02-03 08:10:32.000000 ec2-gazua-0.0.3/LICENSE
--rw-r--r--   0 hodolman   (501) staff       (20)       43 2021-05-15 07:24:52.000000 ec2-gazua-0.0.3/MANIFEST.in
--rw-r--r--   0 hodolman   (501) staff       (20)     1410 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/PKG-INFO
--rw-r--r--   0 hodolman   (501) staff       (20)     5385 2021-05-15 07:05:50.000000 ec2-gazua-0.0.3/README.md
-drwxr-xr-x   0 hodolman   (501) staff       (20)        0 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/
--rw-r--r--   0 hodolman   (501) staff       (20)     1410 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/PKG-INFO
--rw-r--r--   0 hodolman   (501) staff       (20)      465 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/SOURCES.txt
--rw-r--r--   0 hodolman   (501) staff       (20)        1 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/dependency_links.txt
--rw-r--r--   0 hodolman   (501) staff       (20)       40 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/entry_points.txt
--rw-r--r--   0 hodolman   (501) staff       (20)        1 2021-05-15 06:10:16.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/not-zip-safe
--rw-r--r--   0 hodolman   (501) staff       (20)       83 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/requires.txt
--rw-r--r--   0 hodolman   (501) staff       (20)       16 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2_gazua.egg-info/top_level.txt
--rwxr-xr-x   0 hodolman   (501) staff       (20)      122 2021-05-15 07:05:50.000000 ec2-gazua-0.0.3/ec2_gz.py
-drwxr-xr-x   0 hodolman   (501) staff       (20)        0 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/ec2gazua/
--rw-r--r--   0 hodolman   (501) staff       (20)        0 2021-04-09 03:34:54.000000 ec2-gazua-0.0.3/ec2gazua/__init__.py
--rw-r--r--   0 hodolman   (501) staff       (20)       59 2021-04-09 03:34:54.000000 ec2-gazua-0.0.3/ec2gazua/__main__.py
--rw-r--r--   0 hodolman   (501) staff       (20)     1166 2021-05-15 07:07:35.000000 ec2-gazua-0.0.3/ec2gazua/config.py
--rw-r--r--   0 hodolman   (501) staff       (20)     5670 2021-05-15 07:05:50.000000 ec2-gazua-0.0.3/ec2gazua/ec2.py
--rw-r--r--   0 hodolman   (501) staff       (20)    10272 2021-05-14 01:31:40.000000 ec2-gazua-0.0.3/ec2gazua/gazua.py
--rw-r--r--   0 hodolman   (501) staff       (20)     1499 2021-04-09 03:34:54.000000 ec2-gazua-0.0.3/ec2gazua/logger.py
--rw-r--r--   0 hodolman   (501) staff       (20)     1508 2021-04-09 03:34:54.000000 ec2-gazua-0.0.3/ec2gazua/tmux.py
--rw-r--r--   0 hodolman   (501) staff       (20)      280 2021-04-09 03:34:54.000000 ec2-gazua-0.0.3/ec2gazua/utils.py
--rw-r--r--   0 hodolman   (501) staff       (20)     3211 2021-04-09 03:34:54.000000 ec2-gazua-0.0.3/ec2gazua/widget.py
--rw-r--r--   0 hodolman   (501) staff       (20)       83 2021-05-15 07:05:50.000000 ec2-gazua-0.0.3/requirements.txt
--rw-r--r--   0 hodolman   (501) staff       (20)       38 2021-05-15 07:25:28.000000 ec2-gazua-0.0.3/setup.cfg
--rw-r--r--   0 hodolman   (501) staff       (20)      884 2021-05-15 07:25:09.000000 ec2-gazua-0.0.3/setup.py
+drwxr-xr-x   0 hodolman   (501) staff       (20)        0 2024-05-03 02:07:26.300726 ec2-gazua-0.1.0/
+-rw-r--r--   0 hodolman   (501) staff       (20)     1067 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/LICENSE
+-rw-r--r--   0 hodolman   (501) staff       (20)       43 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/MANIFEST.in
+-rw-r--r--   0 hodolman   (501) staff       (20)     1561 2024-05-03 02:07:26.300590 ec2-gazua-0.1.0/PKG-INFO
+-rw-r--r--   0 hodolman   (501) staff       (20)     5385 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/README.md
+drwxr-xr-x   0 hodolman   (501) staff       (20)        0 2024-05-03 02:07:26.298800 ec2-gazua-0.1.0/ec2_gazua.egg-info/
+-rw-r--r--   0 hodolman   (501) staff       (20)     1561 2024-05-03 02:07:26.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/PKG-INFO
+-rw-r--r--   0 hodolman   (501) staff       (20)      465 2024-05-03 02:07:26.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/SOURCES.txt
+-rw-r--r--   0 hodolman   (501) staff       (20)        1 2024-05-03 02:07:26.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/dependency_links.txt
+-rw-r--r--   0 hodolman   (501) staff       (20)       39 2024-05-03 02:07:26.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/entry_points.txt
+-rw-r--r--   0 hodolman   (501) staff       (20)        1 2024-05-03 02:01:35.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/not-zip-safe
+-rw-r--r--   0 hodolman   (501) staff       (20)       87 2024-05-03 02:07:26.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/requires.txt
+-rw-r--r--   0 hodolman   (501) staff       (20)       16 2024-05-03 02:07:26.000000 ec2-gazua-0.1.0/ec2_gazua.egg-info/top_level.txt
+-rwxr-xr-x   0 hodolman   (501) staff       (20)      122 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2_gz.py
+drwxr-xr-x   0 hodolman   (501) staff       (20)        0 2024-05-03 02:07:26.300280 ec2-gazua-0.1.0/ec2gazua/
+-rw-r--r--   0 hodolman   (501) staff       (20)        0 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/__init__.py
+-rw-r--r--   0 hodolman   (501) staff       (20)       59 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/__main__.py
+-rw-r--r--   0 hodolman   (501) staff       (20)     1166 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/config.py
+-rw-r--r--   0 hodolman   (501) staff       (20)     5670 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/ec2.py
+-rw-r--r--   0 hodolman   (501) staff       (20)    10272 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/gazua.py
+-rw-r--r--   0 hodolman   (501) staff       (20)     1499 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/logger.py
+-rw-r--r--   0 hodolman   (501) staff       (20)     1508 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/tmux.py
+-rw-r--r--   0 hodolman   (501) staff       (20)      280 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/utils.py
+-rw-r--r--   0 hodolman   (501) staff       (20)     3211 2024-05-03 01:46:11.000000 ec2-gazua-0.1.0/ec2gazua/widget.py
+-rw-r--r--   0 hodolman   (501) staff       (20)       87 2024-05-03 01:58:56.000000 ec2-gazua-0.1.0/requirements.txt
+-rw-r--r--   0 hodolman   (501) staff       (20)       38 2024-05-03 02:07:26.300769 ec2-gazua-0.1.0/setup.cfg
+-rw-r--r--   0 hodolman   (501) staff       (20)      884 2024-05-03 01:58:56.000000 ec2-gazua-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ec2-gazua-0.0.3/LICENSE` & `ec2-gazua-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/PKG-INFO` & `ec2-gazua-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ec2-gazua
-Version: 0.0.3
+Version: 0.1.0
 Summary: Easy accessing EC2 SSH through tmux
 Home-page: https://github.com/leejaycoke/ec2-gazua
 Author: leejaycoke
 Author-email: leejaycoke@gmail.com
 License: MIT License
-
-Copyright (c) 2018 JuHyun Lee
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-Description: UNKNOWN
+        
+        Copyright (c) 2018 JuHyun Lee
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Keywords: ec2 ssh
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
+License-File: LICENSE
```

### Comparing `ec2-gazua-0.0.3/README.md` & `ec2-gazua-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/ec2_gazua.egg-info/PKG-INFO` & `ec2-gazua-0.1.0/ec2_gazua.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ec2-gazua
-Version: 0.0.3
+Version: 0.1.0
 Summary: Easy accessing EC2 SSH through tmux
 Home-page: https://github.com/leejaycoke/ec2-gazua
 Author: leejaycoke
 Author-email: leejaycoke@gmail.com
 License: MIT License
-
-Copyright (c) 2018 JuHyun Lee
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-Description: UNKNOWN
+        
+        Copyright (c) 2018 JuHyun Lee
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Keywords: ec2 ssh
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
+License-File: LICENSE
```

### Comparing `ec2-gazua-0.0.3/ec2gazua/config.py` & `ec2-gazua-0.1.0/ec2gazua/config.py`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/ec2gazua/ec2.py` & `ec2-gazua-0.1.0/ec2gazua/ec2.py`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/ec2gazua/gazua.py` & `ec2-gazua-0.1.0/ec2gazua/gazua.py`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/ec2gazua/logger.py` & `ec2-gazua-0.1.0/ec2gazua/logger.py`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/ec2gazua/tmux.py` & `ec2-gazua-0.1.0/ec2gazua/tmux.py`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/ec2gazua/widget.py` & `ec2-gazua-0.1.0/ec2gazua/widget.py`

 * *Files identical despite different names*

### Comparing `ec2-gazua-0.0.3/setup.py` & `ec2-gazua-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = [line.strip() for line in fp.readlines()]
 
 with open('LICENSE') as f:
     mit_license = f.read()
 
 setup(
     name='ec2-gazua',
-    version='0.0.3',
+    version='0.1.0',
     description='Easy accessing EC2 SSH through tmux',
     author='leejaycoke',
     author_email='leejaycoke@gmail.com',
     url='https://github.com/leejaycoke/ec2-gazua',
     license=mit_license,
     install_requires=requirements,
     packages=find_packages(include=['ec2gazua'], exclude=['tests', 'image']),
```

