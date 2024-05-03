# Comparing `tmp/open-ephys-audio-0.1.6.tar.gz` & `tmp/open_ephys_audio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-ephys-audio-0.1.6.tar", last modified: Tue Dec  5 16:03:26 2023, max compression
+gzip compressed data, was "open_ephys_audio-0.1.7.tar", last modified: Fri May  3 13:50:57 2024, max compression
```

## Comparing `open-ephys-audio-0.1.6.tar` & `open_ephys_audio-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-05 16:03:26.042055 open-ephys-audio-0.1.6/
--rw-r--r--   0 dmeliza    (503) staff       (20)     2189 2023-12-05 16:03:26.041725 open-ephys-audio-0.1.6/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)     1563 2023-09-21 15:21:56.000000 open-ephys-audio-0.1.6/README.md
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-05 16:03:26.031363 open-ephys-audio-0.1.6/oeaudio/
--rw-r--r--   0 dmeliza    (503) staff       (20)       46 2023-12-05 16:02:38.000000 open-ephys-audio-0.1.6/oeaudio/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)       64 2020-10-26 16:44:29.000000 open-ephys-audio-0.1.6/oeaudio/__main__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     6547 2023-12-05 15:24:24.000000 open-ephys-audio-0.1.6/oeaudio/core.py
--rw-r--r--   0 dmeliza    (503) staff       (20)    10408 2023-12-05 15:24:53.000000 open-ephys-audio-0.1.6/oeaudio/script.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-05 16:03:26.041187 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/
--rw-r--r--   0 dmeliza    (503) staff       (20)     2189 2023-12-05 16:03:25.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      398 2023-12-05 16:03:26.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/SOURCES.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-12-05 16:03:25.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/dependency_links.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)       56 2023-12-05 16:03:25.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/entry_points.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2020-10-26 16:44:43.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/not-zip-safe
--rw-r--r--   0 dmeliza    (503) staff       (20)       41 2023-12-05 16:03:25.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/requires.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        8 2023-12-05 16:03:25.000000 open-ephys-audio-0.1.6/open_ephys_audio.egg-info/top_level.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)       90 2020-10-26 16:44:29.000000 open-ephys-audio-0.1.6/pyproject.toml
--rw-r--r--   0 dmeliza    (503) staff       (20)      922 2023-12-05 16:03:26.044096 open-ephys-audio-0.1.6/setup.cfg
--rw-r--r--   0 dmeliza    (503) staff       (20)      107 2021-01-08 19:13:18.000000 open-ephys-audio-0.1.6/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2024-05-03 13:50:57.357952 open_ephys_audio-0.1.7/
+-rw-r--r--   0 dmeliza    (503) staff       (20)      801 2024-05-03 13:50:57.357763 open_ephys_audio-0.1.7/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2845 2024-02-01 20:25:26.000000 open_ephys_audio-0.1.7/README.rst
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2024-05-03 13:50:57.351417 open_ephys_audio-0.1.7/oeaudio/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       22 2024-05-03 13:50:33.000000 open_ephys_audio-0.1.7/oeaudio/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)       64 2020-10-26 16:44:29.000000 open_ephys_audio-0.1.7/oeaudio/__main__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     6534 2024-05-03 13:50:33.000000 open_ephys_audio-0.1.7/oeaudio/core.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)    10413 2024-05-03 13:50:33.000000 open_ephys_audio-0.1.7/oeaudio/script.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2024-05-03 13:50:57.357392 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)      801 2024-05-03 13:50:57.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      399 2024-05-03 13:50:57.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2024-05-03 13:50:57.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)       56 2024-05-03 13:50:57.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/entry_points.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2020-10-26 16:44:43.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)       43 2024-05-03 13:50:57.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/requires.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        8 2024-05-03 13:50:57.000000 open_ephys_audio-0.1.7/open_ephys_audio.egg-info/top_level.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)      307 2024-01-29 18:15:33.000000 open_ephys_audio-0.1.7/pyproject.toml
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1037 2024-05-03 13:50:57.360363 open_ephys_audio-0.1.7/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)       83 2024-01-16 21:42:44.000000 open_ephys_audio-0.1.7/setup.py
```

### Comparing `open-ephys-audio-0.1.6/oeaudio/core.py` & `open_ephys_audio-0.1.7/oeaudio/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # -*- mode: python -*-
 import datetime
 import logging
 from typing import Optional
 
 import sounddevice as sd
 import zmq
@@ -83,14 +82,15 @@
 
     def read(self, block_size):
         pos = self.fp.tell()
         data = self.fp.buffer_read(block_size, dtype="float32")
         if self.click is None or self.fp.channels > 1 or len(data) == 0:
             return data
         data = np.frombuffer(data, dtype="float32")
+        # log.debug("- read %d samples", data.size)
         sync = np.zeros_like(data)
         if pos == 0:
             click_frames = int(self.click * self.samplerate / 1000.0)
             sync[:click_frames] = 1.0
         data = np.column_stack((data, sync))
         return memoryview(data).cast("B")
 
