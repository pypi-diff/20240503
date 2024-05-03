# Comparing `tmp/whisperx_karaoke-0.1.0.tar.gz` & `tmp/whisperx_karaoke-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperx_karaoke-0.1.0.tar", last modified: Wed May  1 20:46:37 2024, max compression
+gzip compressed data, was "whisperx_karaoke-0.1.1.tar", last modified: Fri May  3 16:41:21 2024, max compression
```

## Comparing `whisperx_karaoke-0.1.0.tar` & `whisperx_karaoke-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:46:37.589052 whisperx_karaoke-0.1.0/
--rw-rw-rw-   0        0        0     1562 2024-05-01 20:46:37.588052 whisperx_karaoke-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-01 20:46:12.000000 whisperx_karaoke-0.1.0/README.md
--rw-rw-rw-   0        0        0      684 2024-05-01 20:20:48.000000 whisperx_karaoke-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 20:46:37.589052 whisperx_karaoke-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 20:46:37.570637 whisperx_karaoke-0.1.0/whisperx_karaoke/
--rw-rw-rw-   0        0        0        0 2024-05-01 14:49:15.000000 whisperx_karaoke-0.1.0/whisperx_karaoke/__init__.py
--rw-rw-rw-   0        0        0       47 2024-05-01 20:21:48.000000 whisperx_karaoke-0.1.0/whisperx_karaoke/__main__.py
--rw-rw-rw-   0        0        0     3869 2024-05-01 19:41:35.000000 whisperx_karaoke-0.1.0/whisperx_karaoke/ass.py
--rw-rw-rw-   0        0        0     4037 2024-05-01 20:39:01.000000 whisperx_karaoke-0.1.0/whisperx_karaoke/cli.py
--rw-rw-rw-   0        0        0     1739 2024-05-01 19:39:29.000000 whisperx_karaoke-0.1.0/whisperx_karaoke/resolver.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:46:37.587051 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/
--rw-rw-rw-   0        0        0     1562 2024-05-01 20:46:37.000000 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-05-01 20:46:37.000000 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:46:37.000000 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-01 20:46:37.000000 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-01 20:46:37.000000 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-01 20:46:37.000000 whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 16:41:21.558322 whisperx_karaoke-0.1.1/
+-rw-rw-rw-   0        0        0     2362 2024-05-03 16:41:21.557322 whisperx_karaoke-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2176 2024-05-03 16:15:25.000000 whisperx_karaoke-0.1.1/README.md
+-rw-rw-rw-   0        0        0      684 2024-05-03 16:41:09.000000 whisperx_karaoke-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 16:41:21.558322 whisperx_karaoke-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 16:41:21.550149 whisperx_karaoke-0.1.1/whisperx_karaoke/
+-rw-rw-rw-   0        0        0        0 2024-05-01 14:49:15.000000 whisperx_karaoke-0.1.1/whisperx_karaoke/__init__.py
+-rw-rw-rw-   0        0        0       47 2024-05-01 20:21:48.000000 whisperx_karaoke-0.1.1/whisperx_karaoke/__main__.py
+-rw-rw-rw-   0        0        0     4277 2024-05-03 16:17:42.000000 whisperx_karaoke-0.1.1/whisperx_karaoke/ass.py
+-rw-rw-rw-   0        0        0     4066 2024-05-03 14:58:30.000000 whisperx_karaoke-0.1.1/whisperx_karaoke/cli.py
+-rw-rw-rw-   0        0        0     1739 2024-05-03 14:41:51.000000 whisperx_karaoke-0.1.1/whisperx_karaoke/resolver.py
+drwxrwxrwx   0        0        0        0 2024-05-03 16:41:21.557322 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/
+-rw-rw-rw-   0        0        0     2362 2024-05-03 16:41:21.000000 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-03 16:41:21.000000 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 16:41:21.000000 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-03 16:41:21.000000 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 16:41:21.000000 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 16:41:21.000000 whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/top_level.txt
```

### Comparing `whisperx_karaoke-0.1.0/PKG-INFO` & `whisperx_karaoke-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 Metadata-Version: 2.1
 Name: whisperx-karaoke
-Version: 0.1.0
+Version: 0.1.1
 Author: Darwin
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: whisperx
 
 # README
 
+<a target="_blank" href="https://colab.research.google.com/github/darwintree/whisperx-karaoke/blob/main/main.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
 ## 介绍
 
