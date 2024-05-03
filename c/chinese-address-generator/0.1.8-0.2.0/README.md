# Comparing `tmp/chinese_address_generator-0.1.8.tar.gz` & `tmp/chinese_address_generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chinese_address_generator-0.1.8.tar", last modified: Sat Aug 13 09:02:29 2022, max compression
+gzip compressed data, was "chinese_address_generator-0.2.0.tar", last modified: Fri May  3 13:43:21 2024, max compression
```

## Comparing `chinese_address_generator-0.1.8.tar` & `chinese_address_generator-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-08-13 09:02:29.851679 chinese_address_generator-0.1.8/
--rw-rw-rw-   0        0        0     1090 2022-08-13 03:14:40.000000 chinese_address_generator-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      270 2022-08-13 09:02:29.850682 chinese_address_generator-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      468 2022-08-13 05:07:11.000000 chinese_address_generator-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-08-13 09:02:29.841707 chinese_address_generator-0.1.8/chinese_address_generator/
--rw-rw-rw-   0        0        0      702 2022-08-13 08:57:39.000000 chinese_address_generator-0.1.8/chinese_address_generator/__init__.py
--rw-rw-rw-   0        0        0      274 2022-08-13 09:01:55.000000 chinese_address_generator-0.1.8/chinese_address_generator/__main__.py
--rw-rw-rw-   0        0        0     2573 2022-08-13 09:01:40.000000 chinese_address_generator-0.1.8/chinese_address_generator/generator.py
-drwxrwxrwx   0        0        0        0 2022-08-13 09:02:29.847690 chinese_address_generator-0.1.8/chinese_address_generator/src/
--rw-rw-rw-   0        0        0   324270 2022-08-13 07:24:30.000000 chinese_address_generator-0.1.8/chinese_address_generator/src/level3.json
--rw-rw-rw-   0        0        0  1106120 2022-08-13 07:24:30.000000 chinese_address_generator-0.1.8/chinese_address_generator/src/level4.txt
-drwxrwxrwx   0        0        0        0 2022-08-13 09:02:29.845695 chinese_address_generator-0.1.8/chinese_address_generator.egg-info/
--rw-rw-rw-   0        0        0      270 2022-08-13 09:02:29.000000 chinese_address_generator-0.1.8/chinese_address_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2022-08-13 09:02:29.000000 chinese_address_generator-0.1.8/chinese_address_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-13 09:02:29.000000 chinese_address_generator-0.1.8/chinese_address_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-08-13 09:02:29.000000 chinese_address_generator-0.1.8/chinese_address_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-13 09:02:29.851679 chinese_address_generator-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      440 2022-08-13 09:02:24.000000 chinese_address_generator-0.1.8/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-03 13:43:21.286882 chinese_address_generator-0.2.0/
+-rw-r--r--   0 li         (501) staff       (20)     1065 2024-05-03 11:33:16.000000 chinese_address_generator-0.2.0/LICENSE
+-rw-r--r--   0 li         (501) staff       (20)     2883 2024-05-03 13:43:21.286634 chinese_address_generator-0.2.0/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)     2127 2024-05-03 13:18:56.000000 chinese_address_generator-0.2.0/README.md
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-03 13:43:21.283894 chinese_address_generator-0.2.0/chinese_address_generator/
+-rw-r--r--   0 li         (501) staff       (20)      887 2024-05-03 12:12:54.000000 chinese_address_generator-0.2.0/chinese_address_generator/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)       66 2024-05-03 12:40:35.000000 chinese_address_generator-0.2.0/chinese_address_generator/__main__.py
+-rw-r--r--   0 li         (501) staff       (20)     1179 2024-05-03 12:30:40.000000 chinese_address_generator-0.2.0/chinese_address_generator/cnaddrgen.py
+-rw-r--r--   0 li         (501) staff       (20)     5646 2024-05-03 11:07:56.000000 chinese_address_generator-0.2.0/chinese_address_generator/crawler.py
+-rw-r--r--   0 li         (501) staff       (20)     2733 2024-05-03 13:08:06.000000 chinese_address_generator-0.2.0/chinese_address_generator/generator.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-03 13:43:21.285459 chinese_address_generator-0.2.0/chinese_address_generator/src/
+-rw-r--r--   0 li         (501) staff       (20)    61783 2024-05-03 11:09:27.000000 chinese_address_generator-0.2.0/chinese_address_generator/src/new_level3.json
+-rw-r--r--   0 li         (501) staff       (20)   160857 2024-05-03 11:09:27.000000 chinese_address_generator-0.2.0/chinese_address_generator/src/new_level4.txt
+drwxr-xr-x   0 li         (501) staff       (20)        0 2024-05-03 13:43:21.286362 chinese_address_generator-0.2.0/chinese_address_generator.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)     2883 2024-05-03 13:43:21.000000 chinese_address_generator-0.2.0/chinese_address_generator.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)      556 2024-05-03 13:43:21.000000 chinese_address_generator-0.2.0/chinese_address_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2024-05-03 13:43:21.000000 chinese_address_generator-0.2.0/chinese_address_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)       71 2024-05-03 13:43:21.000000 chinese_address_generator-0.2.0/chinese_address_generator.egg-info/entry_points.txt
+-rw-r--r--   0 li         (501) staff       (20)       26 2024-05-03 13:43:21.000000 chinese_address_generator-0.2.0/chinese_address_generator.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)       38 2024-05-03 13:43:21.286931 chinese_address_generator-0.2.0/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)     1144 2024-05-03 13:43:14.000000 chinese_address_generator-0.2.0/setup.py
```

### Comparing `chinese_address_generator-0.1.8/LICENSE` & `chinese_address_generator-0.2.0/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 花恋流年
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
+MIT License
+
+Copyright (c) 2022 Ginkgoty
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chinese_address_generator-0.1.8/chinese_address_generator/generator.py` & `chinese_address_generator-0.2.0/chinese_address_generator/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 #!/usr/bin/python3
 """
-@Author  :   uint8_t
+@Author  :   Ginkgoty
 @Time    :   2022/08/12
-@Version :   0.1.0
+@Version :   0.2.0
 """
 import json
 import random
 import os
 import platform
