# Comparing `tmp/all_in_one_chay-2.4.9.tar.gz` & `tmp/all_in_one_chay-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all_in_one_chay-2.4.9.tar", last modified: Thu Apr 25 14:59:33 2024, max compression
+gzip compressed data, was "all_in_one_chay-3.0.0.tar", last modified: Fri May  3 15:28:12 2024, max compression
```

## Comparing `all_in_one_chay-2.4.9.tar` & `all_in_one_chay-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.745245 all_in_one_chay-2.4.9/
--rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-2.4.9/LICENSE
--rw-rw-rw-   0        0        0     5329 2024-04-25 14:59:33.743243 all_in_one_chay-2.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     4662 2024-04-25 14:55:07.000000 all_in_one_chay-2.4.9/README.md
--rw-rw-rw-   0        0        0      642 2024-04-25 14:58:59.000000 all_in_one_chay-2.4.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 14:59:33.745245 all_in_one_chay-2.4.9/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-25 14:58:49.000000 all_in_one_chay-2.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.720243 all_in_one_chay-2.4.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.726243 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/
--rw-rw-rw-   0        0        0     9838 2024-04-25 14:51:01.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/Allinone.py
--rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.735243 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/
--rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/book.py
--rw-rw-rw-   0        0        0    12741 2024-04-19 15:49:01.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/calculator.py
--rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
--rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/math_cal_py.py
--rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/student_py.py
--rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/tuxing_cal.py
--rw-rw-rw-   0        0        0     4090 2024-04-25 14:55:09.000000 all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/xiaogongju.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:59:33.742243 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/
--rw-rw-rw-   0        0        0     5329 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-25 14:59:33.000000 all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 15:28:12.969083 all_in_one_chay-3.0.0/
+-rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5329 2024-05-03 15:28:12.969083 all_in_one_chay-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4662 2024-04-25 14:55:07.000000 all_in_one_chay-3.0.0/README.md
+-rw-rw-rw-   0        0        0      642 2024-05-03 15:24:16.000000 all_in_one_chay-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:28:12.969083 all_in_one_chay-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-03 15:24:42.000000 all_in_one_chay-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:28:12.849212 all_in_one_chay-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 15:28:12.879084 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/
+-rw-rw-rw-   0        0        0    10078 2024-05-03 15:25:57.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/Allinone.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:28:12.939167 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/
+-rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/book.py
+-rw-rw-rw-   0        0        0    12741 2024-04-19 15:49:01.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/calculator.py
+-rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+-rw-rw-rw-   0        0        0     3908 2024-05-03 15:26:00.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/lotterytickets.py
+-rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/math_cal_py.py
+-rw-rw-rw-   0        0        0     2181 2024-05-03 15:26:00.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/numbertochinese.py
+-rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/student_py.py
+-rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/tuxing_cal.py
+-rw-rw-rw-   0        0        0     4090 2024-04-25 14:55:09.000000 all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/xiaogongju.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:28:12.969083 all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/
+-rw-rw-rw-   0        0        0     5329 2024-05-03 15:28:12.000000 all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-05-03 15:28:12.000000 all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:28:12.000000 all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-03 15:28:12.000000 all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/top_level.txt
```

### Comparing `all_in_one_chay-2.4.9/LICENSE` & `all_in_one_chay-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/PKG-INFO` & `all_in_one_chay-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.9
+Version: 3.0.0
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
+Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v3.0.0
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v3.0.0
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one-Including/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `all_in_one_chay-2.4.9/README.md` & `all_in_one_chay-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/pyproject.toml` & `all_in_one_chay-3.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "All-in-one-chay"
-version = "2.4.9"
+version = "3.0.0"
 authors = [
   { name="chay", email="lichenyi_2020@qq.com" },
 ]
 description = "多功能一体机（All-in-one）"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9"
+Homepage = "https://github.com/lichenyichay/All-in-one-Including/releases/tag/v3.0.0"
 Issues = "https://github.com/lichenyichay/All-in-one-Including/issues"
```

