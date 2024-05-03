# Comparing `tmp/imbue-1.0.0.tar.gz` & `tmp/imbue-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbue-1.0.0.tar", max compression
+gzip compressed data, was "imbue-2.0.0.tar", max compression
```

## Comparing `imbue-1.0.0.tar` & `imbue-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2024-04-10 17:52:04.806052 imbue-1.0.0/LICENSE
--rw-r--r--   0        0        0     5047 2024-04-10 17:52:04.806052 imbue-1.0.0/README.md
--rw-r--r--   0        0        0      565 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/__init__.py
--rw-r--r--   0        0        0      786 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/abc.py
--rw-r--r--   0        0        0     5928 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/container.py
--rw-r--r--   0        0        0        0 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/__init__.py
--rw-r--r--   0        0        0     3046 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/abc.py
--rw-r--r--   0        0        0     1782 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/application.py
--rw-r--r--   0        0        0     4199 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/base.py
--rw-r--r--   0        0        0      461 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/factory.py
--rw-r--r--   0        0        0      587 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/task.py
--rw-r--r--   0        0        0     1188 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/contexts/thread.py
--rw-r--r--   0        0        0     1237 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/dependency.py
--rw-r--r--   0        0        0      288 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/exceptions.py
--rw-r--r--   0        0        0      964 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/package.py
--rw-r--r--   0        0        0        0 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/__init__.py
--rw-r--r--   0        0        0      967 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/abc.py
--rw-r--r--   0        0        0     1728 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/common.py
--rw-r--r--   0        0        0     2036 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/function.py
--rw-r--r--   0        0        0     3333 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/providers/instance.py
--rw-r--r--   0        0        0        0 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/py.typed
--rw-r--r--   0        0        0     4172 2024-04-10 17:52:04.806052 imbue-1.0.0/imbue/utils.py
--rw-r--r--   0        0        0      870 2024-04-10 17:52:04.806052 imbue-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5738 1970-01-01 00:00:00.000000 imbue-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 09:12:37.480893 imbue-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5273 2024-05-03 09:12:37.480893 imbue-2.0.0/README.md
+-rw-r--r--   0        0        0      565 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/__init__.py
+-rw-r--r--   0        0        0      786 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/abc.py
+-rw-r--r--   0        0        0     6735 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/container.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/__init__.py
+-rw-r--r--   0        0        0     3089 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/abc.py
+-rw-r--r--   0        0        0     1782 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/application.py
+-rw-r--r--   0        0        0     4213 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/base.py
+-rw-r--r--   0        0        0      461 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/factory.py
+-rw-r--r--   0        0        0      587 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/task.py
+-rw-r--r--   0        0        0     1188 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/contexts/thread.py
+-rw-r--r--   0        0        0     1237 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/dependency.py
+-rw-r--r--   0        0        0      288 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/exceptions.py
+-rw-r--r--   0        0        0     1209 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/package.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/providers/__init__.py
+-rw-r--r--   0        0        0      966 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/providers/abc.py
+-rw-r--r--   0        0        0     1728 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/providers/common.py
+-rw-r--r--   0        0        0     2036 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/providers/function.py
+-rw-r--r--   0        0        0     3333 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/providers/instance.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/py.typed
+-rw-r--r--   0        0        0     4172 2024-05-03 09:12:37.480893 imbue-2.0.0/imbue/utils.py
+-rw-r--r--   0        0        0      871 2024-05-03 09:12:37.480893 imbue-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5964 1970-01-01 00:00:00.000000 imbue-2.0.0/PKG-INFO
```

### Comparing `imbue-1.0.0/LICENSE` & `imbue-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/README.md` & `imbue-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,17 +43,19 @@
 container = Container(
     APkg(...),  # Packages would typically be passed config.
     ContextualizedDependency(ADep, Context.THREAD, eager=True),
 )
 
 ...
 
+# The application context should be entered through the framework initialization.
 async with container.application_context() as app_container:
     a_dep = await app_container.get(ADep)
     ...
+    # The task context should be entered in each request.
     async with app_container.task_context() as task_container:
         b_dep = await task_container.get(BDep)
 ```
 
 > 💡 A dependency can require other dependencies, the container will resolve the graph and raise errors if circular dependencies are found.
 
 ### In the details
@@ -63,45 +65,45 @@
 This might be because dependencies depend on config and other reasons.
 You can use the `Package` class:
 ```python
 from typing import AsyncIterator
 
 from imbue import Package, application_context
 
