# Comparing `tmp/fuo_netease-1.0.1.tar.gz` & `tmp/fuo_netease-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_netease-1.0.1.tar", last modified: Mon Mar  4 13:22:37 2024, max compression
+gzip compressed data, was "fuo_netease-1.0.2.tar", last modified: Fri May  3 13:29:33 2024, max compression
```

## Comparing `fuo_netease-1.0.1.tar` & `fuo_netease-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/fuo_netease/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24427 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/fuo_netease/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/assets/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/fuo_netease/cloud_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/cloud_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/cloud_helpers/cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/cloud_helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/login_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/page_fav.py
--rw-r--r--   0 runner    (1001) docker     (127)    19151 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/fuo_netease/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/fuo_netease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-04 13:22:37.000000 fuo_netease-1.0.1/fuo_netease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-04 13:22:37.000000 fuo_netease-1.0.1/fuo_netease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:22:37.000000 fuo_netease-1.0.1/fuo_netease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-04 13:22:37.000000 fuo_netease-1.0.1/fuo_netease.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-04 13:22:37.000000 fuo_netease-1.0.1/fuo_netease.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-04 13:22:37.000000 fuo_netease-1.0.1/fuo_netease.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-04 13:22:37.774239 fuo_netease-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-04 13:22:36.000000 fuo_netease-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24566 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease/cloud_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/cloud_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/cloud_helpers/cloud_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/cloud_helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/login_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/page_fav.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19219 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/fuo_netease/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/fuo_netease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 13:29:33.000000 fuo_netease-1.0.2/fuo_netease.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 13:29:33.888115 fuo_netease-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-03 13:29:31.000000 fuo_netease-1.0.2/setup.py
```

### Comparing `fuo_netease-1.0.1/PKG-INFO` & `fuo_netease-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo_netease
-Version: 1.0.1
+Version: 1.0.2
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-1.0.1/README.md` & `fuo_netease-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 ## 安装
 
 ```sh
 pip3 install fuo-netease
 ```
 
 ## changelog
+### 1.0.2 (2024-05-03)
+- 修复歌手歌曲列表
+
 ### 1.0.1 (2024-03-04)
 - 支持识别 vip 歌曲
 - 修复纯音乐歌曲的歌词
 
 ### 1.0 (2024-01-11)
 - 支持推荐接口
 - 使用 FeelUOwn 提供的发现页，推荐页（而不是自己实现）
```

### Comparing `fuo_netease-1.0.1/fuo_netease/__init__.py` & `fuo_netease-1.0.2/fuo_netease/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/api.py` & `fuo_netease-1.0.2/fuo_netease/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,16 +246,21 @@
         }
         """
         action = uri + '/artist/' + str(artist_id)
         data = self.request('GET', action)
         return data
 
     def artist_songs(self, artist_id, offset=0, limit=50):
-        action = uri_we + '/artist/songs'
-        data = dict(id=artist_id, limit=limit, offset=offset, n=limit)
+        action = uri_v1 + '/artist/songs'
+        data = dict(id=artist_id,
+                    limit=limit,
+                    offset=offset,
+                    order='hot',
+                    work_type=1,
+                    private_cloud='true')
         payload = self.encrypt_request(data)
         res_data = self.request('POST', action, payload)
         if res_data['code'] == 200:
             return res_data
         raise CodeShouldBe200(res_data)
 
     def artist_albums(self, artist_id, offset=0, limit=20):
```

### Comparing `fuo_netease-1.0.1/fuo_netease/assets/icon.svg` & `fuo_netease-1.0.2/fuo_netease/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/cloud_helpers/__init__.py` & `fuo_netease-1.0.2/fuo_netease/cloud_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/cloud_helpers/cloud_api.py` & `fuo_netease-1.0.2/fuo_netease/cloud_helpers/cloud_api.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/cloud_helpers/security.py` & `fuo_netease-1.0.2/fuo_netease/cloud_helpers/security.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/downloader.py` & `fuo_netease-1.0.2/fuo_netease/downloader.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/login_controller.py` & `fuo_netease-1.0.2/fuo_netease/login_controller.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/models.py` & `fuo_netease-1.0.2/fuo_netease/models.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/page_fav.py` & `fuo_netease-1.0.2/fuo_netease/page_fav.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/provider.py` & `fuo_netease-1.0.2/fuo_netease/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,17 @@
         if songs_data is None:
             logger.error('data should not be None')
             return None
         return [_deserialize(song_data, V2SongSchema)
                 for song_data in songs_data]
 
     def rec_list_daily_playlists(self):
+        if not self.has_current_user():
+            return []
+
         playlists_data = self.api.get_recommend_playlists()
         rec_playlists = []
         for playlist_data in playlists_data:
             # FIXME: GUI模式下无法显示歌单描述
             playlist_data['coverImgUrl'] = playlist_data['picUrl']
             playlist_data['description'] = None
             playlist = _deserialize(playlist_data, V2PlaylistSchema)
@@ -323,15 +326,15 @@
 
         def g():
             offset = 0
             per = 50
             while offset < count:
                 data = self.api.artist_songs(artist.identifier, offset, per)
                 for song_data in data['songs']:
-                    yield _deserialize(song_data, V2SongSchema)
+                    yield _deserialize(song_data, V2SongSchemaForV3)
                     # In reality, len(data['songs']) may smaller than per,
                     # which is a bug of netease server side, so we set
                     # offset to `offset + per` here.
                 offset += per
                 per = 100
 
         return SequentialReader(g(), count)
```

### Comparing `fuo_netease-1.0.1/fuo_netease/provider_ui.py` & `fuo_netease-1.0.2/fuo_netease/provider_ui.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/schemas.py` & `fuo_netease-1.0.2/fuo_netease/schemas.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease/ui.py` & `fuo_netease-1.0.2/fuo_netease/ui.py`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/fuo_netease.egg-info/PKG-INFO` & `fuo_netease-1.0.2/fuo_netease.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo-netease
-Version: 1.0.1
+Version: 1.0.2
 Summary: feeluown netease plugin
 Home-page: https://github.com/feeluown/feeluown-netease
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: feeluown,plugin,netease
```

### Comparing `fuo_netease-1.0.1/fuo_netease.egg-info/SOURCES.txt` & `fuo_netease-1.0.2/fuo_netease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo_netease-1.0.1/setup.py` & `fuo_netease-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='fuo_netease',
-    version='1.0.1',
+    version='1.0.2',
     description='feeluown netease plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=find_packages(exclude=('tests*',)),
     package_data={
         '': ['assets/*.svg',
              ]
```

