# Comparing `tmp/arclet_entari-0.3.3.tar.gz` & `tmp/arclet_entari-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_entari-0.3.3.tar", last modified: Wed May  1 15:05:54 2024, max compression
+gzip compressed data, was "arclet_entari-0.4.0.tar", last modified: Fri May  3 15:14:27 2024, max compression
```

## Comparing `arclet_entari-0.3.3.tar` & `arclet_entari-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/LICENSE
--rw-r--r--   0        0        0      880 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/README.md
--rw-r--r--   0        0        0     2147 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/__init__.py
--rw-r--r--   0        0        0      110 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/command/__init__.py
--rw-r--r--   0        0        0      480 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/command/argv.py
--rw-r--r--   0        0        0     8556 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/command/main.py
--rw-r--r--   0        0        0     1142 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/command/model.py
--rw-r--r--   0        0        0      787 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/command/plugin.py
--rw-r--r--   0        0        0     5569 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/command/provider.py
--rw-r--r--   0        0        0     3442 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/core.py
--rw-r--r--   0        0        0    10616 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/event.py
--rw-r--r--   0        0        0      950 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/filter.py
--rw-r--r--   0        0        0     9684 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/message.py
--rw-r--r--   0        0        0     3295 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/plugin.py
--rw-r--r--   0        0        0    11175 2024-05-01 15:05:27.239424 arclet_entari-0.3.3/arclet/entari/session.py
--rw-r--r--   0        0        0     1821 2024-05-01 15:05:54.919368 arclet_entari-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 arclet_entari-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/LICENSE
+-rw-r--r--   0        0        0      872 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/README.md
+-rw-r--r--   0        0        0     2147 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/argv.py
+-rw-r--r--   0        0        0     8556 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/main.py
+-rw-r--r--   0        0        0     1142 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/model.py
+-rw-r--r--   0        0        0      914 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/plugin.py
+-rw-r--r--   0        0        0     5590 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/command/provider.py
+-rw-r--r--   0        0        0     3532 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/core.py
+-rw-r--r--   0        0        0    10616 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/event.py
+-rw-r--r--   0        0        0      950 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/filter.py
+-rw-r--r--   0        0        0     9684 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/message.py
+-rw-r--r--   0        0        0     4772 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/plugin.py
+-rw-r--r--   0        0        0    13585 2024-05-03 15:14:03.946499 arclet_entari-0.4.0/arclet/entari/session.py
+-rw-r--r--   0        0        0     1821 2024-05-03 15:14:27.598539 arclet_entari-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 arclet_entari-0.4.0/PKG-INFO
```

### Comparing `arclet_entari-0.3.3/LICENSE` & `arclet_entari-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/README.md` & `arclet_entari-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from arclet.entari import ContextSession, Entari, EntariCommands, WebsocketsInfo
 
 command = EntariCommands()
 
 
 @command.on("add {a} {b}")
 async def add(a: int, b: int, session: ContextSession):
-    await session.send_message(f"{a + b =}")
+    await session.send(f"{a + b =}")
 
 
 app = Entari()
 app.apply(WebsocketsInfo(port=5500, token="XXX"))
 
 app.run()
```

### Comparing `arclet_entari-0.3.3/arclet/entari/__init__.py` & `arclet_entari-0.4.0/arclet/entari/__init__.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/arclet/entari/command/main.py` & `arclet_entari-0.4.0/arclet/entari/command/main.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/arclet/entari/command/model.py` & `arclet_entari-0.4.0/arclet/entari/command/model.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/arclet/entari/command/plugin.py` & `arclet_entari-0.4.0/arclet/entari/command/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from arclet.alconna import Alconna
 
 from ..event import MessageEvent
