# Comparing `tmp/arclet-letoderea-0.9.0.tar.gz` & `tmp/arclet-letoderea-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-letoderea-0.9.0.tar", last modified: Sun Dec  3 09:16:38 2023, max compression
+gzip compressed data, was "arclet-letoderea-0.9.2.tar", last modified: Tue Dec  5 12:18:35 2023, max compression
```

## Comparing `arclet-letoderea-0.9.0.tar` & `arclet-letoderea-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1926 2023-12-01 10:22:42.361381 arclet-letoderea-0.9.0/arclet/letoderea/__init__.py
--rw-r--r--   0        0        0     5943 2023-12-01 10:26:14.316082 arclet-letoderea-0.9.0/arclet/letoderea/auxiliary.py
--rw-r--r--   0        0        0        0 2023-03-19 17:38:39.637869 arclet-letoderea-0.9.0/arclet/letoderea/builtin/__init__.py
--rw-r--r--   0        0        0     4069 2023-12-03 09:06:21.699895 arclet-letoderea-0.9.0/arclet/letoderea/builtin/breakpoint.py
--rw-r--r--   0        0        0      824 2023-11-27 07:14:06.936127 arclet-letoderea-0.9.0/arclet/letoderea/builtin/depend.py
--rw-r--r--   0        0        0      309 2023-09-15 08:04:19.543316 arclet-letoderea-0.9.0/arclet/letoderea/context.py
--rw-r--r--   0        0        0     3333 2023-12-03 09:11:51.888623 arclet-letoderea-0.9.0/arclet/letoderea/core.py
--rw-r--r--   0        0        0     2781 2023-11-27 06:30:19.231715 arclet-letoderea-0.9.0/arclet/letoderea/decorate.py
--rw-r--r--   0        0        0     1373 2023-12-01 10:22:13.600826 arclet-letoderea-0.9.0/arclet/letoderea/event.py
--rw-r--r--   0        0        0      304 2023-04-07 06:45:50.801739 arclet-letoderea-0.9.0/arclet/letoderea/exceptions.py
--rw-r--r--   0        0        0     5551 2023-12-03 09:12:33.947326 arclet-letoderea-0.9.0/arclet/letoderea/handler.py
--rw-r--r--   0        0        0     2879 2023-12-01 10:26:23.904058 arclet-letoderea-0.9.0/arclet/letoderea/provider.py
--rw-r--r--   0        0        0     6293 2023-12-03 09:08:32.929679 arclet-letoderea-0.9.0/arclet/letoderea/publisher.py
--rw-r--r--   0        0        0     2944 2023-11-27 06:30:19.281720 arclet-letoderea-0.9.0/arclet/letoderea/ref.py
--rw-r--r--   0        0        0     5262 2023-12-01 10:26:23.955256 arclet-letoderea-0.9.0/arclet/letoderea/subscriber.py
--rw-r--r--   0        0        0     1184 2023-11-27 07:34:11.859029 arclet-letoderea-0.9.0/arclet/letoderea/typing.py
--rw-r--r--   0        0        0     1091 2022-01-26 08:43:52.013649 arclet-letoderea-0.9.0/LICENSE
--rw-r--r--   0        0        0     1253 2023-12-03 09:14:55.480564 arclet-letoderea-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5194 2023-12-03 08:28:49.076537 arclet-letoderea-0.9.0/README.md
--rw-r--r--   0        0        0      833 2023-12-03 09:13:37.909800 arclet-letoderea-0.9.0/tests/annotated.py
--rw-r--r--   0        0        0     1439 2023-12-03 08:45:52.697686 arclet-letoderea-0.9.0/tests/breakpoint.py
--rw-r--r--   0        0        0     1967 2023-12-03 08:41:02.442626 arclet-letoderea-0.9.0/tests/breakpoint1.py
--rw-r--r--   0        0        0     2282 2023-04-07 06:47:47.105418 arclet-letoderea-0.9.0/tests/combine.py
--rw-r--r--   0        0        0     1840 2023-12-03 08:36:38.389078 arclet-letoderea-0.9.0/tests/condition.py
--rw-r--r--   0        0        0     1391 2023-12-03 08:36:17.550540 arclet-letoderea-0.9.0/tests/decorator.py
--rw-r--r--   0        0        0      739 2023-12-03 08:36:17.540959 arclet-letoderea-0.9.0/tests/depend.py
--rw-r--r--   0        0        0      560 2023-12-03 08:36:17.532380 arclet-letoderea-0.9.0/tests/except.py
--rw-r--r--   0        0        0      899 2023-12-03 08:35:13.206625 arclet-letoderea-0.9.0/tests/nest_except.py
--rw-r--r--   0        0        0     1148 2023-12-03 08:35:13.197634 arclet-letoderea-0.9.0/tests/shortcut.py
--rw-r--r--   0        0        0      874 2023-06-06 15:59:52.464023 arclet-letoderea-0.9.0/tests/test_handler.py
--rw-r--r--   0        0        0      649 2023-11-27 07:00:19.298564 arclet-letoderea-0.9.0/tests/test_param_parser.py
--rw-r--r--   0        0        0     1850 2023-09-15 08:13:08.875513 arclet-letoderea-0.9.0/tests/test_provider.py
--rw-r--r--   0        0        0      900 2023-12-03 08:34:12.132807 arclet-letoderea-0.9.0/tests/test_provider_validate.py
--rw-r--r--   0        0        0      899 2023-12-03 08:25:09.539739 arclet-letoderea-0.9.0/tests/test_publisher.py
--rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 arclet-letoderea-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1938 2023-12-05 12:16:12.684612 arclet-letoderea-0.9.2/arclet/letoderea/__init__.py
+-rw-r--r--   0        0        0     5943 2023-12-01 10:26:14.316082 arclet-letoderea-0.9.2/arclet/letoderea/auxiliary.py
+-rw-r--r--   0        0        0        0 2023-03-19 17:38:39.637869 arclet-letoderea-0.9.2/arclet/letoderea/builtin/__init__.py
+-rw-r--r--   0        0        0     4069 2023-12-03 09:06:21.699895 arclet-letoderea-0.9.2/arclet/letoderea/builtin/breakpoint.py
+-rw-r--r--   0        0        0      824 2023-11-27 07:14:06.936127 arclet-letoderea-0.9.2/arclet/letoderea/builtin/depend.py
+-rw-r--r--   0        0        0      309 2023-09-15 08:04:19.543316 arclet-letoderea-0.9.2/arclet/letoderea/context.py
+-rw-r--r--   0        0        0     3333 2023-12-03 09:11:51.888623 arclet-letoderea-0.9.2/arclet/letoderea/core.py
+-rw-r--r--   0        0        0     2787 2023-12-05 12:16:12.701605 arclet-letoderea-0.9.2/arclet/letoderea/decorate.py
+-rw-r--r--   0        0        0     1815 2023-12-05 12:16:55.792450 arclet-letoderea-0.9.2/arclet/letoderea/event.py
+-rw-r--r--   0        0        0      304 2023-04-07 06:45:50.801739 arclet-letoderea-0.9.2/arclet/letoderea/exceptions.py
+-rw-r--r--   0        0        0     5570 2023-12-05 05:44:44.663863 arclet-letoderea-0.9.2/arclet/letoderea/handler.py
+-rw-r--r--   0        0        0     2879 2023-12-01 10:26:23.904058 arclet-letoderea-0.9.2/arclet/letoderea/provider.py
+-rw-r--r--   0        0        0     6450 2023-12-05 05:44:44.664536 arclet-letoderea-0.9.2/arclet/letoderea/publisher.py
+-rw-r--r--   0        0        0     2944 2023-11-27 06:30:19.281720 arclet-letoderea-0.9.2/arclet/letoderea/ref.py
+-rw-r--r--   0        0        0     5263 2023-12-05 05:44:44.664536 arclet-letoderea-0.9.2/arclet/letoderea/subscriber.py
+-rw-r--r--   0        0        0     1184 2023-11-27 07:34:11.859029 arclet-letoderea-0.9.2/arclet/letoderea/typing.py
+-rw-r--r--   0        0        0     1091 2022-01-26 08:43:52.013649 arclet-letoderea-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1253 2023-12-05 12:18:09.540590 arclet-letoderea-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5484 2023-12-05 05:44:46.183824 arclet-letoderea-0.9.2/README.md
+-rw-r--r--   0        0        0      833 2023-12-03 09:13:37.909800 arclet-letoderea-0.9.2/tests/annotated.py
+-rw-r--r--   0        0        0     1439 2023-12-03 08:45:52.697686 arclet-letoderea-0.9.2/tests/breakpoint.py
+-rw-r--r--   0        0        0     1967 2023-12-03 08:41:02.442626 arclet-letoderea-0.9.2/tests/breakpoint1.py
+-rw-r--r--   0        0        0     2282 2023-04-07 06:47:47.105418 arclet-letoderea-0.9.2/tests/combine.py
+-rw-r--r--   0        0        0     1840 2023-12-03 08:36:38.389078 arclet-letoderea-0.9.2/tests/condition.py
+-rw-r--r--   0        0        0     1391 2023-12-03 08:36:17.550540 arclet-letoderea-0.9.2/tests/decorator.py
+-rw-r--r--   0        0        0      739 2023-12-03 08:36:17.540959 arclet-letoderea-0.9.2/tests/depend.py
+-rw-r--r--   0        0        0      560 2023-12-03 08:36:17.532380 arclet-letoderea-0.9.2/tests/except.py
+-rw-r--r--   0        0        0      899 2023-12-03 08:35:13.206625 arclet-letoderea-0.9.2/tests/nest_except.py
+-rw-r--r--   0        0        0     1138 2023-12-05 12:16:12.642712 arclet-letoderea-0.9.2/tests/shortcut.py
+-rw-r--r--   0        0        0      874 2023-06-06 15:59:52.464023 arclet-letoderea-0.9.2/tests/test_handler.py
+-rw-r--r--   0        0        0      649 2023-11-27 07:00:19.298564 arclet-letoderea-0.9.2/tests/test_param_parser.py
+-rw-r--r--   0        0        0     2149 2023-12-05 05:44:44.665535 arclet-letoderea-0.9.2/tests/test_provider.py
+-rw-r--r--   0        0        0      900 2023-12-03 08:34:12.132807 arclet-letoderea-0.9.2/tests/test_provider_validate.py
+-rw-r--r--   0        0        0      899 2023-12-03 08:25:09.539739 arclet-letoderea-0.9.2/tests/test_publisher.py
+-rw-r--r--   0        0        0     6136 1970-01-01 00:00:00.000000 arclet-letoderea-0.9.2/PKG-INFO
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/__init__.py` & `arclet-letoderea-0.9.2/arclet/letoderea/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from .builtin.breakpoint import StepOut as StepOut
 from .builtin.depend import Depend as Depend
 from .builtin.depend import Depends as Depends
 from .context import system_ctx as system_ctx
 from .core import EventSystem as EventSystem
 from .decorate import bind as bind
 from .decorate import bypass_if as bypass_if
