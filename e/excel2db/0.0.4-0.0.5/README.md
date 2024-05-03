# Comparing `tmp/excel2db-0.0.4.tar.gz` & `tmp/excel2db-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\excel2db-0.0.4.tar", last modified: Tue Apr 30 07:58:23 2024, max compression
+gzip compressed data, was "dist\excel2db-0.0.5.tar", last modified: Fri May  3 08:35:54 2024, max compression
```

## Comparing `excel2db-0.0.4.tar` & `excel2db-0.0.5.tar`

### file list

```diff
@@ -1,58 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/
--rw-rw-rw-   0        0        0      171 2024-04-30 07:58:23.000000 excel2db-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/
--rw-rw-rw-   0        0        0        0 2024-04-24 13:59:30.000000 excel2db-0.0.4/excel2db/__init__.py
--rw-rw-rw-   0        0        0    19638 2024-04-30 04:24:41.000000 excel2db-0.0.4/excel2db/cheakConf.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/com/
--rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.4/excel2db/com/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/com/util/
--rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.4/excel2db/com/util/__init__.py
--rw-rw-rw-   0        0        0     8036 2023-06-28 01:48:10.000000 excel2db-0.0.4/excel2db/com/util/coordinate.py
--rw-rw-rw-   0        0        0     1633 2024-04-30 03:24:30.000000 excel2db-0.0.4/excel2db/com/util/dbconnect.py
--rw-rw-rw-   0        0        0     3933 2024-03-01 03:05:42.000000 excel2db-0.0.4/excel2db/com/util/excelTool.py
--rw-rw-rw-   0        0        0     6194 2023-10-17 13:38:33.000000 excel2db-0.0.4/excel2db/com/util/fileTool.py
--rw-rw-rw-   0        0        0     8838 2024-04-30 03:24:30.000000 excel2db-0.0.4/excel2db/com/util/timeTool.py
--rw-rw-rw-   0        0        0     5520 2024-04-30 06:48:39.000000 excel2db-0.0.4/excel2db/defaultConf.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/
--rw-rw-rw-   0        0        0        0 2024-04-25 03:02:41.000000 excel2db-0.0.4/excel2db/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo1/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo1/__init__.py
--rw-rw-rw-   0        0        0      173 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo1/demo1.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo2/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo2/__init__.py
--rw-rw-rw-   0        0        0      190 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo2/demo2.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo3/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo3/__init__.py
--rw-rw-rw-   0        0        0      190 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo3/demo3.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo4/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo4/__init__.py
--rw-rw-rw-   0        0        0      175 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo4/demo4.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo5/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo5/__init__.py
--rw-rw-rw-   0        0        0      192 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo5/demo5.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo6/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo6/__init__.py
--rw-rw-rw-   0        0        0      199 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo6/demo6.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db/demo/demo7/
--rw-rw-rw-   0        0        0        0 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo7/__init__.py
--rw-rw-rw-   0        0        0      199 2024-04-30 07:56:24.000000 excel2db-0.0.4/excel2db/demo/demo7/demo7.py
--rw-rw-rw-   0        0        0     7302 2024-04-30 07:56:17.000000 excel2db-0.0.4/excel2db/demo/generalDemoFile.py
--rw-rw-rw-   0        0        0     2646 2024-04-30 04:24:41.000000 excel2db-0.0.4/excel2db/detailData.py
--rw-rw-rw-   0        0        0     2653 2024-04-30 04:24:41.000000 excel2db-0.0.4/excel2db/detailTitle.py
--rw-rw-rw-   0        0        0     2527 2024-04-30 03:24:30.000000 excel2db-0.0.4/excel2db/excel.py
--rw-rw-rw-   0        0        0      712 2024-04-30 03:24:30.000000 excel2db-0.0.4/excel2db/excel2db.py
--rw-rw-rw-   0        0        0     2050 2024-04-30 03:24:30.000000 excel2db-0.0.4/excel2db/extraFuction.py
--rw-rw-rw-   0        0        0     5816 2024-04-30 07:41:06.000000 excel2db-0.0.4/excel2db/insert2sqlite.py
--rw-rw-rw-   0        0        0     3057 2024-04-30 03:27:24.000000 excel2db-0.0.4/excel2db/mainData.py
--rw-rw-rw-   0        0        0     5144 2024-04-30 07:41:06.000000 excel2db-0.0.4/excel2db/mainTitle.py
--rw-rw-rw-   0        0        0     6943 2024-04-30 03:27:24.000000 excel2db-0.0.4/excel2db/scale.py
--rw-rw-rw-   0        0        0     5228 2024-04-30 04:24:41.000000 excel2db-0.0.4/excel2db/sheet.py
--rw-rw-rw-   0        0        0     7190 2024-04-30 04:24:41.000000 excel2db-0.0.4/excel2db/value.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db.egg-info/
--rw-rw-rw-   0        0        0      171 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 07:58:23.000000 excel2db-0.0.4/excel2db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 07:58:23.000000 excel2db-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      493 2024-04-30 07:58:21.000000 excel2db-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:35:54.000000 excel2db-0.0.5/
+-rw-rw-rw-   0        0        0      171 2024-05-03 08:35:54.000000 excel2db-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db/
+-rw-rw-rw-   0        0        0        0 2024-04-24 13:59:30.000000 excel2db-0.0.5/excel2db/__init__.py
+-rw-rw-rw-   0        0        0    19638 2024-04-30 04:24:41.000000 excel2db-0.0.5/excel2db/cheakConf.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db/com/
+-rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.5/excel2db/com/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db/com/util/
+-rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.5/excel2db/com/util/__init__.py
+-rw-rw-rw-   0        0        0     8036 2023-06-28 01:48:10.000000 excel2db-0.0.5/excel2db/com/util/coordinate.py
+-rw-rw-rw-   0        0        0     3847 2024-05-03 08:31:30.000000 excel2db-0.0.5/excel2db/com/util/dbconnect.py
+-rw-rw-rw-   0        0        0     3933 2024-03-01 03:05:42.000000 excel2db-0.0.5/excel2db/com/util/excelTool.py
+-rw-rw-rw-   0        0        0     6194 2023-10-17 13:38:33.000000 excel2db-0.0.5/excel2db/com/util/fileTool.py
+-rw-rw-rw-   0        0        0     8838 2024-04-30 03:24:30.000000 excel2db-0.0.5/excel2db/com/util/timeTool.py
+-rw-rw-rw-   0        0        0     5520 2024-04-30 06:48:39.000000 excel2db-0.0.5/excel2db/defaultConf.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db/demo/
+-rw-rw-rw-   0        0        0        0 2024-05-03 08:34:25.000000 excel2db-0.0.5/excel2db/demo/__init__.py
+-rw-rw-rw-   0        0        0     7637 2024-05-03 08:34:25.000000 excel2db-0.0.5/excel2db/demo/generalDemoFile.py
+-rw-rw-rw-   0        0        0     2646 2024-04-30 04:24:41.000000 excel2db-0.0.5/excel2db/detailData.py
+-rw-rw-rw-   0        0        0     2653 2024-04-30 04:24:41.000000 excel2db-0.0.5/excel2db/detailTitle.py
+-rw-rw-rw-   0        0        0     2527 2024-04-30 03:24:30.000000 excel2db-0.0.5/excel2db/excel.py
+-rw-rw-rw-   0        0        0      712 2024-04-30 03:24:30.000000 excel2db-0.0.5/excel2db/excel2db.py
+-rw-rw-rw-   0        0        0     2050 2024-04-30 03:24:30.000000 excel2db-0.0.5/excel2db/extraFuction.py
+-rw-rw-rw-   0        0        0     5816 2024-05-03 07:45:33.000000 excel2db-0.0.5/excel2db/insert2sqlite.py
+-rw-rw-rw-   0        0        0     3057 2024-04-30 03:27:24.000000 excel2db-0.0.5/excel2db/mainData.py
+-rw-rw-rw-   0        0        0     5144 2024-04-30 07:41:06.000000 excel2db-0.0.5/excel2db/mainTitle.py
+-rw-rw-rw-   0        0        0     6943 2024-04-30 03:27:24.000000 excel2db-0.0.5/excel2db/scale.py
+-rw-rw-rw-   0        0        0     5228 2024-04-30 04:24:41.000000 excel2db-0.0.5/excel2db/sheet.py
+-rw-rw-rw-   0        0        0     7182 2024-05-03 07:45:33.000000 excel2db-0.0.5/excel2db/value.py
+drwxrwxrwx   0        0        0        0 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db.egg-info/
+-rw-rw-rw-   0        0        0      171 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 08:35:54.000000 excel2db-0.0.5/excel2db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 08:35:54.000000 excel2db-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      493 2024-04-30 08:12:26.000000 excel2db-0.0.5/setup.py
```

### Comparing `excel2db-0.0.4/excel2db/cheakConf.py` & `excel2db-0.0.5/excel2db/cheakConf.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/com/util/coordinate.py` & `excel2db-0.0.5/excel2db/com/util/coordinate.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/com/util/excelTool.py` & `excel2db-0.0.5/excel2db/com/util/excelTool.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/com/util/fileTool.py` & `excel2db-0.0.5/excel2db/com/util/fileTool.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/com/util/timeTool.py` & `excel2db-0.0.5/excel2db/com/util/timeTool.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/defaultConf.py` & `excel2db-0.0.5/excel2db/defaultConf.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/detailData.py` & `excel2db-0.0.5/excel2db/detailData.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/detailTitle.py` & `excel2db-0.0.5/excel2db/detailTitle.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/excel.py` & `excel2db-0.0.5/excel2db/excel.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/excel2db.py` & `excel2db-0.0.5/excel2db/excel2db.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/extraFuction.py` & `excel2db-0.0.5/excel2db/extraFuction.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/insert2sqlite.py` & `excel2db-0.0.5/excel2db/insert2sqlite.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/mainData.py` & `excel2db-0.0.5/excel2db/mainData.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/mainTitle.py` & `excel2db-0.0.5/excel2db/mainTitle.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/scale.py` & `excel2db-0.0.5/excel2db/scale.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/sheet.py` & `excel2db-0.0.5/excel2db/sheet.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.4/excel2db/value.py` & `excel2db-0.0.5/excel2db/value.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         self.dbConnect = None ##数据库连接
         self.datLoad = ""  ##生成的数据库文件路径
         self.datLoad = "./test.db"
         self.tableName = "" ##当前主表名
         self.tableDtlName = ""##明细表名
         self.columnsType = {} ##主表字段名及类型
         self.columnsDtlType = []##明细表字段名
