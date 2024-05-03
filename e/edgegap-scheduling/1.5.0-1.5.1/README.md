# Comparing `tmp/edgegap_scheduling-1.5.0.tar.gz` & `tmp/edgegap_scheduling-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_scheduling-1.5.0.tar", max compression
+gzip compressed data, was "edgegap_scheduling-1.5.1.tar", max compression
```

## Comparing `edgegap_scheduling-1.5.0.tar` & `edgegap_scheduling-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/LICENSE
--rw-r--r--   0        0        0     2164 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/README.md
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/BUILD
--rw-r--r--   0        0        0      330 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/__init__.py
--rw-r--r--   0        0        0      128 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_depends.py
--rw-r--r--   0        0        0     4269 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_runner.py
--rw-r--r--   0        0        0     4436 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_scheduler.py
--rw-r--r--   0        0        0     1303 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_signature.py
--rw-r--r--   0        0        0      482 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_singleton.py
--rw-r--r--   0        0        0     1468 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_sleep.py
--rw-r--r--   0        0        0      550 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_state.py
--rw-r--r--   0        0        0     4291 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/_task.py
--rw-r--r--   0        0        0       17 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/errors/BUILD
--rw-r--r--   0        0        0      133 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/errors/__init__.py
--rw-r--r--   0        0        0      103 2024-05-02 18:20:19.991672 edgegap_scheduling-1.5.0/edgegap_scheduling/errors/_errors.py
--rw-r--r--   0        0        0      691 2024-05-02 18:20:32.343986 edgegap_scheduling-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 edgegap_scheduling-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-03 03:42:53.861682 edgegap_scheduling-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2164 2024-05-03 03:42:53.861839 edgegap_scheduling-1.5.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.861961 edgegap_scheduling-1.5.1/edgegap_scheduling/BUILD
+-rw-r--r--   0        0        0      380 2024-05-03 03:42:53.862180 edgegap_scheduling-1.5.1/edgegap_scheduling/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-03 03:42:53.862378 edgegap_scheduling-1.5.1/edgegap_scheduling/_depends.py
+-rw-r--r--   0        0        0     4688 2024-05-03 03:42:53.862654 edgegap_scheduling-1.5.1/edgegap_scheduling/_runner.py
+-rw-r--r--   0        0        0     5621 2024-05-03 03:42:53.862996 edgegap_scheduling-1.5.1/edgegap_scheduling/_scheduler.py
+-rw-r--r--   0        0        0     1375 2024-05-03 03:42:53.863293 edgegap_scheduling-1.5.1/edgegap_scheduling/_signature.py
+-rw-r--r--   0        0        0      482 2024-05-03 03:42:53.863651 edgegap_scheduling-1.5.1/edgegap_scheduling/_singleton.py
+-rw-r--r--   0        0        0     1468 2024-05-03 03:42:53.864167 edgegap_scheduling-1.5.1/edgegap_scheduling/_sleep.py
+-rw-r--r--   0        0        0      550 2024-05-03 03:42:53.864596 edgegap_scheduling-1.5.1/edgegap_scheduling/_state.py
+-rw-r--r--   0        0        0     4351 2024-05-03 03:42:53.864906 edgegap_scheduling-1.5.1/edgegap_scheduling/_task.py
+-rw-r--r--   0        0        0       17 2024-05-03 03:42:53.865038 edgegap_scheduling-1.5.1/edgegap_scheduling/errors/BUILD
+-rw-r--r--   0        0        0      133 2024-05-03 03:42:53.865426 edgegap_scheduling-1.5.1/edgegap_scheduling/errors/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-03 03:42:53.865809 edgegap_scheduling-1.5.1/edgegap_scheduling/errors/_errors.py
+-rw-r--r--   0        0        0      691 2024-05-03 14:08:53.099062 edgegap_scheduling-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 edgegap_scheduling-1.5.1/PKG-INFO
```

### Comparing `edgegap_scheduling-1.5.0/LICENSE` & `edgegap_scheduling-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.0/README.md` & `edgegap_scheduling-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.0/edgegap_scheduling/_runner.py` & `edgegap_scheduling-1.5.1/edgegap_scheduling/_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import inspect
 import logging
 from datetime import datetime, timezone
+from types import AsyncGeneratorType
 from typing import Callable
 
 from pydantic import BaseModel
 
 from ._signature import TaskSignature
 from ._state import TaskState
 from ._task import Task
 
 logger = logging.getLogger('scheduling.Runner')
 
 
 class TaskRunner:
     def __init__(self, task: Task, sleep: Callable):
         super().__init__()
+        self.async_task = None
         self.__task = task
         self.__sleep = sleep
         self.__signature = TaskSignature(task.identifier, task.name, task.func)
 
     def __str__(self):
         return f'Runner: {self.__task}'
 
@@ -26,16 +29,16 @@
         return self.__task.need_to_loop
 
     def get_task(self) -> Task:
         return self.__task.model_copy()
 
     def update_task(
         self,
-        every: str | None,
-        delay: str | None,
+        every: str | None = None,
+        delay: str | None = None,
         parameters: dict | None = None,
     ):
         if isinstance(every, str):
             self.__task.every = every or None
 
         if isinstance(delay, str):
             self.__task.delay = delay or None
