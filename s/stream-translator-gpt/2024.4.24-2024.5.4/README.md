# Comparing `tmp/stream_translator_gpt-2024.4.24.tar.gz` & `tmp/stream_translator_gpt-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stream_translator_gpt-2024.4.24.tar", last modified: Wed Apr 24 15:26:35 2024, max compression
+gzip compressed data, was "stream_translator_gpt-2024.5.4.tar", last modified: Fri May  3 19:09:29 2024, max compression
```

## Comparing `stream_translator_gpt-2024.4.24.tar` & `stream_translator_gpt-2024.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:26:35.378684 stream_translator_gpt-2024.4.24/
--rw-rw-rw-   0        0        0     1089 2023-03-12 08:56:05.000000 stream_translator_gpt-2024.4.24/LICENSE
--rw-rw-rw-   0        0        0     6293 2024-04-24 15:26:35.377685 stream_translator_gpt-2024.4.24/PKG-INFO
--rw-rw-rw-   0        0        0    15478 2024-04-24 15:23:39.000000 stream_translator_gpt-2024.4.24/README.md
--rw-rw-rw-   0        0        0     4813 2024-03-26 11:06:30.000000 stream_translator_gpt-2024.4.24/README_PyPI.md
--rw-rw-rw-   0        0        0     1745 2024-04-24 15:25:58.000000 stream_translator_gpt-2024.4.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 15:26:35.378684 stream_translator_gpt-2024.4.24/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 15:26:35.360503 stream_translator_gpt-2024.4.24/stream_translator_gpt/
--rw-rw-rw-   0        0        0        0 2024-03-03 09:46:32.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/__init__.py
--rw-rw-rw-   0        0        0       68 2024-03-03 10:18:23.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/__main__.py
--rw-rw-rw-   0        0        0     5572 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_getter.py
--rw-rw-rw-   0        0        0     4102 2024-03-03 13:47:24.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_slicer.py
--rw-rw-rw-   0        0        0     3821 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_transcriber.py
--rw-rw-rw-   0        0        0      970 2024-03-25 19:53:37.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/common.py
--rw-rw-rw-   0        0        0     1384 2024-03-14 15:15:25.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/filters.py
--rw-rw-rw-   0        0        0     8300 2024-03-05 13:52:21.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/llm_translator.py
--rw-rw-rw-   0        0        0     2731 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/result_exporter.py
--rw-rw-rw-   0        0        0  1439299 2024-03-05 16:52:38.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/silero_vad.jit
--rw-rw-rw-   0        0        0    17087 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt/translator.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:26:35.377685 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/
--rw-rw-rw-   0        0        0     6293 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-24 15:26:35.000000 stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 19:09:29.063574 stream_translator_gpt-2024.5.4/
+-rw-rw-rw-   0        0        0     1089 2023-03-12 08:56:05.000000 stream_translator_gpt-2024.5.4/LICENSE
+-rw-rw-rw-   0        0        0     6292 2024-05-03 19:09:29.062577 stream_translator_gpt-2024.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15478 2024-05-03 19:05:57.000000 stream_translator_gpt-2024.5.4/README.md
+-rw-rw-rw-   0        0        0     4813 2024-03-26 11:06:30.000000 stream_translator_gpt-2024.5.4/README_PyPI.md
+-rw-rw-rw-   0        0        0     1744 2024-05-03 19:08:52.000000 stream_translator_gpt-2024.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 19:09:29.063574 stream_translator_gpt-2024.5.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 19:09:29.051614 stream_translator_gpt-2024.5.4/stream_translator_gpt/
+-rw-rw-rw-   0        0        0        0 2024-03-03 09:46:32.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-03-03 10:18:23.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/__main__.py
+-rw-rw-rw-   0        0        0     5572 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_getter.py
+-rw-rw-rw-   0        0        0     4102 2024-04-25 09:10:57.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_slicer.py
+-rw-rw-rw-   0        0        0     3821 2024-03-26 11:43:09.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_transcriber.py
+-rw-rw-rw-   0        0        0      968 2024-04-25 17:12:13.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/common.py
+-rw-rw-rw-   0        0        0     1384 2024-03-14 15:15:25.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/filters.py
+-rw-rw-rw-   0        0        0     8300 2024-04-25 09:26:14.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/llm_translator.py
+-rw-rw-rw-   0        0        0     2731 2024-04-16 06:16:00.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/result_exporter.py
+-rw-rw-rw-   0        0        0  1439299 2024-03-05 16:52:38.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/silero_vad.jit
+-rw-rw-rw-   0        0        0    17068 2024-05-03 19:08:00.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt/translator.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:09:29.062577 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/
+-rw-rw-rw-   0        0        0     6292 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-03 19:09:29.000000 stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/top_level.txt
```

### Comparing `stream_translator_gpt-2024.4.24/LICENSE` & `stream_translator_gpt-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/PKG-INFO` & `stream_translator_gpt-2024.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-translator-gpt
-Version: 2024.4.24
+Version: 2024.5.4
 Summary: Command line tool to transcribe & translate audio from livestreams in real time
 Author-email: ion <ionicbond3@gmail.com>
 Project-URL: Homepage, https://github.com/ionic-bond/stream-translator-gpt
 Project-URL: Issues, https://github.com/ionic-bond/stream-translator-gpt/issues
 Keywords: translator,translation,translate,transcribe,yt-dlp,vad,whisper,faster-whisper,whisper-api,gpt,gemini
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stream_translator_gpt-2024.4.24/README.md` & `stream_translator_gpt-2024.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 | :--------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | **Input Options**                  |
 | `URL`                              |               | The URL of the stream. If a local file path is filled in, it will be used as input. If fill in "device", the input will be obtained from your PC device.                                                 |
 | `--format`                         | wa*           | Stream format code, this parameter will be passed directly to yt-dlp.                                                                                                                                    |
 | `--cookies`                        |               | Used to open member-only stream, this parameter will be passed directly to yt-dlp.                                                                                                                       |
 | `--device_index`                   |               | The index of the device that needs to be recorded. If not set, the system default recording device will be used.                                                                                         |
 | **Audio Slicing Options**          |
