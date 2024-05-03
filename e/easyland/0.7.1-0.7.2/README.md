# Comparing `tmp/easyland-0.7.1.tar.gz` & `tmp/easyland-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyland-0.7.1.tar", last modified: Thu May  2 09:46:05 2024, max compression
+gzip compressed data, was "easyland-0.7.2.tar", last modified: Fri May  3 09:08:32 2024, max compression
```

## Comparing `easyland-0.7.1.tar` & `easyland-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.306784 easyland-0.7.1/
--rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.1/LICENSE.txt
--rw-r--r--   0 ju        (1000) ju        (1000)    13317 2024-05-02 09:46:05.306784 easyland-0.7.1/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)    12446 2024-05-01 21:56:58.000000 easyland-0.7.1/README.md
--rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-01 21:54:38.000000 easyland-0.7.1/pyproject.toml
--rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-02 09:46:05.306784 easyland-0.7.1/setup.cfg
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.303451 easyland-0.7.1/src/
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.306784 easyland-0.7.1/src/easyland/
--rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.1/src/easyland/__init__.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-01 17:31:04.000000 easyland-0.7.1/src/easyland/command.py
--rw-r--r--   0 ju        (1000) ju        (1000)     4656 2024-05-01 20:22:29.000000 easyland-0.7.1/src/easyland/daemon.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2229 2024-05-01 20:26:14.000000 easyland-0.7.1/src/easyland/idle.py
--rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.1/src/easyland/log.py
--rwxr-xr-x   0 ju        (1000) ju        (1000)     1245 2024-05-01 21:54:48.000000 easyland-0.7.1/src/easyland/main.py
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.306784 easyland-0.7.1/src/easyland.egg-info/
--rw-r--r--   0 ju        (1000) ju        (1000)    13317 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/SOURCES.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/dependency_links.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/entry_points.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/requires.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/top_level.txt
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.276980 easyland-0.7.2/
+-rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.2/LICENSE.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-03 09:08:32.276980 easyland-0.7.2/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)    13475 2024-05-03 08:13:49.000000 easyland-0.7.2/README.md
+-rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-02 15:06:34.000000 easyland-0.7.2/pyproject.toml
+-rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-03 09:08:32.276980 easyland-0.7.2/setup.cfg
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.273646 easyland-0.7.2/src/
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.276980 easyland-0.7.2/src/easyland/
+-rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.2/src/easyland/__init__.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-01 17:31:04.000000 easyland-0.7.2/src/easyland/command.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     4904 2024-05-03 07:32:12.000000 easyland-0.7.2/src/easyland/daemon.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2229 2024-05-01 20:26:14.000000 easyland-0.7.2/src/easyland/idle.py
+-rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.2/src/easyland/log.py
+-rwxr-xr-x   0 ju        (1000) ju        (1000)     1245 2024-05-02 15:06:52.000000 easyland-0.7.2/src/easyland/main.py
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-03 09:08:32.276980 easyland-0.7.2/src/easyland.egg-info/
+-rw-r--r--   0 ju        (1000) ju        (1000)    14346 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/SOURCES.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/dependency_links.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/entry_points.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/requires.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-03 09:08:32.000000 easyland-0.7.2/src/easyland.egg-info/top_level.txt
```

### Comparing `easyland-0.7.1/LICENSE.txt` & `easyland-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyland-0.7.1/PKG-INFO` & `easyland-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyland
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python swiss-knife to manage wayand compositors like Hyprland and Sway
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/easyland
 Project-URL: Issues, https://github.com/juienpro/easyland/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,29 @@
 
 To give an example, my laptop screen brightness was always at 100% when I undock it, and Kanshi does not allow to add shell commands. This is only one small example of the numerous limitations I met during my setup of Hyprland.
 
 By scripting my Desktop in Python, I have more control to implement what I want.
 
 ## Installation
 
