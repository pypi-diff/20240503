# Comparing `tmp/py2saber-0.12.2.tar.gz` & `tmp/py2saber-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.12.2.tar", last modified: Tue Apr  9 01:21:08 2024, max compression
+gzip compressed data, was "py2saber-0.13.tar", last modified: Fri May  3 18:50:38 2024, max compression
```

## Comparing `py2saber-0.12.2.tar` & `py2saber-0.13.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-04-09 01:21:08.048859 py2saber-0.12.2/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.12.2/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-04-09 01:21:08.048700 py2saber-0.12.2/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.12.2/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-04-09 01:21:08.048497 py2saber-0.12.2/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-04-09 01:21:08.000000 py2saber-0.12.2/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    26727 2024-04-08 21:02:56.000000 py2saber-0.12.2/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-03-22 23:21:26.000000 py2saber-0.12.2/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-04-09 01:21:08.048895 py2saber-0.12.2/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-03 18:50:38.635116 py2saber-0.13/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.13/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)    43209 2024-05-03 18:50:38.634920 py2saber-0.13/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.13/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-03 18:50:38.634731 py2saber-0.13/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43209 2024-05-03 18:50:38.000000 py2saber-0.13/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-03 18:50:38.000000 py2saber-0.13/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-03 18:50:38.000000 py2saber-0.13/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-03 18:50:38.000000 py2saber-0.13/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-03 18:50:38.000000 py2saber-0.13/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-03 18:50:38.000000 py2saber-0.13/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)    28662 2024-05-02 15:09:58.000000 py2saber-0.13/py2saber.py
+-rw-r--r--   0 jramboz    (501) staff       (20)      791 2024-05-03 18:50:30.000000 py2saber-0.13/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-03 18:50:38.635151 py2saber-0.13/setup.cfg
```

### Comparing `py2saber-0.12.2/COPYING` & `py2saber-0.13/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.12.2/PKG-INFO` & `py2saber-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.12.2
+Version: 0.13
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.12.2/README.md` & `py2saber-0.13/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.12.2/py2saber.egg-info/PKG-INFO` & `py2saber-0.13/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.12.2
+Version: 0.13
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.12.2/py2saber.py` & `py2saber-0.13/py2saber.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# py2saber Copyright © 2023 Jason Ramboz
+# py2saber Copyright © 2023-2024 Jason Ramboz
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.
 
@@ -22,24 +22,25 @@
 import sys
 import argparse
 import errno
 from getch import pause_exit
 import glob
 import time
 
-script_version = '0.12.2b'
+script_version = '0.13'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
-    def __init__(self, msg=None, detail="", *args, **kwargs):
+    def __init__(self, msg=None, *args, **kwargs):
+        if msg:
+            msg = self.__doc__ + '\n' + msg
         super().__init__(msg or self.__doc__, *args, **kwargs)
-        self.detail = detail
 
 # Custom Exceptions
 class NoAnimaSaberException(DocDefaultException):
     '''No compatible Anima found. If an Anima is connected, try restarting it with the on/off switch. If the problem persists, try a different USB cable.'''
 
 class AnimaNotReadyException(DocDefaultException):
     '''Anima is not ready to receive commands. Try restarting the Anima using the on/off switch.'''
@@ -49,14 +50,17 @@
 
 class AnimaFileWriteException(DocDefaultException):
     '''Error writing file(s) to Anima. Files are possibly corrupt. You should erase all files and re-upload.'''
 
 class InvalidSaberResponseException(DocDefaultException):
     '''Received invalid response from saber.'''
 
+class InvalidSoundEffectSpecifiedException(DocDefaultException):
+    '''Invalid sound effect specified.'''
+
 class Saber_Controller:
     '''Controls communication with an OpenCore-based lightsaber.'''
     # Serial port communication settings
     _SERIAL_SETTINGS = {'baudrate': 115200, 
                         'bytesize': 8, 
                         'parity': 'N', 
                         'stopbits': 1, 
@@ -66,19 +70,14 @@
                         'timeout': 3, 
                         'write_timeout': None, 
                         'inter_byte_timeout': None}
 
     def __init__(self, port: str=None, gui: bool = False, loglevel: int = logging.ERROR) -> None:
         self.log = logging.getLogger('Saber_Controller')
         self.log.setLevel(loglevel)
