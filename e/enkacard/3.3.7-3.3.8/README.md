# Comparing `tmp/enkacard-3.3.7.tar.gz` & `tmp/enkacard-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkacard-3.3.7.tar", max compression
+gzip compressed data, was "enkacard-3.3.8.tar", max compression
```

## Comparing `enkacard-3.3.7.tar` & `enkacard-3.3.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      313 2022-12-17 00:40:06.925303 enkacard-3.3.7/enkacard/enc_error.py
--rw-r--r--   0        0        0    10920 2024-04-29 23:52:09.075125 enkacard-3.3.7/enkacard/encbanner.py
--rw-r--r--   0        0        0     4988 2024-04-29 23:50:06.861398 enkacard-3.3.7/enkacard/enkatools.py
--rw-r--r--   0        0        0 11514084 2022-07-25 21:33:51.994087 enkacard-3.3.7/enkacard/src/assets/font/Genshin_Impact.ttf
--rw-r--r--   0        0        0    79268 2023-04-05 20:05:44.281954 enkacard-3.3.7/enkacard/src/assets/font/GSEnochian.ttf
--rw-r--r--   0        0        0     3796 2024-04-25 11:36:07.075682 enkacard-3.3.7/enkacard/src/generator/akasha_rank.py
--rw-r--r--   0        0        0     6657 2023-12-10 18:28:18.819703 enkacard-3.3.7/enkacard/src/generator/one/artifact.py
--rw-r--r--   0        0        0     2363 2023-12-03 21:02:32.344488 enkacard-3.3.7/enkacard/src/generator/one/background.py
--rw-r--r--   0        0        0     1235 2023-12-10 20:39:47.204162 enkacard-3.3.7/enkacard/src/generator/one/constant.py
--rw-r--r--   0        0        0      869 2023-12-01 21:40:04.470207 enkacard-3.3.7/enkacard/src/generator/one/prop.py
--rw-r--r--   0        0        0     1378 2023-12-21 20:00:52.547008 enkacard-3.3.7/enkacard/src/generator/one/skill.py
--rw-r--r--   0        0        0     5749 2023-12-07 00:50:46.885608 enkacard-3.3.7/enkacard/src/generator/one/stat.py
--rw-r--r--   0        0        0     2989 2023-12-23 01:15:33.050226 enkacard-3.3.7/enkacard/src/generator/one/weapon.py
--rw-r--r--   0        0        0     6132 2024-01-06 15:22:38.238244 enkacard-3.3.7/enkacard/src/generator/profile_teample_one.py
--rw-r--r--   0        0        0     5229 2024-04-21 10:32:11.269924 enkacard-3.3.7/enkacard/src/generator/profile_teample_two.py
--rw-r--r--   0        0        0     6711 2024-04-29 23:31:40.343039 enkacard-3.3.7/enkacard/src/generator/teample_one.py
--rw-r--r--   0        0        0     9657 2024-04-29 23:40:21.286778 enkacard-3.3.7/enkacard/src/generator/teample_two.py
--rw-r--r--   0        0        0     6377 2023-12-18 23:30:42.003393 enkacard-3.3.7/enkacard/src/generator/two/artifact.py
--rw-r--r--   0        0        0     3103 2024-04-29 23:46:08.146583 enkacard-3.3.7/enkacard/src/generator/two/background.py
--rw-r--r--   0        0        0     1368 2023-12-21 20:52:29.332377 enkacard-3.3.7/enkacard/src/generator/two/skill.py
--rw-r--r--   0        0        0     3346 2023-12-21 19:58:52.526652 enkacard-3.3.7/enkacard/src/generator/two/stat.py
--rw-r--r--   0        0        0     2553 2024-03-12 11:14:42.124404 enkacard-3.3.7/enkacard/src/modal/enkacardCread.py
--rw-r--r--   0        0        0      771 2023-12-17 22:08:52.342906 enkacard-3.3.7/enkacard/src/modal/enkaToolsModel.py
--rw-r--r--   0        0        0    59616 2023-12-25 12:23:22.739379 enkacard-3.3.7/enkacard/src/pickle_cashe/data_characters.pkz
--rw-r--r--   0        0        0        0 2023-12-25 12:23:29.173879 enkacard-3.3.7/enkacard/src/pickle_cashe/data_characters.pkz~
--rw-r--r--   0        0        0    18462 2023-11-30 22:40:24.144568 enkacard-3.3.7/enkacard/src/utils/affixes.py
--rw-r--r--   0        0        0     5338 2024-04-26 16:53:05.168162 enkacard-3.3.7/enkacard/src/utils/diagram.py
--rw-r--r--   0        0        0     5722 2023-12-25 11:21:01.889033 enkacard-3.3.7/enkacard/src/utils/git.py
--rw-r--r--   0        0        0     7434 2024-04-29 23:35:31.996665 enkacard-3.3.7/enkacard/src/utils/options.py
--rw-r--r--   0        0        0     6868 2023-12-13 21:43:08.363154 enkacard-3.3.7/enkacard/src/utils/pickle_cashe.py
--rw-r--r--   0        0        0    17229 2023-12-23 00:44:36.688489 enkacard-3.3.7/enkacard/src/utils/pill.py
--rw-r--r--   0        0        0     1852 2023-04-05 20:09:26.777243 enkacard-3.3.7/enkacard/src/utils/translation.py
--rw-r--r--   0        0        0      870 2024-04-29 23:51:54.617325 enkacard-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     3699 2023-12-23 16:26:14.431089 enkacard-3.3.7/README.md
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 enkacard-3.3.7/PKG-INFO
+-rw-r--r--   0        0        0      313 2022-12-17 00:40:06.925303 enkacard-3.3.8/enkacard/enc_error.py
+-rw-r--r--   0        0        0    10920 2024-04-29 23:52:09.075125 enkacard-3.3.8/enkacard/encbanner.py
+-rw-r--r--   0        0        0     4988 2024-04-29 23:50:06.861398 enkacard-3.3.8/enkacard/enkatools.py
+-rw-r--r--   0        0        0 11514084 2022-07-25 21:33:51.994087 enkacard-3.3.8/enkacard/src/assets/font/Genshin_Impact.ttf
+-rw-r--r--   0        0        0    79268 2023-04-05 20:05:44.281954 enkacard-3.3.8/enkacard/src/assets/font/GSEnochian.ttf
+-rw-r--r--   0        0        0     3796 2024-04-25 11:36:07.075682 enkacard-3.3.8/enkacard/src/generator/akasha_rank.py
+-rw-r--r--   0        0        0     6657 2023-12-10 18:28:18.819703 enkacard-3.3.8/enkacard/src/generator/one/artifact.py
+-rw-r--r--   0        0        0     2363 2023-12-03 21:02:32.344488 enkacard-3.3.8/enkacard/src/generator/one/background.py
+-rw-r--r--   0        0        0     1235 2023-12-10 20:39:47.204162 enkacard-3.3.8/enkacard/src/generator/one/constant.py
+-rw-r--r--   0        0        0      869 2023-12-01 21:40:04.470207 enkacard-3.3.8/enkacard/src/generator/one/prop.py
+-rw-r--r--   0        0        0     1378 2023-12-21 20:00:52.547008 enkacard-3.3.8/enkacard/src/generator/one/skill.py
+-rw-r--r--   0        0        0     5749 2023-12-07 00:50:46.885608 enkacard-3.3.8/enkacard/src/generator/one/stat.py
+-rw-r--r--   0        0        0     2989 2023-12-23 01:15:33.050226 enkacard-3.3.8/enkacard/src/generator/one/weapon.py
+-rw-r--r--   0        0        0     6132 2024-01-06 15:22:38.238244 enkacard-3.3.8/enkacard/src/generator/profile_teample_one.py
+-rw-r--r--   0        0        0     5229 2024-04-21 10:32:11.269924 enkacard-3.3.8/enkacard/src/generator/profile_teample_two.py
+-rw-r--r--   0        0        0     6711 2024-04-29 23:31:40.343039 enkacard-3.3.8/enkacard/src/generator/teample_one.py
+-rw-r--r--   0        0        0     9723 2024-05-03 15:19:31.133764 enkacard-3.3.8/enkacard/src/generator/teample_two.py
+-rw-r--r--   0        0        0     6377 2023-12-18 23:30:42.003393 enkacard-3.3.8/enkacard/src/generator/two/artifact.py
+-rw-r--r--   0        0        0     3103 2024-04-29 23:46:08.146583 enkacard-3.3.8/enkacard/src/generator/two/background.py
+-rw-r--r--   0        0        0     1368 2023-12-21 20:52:29.332377 enkacard-3.3.8/enkacard/src/generator/two/skill.py
+-rw-r--r--   0        0        0     3346 2023-12-21 19:58:52.526652 enkacard-3.3.8/enkacard/src/generator/two/stat.py
+-rw-r--r--   0        0        0     2553 2024-03-12 11:14:42.124404 enkacard-3.3.8/enkacard/src/modal/enkacardCread.py
+-rw-r--r--   0        0        0      771 2023-12-17 22:08:52.342906 enkacard-3.3.8/enkacard/src/modal/enkaToolsModel.py
+-rw-r--r--   0        0        0    59616 2023-12-25 12:23:22.739379 enkacard-3.3.8/enkacard/src/pickle_cashe/data_characters.pkz
+-rw-r--r--   0        0        0        0 2023-12-25 12:23:29.173879 enkacard-3.3.8/enkacard/src/pickle_cashe/data_characters.pkz~
+-rw-r--r--   0        0        0    18462 2023-11-30 22:40:24.144568 enkacard-3.3.8/enkacard/src/utils/affixes.py
+-rw-r--r--   0        0        0     5356 2024-05-03 15:15:26.208551 enkacard-3.3.8/enkacard/src/utils/diagram.py
+-rw-r--r--   0        0        0     5722 2023-12-25 11:21:01.889033 enkacard-3.3.8/enkacard/src/utils/git.py
+-rw-r--r--   0        0        0     7434 2024-04-29 23:35:31.996665 enkacard-3.3.8/enkacard/src/utils/options.py
+-rw-r--r--   0        0        0     6868 2023-12-13 21:43:08.363154 enkacard-3.3.8/enkacard/src/utils/pickle_cashe.py
+-rw-r--r--   0        0        0    17275 2024-05-03 07:35:34.776114 enkacard-3.3.8/enkacard/src/utils/pill.py
+-rw-r--r--   0        0        0     1852 2023-04-05 20:09:26.777243 enkacard-3.3.8/enkacard/src/utils/translation.py
+-rw-r--r--   0        0        0      870 2024-05-03 15:22:20.319876 enkacard-3.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3699 2023-12-23 16:26:14.431089 enkacard-3.3.8/README.md
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 enkacard-3.3.8/PKG-INFO
```

### Comparing `enkacard-3.3.7/enkacard/encbanner.py` & `enkacard-3.3.8/enkacard/encbanner.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/enkatools.py` & `enkacard-3.3.8/enkacard/enkatools.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/assets/font/Genshin_Impact.ttf` & `enkacard-3.3.8/enkacard/src/assets/font/Genshin_Impact.ttf`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/assets/font/GSEnochian.ttf` & `enkacard-3.3.8/enkacard/src/assets/font/GSEnochian.ttf`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/akasha_rank.py` & `enkacard-3.3.8/enkacard/src/generator/akasha_rank.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/artifact.py` & `enkacard-3.3.8/enkacard/src/generator/one/artifact.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/background.py` & `enkacard-3.3.8/enkacard/src/generator/one/background.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/constant.py` & `enkacard-3.3.8/enkacard/src/generator/one/constant.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/prop.py` & `enkacard-3.3.8/enkacard/src/generator/one/prop.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/skill.py` & `enkacard-3.3.8/enkacard/src/generator/one/skill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/stat.py` & `enkacard-3.3.8/enkacard/src/generator/one/stat.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/one/weapon.py` & `enkacard-3.3.8/enkacard/src/generator/one/weapon.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/profile_teample_one.py` & `enkacard-3.3.8/enkacard/src/generator/profile_teample_one.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/profile_teample_two.py` & `enkacard-3.3.8/enkacard/src/generator/profile_teample_two.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/teample_one.py` & `enkacard-3.3.8/enkacard/src/generator/teample_one.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/teample_two.py` & `enkacard-3.3.8/enkacard/src/generator/teample_two.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,36 +107,38 @@
         akasha_data = []
 
         
         for key in chartsData:
             if user_diagram:
                 name = options.assets.get_hash_map(options._mapHash.get(key))
                 value = options.map_enka(key, self.character.stats)