-from .decorate import is_event as is_event
-from .decorate import not_event as not_event
+from .decorate import allow_event as allow_event
+from .decorate import refuse_event as refuse_event
 from .decorate import subscribe as subscribe
 from .event import BaseEvent as BaseEvent
 from .event import make_event as make_event
 from .exceptions import JudgementError as JudgementError
 from .exceptions import ParsingStop as ParsingStop
 from .exceptions import PropagationCancelled as PropagationCancelled
 from .provider import Param as Param
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/auxiliary.py` & `arclet-letoderea-0.9.2/arclet/letoderea/auxiliary.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/builtin/breakpoint.py` & `arclet-letoderea-0.9.2/arclet/letoderea/builtin/breakpoint.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/builtin/depend.py` & `arclet-letoderea-0.9.2/arclet/letoderea/builtin/depend.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/core.py` & `arclet-letoderea-0.9.2/arclet/letoderea/core.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/decorate.py` & `arclet-letoderea-0.9.2/arclet/letoderea/decorate.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,13 @@
                 else:
                     getattr(target, "__auxiliaries__").append(inner)
             return target
 
         return wrapper
 
 
-def is_event(*events: Type[BaseEvent]):
+def allow_event(*events: Type[BaseEvent]):
     return bypass_if(lambda ctx: not isinstance(ctx["$event"], events))
 
 