@@ -90,36 +93,40 @@
 
             if self.__task.every_in_seconds is None:
                 logger.warning(f'Every changed in task {self.__task.name} without stopping it first!')
                 break
 
             sleep_duration = self.__task.next_sleep_duration
 
-            if sleep_duration <= 0 and self.__task.remove_running_time:
-                logger.warning(f'{self.__task.name} process for too long and the sleep duration is zero!')
-
-            elif sleep_duration is None:
+            if sleep_duration is None:
                 sleep_duration = self.__task.every_in_seconds
+            elif sleep_duration == 0 and self.__task.remove_running_time:
+                logger.warning(f'{self.__task.name} process for too long and the sleep duration is zero!')
 
             self.__task.sleep_at = datetime.now(tz=timezone.utc)
 
             await self.__sleep(self.__task.identifier, sleep_duration)
 
     async def __run(self, parameters: BaseModel | type[BaseModel] | None = None):
         arguments, generators = self.__signature.get_arguments(parameters or self.__task.parameters)
 
         try:
             for name, generator in generators.items():
-                arguments[name] = next(generator)
-
-            await self.__task.func(**arguments)
+                arguments[name] = (
+                    await generator.__anext__() if isinstance(generator, AsyncGeneratorType) else next(generator)
+                )
+
+            if inspect.iscoroutinefunction(self.__task.func):
+                await self.__task.func(**arguments)
+            else:
+                self.__task.func(**arguments)
 
         finally:
             for generator in generators.values():
-                generator.close()
+                await generator.aclose() if isinstance(generator, AsyncGeneratorType) else generator.close()
 
     def stop(self) -> bool:
         can_stop = self.__task.state == TaskState.RUNNING
 
         if can_stop:
             self.__task.state = TaskState.STOPPING
```

### Comparing `edgegap_scheduling-1.5.0/edgegap_scheduling/_scheduler.py` & `edgegap_scheduling-1.5.1/edgegap_scheduling/_scheduler.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,38 +25,52 @@
         identifier: str = None,
         continue_on_exception: bool = True,
         manual_run_allowed: bool = False,
         remove_running_time: bool = False,
         parameters: BaseModel | type[BaseModel] | None = None,
     ):
         def decorator(func):
+            _name = name or func.__name__
             task = Task(
-                name=name or func.__name__,
-                identifier=identifier or name.lower().replace(' ', '_'),
+                name=_name,
+                identifier=identifier or _name.lower().replace(' ', '_'),
                 func=func,
                 every=every,
                 delay=delay,
                 continue_on_exception=continue_on_exception,
                 manual_run_allowed=manual_run_allowed,
                 remove_running_time=remove_running_time,
-                parameters=parameters if isinstance(parameters, BaseModel) or parameters is None else parameters(),
+                parameters=parameters,
             )
             runner = TaskRunner(
                 task=task,
                 sleep=self.__async_sleep.sleep,
             )
             self.__register(task.identifier, runner)
 
         return decorator
 
     def __register(self, identifier: str, runner: TaskRunner) -> None:
         if identifier in self.__runners.keys():
-            raise Exception(f'Task {Format.squared(identifier, Color.RED)} already exists')
+            self.logger.warning(f'Task {Format.squared(identifier, Color.RED)} already exists')
+        else:
+            self.__runners[identifier] = runner
+
+    def unregister(self, identifier: str) -> None:
+        runner = self.__get_or_raise(identifier)
+        self.logger.info(f'Unregistering task {Format.squared(identifier, Color.YELLOW)}')
+        runner.stop()
+        del self.__runners[identifier]
+
+    def unregister_all(self) -> None:
+        self.logger.info('Unregistering all tasks')
+        for identifier, runner in self.__runners.items():
+            runner.stop()
 
-        self.__runners[identifier] = runner
+        self.__runners = {}
 
     def __get_or_raise(self, identifier: str) -> TaskRunner:
         runner = self.__runners.get(identifier)
 
         if runner is None:
             raise ValueError(f'Task [{identifier}] does not exist')
 
@@ -65,17 +79,17 @@
     async def get(self, identifier) -> Task:
         runner = self.__get_or_raise(identifier)
         return runner.get_task()
 
     async def update(
         self,
         identifier: str,
-        every: str | None,
-        delay: str | None,
-        parameters: dict | None,
+        every: str | None = None,
+        delay: str | None = None,
+        parameters: dict | None = None,
     ) -> Task:
         runner = self.__get_or_raise(identifier)
         runner.update_task(
             every=every,
             delay=delay,
             parameters=parameters,
         )
@@ -87,25 +101,50 @@
 
     async def start(self, identifier: str) -> Task:
         runner = self.__get_or_raise(identifier)
         self.logger.info(f'Starting {runner}')
         task = runner.get_task()
 
         if task.safe_to_start:
-            asyncio.ensure_future(runner.start())
+            _task = asyncio.ensure_future(runner.start())
+            runner.async_task = _task
+
         else:
             task.message = 'Task already started'
 
         return task
 
-    async def start_all(self):
+    async def gather(self, identifier: str) -> bool:
+        runner = self.__get_or_raise(identifier)
+        success = False
+
+        if runner.async_task:
+            await asyncio.gather(runner.async_task)
+            success = True
+
+        return success
+
+    async def gather_all(self) -> int:
+        tasks = [runner.async_task for runner in self.__runners.values() if runner.async_task is not None]
+        await asyncio.gather(
+            *tasks,
+        )
+        return len(tasks)
+
+    async def start_all(self) -> int:
+        tasks_started = 0
         self.logger.info('Starting All Tasks')
+
         for runner in self.__runners.values():
             if runner.should_schedule:
-                await runner.start()
+                _task = asyncio.ensure_future(runner.start())
+                runner.async_task = _task
+                tasks_started += 1
+
+        return tasks_started
 
     async def stop(self, identifier: str) -> Task:
         runner = self.__get_or_raise(identifier)
         self.logger.info(f'Stopping {runner}')
         can_stop = runner.stop()
         task = runner.get_task()
 
@@ -126,16 +165,18 @@
 
         params = task.parameters.model_copy(update=parameters) if isinstance(parameters, dict) else None
 
         await runner.run(params)
 
         return runner.get_task()
 
-    async def stop_all(self):
+    async def stop_all(self) -> int:
         self.logger.info('Stopping All Running Tasks')
 
         for runner in self.__runners.values():
             runner.stop()
             self.logger.info(f'Stopping {runner}')
 
         count = await self.__async_sleep.cancel_all()
         self.logger.info(f'{count} tasks stopped')
+
+        return count
```

### Comparing `edgegap_scheduling-1.5.0/edgegap_scheduling/_signature.py` & `edgegap_scheduling-1.5.1/edgegap_scheduling/_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 import logging
-from types import GeneratorType
+from types import AsyncGeneratorType, GeneratorType
 from typing import Any, Callable
 
 from pydantic import BaseModel
 
 from ._depends import Depends
 
 
@@ -19,25 +19,27 @@
         parameters: BaseModel | type[BaseModel] | None = None,
     ) -> tuple[dict[str, Any], dict[str, Any]]:
         specs = {}
         generators = {}
         signature = inspect.signature(self.__func)
 
         for name, param in signature.parameters.items():
-            match param.annotation:
-                case logging.Logger:
-                    specs[name] = logging.getLogger(f'scheduling.{self.__identifier}')
-                case parameters.__class__:
-                    specs[name] = parameters
-                case parameters:
-                    specs[name] = parameters()
-
             match param.default:
                 case Depends():
                     value = param.default.dependency()
 
-                    if isinstance(value, GeneratorType):
+                    if isinstance(value, (GeneratorType, AsyncGeneratorType)):
                         generators[name] = value
                     else:
                         specs[name] = value
 
+                    continue
+
+            match param.annotation:
+                case logging.Logger:
+                    specs[name] = logging.getLogger(f'scheduling.{self.__identifier}')
+                case parameters.__class__:
+                    specs[name] = parameters
+                case parameters:
+                    specs[name] = parameters()
+
         return specs, generators
```

### Comparing `edgegap_scheduling-1.5.0/edgegap_scheduling/_sleep.py` & `edgegap_scheduling-1.5.1/edgegap_scheduling/_sleep.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.0/edgegap_scheduling/_state.py` & `edgegap_scheduling-1.5.1/edgegap_scheduling/_state.py`

 * *Files identical despite different names*

### Comparing `edgegap_scheduling-1.5.0/edgegap_scheduling/_task.py` & `edgegap_scheduling-1.5.1/edgegap_scheduling/_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,18 +66,19 @@
                 return (self.sleep_at - self.begin_at).total_seconds()
 
     @computed_field(description='If the task is currently processing or sleeping')
     @property
     def is_processing(self) -> bool:
         is_running = False
 
-        if self.begin_at and self.sleep_at:
-            is_running = self.begin_at > self.sleep_at
-        elif self.begin_at and self.sleep_at is None:
-            is_running = True
+        if self.state == TaskState.RUNNING:
+            if self.begin_at and self.sleep_at:
+                is_running = self.begin_at > self.sleep_at
+            elif self.begin_at and self.sleep_at is None:
+                is_running = True
 
         return is_running
 
     @computed_field(description='If the task is currently sleeping (will be false if the task is not running)')
     @property
     def is_sleeping(self) -> bool:
         is_sleeping = False
```

### Comparing `edgegap_scheduling-1.5.0/pyproject.toml` & `edgegap_scheduling-1.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-scheduling"
-version = "1.5.0"
+version = "1.5.1"
 description = "The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.7.1"
```

### Comparing `edgegap_scheduling-1.5.0/PKG-INFO` & `edgegap_scheduling-1.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-scheduling
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Edgegap library includes various tools and helpers for helping with Scheduling Task. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edgegap Scheduling Library
```