-        self.mainDBData = None ##主表数据
+        self.mainDBData = [] ##主表数据
         self.detailDBTitleData = {} ##明细表标题行数据
-        self.detailDBData = None ##明细表数据
+        self.detailDBData = [] ##明细表数据
 
         ##配置文件相关
         self.rawConf = {}  ##合并后的原始配置文件
         self.excelConf = {}  ##当前的excel级别配置文件
         self.excelConfDown = {}  ##当前的excel级别向下配置文件
         self.sheetConf = {}  ##当前的sheet级别配置文件
         self.sheetConfDown = {}  ##当前的sheet级别向下配置文件
@@ -123,17 +123,17 @@
         self.cycleColumns = 0  ##明细表一个循环的列数
 
         ##数据库相关
         self.tableName = ""  ##当前主表名
         self.tableDtlName = ""  ##明细表名
         self.columnsType = {}  ##主表字段名及类型
         self.columnsDtlType = []  ##明细表字段名
-        self.mainDBData = None  ##主表数据
+        self.mainDBData = []  ##主表数据
         self.detailDBTitleData = {}  ##明细表标题行数据
-        self.detailDBData = None  ##明细表数据
+        self.detailDBData = []  ##明细表数据
 
         ##配置文件相关
         self.mainTitleConf = {}  ##当前的sheet级别配置文件
         self.mainTitleConfDown = {}  ##当前的sheet级别向下配置文件
         self.mainDataConf = {}  ##当前的sheet级别配置文件
         self.mainDataConfDown = {}  ##当前的sheet级别向下配置文件
         self.detailTitleConf = {}  ##当前的sheet级别配置文件
```

### Comparing `excel2db-0.0.4/excel2db.egg-info/SOURCES.txt` & `excel2db-0.0.5/excel2db.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -22,22 +22,8 @@
 excel2db/com/util/__init__.py
 excel2db/com/util/coordinate.py
 excel2db/com/util/dbconnect.py
 excel2db/com/util/excelTool.py
 excel2db/com/util/fileTool.py
 excel2db/com/util/timeTool.py
 excel2db/demo/__init__.py
-excel2db/demo/generalDemoFile.py
-excel2db/demo/demo1/__init__.py
-excel2db/demo/demo1/demo1.py
-excel2db/demo/demo2/__init__.py
-excel2db/demo/demo2/demo2.py
-excel2db/demo/demo3/__init__.py
-excel2db/demo/demo3/demo3.py
-excel2db/demo/demo4/__init__.py
-excel2db/demo/demo4/demo4.py
-excel2db/demo/demo5/__init__.py
-excel2db/demo/demo5/demo5.py
-excel2db/demo/demo6/__init__.py
-excel2db/demo/demo6/demo6.py
-excel2db/demo/demo7/__init__.py
-excel2db/demo/demo7/demo7.py
+excel2db/demo/generalDemoFile.py
```

