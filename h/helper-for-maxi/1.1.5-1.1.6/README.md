# Comparing `tmp/helper_for_maxi-1.1.5.tar.gz` & `tmp/helper_for_maxi-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helper_for_maxi-1.1.5.tar", last modified: Sat Apr 27 16:26:29 2024, max compression
+gzip compressed data, was "helper_for_maxi-1.1.6.tar", last modified: Fri May  3 15:20:45 2024, max compression
```

## Comparing `helper_for_maxi-1.1.5.tar` & `helper_for_maxi-1.1.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 16:26:29.200361 helper_for_maxi-1.1.5/
--rw-rw-rw-   0        0        0     1088 2024-03-21 21:19:01.000000 helper_for_maxi-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      962 2024-04-27 16:26:29.199360 helper_for_maxi-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-26 23:52:41.000000 helper_for_maxi-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 16:26:29.151188 helper_for_maxi-1.1.5/helper/
--rw-rw-rw-   0        0        0      774 2024-03-26 20:16:33.000000 helper_for_maxi-1.1.5/helper/__init__.py
--rw-rw-rw-   0        0        0      331 2023-11-06 19:03:02.000000 helper_for_maxi-1.1.5/helper/append_clipboard.py
--rw-rw-rw-   0        0        0     1055 2023-08-21 18:12:43.000000 helper_for_maxi-1.1.5/helper/better_color_input.py
--rw-rw-rw-   0        0        0      575 2023-08-21 18:19:43.000000 helper_for_maxi-1.1.5/helper/better_input.py
--rw-rw-rw-   0        0        0      659 2023-02-26 18:22:53.000000 helper_for_maxi-1.1.5/helper/better_print.py
--rw-rw-rw-   0        0        0      823 2023-08-21 18:27:01.000000 helper_for_maxi-1.1.5/helper/color_input.py
--rw-rw-rw-   0        0        0      621 2024-03-26 20:10:50.000000 helper_for_maxi-1.1.5/helper/key_dict.py
--rw-rw-rw-   0        0        0     1803 2023-12-25 14:34:47.000000 helper_for_maxi-1.1.5/helper/kwargs_handler.py
--rw-rw-rw-   0        0        0      335 2023-08-21 18:37:51.000000 helper_for_maxi-1.1.5/helper/output_stdout.py
--rw-rw-rw-   0        0        0     3149 2023-12-25 14:42:02.000000 helper_for_maxi-1.1.5/helper/terminal.py
-drwxrwxrwx   0        0        0        0 2024-04-27 16:26:29.198363 helper_for_maxi-1.1.5/helper_for_maxi.egg-info/
--rw-rw-rw-   0        0        0      962 2024-04-27 16:26:29.000000 helper_for_maxi-1.1.5/helper_for_maxi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      929 2024-04-27 16:26:29.000000 helper_for_maxi-1.1.5/helper_for_maxi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 16:26:29.000000 helper_for_maxi-1.1.5/helper_for_maxi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-27 16:26:29.000000 helper_for_maxi-1.1.5/helper_for_maxi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 16:26:29.000000 helper_for_maxi-1.1.5/helper_for_maxi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 16:26:29.187843 helper_for_maxi-1.1.5/maximyoga/
-drwxrwxrwx   0        0        0        0 2024-04-27 16:26:29.190852 helper_for_maxi-1.1.5/maximyoga/Terminal/
--rw-rw-rw-   0        0        0      172 2024-04-26 21:34:02.000000 helper_for_maxi-1.1.5/maximyoga/Terminal/__init__.py
--rw-rw-rw-   0        0        0     4436 2024-04-27 16:15:54.000000 helper_for_maxi-1.1.5/maximyoga/Terminal/_choices_interface.py
-drwxrwxrwx   0        0        0        0 2024-04-27 16:26:29.196352 helper_for_maxi-1.1.5/maximyoga/Terminal/color/
--rw-rw-rw-   0        0        0      230 2024-04-26 21:52:37.000000 helper_for_maxi-1.1.5/maximyoga/Terminal/color/__init__.py
--rw-rw-rw-   0        0        0      469 2024-04-26 21:52:59.000000 helper_for_maxi-1.1.5/maximyoga/Terminal/color/_background.py
--rw-rw-rw-   0        0        0      506 2024-04-26 21:53:06.000000 helper_for_maxi-1.1.5/maximyoga/Terminal/color/_foreground.py
--rw-rw-rw-   0        0        0      691 2024-03-26 21:46:16.000000 helper_for_maxi-1.1.5/maximyoga/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-27 16:22:28.000000 helper_for_maxi-1.1.5/maximyoga/_append_clipboard.py
--rw-rw-rw-   0        0        0      733 2024-04-26 22:02:44.000000 helper_for_maxi-1.1.5/maximyoga/_better_color_input.py
--rw-rw-rw-   0        0        0      442 2024-04-26 21:59:50.000000 helper_for_maxi-1.1.5/maximyoga/_better_input.py
--rw-rw-rw-   0        0        0      466 2024-04-26 22:00:43.000000 helper_for_maxi-1.1.5/maximyoga/_better_print.py
--rw-rw-rw-   0        0        0      478 2024-04-26 22:04:38.000000 helper_for_maxi-1.1.5/maximyoga/_color_input.py
--rw-rw-rw-   0        0        0      317 2024-04-26 22:17:15.000000 helper_for_maxi-1.1.5/maximyoga/_key_dict.py
--rw-rw-rw-   0        0        0     2127 2024-04-26 23:42:00.000000 helper_for_maxi-1.1.5/maximyoga/_kwargs_handler.py
--rw-rw-rw-   0        0        0      227 2024-04-26 23:42:26.000000 helper_for_maxi-1.1.5/maximyoga/_output_stdout.py
--rw-rw-rw-   0        0        0     3448 2024-04-27 16:23:28.000000 helper_for_maxi-1.1.5/maximyoga/_repr_iterable.py
--rw-rw-rw-   0        0        0      108 2022-12-23 14:16:08.000000 helper_for_maxi-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      713 2024-04-27 16:26:29.202363 helper_for_maxi-1.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:45.591808 helper_for_maxi-1.1.6/
+-rw-rw-rw-   0        0        0     1088 2024-03-21 21:19:01.000000 helper_for_maxi-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      939 2024-05-03 15:20:45.591808 helper_for_maxi-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-26 23:52:41.000000 helper_for_maxi-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:45.522105 helper_for_maxi-1.1.6/helper/
+-rw-rw-rw-   0        0        0      774 2024-03-26 20:16:33.000000 helper_for_maxi-1.1.6/helper/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-11-06 19:03:02.000000 helper_for_maxi-1.1.6/helper/append_clipboard.py
+-rw-rw-rw-   0        0        0     1055 2023-08-21 18:12:43.000000 helper_for_maxi-1.1.6/helper/better_color_input.py
+-rw-rw-rw-   0        0        0      575 2023-08-21 18:19:43.000000 helper_for_maxi-1.1.6/helper/better_input.py
+-rw-rw-rw-   0        0        0      659 2023-02-26 18:22:53.000000 helper_for_maxi-1.1.6/helper/better_print.py
+-rw-rw-rw-   0        0        0      823 2023-08-21 18:27:01.000000 helper_for_maxi-1.1.6/helper/color_input.py
+-rw-rw-rw-   0        0        0      621 2024-03-26 20:10:50.000000 helper_for_maxi-1.1.6/helper/key_dict.py
+-rw-rw-rw-   0        0        0     1803 2023-12-25 14:34:47.000000 helper_for_maxi-1.1.6/helper/kwargs_handler.py
+-rw-rw-rw-   0        0        0      335 2023-08-21 18:37:51.000000 helper_for_maxi-1.1.6/helper/output_stdout.py
+-rw-rw-rw-   0        0        0     3149 2023-12-25 14:42:02.000000 helper_for_maxi-1.1.6/helper/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:45.590809 helper_for_maxi-1.1.6/helper_for_maxi.egg-info/
+-rw-rw-rw-   0        0        0      939 2024-05-03 15:20:45.000000 helper_for_maxi-1.1.6/helper_for_maxi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      966 2024-05-03 15:20:45.000000 helper_for_maxi-1.1.6/helper_for_maxi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:20:45.000000 helper_for_maxi-1.1.6/helper_for_maxi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-03 15:20:45.000000 helper_for_maxi-1.1.6/helper_for_maxi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 15:20:45.000000 helper_for_maxi-1.1.6/helper_for_maxi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:45.580274 helper_for_maxi-1.1.6/maximyoga/
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:45.584281 helper_for_maxi-1.1.6/maximyoga/Terminal/
+-rw-rw-rw-   0        0        0      172 2024-04-26 21:34:02.000000 helper_for_maxi-1.1.6/maximyoga/Terminal/__init__.py
+-rw-rw-rw-   0        0        0     4436 2024-04-27 16:15:54.000000 helper_for_maxi-1.1.6/maximyoga/Terminal/_choices_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:20:45.588815 helper_for_maxi-1.1.6/maximyoga/Terminal/color/
+-rw-rw-rw-   0        0        0      230 2024-04-26 21:52:37.000000 helper_for_maxi-1.1.6/maximyoga/Terminal/color/__init__.py
+-rw-rw-rw-   0        0        0      469 2024-04-26 21:52:59.000000 helper_for_maxi-1.1.6/maximyoga/Terminal/color/_background.py
+-rw-rw-rw-   0        0        0      506 2024-04-26 21:53:06.000000 helper_for_maxi-1.1.6/maximyoga/Terminal/color/_foreground.py
+-rw-rw-rw-   0        0        0      691 2024-03-26 21:46:16.000000 helper_for_maxi-1.1.6/maximyoga/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-27 16:22:28.000000 helper_for_maxi-1.1.6/maximyoga/_append_clipboard.py
+-rw-rw-rw-   0        0        0      733 2024-04-26 22:02:44.000000 helper_for_maxi-1.1.6/maximyoga/_better_color_input.py
+-rw-rw-rw-   0        0        0      442 2024-04-26 21:59:50.000000 helper_for_maxi-1.1.6/maximyoga/_better_input.py
+-rw-rw-rw-   0        0        0      466 2024-04-26 22:00:43.000000 helper_for_maxi-1.1.6/maximyoga/_better_print.py
+-rw-rw-rw-   0        0        0     1054 2024-05-03 15:10:59.000000 helper_for_maxi-1.1.6/maximyoga/_check_params_decorator.py
+-rw-rw-rw-   0        0        0      478 2024-04-26 22:04:38.000000 helper_for_maxi-1.1.6/maximyoga/_color_input.py
+-rw-rw-rw-   0        0        0      317 2024-04-26 22:17:15.000000 helper_for_maxi-1.1.6/maximyoga/_key_dict.py
+-rw-rw-rw-   0        0        0     2683 2024-05-03 15:03:02.000000 helper_for_maxi-1.1.6/maximyoga/_kwargs_handler.py
+-rw-rw-rw-   0        0        0      227 2024-04-26 23:42:26.000000 helper_for_maxi-1.1.6/maximyoga/_output_stdout.py
+-rw-rw-rw-   0        0        0     3448 2024-04-27 16:23:28.000000 helper_for_maxi-1.1.6/maximyoga/_repr_iterable.py
+-rw-rw-rw-   0        0        0      108 2022-12-23 14:16:08.000000 helper_for_maxi-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      704 2024-05-03 15:20:45.599337 helper_for_maxi-1.1.6/setup.cfg
```

### Comparing `helper_for_maxi-1.1.5/LICENSE` & `helper_for_maxi-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/PKG-INFO` & `helper_for_maxi-1.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: helper_for_maxi
-Version: 1.1.5
+Version: 1.1.6
 Summary: Contains all Functions
 Author: Maxi Myoga
-Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.5/package
-Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.5/CHANGELOG.md
+Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.6/package
+Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.6/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
-Requires-Dist: typing
 Requires-Dist: pynput
 Requires-Dist: pygetwindow
 
 # Helper for Maxi
 
 All the Functions I could need multiple times
```

### Comparing `helper_for_maxi-1.1.5/helper/__init__.py` & `helper_for_maxi-1.1.6/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/better_color_input.py` & `helper_for_maxi-1.1.6/helper/better_color_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/better_input.py` & `helper_for_maxi-1.1.6/helper/better_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/better_print.py` & `helper_for_maxi-1.1.6/helper/better_print.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/color_input.py` & `helper_for_maxi-1.1.6/helper/color_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/key_dict.py` & `helper_for_maxi-1.1.6/helper/key_dict.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/kwargs_handler.py` & `helper_for_maxi-1.1.6/helper/kwargs_handler.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper/terminal.py` & `helper_for_maxi-1.1.6/helper/terminal.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/helper_for_maxi.egg-info/PKG-INFO` & `helper_for_maxi-1.1.6/helper_for_maxi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: helper_for_maxi
-Version: 1.1.5
+Version: 1.1.6
 Summary: Contains all Functions
 Author: Maxi Myoga
-Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.5/package
-Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.5/CHANGELOG.md
+Project-URL: Github, https://github.com/CatMaxiMyoga/helper_for_maxi/tree/main/1.1.6/package
+Project-URL: Changelog, https://github.com/CatMaxiMyoga/helper_for_maxi/blob/main/1.1.6/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
-Requires-Dist: typing
 Requires-Dist: pynput
 Requires-Dist: pygetwindow
 
 # Helper for Maxi
 
 All the Functions I could need multiple times