-                if value.value == 0 and chartsData[key] == 0:
+                if value.value == 0 and chartsData[key] == 0 or value.value == 0.0:
                     continue
                 try:
                     value = value.to_percentage()
                 except:
                     value = value.to_rounded()
                 chartsData[key] = options.format_value(key, chartsData[key], options._mapProcent.get(key), 1)
                 user_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": value})
                 akasha_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": value})
             else:
                 name = options.assets.get_hash_map(options._mapHash.get(key))
                 value = options.map_enka(key, self.character.stats)
-                if value.value == 0 and chartsData[key] == 0:
+                if value.value == 0 and chartsData[key] == 0 or value.value == 0.0:
                     continue
                 try:
                     value = value.to_percentage()
                 except:
                     value = value.to_rounded()
                 chartsData[key] = options.format_value(key, chartsData[key], options._mapProcent.get(key), 1)
                 user_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": value})
                 akasha_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": chartsData[key]})
-                
+
+        print(akasha_data)
+        
         self.diagram = await diagram.RadialChart(user_data, akasha_data, self.character.element.value).create_normalized_radial_chart() #create_normalized_radial_chart(user_data,akasha_data,self.character.element.value)
 
     async def creat_stat(self):
         self.stat_background = Image.new("RGBA", (519, 601), (0,0,0,0))
         result = await stat.Stat(self.character.stats, self.character.element.value).start()
         if len(result) <= 1:
             x = 0