### Comparing `all_in_one_chay-2.4.9/setup.py` & `all_in_one_chay-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding:UTF-8
 import setuptools
 
 setuptools.setup(
     name="All-in-one-chay",
-    version="2.4.8",
+    version="3.0.0",
     author="Chay",
     author_email="lichenyi_2020@qq.com",
-    url="https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9",
+    url="https://github.com/lichenyichay/All-in-one-Including/releases/tag/v3.0.0",
     description="All-in-one",
     long_description="多功能一体机",
     python_requires=">=3.5",
     # packages=setuptools.find_packages("src"),
     packages_dir={"": "src"},
     packages_data={"": ["*.txt", "*.info", "*.properties"], "": ["data/*.*"]},
     exclude=["*.test", "*.test.*", "test.*", "test"],
```

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/Allinone.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/Allinone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding:UTF-8 -*-
 # @Author:Chay
-# @TIME:2024/4/19 23:41
+# @TIME:2024/5/3 23:25
 # @FILE:Allinone.py
 # @version:2.4.8
 # @Software:Visual Studio Code
 import math,random
 import module.book as book
 import module.calculator as calculator
 import module.erfenchazhao_py  as erfenchazhao_py
 import module.math_cal_py as math_cal
 import module.student_py as student_py
 import module.tuxing_cal as tuxing_cal
 import module.xiaogongju as xiaogongju
+import module.lotterytickets as lt
+import module.numbertochinese as ntoc
 def allinone(fuwu,mode,*args):
     """
     :param fuwu 需要服务的功能
     :param mode 部分功能需要的模式（详见Github中All-in-one2.4.0分支的Wiki页）
     :param *args 可变参数，表示需要传入的参数，建议用元组或列表类型，具体所需类型见README.MD
     :return: 0：正常，1：不正常，其他返回值表示功能的结果
 
@@ -79,14 +81,18 @@
         return math_cal.math_cal(mode,args[0],args[1])
     elif fuwu == "分解因式":
         return calculator.factorization(args[0])
     elif fuwu == "提取密码":
         return calculator.mima(args[0],args[1])
     elif fuwu == "凯撒密码计算":
         return xiaogongju.kaisamima(args[0],mode,args[1])
+    elif fuwu == "彩票一体机":
+        return lt.lotterytickets(args[0],args[1],mode)
+    elif fuwu == "数字转中文":
+        return ntoc.No2Cn(args[0])
     elif fuwu == "图形计算器":
         while True:
             huida = args[0]
             try:
                 args2=[]
                 for i in range(1,len(args)):
                     args2.append(args[i])
```

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/book.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/book.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/calculator.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/calculator.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/math_cal_py.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/math_cal_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/student_py.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/student_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/tuxing_cal.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/tuxing_cal.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All-in-one_chayLichenyi/module/xiaogongju.py` & `all_in_one_chay-3.0.0/src/All-in-one_chayLichenyi/module/xiaogongju.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/PKG-INFO` & `all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.9
+Version: 3.0.0
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
+Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v3.0.0
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.9
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v3.0.0
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one-Including/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `all_in_one_chay-2.4.9/src/All_in_one_chay.egg-info/SOURCES.txt` & `all_in_one_chay-3.0.0/src/All_in_one_chay.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 pyproject.toml
 setup.py
 src/All-in-one_chayLichenyi/Allinone.py
 src/All-in-one_chayLichenyi/__init__.py
 src/All-in-one_chayLichenyi/module/book.py
 src/All-in-one_chayLichenyi/module/calculator.py
 src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+src/All-in-one_chayLichenyi/module/lotterytickets.py
 src/All-in-one_chayLichenyi/module/math_cal_py.py
+src/All-in-one_chayLichenyi/module/numbertochinese.py
 src/All-in-one_chayLichenyi/module/student_py.py
 src/All-in-one_chayLichenyi/module/tuxing_cal.py
 src/All-in-one_chayLichenyi/module/xiaogongju.py
 src/All_in_one_chay.egg-info/PKG-INFO
 src/All_in_one_chay.egg-info/SOURCES.txt
 src/All_in_one_chay.egg-info/dependency_links.txt
 src/All_in_one_chay.egg-info/top_level.txt
```