-from myapp import LoggingConfig, LoggerTransportInterface, LoggerTransport, LoggerInterface, Logger
+from myapp import LoggingConfig, MyLoggerTransport, LoggerTransport, MyLogger, Logger
 
 class LoggingPackage(Package):
     def __init__(self, config: LoggingConfig):
         self._config = config
         
     @application_context(eager=True)  # You can autoload dependencies.
     # The method should expose the interface as the type and return the implementation.
-    def logger_transport(self) -> LoggerTransportInterface:
-        return LoggerTransport(self._config.transport)
+    def logger_transport(self) -> LoggerTransport:
+        return MyLoggerTransport(self._config.transport)
 
     @application_context
     # Sub dependencies should be required through their interface.
-    async def logger(self, transport: LoggerTransportInterface) -> AsyncIterator[LoggerInterface]:
+    async def logger(self, transport: LoggerTransport) -> AsyncIterator[Logger]:
         # Package methods also allow you to handle context managers.
-        async with Logger(transport, self._config.logger) as logger:
+        async with MyLogger(transport, self._config.logger) as logger:
+            # Using generators allow cleaning up resources when the context closes.
             yield logger
 ```
 
 ##### Declaring dependencies
 It's done via methods that can be:
 - functions
 - async functions
 - generators
 - async generators
 
 To declare the method returns a dependency, you simply choose the appropriate context and add the context decorator on the method.
 
 > 💡 Eager dependencies are instantiated as soon as we enter their context.
-> This is useful to configure globals (the transport in this example)
-> or if we want to make sure a dependency will use the main thread's event loop.
+> This is useful if we want to make sure a dependency will use the main thread's event loop.
 
 ##### Cleaning resources
 When you need to close resources you can do so via a generator.
 The generator should yield the dependency.
 
 > 💡 You should watch out for errors, if the context is closed handling an error, it will be raised in the generator.
 
@@ -116,8 +118,10 @@
     # You can also this to control context and eagerness.
     ContextualizedDependency(CDep, Context.THREAD, eager=True),
     ...,
 )
 ```
 or if you want to include them in a `Package`, add them in `EXTRA_DEPENDENCIES`.
 
-> 💡 By default their context will be at the task level, which can be changed if needed.
+> 💡 Whatever the method of adding dependencies,
+> non-contextualized ones will have the context automatically set based on sub-dependencies.
+> The lowest possible context will be used.
```

### Comparing `imbue-1.0.0/imbue/__init__.py` & `imbue-2.0.0/imbue/__init__.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/abc.py` & `imbue-2.0.0/imbue/abc.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/container.py` & `imbue-2.0.0/imbue/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Dict, Iterator, List, Union
+from typing import Dict, Iterator, List, Union, cast
 
 from imbue.abc import InternalContainer
 from imbue.contexts.application import ApplicationContainer
 from imbue.contexts.base import (
     Context,
     ContextualizedDependency,
     ContextualizedProvider,
@@ -24,19 +24,28 @@
 
     def add(self, provider: ContextualizedProvider) -> "DependencyChain":
         """Create a new chain, adding the provider at the end."""
         chain = DependencyChain([*self.chain, provider])
         # Check for cycles.
         if provider in self.chain:
             raise DependencyResolutionError(f"circular dependency found:\n{chain}")
+        return chain
+
+    def check(self) -> None:
+        if self.last.context is None:
+            raise DependencyResolutionError(
+                f"provider {self.last} does not have a context set"
+            )
+        # If previous context is not set, it will be done automatically so no check is required.
+        if len(self.chain) < 2 or self.chain[-2].context is None:
+            return
         # The deeper the chain, the lower the context must be.
         # App dependencies cannot have task dependencies but the inverse is possible.
-        if provider.context > self.last.context:
-            raise DependencyResolutionError(f"context error:\n{chain}")
-        return chain
+        if self.last.context > self.chain[-2].context:
+            raise DependencyResolutionError(f"context error:\n{self}")
 
     @property
     def last(self) -> ContextualizedProvider:
         """Get the last provider in the chain."""
         return self.chain[-1]
 
     def __str__(self) -> str:
@@ -48,15 +57,14 @@
         )
 
 
 class Container(InternalContainer):
     def __init__(
         self,
         *dependencies_or_packages: Union[Dependency, ContextualizedDependency, Package],
-        default_dependency_context: Context = Context.TASK,
     ):
         # The link between an interface and its provider.
         self._providers: Dict[Interface, ContextualizedProvider] = {}
         # Cache sub dependencies for each interface.
         self._sub_dependencies: Dict[Interface, List[SubDependency]] = {}
         # All providers that should be eager inited.
         self._by_context_eager_providers: Dict[
@@ -66,17 +74,15 @@
         )
 
         # Add all dependencies.
         for dep_or_pkg in dependencies_or_packages:
             if isinstance(dep_or_pkg, (ContextualizedDependency, Package)):
                 providers_iterator = dep_or_pkg.get_providers()
             else:
-                providers_iterator = ContextualizedProvider.from_dependency(
-                    dep_or_pkg, default_dependency_context
-                )
+                providers_iterator = ContextualizedProvider.from_dependency(dep_or_pkg)
             for provider in providers_iterator:
                 if provider.interface in self._providers:
                     raise DependencyResolutionError(
                         "multiple providers found for the same type: "
                         f"{self._providers[provider.interface]!r}, {provider!r}",
                     )
                 self._providers[provider.interface] = provider
@@ -84,30 +90,42 @@
         for provider in self._providers.values():
             self._resolve(DependencyChain([provider]))
 
     def _resolve(self, chain: DependencyChain) -> None:
         """Construct the graph of sub dependencies."""
         provider = chain.last
         if provider.interface in self._sub_dependencies:
-            # Already handled.
+            # Already handled, we just need to check the full chain.
+            chain.check()
             return
         dependencies: List[SubDependency] = []
+        sub_providers: List[ContextualizedProvider] = []
         for sub_dependency in provider.sub_dependencies:
             if (
                 not sub_dependency.mandatory
                 and sub_dependency.interface not in self._providers
             ):
                 continue
             if sub_dependency.interface not in self._providers:
                 raise DependencyResolutionError(
                     f"no provider found for {sub_dependency.interface}, from provider {provider!r}",
                 )
             sub_provider = self._providers[sub_dependency.interface]
+            sub_providers.append(sub_provider)
             self._resolve(chain.add(sub_provider))
             dependencies.append(sub_dependency)