```

### Comparing `enkacard-3.3.7/enkacard/src/generator/two/artifact.py` & `enkacard-3.3.8/enkacard/src/generator/two/artifact.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/two/background.py` & `enkacard-3.3.8/enkacard/src/generator/two/background.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/two/skill.py` & `enkacard-3.3.8/enkacard/src/generator/two/skill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/generator/two/stat.py` & `enkacard-3.3.8/enkacard/src/generator/two/stat.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/modal/enkacardCread.py` & `enkacard-3.3.8/enkacard/src/modal/enkacardCread.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/modal/enkaToolsModel.py` & `enkacard-3.3.8/enkacard/src/modal/enkaToolsModel.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/pickle_cashe/data_characters.pkz` & `enkacard-3.3.8/enkacard/src/pickle_cashe/data_characters.pkz`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/utils/affixes.py` & `enkacard-3.3.8/enkacard/src/utils/affixes.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/utils/diagram.py` & `enkacard-3.3.8/enkacard/src/utils/diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         plt.close(fig)
 
         return img
 
     @staticmethod
     def _get_value(value_info, max_value_dict):
         max_value = max_value_dict.get(value_info['name'], None)
-        if max_value is None:
+        if max_value is None or max_value == 0:
             return 1
         if value_info['value'] > max_value:
             normalized_value = 7 + (value_info['value'] - max_value) / (max_value * 0.3)
             return min(7.5, normalized_value)
         else:
             return int(1 + 5 * ((value_info['value'] / max_value) ** 2.5))
```