-        if not self.log.hasHandlers():
-            stream = logging.StreamHandler(sys.stdout)
-            #stream.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s: %(message)s'))
-            stream.setFormatter(logging.Formatter('%(levelname)s: %(message)s'))
-            self.log.addHandler(stream)
         self.log.info('Initializing saber connection.')
         self.gui = gui # Flag for whether to output signals for PySide GUI
         self.port = port
 
         # If a specific port is supplied, check that it is an OpenCore saber
         if self.port: 
             if not Saber_Controller.port_is_anima(port):
@@ -254,26 +253,24 @@
             info = {}
             
             # get firmware version
             cmd = b'V?'
             self.send_command(cmd)
             response = self.read_line()
             if not response or not response.startswith(b'V='):
-                self.log.error(f'Invalid response received.\nCommand: {cmd}\nResponse: {response}')
-                raise InvalidSaberResponseException
+                raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
             else:
                 info['version'] = response.decode().strip()[2:]
 
             # get serial number
             cmd = b'S?'
             self.send_command(cmd)
             response = self.read_line()
             if not response or not response.startswith(b'S='):
-                self.log.error(f'Invalid response received.\nCommand: {cmd}\nResponse: {response}')
-                raise InvalidSaberResponseException
+                raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
             else:
                 info['serial'] = response.decode().strip()[2:]
             
             self.log.info(f'Found saber info: {info}')
             return info
         else:
             raise AnimaNotReadyException
@@ -340,14 +337,36 @@
         cmd = b'FREE?'
         self.send_command(cmd)
         response = self.read_line()
         r = response.decode().strip()
         free_space = int(r[5:])
         self.log.info(f'Free space: {free_space} bytes')
         return free_space
+    
+    def get_used_space(self) -> int:
+        '''Returns the amount of used space in Anima storage in bytes.'''
+        self.log.info('Getting used space on Anima.')
+        cmd = b'USED?'
+        self.send_command(cmd)
+        response = self.read_line()
+        r = response.decode().strip()
+        used_space = int(r[5:])
+        self.log.info(f'Used space: {used_space} bytes')
+        return used_space
+    
+    def get_total_space(self) -> int:
+        '''Returns the amount of total storage space in Anima storage in bytes.'''
+        self.log.info('Getting total storage space on Anima.')
+        cmd = b'SIZE?'
+        self.send_command(cmd)
+        response = self.read_line()
+        r = response.decode().strip()
+        total_space = int(r[5:])
+        self.log.info(f'Total space: {total_space} bytes')
+        return total_space
 
     def read_config_ini(self) -> str:
         '''Read the config.ini file from saber and return as a string'''
         self.log.info('Reading config.ini from saber')
         cmd = b'RD?config.ini\n'
         self.send_command(cmd)
         # Anima doesn't seem to properly sent STX/ETX bytes. Instead just sends '2' and '3'
@@ -370,16 +389,15 @@
             self.log.info(f'Writing file to saber: {file}')
             
             # Check for enough free space
             file_size = os.path.getsize(file)
             self.log.debug(f'File size: {file_size}')
             free_space = self.get_free_space()
             if free_space < file_size:
-                self.log.error(f'Not enough free space on saber for file {file}')
-                raise NotEnoughFreeSpaceException
+                raise NotEnoughFreeSpaceException(f'File: {file}')
 
             # Write the file
             with open(file, mode='rb') as binary_file:
                 if self.saber_is_ready():
                     bytes_sent = 0
                     fname = os.path.basename(file)
                     report_every_n_bytes = 512 # How often to update the bytes sent display
@@ -403,31 +421,29 @@
                                 progress_callback.emit(bytes_sent)
                     print(f'\r{fname} - Bytes sent: {bytes_sent} - Bytes remaining: {file_size - bytes_sent}     ')
                 else:
                     raise AnimaNotReadyException
             
             response = self.read_line()
             if not response == b'OK, Write Complete\n':