+        # Set the context automatically based on dependencies if not set.
+        # We want to set the lowest context possible.
+        if provider.context is None:
+            provider.context = (
+                max(cast(Context, s.context) for s in sub_providers)
+                if sub_providers
+                else Context.APPLICATION
+            )
+        chain.check()
         self._sub_dependencies[provider.interface] = dependencies
         if provider.eager:
             self._by_context_eager_providers[provider.context].append(provider)
 
     def add(self, dependency: Dependency, context: Context = Context.TASK) -> None:
         """Add another interface, used to eagerly add all task functions/methods as providers.
         This allows to make all necessary checks at application start rather than during task processing.
```

### Comparing `imbue-1.0.0/imbue/contexts/abc.py` & `imbue-2.0.0/imbue/contexts/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 from contextlib import (
     AbstractAsyncContextManager,
     AbstractContextManager,
     AsyncExitStack,
 )
-from typing import Any, Callable, ClassVar, Dict, Type, TypeVar, overload
+from typing import Any, Callable, ClassVar, Dict, Type, TypeVar, cast, overload
 
 from imbue.abc import InternalContainer
 from imbue.contexts.base import Context, ContextualizedProvider
 from imbue.dependency import Interface
 from imbue.providers.instance import DelegatedInstanceProvider
 
 V = TypeVar("V")
@@ -39,15 +39,17 @@
     @overload
     async def get(self, interface: Callable) -> Callable:
         """Specific type annotation for functions."""
 
     async def get(self, interface: Interface) -> Any:
         """Find the proper container based on context and provide."""
         provider = self._container.get_provider(interface)
-        return await self._contextualized[provider.context]._get_or_provide(provider)
+        return await self._contextualized[
+            cast(Context, provider.context)
+        ]._get_or_provide(provider)
 
     async def _get_or_provide(self, provider: ContextualizedProvider) -> Any:
         """Get from already provided or provide the dependency."""
         if provided := self._provided.get(provider.interface):
             return provided
         provided = await self._provide(provider)
         self._provided[provider.interface] = provided
```

### Comparing `imbue-1.0.0/imbue/contexts/application.py` & `imbue-2.0.0/imbue/contexts/application.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/contexts/base.py` & `imbue-2.0.0/imbue/contexts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 T = TypeVar("T")
 V = TypeVar("V")
 
 
 @dataclass
 class ContextualizedDependency:
     dependency: Dependency
-    context: Context = Context.TASK
+    context: Optional[Context] = None
     eager: bool = False
 
     def get_providers(self) -> Iterator[ContextualizedProvider]:
         yield from ContextualizedProvider.from_dependency(
             self.dependency,
             self.context,
             self.eager,
@@ -54,22 +54,22 @@
 
 
 @dataclass
 class ContextualizedProvider(Generic[T, V]):
     """Wrap a provider to handle context and lifetime."""
 
     provider: Provider[T, V]
-    context: Context
+    context: Optional[Context]
     eager: bool
 
     @classmethod
     def from_dependency(
         cls,
         dependency: Dependency,
-        context: Context = Context.TASK,
+        context: Optional[Context] = None,
         eager: bool = False,
     ) -> Iterator["ContextualizedProvider"]:
         """In some cases, an interface yields multiple providers.
         Ex: a method yields a provider for a class and one for the method.
         """
         for provider in get_providers(dependency):
             yield cls(
```

### Comparing `imbue-1.0.0/imbue/contexts/task.py` & `imbue-2.0.0/imbue/contexts/task.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/contexts/thread.py` & `imbue-2.0.0/imbue/contexts/thread.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/dependency.py` & `imbue-2.0.0/imbue/dependency.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/package.py` & `imbue-2.0.0/imbue/package.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import inspect
-from typing import ClassVar, Iterable, Iterator
+from typing import ClassVar, Iterable, Iterator, Union
 
 from imbue.contexts.base import (
     ContextualizedDependency,
     ContextualizedProvider,
     DelegatedProviderWrapper,
 )
+from imbue.dependency import Dependency
 
 
 class Package:
     """Container class to group dependency providers.
     Each dependency is provided by a method.
     Additionally, you can specify dependencies for which no
     provider function is required in `EXTRA_DEPENDENCIES`.
     """
 
-    EXTRA_DEPENDENCIES: ClassVar[Iterable[ContextualizedDependency]] = ()
+    EXTRA_DEPENDENCIES: ClassVar[
+        Iterable[Union[Dependency, ContextualizedDependency]]
+    ] = ()
 
     def get_providers(self) -> Iterator[ContextualizedProvider]:
         for dependency in self.EXTRA_DEPENDENCIES:
-            yield from dependency.get_providers()
+            if isinstance(dependency, ContextualizedDependency):
+                yield from dependency.get_providers()
+            else:
+                yield from ContextualizedProvider.from_dependency(dependency)
         for _, member in inspect.getmembers(self):
             if not isinstance(member, DelegatedProviderWrapper):
                 continue
             # Now that we have an instance to bind, we can get the final provider.
             yield member.to_contextualized_provider(instance=self)
```

### Comparing `imbue-1.0.0/imbue/providers/abc.py` & `imbue-2.0.0/imbue/providers/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 T = TypeVar("T")
 V = TypeVar("V")
 
 
 class Provider(Generic[T, V], ABC):
     """The foundation of dependency injection.