### Comparing `enkacard-3.3.7/enkacard/src/utils/git.py` & `enkacard-3.3.8/enkacard/src/utils/git.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/utils/options.py` & `enkacard-3.3.8/enkacard/src/utils/options.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/utils/pickle_cashe.py` & `enkacard-3.3.8/enkacard/src/utils/pickle_cashe.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/enkacard/src/utils/pill.py` & `enkacard-3.3.8/enkacard/src/utils/pill.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 
 async def get_icon_add(prop_id, recolor = (255,255,255), size = None):
     if f"{prop_id}_{recolor}_{size}" in cache:
         return cache[f"{prop_id}_{recolor}_{size}"]
     
     icon = await git.ImageCache().download_icon_stats(prop_id = prop_id)
-    if "ADD_HURT" not in prop_id:
+    if "ADD_HURT" not in prop_id and prop_id != "FIGHT_PROP_PHYSICAL_ADD_HURT":
         icon = await recolor_image(icon,recolor)
     if size:
         icon.thumbnail(size)
         cache[f"{prop_id}_{recolor}_{size}"] = icon.convert("RGBA").copy()
         return cache[f"{prop_id}_{recolor}_{size}"]
     else:
         cache[f"{prop_id}_{recolor}_{size}"] = icon.convert("RGBA").copy()
```

### Comparing `enkacard-3.3.7/enkacard/src/utils/translation.py` & `enkacard-3.3.8/enkacard/src/utils/translation.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/pyproject.toml` & `enkacard-3.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enkacard"
-version = "3.3.7"
+version = "3.3.8"
 description = "An asynchronous module and API that allows you to connect to your bot the generation of Genshin character cards from the Enka.Network website."
 authors = ["None"]
 
 readme = 'README.md'  # Поддерживаются файлы в формате Markdown
 
 repository = "https://github.com/DEViantUA/EnkaCard"
 homepage = "https://github.com/DEViantUA/EnkaCard"
```

### Comparing `enkacard-3.3.7/README.md` & `enkacard-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.7/PKG-INFO` & `enkacard-3.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkacard
-Version: 3.3.7
+Version: 3.3.8
 Summary: An asynchronous module and API that allows you to connect to your bot the generation of Genshin character cards from the Enka.Network website.
 Home-page: https://github.com/DEViantUA/EnkaCard
 Author: None
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