-def not_event(*events: Type[BaseEvent]):
+def refuse_event(*events: Type[BaseEvent]):
     return bypass_if(lambda ctx: isinstance(ctx["$event"], events))
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/event.py` & `arclet-letoderea-0.9.2/arclet/letoderea/event.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,32 +15,47 @@
         ...
 
 
 @lru_cache(4096)
 def get_providers(
     event: type[BaseEvent] | BaseEvent,
 ) -> list[Provider | ProviderFactory]:
-    res = getattr(event, "providers", [])
+    res = []
+    for cls in reversed(event.__mro__[:-1]):
+        res.extend(getattr(cls, "providers", []))
     res.extend(
         p
         for _, p in inspect.getmembers(
             event,
             lambda x: inspect.isclass(x) and issubclass(x, (Provider, ProviderFactory)),
         )
     )
     return [p() if isinstance(p, type) else p for p in res]
 
 
 @lru_cache(4096)
 def get_auxiliaries(event: type[BaseEvent] | BaseEvent) -> list[BaseAuxiliary]:
-    res = getattr(event, "auxiliaries", [])
-    res.extend(p for _, p in inspect.getmembers(event, lambda x: inspect.isclass(x) and issubclass(x, BaseAuxiliary)))
+    res = []
+    for cls in reversed(event.__mro__[:-1]):
+        res.extend(getattr(cls, "auxiliaries", []))
+    res.extend(
+        p
+        for _, p in inspect.getmembers(
+            event,
+            lambda x: inspect.isclass(x) and issubclass(x, BaseAuxiliary),
+        )
+    )
     return [a() if isinstance(a, type) else a for a in res]
 
 
 def make_event(cls: type) -> type:
