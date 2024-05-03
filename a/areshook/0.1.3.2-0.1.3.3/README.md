# Comparing `tmp/areshook-0.1.3.2.tar.gz` & `tmp/areshook-0.1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "areshook-0.1.3.2.tar", last modified: Sun Apr 28 08:26:40 2024, max compression
+gzip compressed data, was "areshook-0.1.3.3.tar", last modified: Fri May  3 15:39:08 2024, max compression
```

## Comparing `areshook-0.1.3.2.tar` & `areshook-0.1.3.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:26:40.990585 areshook-0.1.3.2/
--rw-rw-r--   0 mark      (1000) mark      (1000)       64 2024-04-23 06:07:42.000000 areshook-0.1.3.2/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      634 2024-04-28 08:26:40.990585 areshook-0.1.3.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      257 2024-04-19 09:23:58.000000 areshook-0.1.3.2/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-19 09:23:58.000000 areshook-0.1.3.2/README.zh.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:26:40.990585 areshook-0.1.3.2/areshook/
--rw-rw-r--   0 mark      (1000) mark      (1000)      298 2024-04-28 01:56:01.000000 areshook-0.1.3.2/areshook/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1112 2024-04-26 10:22:24.000000 areshook-0.1.3.2/areshook/_exceptions.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     6048 2024-04-28 07:10:39.000000 areshook-0.1.3.2/areshook/_frida.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      245 2024-04-28 07:10:39.000000 areshook-0.1.3.2/areshook/_modules.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:26:40.990585 areshook-0.1.3.2/areshook.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      634 2024-04-28 08:26:40.000000 areshook-0.1.3.2/areshook.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      303 2024-04-28 08:26:40.000000 areshook-0.1.3.2/areshook.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 08:26:40.000000 areshook-0.1.3.2/areshook.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       36 2024-04-28 08:26:40.000000 areshook-0.1.3.2/areshook.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        9 2024-04-28 08:26:40.000000 areshook-0.1.3.2/areshook.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       79 2024-04-28 08:26:40.000000 areshook-0.1.3.2/requirements.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 08:26:40.990585 areshook-0.1.3.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      680 2024-04-28 08:26:40.000000 areshook-0.1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:39:08.391429 areshook-0.1.3.3/
+-rw-rw-rw-   0        0        0       71 2024-05-03 14:48:16.000000 areshook-0.1.3.3/.gitignore
+-rw-rw-rw-   0        0        0      661 2024-05-03 15:39:08.390428 areshook-0.1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-03 14:49:16.000000 areshook-0.1.3.3/README.md
+-rw-rw-rw-   0        0        0      212 2024-05-03 14:48:16.000000 areshook-0.1.3.3/README.zh.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:39:08.387425 areshook-0.1.3.3/areshook/
+-rw-rw-rw-   0        0        0      308 2024-05-03 14:48:16.000000 areshook-0.1.3.3/areshook/__init__.py
+-rw-rw-rw-   0        0        0     1145 2024-05-03 14:48:16.000000 areshook-0.1.3.3/areshook/_exceptions.py
+-rw-rw-rw-   0        0        0     6219 2024-05-03 14:48:16.000000 areshook-0.1.3.3/areshook/_frida.py
+-rw-rw-rw-   0        0        0      233 2024-05-03 15:26:38.000000 areshook-0.1.3.3/areshook/_modules.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:39:08.390428 areshook-0.1.3.3/areshook.egg-info/
+-rw-rw-rw-   0        0        0      661 2024-05-03 15:39:08.000000 areshook-0.1.3.3/areshook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-03 15:39:08.000000 areshook-0.1.3.3/areshook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:39:08.000000 areshook-0.1.3.3/areshook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-03 15:39:08.000000 areshook-0.1.3.3/areshook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 15:39:08.000000 areshook-0.1.3.3/areshook.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2024-05-03 14:48:16.000000 areshook-0.1.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:39:08.391429 areshook-0.1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      707 2024-05-03 14:49:29.000000 areshook-0.1.3.3/setup.py
+-rw-rw-rw-   0        0        0       56 2024-05-03 14:48:16.000000 areshook-0.1.3.3/upload_twine.sh
```

### Comparing `areshook-0.1.3.2/areshook/_exceptions.py` & `areshook-0.1.3.3/areshook/_exceptions.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-class AresException(Exception):
-    def __init__(self, message: str):
-        super().__init__(message)
-
-
-class FridaServerNotRunningException(AresException):
-    def __init__(self, device_serial: str):
-        super().__init__(
-            f"Frida server is not running on device with serial {device_serial}"
-        )
-
-
-class FridaDeviceNotFoundException(AresException):
-    def __init__(self, device_serial: str):
-        super().__init__(f"Device with serial {device_serial} not found")
-
-
-class FridaProcessNotAttachedException(AresException):
-    def __init__(self):
-        super().__init__("No session attached. Please call attach() method first.")
-
-
-class FridaTargetNotRunningException(AresException):
-    def __init__(self, target: [str, int]):
-        if isinstance(target, int):
-            super().__init__(f"Target with PID {target} is not running")
-        else:
-            super().__init__(f"Target {target} is not running")
-
-
-class FridaPackageNotInstalledException(AresException):
-    def __init__(self, package_name: str):
-        super().__init__(f"Package {package_name} is not installed")
+class AresException(Exception):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
+class FridaServerNotRunningException(AresException):
+    def __init__(self, device_serial: str):
+        super().__init__(
+            f"Frida server is not running on device with serial {device_serial}"
+        )
+
+
+class FridaDeviceNotFoundException(AresException):
+    def __init__(self, device_serial: str):
+        super().__init__(f"Device with serial {device_serial} not found")
+
+
+class FridaProcessNotAttachedException(AresException):
+    def __init__(self):
+        super().__init__("No session attached. Please call attach() method first.")
+
+
+class FridaTargetNotRunningException(AresException):
+    def __init__(self, target: [str, int]):
+        if isinstance(target, int):
+            super().__init__(f"Target with PID {target} is not running")
+        else:
+            super().__init__(f"Target {target} is not running")
+
+
+class FridaPackageNotInstalledException(AresException):
+    def __init__(self, package_name: str):
+        super().__init__(f"Package {package_name} is not installed")
```

### Comparing `areshook-0.1.3.2/areshook/_frida.py` & `areshook-0.1.3.3/areshook/_frida.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import time
-from functools import wraps
-
-import frida
-from frida.core import Device, Script, Session
-from heradata import ElasticsearchSingleton
-
-from ._exceptions import FridaProcessNotAttachedException, \
-    FridaServerNotRunningException, FridaTargetNotRunningException, \
-    FridaPackageNotInstalledException
-from ._modules import AresMessage
-
-
-class FridaHooker:
-    _serial: str
-    _device: Device = None
-    _session: Session = None
-    _session_id: str = None
-    _package_name: str = None
-    _attached_process_name: str = None
-    _attached_pid: int = None
-    _running_script: dict[str, Script] = {}
-    _es_client: ElasticsearchSingleton = None
-
-    @staticmethod
-    def __check_session(func):
-        @wraps(func)
-        def inner(self, *args, **kwargs):
-            if self._session is None:
-                raise FridaProcessNotAttachedException()
-            return func(self, *args, **kwargs)
-
-        return inner
-
-    @staticmethod
-    def __get_frida_device(device_serial: str) -> [Device | None]:
-        try:
-            return frida.get_device(device_serial)
-        except frida.ServerNotRunningError:
-            return None
-
-    def __init__(self, device_serial: str):
-        self._device = self.__get_frida_device(device_serial)
-        if self._device is None:
-            raise FridaServerNotRunningException(device_serial)
-        self._serial = device_serial
-        self._es_client = ElasticsearchSingleton()
-
-    def __del__(self):
-        if self._running_script:
-            for script in self._running_script:
-                script.unload()
-        if self._session is not None:
-            self._session.detach()
-
-    def __is_package_running(self, target: [str | int]) -> bool:
-        return target in [process.pid if isinstance(target, int) else process.name
-                          for process in self._device.enumerate_processes()]
-
-    def __is_package_installed(self, package_name: str) -> bool:
-        return package_name in [app.identifier for app in
-                                self._device.enumerate_applications()]
-
-    def __get_pid(self, target: [str | int]) -> int:
-        if isinstance(target, int):
-            return target
-        return self._device.get_process(target).pid
-
-    def __get_process_name(self, target: int) -> str:
-        for process in self._device.enumerate_processes():
-            if process.pid == target:
-                return process.name
-
-    def attach(self, target: [str | int]) -> "FridaHooker":
-        if not self.__is_package_running(target):
-            raise FridaTargetNotRunningException(target)
-        if isinstance(target, str):
-            self._package_name = target
-        target = self.__get_pid(target)
-        if self._session is None:
-            self._session = self._device.attach(target)
-            self._attached_pid = target
-        else:
-            self._session.detach()
-            self._session = self._device.attach(target)
-            self._attached_pid = target
-        self._session_id = self.__get_process_name(
-            self._attached_pid
-        ) + '_' + str(int(time.time() * 1000))
-        return self
-
-    def spawn(self, package_name: str, resume=True) -> "FridaHooker":
-        if not self.__is_package_installed(package_name):
-            raise FridaPackageNotInstalledException(package_name)
-        self._package_name = package_name
-        pid = self._device.spawn(package_name)
-        self._session = self._device.attach(pid)
-        self._attached_pid = pid
-        if resume:
-            self.resume()
-        self._session_id = self.__get_process_name(
-            self._attached_pid
-        ) + '_' + str(int(time.time() * 1000))
-        return self
-
-    def resume(self) -> "FridaHooker":
-        if self._attached_pid is not None:
-            self._device.resume(self._attached_pid)
-        return self
-
-    def __logger_bind_script_name(self, script_name):
-        def on_logger(level, text):
-            self._es_client.es.index(
-                index='ares',
-                body=AresMessage(
-                    device_serial=self._serial,
-                    package_name=self._package_name,
-                    pid=self._attached_pid,
-                    session_id=self._session_id,
-                    script_name=script_name,
-                    message_type='log',
-                    message={
-                        'level': level,
-                        'text': text
-                    },
-                    timestamp=int(time.time() * 1000)
-                ).dict()
-            )
-
-        return on_logger
-
-    def __message_bind_script_name(self, script_name):
-        def on_message(message, data):
-            self._es_client.es.index(
-                index='ares',
-                body=AresMessage(
-                    device_serial=self._serial,
-                    package_name=self._package_name,
-                    pid=self._attached_pid,
-                    session_id=self._session_id,
-                    script_name=script_name,
-                    message_type='message',
-                    message={
-                        'message': message,
-                        'data': data
-                    },
-                    timestamp=int(time.time() * 1000)
-                ).dict()
-            )
-
-        return on_message
-
-    @__check_session
-    def run_script(self, script_content: str, script_name: str) -> "FridaHooker":
-        if script_name in self._running_script:
-            self._running_script[script_name].unload()
-        script: Script = self._session.create_script(script_content)
-        script.set_log_handler(self.__logger_bind_script_name(script_name))
-        script.on('message', self.__message_bind_script_name(script_name))
-        script.load()
-        self._running_script[script_name] = script
-        return self
-
-    def get_session_id(self):
-        return self._session_id
-
-    def get_script_names(self):
-        return self._running_script.keys()
-
-    def get_script(self, name):
-        return self._running_script[name]
+import time
+from functools import wraps
+
+import frida
+from frida.core import Device, Script, Session
+from heradata import ElasticsearchSingleton
+
+from ._exceptions import FridaProcessNotAttachedException, \
+    FridaServerNotRunningException, FridaTargetNotRunningException, \
+    FridaPackageNotInstalledException
+from ._modules import AresMessage
+
+
+class FridaHooker:
+    _serial: str
+    _device: Device = None
+    _session: Session = None
+    _session_id: str = None
+    _package_name: str = None
+    _attached_process_name: str = None
+    _attached_pid: int = None
+    _running_script: dict[str, Script] = {}
+    _es_client: ElasticsearchSingleton = None
+
+    @staticmethod
+    def __check_session(func):
+        @wraps(func)
+        def inner(self, *args, **kwargs):
+            if self._session is None:
+                raise FridaProcessNotAttachedException()
+            return func(self, *args, **kwargs)
+
+        return inner
+
+    @staticmethod
+    def __get_frida_device(device_serial: str) -> [Device | None]:
+        try:
+            return frida.get_device(device_serial)
+        except frida.ServerNotRunningError:
+            return None
+
+    def __init__(self, device_serial: str):
+        self._device = self.__get_frida_device(device_serial)
+        if self._device is None:
+            raise FridaServerNotRunningException(device_serial)
+        self._serial = device_serial
+        self._es_client = ElasticsearchSingleton()
+
+    def __del__(self):
+        if self._running_script:
+            for script in self._running_script:
+                script.unload()
+        if self._session is not None:
+            self._session.detach()
+
+    def __is_package_running(self, target: [str | int]) -> bool:
+        return target in [process.pid if isinstance(target, int) else process.name
+                          for process in self._device.enumerate_processes()]
+
+    def __is_package_installed(self, package_name: str) -> bool:
+        return package_name in [app.identifier for app in
+                                self._device.enumerate_applications()]
+
+    def __get_pid(self, target: [str | int]) -> int:
+        if isinstance(target, int):
+            return target
+        return self._device.get_process(target).pid
+
+    def __get_process_name(self, target: int) -> str:
+        for process in self._device.enumerate_processes():
+            if process.pid == target:
+                return process.name
+
+    def attach(self, target: [str | int]) -> "FridaHooker":
+        if not self.__is_package_running(target):
+            raise FridaTargetNotRunningException(target)
+        if isinstance(target, str):
+            self._package_name = target
+        target = self.__get_pid(target)
+        if self._session is None:
+            self._session = self._device.attach(target)
+            self._attached_pid = target
+        else:
+            self._session.detach()
+            self._session = self._device.attach(target)
+            self._attached_pid = target
+        self._session_id = self.__get_process_name(
+            self._attached_pid
+        ) + '_' + str(int(time.time() * 1000))
+        return self
+
+    def spawn(self, package_name: str, resume=True) -> "FridaHooker":
+        if not self.__is_package_installed(package_name):
+            raise FridaPackageNotInstalledException(package_name)
+        self._package_name = package_name
+        pid = self._device.spawn(package_name)
+        self._session = self._device.attach(pid)
+        self._attached_pid = pid
+        if resume:
+            self.resume()
+        self._session_id = self.__get_process_name(
+            self._attached_pid
+        ) + '_' + str(int(time.time() * 1000))
+        return self
+
+    def resume(self) -> "FridaHooker":
+        if self._attached_pid is not None:
+            self._device.resume(self._attached_pid)
+        return self
+
+    def __logger_bind_script_name(self, script_name):
+        def on_logger(level, text):
+            self._es_client.es.index(
+                index='ares',
+                body=AresMessage(
+                    device_serial=self._serial,
+                    package_name=self._package_name,
+                    pid=self._attached_pid,
+                    session_id=self._session_id,
+                    script_name=script_name,
+                    message_type='log',
+                    message={
+                        'level': level,
+                        'text': text
+                    },
+                    timestamp=int(time.time() * 1000)
+                ).dict()
+            )
+
+        return on_logger
+
+    def __message_bind_script_name(self, script_name):
+        def on_message(message, data):
+            self._es_client.es.index(
+                index='ares',
+                body=AresMessage(
+                    device_serial=self._serial,
+                    package_name=self._package_name,
+                    pid=self._attached_pid,
+                    session_id=self._session_id,
+                    script_name=script_name,
+                    message_type='message',
+                    message={
+                        'message': message,
+                        'data': data
+                    },
+                    timestamp=int(time.time() * 1000)
+                ).dict()
+            )
+
+        return on_message
+
+    @__check_session
+    def run_script(self, script_content: str, script_name: str) -> "FridaHooker":
+        if script_name in self._running_script:
+            self._running_script[script_name].unload()
+        script: Script = self._session.create_script(script_content)
+        script.set_log_handler(self.__logger_bind_script_name(script_name))
+        script.on('message', self.__message_bind_script_name(script_name))
+        script.load()
+        self._running_script[script_name] = script
+        return self
+
+    def get_session_id(self):
+        return self._session_id
+
+    def get_script_names(self):
+        return self._running_script.keys()
+
+    def get_script(self, name):
+        return self._running_script[name]
```

