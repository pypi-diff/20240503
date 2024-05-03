# Comparing `tmp/pbix_refresh-0.4.30.tar.gz` & `tmp/pbix_refresh-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbix_refresh-0.4.30.tar", last modified: Sun Apr 28 13:32:02 2024, max compression
+gzip compressed data, was "pbix_refresh-0.5.3.tar", last modified: Fri May  3 03:35:55 2024, max compression
```

## Comparing `pbix_refresh-0.4.30.tar` & `pbix_refresh-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:32:02.073362 pbix_refresh-0.4.30/
--rw-rw-rw-   0        0        0      126 2024-04-28 13:32:02.073362 pbix_refresh-0.4.30/PKG-INFO
--rw-rw-rw-   0        0        0       34 2024-04-28 06:42:39.000000 pbix_refresh-0.4.30/README.txt
--rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 pbix_refresh-0.4.30/license.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 13:32:02.067377 pbix_refresh-0.4.30/pbix_refresh/
--rw-rw-rw-   0        0        0       29 2024-04-28 13:17:31.000000 pbix_refresh-0.4.30/pbix_refresh/__init__.py
--rw-rw-rw-   0        0        0     2386 2024-04-28 13:30:16.000000 pbix_refresh-0.4.30/pbix_refresh/pbix_refresh.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:32:02.072365 pbix_refresh-0.4.30/pbix_refresh.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-28 13:32:01.000000 pbix_refresh-0.4.30/pbix_refresh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-04-28 13:32:02.000000 pbix_refresh-0.4.30/pbix_refresh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:32:01.000000 pbix_refresh-0.4.30/pbix_refresh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-28 13:32:01.000000 pbix_refresh-0.4.30/pbix_refresh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 13:32:02.073362 pbix_refresh-0.4.30/setup.cfg
--rw-rw-rw-   0        0        0      250 2024-04-28 13:31:32.000000 pbix_refresh-0.4.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:35:55.592828 pbix_refresh-0.5.3/
+-rw-rw-rw-   0        0        0      157 2024-05-03 03:35:55.592828 pbix_refresh-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2024-04-28 06:42:39.000000 pbix_refresh-0.5.3/README.txt
+-rw-rw-rw-   0        0        0       52 2024-04-06 07:14:29.000000 pbix_refresh-0.5.3/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 03:35:55.580861 pbix_refresh-0.5.3/pbix_refresh/
+-rw-rw-rw-   0        0        0       29 2024-04-28 13:17:31.000000 pbix_refresh-0.5.3/pbix_refresh/__init__.py
+-rw-rw-rw-   0        0        0     2394 2024-05-03 03:30:42.000000 pbix_refresh-0.5.3/pbix_refresh/pbix_refresh.py
+drwxrwxrwx   0        0        0        0 2024-05-03 03:35:55.590833 pbix_refresh-0.5.3/pbix_refresh.egg-info/
+-rw-rw-rw-   0        0        0      157 2024-05-03 03:35:55.000000 pbix_refresh-0.5.3/pbix_refresh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-03 03:35:55.000000 pbix_refresh-0.5.3/pbix_refresh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 03:35:55.000000 pbix_refresh-0.5.3/pbix_refresh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 03:35:55.000000 pbix_refresh-0.5.3/pbix_refresh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 03:35:55.593841 pbix_refresh-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      281 2024-05-03 03:34:17.000000 pbix_refresh-0.5.3/setup.py
```

### Comparing `pbix_refresh-0.4.30/pbix_refresh/pbix_refresh.py` & `pbix_refresh-0.5.3/pbix_refresh/pbix_refresh.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     # 通过 connect 方法连接进程
     app = Application(backend='uia').connect(path=procname)
     # title_re可以通过正则表达式连接：".*Power BI Desktop", 仅限 2023年9月之前的 Power bi版本
     # 2023年10月之后的版本没有此窗口后缀, 因此需用文件名找窗口
     # 如果同时打开了其他同名的文件（非 power bi文件时）, 可能会引发错误
     _filename = os.path.splitext(os.path.basename(_path))[0]  # 文件名不含后缀
-    win = app.window(title_re=_filename)  # 连接 pbi 窗口
+    win = app.window(title_re=f'{_filename}.*?')  # 连接 pbi 窗口
     time.sleep(10)
     # win.print_control_identifiers()  # 打印窗口全部信息, 推荐使用 inspect 开发工具查询窗口句柄信息
     num = 0
     while True:
         try:
             win['刷新'].wait("enabled", timeout=_timeout)
             time.sleep(3)
```

