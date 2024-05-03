# Comparing `tmp/CachedFileDic-0.2.5.tar.gz` & `tmp/CachedFileDic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CachedFileDic-0.2.5.tar", last modified: Sun Apr 28 05:02:06 2024, max compression
+gzip compressed data, was "CachedFileDic-0.3.0.tar", last modified: Fri May  3 05:04:50 2024, max compression
```

## Comparing `CachedFileDic-0.2.5.tar` & `CachedFileDic-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 05:02:06.707538 CachedFileDic-0.2.5/
-drwxrwxrwx   0        0        0        0 2024-04-28 05:02:06.692075 CachedFileDic-0.2.5/CachedFileDic/
--rw-rw-rw-   0        0        0     7378 2024-04-28 05:01:40.000000 CachedFileDic-0.2.5/CachedFileDic/__init__.py
--rw-rw-rw-   0        0        0     6595 2024-04-28 04:45:05.000000 CachedFileDic-0.2.5/CachedFileDic/__init__BACKUP_commit効率化変更前.py
--rw-rw-rw-   0        0        0     6952 2024-04-25 01:06:02.000000 CachedFileDic-0.2.5/CachedFileDic/__init__BACKUP_lazy_commitバグあり版.py
--rw-rw-rw-   0        0        0      833 2024-03-11 04:00:17.000000 CachedFileDic-0.2.5/CachedFileDic/test.py
-drwxrwxrwx   0        0        0        0 2024-04-28 05:02:06.706545 CachedFileDic-0.2.5/CachedFileDic.egg-info/
--rw-rw-rw-   0        0        0     7310 2024-04-28 05:02:06.000000 CachedFileDic-0.2.5/CachedFileDic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-04-28 05:02:06.000000 CachedFileDic-0.2.5/CachedFileDic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 05:02:06.000000 CachedFileDic-0.2.5/CachedFileDic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-28 05:02:06.000000 CachedFileDic-0.2.5/CachedFileDic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-28 05:02:06.000000 CachedFileDic-0.2.5/CachedFileDic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7310 2024-04-28 05:02:06.706545 CachedFileDic-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6931 2023-12-23 00:25:59.000000 CachedFileDic-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 05:02:06.707538 CachedFileDic-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-28 05:01:54.000000 CachedFileDic-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:04:50.847451 CachedFileDic-0.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-03 05:04:50.832700 CachedFileDic-0.3.0/CachedFileDic/
+-rw-rw-rw-   0        0        0     7531 2024-05-03 05:01:44.000000 CachedFileDic-0.3.0/CachedFileDic/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-05-03 05:04:00.000000 CachedFileDic-0.3.0/CachedFileDic/test.py
+drwxrwxrwx   0        0        0        0 2024-05-03 05:04:50.846391 CachedFileDic-0.3.0/CachedFileDic.egg-info/
+-rw-rw-rw-   0        0        0     7310 2024-05-03 05:04:50.000000 CachedFileDic-0.3.0/CachedFileDic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-03 05:04:50.000000 CachedFileDic-0.3.0/CachedFileDic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 05:04:50.000000 CachedFileDic-0.3.0/CachedFileDic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-03 05:04:50.000000 CachedFileDic-0.3.0/CachedFileDic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-03 05:04:50.000000 CachedFileDic-0.3.0/CachedFileDic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7310 2024-05-03 05:04:50.846391 CachedFileDic-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6931 2023-12-23 00:25:59.000000 CachedFileDic-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-03 05:04:50.847451 CachedFileDic-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-05-03 05:04:31.000000 CachedFileDic-0.3.0/setup.py
```

### Comparing `CachedFileDic-0.2.5/CachedFileDic/__init__.py` & `CachedFileDic-0.3.0/CachedFileDic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 		return self.loaded_cont_dic[cont_name]
 	# spill処理 (データが規定容量を超えたら、latest_contとして新しいコンテナを設定)
 	def spill(self):
 		# 溢れていない場合は何もしない
 		if self.index["latest_cont_size"] <= self.cont_size_th: return None
 		# 新しいコンテナを作成
 		def exists(new_id): return os.path.exists(os.path.join(self.dir_name, f"cont_{new_id}.{self.fmt}"))
-		new_cont_name = "cont_" + slim_id.gen(exists, length = 1)
+		new_cont_name = "cont_" + slim_id.gen(exists, length = 1, ab = "16")	# 注意: 大文字・小文字を区別できないOSがあるため、安全のため小文字のみのアルファベットとしている
 		self.index["latest_cont"] = new_cont_name	# 書き込み対象コンテナの更新
 		self.index["latest_cont_size"] = 0	# 新コンテナの容量
 		fies[self.dir_name][f"{new_cont_name}.{self.fmt}"] = {}
 	# 最優先idxの取得
 	def _max_priority(self):
 		if len(self.priority_idx_dic) == 0: return 0
 		return max([self.priority_idx_dic[k] for k in self.priority_idx_dic])
```

### Comparing `CachedFileDic-0.2.5/CachedFileDic/test.py` & `CachedFileDic-0.3.0/CachedFileDic/test.py`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.5/CachedFileDic.egg-info/PKG-INFO` & `CachedFileDic-0.3.0/CachedFileDic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CachedFileDic
-Version: 0.2.5
+Version: 0.3.0
 Summary: Fast Dictionary-Type Database
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `CachedFileDic-0.2.5/PKG-INFO` & `CachedFileDic-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CachedFileDic
-Version: 0.2.5
+Version: 0.3.0
 Summary: Fast Dictionary-Type Database
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `CachedFileDic-0.2.5/README.md` & `CachedFileDic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.5/setup.py` & `CachedFileDic-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 4361 6368 6564 4669  develop_CachedFi
 000000c0: 6c65 4469 632f 2229 2061 7320 703a 0d0a  leDic/") as p:..
 000000d0: 0973 6574 7570 280d 0a09 096e 616d 6520  .setup(....name 
 000000e0: 3d20 2243 6163 6865 6446 696c 6544 6963  = "CachedFileDic
 000000f0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-00000100: 2230 2e32 2e35 222c 0d0a 0909 6465 7363  "0.2.5",....desc
+00000100: 2230 2e33 2e30 222c 0d0a 0909 6465 7363  "0.3.0",....desc
 00000110: 7269 7074 696f 6e20 3d20 2246 6173 7420  ription = "Fast 
 00000120: 4469 6374 696f 6e61 7279 2d54 7970 6520  Dictionary-Type 
 00000130: 4461 7461 6261 7365 222c 0d0a 0909 6175  Database",....au
 00000140: 7468 6f72 203d 2022 6269 625f 696e 6622  thor = "bib_inf"
 00000150: 2c0d 0a09 0961 7574 686f 725f 656d 6169  ,....author_emai
 00000160: 6c20 3d20 2263 6f6e 7461 6374 2e62 6962  l = "contact.bib
 00000170: 696e 6640 676d 6169 6c2e 636f 6d22 2c0d  inf@gmail.com",.
```

