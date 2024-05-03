# Comparing `tmp/picox-1.2.0.tar.gz` & `tmp/picox-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picox-1.2.0.tar", last modified: Tue Apr 30 20:47:52 2024, max compression
+gzip compressed data, was "picox-1.3.0.tar", last modified: Fri May  3 20:14:54 2024, max compression
```

## Comparing `picox-1.2.0.tar` & `picox-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.410638 picox-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 20:47:48.000000 picox-1.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-30 20:47:52.410638 picox-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-30 20:47:48.000000 picox-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 20:47:48.000000 picox-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:47:52.410638 picox-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.406638 picox-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.410638 picox-1.2.0/src/picox/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-30 20:47:48.000000 picox-1.2.0/src/picox/upy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:47:52.410638 picox-1.2.0/src/picox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 20:47:52.000000 picox-1.2.0/src/picox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.471385 picox-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 20:14:49.000000 picox-1.3.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-03 20:14:54.471385 picox-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-03 20:14:49.000000 picox-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:14:49.000000 picox-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:14:54.471385 picox-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.467384 picox-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.471385 picox-1.3.0/src/picox/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/upy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.471385 picox-1.3.0/src/picox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/top_level.txt
```

### Comparing `picox-1.2.0/LICENCE` & `picox-1.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `picox-1.2.0/PKG-INFO` & `picox-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picox
-Version: 1.2.0
+Version: 1.3.0
 Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
 Author: Harvey
 License: MIT License
         
         Copyright (c) 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,14 +88,19 @@
 ```
 
 ### View console output from already running pico
 ``` bash
 picox attach /dev/ttyUSB0
 ```
 
+### Soft reboot pico
+``` bash
+picox reboot /dev/ttyUSB0
+```
+
 ### Listing files on Pi Pico:
 ``` bash
 picox ls /dev/ttyUSB0
 
 # exmaple output:
 # demo.py
 # home.py
```

### Comparing `picox-1.2.0/README.md` & `picox-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 ```
 
 ### View console output from already running pico
 ``` bash
 picox attach /dev/ttyUSB0
 ```
 
+### Soft reboot pico
+``` bash
+picox reboot /dev/ttyUSB0
+```
+
 ### Listing files on Pi Pico:
 ``` bash
 picox ls /dev/ttyUSB0
 
 # exmaple output:
 # demo.py
 # home.py
```

