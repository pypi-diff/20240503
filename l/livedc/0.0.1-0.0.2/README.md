# Comparing `tmp/livedc-0.0.1.tar.gz` & `tmp/livedc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livedc-0.0.1.tar", last modified: Fri May  3 14:51:19 2024, max compression
+gzip compressed data, was "livedc-0.0.2.tar", last modified: Fri May  3 15:21:55 2024, max compression
```

## Comparing `livedc-0.0.1.tar` & `livedc-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 14:51:19.892731 livedc-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-03 13:31:15.000000 livedc-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2089 2024-05-03 14:51:19.889987 livedc-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       83 2024-05-03 13:31:15.000000 livedc-0.0.1/README.md
--rw-rw-rw-   0        0        0      854 2024-05-03 14:51:19.000000 livedc-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 14:51:19.893746 livedc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1079 2024-05-03 13:54:21.000000 livedc-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:51:19.854310 livedc-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 14:51:19.865203 livedc-0.0.1/src/livedc/
--rw-rw-rw-   0        0        0       21 2024-05-03 13:53:23.000000 livedc-0.0.1/src/livedc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:51:19.854310 livedc-0.0.1/src/livedc/math/
-drwxrwxrwx   0        0        0        0 2024-05-03 14:51:19.880785 livedc-0.0.1/src/livedc/math/financial/
--rw-rw-rw-   0        0        0     2364 2024-05-03 14:10:50.000000 livedc-0.0.1/src/livedc/math/financial/compound.py
-drwxrwxrwx   0        0        0        0 2024-05-03 14:51:19.887158 livedc-0.0.1/src/livedc.egg-info/
--rw-rw-rw-   0        0        0     2089 2024-05-03 14:51:19.000000 livedc-0.0.1/src/livedc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-05-03 14:51:19.000000 livedc-0.0.1/src/livedc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 14:51:19.000000 livedc-0.0.1/src/livedc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-03 14:51:19.000000 livedc-0.0.1/src/livedc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2024-05-03 14:51:19.000000 livedc-0.0.1/src/livedc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 14:51:19.000000 livedc-0.0.1/src/livedc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 15:21:55.705134 livedc-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-03 13:31:15.000000 livedc-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2089 2024-05-03 15:21:55.703139 livedc-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2024-05-03 13:31:15.000000 livedc-0.0.2/README.md
+-rw-rw-rw-   0        0        0      854 2024-05-03 15:21:55.000000 livedc-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:21:55.705134 livedc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2024-05-03 13:54:21.000000 livedc-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:21:55.675745 livedc-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 15:21:55.687301 livedc-0.0.2/src/livedc/
+-rw-rw-rw-   0        0        0       51 2024-05-03 15:16:06.000000 livedc-0.0.2/src/livedc/__init__.py
+-rw-rw-rw-   0        0        0     1427 2024-05-03 15:12:25.000000 livedc-0.0.2/src/livedc/desc.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:21:55.677236 livedc-0.0.2/src/livedc/math/
+drwxrwxrwx   0        0        0        0 2024-05-03 15:21:55.699149 livedc-0.0.2/src/livedc/math/financial/
+-rw-rw-rw-   0        0        0     2405 2024-05-03 15:15:05.000000 livedc-0.0.2/src/livedc/math/financial/compound.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:21:55.701143 livedc-0.0.2/src/livedc.egg-info/
+-rw-rw-rw-   0        0        0     2089 2024-05-03 15:21:55.000000 livedc-0.0.2/src/livedc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-03 15:21:55.000000 livedc-0.0.2/src/livedc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:21:55.000000 livedc-0.0.2/src/livedc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-03 15:21:55.000000 livedc-0.0.2/src/livedc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       61 2024-05-03 15:21:55.000000 livedc-0.0.2/src/livedc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 15:21:55.000000 livedc-0.0.2/src/livedc.egg-info/top_level.txt
```

### Comparing `livedc-0.0.1/LICENSE` & `livedc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `livedc-0.0.1/PKG-INFO` & `livedc-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livedc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful mathmatical models/caculators for daily life and cloud deployment
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 jinsanity07git
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `livedc-0.0.1/pyproject.toml` & `livedc-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "livedc"
-version = "0.0.1"
+version = "0.0.2"
 description = "Useful mathmatical models/caculators for daily life and cloud deployment"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3",]
 keywords = [ "cpu", "gpu", "benchmark",]
 dependencies = [ "nodespecs >= 0.0.14",]
 requires-python = ">=3.6"
 [[project.authors]]
```

### Comparing `livedc-0.0.1/setup.py` & `livedc-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `livedc-0.0.1/src/livedc/math/financial/compound.py` & `livedc-0.0.2/src/livedc/math/financial/compound.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 https://www.bilibili.com/video/BV1Ks41157Aj/?spm_id_from=333.337.search-card.all.click
 人生中最重要的概念：复利，是什么？想贷款和分期就必须要了解它
 
 https://qwtel.com/posts/finance/continuously-compounding-interest/
 """
 
 import pandas as pd
+from ...desc import add_rdoc
 ### 自然对是的底 -- e
 
 
 def approx_Euler(n):
   x = (1+1/n)**n
   return x
 
@@ -21,14 +22,15 @@
   x = [ i for i in range(1,10*10000) ]
   df = pd.DataFrame(data={"x":x})
   df["y"] = df.x.apply(approx_Euler)
   print (df.y.iloc[-1])
   df.plot(x="x",y="y",kind="line")
 
 
+@add_rdoc
 def compound_interest(r=0.1, P=100,n=12,t=1):
   """
   Calculate the compound interest.
   - A	=	final amount || 终值
   - P	=	initial principal balance || 现值
   - r	=	interest rate || （年化）利率
   - n	=	number of times interest applied per time period || 期数
```

### Comparing `livedc-0.0.1/src/livedc.egg-info/PKG-INFO` & `livedc-0.0.2/src/livedc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livedc
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful mathmatical models/caculators for daily life and cloud deployment
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 jinsanity07git
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