-借助whisperx生成卡拉ok歌词所需的k轴ass文件。注意，生成的准确性与输入质量相关，请确保lrc文件的时间戳准确。
+借助whisperx生成卡拉ok歌词所需的k轴ass文件。注意，生成的准确性与输入质量相关，请确保lrc文件的时间戳准确。此外，使用UVR5处理后的人声文件作为输入会得到更准确的时间戳。
 
 ## 使用
 
+可以在windows本地使用或者在 Colab 中运行
+
 需要准备输入：
 
 1. 音频
 2. lrc文件（需要以行为单位的时间戳）
 
 之后在任意位置新建文件夹，放入这两个文件即可。
 
-## 安装
+### 在 Colab 中运行
+
+<a target="_blank" href="https://colab.research.google.com/github/darwintree/whisperx-karaoke/blob/main/main.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+选择运行时为 GPU，在默认工作文件夹内新建`raw`文件夹，之后将音频文件与lrc文件放入其中。依次执行单元格即可。
+
+### 在本地运行
+
+#### 安装依赖
 
 ```shell
 conda install pytorch==2.0.0 torchaudio==2.0.0 pytorch-cuda=11.8 -c pytorch -c nvidia
 pip install git+https://github.com/m-bain/whisperx.git
 pip install whisperx-karaoke
 ```
 
-## 使用
+#### 运行
 
 例如文件被放置在了 `./raw/song1` 文件夹内
 
 ```shell
 python -m whisperx_karaoke ./raw/song1
 # usage: __main__.py [-h] [--device DEVICE] [--language LANGUAGE] [--offset OFFSET] dir [dir ...]
 # __main__.py: error: the following arguments are required: dir
```

### Comparing `whisperx_karaoke-0.1.0/pyproject.toml` & `whisperx_karaoke-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "whisperx-karaoke"
 description = ""