@@ -170,37 +170,35 @@
         else:
             self.socket.send_string(message)
             # req sockets have to be read after each message
             ret = self.socket.recv_string()
             if expected is not None and ret != expected:
                 log.error(" - unexpected reply: %s", ret)
                 raise RuntimeError(
-                    "open-ephys replied '%s', expecting '%s'" % (ret, expected)
+                    f"open-ephys replied '{ret}', expecting '{expected}'"
                 )
             log.debug(" - reply: %s", ret)
             return ret
 
     def start_acquisition(self):
         log.info("open-ephys: starting acquisition")
         now = datetime.datetime.now()
         logfile_name = now.strftime("oeaudio_%Y%m%d-%H%M%S.log")
         log.info("logging open-ephys messages to %s", logfile_name)
-        self.logfile = open(logfile_name, "wt")
+        self.logfile = open(logfile_name, "w")
         self._send("StartAcquisition", "StartedAcquisition")
 
     def stop_acquisition(self):
         log.info("open-ephys: stopping acquisition")
         self._send("StopAcquisition", "StoppedAcquisition")
         self.logfile.close()
         self.logfile = None
 
     def start_recording(self, rec_dir, prepend="", append=""):
-        cmd = "StartRecord RecDir={} PrependText={} AppendText={}".format(
-            rec_dir, prepend, append
-        )
+        cmd = f"StartRecord RecDir={rec_dir} PrependText={prepend} AppendText={append}"
         log.info("open-ephys: starting recording")
         self._send(cmd, "StartedRecording")
         rec_path = self._send("GetRecordingPath")
         log.info(" - recording path: %s", rec_path)
 
     def stop_recording(self):
         log.info("open-ephys: stopping recording")
```

### Comparing `open-ephys-audio-0.1.6/oeaudio/script.py` & `open_ephys_audio-0.1.7/oeaudio/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
 # -*- mode: python -*-
 """Presents acoustic stimuli for open-ephys experiments
 
 Stimuli are read from sound files (e.g. wave format) with 1 or 2 channels. The
 second channel is typically used as a synchronization signal. For one-channel
 files, by default a click is added to the second channel at the start of each
 stimulus.
 
 """
 
-import os
 import argparse
-import datetime
+import ctypes
+import json
 import logging
+import os
 import queue
 import threading
 import time
-import json
-import yaml
-import ctypes
+
 import sounddevice as sd
+import yaml
 
 from oeaudio import __version__
 
 log = logging.getLogger("oe-audio")  # root logger
 
 
 def setup_log(log, debug=False):
@@ -235,27 +234,28 @@
     def _process(outdata, frames, time, status):
         """Callback function for output stream thread"""
         assert frames == args.block_size, "frame count doesn't match buffer block size"
         if status.output_underflow:
             log.error("Output underflow: increase blocksize?")
             raise sd.CallbackAbort
         assert not status
+        # zero out the buffer to make sure there's nothing hanging around from last time
+        outdata[:] = b"\x00" * len(outdata)
         try:
             data = sample_queue.get_nowait()
             if data is None:
                 raise sd.CallbackStop
             elif isinstance(data, str):
                 controller.message(data)
             else:
                 assert len(data) <= len(outdata), "block has too much data"
                 outdata[: len(data)] = data
-                outdata[len(data) :] = b"\x00" * (len(outdata) - len(data))
         except queue.Empty:
-            # if the queue is empty, we just zero out the buffer
-            outdata[:] = b"\x00"
+            # if the queue is empty, we just leave the buffer empty
+            pass
 
     # The main thread sends data into the queue from files in the stimulus
     # queue. Between stimuli, it sends blocks of zeros. To stop the stream
     # thread, we send None.
 
     # We first need to prefill the queue so that the buffer starts full.
     stimiter = iter(stim_queue)
```

### Comparing `open-ephys-audio-0.1.6/setup.cfg` & `open_ephys_audio-0.1.7/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[bdist_wheel]
-universal = 1
-
 [pep8]
 ignore = E221,E501,E701
 
 [metadata]
 name = open-ephys-audio
 version = attr: oeaudio.__version__
 description = Scripts for acoustic stimulus presentation with open-ephys
 long_description = file: README.md
-keywords = one, two
+keywords = audio playback, neuroscience
 license = BSD 3-Clause License
 classifiers = 
 	License :: OSI Approved :: BSD License
-	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 author = Dan Meliza
 author_email = dan@meliza.org
 maintainer = Dan Meliza
 maintainer_email = dan@meliza.org
 url = https://github.com/melizalab/open-ephys-audio
 
 [options]
 zip_safe = false
 packages = oeaudio
 python_requires = >= 3.6
 setup_requires = 
-	setuptools >=38.3.0
+	setuptools >=58.1.0
 install_requires = 
+	numpy <2
 	sounddevice
 	pyzmq
 	soundfile
 	PyYAML
-	numpy
 
 [options.entry_points]
 console_scripts = 
 	oeaudio-present = oeaudio.script:main
 
 [options.packages.find]
 exclude = *test*
```