-    The role of the provider is to expose sub dependencies and provide the depdendencies given sub dependencies.
+    The role of the provider is to expose sub dependencies and provide the dependencies given sub dependencies.
     """
 
     def __init__(self, interface: T):
         self.interface: T = interface
 
     @property
     @abstractmethod
```

### Comparing `imbue-1.0.0/imbue/providers/common.py` & `imbue-2.0.0/imbue/providers/common.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/providers/function.py` & `imbue-2.0.0/imbue/providers/function.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/providers/instance.py` & `imbue-2.0.0/imbue/providers/instance.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/imbue/utils.py` & `imbue-2.0.0/imbue/utils.py`

 * *Files identical despite different names*

### Comparing `imbue-1.0.0/pyproject.toml` & `imbue-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "imbue"
-version = "1.0.0"
+version = "2.0.0"
 description = "Type based python dependency injection framework."
 authors = ["Gabriel Pajot <gab@lescactus.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/imbue"
 include = ["imbue/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
 [tool.poetry.group.test.dependencies]
-pytest = "==8.0.2"
-pytest-asyncio = "==0.23.5"
-pytest-mock = "==3.12.0"
-ruff = "==0.3.2"
-mypy = "==1.8.0"
+pytest = "==8.2.0"
+pytest-asyncio = "==0.23.6"
+pytest-mock = "==3.14.0"
+ruff = "==0.4.2"
+mypy = "==1.10.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `imbue-1.0.0/PKG-INFO` & `imbue-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imbue
-Version: 1.0.0
+Version: 2.0.0
 Summary: Type based python dependency injection framework.
 Home-page: https://github.com/gpajot/imbue
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@lescactus.eu
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -62,17 +62,19 @@
 container = Container(
     APkg(...),  # Packages would typically be passed config.
     ContextualizedDependency(ADep, Context.THREAD, eager=True),
 )
 
 ...
 
+# The application context should be entered through the framework initialization.
 async with container.application_context() as app_container:
     a_dep = await app_container.get(ADep)
     ...
+    # The task context should be entered in each request.
     async with app_container.task_context() as task_container:
         b_dep = await task_container.get(BDep)
 ```
 
 > 💡 A dependency can require other dependencies, the container will resolve the graph and raise errors if circular dependencies are found.
 
 ### In the details
@@ -82,45 +84,45 @@
 This might be because dependencies depend on config and other reasons.
 You can use the `Package` class:
 ```python
 from typing import AsyncIterator
 
 from imbue import Package, application_context
 
-from myapp import LoggingConfig, LoggerTransportInterface, LoggerTransport, LoggerInterface, Logger
+from myapp import LoggingConfig, MyLoggerTransport, LoggerTransport, MyLogger, Logger
 
 class LoggingPackage(Package):
     def __init__(self, config: LoggingConfig):
         self._config = config
         
     @application_context(eager=True)  # You can autoload dependencies.
     # The method should expose the interface as the type and return the implementation.
-    def logger_transport(self) -> LoggerTransportInterface:
-        return LoggerTransport(self._config.transport)
+    def logger_transport(self) -> LoggerTransport:
+        return MyLoggerTransport(self._config.transport)
 
     @application_context
     # Sub dependencies should be required through their interface.
-    async def logger(self, transport: LoggerTransportInterface) -> AsyncIterator[LoggerInterface]:
+    async def logger(self, transport: LoggerTransport) -> AsyncIterator[Logger]:
         # Package methods also allow you to handle context managers.
-        async with Logger(transport, self._config.logger) as logger:
+        async with MyLogger(transport, self._config.logger) as logger:
+            # Using generators allow cleaning up resources when the context closes.
             yield logger
 ```
 
 ##### Declaring dependencies
 It's done via methods that can be:
 - functions
 - async functions
 - generators
 - async generators
 
 To declare the method returns a dependency, you simply choose the appropriate context and add the context decorator on the method.
 
 > 💡 Eager dependencies are instantiated as soon as we enter their context.
-> This is useful to configure globals (the transport in this example)
-> or if we want to make sure a dependency will use the main thread's event loop.
+> This is useful if we want to make sure a dependency will use the main thread's event loop.
 
 ##### Cleaning resources
 When you need to close resources you can do so via a generator.
 The generator should yield the dependency.
 
 > 💡 You should watch out for errors, if the context is closed handling an error, it will be raised in the generator.
 
@@ -135,9 +137,11 @@
     # You can also this to control context and eagerness.
     ContextualizedDependency(CDep, Context.THREAD, eager=True),
     ...,
 )
 ```
 or if you want to include them in a `Package`, add them in `EXTRA_DEPENDENCIES`.
 
-> 💡 By default their context will be at the task level, which can be changed if needed.
+> 💡 Whatever the method of adding dependencies,
+> non-contextualized ones will have the context automatically set based on sub-dependencies.
+> The lowest possible context will be used.
```