-| `--frame_duration`                 | 0.1           | The unit that processes live streaming data in seconds.                                                                                                                                                  |
+| `--frame_duration`                 | 0.05          | The unit that processes live streaming data in seconds, should be >= 0.03                                                                                                                                |
 | `--continuous_no_speech_threshold` | 0.5           | Slice if there is no speech for a continuous period in second.                                                                                                                                           |
 | `--min_audio_length`               | 3.0           | Minimum slice audio length in seconds.                                                                                                                                                                   |
 | `--max_audio_length`               | 30.0          | Maximum slice audio length in seconds.                                                                                                                                                                   |
 | `--prefix_retention_length`        | 0.5           | The length of the retention prefix audio during slicing.                                                                                                                                                 |
 | `--vad_threshold`                  | 0.35          | The threshold of Voice activity detection. if the speech probability of a frame is higher than this value, then this frame is speech.                                                                    |
 | **Transcription Options**          |
 | `--model`                          | small         | Select model size. See [here](https://github.com/openai/whisper#available-models-and-languages) for available models.                                                                                    |
```

### Comparing `stream_translator_gpt-2024.4.24/README_PyPI.md` & `stream_translator_gpt-2024.5.4/README_PyPI.md`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/pyproject.toml` & `stream_translator_gpt-2024.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stream-translator-gpt"
-version = "2024.4.24"
+version = "2024.5.4"
 authors = [
   { name="ion", email="ionicbond3@gmail.com" },
 ]
 description = "Command line tool to transcribe & translate audio from livestreams in real time"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_getter.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_getter.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_slicer.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_slicer.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/audio_transcriber.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/audio_transcriber.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/common.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         obj = cls(**_auto_args(cls.__init__, kwargs))
         obj.loop(**_auto_args(obj.loop, kwargs))
 
 
 def sec2str(second: float):
     dt = datetime.utcfromtimestamp(second)
     result = dt.strftime('%H:%M:%S')
-    result += ',' + str(round(second * 10 % 10))
+    result += ',' + str(int(second * 10 % 10))
     return result
```

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/filters.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/filters.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/llm_translator.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/llm_translator.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/result_exporter.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/result_exporter.py`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/silero_vad.jit` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt/translator.py` & `stream_translator_gpt-2024.5.4/stream_translator_gpt/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,18 +157,19 @@
                         type=int,
                         default=None,
                         help='The index of the device that needs to be recorded. '
                         'If not set, the system default recording device will be used.')
     parser.add_argument('--print_all_devices',
                         action='store_true',
                         help='Print all audio devices info then exit.')
-    parser.add_argument('--frame_duration',
-                        type=float,
-                        default=0.1,
-                        help='The unit that processes live streaming data in seconds.')
+    parser.add_argument(
+        '--frame_duration',
+        type=float,
+        default=0.05,
+        help='The unit that processes live streaming data in seconds, should be >= 0.03')
     parser.add_argument('--continuous_no_speech_threshold',
                         type=float,
                         default=0.5,
                         help='Slice if there is no speech for a continuous period in second.')
     parser.add_argument('--min_audio_length',
                         type=float,
                         default=3.0,
```

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/PKG-INFO` & `stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-translator-gpt
-Version: 2024.4.24
+Version: 2024.5.4
 Summary: Command line tool to transcribe & translate audio from livestreams in real time
 Author-email: ion <ionicbond3@gmail.com>
 Project-URL: Homepage, https://github.com/ionic-bond/stream-translator-gpt
 Project-URL: Issues, https://github.com/ionic-bond/stream-translator-gpt/issues
 Keywords: translator,translation,translate,transcribe,yt-dlp,vad,whisper,faster-whisper,whisper-api,gpt,gemini
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stream_translator_gpt-2024.4.24/stream_translator_gpt.egg-info/SOURCES.txt` & `stream_translator_gpt-2024.5.4/stream_translator_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