+    if not hasattr(cls, "__annotations__"):
+        raise ValueError(f"@make_event can only take effect for class with attribute annotations, not {cls}")
+
     async def _gather(self, context: Contexts):
         for key in cls.__annotations__:
-            context[key] = getattr(self, key)
+            if key in ("providers", "auxiliaries"):
+                continue
+            context[key] = getattr(self, key, None)
 
     cls.gather = _gather  # type: ignore
     return cls  # type: ignore
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/handler.py` & `arclet-letoderea-0.9.2/arclet/letoderea/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,21 +88,21 @@
 
 
 async def depend_handler(
     target: Subscriber | Callable, event: BaseEvent | None = None, source: Contexts | None = None, inner: bool = False
 ):
     if event:
         if target.__class__ != Subscriber:
-            target = Subscriber(target, providers=get_providers(source))  # type: ignore
+            target = Subscriber(target, providers=get_providers(event.__class__))  # type: ignore
         contexts: Contexts = {"$event": event, "$subscriber": target}  # type: ignore
         await event.gather(contexts)
     elif source:
         contexts = source
         if target.__class__ != Subscriber:
-            target = Subscriber(target, providers=get_providers(source["$event"]))  # type: ignore
+            target = Subscriber(target, providers=get_providers(source["$event"].__class__))  # type: ignore
         contexts["$subscriber"] = target
     else:
         raise ValueError("Empty source")
     try:
         if Prepare in target.auxiliaries:
             for aux in target.auxiliaries[Prepare]:
                 await prepare(aux, contexts)
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/provider.py` & `arclet-letoderea-0.9.2/arclet/letoderea/provider.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/publisher.py` & `arclet-letoderea-0.9.2/arclet/letoderea/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,26 @@
         self.id = f"{id_}::{sorted(events, key=lambda e: id(e))}"
         self.event_queue = Queue(queue_size)
         self.subscribers = []
         self.providers = []
         self.auxiliaries = []
 
         if not events:
-            raise ValueError("events cannot be None")
-        for event in events:
-            self.providers.extend(get_providers(event))
-            self.auxiliaries.extend(get_auxiliaries(event))
-        if predicate:
-            self.id += f"::{predicate}"
-            self.validate = lambda e: isinstance(e, events) and predicate(e)
+            if not predicate:
+                raise ValueError("events cannot be None")
+            self.validate = predicate
         else:
-            self.validate = lambda e: isinstance(e, events)
+            for event in events:
+                self.providers.extend(get_providers(event))
+                self.auxiliaries.extend(get_auxiliaries(event))
+            if predicate:
+                self.id += f"::{predicate}"
+                self.validate = lambda e: isinstance(e, events) and predicate(e)
+            else:
+                self.validate = lambda e: isinstance(e, events)
 
     def __repr__(self):
         return f"{self.__class__.__name__}::{self.id}"
 
     async def publish(self, event: BaseEvent) -> Any:
         """主动向自己的订阅者发布事件"""
         await dispatch(self.subscribers, event)
@@ -141,14 +144,15 @@
         def register_wrapper(exec_target: Callable) -> Subscriber:
             _providers = [
                 *global_providers,
                 *self.providers,
                 *providers,
             ]
             _auxiliaries = [
+                *self.auxiliaries,
                 *auxiliaries,
             ]
             res = Subscriber(
                 exec_target,
                 priority=priority,
                 auxiliaries=_auxiliaries,
                 providers=_providers,
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/ref.py` & `arclet-letoderea-0.9.2/arclet/letoderea/ref.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/subscriber.py` & `arclet-letoderea-0.9.2/arclet/letoderea/subscriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         param = CompileParam(name, anno, default, [], None, None)
         for _provider in providers:
             if isinstance(_provider, ProviderFactory):
                 if result := _provider.validate(Param(name, anno, default, bool(param.providers))):
                     param.providers.append(result)
             elif _provider.validate(Param(name, anno, default, bool(param.providers))):
                 param.providers.append(_provider)
+        param.providers.sort(key=lambda x: x.priority)
         if get_origin(anno) is Annotated:
             org, *meta = get_args(anno)
             for m in reversed(meta):
                 if isinstance(m, Provider):
                     param.providers.insert(0, m)
                 elif isinstance(m, str):
                     param.providers.insert(0, provide(org, name, lambda x: x.get(m)))
@@ -107,15 +108,14 @@
         if hasattr(callable_target, "__providers__"):
             self.providers.extend(getattr(callable_target, "__providers__", []))
         for aux in auxiliaries:
             for scope in aux.scopes:
                 self.auxiliaries.setdefault(scope, []).append(aux)
         for scope, value in self.auxiliaries.items():
             self.auxiliaries[scope] = combine(value)  # type: ignore
-        self.providers.sort(key=lambda x: x.priority)
         self.params = _compile(callable_target, self.providers)
         if is_async(callable_target):
             self.callable_target = callable_target
         else:
             self.callable_target = run_sync(callable_target)
 
     async def __call__(self, *args, **kwargs) -> R:
```

### Comparing `arclet-letoderea-0.9.0/arclet/letoderea/typing.py` & `arclet-letoderea-0.9.2/arclet/letoderea/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/LICENSE` & `arclet-letoderea-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/pyproject.toml` & `arclet-letoderea-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-letoderea"
-version = "0.9.0"
+version = "0.9.2"
 description = "A high-performance, simple-structured event system, relies on asyncio"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "tarina>=0.3.0",
 ]
```

### Comparing `arclet-letoderea-0.9.0/README.md` & `arclet-letoderea-0.9.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,28 +39,29 @@
 ## 说明
 
 ### 事件
 
 - 事件可以是任何对象，只要实现了 `gather` 异步方法
 - `gather` 方法的参数为 `Contexts` 类型，用于传递上下文信息
 - 事件可以通过 `gather` 方法将自身想要传递的信息整合进 `Contexts` 中
