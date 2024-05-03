# Comparing `tmp/asyncgui_ext_clock-0.1.0.tar.gz` & `tmp/asyncgui_ext_clock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncgui_ext_clock-0.1.0.tar", max compression
+gzip compressed data, was "asyncgui_ext_clock-0.2.0.tar", max compression
```

## Comparing `asyncgui_ext_clock-0.1.0.tar` & `asyncgui_ext_clock-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1059 2024-01-15 07:23:25.776854 asyncgui_ext_clock-0.1.0/LICENSE
--rw-r--r--   0        0        0     1498 2024-01-19 07:56:59.509512 asyncgui_ext_clock-0.1.0/README.md
--rw-r--r--   0        0        0     1140 2024-01-18 03:04:34.168614 asyncgui_ext_clock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    20679 2024-01-19 07:54:34.382134 asyncgui_ext_clock-0.1.0/src/asyncgui_ext/clock.py
--rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 asyncgui_ext_clock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-23 12:51:00.638097 asyncgui_ext_clock-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1805 2024-05-03 11:27:56.708517 asyncgui_ext_clock-0.2.0/README.md
+-rw-r--r--   0        0        0     1186 2024-05-03 11:21:39.556898 asyncgui_ext_clock-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16525 2024-05-03 11:21:23.029090 asyncgui_ext_clock-0.2.0/src/asyncgui_ext/clock.py
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 asyncgui_ext_clock-0.2.0/PKG-INFO
```

### Comparing `asyncgui_ext_clock-0.1.0/LICENSE` & `asyncgui_ext_clock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncgui_ext_clock-0.1.0/pyproject.toml` & `asyncgui_ext_clock-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "asyncgui-ext-clock"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Nattōsai Mitō <flow4re2c@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/asyncgui/asyncgui-ext-clock'
 homepage = 'https://github.com/asyncgui/asyncgui-ext-clock'
 keywords = ['async', ]
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Developers',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Software Development :: Libraries',
     'Operating System :: OS Independent',
 ]
 packages = [
     { include = "asyncgui_ext", from = "src" },
 ]
```

### Comparing `asyncgui_ext_clock-0.1.0/PKG-INFO` & `asyncgui_ext_clock-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncgui-ext-clock
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/asyncgui/asyncgui-ext-clock
 License: MIT
 Keywords: async
 Author: Nattōsai Mitō
 Author-email: flow4re2c@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -12,85 +12,97 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: asyncgui (>=0.6,<0.7)
 Project-URL: Repository, https://github.com/asyncgui/asyncgui-ext-clock
 Description-Content-Type: text/markdown
 
 # Clock
 
-An event scheduler.
+*An event scheduler designed for asyncgui programs.*
+
+First, take a look at the callback-style code below that has nothing to do with `asyncgui`.
+If you've ever used `Kivy` or `Pyglet`, you may find it familiar.
 
 ```python
 from asyncgui_ext.clock import Clock
 
 clock = Clock()
 
 # Schedules a function to be called after a delay of 20 time units.
 clock.schedule_once(lambda dt: print("Hello"), 20)
 
 # Advances the clock by 10 time units.
 clock.tick(10)
 
-# The clock advanced by a total of 20 time units, and the callback function will be called.
+# The clock advanced by a total of 20 time units.
+# The callback function will be called.
 clock.tick(10)  # => Hello
 ```
 
-It also supports async-style APIs. The code below does the same thing as the previous one but in an async-style.
+Next one is async/await-style code that involves `asyncgui`, and does the same thing as the previous.
 
 ```python
 import asyncgui
-from asyncgui_ext.clock import Clock
+from asyncgui_ext.clock import Clock, sleep
 
 clock = Clock()
 
-async def main():
-    await clock.sleep(20)
+async def async_fn():
+    await sleep(clock, 20)
     print("Hello")
 
-asyncgui.start(main())
+asyncgui.start(async_fn())
 clock.tick(10)
 clock.tick(10)  # => Hello
 ```
 
-The two examples above effectively illustrate how this module works, but they are not practical.
+These two examples effectively illustrate how this module works but they are not practical.
 In a real-world program, you probably want to call ``clock.tick()`` in a loop or schedule it to be called repeatedly using another scheduling API.
-For example, if you are using `PyGame`, you want to do:
+For example, if you are using `PyGame`, you may want to do:
 
 ```python
 clock = pygame.time.Clock()
-vclock = asyncui_ext.clock.Clock()
+vclock = asyncgui_ext.clock.Clock()
 
 # main loop
 while running:
     ...
 
     dt = clock.tick(fps)
     vclock.tick(dt)
 ```
 
-And if you are using `Kivy`, you want to do:
+And if you are using `Kivy`, you may want to do:
 
 ```python
 from kivy.clock import Clock
-vclock = asyncui_ext.clock.Clock()
 
+vclock = asyncui_ext.clock.Clock()
 Clock.schedule_interval(vclock.tick, 0)
 ```
 
 ## Installation
 
+Pin the minor version.
+
 ```
-poetry add asyncgui-ext-clock@~0.1
-pip install "asyncgui-ext-clock>=0.1,<0.2"
+poetry add asyncgui-ext-clock@~0.2
+pip install "asyncgui-ext-clock>=0.2,<0.3"
 ```
 
 ## Tested on
 
 - CPython 3.10
 - CPython 3.11
+- CPython 3.12
+
+## Misc
+
+- [YouTube Demo](https://youtu.be/kPVzO8fF0yg) (with Kivy)
```