+1. Install Easyland in a python environment
+
+```
+pip3 -i easyland
+```
+
+2. Copy an example of configuration files from [here](https://github.com/juienpro/easyland/tree/main/config_examples)
+
+3. Modify it according to your needs
+
+4. Launch `easyland -c <path_to_your_config_file`
+
+
 This program needs the following external tools: 
+
 - The `socat` binary ([Arch](https://archlinux.org/packages/extra/x86_64/socat/))
 - The `gdbus` binary ([Arch](https://archlinux.org/packages/core/x86_64/glib2/))
 
 
 Depending if you use Hyprland or Sway, you will need `hyprctl` or `swaymsg`.
 
 If it's not done automatically, before using PyWayland, you will need to execute `pywayland.scanner` to generate all protocols:
@@ -79,15 +93,23 @@
 ```
 from easyland import logger, command
 
 ###############################################################################
 # Set active listeners
 ###############################################################################
 
-listeners = ['hyprland', 'systemd_logind', 'idle']
+listeners = {
+    "hyprland": { "socket_path": "/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock" },
+    'systemd_logind': {},
+    'idle': {}
+}
+
+###############################################################################
+# Method executed at start 
+###############################################################################
 
 def init():
     set_monitors()
 
 ###############################################################################
 # Idle configuration
 # Format: [timeout in seconds, [commands to run], [commands to run on resume]]
@@ -107,15 +129,15 @@
 
 def on_hyprland_event(event, argument):
     if event in [ "monitoradded", "monitorremoved" ]:
         logger.info('Handling hyprland event: ' + event)
         set_monitors()
 
 ###############################################################################
-# Handlers of Systemd logind eventz
+# Handlers of Systemd logind events
 ###############################################################################
 
 def on_PrepareForSleep(payload):
     if 'true' in payload:
         logger.info("Locking the screen before suspend")
         command.exec("pidof hyprlock || hyprlock", True)
 
@@ -153,22 +175,27 @@
 ```
 
 Easyland has helper tools to log everything (console and file) and execute commands. Just import the two. 
 
 #### Configure listeners
 
 ```
-listeners = ['hyprland', 'systemd_logind', 'idle']
+listeners = {
+    "hyprland": { "socket_path": "/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock" },
+    'systemd_logind': {},
+    'idle': {}
+}
 ```
 
 The listeners to launch at the startup. There are currently three listeners: 
 - `hyprland` to listen Hyprland IPC events
 - `systemd_logind` to monitor for Systemd Logind events
 - `idle` which allows you to react when your computer has no activity
 
+Each one can take take on or more parameters. See reference below.
 
 #### Configure Idling
 
 ```
 def idle_config():
     return [
         [150, ['brightnessctl -s set 0'], ['brightnessctl -r']],
@@ -232,40 +259,58 @@
 
 ```
 # To use this handler, you need to launch your locker (hyprlock or swaylock) like this: hyprlock && loginctl unlock-session
 def on_Unlock():
     logger.info("Unlocking the screen")
 ```
 
-To receive the Systemd `Unlock` signal, you should launch your screen locker with the following command: `hyprlock && loginctl unlock-session`, so Systemd will launch the `Unlock` signal when the screen is unlocked.
+To receive the Systemd `Unlock` signal, you should launch your screen locker with the following command: `hyprlock && loginctl unlock-session`, so Systemd will send the `Unlock` signal when the screen is unlocked.
 
 For locking, keep in mind that `hyprlock` and `swaylock` do not listen for the Systemd `Lock` event, so you need to it manually. 
 
 ```
 # To use this handler, you need to launch your locker like this: loginctl lock-session
 def on_Lock():
      logger.info("Locking the screen")
      command.exec('pidof hyprlock || hyprlock', True)
      # Do other actions if needed
 ```
 
 #### Alternative to on_WhateverSignal method
 
-Alternatively to write several methods to listen for Systemd events, you can also define method `on_systemd_event` and test the signal to achieve what you want:
+Alternatively to write several methods to listen for Systemd events, you can also define method `on_systemd_event` and add a condition to achieve what you want:
 
 ```
 def on_systemd_event(sender, signal, payload)
     if signal == 'Lock':
         ...
     if signal == 'PrepareForSleep':
         ...
 ```
 
 ## References
 
+### Listeners parameters
+
+#### Hyprland listener parameters
+
+- `socket_path`: The path of the Hyprland IPC socket
+
+#### Sway listener parameters
+
+- `event_types`: The type of events to be listened for
+
+#### Idle listener parameters
+
+None.
+
+#### systemd_logind parameters
+
+None.
+
 ### Listeners handler methods
 
 
 | Sender            | Handler method to add to your class | Arguments                               |
 |-------------------|-------------------------------------|---------------------------------------- |
 | Hyprland          | on_hyprland_event                   | event, argument                        |
 | Sway              | on_sway_event_[type]                   | payload                        |
@@ -310,16 +355,16 @@
 | command.sway_get_monitor | Get the config of one monitor, None if not found | name, make, model |
 | logger | Log messages to easyland.log and to STDOUT | use logger.info, logger.error, for the severity etc. |
 | idle_config | Set the idle configuration | None
 
 
 ## Contributions
 
-- Integrating other DBUS services should be easy with Easyland (type `dbusctl` to list all avalable DBUS on your system). Do not hesitate to let know what you need.
-- Better tests for Sway. I use Hyprland so feel free to submit bugs if you are using Sway
+- Integrating other DBUS services should be easy with Easyland (type `dbusctl` to list all avalable DBUS on your system). Do not hesitate to let me know what you need.
+- Better tests for Sway. I use Hyprland so feel free to submit bugs if you are using Sway and see an issue.
 
 If you see some bugs or propose patches, feel free to contribute.
 
 
 ## Thanks
 
 Thanks to the developer(s) of [Hyprland](https://hyprland.org) for their fantastic compositor. I tried so many ones in the past, and this has been Hyprland that convinced me to do the switch from KDE :-)
```

### Comparing `easyland-0.7.1/README.md` & `easyland-0.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,29 @@
 
 To give an example, my laptop screen brightness was always at 100% when I undock it, and Kanshi does not allow to add shell commands. This is only one small example of the numerous limitations I met during my setup of Hyprland.
 
 By scripting my Desktop in Python, I have more control to implement what I want.
 
 ## Installation
 
+1. Install Easyland in a python environment
+
+```
+pip3 -i easyland
+```
+
+2. Copy an example of configuration files from [here](https://github.com/juienpro/easyland/tree/main/config_examples)
+
+3. Modify it according to your needs
+
+4. Launch `easyland -c <path_to_your_config_file`
+
+
 This program needs the following external tools: 
+
 - The `socat` binary ([Arch](https://archlinux.org/packages/extra/x86_64/socat/))
 - The `gdbus` binary ([Arch](https://archlinux.org/packages/core/x86_64/glib2/))
 
 
 Depending if you use Hyprland or Sway, you will need `hyprctl` or `swaymsg`.
 
 If it's not done automatically, before using PyWayland, you will need to execute `pywayland.scanner` to generate all protocols:
@@ -58,15 +72,23 @@
 ```
 from easyland import logger, command
 
 ###############################################################################
 # Set active listeners
 ###############################################################################
 
-listeners = ['hyprland', 'systemd_logind', 'idle']
+listeners = {
+    "hyprland": { "socket_path": "/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock" },
+    'systemd_logind': {},
+    'idle': {}
+}
+
+###############################################################################
+# Method executed at start 
+###############################################################################
 
 def init():
     set_monitors()
 
 ###############################################################################
 # Idle configuration
 # Format: [timeout in seconds, [commands to run], [commands to run on resume]]
@@ -86,15 +108,15 @@
 
 def on_hyprland_event(event, argument):
     if event in [ "monitoradded", "monitorremoved" ]:
         logger.info('Handling hyprland event: ' + event)
         set_monitors()
 
 ###############################################################################
-# Handlers of Systemd logind eventz
+# Handlers of Systemd logind events
 ###############################################################################
 
 def on_PrepareForSleep(payload):
     if 'true' in payload:
         logger.info("Locking the screen before suspend")
         command.exec("pidof hyprlock || hyprlock", True)
 
@@ -132,22 +154,27 @@
 ```
 
 Easyland has helper tools to log everything (console and file) and execute commands. Just import the two. 
 
 #### Configure listeners
 
 ```
-listeners = ['hyprland', 'systemd_logind', 'idle']
+listeners = {
+    "hyprland": { "socket_path": "/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock" },
+    'systemd_logind': {},
+    'idle': {}
+}
 ```
 
 The listeners to launch at the startup. There are currently three listeners: 
 - `hyprland` to listen Hyprland IPC events
 - `systemd_logind` to monitor for Systemd Logind events
 - `idle` which allows you to react when your computer has no activity
 
+Each one can take take on or more parameters. See reference below.
 
 #### Configure Idling
 
 ```
 def idle_config():
     return [
         [150, ['brightnessctl -s set 0'], ['brightnessctl -r']],
@@ -211,40 +238,58 @@
 
 ```
 # To use this handler, you need to launch your locker (hyprlock or swaylock) like this: hyprlock && loginctl unlock-session
 def on_Unlock():
     logger.info("Unlocking the screen")
 ```
 
-To receive the Systemd `Unlock` signal, you should launch your screen locker with the following command: `hyprlock && loginctl unlock-session`, so Systemd will launch the `Unlock` signal when the screen is unlocked.
+To receive the Systemd `Unlock` signal, you should launch your screen locker with the following command: `hyprlock && loginctl unlock-session`, so Systemd will send the `Unlock` signal when the screen is unlocked.
 
 For locking, keep in mind that `hyprlock` and `swaylock` do not listen for the Systemd `Lock` event, so you need to it manually. 
 
 ```
 # To use this handler, you need to launch your locker like this: loginctl lock-session
 def on_Lock():
      logger.info("Locking the screen")
      command.exec('pidof hyprlock || hyprlock', True)
      # Do other actions if needed
 ```
 
 #### Alternative to on_WhateverSignal method
 
-Alternatively to write several methods to listen for Systemd events, you can also define method `on_systemd_event` and test the signal to achieve what you want:
+Alternatively to write several methods to listen for Systemd events, you can also define method `on_systemd_event` and add a condition to achieve what you want:
 
 ```
 def on_systemd_event(sender, signal, payload)
     if signal == 'Lock':
         ...
     if signal == 'PrepareForSleep':
         ...
 ```
 
 ## References
 
+### Listeners parameters
+
+#### Hyprland listener parameters
+
+- `socket_path`: The path of the Hyprland IPC socket
+
+#### Sway listener parameters
+
+- `event_types`: The type of events to be listened for
+
+#### Idle listener parameters
+
+None.
+
+#### systemd_logind parameters
+
+None.
+
 ### Listeners handler methods
 
 
 | Sender            | Handler method to add to your class | Arguments                               |
 |-------------------|-------------------------------------|---------------------------------------- |
 | Hyprland          | on_hyprland_event                   | event, argument                        |
 | Sway              | on_sway_event_[type]                   | payload                        |
@@ -289,16 +334,16 @@
 | command.sway_get_monitor | Get the config of one monitor, None if not found | name, make, model |
 | logger | Log messages to easyland.log and to STDOUT | use logger.info, logger.error, for the severity etc. |
 | idle_config | Set the idle configuration | None
 
 
 ## Contributions
 
-- Integrating other DBUS services should be easy with Easyland (type `dbusctl` to list all avalable DBUS on your system). Do not hesitate to let know what you need.
-- Better tests for Sway. I use Hyprland so feel free to submit bugs if you are using Sway
+- Integrating other DBUS services should be easy with Easyland (type `dbusctl` to list all avalable DBUS on your system). Do not hesitate to let me know what you need.
+- Better tests for Sway. I use Hyprland so feel free to submit bugs if you are using Sway and see an issue.
 
 If you see some bugs or propose patches, feel free to contribute.
 
 
 ## Thanks
 
 Thanks to the developer(s) of [Hyprland](https://hyprland.org) for their fantastic compositor. I tried so many ones in the past, and this has been Hyprland that convinced me to do the switch from KDE :-)
```

### Comparing `easyland-0.7.1/pyproject.toml` & `easyland-0.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "easyland"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
     { name="Julien Pro", email="contact@julienpro.com"}
 ]
 description = "A python swiss-knife to manage wayand compositors like Hyprland and Sway"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `easyland-0.7.1/src/easyland/command.py` & `easyland-0.7.2/src/easyland/command.py`

 * *Files identical despite different names*

### Comparing `easyland-0.7.1/src/easyland/daemon.py` & `easyland-0.7.2/src/easyland/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,42 +7,44 @@
 from easyland.log import logger
 from easyland.idle import Idle
 
 class Daemon():
 
     def __init__(self, config):
         self.config = config 
-        listeners = self.get_listeners()
+        self.listeners = self.get_listeners()
+        listener_names = self.listeners.keys()
+
         logger.info('Starting easyland daemon')
 
-        if 'hyprland' in listeners:
+        if 'hyprland' in listener_names:
             hyprland_thread = threading.Thread(target=self.launch_hyprland_daemon)
             hyprland_thread.daemon = True
             hyprland_thread.start()
 
-        if 'sway' in listeners: 
-            if not hasattr(self.config, 'sway_event_types'):
+        if 'sway' in listener_names: 
+            if not 'event_types' in self.listeners['sway']:
                 logger.error('No sway event types defined for Sway listeners in the config file')
                 sys.exit(1)
             existing_types = ['workspace', 'window', 'output', 'mode', 'barconfig_update', 'binding', 'shutdown', 'tick', 'bar_state_update', 'input']
-            sway_threads = [None] * len(self.config.sway_event_types)
-            for idx, event_type in enumerate(self.config.sway_event_types):
+            sway_threads = [None] * len(self.listeners['sway']['event_types'])
+            for idx, event_type in enumerate(self.listeners['sway']['event_types']):
                 if event_type not in existing_types:
                     logger.error('Sway - Invalid event type: ' + event_type)
                     sys.exit(1)
                 sway_threads[idx] = threading.Thread(target=self.launch_sway_daemon, args=(event_type,)) 
                 sway_threads[idx].daemon = True
                 sway_threads[idx].start()
 
-        if 'systemd_logind' in listeners:
+        if 'systemd_logind' in listener_names:
             systemd_thread = threading.Thread(target=self.launch_systemd_login_daemon)
             systemd_thread.daemon = True
             systemd_thread.start()
 
-        if 'idle' in listeners:
+        if 'idle' in listener_names:
             if callable(getattr(self.config, 'idle_config', None)):
                 idle_thread = threading.Thread(target=self.launch_idle_daemon)
                 idle_thread.daemon = True
                 idle_thread.start()
 
         self.call_handler('init')
 
@@ -62,15 +64,16 @@
     def launch_idle_daemon(self):
         idle_config = self.config.idle_config()
         idle = Idle(idle_config)
         idle.setup()
 
     def launch_hyprland_daemon(self):
         logger.info('Launching hyprland daemon')
-        cmd = "socat -U - UNIX-CONNECT:/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock"
+        socket = self.listeners['hyprland'].get('socket_path', '/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock')
+        cmd = "socat -U - UNIX-CONNECT:"+socket
         ps = subprocess.Popen(cmd,shell=True,stdout=subprocess.PIPE,stderr=subprocess.STDOUT)
         while True:
             for line in iter(ps.stdout.readline, ""):
                 self.last_event_time = time.time()
                 decoded_line = line.decode("utf-8")
                 if '>>' in decoded_line:
                     data = decoded_line.split('>>')
@@ -84,14 +87,16 @@
             for line in iter(ps.stdout.readline, ""):
                 decoded_line = line.decode("utf-8").strip()
                 try:
                     json_output = json.loads(decoded_line)
                     self.call_handler('on_sway_event_' + event_type, json_output)
                 except json.decoder.JSONDecodeError:
                     logger.error('Sway daemon: Invalid JSON: '+ decoded_line)
+                    logger.error('Sway daemon: Exiting')
+                    return
 
     def launch_systemd_login_daemon(self):
         logger.info('Launching systemd daemon')
         cmd = "gdbus monitor --system --dest org.freedesktop.login1"
         ps = subprocess.Popen(cmd,shell=True,stdout=subprocess.PIPE,stderr=subprocess.STDOUT)
         while True:
             for line in iter(ps.stdout.readline, ""):
```

### Comparing `easyland-0.7.1/src/easyland/idle.py` & `easyland-0.7.2/src/easyland/idle.py`

 * *Files identical despite different names*

### Comparing `easyland-0.7.1/src/easyland/main.py` & `easyland-0.7.2/src/easyland/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib.util
 import importlib.machinery
 import sys
 import time
 import os
 from easyland.daemon import Daemon
 
-version = '0.7.1'
+version = '0.7.2'
 
 def import_from_path(path):
     module_name = os.path.basename(path).replace('-', '_').replace('.py', '')
     spec = importlib.util.spec_from_loader(module_name, importlib.machinery.SourceFileLoader(module_name, path))
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     sys.modules[module_name] = module
```

### Comparing `easyland-0.7.1/src/easyland.egg-info/PKG-INFO` & `easyland-0.7.2/src/easyland.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyland
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python swiss-knife to manage wayand compositors like Hyprland and Sway
 Author-email: Julien Pro <contact@julienpro.com>
 Project-URL: Homepage, https://github.com/juienpro/easyland
 Project-URL: Issues, https://github.com/juienpro/easyland/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,29 @@
 
 To give an example, my laptop screen brightness was always at 100% when I undock it, and Kanshi does not allow to add shell commands. This is only one small example of the numerous limitations I met during my setup of Hyprland.
 
 By scripting my Desktop in Python, I have more control to implement what I want.
 
 ## Installation
 
+1. Install Easyland in a python environment
+
+```
+pip3 -i easyland
+```
+
+2. Copy an example of configuration files from [here](https://github.com/juienpro/easyland/tree/main/config_examples)
+
+3. Modify it according to your needs
+
+4. Launch `easyland -c <path_to_your_config_file`
+
+
 This program needs the following external tools: 
+
 - The `socat` binary ([Arch](https://archlinux.org/packages/extra/x86_64/socat/))
 - The `gdbus` binary ([Arch](https://archlinux.org/packages/core/x86_64/glib2/))
 
 
 Depending if you use Hyprland or Sway, you will need `hyprctl` or `swaymsg`.
 
 If it's not done automatically, before using PyWayland, you will need to execute `pywayland.scanner` to generate all protocols:
@@ -79,15 +93,23 @@
 ```
 from easyland import logger, command
 
 ###############################################################################
 # Set active listeners
 ###############################################################################
 
-listeners = ['hyprland', 'systemd_logind', 'idle']
+listeners = {
+    "hyprland": { "socket_path": "/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock" },
+    'systemd_logind': {},
+    'idle': {}
+}
+
+###############################################################################
+# Method executed at start 
+###############################################################################
 
 def init():
     set_monitors()
 
 ###############################################################################
 # Idle configuration
 # Format: [timeout in seconds, [commands to run], [commands to run on resume]]
@@ -107,15 +129,15 @@
 
 def on_hyprland_event(event, argument):
     if event in [ "monitoradded", "monitorremoved" ]:
         logger.info('Handling hyprland event: ' + event)
         set_monitors()
 
 ###############################################################################
-# Handlers of Systemd logind eventz
+# Handlers of Systemd logind events
 ###############################################################################
 
 def on_PrepareForSleep(payload):
     if 'true' in payload:
         logger.info("Locking the screen before suspend")
         command.exec("pidof hyprlock || hyprlock", True)
 
@@ -153,22 +175,27 @@
 ```
 
 Easyland has helper tools to log everything (console and file) and execute commands. Just import the two. 
 
 #### Configure listeners
 
 ```
-listeners = ['hyprland', 'systemd_logind', 'idle']
+listeners = {
+    "hyprland": { "socket_path": "/tmp/hypr/$HYPRLAND_INSTANCE_SIGNATURE/.socket2.sock" },
+    'systemd_logind': {},
+    'idle': {}
+}
 ```
 
 The listeners to launch at the startup. There are currently three listeners: 
 - `hyprland` to listen Hyprland IPC events
 - `systemd_logind` to monitor for Systemd Logind events
 - `idle` which allows you to react when your computer has no activity
 
+Each one can take take on or more parameters. See reference below.
 
 #### Configure Idling
 
 ```
 def idle_config():
     return [
         [150, ['brightnessctl -s set 0'], ['brightnessctl -r']],
@@ -232,40 +259,58 @@
 
 ```
 # To use this handler, you need to launch your locker (hyprlock or swaylock) like this: hyprlock && loginctl unlock-session
 def on_Unlock():
     logger.info("Unlocking the screen")
 ```
 
-To receive the Systemd `Unlock` signal, you should launch your screen locker with the following command: `hyprlock && loginctl unlock-session`, so Systemd will launch the `Unlock` signal when the screen is unlocked.
+To receive the Systemd `Unlock` signal, you should launch your screen locker with the following command: `hyprlock && loginctl unlock-session`, so Systemd will send the `Unlock` signal when the screen is unlocked.
 
 For locking, keep in mind that `hyprlock` and `swaylock` do not listen for the Systemd `Lock` event, so you need to it manually. 
 
 ```
 # To use this handler, you need to launch your locker like this: loginctl lock-session
 def on_Lock():
      logger.info("Locking the screen")
      command.exec('pidof hyprlock || hyprlock', True)
      # Do other actions if needed
 ```
 
 #### Alternative to on_WhateverSignal method
 
-Alternatively to write several methods to listen for Systemd events, you can also define method `on_systemd_event` and test the signal to achieve what you want:
+Alternatively to write several methods to listen for Systemd events, you can also define method `on_systemd_event` and add a condition to achieve what you want:
 
 ```
 def on_systemd_event(sender, signal, payload)
     if signal == 'Lock':
         ...
     if signal == 'PrepareForSleep':
         ...
 ```
 
 ## References
 
+### Listeners parameters
+
+#### Hyprland listener parameters
+
+- `socket_path`: The path of the Hyprland IPC socket
+
+#### Sway listener parameters
+
+- `event_types`: The type of events to be listened for
+
+#### Idle listener parameters
+
+None.
+
+#### systemd_logind parameters
+
+None.
+
 ### Listeners handler methods
 
 
 | Sender            | Handler method to add to your class | Arguments                               |
 |-------------------|-------------------------------------|---------------------------------------- |
 | Hyprland          | on_hyprland_event                   | event, argument                        |
 | Sway              | on_sway_event_[type]                   | payload                        |
@@ -310,16 +355,16 @@
 | command.sway_get_monitor | Get the config of one monitor, None if not found | name, make, model |
 | logger | Log messages to easyland.log and to STDOUT | use logger.info, logger.error, for the severity etc. |
 | idle_config | Set the idle configuration | None
 
 
 ## Contributions
 
-- Integrating other DBUS services should be easy with Easyland (type `dbusctl` to list all avalable DBUS on your system). Do not hesitate to let know what you need.
-- Better tests for Sway. I use Hyprland so feel free to submit bugs if you are using Sway
+- Integrating other DBUS services should be easy with Easyland (type `dbusctl` to list all avalable DBUS on your system). Do not hesitate to let me know what you need.
+- Better tests for Sway. I use Hyprland so feel free to submit bugs if you are using Sway and see an issue.
 
 If you see some bugs or propose patches, feel free to contribute.
 
 
 ## Thanks
 
 Thanks to the developer(s) of [Hyprland](https://hyprland.org) for their fantastic compositor. I tried so many ones in the past, and this has been Hyprland that convinced me to do the switch from KDE :-)
```