-- 事件系统支持直接查找属性, 例如 `Event.name` 可以直接注入进 `foo(name: str)` 的参数中
 - 事件可以携带 `Provider` 与 `Auxiliary`，它们会在事件被订阅时注入到订阅者中
+- 订阅子类事件时，父类事件的 `Provider` 与 `Auxiliary` 会被继承
+- 订阅父类事件时，其子类事件也会被分发给订阅者
 
 ### 订阅
 
-- 通过 `EventSystem.on` 或 `subscribe` 装饰器可以将一个函数注册为事件的订阅者
+- 通过 `Publisher.register`, `EventSystem.on` 或 `subscribe` 装饰器可以将一个函数注册为事件的订阅者
 - 订阅者的参数可以是任何类型，事件系统会尝试从 `Contexts` 中查找对应的值并注入
 - 默认情况下 `event` 为名字的参数会被注入为事件的实例
 - 订阅者可以设置优先级，值越小优先级越高
 
 ### 上下文
 
-- `Contexts` 类型是一个 `dict` 的子类，用于传递上下文信息
-- `Contexts` 默认包含 `event` 键，其值为事件的实例
+- `Contexts` 类型是一个 `dict` 的子类，用于传递上下文信息，除此之外与 `dict` 没有区别
+- `Contexts` 默认包含 `$event` 键，其值为事件的实例
 - `Contexts` 默认包含 `$subscriber` 键，其值为订阅者的实例
 
 
 ### 依赖注入
 
 - `Provider[T]` 负责管理参数的注入, 其会尝试从 `Contexts` 中选择需求的参数返回
 - 对于订阅者的每个参数，在订阅者注册后，事件系统会遍历该订阅者拥有的所有 `Provider`，
@@ -70,23 +71,25 @@
 - `Provider.validate` 方法用于验证订阅函数的参数是否为该 `Provider` 可绑定的参数。默认实现为检查目标参数的类型声明是否为 `T`。
     也可以通过重写该方法来实现自定义的验证逻辑。
 - `Provider.__call__` 方法用于从 `Contexts` 中获取参数
 - 原则上 `Provider` 只负责注入单一类型的参数。若想处理多个类型的参数，可以声明自己为 `Provider[Union[A, B, ...]]` 类型，
     并在 `Provider.validate` 方法中进行自定义的逻辑判断。但更推荐的做法是构造多个 `Provider`，并将其绑定到同一个参数上。
 - 对于特殊的辅助器 `Depend`，事件系统会将其作为特殊的 `Provider` 处理，绑定了 `Depend` 的参数在解析时将直接调用
     `Depend.__call__` 方法。
+- `Provider` 可以设置优先级，值越小优先级越高
+- 另有 `ProviderFactory`，用于集成多个 `Provider` 的分配，以方便 `event.providers` 的设置
 
 ### 事件发布
 
 - 一般情况下通过 `EventSystem.publish` 方法可以发布一个事件让事件系统进行处理
 - `Publisher` 类负责管理订阅者与事件的交互
 - `Publisher.validate` 方法用于验证该事件是否为该发布者的订阅者所关注的事件
-- `Publisher.publish` 方法用于将事件不经过事件系统主动分发给订阅者
-- `Publisher.supply` 方法用于让事件系统主动获取事件并分发给订阅者
-- `EventSystem.on` 与 `EventSystem.publish` 可以指定 `Publisher`，默认为事件系统内的全局 `Publisher`
+- `Publisher.publish` 方法用于将事件直接分发给属于自身的订阅者
+- `Publisher.supply` 方法用于让事件系统主动获取事件并分发给所有订阅者
+- `EventSystem.on` 与 `EventSystem.publish` 可以指定 `Publisher`
 
 ### 辅助
 
 - `Auxiliary` 提供了一系列辅助方法，方便事件的处理
 - `Auxiliary` 分为 `Judge`, `Supply` 与 `Depend` 三类:
     - `Judge`: 用于判断此时是否应该处理事件
     - `Supply`: 用于为 `Contexts` 提供额外的信息