```

### Comparing `helper_for_maxi-1.1.5/helper_for_maxi.egg-info/SOURCES.txt` & `helper_for_maxi-1.1.6/helper_for_maxi.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 helper_for_maxi.egg-info/requires.txt
 helper_for_maxi.egg-info/top_level.txt
 maximyoga/__init__.py
 maximyoga/_append_clipboard.py
 maximyoga/_better_color_input.py
 maximyoga/_better_input.py
 maximyoga/_better_print.py
+maximyoga/_check_params_decorator.py
 maximyoga/_color_input.py
 maximyoga/_key_dict.py
 maximyoga/_kwargs_handler.py
 maximyoga/_output_stdout.py
 maximyoga/_repr_iterable.py
 maximyoga/Terminal/__init__.py
 maximyoga/Terminal/_choices_interface.py
```

### Comparing `helper_for_maxi-1.1.5/maximyoga/Terminal/_choices_interface.py` & `helper_for_maxi-1.1.6/maximyoga/Terminal/_choices_interface.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/maximyoga/__init__.py` & `helper_for_maxi-1.1.6/maximyoga/__init__.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/maximyoga/_better_color_input.py` & `helper_for_maxi-1.1.6/maximyoga/_better_color_input.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/maximyoga/_kwargs_handler.py` & `helper_for_maxi-1.1.6/maximyoga/_kwargs_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 class KWArgsHandler[_VT]:
+	type __allowedKeywordsType = str |\
+		tuple[str, type | tuple[type, ...]] |\
+		tuple[str, type | tuple[type, ...], object]
+
 	def __init__(
 			self,
 			kwargs: dict[str, _VT],
-			*allowedKeywords: str | tuple[str, type | tuple[type, ...], object]
+			*allowedKeywords: __allowedKeywordsType
 	) -> None:
 		r"""
 		Handles Keyword Arguments for a function
 		:param kwargs:
 		:param allowedKeywords:
+		:raises ValueError: Invalid format for 'allowedKeywords' or disallowed keyword in 'kwargs'
+		:raises TypeError: Invalid value type for keyword in 'kwargs'
 		"""
 		allowedKeywords_: dict[str, tuple[type | tuple[type, ...], object]] = {}
 		self.kwargs = {}