-                self.log.error(f'Error writing file to saber. Error message: {response}')
-                raise AnimaFileWriteException
+                raise AnimaFileWriteException(f'Error message: {response}')
         
             self.log.info(f'Successfully wrote file to saber: {file}')
             time.sleep(1)
 
     @staticmethod
     def rgbw_to_byte_str(r: int, g: int, b:int, w: int):
         return bytes(str(r), 'ascii') + b',' + bytes(str(g), 'ascii') + b',' + bytes(str(b), 'ascii') + b','+ bytes(str(w), 'ascii')
 
     def preview_color(self, r: int, g: int, b: int, w: int):
         cmd = b'P=' + self.rgbw_to_byte_str(r, g, b, w) + b'\n'
         self.send_command(cmd)
         response = self.read_line()
         if response[:2] != b'OK':
-            self.log.error(f'Invalid response received.\nCommand: {cmd}\nResponse: {response}')
-            raise InvalidSaberResponseException
+            raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
     
     def set_color(self, bank: int, effect: str, r: int, g: int, b: int, w:int):
         '''Writes a color setting to the saber. 
         bank specifies which bank (0-7). 
         effect is one of "color", "clash", or "swing". 
         RGBW values are 0-255'''
         match effect:
@@ -441,38 +457,73 @@
                 self.log.error(f'Invalid effect type specified: {effect}')
                 return
         
         cmd = cmd + bytes(str(bank),'ascii') + b'=' + self.rgbw_to_byte_str(r, g, b, w) + b'\n'
         self.send_command(cmd)
         response = self.read_line()
         if response[:2] != b'OK':
-            self.log.error(f'Invalid response received.\nCommand: {cmd}\nResponse: {response}')
-            raise InvalidSaberResponseException
+            raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
     
     def set_active_bank(self, bank:int):
         '''Sets the active bank (0-7)'''
         cmd = b'B=' + bytes(str(bank), 'ascii') + b'\n'
         self.send_command(cmd)
         response = self.read_line()
         if response[:2] != b'OK':
-            self.log.error(f'Invalid response received.\nCommand: {cmd}\nResponse: {response}')
-            raise InvalidSaberResponseException
+            raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
     
+    @staticmethod
+    def _get_cmd_for_sound_effect(effect: str) -> bytes:
+        '''returns the command header for the given sound effect. Calling function needs to either add '?' or '=' to the end.'''
+        match effect:
+            case 'on':
+                return b'sON'
+            case 'off':
+                return b'sOFF'
+            case 'hum':
+                return b'sHUM'
+            case 'swing':
+                return b'sSW'
+            case 'clash':
+                return b'sCL'
+            case 'smoothSwingA':
+                return b'sSMA'
+            case 'smoothSwingB':
+                return b'sSMB'
+            case _:
+                raise InvalidSoundEffectSpecifiedException(f'Specified effect: {effect}')
+
+    def set_sounds_for_effect(self, effect: str, files: list[str]):
+        '''Sets the sound list for a given effect.'''
+        self.log.debug(f'Setting sound files {str(files)} for effect "{effect}".')
+        cmd = self._get_cmd_for_sound_effect(effect) + b'=' + ','.join(files).encode('utf-8')
+        self.send_command(cmd)
+        response = self.read_line()
+        if response != b'OK ' + cmd + b'\n':
+            raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
+
+    def get_sounds_for_effect(self, effect: str) -> list[str]:
+        '''Returns a list of filenames Anima is using for the specified effect.'''
+        self.log.debug(f'Retrieving list of sound files for effect "{effect}".')
+        cmd = self._get_cmd_for_sound_effect(effect) + b'?'
+        self.send_command(cmd)
+        response = self.read_line()
+        r = response.split(b'=')
+        if r[0] != self._get_cmd_for_sound_effect(effect):
+            raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
+        return r[1].decode().strip().split(',')
+
 # ---------------------------------------------------------------------- #
 # Command Line Operations                                                #
 # ---------------------------------------------------------------------- #
 
 def error_handler(e: DocDefaultException):
-    '''Print an exception to the log, with details if provided in Exception'''
+    '''Print an exception to the log.'''
     log = logging.getLogger()
     log.debug(e, exc_info=True)
-    if e.detail:
-        log.error(str(e) + '\nDetails: ' + e.detail)
-    else:
-        log.error(e)
 
 def main_func():
     log = logging.getLogger()
 
     exit_code = 0
 
     # configure command line parser and options
```

### Comparing `py2saber-0.12.2/pyproject.toml` & `py2saber-0.13/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.12.2"
+version = "0.13"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