@@ -96,10 +99,11 @@
     - `parsing`: 表示该 `Auxiliary` 会在依赖注入解析时执行
     - `complete`: 表示该 `Auxiliary` 会在依赖注入完成后执行
     - `cleanup`: 表示该 `Auxiliary` 会在事件处理完成后执行
 - `Auxiliary` 可以设置 `CombineMode`, 用来设置多个 `Auxiliary` 的组合方式:
     - `single`: 表示该 `Auxiliary` 独立执行
     - `and`: 表示该 `Auxiliary` 的执行结果应该与其他 `Auxiliary` 的执行结果都为有效值
     - `or`: 表示该 `Auxiliary` 的执行结果应该与其他 `Auxiliary` 的执行结果至少有一个为有效值
+- `Auxiliary` 可以设置优先级，值越小优先级越高
 
 ## 开源协议
 本实现以 MIT 为开源协议。
```

### Comparing `arclet-letoderea-0.9.0/tests/annotated.py` & `arclet-letoderea-0.9.2/tests/annotated.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/breakpoint.py` & `arclet-letoderea-0.9.2/tests/breakpoint.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/breakpoint1.py` & `arclet-letoderea-0.9.2/tests/breakpoint1.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/combine.py` & `arclet-letoderea-0.9.2/tests/combine.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/condition.py` & `arclet-letoderea-0.9.2/tests/condition.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/decorator.py` & `arclet-letoderea-0.9.2/tests/decorator.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/depend.py` & `arclet-letoderea-0.9.2/tests/depend.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/except.py` & `arclet-letoderea-0.9.2/tests/except.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/nest_except.py` & `arclet-letoderea-0.9.2/tests/nest_except.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/shortcut.py` & `arclet-letoderea-0.9.2/tests/shortcut.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 
 from typing_extensions import Annotated
 
-from arclet.letoderea import EventSystem, bypass_if, is_event, subscribe
+from arclet.letoderea import EventSystem, bypass_if, subscribe
 from arclet.letoderea.ref import deref
 
 es = EventSystem()
 
 
 class TestEvent:
     type: str = "TestEvent"
```

### Comparing `arclet-letoderea-0.9.0/tests/test_handler.py` & `arclet-letoderea-0.9.2/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/test_param_parser.py` & `arclet-letoderea-0.9.2/tests/test_param_parser.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/test_provider_validate.py` & `arclet-letoderea-0.9.2/tests/test_provider_validate.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/tests/test_publisher.py` & `arclet-letoderea-0.9.2/tests/test_publisher.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.9.0/PKG-INFO` & `arclet-letoderea-0.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-letoderea
-Version: 0.9.0
+Version: 0.9.2
 Summary: A high-performance, simple-structured event system, relies on asyncio
 License: MIT
 Keywords: asyncio,event-system,dispatch,dependency-injection
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,28 +57,29 @@
 ## 说明
 
 ### 事件
 
 - 事件可以是任何对象，只要实现了 `gather` 异步方法
 - `gather` 方法的参数为 `Contexts` 类型，用于传递上下文信息
 - 事件可以通过 `gather` 方法将自身想要传递的信息整合进 `Contexts` 中
-- 事件系统支持直接查找属性, 例如 `Event.name` 可以直接注入进 `foo(name: str)` 的参数中
 - 事件可以携带 `Provider` 与 `Auxiliary`，它们会在事件被订阅时注入到订阅者中
+- 订阅子类事件时，父类事件的 `Provider` 与 `Auxiliary` 会被继承
+- 订阅父类事件时，其子类事件也会被分发给订阅者
 
 ### 订阅
 
-- 通过 `EventSystem.on` 或 `subscribe` 装饰器可以将一个函数注册为事件的订阅者
+- 通过 `Publisher.register`, `EventSystem.on` 或 `subscribe` 装饰器可以将一个函数注册为事件的订阅者
 - 订阅者的参数可以是任何类型，事件系统会尝试从 `Contexts` 中查找对应的值并注入
 - 默认情况下 `event` 为名字的参数会被注入为事件的实例
 - 订阅者可以设置优先级，值越小优先级越高
 
 ### 上下文
 