-from ..plugin import Plugin, PluginDispatcher, PluginDispatcherFactory
+from ..plugin import Plugin, PluginDispatcher, PluginDispatcherFactory, register_factory
 from .provider import AlconnaProviderFactory, AlconnaSuppiler, MessageJudger
 
 
 class AlconnaDispatcher(PluginDispatcherFactory):
 
     def __init__(
         self,
@@ -18,7 +18,13 @@
         self.remove_tome = remove_tome
 
     def dispatch(self, plugin: Plugin) -> PluginDispatcher:
         disp = PluginDispatcher(plugin, MessageEvent)
         disp.bind(MessageJudger(), AlconnaSuppiler(self.command, self.need_tome, self.remove_tome))
         disp.bind(AlconnaProviderFactory())
         return disp
+
+
+register_factory(
+    Alconna,
+    lambda cmd, *args, **kwargs: AlconnaDispatcher(cmd, *args, **kwargs),
+)
```

### Comparing `arclet_entari-0.3.3/arclet/entari/command/provider.py` & `arclet_entari-0.4.0/arclet/entari/command/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             may_help_text: Optional[str] = cap.get("output", None)
         if _res.matched:
             context["alc_result"] = CommandResult(self.cmd, _res, may_help_text)
             return context
         elif may_help_text:
             await account.send(context["$event"], MessageChain(may_help_text))
             return False
+        return False
 
     @property
     def scopes(self) -> set[Scope]:
         return {Scope.prepare}
 
 
 class AlconnaProvider(Provider[Any]):
```

### Comparing `arclet_entari-0.3.3/arclet/entari/core.py` & `arclet_entari-0.4.0/arclet/entari/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     async def __call__(self, context: Contexts):
         if account := context.get("$account"):
             return account.session
 
 
 class ContextSessionProvider(Provider[ContextSession]):
     async def __call__(self, context: Contexts):
-        if "$origin_event" and "$account" in context:
+        if "$origin_event" in context and "$account" in context:
             return ContextSession(context["$account"], context["$origin_event"])
 
 
 global_providers.extend([SessionProvider(), ContextSessionProvider()])
 
 
 class Entari(App):
@@ -44,14 +44,16 @@
     async def handle_event(self, account: Account, event: Event):
         async def event_parse_task(connection: Account, raw: Event):
             loop = asyncio.get_running_loop()
             with suppress(NotImplementedError):
                 ev = event_parse(connection, raw)
                 self.event_system.publish(ev)
                 for disp in dispatchers.values():
+                    if not disp.validate(ev):
+                        continue
                     task = loop.create_task(disp.publish(ev))
                     self._ref_tasks.add(task)
                     task.add_done_callback(self._ref_tasks.discard)
                 return
 
             logger.warning(f"received unsupported event {raw.type}: {raw}")
```

### Comparing `arclet_entari-0.3.3/arclet/entari/event.py` & `arclet_entari-0.4.0/arclet/entari/event.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/arclet/entari/filter.py` & `arclet_entari-0.4.0/arclet/entari/filter.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/arclet/entari/message.py` & `arclet_entari-0.4.0/arclet/entari/message.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.3.3/arclet/entari/plugin.py` & `arclet_entari-0.4.0/arclet/entari/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 from abc import ABC, abstractmethod
 from contextlib import suppress
 from dataclasses import dataclass, field
 import importlib
 import inspect
 from os import PathLike
 from pathlib import Path
-from typing import Callable
+from typing import Any, Callable, TypeVar, overload
+from typing_extensions import Unpack
 
-from arclet.letoderea import BaseEvent, Publisher, system_ctx
+from arclet.letoderea import BaseAuxiliary, BaseEvent, Provider, Publisher, StepOut, system_ctx
+from arclet.letoderea.builtin.breakpoint import R
+from arclet.letoderea.typing import TTarget
 from loguru import logger
 
-dispatchers = {}
+dispatchers: dict[str, PluginDispatcher] = {}
 
 
 class PluginDispatcher(Publisher):
     def __init__(
         self,
         plugin: Plugin,
         *events: type[BaseEvent],
@@ -24,24 +27,50 @@
     ):
         super().__init__(plugin.name, *events, predicate=predicate)  # type: ignore
         self.plugin = plugin
         if es := system_ctx.get():
             es.register(self)
         else:
             dispatchers[self.id] = self
+        self._events = events
+
+    def waiter(
+        self,
+        *events: type[BaseEvent],
+        providers: list[Provider | type[Provider]] | None = None,
+        auxiliaries: list[BaseAuxiliary] | None = None,
+        priority: int = 15,
+        block: bool = False,
+    ) -> Callable[[TTarget[R]], StepOut[R]]:
+        def wrapper(func: TTarget[R]):
+            nonlocal events
+            if not events:
+                events = self._events
+            return StepOut(list(events), func, providers, auxiliaries, priority, block)  # type: ignore
+
+        return wrapper
 
     on = Publisher.register
     handle = Publisher.register
 
 
 class PluginDispatcherFactory(ABC):
     @abstractmethod
     def dispatch(self, plugin: Plugin) -> PluginDispatcher: ...
 
 
+MAPPING: dict[type, Callable[..., PluginDispatcherFactory]] = {}
+
+T = TypeVar("T")
+
+
+def register_factory(cls: type[T], factory: Callable[[T, Unpack[tuple[Any, ...]]], PluginDispatcherFactory]):
+    MAPPING[cls] = factory
+
+
 @dataclass
 class Plugin:
     author: list[str] = field(default_factory=list)
     name: str | None = None
     version: str | None = None
     license: str | None = None
     urls: dict[str, str] | None = None
@@ -61,16 +90,27 @@
         self.name = self.name or self.__module__
 
     def dispatch(self, *events: type[BaseEvent], predicate: Callable[[BaseEvent], bool] | None = None):
         disp = PluginDispatcher(self, *events, predicate=predicate)
         self._dispatchers[disp.id] = disp
         return disp
 
-    def mount(self, factory: PluginDispatcherFactory):
-        disp = factory.dispatch(self)
+    @overload
+    def mount(self, factory: PluginDispatcherFactory) -> PluginDispatcher: ...
+
+    @overload
+    def mount(self, factory: object, *args, **kwargs) -> PluginDispatcher: ...
+
+    def mount(self, factory: Any, *args, **kwargs):
+        if isinstance(factory, PluginDispatcherFactory):
+            disp = factory.dispatch(self)
+        elif factory_cls := MAPPING.get(factory.__class__):
+            disp = factory_cls(factory, *args, **kwargs).dispatch(self)
+        else:
+            raise TypeError(f"unsupported factory {factory!r}")
         self._dispatchers[disp.id] = disp
         return disp
 
     def dispose(self):
         for disp in self._dispatchers.values():
             if disp.id in dispatchers:
                 del dispatchers[disp.id]
```

### Comparing `arclet_entari-0.3.3/arclet/entari/session.py` & `arclet_entari-0.4.0/arclet/entari/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,98 @@
 from __future__ import annotations
 
 from collections.abc import Iterable
+from typing import NoReturn
 
+from arclet.letoderea import ParsingStop, StepOut
 from satori.client.account import Account
 from satori.const import EventType
 from satori.element import Element
-from satori.model import Channel, Event, Member, MessageObject, PageResult, Role, User
+from satori.model import Channel, Event, Guild, Member, MessageObject, PageResult, Role, User
+
+from .event import MessageEvent
+from .message import MessageChain
 
 
 class ContextSession:
     """在 Satori-Python 的 Session 的基础上存储了当次事件的信息"""
 
     def __init__(self, account: Account, event: Event):
         self.account = account
         self.context = event
 
+    async def prompt(
+        self,
+        message: str | Iterable[str | Element],
+        timeout: float = 120,
+        timeout_message: str | Iterable[str | Element] = "等待超时",
+    ) -> MessageChain:
+        """发送提示消息, 并等待回复
+
+        参数:
+            message: 要发送的消息
+        """
+        if self.context.type != EventType.MESSAGE_CREATED:
+            raise RuntimeError("Event cannot be prompted!")
+
+        await self.send(message)
+
+        async def waiter(content: MessageChain, session: ContextSession):
+            if (
+                self.context.channel
+                and session.context.channel
+                and self.context.channel.id == session.context.channel.id
+            ):
+                return content
+            if self.context.user and session.context.user and self.context.user.id == session.context.user.id:
+                return content
+
+        waiter.__annotations__ = {"content": MessageChain, "session": self.__class__}
+
+        step = StepOut([MessageEvent], waiter)
+
+        result = await step.wait(timeout=timeout)
+        if not result:
+            await self.send(timeout_message)
+            raise ParsingStop()
+        return result
+
+    def stop(self) -> NoReturn:
+        raise ParsingStop()
+
+    @property
+    def user(self) -> User:
+        if not self.context.user:
+            raise RuntimeError(f"Event {self.context.type!r} has no User")
+        return self.context.user
+
+    @property
+    def guild(self) -> Guild:
+        if not self.context.guild:
+            raise RuntimeError(f"Event {self.context.type!r} has no Guild")
+        return self.context.guild
+
+    @property
+    def channel(self) -> Channel:
+        if not self.context.channel:
+            raise RuntimeError(f"Event {self.context.type!r} has no Channel")
+        return self.context.channel
+
+    @property
+    def member(self) -> Member:
+        if not self.context.member:
+            raise RuntimeError(f"Event {self.context.type!r} has no Member")
+        return self.context.member
+
+    @property
+    def content(self) -> str:
+        if not self.context.message:
+            raise RuntimeError(f"Event {self.context.type!r} has no Content")
+        return self.context.message.content
+
     def __getattr__(self, item):
         return getattr(self.account.session, item)
 
     async def send(
         self,
         message: str | Iterable[str | Element],
     ) -> list[MessageObject]:
```

### Comparing `arclet_entari-0.3.3/pyproject.toml` & `arclet_entari-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-entari"
-version = "0.3.3"
+version = "0.4.0"
 description = "Simple IM Framework based on satori-python"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "arclet-letoderea>=0.9.2",
     "arclet-alconna>=1.8.11",
```

### Comparing `arclet_entari-0.3.3/PKG-INFO` & `arclet_entari-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-entari
-Version: 0.3.3
+Version: 0.4.0
 Summary: Simple IM Framework based on satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -39,15 +39,15 @@
 from arclet.entari import ContextSession, Entari, EntariCommands, WebsocketsInfo
 
 command = EntariCommands()
 
 
 @command.on("add {a} {b}")
 async def add(a: int, b: int, session: ContextSession):
-    await session.send_message(f"{a + b =}")
+    await session.send(f"{a + b =}")
 
 
 app = Entari()
 app.apply(WebsocketsInfo(port=5500, token="XXX"))
 
 app.run()
```