+from pathlib2 import Path
+import re
 
 
 # class Generator:
 
 # def __init__(self):
 #     self.__address_list = self.__jsonreader()
 #
 #     self.__level4_list = self.__txtreader()
 #
 #     self.__level4_temp = []
 
 # read json file to get level3 address
 def jsonreader():
-    if platform.system() == 'Windows':
-        path = os.path.dirname(os.__file__) + '\\site-packages\\chinese_address_generator\\src\\level3.json'
-    else:
-        path = os.path.dirname(os.__file__) + '/site-packages/chinese_address_generator/src/level3.json'
+    path = Path(__file__).parent.joinpath("src").joinpath("new_level3.json")
+    # if platform.system() == 'Windows':
+    #     path = os.path.dirname(os.__file__) + '\\site-packages\\chinese_address_generator\\src\\level3.json'
+    # else:
+    #     path = os.path.dirname(os.__file__) + '/site-packages/chinese_address_generator/src/level3.json'
     return json.loads(open(path, 'r', encoding='utf-8').read())
 
 
 # read txt file to get level4 address
 def txtreader():
-    if platform.system() == 'Windows':
-        path = os.path.dirname(os.__file__) + '\\site-packages\\chinese_address_generator\\src\\level4.txt'
-    else:
-        path = os.path.dirname(os.__file__) + '/site-packages/chinese_address_generator/src/level4.txt'
+    path = Path(__file__).parent.joinpath("src").joinpath("new_level4.txt")
+    # if platform.system() == 'Windows':
+    #     path = os.path.dirname(os.__file__) + '\\site-packages\\chinese_address_generator\\src\\level4.txt'
+    # else:
+    #     path = os.path.dirname(os.__file__) + '/site-packages/chinese_address_generator/src/level4.txt'
     return open(path, 'r', encoding='utf-8').readlines()
 
 
 __address_list = jsonreader()
 
 __level4_list = txtreader()
 
-__level4_temp = []
-
-
 # generate level1 address, province
 def generatelevel1():
     try:
-        province = random.choice(__address_list[:-3])
+        province = random.choice(__address_list)
         return province['region'] + " " + province['code']
     except:
         pass
 
 
 # generate level2 address, province + city
 def generatelevel2():
     try:
-        province = random.choice(__address_list[:-3])
+        province = random.choice(__address_list)
         city = random.choice(province['regionEntitys'])
         return province['region'] + city['region'] + " " + city['code']
     except:
         pass
 
 
 # generate level3 address, province + city + county
 def generatelevel3():
     try:
-        province = random.choice(__address_list[:-3])
+        province = random.choice(__address_list)
         city = random.choice(province['regionEntitys'])
         county = random.choice(city['regionEntitys'][1:])
         return province['region'] + city['region'] + county['region'] + " " + county['code']
     except:
         pass
 
 
 # generate level4 address, province + city + county + town
 def generatelevel4():
     try:
-        province = random.choice(__address_list[:-3])
+        province = random.choice(__address_list)
         city = random.choice(province['regionEntitys'])
-        county = random.choice(city['regionEntitys'][1:])
-        for item in __level4_list:
-            if item[0:6] == county['code']:
-                __level4_temp.append(item[13:])
-        town = random.choice(__level4_temp)
+        county = random.choice(city['regionEntitys'])
+        pattern = re.compile(f"^{county['code']}")
+        matches = [item[13:-1] for item in __level4_list if pattern.match(item)]
+        town = random.choice(matches)
         return province['region'] + city['region'] + county['region'] + town + " " + county['code']
     except:
         pass
```