-- `Contexts` 类型是一个 `dict` 的子类，用于传递上下文信息
-- `Contexts` 默认包含 `event` 键，其值为事件的实例
+- `Contexts` 类型是一个 `dict` 的子类，用于传递上下文信息，除此之外与 `dict` 没有区别
+- `Contexts` 默认包含 `$event` 键，其值为事件的实例
 - `Contexts` 默认包含 `$subscriber` 键，其值为订阅者的实例
 
 
 ### 依赖注入
 
 - `Provider[T]` 负责管理参数的注入, 其会尝试从 `Contexts` 中选择需求的参数返回
 - 对于订阅者的每个参数，在订阅者注册后，事件系统会遍历该订阅者拥有的所有 `Provider`，
@@ -88,23 +89,25 @@
 - `Provider.validate` 方法用于验证订阅函数的参数是否为该 `Provider` 可绑定的参数。默认实现为检查目标参数的类型声明是否为 `T`。
     也可以通过重写该方法来实现自定义的验证逻辑。
 - `Provider.__call__` 方法用于从 `Contexts` 中获取参数
 - 原则上 `Provider` 只负责注入单一类型的参数。若想处理多个类型的参数，可以声明自己为 `Provider[Union[A, B, ...]]` 类型，
     并在 `Provider.validate` 方法中进行自定义的逻辑判断。但更推荐的做法是构造多个 `Provider`，并将其绑定到同一个参数上。
 - 对于特殊的辅助器 `Depend`，事件系统会将其作为特殊的 `Provider` 处理，绑定了 `Depend` 的参数在解析时将直接调用
     `Depend.__call__` 方法。
+- `Provider` 可以设置优先级，值越小优先级越高
+- 另有 `ProviderFactory`，用于集成多个 `Provider` 的分配，以方便 `event.providers` 的设置
 
 ### 事件发布
 
 - 一般情况下通过 `EventSystem.publish` 方法可以发布一个事件让事件系统进行处理
 - `Publisher` 类负责管理订阅者与事件的交互
 - `Publisher.validate` 方法用于验证该事件是否为该发布者的订阅者所关注的事件
-- `Publisher.publish` 方法用于将事件不经过事件系统主动分发给订阅者
-- `Publisher.supply` 方法用于让事件系统主动获取事件并分发给订阅者
-- `EventSystem.on` 与 `EventSystem.publish` 可以指定 `Publisher`，默认为事件系统内的全局 `Publisher`
+- `Publisher.publish` 方法用于将事件直接分发给属于自身的订阅者
+- `Publisher.supply` 方法用于让事件系统主动获取事件并分发给所有订阅者
+- `EventSystem.on` 与 `EventSystem.publish` 可以指定 `Publisher`
 
 ### 辅助
 
 - `Auxiliary` 提供了一系列辅助方法，方便事件的处理
 - `Auxiliary` 分为 `Judge`, `Supply` 与 `Depend` 三类:
     - `Judge`: 用于判断此时是否应该处理事件
     - `Supply`: 用于为 `Contexts` 提供额外的信息
@@ -114,11 +117,12 @@
     - `parsing`: 表示该 `Auxiliary` 会在依赖注入解析时执行
     - `complete`: 表示该 `Auxiliary` 会在依赖注入完成后执行
     - `cleanup`: 表示该 `Auxiliary` 会在事件处理完成后执行
 - `Auxiliary` 可以设置 `CombineMode`, 用来设置多个 `Auxiliary` 的组合方式:
     - `single`: 表示该 `Auxiliary` 独立执行
     - `and`: 表示该 `Auxiliary` 的执行结果应该与其他 `Auxiliary` 的执行结果都为有效值
     - `or`: 表示该 `Auxiliary` 的执行结果应该与其他 `Auxiliary` 的执行结果至少有一个为有效值
+- `Auxiliary` 可以设置优先级，值越小优先级越高
 
 ## 开源协议
 本实现以 MIT 为开源协议。
```