-		print(allowedKeywords)
 		for kw in allowedKeywords:
 			if isinstance(kw, tuple) and len(kw) in (2, 3):
 				keyword, argType = kw[:2]
 				defValue = kw[2] if len(kw) == 3 else None
 				allowedKeywords_[keyword] = (argType, defValue)
 			elif isinstance(kw, str):
 				allowedKeywords_[kw] = (object, None)
 			else:
 				raise ValueError('Invalid format for allowedKeywords. \n'
 				                 'Use either ("keyword", type, defaultValue) ("keyword", type) or "keyword".')
-		print(allowedKeywords_)
 		for keyword, value in kwargs.items():
 			if keyword not in allowedKeywords_:
 				raise ValueError(f"Invalid keyword '{keyword}' provided.")
 			if not isinstance(value, expVT := allowedKeywords_[keyword][0]):
 				raise TypeError(
 					f"Invalid type for keyword '{keyword}'. Expected {
 						expVT.__name__ 
@@ -42,14 +46,23 @@
 			if valueType is not None and not isinstance(value, valueType):
 				raise TypeError(
 					f"Invalid type for keyword '{keyword}'. Expected {
 						valueType.__name__ if not isinstance(valueType, tuple) else (vt.__name__ for vt in valueType)
 					}, got {type(value).__name__}.")
 			self.kwargs[keyword] = value
 
-	def __getattr__(self, name) -> _VT:
-		if name in self.kwargs:
-			return self.kwargs[name]
-		raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'.")
+	def __getattr__(self, attr) -> _VT:
+		if attr in self.kwargs:
+			return self.kwargs[attr]
+		raise AttributeError(f"'KWArgsHandler' object has no attribute '{attr}'.")
+
+	def __getitem__(self, item):
+		if isinstance(item, int):
+			raise IndexError("KWArgsHandler does not support indexing!")
+		elif not isinstance(item, str):
+			raise KeyError("KWArgsHandler only supports keys of type 'str'!")
+		if item in self.kwargs:
+			return self.kwargs[item]
+		raise KeyError(f"KWArgsHandler object has no attribute '{item}'")
 
 	def __repr__(self) -> str:
 		return f"KWArgsHandler: {self.kwargs}"
```

### Comparing `helper_for_maxi-1.1.5/maximyoga/_repr_iterable.py` & `helper_for_maxi-1.1.6/maximyoga/_repr_iterable.py`

 * *Files identical despite different names*

### Comparing `helper_for_maxi-1.1.5/setup.cfg` & `helper_for_maxi-1.1.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 656c 7065 725f 666f 725f 6d61   = helper_for_ma
 00000020: 7869 0d0a 7665 7273 696f 6e20 3d20 312e  xi..version = 1.
-00000030: 312e 350d 0a61 7574 686f 7220 3d20 4d61  1.5..author = Ma
+00000030: 312e 360d 0a61 7574 686f 7220 3d20 4d61  1.6..author = Ma
 00000040: 7869 204d 796f 6761 0d0a 6465 7363 7269  xi Myoga..descri
 00000050: 7074 696f 6e20 3d20 436f 6e74 6169 6e73  ption = Contains
 00000060: 2061 6c6c 2046 756e 6374 696f 6e73 0d0a   all Functions..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 000000a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 000000b0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
 000000c0: 6e0d 0a70 726f 6a65 6374 5f75 726c 7320  n..project_urls 
 000000d0: 3d20 0d0a 0947 6974 6875 6220 3d20 6874  = ...Github = ht
 000000e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000f0: 2f43 6174 4d61 7869 4d79 6f67 612f 6865  /CatMaxiMyoga/he
 00000100: 6c70 6572 5f66 6f72 5f6d 6178 692f 7472  lper_for_maxi/tr
-00000110: 6565 2f6d 6169 6e2f 312e 312e 352f 7061  ee/main/1.1.5/pa
+00000110: 6565 2f6d 6169 6e2f 312e 312e 362f 7061  ee/main/1.1.6/pa
 00000120: 636b 6167 650d 0a09 4368 616e 6765 6c6f  ckage...Changelo
 00000130: 6720 3d20 6874 7470 733a 2f2f 6769 7468  g = https://gith
 00000140: 7562 2e63 6f6d 2f43 6174 4d61 7869 4d79  ub.com/CatMaxiMy
 00000150: 6f67 612f 6865 6c70 6572 5f66 6f72 5f6d  oga/helper_for_m
 00000160: 6178 692f 626c 6f62 2f6d 6169 6e2f 312e  axi/blob/main/1.
-00000170: 312e 352f 4348 414e 4745 4c4f 472e 6d64  1.5/CHANGELOG.md
+00000170: 312e 362f 4348 414e 4745 4c4f 472e 6d64  1.6/CHANGELOG.md
 00000180: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
 00000190: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
 000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000001b0: 6e20 3a3a 2033 0d0a 0944 6576 656c 6f70  n :: 3...Develop
 000001c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
 000001d0: 202d 2041 6c70 6861 0d0a 094f 7065 7261   - Alpha...Opera
 000001e0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
@@ -33,13 +33,12 @@
 00000200: 6f77 730d 0a0d 0a5b 6f70 7469 6f6e 735d  ows....[options]
 00000210: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 00000220: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
 00000230: 7265 7320 3d20 3e3d 2033 2e31 320d 0a69  res = >= 3.12..i
 00000240: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
 00000250: 6174 6120 3d20 5472 7565 0d0a 696e 7374  ata = True..inst
 00000260: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-00000270: 0a09 7079 7065 7263 6c69 700d 0a09 7479  ..pyperclip...ty
-00000280: 7069 6e67 0d0a 0970 796e 7075 740d 0a09  ping...pynput...
-00000290: 7079 6765 7477 696e 646f 770d 0a0d 0a5b  pygetwindow....[
-000002a0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000002b0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000002c0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000270: 0a09 7079 7065 7263 6c69 700d 0a09 7079  ..pyperclip...py
+00000280: 6e70 7574 0d0a 0970 7967 6574 7769 6e64  nput...pygetwind
+00000290: 6f77 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ow....[egg_info]
+000002a0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000002b0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