### Comparing `picox-1.2.0/pyproject.toml` & `picox-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "picox"
-version = "1.2.0"
+version = "1.3.0"
 authors = [{name = "Harvey"}]
 description = "Tools for working with a Rasbperry Pi Pico running MicroPython"
 readme = "README.md"
 license = {file = "LICENCE"}
 dependencies = [
     "pyserial == 3.5",
     'pyreadline3 == 3.4.1 ; platform_system == "Windows"',
```

### Comparing `picox-1.2.0/src/picox/cli.py` & `picox-1.3.0/src/picox/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     repl_parser     = subparsers.add_parser("repl", help="Start REPL session on Pi Pico")
     ls_parser       = subparsers.add_parser("ls", help="Directory listing on Pi Pico")
     upload_parser   = subparsers.add_parser("upload", help="Upload a file")
     download_parser = subparsers.add_parser("download", help="Download a file")
     exec_parser     = subparsers.add_parser("exec", help="Execute a file")
     stop_parser     = subparsers.add_parser("stop", help="Send a stop to Pico")
     attach_parser   = subparsers.add_parser('attach', help="Attach to console output from Pico")
+    reboot_parser   = subparsers.add_parser('reboot', help="Soft reboot Pico")
 
     detect_parser.add_argument("--all", action="store_true", help="Detect all pico devices and return a list")
 
     repl_parser.add_argument("device", help="Serial device")
 
     ls_parser.add_argument("device", help="Serial device")
 
@@ -43,14 +44,16 @@
     exec_parser.add_argument("device", help="Serial device")
     exec_parser.add_argument("file", help="File to execute")
 
     stop_parser.add_argument("device", help="Serial device")
 
     attach_parser.add_argument('device', help="Serial device")
 
+    reboot_parser.add_argument("device", help="Serial device")
+
     # Re-parse with the remaining arguments
     args = parser.parse_args(remaining_argv, namespace=args)
     
     return args
 
 
 def main():
@@ -74,15 +77,15 @@
     match args.command:
         case "repl":
             pico.start_repl()
         case "ls":
             for file in pico.get_file_list():
                 print(file) # Print to stdout
         case "stop":
-            pass # Technically just opening it successfully will 
+            pass # Technically just opening it successfully will stop it
         case "upload":
             with open(args.read_file, "rb") as read_file:
                 pico.upload_file(read_file, args.file, overwrite=args.overwrite)
         case "download":
             with open(args.save_file, "w") as save_file:
                 pico.download_file(args.file, save_file)
         case "exec":
@@ -95,10 +98,12 @@
                 detected = get_first_pico_serial()
             print(detected) # show device to stdout
         case "attach":
             try:
                 pico.start_console_attach()
             except KeyboardInterrupt:
                 LOGGER.info("Received KeyboardInterrupt. Exiting...")
+        case "reboot":
+            pico.send_soft_reboot()
 
 if __name__ == "__main__":
     main()
```

### Comparing `picox-1.2.0/src/picox/detect.py` & `picox-1.3.0/src/picox/detect.py`

 * *Files identical despite different names*

### Comparing `picox-1.2.0/src/picox/logconfig.py` & `picox-1.3.0/src/picox/logconfig.py`

 * *Files identical despite different names*

### Comparing `picox-1.2.0/src/picox/upy.py` & `picox-1.3.0/src/picox/upy.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             raise RuntimeError(f"Did not get back a list from file listing command :: {string_list}")
         else:
             return ast.literal_eval(string_list) if string_list else []
 
     def stop_exec(self):
         """ Stop execution by a combinatino of reboot and Ctrl+C. Flushes buffers afterwards to get device in known state """
         self._send_stop_exec(quantity=5)
-        self._send_soft_reboot()
+        self.send_soft_reboot()
         time.sleep(0.2)
         self._send_stop_exec(quantity=5) # If there is an auto boot script, this will clear it
         time.sleep(0.2)
         self._send_enter()
         self._serial.reset_input_buffer()
         self._serial.reset_output_buffer()
 
@@ -208,15 +208,15 @@
         args:
             quantity (int) : How many Ctrl+C to send
         """
         LOGGER.debug("Sending stop exec (Ctrl+C) to Pico")
         for _ in range(quantity):
             self._serial_write(b'\x03')  # Ctrl+C -> stop execution
 
-    def _send_soft_reboot(self):
+    def send_soft_reboot(self):
         """ Send soft reboot command (Ctrl+D) """
         LOGGER.debug("Sending soft reboot to Pico (Ctrl+D)")
         self._serial_write(b'\x04')  # Ctrl+D -> Soft reboot if nothing executing and blank REPL
 
     def _send_enter(self):
         """ Send a blank enter to exit a block statement """
         self._serial_write(b'\r\n')
@@ -239,15 +239,14 @@
         file_data = self._communicate(
             f"exec(\"try:\\n  with open('{pico_filename}', 'r') as f: print(f.read(), end='')\\nexcept Exception as e: print(f'{download_failed_marker}{{str(e)}}')\")",
             is_block_command=True
         )
         if file_data.startswith(download_failed_marker):
             LOGGER.error(f"Upload was not successful: {file_data.replace(download_failed_marker, '')}")
         save_fp.write(file_data)
-        #TODO better exception handling...
 
     def upload_file(self, local_fp: IO[bytes], pico_file_path, overwrite=False):
         """ Upload a file from the host to the Pico """
         if pico_file_path in self.get_file_list():
             if not overwrite:
                 raise FileExistsError(f"File '{pico_file_path}' already exists on the Pico. Set overwrite=True to overwrite.")
             else:
```

### Comparing `picox-1.2.0/src/picox.egg-info/PKG-INFO` & `picox-1.3.0/src/picox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picox
-Version: 1.2.0
+Version: 1.3.0
 Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
 Author: Harvey
 License: MIT License
         
         Copyright (c) 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,14 +88,19 @@
 ```
 
 ### View console output from already running pico
 ``` bash
 picox attach /dev/ttyUSB0
 ```
 
+### Soft reboot pico
+``` bash
+picox reboot /dev/ttyUSB0
+```
+
 ### Listing files on Pi Pico:
 ``` bash
 picox ls /dev/ttyUSB0
 
 # exmaple output:
 # demo.py
 # home.py
```