-version     = "0.1.0"
+version     = "0.1.1"
 readme      = "README.md"
 requires-python = ">=3.10"
 authors = [
   { name= "Darwin" },
 ]
 license = { text = "MIT" }
 dependencies = [
```

### Comparing `whisperx_karaoke-0.1.0/whisperx_karaoke/ass.py` & `whisperx_karaoke-0.1.1/whisperx_karaoke/ass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from whisperx.types import SingleAlignedSegment, SingleWordSegment
+import datetime
 
 def formatted_word_with_length(text: str, milliseconds: int):
     return "{\\kf" + str(milliseconds) + "}" + text
 
 def insert(s: str, index: int, substring: str):
     return s[:index] + substring + s[index:]
 
@@ -15,43 +16,52 @@
     # if last != -1:
     #     print(words[last]["word"])
     return last
 
 def get_duration_mark(duraction_in_seconds: float):
     return "{\\kf" + str(int(100* duraction_in_seconds)) + "}"
 
+
+def convert_seconds_to_hhmmss(seconds):
+    time_delta = datetime.timedelta(seconds=seconds)
+    hours = time_delta.seconds // 3600
+    minutes = (time_delta.seconds % 3600) // 60
+    seconds = time_delta.seconds % 60
+    return f"{hours:02d}:{minutes:02d}:{seconds:2f}"
+
+
 def segment_to_ass_line(segment: SingleAlignedSegment, next_segment=None):
     words = segment["words"]
-    studying_substr = "Make it through"
+    studying_substr = ""
 
-    line_prefix = (
-        f"Dialogue: 0,{segment['start']:.3f},{segment['end']:.3f},orig,,0,0,0,,"
-    )
+    line_prefix = f"Dialogue: 0,{convert_seconds_to_hhmmss(segment['start'])},{convert_seconds_to_hhmmss(segment['end'])},orig,,0,0,0,,"
     last_word_end: float = segment["start"]
     # append word to the line
     last_index = -1
     line_lyric: str = segment["text"]
-    # try:
-    #     line_lyric.index(studying_substr)
-    #     print(segment)
-    # except:
-    #     pass
+    try:
+        if studying_substr:
+            line_lyric.index(studying_substr)
+            print(segment)
+    except:
+        pass
 
     last_duration_insertion = index_of_last_word_with_time(segment["words"])
     first_inserted = True
 
     for i in range(len(words)):
         word = words[i]
         if not word.get("end"):
             last_index = line_lyric.index(word["word"], last_index + 1)
-            # try:
-            #     line_lyric.index(studying_substr)
-            #     print(line_lyric)
-            # except:
-            #     pass
+            try:
+                if studying_substr:
+                    line_lyric.index(studying_substr)
+                    print(line_lyric)
+            except:
+                pass
             continue
 
         word_duration = word.get("end") - last_word_end
         # if this is the last duration insertion, duration takes segment end into account
         if i == last_duration_insertion:
             word_duration = segment["end"] - last_word_end
 
@@ -61,20 +71,21 @@
             line_lyric = insert(line_lyric, 0, duration_mark)
             first_inserted = False
         else:
             line_lyric = insert(line_lyric, place_to_insert_duration, duration_mark)
 
         last_index = place_to_insert_duration + len(duration_mark)
         last_word_end = word.get("end")
-        # try:
-        #     line_lyric.index(studying_substr)
-        #     print(i)
-        #     print(line_lyric)
-        # except:
-        #     pass
+        try:
+            if studying_substr:
+                line_lyric.index(studying_substr)
+                print(i)
+                print(line_lyric)
+        except:
+            pass
 
     # this means no duration insertion was made
     # use segment as duration
     if first_inserted:
         word_duration = segment["end"] - segment["start"]
         duration_mark = get_duration_mark(word_duration)
         line_lyric = insert(line_lyric, 0, duration_mark)
```

### Comparing `whisperx_karaoke-0.1.0/whisperx_karaoke/cli.py` & `whisperx_karaoke-0.1.1/whisperx_karaoke/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     result = whisperx.align(
         cleared["segments"],
         model_a,
         metadata,
         audio,
         device,
         return_char_alignments=False,
+        print_progress=True
     )
 
     use_lrc_start_and_end(result["segments"], cleared["segments"])
 
     ass_output = segments_to_ass_text(result["segments"])
     ass_filename = os.path.join(dir_path, f"{os.path.basename(audio_path)}.ass")
     with open(ass_filename, "w", encoding="utf-8") as f:
```

### Comparing `whisperx_karaoke-0.1.0/whisperx_karaoke/resolver.py` & `whisperx_karaoke-0.1.1/whisperx_karaoke/resolver.py`

 * *Files identical despite different names*

### Comparing `whisperx_karaoke-0.1.0/whisperx_karaoke.egg-info/PKG-INFO` & `whisperx_karaoke-0.1.1/whisperx_karaoke.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 Metadata-Version: 2.1
 Name: whisperx-karaoke
-Version: 0.1.0
+Version: 0.1.1
 Author: Darwin
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: whisperx
 
 # README
 
+<a target="_blank" href="https://colab.research.google.com/github/darwintree/whisperx-karaoke/blob/main/main.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
 ## 介绍
 
-借助whisperx生成卡拉ok歌词所需的k轴ass文件。注意，生成的准确性与输入质量相关，请确保lrc文件的时间戳准确。
+借助whisperx生成卡拉ok歌词所需的k轴ass文件。注意，生成的准确性与输入质量相关，请确保lrc文件的时间戳准确。此外，使用UVR5处理后的人声文件作为输入会得到更准确的时间戳。
 
 ## 使用
 
+可以在windows本地使用或者在 Colab 中运行
+
 需要准备输入：
 
 1. 音频
 2. lrc文件（需要以行为单位的时间戳）
 
 之后在任意位置新建文件夹，放入这两个文件即可。
 
-## 安装
+### 在 Colab 中运行
+
+<a target="_blank" href="https://colab.research.google.com/github/darwintree/whisperx-karaoke/blob/main/main.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+选择运行时为 GPU，在默认工作文件夹内新建`raw`文件夹，之后将音频文件与lrc文件放入其中。依次执行单元格即可。
+
+### 在本地运行
+
+#### 安装依赖
 
 ```shell
 conda install pytorch==2.0.0 torchaudio==2.0.0 pytorch-cuda=11.8 -c pytorch -c nvidia
 pip install git+https://github.com/m-bain/whisperx.git
 pip install whisperx-karaoke
 ```
 
-## 使用
+#### 运行
 
 例如文件被放置在了 `./raw/song1` 文件夹内
 
 ```shell
 python -m whisperx_karaoke ./raw/song1
 # usage: __main__.py [-h] [--device DEVICE] [--language LANGUAGE] [--offset OFFSET] dir [dir ...]
 # __main__.py: error: the following arguments are required: dir
```

