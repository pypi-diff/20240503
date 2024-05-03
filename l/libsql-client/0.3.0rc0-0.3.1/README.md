# Comparing `tmp/libsql_client-0.3.0rc0.tar.gz` & `tmp/libsql_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsql_client-0.3.0rc0.tar", max compression
+gzip compressed data, was "libsql_client-0.3.1.tar", max compression
```

## Comparing `libsql_client-0.3.0rc0.tar` & `libsql_client-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-05-04 20:47:51.106565 libsql_client-0.3.0rc0/LICENSE.md
--rw-r--r--   0        0        0     2912 2023-05-04 20:47:51.106814 libsql_client-0.3.0rc0/README.md
--rw-r--r--   0        0        0      268 2023-05-04 20:47:51.108622 libsql_client-0.3.0rc0/libsql_client/__init__.py
--rw-r--r--   0        0        0     3215 2023-05-22 13:09:47.355780 libsql_client-0.3.0rc0/libsql_client/client.py
--rw-r--r--   0        0        0      993 2023-05-04 20:47:51.108918 libsql_client-0.3.0rc0/libsql_client/config.py
--rw-r--r--   0        0        0      801 2023-05-04 20:47:51.109050 libsql_client-0.3.0rc0/libsql_client/create_client.py
--rw-r--r--   0        0        0     2986 2023-05-24 18:03:12.709676 libsql_client-0.3.0rc0/libsql_client/dbapi2/__init__.py
--rw-r--r--   0        0        0      839 2023-05-24 18:03:12.710251 libsql_client-0.3.0rc0/libsql_client/dbapi2/__main__.py
--rw-r--r--   0        0        0     6335 2023-05-24 18:03:12.711562 libsql_client-0.3.0rc0/libsql_client/dbapi2/_async_executor.py
--rw-r--r--   0        0        0    13537 2023-05-24 18:03:12.712336 libsql_client-0.3.0rc0/libsql_client/dbapi2/_reexports.py
--rw-r--r--   0        0        0       41 2023-05-24 18:03:12.712831 libsql_client-0.3.0rc0/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/__init__.py
--rw-r--r--   0        0        0      661 2023-05-24 18:03:12.713309 libsql_client-0.3.0rc0/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/dbapi2.py
--rw-r--r--   0        0        0     6261 2023-05-24 18:03:12.713933 libsql_client-0.3.0rc0/libsql_client/dbapi2/_utils.py
--rw-r--r--   0        0        0    12432 2023-05-24 18:03:12.714427 libsql_client-0.3.0rc0/libsql_client/dbapi2/hrana.py
--rw-r--r--   0        0        0    48342 2023-05-24 18:03:12.715290 libsql_client-0.3.0rc0/libsql_client/dbapi2/types.py
--rw-r--r--   0        0        0       85 2023-05-04 20:47:51.109237 libsql_client-0.3.0rc0/libsql_client/hrana/__init__.py
--rw-r--r--   0        0        0     4261 2023-05-22 14:41:16.889969 libsql_client-0.3.0rc0/libsql_client/hrana/client.py
--rw-r--r--   0        0        0    14518 2023-05-22 14:41:16.890806 libsql_client-0.3.0rc0/libsql_client/hrana/conn.py
--rw-r--r--   0        0        0     4853 2023-05-22 13:09:47.357397 libsql_client-0.3.0rc0/libsql_client/hrana/convert.py
--rw-r--r--   0        0        0     1610 2023-05-04 20:47:51.109936 libsql_client-0.3.0rc0/libsql_client/hrana/id_alloc.py
--rw-r--r--   0        0        0     4988 2023-05-22 14:41:16.891594 libsql_client-0.3.0rc0/libsql_client/hrana/proto.py
--rw-r--r--   0        0        0     3631 2023-05-22 14:41:16.892225 libsql_client-0.3.0rc0/libsql_client/http.py
--rw-r--r--   0        0        0     3071 2023-05-04 20:47:51.110394 libsql_client-0.3.0rc0/libsql_client/result.py
--rw-r--r--   0        0        0     4896 2023-05-22 13:09:47.358497 libsql_client-0.3.0rc0/libsql_client/sqlite3.py
--rw-r--r--   0        0        0     7175 2023-05-22 13:09:47.358757 libsql_client-0.3.0rc0/libsql_client/sync.py
--rw-r--r--   0        0        0     1009 2023-05-25 14:16:00.085239 libsql_client-0.3.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 libsql_client-0.3.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-03 09:28:41.329891 libsql_client-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     3059 2024-05-03 09:28:41.330039 libsql_client-0.3.1/README.md
+-rw-r--r--   0        0        0      429 2024-05-03 09:28:41.332462 libsql_client-0.3.1/libsql_client/__init__.py
+-rw-r--r--   0        0        0     3564 2024-05-03 09:28:41.332605 libsql_client-0.3.1/libsql_client/client.py
+-rw-r--r--   0        0        0     1992 2024-05-03 09:28:41.332744 libsql_client-0.3.1/libsql_client/config.py
+-rw-r--r--   0        0        0      956 2024-05-03 09:28:41.332872 libsql_client-0.3.1/libsql_client/create_client.py
+-rw-r--r--   0        0        0     3081 2024-05-03 09:28:41.333231 libsql_client-0.3.1/libsql_client/dbapi2/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-03 09:28:41.333492 libsql_client-0.3.1/libsql_client/dbapi2/__main__.py
+-rw-r--r--   0        0        0     6460 2024-05-03 09:28:41.333654 libsql_client-0.3.1/libsql_client/dbapi2/_async_executor.py
+-rw-r--r--   0        0        0    17537 2024-05-03 09:28:41.333825 libsql_client-0.3.1/libsql_client/dbapi2/_reexports.py
+-rw-r--r--   0        0        0       41 2024-05-03 09:28:41.334625 libsql_client-0.3.1/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/__init__.py
+-rw-r--r--   0        0        0      662 2024-05-03 09:28:41.334744 libsql_client-0.3.1/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/dbapi2.py
+-rw-r--r--   0        0        0     6301 2024-05-03 09:28:41.334923 libsql_client-0.3.1/libsql_client/dbapi2/_utils.py
+-rw-r--r--   0        0        0    13069 2024-05-03 09:28:41.335253 libsql_client-0.3.1/libsql_client/dbapi2/hrana.py
+-rw-r--r--   0        0        0    48617 2024-05-03 09:28:41.335546 libsql_client-0.3.1/libsql_client/dbapi2/types.py
+-rw-r--r--   0        0        0      142 2024-05-03 09:28:41.335758 libsql_client-0.3.1/libsql_client/hrana/__init__.py
+-rw-r--r--   0        0        0     5031 2024-05-03 09:28:41.335913 libsql_client-0.3.1/libsql_client/hrana/client.py
+-rw-r--r--   0        0        0    15263 2024-05-03 09:28:41.336095 libsql_client-0.3.1/libsql_client/hrana/conn.py
+-rw-r--r--   0        0        0     5312 2024-05-03 09:28:41.336246 libsql_client-0.3.1/libsql_client/hrana/convert.py
+-rw-r--r--   0        0        0     1651 2024-05-03 09:28:41.336361 libsql_client-0.3.1/libsql_client/hrana/id_alloc.py
+-rw-r--r--   0        0        0     5776 2024-05-03 09:28:41.336510 libsql_client-0.3.1/libsql_client/hrana/proto.py
+-rw-r--r--   0        0        0     4391 2024-05-03 09:28:41.336677 libsql_client-0.3.1/libsql_client/http.py
+-rw-r--r--   0        0        0     3243 2024-05-03 09:28:41.336796 libsql_client-0.3.1/libsql_client/result.py
+-rw-r--r--   0        0        0     5094 2024-05-03 09:28:41.336948 libsql_client-0.3.1/libsql_client/sqlite3_utils.py
+-rw-r--r--   0        0        0     7506 2024-05-03 09:28:41.337085 libsql_client-0.3.1/libsql_client/sync.py
+-rw-r--r--   0        0        0     1607 2024-05-03 09:29:17.123176 libsql_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 libsql_client-0.3.1/PKG-INFO
```

### Comparing `libsql_client-0.3.0rc0/LICENSE.md` & `libsql_client-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libsql_client-0.3.0rc0/README.md` & `libsql_client-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 [reference]: https://libsql.org/libsql-client-py/reference.html
 [github]: https://github.com/libsql/libsql-client-py
 [pypi]: https://pypi.org/project/libsql-client/
 
 This is the source repository of the Python SDK for libSQL. You can either connect to a local SQLite database or to a remote libSQL server ([sqld][sqld]).
 
+> **_NOTE:_**  If you want to use libSQL with SQLAlchemy, you should check out the [libSQL dialect](https://github.com/libsql/sqlalchemy-libsql).
+
 [sqld]: https://github.com/libsql/sqld
 
 ## Installation
 
 ```
 pip install libsql-client
 ```
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/client.py` & `libsql_client-0.3.1/libsql_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,137 @@
 from __future__ import annotations
-from abc import ABC, abstractmethod
-from collections.abc import Sequence
+
+from abc import ABC
+from abc import abstractmethod
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple, TypeVar, Union
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Tuple
+from typing import TYPE_CHECKING
+from typing import TypeVar
+from typing import Union
 
-from .result import ResultSet, Value
+from .result import ResultSet
+from .result import Value
 
 if TYPE_CHECKING:
     from _typeshed import ReadableBuffer
 else:
     ReadableBuffer = bytes
 
 InValue = Union[Value, bool, datetime, ReadableBuffer]
 InArgs = Union[List[InValue], Tuple[InValue, ...], Dict[str, InValue], None]
 InStatement = Union["Statement", str, Tuple[str], Tuple[str, InArgs]]
 
+
 class Statement:
     sql: str
     args: InArgs
 
     def __init__(self, sql: str, args: InArgs = None):
         self.sql = sql
         self.args = args
 
     @staticmethod
     def convert(stmt: InStatement, args: InArgs = None) -> Statement:
         if isinstance(stmt, tuple):
             if len(stmt) == 1:
                 return Statement(stmt[0], args)
             if len(stmt) > 2:
-                raise TypeError(f"Statement must be a 1-tuple or 2-tuple, but got a {len(stmt)}-tuple")
+                raise TypeError(
+                    "Statement must be a 1-tuple or 2-tuple, "
+                    f"but got a {len(stmt)}-tuple"
+                )
             if args:
-                raise TypeError("Cannot pass additional args to a statement passed as tuple")
-            return Statement(stmt[0], stmt[1]) # type: ignore[misc]
+                raise TypeError(
+                    "Cannot pass additional args to a statement passed as tuple"
+                )
+            return Statement(stmt[0], stmt[1])  # type: ignore[misc]
         if isinstance(stmt, Statement):
             if args:
                 raise TypeError("Cannot pass additional args to a Statement instance")
             return stmt
         return Statement(stmt, args)
 
+
 class LibsqlError(RuntimeError):
     code: str
+    explanation: str
 
     def __init__(self, message: str, code: str):
         super(RuntimeError, self).__init__(f"{code}: {message}")
         self.code = code
+        self.explanation = message
+
 
 TClient = TypeVar("TClient", bound="Client")
 
+
 class Client(ABC):
     @abstractmethod
-    async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet: pass
+    async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
+        pass
 
     @abstractmethod
-    async def batch(self, stmts: List[InStatement]) -> List[ResultSet]: pass
+    async def batch(self, stmts: List[InStatement]) -> List[ResultSet]:
+        pass
 
     @abstractmethod
-    def transaction(self) -> Transaction: pass
+    def transaction(self) -> Transaction:
+        pass
 
     @abstractmethod
-    async def close(self) -> None: pass
+    async def close(self) -> None:
+        pass
 
     @property
     @abstractmethod
-    def closed(self) -> bool: pass
+    def closed(self) -> bool:
+        pass
 
     async def __aenter__(self: TClient) -> TClient:
         return self
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         await self.close()
 
+
 TTransaction = TypeVar("TTransaction", bound="Transaction")
 
+
 class Transaction(ABC):
     @abstractmethod
-    async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet: ...
+    async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
+        ...
 
     @abstractmethod
-    async def rollback(self) -> None: ...
+    async def rollback(self) -> None:
+        ...
 
     @abstractmethod
-    async def commit(self) -> None: ...
+    async def commit(self) -> None:
+        ...
 
     @abstractmethod
-    def close(self) -> None: ...
+    def close(self) -> None:
+        ...
 
     @property
     @abstractmethod
-    def closed(self) -> bool: ...
+    def closed(self) -> bool:
+        ...
 
     def __enter__(self: TTransaction) -> TTransaction:
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.close()
 
+
 def _normalize_value(in_value: InValue) -> Value:
     if isinstance(in_value, datetime):
         return int(in_value.timestamp() * 1000)
     elif isinstance(in_value, bool):
         return int(in_value)
     elif isinstance(in_value, (str, int, float)) or in_value is None:
         return in_value
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/create_client.py` & `libsql_client-0.3.1/libsql_client/create_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+from __future__ import annotations
+
 from typing import Optional
 
-from .client import Client, LibsqlError
+from .client import Client
+from .client import LibsqlError
 from .config import _expand_config
 from .hrana import _create_hrana_client
 from .http import _create_http_client
-from .sqlite3 import _create_sqlite3_client
+from .sqlite3_utils import _create_sqlite3_client
 
-def create_client(url: str, *, auth_token: Optional[str] = None) -> Client:
-    config = _expand_config(url, auth_token=auth_token)
-    if config.scheme == "libsql":
-        config = config._replace(scheme="wss")
 
+def create_client(
+    url: str, *, auth_token: Optional[str] = None, tls: Optional[bool] = None
+) -> Client:
+    config = _expand_config(url, auth_token=auth_token, tls=tls)
     if config.scheme == "file":
         return _create_sqlite3_client(config)
     elif config.scheme in ("ws", "wss"):
         return _create_hrana_client(config)
     elif config.scheme in ("http", "https"):
         return _create_http_client(config)
+    elif not url:
+        raise LibsqlError(
+            f"Database URL is {url}.", "URL_UNDEFINED"
+        )
     else:
-        raise LibsqlError(f"Unsupported URL scheme {config.scheme!r}", "URL_SCHEME_NOT_SUPPORTED")
+        raise LibsqlError(
+            f"Unsupported URL scheme {config.scheme!r}", "URL_SCHEME_NOT_SUPPORTED"
+        )
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/__init__.py` & `libsql_client-0.3.1/libsql_client/dbapi2/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,59 @@
+from __future__ import annotations
+
+import sqlite3.dbapi2
+from typing import Any
+from typing import Mapping
+from typing import Optional
+from urllib.parse import urlparse
+
+from ._reexports import *
+from .hrana import ConnectionHrana as Connection
+from .hrana import CursorHrana as Cursor
+from .types import ConnectFactory
+from .types import Connection as BaseConnection
+from .types import ConnectionTypes
+from .types import Cursor as BaseCursor
+from .types import enable_callback_tracebacks
+from .types import IsolationLevel
+from .types import LEGACY_TRANSACTION_CONTROL
+from .types import PathLike
+from .types import Row
+
 """
 This module implements `Python Database API Specification v2.0
 <https://peps.python.org/pep-0249/>`_
 mimicking as much as possible :py:mod:`sqlite3` in order to provide a
 drop-in replacement. Whenever explicitly undocumented, please refer its
 documentation.
 
 """
-__docformat__ = 'reStructuredText en'
-
-
-import sqlite3.dbapi2
-from urllib.parse import urlparse
-from typing import Any, Mapping, Optional
-
-from ._reexports import *  # noqa: F401,F403
-from .types import (  # noqa: F401
-    ConnectFactory,
-    Connection as BaseConnection,
-    ConnectionTypes,
-    Cursor as BaseCursor,
-    enable_callback_tracebacks,
-    IsolationLevel,
-    LEGACY_TRANSACTION_CONTROL,
-    PathLike,
-    Row,
-)
-
-from .hrana import (  # noqa: F401
-    ConnectionHrana as Connection,
-    CursorHrana as Cursor,
-)
+__docformat__ = "reStructuredText en"
 
 
 _connection_handlers: Mapping[str, ConnectFactory] = {
     "file": sqlite3.dbapi2.connect,
     "libsql": Connection,
     "ws": Connection,
     "wss": Connection,
 }
 
 _uri_forced_databases_prefixes = ("libsql://", "ws://", "wss://")
 
 
 def connect(
-        database: PathLike,
-        timeout: float = 5.0,
-        detect_types: int = 0,
-        isolation_level: Optional[IsolationLevel] = "",
-        check_same_thread: bool = True,
-        factory: Optional[ConnectFactory] = None,
-        cached_statements: int = 128,
-        uri: bool = False,
-        **kwargs: Any,
+    database: PathLike,
+    timeout: float = 5.0,
+    detect_types: int = 0,
+    isolation_level: Optional[IsolationLevel] = "",
+    check_same_thread: bool = True,
+    factory: Optional[ConnectFactory] = None,
+    cached_statements: int = 128,
+    uri: bool = False,
+    **kwargs: Any,
 ) -> ConnectionTypes:
     """
     Open a connection to an SQLite (local) or sqld (remote) database.
 
     In addition to :py:func:`sqlite3.connect`, this function allows
     connecting to remote servers using the following protocols:
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/__main__.py` & `libsql_client-0.3.1/libsql_client/dbapi2/__main__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import sys
 import os
 import os.path
+import sys
 
 args = sys.argv[1:]
 env = os.environ
 
 bootstrap_path = os.path.join(
     os.path.dirname(__file__),
     "_replace_modules_pythonpath",
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/_async_executor.py` & `libsql_client-0.3.1/libsql_client/dbapi2/_async_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,44 @@
+from __future__ import annotations
+
 import asyncio
 import concurrent.futures
 import functools
 import logging
 import queue
-import threading
 import sys
+import threading
+from typing import Any
+from typing import Awaitable
+from typing import Callable
+from typing import NamedTuple
+from typing import Optional
+from typing import overload
+from typing import TypeVar
 
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    NamedTuple,
-    Optional,
-    overload,
-    TypeVar,
-)
 from typing_extensions import ParamSpec
 
-from ._utils import log_obj, log_prefix
+from ._utils import log_obj
+from ._utils import log_prefix
+
 _logger = logging.getLogger(__name__)
 _log_obj = functools.partial(log_obj, _logger)
 _log_prefix = functools.partial(log_prefix, _logger)
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 class LoopControl(NamedTuple):
     loop: asyncio.AbstractEventLoop
     stop_event: asyncio.Event
 
 
-if sys.version_info[:2] >= (3, 9):
-    MainQueue = queue.Queue[LoopControl]
-else:
-    MainQueue = queue.Queue
-
-
 # NOTE: keep outside of class, do not touch self, not even keep a reference
-def _thread_main(log_prefix: str, q: MainQueue) -> None:
+def _thread_main(log_prefix: str, q: queue.Queue[LoopControl]) -> None:
     loop: Optional[asyncio.AbstractEventLoop] = None
 
     def dbg(
         msg: str,
         *args: object,
         exc_info: Optional[BaseException] = None,
     ) -> None:
@@ -73,21 +69,17 @@
 class AsyncExecutor(threading.Thread):
     _lock: threading.Lock
     _control: Optional[LoopControl]
     __slots__ = ("_control", "_lock")
 
     def __init__(self) -> None:
         self._control = None
-        q: MainQueue = queue.Queue(1)
+        q: queue.Queue[LoopControl] = queue.Queue(1)
         log_prefix = f"<{self.__class__.__name__} at {id(self):x}>"
-        super().__init__(
-            daemon=True,
-            target=_thread_main,
-            args=(log_prefix, q)
-        )
+        super().__init__(daemon=True, target=_thread_main, args=(log_prefix, q))
         self._inf("created")
         self.start()
         self._lock = threading.Lock()
         self._control = q.get()
         self._inf("thread ready")
 
     def __del__(self) -> None:
@@ -125,14 +117,15 @@
         coro = run_in_main_loop()
         future = asyncio.run_coroutine_threadsafe(coro, loop)
         future.result()
         self.join()
         self._inf("thread did stop")
 
     if sys.version_info[:2] >= (3, 9):
+
         @overload
         def submit(
             self,
             fn: Callable[P, Awaitable[asyncio.Future[T]]],
             *args: P.args,
             **kwargs: P.kwargs,
         ) -> concurrent.futures.Future[T]:
@@ -153,14 +146,15 @@
             fn: Callable[P, T],
             *args: P.args,
             **kwargs: P.kwargs,
         ) -> concurrent.futures.Future[T]:
             ...
 
     else:
+
         @overload
         def submit(
             self,
             fn: Callable[P, Awaitable[asyncio.Future]],
             *args: P.args,
             **kwargs: P.kwargs,
         ) -> concurrent.futures.Future:
@@ -206,20 +200,26 @@
             try:
                 self._dbg("calling: %s, args=%s, kwargs=%s", fn, args, kwargs)
                 r = fn(*args, **kwargs)
                 while asyncio.iscoroutine(r) or asyncio.isfuture(r):
                     r = await r
                 self._dbg(
                     "finished: %s, args=%s, kwargs=%s, result=%s",
-                    fn, args, kwargs, r,
+                    fn,
+                    args,
+                    kwargs,
+                    r,
                 )
                 return r
             except Exception as e:
                 self._dbg(
                     "failed: %s, args=%s, kwargs=%s, exc=%s",
-                    fn, args, kwargs, e,
+                    fn,
+                    args,
+                    kwargs,
+                    e,
                     exc_info=e,
                 )
                 raise
 
         coro = run_in_main_loop()
         return asyncio.run_coroutine_threadsafe(coro, self._control.loop)
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/dbapi2.py` & `libsql_client-0.3.1/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/dbapi2.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 # This MUST be done before libsql_client.dbapi2 is imported
 # since it will use the stdlib sqlite3
 sys.path.remove(bootstrap_path)
 del sys.modules[sqlite3_modname]
 del sys.modules[sqlite3_dbapi2_modname]
 
 import libsql_client.dbapi2 as wrapper_dbapi2  # noqa: I900,E402
+
 sys.modules[sqlite3_modname] = wrapper_dbapi2
 sys.modules[sqlite3_dbapi2_modname] = wrapper_dbapi2
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/_utils.py` & `libsql_client-0.3.1/libsql_client/dbapi2/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-import logging
+from __future__ import annotations
 
-from typing import List, Iterable, Optional, Sequence
+import logging
+from typing import Iterable
+from typing import List
+from typing import Optional
+from typing import Sequence
 
 
 def log_prefix(
-        logger: logging.Logger,
-        prefix: str,
-        level: int,
-        msg: str,
-        *args: object,
-        exc_info: Optional[BaseException] = None,
+    logger: logging.Logger,
+    prefix: str,
+    level: int,
+    msg: str,
+    *args: object,
+    exc_info: Optional[BaseException] = None,
 ) -> None:
     logger.log(level, prefix + msg, *args, exc_info=exc_info)
 
 
 def log_obj(
-        logger: logging.Logger,
-        obj: object,
-        level: int,
-        msg: str,
-        *args: object,
-        exc_info: Optional[BaseException] = None,
+    logger: logging.Logger,
+    obj: object,
+    level: int,
+    msg: str,
+    *args: object,
+    exc_info: Optional[BaseException] = None,
 ) -> None:
     prefix = getattr(obj, "_log_prefix", None)
     if prefix is None:
         prefix = f"{obj!r}: "
     log_prefix(logger, prefix, level, msg, *args, exc_info=exc_info)
 
 
@@ -91,15 +95,15 @@
     return None
 
 
 _iter_sql_delim_chars = {";", ",", "(", ")", "[", "]"}
 _iter_sql_stop_chars = _lstrip_sql_whitespace_chars.union(
     _iter_sql_delim_chars,
 )
-_iter_sql_quote_chars = {"\"", "'"}
+_iter_sql_quote_chars = {'"', "'"}
 
 
 def _iter_sql_get_quoted_end(sql: str, pos: int, end_pos: int) -> int:
     """Find the end of the quoted string starting at ``pos``.
 
     The returned position includes the position of the quote character,
     that matches the one at ``pos``.
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/hrana.py` & `libsql_client-0.3.1/libsql_client/dbapi2/hrana.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,146 @@
-import aiohttp
+from __future__ import annotations
+
 import asyncio
 import collections.abc
-import urllib.parse
 import sqlite3.dbapi2
 import sys
+from typing import Awaitable
+from typing import Callable
+from typing import Iterable
+from typing import List
+from typing import Optional
+from typing import overload
+from typing import Tuple
+from typing import Type
+from typing import TYPE_CHECKING
+from typing import TypeVar
 
-from typing import (
-    Awaitable,
-    Callable,
-    Iterable,
-    List,
-    Optional,
-    overload,
-    Tuple,
-    TYPE_CHECKING,
-    Type,
-    TypeVar,
-)
+import aiohttp
 from typing_extensions import ParamSpec
 
-from ..hrana.conn import HranaConn, HranaStream
-from ..hrana.proto import (
-    Batch,
-    BatchResult,
-    BatchStep,
-    Error as ErrorResult,
-    Stmt,
-    StmtResult,
-)
-from ..hrana.convert import _value_to_proto, _error_from_proto
-
-from ..config import _expand_config
-from .types import (
-    Autocommit,
-    Connection,
-    Cursor,
-    IsolationLevel,
-    LEGACY_TRANSACTION_CONTROL,
-    OperationalError,
-    RawExecuteResult,
-    SqlParameters,
-)
 from ._async_executor import AsyncExecutor
+from .types import Autocommit
+from .types import Connection
+from .types import Cursor
+from .types import IsolationLevel
+from .types import LEGACY_TRANSACTION_CONTROL
+from .types import OperationalError
+from .types import RawExecuteResult
+from .types import SqlParameters
+from ..client import LibsqlError
+from ..config import _expand_config
+from ..hrana.client import _config_to_url
+from ..hrana.conn import HranaConn
+from ..hrana.conn import HranaStream
+from ..hrana.convert import _error_from_proto
+from ..hrana.convert import _value_to_proto
+from ..hrana.proto import Batch
+from ..hrana.proto import BatchResult
+from ..hrana.proto import BatchStep
+from ..hrana.proto import Error as ErrorResult
+from ..hrana.proto import Stmt
+from ..hrana.proto import StmtResult
 
 
 # TODO: we're creating a whole sync client for each connection, but we
 # could create a single thread for all connections of the same URL,
 # with a single HranaClient/HranaConn, and just get a HranaStream.
 # But this requires us to change ClientSync and other stuff, will
 # do it later.
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
-if sys.version_info[:2] >= (3, 9):
-    FutureStmtResult = asyncio.Future[StmtResult]
-    FutureBatchResult = asyncio.Future[BatchResult]
-    FutureNone = asyncio.Future[None]
-else:
-    FutureStmtResult = asyncio.Future
-    FutureBatchResult = asyncio.Future
-    FutureNone = asyncio.Future
-
 
 def _create_hrana_connection(
-        session: aiohttp.ClientSession,
-        url: str,
+    session: aiohttp.ClientSession,
+    url: str,
+    auth_token: str = None,
 ) -> HranaConn:
-    config = _expand_config(url, auth_token=None)
+    config = _expand_config(url, auth_token=auth_token, tls=None)
+
+    try:
+        if config.scheme not in ("ws", "wss"):
+            raise LibsqlError(
+                "Only 'libsql', 'ws' and 'wss' URLs are supported,"
+                f" got {config.scheme!r}",
+                "URL_INVALID",
+            )
+        url = _config_to_url(config)
+    except LibsqlError as e:
+        if e.code == "URL_INVALID":
+            sqlite_err = OperationalError(str(e))
+            sqlite_err.sqlite_errorcode = 14  # type: ignore
+            sqlite_err.sqlite_errorname = "SQLITE_CANTOPEN"  # type: ignore
+            raise sqlite_err
+        raise
 
-    # TODO: maybe handle this inside HranaConn?
-    if config.scheme == "libsql":
-        config = config._replace(scheme="wss")
-
-    url = urllib.parse.urlunparse((
-        config.scheme, config.authority, config.path,
-        "", "", "",
-    ))
     return HranaConn(session, url, config.auth_token)
 
 
 def _conv_stmt_plain_to_stored(stmt: Stmt, sql_id: int) -> Stmt:
     del stmt["sql"]
     stmt["sql_id"] = sql_id
     return stmt
 
 
 def _conv_stmt(
-        sql: str,
-        parameters: SqlParameters,
-        want_rows: bool,
+    sql: str,
+    parameters: SqlParameters,
+    want_rows: bool,
 ) -> Stmt:
     stmt: Stmt = {
         "sql": sql,
         "want_rows": want_rows,
     }
     if isinstance(parameters, collections.abc.Mapping):
         stmt["named_args"] = [
-            {"name": k, "value": _value_to_proto(v)}
-            for k, v in parameters.items()
+            {"name": k, "value": _value_to_proto(v)} for k, v in parameters.items()
         ]
     elif parameters:
         # SupportsLenAndGetItem is only __len__ + __getitem__, no __iter__
         # so create the list manually :-(
         args = []
         for i in range(len(parameters)):
             args.append(_value_to_proto(parameters[i]))
         stmt["args"] = args
 
     return stmt
 
 
 def _conv_stmts(
-        sql: str,
-        parameters: Iterable[SqlParameters],
-        want_rows: bool,
+    sql: str,
+    parameters: Iterable[SqlParameters],
+    want_rows: bool,
 ) -> List[Stmt]:
     return [_conv_stmt(sql, p, want_rows) for p in parameters]
 
 
 _aiohttp_error_map = (
     (aiohttp.InvalidURL, "SQLITE_CANTOPEN"),
     (aiohttp.ClientConnectionError, "SQLITE_CANTOPEN"),
     (aiohttp.ClientResponseError, "SQLITE_CANTOPEN"),
     (aiohttp.ClientPayloadError, "SQLITE_IOERR"),
 )
 
 
 def _get_aiohttp_client_error_code(
-        error: aiohttp.ClientError,
+    error: aiohttp.ClientError,
 ) -> Tuple[int, str]:
     for error_cls, error_name in _aiohttp_error_map:
         if isinstance(error, error_cls):
             error_code = getattr(sqlite3.dbapi2, error_name)
             return error_code, error_name
     return 0, ""
 
 
 def _conv_stmt_result(
-        result: Optional[StmtResult],
-        error: Optional[BaseException],
+    result: Optional[StmtResult],
+    error: Optional[BaseException],
 ) -> RawExecuteResult:
     if isinstance(error, aiohttp.ClientError):
         code, name = _get_aiohttp_client_error_code(error)
         error = OperationalError(str(error))
         if code:
             error.sqlite_errorcode = code  # type: ignore
             error.sqlite_errorname = name  # type: ignore
@@ -154,18 +151,20 @@
 def _conv_batch(stmts: List[Stmt]) -> Batch:
     steps: List[BatchStep] = []
 
     for i, stmt in enumerate(stmts):
         if i == 0:
             steps.append({"stmt": stmt})
         else:
-            steps.append({
-                "condition": {"type": "ok", "step": i - 1},
-                "stmt": stmt,
-            })
+            steps.append(
+                {
+                    "condition": {"type": "ok", "step": i - 1},
+                    "stmt": stmt,
+                }
+            )
 
     return {"steps": steps}
 
 
 def _conv_batch_result(resp: BatchResult) -> RawExecuteResult:
     def conv_err(e: Optional[ErrorResult]) -> Optional[BaseException]:
         if e is None:
@@ -174,14 +173,15 @@
 
     errors = [conv_err(e) for e in resp["step_errors"]]
     return RawExecuteResult(resp["step_results"], errors)
 
 
 if TYPE_CHECKING:
     if sys.version_info[:2] >= (3, 9):
+
         @overload
         def run_in_executor(
             fn: Callable[P, Awaitable[asyncio.Future[T]]],
         ) -> Callable[P, T]:
             ...
 
     @overload
@@ -200,14 +200,15 @@
     :py:class:`AsyncExecutor` thread by doing a ``AsyncExecutor.submit()``
     and then ``future.result(timeout)``.
 
     The method itself will block until the executor runs.
 
     :meta private:
     """
+
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         self = args[0]
         assert isinstance(self, ConnectionHrana)
         assert self._executor is not None
 
         future = self._executor.submit(fn, *args, **kwargs)
 
@@ -217,40 +218,44 @@
 
 
 class ConnectionHrana(Connection):
     """Implement :py:class:`sqlite3.Connection` for remote servers
     using the `Hrana Protocol
     <https://github.com/libsql/sqld/blob/main/docs/HRANA_2_SPEC.md>`_.
     """
+
     _executor: Optional[AsyncExecutor]  # TODO: share
     _session: Optional[aiohttp.ClientSession]  # TODO: share (per url)
     _conn: Optional[HranaConn]  # TODO: share (per url)
     _stream: Optional[HranaStream]
     cursor_factory: Type["CursorHrana"]
+    auth_token: str = ""
 
     def __init__(
         self,
         database: str,
+        auth_token: str = None,
         timeout: float = 5.0,
         detect_types: int = 0,
         isolation_level: Optional[IsolationLevel] = "",
         check_same_thread: bool = True,
         cached_statements: int = 128,
         uri: bool = False,
         autocommit: Autocommit = LEGACY_TRANSACTION_CONTROL,
     ) -> None:
         assert uri
+        self.auth_token = auth_token
         super().__init__(
             database=database,
             timeout=timeout,
             detect_types=detect_types,
             isolation_level=isolation_level,
             check_same_thread=check_same_thread,
             cached_statements=cached_statements,
-            autocommit=autocommit
+            autocommit=autocommit,
         )
 
     def _raw_init(self) -> None:
         self.cursor_factory = CursorHrana
         try:
             self._executor = self._acquire_executor()
             self._session = self._acquire_session()
@@ -274,15 +279,15 @@
     async def _dispose_session(self, session: aiohttp.ClientSession) -> None:
         await session.close()  # TODO: share
 
     @run_in_executor
     async def _acquire_connection(self, url: str) -> HranaConn:
         assert self._session is not None
         # TODO: share (per url)
-        conn = _create_hrana_connection(self._session, url)
+        conn = _create_hrana_connection(self._session, url, self.auth_token)
         try:
             await conn.wait_connected()
             return conn
         except Exception as error:
             await conn.close()
             exc = _conv_stmt_result(None, error).errors[0]
             assert exc is not None  # make mypy happy
@@ -301,35 +306,35 @@
 
     @run_in_executor
     def _destroy_stream(self, stream: HranaStream) -> None:
         self._inf("closing stream: %s", stream)
         stream.close()
 
     @run_in_executor
-    def _raw_execute(self, stmt: Stmt) -> FutureStmtResult:
+    def _raw_execute(self, stmt: Stmt) -> asyncio.Future[StmtResult]:
         assert self._stream is not None
         return self._stream.execute(stmt)
 
     @run_in_executor
     def _raw_store_sql(self, sql: str) -> int:
         assert self._conn is not None
         return self._conn.store_sql(sql)
 
     @run_in_executor
     def _raw_close_sql(self, sql_id: int) -> None:
         assert self._conn is not None
         return self._conn.close_sql(sql_id)
 
     @run_in_executor
-    def _raw_execute_script(self, sql_script: str) -> FutureNone:
+    def _raw_execute_script(self, sql_script: str) -> asyncio.Future[None]:
         assert self._stream is not None
         return self._stream.sequence(sql_script)
 
     @run_in_executor
-    def _raw_batch(self, batch: Batch) -> FutureBatchResult:
+    def _raw_batch(self, batch: Batch) -> asyncio.Future[BatchResult]:
         assert self._stream is not None
         return self._stream.batch(batch)
 
     def _raw_close(self) -> None:
         # use of getattr as the object may fail init
         stream = getattr(self, "_stream", None)
         if stream is not None:
@@ -353,14 +358,15 @@
 
 
 class CursorHrana(Cursor):
     """Implement :py:class:`sqlite3.Cursor` for remote servers
     using the `Hrana Protocol
     <https://github.com/libsql/sqld/blob/main/docs/HRANA_2_SPEC.md>`_.
     """
+
     connection: ConnectionHrana
 
     def _raw_execute_one(self, stmt: Stmt) -> RawExecuteResult:
         try:
             if self.connection._trace_callback is not None:
                 self.connection._trace(stmt["sql"])
             result = self.connection._raw_execute(stmt)
@@ -390,19 +396,19 @@
             if sql_id is not None:
                 try:
                     self.connection._raw_close_sql(sql_id)
                 except Exception:
                     pass
 
     def _raw_execute(
-            self,
-            sql: str,
-            parameters: Iterable[SqlParameters],
-            *,
-            want_rows: bool = True,
+        self,
+        sql: str,
+        parameters: Iterable[SqlParameters],
+        *,
+        want_rows: bool = True,
     ) -> RawExecuteResult:
         stmts = _conv_stmts(sql, parameters, want_rows)
         if len(stmts) == 1:
             return self._raw_execute_one(stmts[0])
         elif len(stmts) > 1:
             return self._raw_execute_multiple(stmts)
         else:
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/dbapi2/types.py` & `libsql_client-0.3.1/libsql_client/dbapi2/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,96 +1,95 @@
+from __future__ import annotations
+
+from abc import ABCMeta
+from abc import abstractmethod
 import collections
 import collections.abc
-import os
-import logging
 import functools
+import logging
+import os
 import re
-import threading
+import sqlite3.dbapi2
+from sqlite3.dump import _iterdump as sqlite3_iterdump
 import sys
-
-from abc import ABCMeta, abstractmethod
+import threading
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import ClassVar
+from typing import Dict
+from typing import Iterable
+from typing import Iterator
+from typing import List
+from typing import NoReturn
+from typing import Optional
+from typing import overload
+from typing import Sequence
+from typing import Set
+from typing import Tuple
+from typing import TYPE_CHECKING
+from typing import TypeVar
+from typing import Union
 from weakref import WeakSet
-from typing import (
-    Any,
-    Callable,
-    cast,
-    ClassVar,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
-    NoReturn,
-    Optional,
-    overload,
-    Sequence,
-    Set,
-    Tuple,
-    TYPE_CHECKING,
-    TypeVar,
-    Union,
-)
-from typing_extensions import Literal, Self, ParamSpec
-import sqlite3.dbapi2
-from . import _reexports
-from ._reexports import (
-    DatabaseError,
-    DataError,
-    IntegrityError,
-    InterfaceError,
-    InternalError,
-    NotSupportedError,
-    OperationalError,
-    ProgrammingError,
-    SQLITE_LIMIT_SQL_LENGTH,
-)
-if sys.version_info[:2] >= (3, 11):
-    from ._reexports import Blob
 
-from sqlite3.dump import _iterdump as sqlite3_iterdump  # type: ignore
+from typing_extensions import Literal
+from typing_extensions import ParamSpec
+from typing_extensions import Self
 
+from . import _reexports
+from ._reexports import DatabaseError
+from ._reexports import DataError
+from ._reexports import IntegrityError
+from ._reexports import InterfaceError
+from ._reexports import InternalError
+from ._reexports import NotSupportedError
+from ._reexports import OperationalError
+from ._reexports import ProgrammingError
+from ._reexports import SQLITE_LIMIT_SQL_LENGTH
+from ._utils import iter_sql_statements
+from ._utils import log_obj
+from ..client import LibsqlError
 from ..hrana import proto
 from ..hrana.convert import _value_from_proto
-from ..client import LibsqlError
 
-from ._utils import log_obj, iter_sql_statements
+if sys.version_info[:2] >= (3, 11):
+    from ._reexports import Blob
 
 _logger = logging.getLogger(__name__)
 _log_obj = functools.partial(log_obj, _logger)
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 if TYPE_CHECKING:
-    from sqlite3.dbapi2 import (
-        _Parameters as SqlParameters,
-        _SqliteData as SqlData,
-    )
+    from sqlite3.dbapi2 import _Parameters as SqlParameters
+    from sqlite3.dbapi2 import _SqliteData as SqlData
 else:
     SqlParameters = Any
     SqlData = Any
 
 PathLike = Union[str, bytes, os.PathLike]
 IsolationLevel = Literal["", "DEFERRED", "EXCLUSIVE", "IMMEDIATE"]
 isolation_level_set: Set[IsolationLevel] = {
-    "", "DEFERRED", "EXCLUSIVE", "IMMEDIATE",
+    "",
+    "DEFERRED",
+    "EXCLUSIVE",
+    "IMMEDIATE",
 }
 
 SqlNativeType = Union[None, int, float, str, bytes]
 ConnectionTypes = Union[sqlite3.dbapi2.Connection, "Connection"]
 ConnectFactory = Callable[..., ConnectionTypes]
 CursorFactory = Callable[["Connection"], "Cursor"]
 RowFactory = Callable[["Cursor", Iterable[Any]], Any]
 TextFactory = Callable[[bytes], Any]
 ConverterCallback = Callable[[Any], Any]
 
-AuthorizerCallback = Callable[
-    ...,
-    int  # SQLITE_OK, SQLITE_DENY, or SQLITE_IGNORE
-]
+AuthorizerCallback = Callable[..., int]  # SQLITE_OK, SQLITE_DENY, or SQLITE_IGNORE
 ProgressHandler = Callable[[], int]
 TraceCallback = Callable[[str], None]
 BackupProgressCallback = Callable[[int, int, int], None]
 
 RawResults = proto.StmtResult
 RawColumn = proto.Col
 RawRow = List[proto.Value]
@@ -130,16 +129,17 @@
 _default_limits = _get_local_default_limits()
 
 
 def check_valid_autocommit(value: Any) -> Autocommit:
     ":meta private:"
     if value is LEGACY_TRANSACTION_CONTROL or isinstance(value, bool):
         return value
-    raise ValueError("autocommit must be True, False, or "
-                     "sqlite3.LEGACY_TRANSACTION_CONTROL")
+    raise ValueError(
+        "autocommit must be True, False, or " "sqlite3.LEGACY_TRANSACTION_CONTROL"
+    )
 
 
 _callback_tracebacks: bool = False
 
 
 def enable_callback_tracebacks(flag: bool) -> None:
     """See :py:func:`sqlite3.enable_callback_tracebacks`"""
@@ -148,23 +148,24 @@
 
 
 class RawExecuteResult:
     """Iterable over pairs of ``result, error``.
 
     :meta private:
     """
+
     results: List[Optional[RawResults]]
     errors: List[Optional[BaseException]]
     _idx: int
     __slots__ = ("results", "errors", "_idx")
 
     def __init__(
-            self,
-            results: List[Optional[RawResults]],
-            errors: List[Optional[BaseException]],
+        self,
+        results: List[Optional[RawResults]],
+        errors: List[Optional[BaseException]],
     ) -> None:
         assert len(results) == len(errors)
         self.results = results
         self.errors = errors
         self._idx = 0
 
     def __iter__(self) -> Self:
@@ -184,18 +185,23 @@
     sql: str
     tokens: Sequence[str]
     is_dml: bool
     is_ddl: bool
     __slots__ = ("sql", "tokens", "is_dml", "is_ddl")
 
     _dml_statements: ClassVar[Set[str]] = {
-        "INSERT", "UPDATE", "DELETE", "REPLACE",
+        "INSERT",
+        "UPDATE",
+        "DELETE",
+        "REPLACE",
     }
     _ddl_statements: ClassVar[Set[str]] = {
-        "CREATE", "ALTER", "DROP",
+        "CREATE",
+        "ALTER",
+        "DROP",
     }
 
     @overload
     def __init__(self, sql: str) -> None:
         ...
 
     @overload
@@ -270,14 +276,15 @@
 def check_thread(fn: Callable[P, T]) -> Callable[P, T]:
     """Decorator that checks :py:class:`Connection` thread usage.
 
     Otherwise raises ``ProgrammingError``.
 
     :meta private:
     """
+
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         self = args[0]
         assert len(args) > 0 and isinstance(self, Connection)
         self._do_check_thread()
         return fn(*args, **kwargs)
 
     return wrapper
@@ -286,28 +293,30 @@
 def check_connection(fn: Callable[P, T]) -> Callable[P, T]:
     """Decorator that checks :py:class:`Connection` being valid.
 
         Otherwise raises ``ProgrammingError``.
 
     :meta private:
     """
+
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         self = args[0]
         assert len(args) > 0 and isinstance(self, Connection)
         self._do_check_connection()
         return fn(*args, **kwargs)
 
     return wrapper
 
 
 class Connection(metaclass=ABCMeta):
     """Implement :py:class:`sqlite3.Connection` for remote servers.
 
     :meta private:
     """
+
     _closed: bool
     _thread: Optional[int]
     _database: str
     _timeout: float
     _detect_types: int
     _isolation_level: Optional[IsolationLevel]
     _check_same_thread: bool
@@ -334,17 +343,17 @@
         check_valid_autocommit(autocommit)  # required by test
         self._closed = False
         self._thread = threading.current_thread().ident
         self._database = database
         self._timeout = timeout
         self._detect_types = detect_types
         self._check_same_thread = check_same_thread
-        self._cached_statement_getter = functools.lru_cache(
-            cached_statements
-        )(self.__call__)
+        self._cached_statement_getter = functools.lru_cache(cached_statements)(
+            self.__call__
+        )
         self._in_transaction = False
         self._cursors = WeakSet()
         self.row_factory = None
         self.text_factory = None
         self.cursor_factory = Cursor
         self._autocommit = autocommit
         self._trace_callback = None
@@ -372,19 +381,20 @@
 
     def _do_check_thread(self) -> None:
         # class may not be properly initialized, as in some unit tests
         check = getattr(self, "_check_same_thread", None)
         if check:
             current_ident = threading.current_thread().ident
             if self._thread != current_ident:
-                msg = "SQLite objects created in a thread can only be used " \
-                      "in that same thread. " \
-                      "The object was created in thread id " \
-                      "%s and this is thread id %s." \
-                      % (self._thread, current_ident)
+                msg = (
+                    "SQLite objects created in a thread can only be used "
+                    "in that same thread. "
+                    "The object was created in thread id "
+                    "%s and this is thread id %s." % (self._thread, current_ident)
+                )
                 raise ProgrammingError(msg)
         elif check is None:
             raise ProgrammingError("Base Connection.__init__ not called")
 
     def _do_check_connection(self) -> None:
         # class may not be properly initialized, as in some unit tests
         closed = getattr(self, "_closed", None)
@@ -394,18 +404,18 @@
             raise ProgrammingError("Base Connection.__init__ not called")
 
     @check_connection
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
-            self,
-            exc_type: Any,
-            exc_value: Any,
-            traceback: Any,
+        self,
+        exc_type: Any,
+        exc_value: Any,
+        traceback: Any,
     ) -> Literal[False]:
         # https://docs.python.org/3/library/sqlite3.html#how-to-use-the-connection-context-manager
         # https://github.com/python/cpython/blob/main/Modules/_sqlite/connection.c#L2262
         if exc_type is None:
             self.commit()
         else:
             try:
@@ -502,15 +512,16 @@
     @overload
     def cursor(self) -> "Cursor":
         ...
 
     @check_thread
     @check_connection
     def cursor(
-        self, *args: CursorFactory,
+        self,
+        *args: CursorFactory,
         **kwargs: CursorFactory,
     ) -> "Cursor":
         if args:
             factory = args[0]
         elif "factory" in kwargs:
             factory = kwargs["factory"]
         else:
@@ -545,18 +556,20 @@
             f"BEGIN {self.isolation_level}",
             want_rows=False,
         )
 
     def _begin_transaction_if_needed(self, statement: Statement) -> None:
         # _pysqlite_query_execute()
         # https://github.com/python/cpython/blob/main/Modules/_sqlite/cursor.c#L867-L877
-        if self._autocommit is LEGACY_TRANSACTION_CONTROL \
-           and self.isolation_level is not None \
-           and statement.is_dml \
-           and self._sqlite3_get_autocommit():
+        if (
+            self._autocommit is LEGACY_TRANSACTION_CONTROL
+            and self.isolation_level is not None
+            and statement.is_dml
+            and self._sqlite3_get_autocommit()
+        ):
             self._begin_transaction()
 
     _begin_transaction_tokens: ClassVar[Set[str]] = {"BEGIN"}
     _end_transaction_tokens: ClassVar[Set[str]] = {"END", "COMMIT", "ROLLBACK"}
 
     def _update_in_transaction(self, statement: Statement) -> None:
         # we cannot query sqlite3_get_autocommit(), then emulate
@@ -614,25 +627,25 @@
         self._closed = True
 
     def interrupt(self) -> None:
         "Does nothing"
         pass
 
     def execute(
-            self,
-            sql: str,
-            parameters: SqlParameters = (),
+        self,
+        sql: str,
+        parameters: SqlParameters = (),
     ) -> "Cursor":
         "See :py:meth:`sqlite3.Connection.execute`"
         return self.cursor().execute(sql, parameters)
 
     def executemany(
-            self,
-            sql: str,
-            parameters: Iterable[SqlParameters],
+        self,
+        sql: str,
+        parameters: Iterable[SqlParameters],
     ) -> "Cursor":
         "See :py:meth:`sqlite3.Connection.executemany`"
         return self.cursor().executemany(sql, parameters)
 
     def executescript(self, sql_script: str) -> "Cursor":
         "See :py:meth:`sqlite3.Connection.executescript`"
         return self.cursor().executescript(sql_script)
@@ -647,16 +660,16 @@
         # https://github.com/python/cpython/blob/main/Modules/_sqlite/cursor.c#L186-L207
         upcase_key = key.upper()
         return sqlite3.converters.get(upcase_key)
 
     @check_thread
     @check_connection
     def set_trace_callback(
-            self,
-            trace_callback: Optional[TraceCallback],
+        self,
+        trace_callback: Optional[TraceCallback],
     ) -> None:
         "See :py:meth:`sqlite3.Connection.set_trace_callback`"
         self._trace_callback = trace_callback
 
     def _trace(self, sql: str) -> None:
         if self._trace_callback is None:
             return
@@ -678,80 +691,82 @@
                 sys.unraisablehook(UnraisableHookArgs())  # type: ignore
             else:
                 self._dbg("trace callback failed: %r", sql, exc_info=e)
 
     # BEGIN: methods that are not supported when operating as RPC
 
     if sys.version_info[:2] >= (3, 11):
+
         def blobopen(
-                self,
-                table: str,
-                column: str,
-                row: str,
-                *,
-                readonly: bool = False,
-                name: str = "main",
+            self,
+            table: str,
+            column: str,
+            row: str,
+            *,
+            readonly: bool = False,
+            name: str = "main",
         ) -> Blob:
             "Unsupported by libsql_client.dbapi2"
             raise NotSupportedError()
 
     def create_function(
-            self,
-            name: str,
-            narg: int,
-            func: Optional[Callable[..., SqlNativeType]],
-            *,
-            deterministic: bool = False,
+        self,
+        name: str,
+        narg: int,
+        func: Optional[Callable[..., SqlNativeType]],
+        *,
+        deterministic: bool = False,
     ) -> None:
         "Unsupported by libsql_client.dbapi2"
         # maybe one day support with WASM
         raise NotSupportedError()
 
     def create_aggregate(
-            self,
-            name: str,
-            n_arg: int,
-            aggregate_class: Optional[Callable[..., Any]],
+        self,
+        name: str,
+        n_arg: int,
+        aggregate_class: Optional[Callable[..., Any]],
     ) -> None:
         "Unsupported by libsql_client.dbapi2"
         # maybe one day support with WASM
         raise NotSupportedError()
 
     if sys.version_info[:2] >= (3, 11):
+
         def create_window_function(
-                self,
-                name: str,
-                num_params: int,
-                aggregate_class: Optional[Callable[..., Any]],
+            self,
+            name: str,
+            num_params: int,
+            aggregate_class: Optional[Callable[..., Any]],
         ) -> None:
             "Unsupported by libsql_client.dbapi2"
             # maybe one day support with WASM
             raise NotSupportedError()
 
     def create_collation(
-            self,
-            name: str,
-            _callable: Optional[Callable[[str, str], int]],
+        self,
+        name: str,
+        _callable: Optional[Callable[[str, str], int]],
     ) -> None:
         "Unsupported by libsql_client.dbapi2"
         # maybe one day support with WASM
         raise NotSupportedError()
 
     def set_authorizer(
-            self,
-            authorizer_callback: Optional[AuthorizerCallback],
+        self,
+        authorizer_callback: Optional[AuthorizerCallback],
     ) -> None:
         "Unsupported by libsql_client.dbapi2"
         # maybe one day support with WASM
         raise NotSupportedError()
 
     def set_progress_handler(
-            self,
-            progress_handler: Optional[ProgressHandler],
-            n: int,
+        self,
+        progress_handler: Optional[ProgressHandler],
+        n: int,
     ) -> None:
         "Unsupported by libsql_client.dbapi2"
         # not likely to be supported
         raise NotSupportedError()
 
     def enable_load_extension(self, enabled: bool) -> None:
         "Unsupported by libsql_client.dbapi2"
@@ -760,27 +775,28 @@
 
     def load_extension(self, path: str) -> None:
         "Unsupported by libsql_client.dbapi2"
         # not likely to be supported
         raise NotSupportedError()
 
     def backup(
-            self,
-            target: "Connection",
-            *,
-            pages: int = - 1,
-            progress: Optional[BackupProgressCallback] = None,
-            name: str = "main",
-            sleep: float = 0.250,
+        self,
+        target: "Connection",
+        *,
+        pages: int = -1,
+        progress: Optional[BackupProgressCallback] = None,
+        name: str = "main",
+        sleep: float = 0.250,
     ) -> None:
         "Unsupported by libsql_client.dbapi2"
         # not likely to be supported
         raise NotSupportedError()
 
     if sys.version_info[:2] >= (3, 11):
+
         def getlimit(self, category: int) -> int:
             "Unsupported by libsql_client.dbapi2"
             try:
                 return self._limits[category]
             except KeyError:
                 raise ProgrammingError(f"unknown category: {category}")
 
@@ -815,23 +831,24 @@
     None,  # null_ok
 ]
 CursorDescription = Tuple[CursorColumnDescription, ...]
 RowCastMap = Tuple[Optional[ConverterCallback], ...]
 
 
 def tuple_row_factory(
-        cursor: "Cursor",
-        cells: Iterable[Any],
+    cursor: "Cursor",
+    cells: Iterable[Any],
 ) -> Tuple[Any, ...]:
     ":meta private:"
     return tuple(cells)
 
 
 class Row(collections.abc.Sequence):
     """Implement :py:class:`sqlite3.Row`"""
+
     _description: CursorDescription
     _data: Tuple[Any, ...]
     __slots__ = ("_description", "_data")
 
     def __init__(self, cursor: "Cursor", data: Iterable[Any]) -> None:
         # While isinstance() should do,
         # RowFactoryTests.test_fake_cursor_class() tests for a hack
@@ -896,14 +913,15 @@
 def check_cursor(fn: Callable[P, T]) -> Callable[P, T]:
     """Decorator that checks :py:class:`Cursor` being valid
 
     Otherwise raises ``ProgrammingError``.
 
     :meta private:
     """
+
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
         self = args[0]
         assert len(args) > 0 and isinstance(self, Cursor)
         self._do_check_cursor()
         return fn(*args, **kwargs)
 
     return wrapper
@@ -989,16 +1007,16 @@
         # https://www.sqlite.org/lang_expr.html#castexpr
         return str(v).encode()  # converts to text
 
     raise NotImplementedError(f"cannot handle value type {type(v)}")
 
 
 def _get_value_converted(
-        value: proto.Value,
-        text_factory: Optional[TextFactory],
+    value: proto.Value,
+    text_factory: Optional[TextFactory],
 ) -> Any:
     v = _value_from_proto(value)
     if not isinstance(v, str) or text_factory is None or text_factory is str:
         return v
     b = v.encode()
     if text_factory is bytes:
         return b
@@ -1017,17 +1035,26 @@
     _rows: Optional[List[RawRow]]
     _rows_iter_idx: int
     _raw_results: Optional[RawExecuteResult]
     _closed: bool
     _locked: bool
 
     __slots__ = (
-        "_connection", "_description", "_row_cast_map", "arraysize",
-        "_lastrowid", "_rowcount", "row_factory", "_rows", "_rows_iter_idx",
-        "_raw_results", "_closed", "_locked",
+        "_connection",
+        "_description",
+        "_row_cast_map",
+        "arraysize",
+        "_lastrowid",
+        "_rowcount",
+        "row_factory",
+        "_rows",
+        "_rows_iter_idx",
+        "_raw_results",
+        "_closed",
+        "_locked",
     )
 
     def __init__(self, connection: Connection) -> None:
         if not isinstance(connection, Connection):
             # be safe, pass CursorTests.test_cursor_wrong_class
             raise TypeError("connection must be instance of 'Connection'")
 
@@ -1107,19 +1134,19 @@
     @property
     def rowcount(self) -> int:
         "See :py:attr:`sqlite3.Cursor.rowcount`"
         return self._rowcount
 
     @abstractmethod
     def _raw_execute(
-            self,
-            sql: str,
-            parameters: Iterable[SqlParameters],
-            *,
-            want_rows: bool = True,
+        self,
+        sql: str,
+        parameters: Iterable[SqlParameters],
+        *,
+        want_rows: bool = True,
     ) -> RawExecuteResult:
         # each system should implement this one
         raise NotImplementedError()
 
     def _apply_raw_results(self, raw_results: RawResults) -> None:
         row_id = raw_results["last_insert_rowid"]
         self._lastrowid = int(row_id) if row_id else None
@@ -1147,17 +1174,17 @@
             self._row_cast_map = tuple(row_cast_map)
 
     def _apply_raw_results_rows(self, raw_results: RawResults) -> None:
         self._rows = raw_results["rows"]
         self._rows_iter_idx = 0
 
     def _convert_row(self, row: RawRow) -> Any:
-        row_factory = self.row_factory or \
-            self.connection.row_factory or \
-            tuple_row_factory
+        row_factory = (
+            self.row_factory or self.connection.row_factory or tuple_row_factory
+        )
 
         return row_factory(self, self._get_cells(row))
 
     def _get_cells(self, row: RawRow) -> Iterable[Any]:
         # See _pysqlite_fetch_one_row()
         # https://github.com/python/cpython/blob/main/Modules/_sqlite/cursor.c#L319
         # https://docs.python.org/3/library/sqlite3.html#how-to-convert-sqlite-values-to-custom-python-types
@@ -1186,16 +1213,16 @@
     _row_colname_parser_re = re.compile(
         r"^(?P<name>[^[]+)\s*\[(?P<type_name>[^]]+)\]",
     )
 
     _row_decltype_parser_re = re.compile(r"^(?P<type_name>[^ (]+)")
 
     def _get_column_description_and_cast(
-            self,
-            col: RawColumn,
+        self,
+        col: RawColumn,
     ) -> Tuple[CursorColumnDescription, Optional[ConverterCallback]]:
         name = col.get("name") or ""
         converter: Optional[ConverterCallback] = None
 
         detect_types = self.connection._detect_types
         get_converter = self.connection._get_converter
 
@@ -1254,35 +1281,31 @@
 
             return obj
         except TypeError:
             raise ProgrammingError("can't adapt")
 
     def _adapt_params(self, parameters: SqlParameters) -> SqlParameters:
         if isinstance(parameters, collections.abc.Mapping):
-            return {
-                k: self._adapt_param_value(v)
-                for k, v in parameters.items()
-            }
+            return {k: self._adapt_param_value(v) for k, v in parameters.items()}
         elif parameters:
             # SupportsLenAndGetItem is only __len__ + __getitem__, no __iter__
             # so create the list manually :-(
             return [
-                self._adapt_param_value(parameters[i])
-                for i in range(len(parameters))
+                self._adapt_param_value(parameters[i]) for i in range(len(parameters))
             ]
         return parameters
 
     @check_cursor
     def _query_execute(
-            self,
-            sql: str,
-            parameters: Iterable[SqlParameters] = ((),),
-            *,
-            multiple: bool = False,
-            want_rows: bool = True,
+        self,
+        sql: str,
+        parameters: Iterable[SqlParameters] = ((),),
+        *,
+        multiple: bool = False,
+        want_rows: bool = True,
     ) -> Self:
         if not isinstance(sql, str):
             # required by test CursorTests.test_execute_many_wrong_sql_arg()
             raise TypeError("sql must be a str")
         if not sql:
             return self
 
@@ -1302,45 +1325,47 @@
             # Locking is not that meaningful with libsql_client since
             # we don't callback to python during execution as done by
             # create_function() and the likes. Nevertheless keep it here
             # NOTE: _begin_transaction_if_needed() will call this function
             # so do not lock before this point!
             self._locked = True
             self._raw_results = self._raw_execute(
-                sql, params, want_rows=want_rows,
+                sql,
+                params,
+                want_rows=want_rows,
             )
             for result, error in self._raw_results:
                 if error is not None:
                     self._rowcount = -1  # as per cursor.c
                     _raise_converted_exception(error)
                 assert result is not None
                 self._apply_raw_results(result)
 
             self._connection._update_in_transaction(statement)
             return self
         finally:
             self._locked = False
 
     def execute(
-            self,
-            sql: str,
-            parameters: SqlParameters = (),
+        self,
+        sql: str,
+        parameters: SqlParameters = (),
     ) -> Self:
         "See :py:meth:`sqlite3.Cursor.execute`"
-        if not isinstance(parameters, collections.abc.Mapping) and \
-                not (hasattr(parameters, "__len__")
-                     and hasattr(parameters, "__getitem__")):
+        if not isinstance(parameters, collections.abc.Mapping) and not (
+            hasattr(parameters, "__len__") and hasattr(parameters, "__getitem__")
+        ):
             raise ProgrammingError("parameters are of unsupported type")
         self._query_execute(sql, (parameters,), multiple=False, want_rows=True)
         return self
 
     def executemany(
-            self,
-            sql: str,
-            parameters: Iterable[SqlParameters],
+        self,
+        sql: str,
+        parameters: Iterable[SqlParameters],
     ) -> Self:
         "See :py:meth:`sqlite3.Cursor.executemany`"
         self._query_execute(sql, parameters, multiple=True, want_rows=False)
         return self
 
     @abstractmethod
     def _raw_execute_script(self, sql_script: str) -> None:
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/hrana/client.py` & `libsql_client-0.3.1/libsql_client/hrana/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 from __future__ import annotations
-from typing import List, Optional, Set, Union
-import aiohttp
+
 import asyncio
+from typing import List
+from typing import Optional
+from typing import Set
 import urllib.parse
 
-from ..client import Client, InArgs, InStatement, LibsqlError, Transaction
+import aiohttp
+
+from . import proto
+from .conn import HranaConn
+from .conn import HranaStream
+from .convert import _batch_results_from_proto
+from .convert import _batch_to_proto
+from .convert import _result_set_from_proto
+from .convert import _stmt_to_proto
+from ..client import Client
+from ..client import InArgs
+from ..client import InStatement
+from ..client import LibsqlError
+from ..client import Transaction
 from ..config import _Config
 from ..result import ResultSet
-from . import proto
-from .conn import HranaConn, HranaStream
-from .convert import (
-    _stmt_to_proto, _result_set_from_proto,
-    _batch_to_proto, _batch_results_from_proto,
-    _error_from_proto,
-)
+
 
 def _create_hrana_client(config: _Config) -> HranaClient:
     assert config.scheme in ("ws", "wss")
-    url = urllib.parse.urlunparse((
-        config.scheme, config.authority, config.path,
-        "", "", "",
-    ))
+    url = _config_to_url(config)
     return HranaClient(url, config.auth_token)
 
+
+def _config_to_url(config: _Config) -> str:
+    if config.scheme == "ws" and config.tls:
+        raise LibsqlError(
+            "A 'ws:' URL cannot opt into TLS by using ?tls=1", "URL_INVALID"
+        )
+    elif config.scheme == "wss" and not config.tls:
+        raise LibsqlError(
+            "A 'wss:' URL cannot opt out of TLS by using ?tls=0", "URL_INVALID"
+        )
+
+    return urllib.parse.urlunparse(
+        (
+            config.scheme,
+            config.authority,
+            config.path,
+            "",
+            "",
+            "",
+        )
+    )
+
+
 class HranaClient(Client):
     _session: aiohttp.ClientSession
     _conn: HranaConn
     _close_tasks: Set[asyncio.Task[None]]
     _url: str
     _auth_token: Optional[str]
     _closed: bool
@@ -69,32 +98,37 @@
 
     def _open_conn(self) -> HranaConn:
         return HranaConn(self._session, self._url, self._auth_token)
 
     async def close(self) -> None:
         await self._conn.close()
         if len(self._close_tasks) > 0:
-            await asyncio.wait(list(self._close_tasks), return_when=asyncio.ALL_COMPLETED)
+            await asyncio.wait(
+                list(self._close_tasks), return_when=asyncio.ALL_COMPLETED
+            )
         await self._session.close()
         self._closed = True
 
     @property
     def closed(self) -> bool:
         return self._closed
 
+
 class HranaTransaction(Transaction):
     _stream: HranaStream
     _begin_fut: asyncio.Future[proto.StmtResult]
 
     def __init__(self, stream: HranaStream):
         self._stream = stream
-        self._begin_fut = stream.execute({
-            "sql": "BEGIN",
-            "want_rows": False,
-        })
+        self._begin_fut = stream.execute(
+            {
+                "sql": "BEGIN",
+                "want_rows": False,
+            }
+        )
 
     async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
         await self._begin_fut
         if self._stream.closed:
             raise LibsqlError("The transaction is closed", "TRANSACTION_CLOSED")
 
         proto_stmt = _stmt_to_proto(stmt, args)
@@ -102,30 +136,34 @@
         return _result_set_from_proto(proto_result)
 
     async def rollback(self) -> None:
         await self._begin_fut
         if self._stream.closed:
             return
 
-        fut = self._stream.execute({
-            "sql": "ROLLBACK",
-            "want_rows": False,
-        })
+        fut = self._stream.execute(
+            {
+                "sql": "ROLLBACK",
+                "want_rows": False,
+            }
+        )
         self._stream.close()
         await fut
 
     async def commit(self) -> None:
         await self._begin_fut
         if self._stream.closed:
             raise LibsqlError("The transaction is closed", "TRANSACTION_CLOSED")
 
-        fut = self._stream.execute({
-            "sql": "COMMIT",
-            "want_rows": False,
-        })
+        fut = self._stream.execute(
+            {
+                "sql": "COMMIT",
+                "want_rows": False,
+            }
+        )
         self._stream.close()
         await fut
 
     def close(self) -> None:
         self._stream.close()
 
     @property
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/hrana/conn.py` & `libsql_client-0.3.1/libsql_client/hrana/conn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from __future__ import annotations
-from dataclasses import dataclass
-from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
-import aiohttp
+
 import asyncio
+from dataclasses import dataclass
 import json
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import Dict
+from typing import Optional
+from typing import TypeVar
+from typing import Union
+
+import aiohttp
 
-from ..client import LibsqlError
 from . import proto
 from .convert import _error_from_proto
 from .id_alloc import IdAlloc
+from ..client import LibsqlError
+
 
 @dataclass
 class _ResponseState:
     type: str
     future: asyncio.Future[proto.Response]
 
+
 @dataclass
 class _StreamState:
     stream_id: int
     closed: Optional[BaseException]
 
+
 class HranaConn:
     _connect_task: asyncio.Task[aiohttp.ClientWebSocketResponse]
     _receive_task: Optional[asyncio.Task[None]]
     _send_task: Optional[asyncio.Task[None]]
 
     _socket: Optional[aiohttp.ClientWebSocketResponse]
     _send_msg_queue: asyncio.Queue[str]
@@ -33,15 +44,17 @@
     _response_map: Dict[int, _ResponseState]
     _request_id_alloc: IdAlloc
     _stream_id_alloc: IdAlloc
     _sql_id_alloc: IdAlloc
 
     exception: Optional[BaseException]
 
-    def __init__(self, session: aiohttp.ClientSession, url: str, auth_token: Optional[str] = None):
+    def __init__(
+        self, session: aiohttp.ClientSession, url: str, auth_token: Optional[str] = None
+    ):
         self._connect_task = asyncio.create_task(self._do_connect(session, url))
         self._connect_task.add_done_callback(self._done_connect)
         self._receive_task = None
         self._send_task = None
 
         self._socket = None
         self._send_msg_queue = asyncio.Queue()
@@ -58,23 +71,27 @@
         self._send({"type": "hello", "jwt": auth_token})
 
     async def wait_connected(self) -> None:
         await self._finished_handshake.wait()
         if self.exception:
             raise self.exception
 
-    async def _do_connect(self, session: aiohttp.ClientSession, url: str) -> aiohttp.ClientWebSocketResponse:
+    async def _do_connect(
+        self, session: aiohttp.ClientSession, url: str
+    ) -> aiohttp.ClientWebSocketResponse:
         return await session.ws_connect(
             url,
             protocols=["hrana2"],
             autoclose=False,
             autoping=True,
         )
 
-    def _done_connect(self, task: asyncio.Task[aiohttp.ClientWebSocketResponse]) -> None:
+    def _done_connect(
+        self, task: asyncio.Task[aiohttp.ClientWebSocketResponse]
+    ) -> None:
         e: Optional[BaseException]
         if task.cancelled():
             e = LibsqlError("The connect task was cancelled", "CLIENT_CLOSED")
         else:
             e = task.exception()
         if e is not None:
             self._set_exception(e)
@@ -95,20 +112,26 @@
 
     async def _do_receive(self, socket: aiohttp.ClientWebSocketResponse) -> None:
         while True:
             msg = await socket.receive()
             if msg.type == aiohttp.WSMsgType.TEXT:
                 try:
                     self._receive(msg.data)
-                except Exception as e:
-                    await socket.close(code=3007, message="Could not handle message".encode())
+                except Exception:
+                    await socket.close(
+                        code=3007, message="Could not handle message".encode()
+                    )
                     raise
             elif msg.type == aiohttp.WSMsgType.BINARY:
-                await socket.close(code=3003, message="Only text messages are accepted".encode())
-                raise LibsqlError("Received a binary WebSocket message", "HRANA_PROTO_ERROR")
+                await socket.close(
+                    code=3003, message="Only text messages are accepted".encode()
+                )
+                raise LibsqlError(
+                    "Received a binary WebSocket message", "HRANA_PROTO_ERROR"
+                )
             elif msg.type == aiohttp.WSMsgType.PING:
                 await socket.pong(msg.data)
             elif msg.type == aiohttp.WSMsgType.PONG:
                 pass
             elif msg.type == aiohttp.WSMsgType.CLOSE:
                 code = cast(aiohttp.WSCloseCode, msg.data)
                 reason = cast(str, msg.extra)
@@ -192,47 +215,60 @@
     def _receive(self, text: str) -> None:
         if self.exception is not None:
             return
 
         try:
             msg = json.loads(text)
         except ValueError as e:
-            raise LibsqlError("Server message is not valid JSON", "HRANA_PROTO_ERROR") from e
+            raise LibsqlError(
+                "Server message is not valid JSON", "HRANA_PROTO_ERROR"
+            ) from e
 
         if msg["type"] in ("hello_ok", "hello_error"):
             if self._recvd_hello:
-                raise LibsqlError("Received a duplicated error response", "HRANA_PROTO_ERROR")
+                raise LibsqlError(
+                    "Received a duplicated error response", "HRANA_PROTO_ERROR"
+                )
             self._recvd_hello = True
             self._finished_handshake.set()
 
             if msg["type"] == "hello_error":
                 raise _error_from_proto(msg["error"])
             return
         elif not self._recvd_hello:
-            raise LibsqlError("Received a non-hello message before hello response", "HRANA_PROTO_ERROR")
+            raise LibsqlError(
+                "Received a non-hello message before hello response",
+                "HRANA_PROTO_ERROR",
+            )
 
         if msg["type"] == "response_ok":
             request_id = int(msg["request_id"])
             response_state = self._response_map.pop(request_id, None)
             if response_state is None:
-                raise LibsqlError("Received unexpected OK response", "HRANA_PROTO_ERROR")
+                raise LibsqlError(
+                    "Received unexpected OK response", "HRANA_PROTO_ERROR"
+                )
             self._request_id_alloc.free(request_id)
 
             try:
                 if response_state.type != msg["response"]["type"]:
-                    raise LibsqlError("Received unexpected type of response", "HRANA_PROTO_ERROR")
+                    raise LibsqlError(
+                        "Received unexpected type of response", "HRANA_PROTO_ERROR"
+                    )
                 response_state.future.set_result(msg["response"])
             except Exception as e:
                 response_state.future.set_exception(e)
                 raise
         elif msg["type"] == "response_error":
             request_id = int(msg["request_id"])
             response_state = self._response_map.pop(request_id, None)
             if response_state is None:
-                raise LibsqlError("Received unexpected error response", "HRANA_PROTO_ERROR")
+                raise LibsqlError(
+                    "Received unexpected error response", "HRANA_PROTO_ERROR"
+                )
             self._request_id_alloc.free(request_id)
 
             response_state.future.set_exception(_error_from_proto(msg["error"]))
         else:
             raise LibsqlError("Received unexpected message type", "HRANA_PROTO_ERROR")
 
     def open_stream(self) -> HranaStream:
@@ -244,36 +280,40 @@
             if fut.cancelled():
                 e = asyncio.CancelledError("Stream opening was cancelled")
             else:
                 e = fut.exception()
             if e is not None:
                 self._close_stream(stream_state, e)
 
-        open_fut = self.send_request({
-            "type": "open_stream",
-            "stream_id": stream_id,
-        })
+        open_fut = self.send_request(
+            {
+                "type": "open_stream",
+                "stream_id": stream_id,
+            }
+        )
         open_fut.add_done_callback(open_done)
 
         return HranaStream(self, stream_state)
 
     def _close_stream(self, stream_state: _StreamState, e: BaseException) -> None:
         if stream_state.closed is not None or self.exception is not None:
             return
         stream_state.closed = e
 
         def close_done(fut: asyncio.Future[proto.Response]) -> None:
             self._stream_id_alloc.free(stream_state.stream_id)
             if not fut.cancelled():
                 fut.exception()
 
-        close_fut = self.send_request({
-            "type": "close_stream",
-            "stream_id": stream_state.stream_id,
-        })
+        close_fut = self.send_request(
+            {
+                "type": "close_stream",
+                "stream_id": stream_state.stream_id,
+            }
+        )
         close_fut.add_done_callback(close_done)
 
     async def close(self) -> None:
         self._set_exception(LibsqlError("Client was manually closed", "CLIENT_CLOSED"))
         if self._socket is not None:
             await self._socket.close()
 
@@ -285,64 +325,73 @@
             if fut.cancelled():
                 e = asyncio.CancelledError("store_sql was cancelled")
             else:
                 e = fut.exception()
             if e is not None:
                 self._sql_id_alloc.free(sql_id)
 
-        store_sql_fut = self.send_request({
-            "type": "store_sql",
-            "sql_id": sql_id,
-            "sql": sql,
-        })
+        store_sql_fut = self.send_request(
+            {
+                "type": "store_sql",
+                "sql_id": sql_id,
+                "sql": sql,
+            }
+        )
         store_sql_fut.add_done_callback(store_sql_done)
         return sql_id
 
     def close_sql(self, sql_id: int) -> None:
         if self.exception is not None:
             return
 
         def close_sql_done(fut: asyncio.Future[proto.Response]) -> None:
             self._sql_id_alloc.free(sql_id)
             if not fut.cancelled():
                 fut.exception()
 
-        close_sql_fut = self.send_request( {
-            "type": "close_sql",
-            "sql_id": sql_id,
-        })
+        close_sql_fut = self.send_request(
+            {
+                "type": "close_sql",
+                "sql_id": sql_id,
+            }
+        )
         close_sql_fut.add_done_callback(close_sql_done)
 
 
 class HranaStream:
     _conn: HranaConn
     _state: _StreamState
 
     def __init__(self, conn: HranaConn, state: _StreamState):
         self._conn = conn
         self._state = state
 
     def execute(self, stmt: proto.Stmt) -> asyncio.Future[proto.StmtResult]:
         if self._state.closed is not None:
-            raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
+            raise LibsqlError(
+                "Stream was closed", "STREAM_CLOSED"
+            ) from self._state.closed
 
         request: proto.ExecuteReq = {
             "type": "execute",
             "stream_id": self._state.stream_id,
             "stmt": stmt,
         }
         response_fut = self._conn.send_request(request)
 
         def get_result(response: proto.Response) -> proto.StmtResult:
             return cast(proto.ExecuteResp, response)["result"]
+
         return _map_future(response_fut, get_result)
 
     def sequence(self, stmt: Union[str, int]) -> asyncio.Future[None]:
         if self._state.closed is not None:
-            raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
+            raise LibsqlError(
+                "Stream was closed", "STREAM_CLOSED"
+            ) from self._state.closed
 
         request: proto.SequenceReq
         if isinstance(stmt, str):
             request = {
                 "type": "sequence",
                 "stream_id": self._state.stream_id,
                 "sql": stmt,
@@ -354,29 +403,33 @@
                 "sql_id": stmt,
             }
 
         response_fut = self._conn.send_request(request)
 
         def get_result(response: proto.Response) -> None:
             return None
+
         return _map_future(response_fut, get_result)
 
     def batch(self, batch: proto.Batch) -> asyncio.Future[proto.BatchResult]:
         if self._state.closed is not None:
-            raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
+            raise LibsqlError(
+                "Stream was closed", "STREAM_CLOSED"
+            ) from self._state.closed
 
         request: proto.BatchReq = {
             "type": "batch",
             "stream_id": self._state.stream_id,
             "batch": batch,
         }
         response_fut = self._conn.send_request(request)
 
         def get_result(response: proto.Response) -> proto.BatchResult:
             return cast(proto.BatchResp, response)["result"]
+
         return _map_future(response_fut, get_result)
 
     def close(self) -> None:
         e = LibsqlError("Stream was manually closed", "STREAM_CLOSED")
         self._conn._close_stream(self._state, e)
 
     @property
@@ -385,23 +438,27 @@
 
     def __enter__(self) -> HranaStream:
         return self
 
     def __exit__(self, _exc_type: Any, _exc_value: Any, _traceback: Any) -> None:
         self.close()
 
+
 T = TypeVar("T")
 R = TypeVar("R")
 
+
 def _map_future(fut: asyncio.Future[T], f: Callable[[T], R]) -> asyncio.Future[R]:
     ret: asyncio.Future[R] = asyncio.get_running_loop().create_future()
+
     def done(fut: asyncio.Future[T]) -> None:
         if fut.cancelled():
             ret.cancel()
             return
         e = fut.exception()
         if e is None:
             ret.set_result(f(fut.result()))
         else:
             ret.set_exception(e)
+
     fut.add_done_callback(done)
     return ret
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/hrana/convert.py` & `libsql_client-0.3.1/libsql_client/hrana/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from __future__ import annotations
-from typing import List
+
 import base64
 import math
+from typing import List
 
-from ..client import InArgs, InValue, InStatement, LibsqlError, Statement, _normalize_value
-from ..result import ResultSet, Row, Value
 from . import proto
+from ..client import _normalize_value
+from ..client import InArgs
+from ..client import InStatement
+from ..client import InValue
+from ..client import LibsqlError
+from ..client import Statement
+from ..result import ResultSet
+from ..result import Row
+from ..result import Value
+
 
 def _stmt_to_proto(in_stmt: InStatement, in_args: InArgs = None) -> proto.Stmt:
     stmt = Statement.convert(in_stmt, in_args)
     args: List[proto.Value] = []
     named_args: List[proto.NamedArg] = []
     if stmt.args is None:
         pass
@@ -18,114 +27,142 @@
             {"name": key, "value": _value_to_proto(value)}
             for key, value in stmt.args.items()
         ]
     else:
         args = [_value_to_proto(value) for value in stmt.args]
     return {"sql": stmt.sql, "args": args, "named_args": named_args, "want_rows": True}
 
+
 def _result_set_from_proto(proto_res: proto.StmtResult) -> ResultSet:
     columns = tuple(proto_col["name"] or "" for proto_col in proto_res["cols"])
     column_idxs = {column: idx for idx, column in enumerate(columns)}
     rows = []
     for proto_row in proto_res["rows"]:
         values = tuple(_value_from_proto(proto_val) for proto_val in proto_row)
         rows.append(Row(column_idxs, values))
     rows_affected = proto_res["affected_row_count"]
     last_insert_rowid_str = proto_res.get("last_insert_rowid")
-    last_insert_rowid = int(last_insert_rowid_str) if last_insert_rowid_str is not None else None
+    last_insert_rowid = (
+        int(last_insert_rowid_str) if last_insert_rowid_str is not None else None
+    )
     return ResultSet(columns, rows, rows_affected, last_insert_rowid)
 
+
 def _batch_to_proto(in_stmts: List[InStatement]) -> proto.Batch:
     steps: List[proto.BatchStep] = []
-    steps.append({
-        "stmt": {"sql": "BEGIN", "want_rows": False},
-    })
+    steps.append(
+        {
+            "stmt": {"sql": "BEGIN", "want_rows": False},
+        }
+    )
 
     for in_stmt in in_stmts:
-        steps.append({
+        steps.append(
+            {
+                "condition": {
+                    "type": "ok",
+                    "step": len(steps) - 1,
+                },
+                "stmt": _stmt_to_proto(in_stmt),
+            }
+        )
+
+    steps.append(
+        {
             "condition": {
                 "type": "ok",
                 "step": len(steps) - 1,
             },
-            "stmt": _stmt_to_proto(in_stmt),
-        })
-
-    steps.append({
-        "condition": {
-            "type": "ok",
-            "step": len(steps) - 1,
-        },
-        "stmt": {"sql": "COMMIT", "want_rows": False},
-    })
-    steps.append({
-        "condition": {
-            "type": "not",
-            "cond": {
-                "type": "ok",
-                "step": len(steps) - 1,
+            "stmt": {"sql": "COMMIT", "want_rows": False},
+        }
+    )
+    steps.append(
+        {
+            "condition": {
+                "type": "not",
+                "cond": {
+                    "type": "ok",
+                    "step": len(steps) - 1,
+                },
             },
-        },
-        "stmt": {"sql": "ROLLBACK", "want_rows": False},
-    })
+            "stmt": {"sql": "ROLLBACK", "want_rows": False},
+        }
+    )
 
     return {"steps": steps}
 
-def _batch_results_from_proto(proto_res: proto.BatchResult, stmt_count: int) -> List[ResultSet]:
+
+def _batch_results_from_proto(
+    proto_res: proto.BatchResult, stmt_count: int
+) -> List[ResultSet]:
     if len(proto_res["step_results"]) != stmt_count + 3:
-        raise LibsqlError("Server did not return the expected number of batch results", "HRANA_PROTO_ERROR")
+        raise LibsqlError(
+            "Server did not return the expected number of batch results",
+            "HRANA_PROTO_ERROR",
+        )
     if len(proto_res["step_errors"]) != stmt_count + 3:
-        raise LibsqlError("Server did not return the expected number of batch errors", "HRANA_PROTO_ERROR")
+        raise LibsqlError(
+            "Server did not return the expected number of batch errors",
+            "HRANA_PROTO_ERROR",
+        )
 
     for proto_err in proto_res["step_errors"]:
         if proto_err is not None:
             raise _error_from_proto(proto_err)
 
     result_sets = []
     for stmt_res in proto_res["step_results"][1:-2]:
         if stmt_res is None:
-            raise LibsqlError("Server did not return a result in batch", "HRANA_PROTO_ERROR")
+            raise LibsqlError(
+                "Server did not return a result in batch", "HRANA_PROTO_ERROR"
+            )
         result_sets.append(_result_set_from_proto(stmt_res))
     return result_sets
 
+
 def _error_from_proto(proto_err: proto.Error) -> LibsqlError:
     message = proto_err["message"]
     code = proto_err.get("code") or "UNKNOWN"
     return LibsqlError(message, code)
 
+
 def _value_to_proto(in_value: InValue) -> proto.Value:
     value = _normalize_value(in_value)
     if value is None:
         return {"type": "null"}
     elif isinstance(value, str):
         return {"type": "text", "value": value}
     elif isinstance(value, int):
         if value < _MIN_INTEGER or value > _MAX_INTEGER:
-            raise OverflowError("Integer exceeds the range of SQLite integers (64 bits, signed)")
+            raise OverflowError(
+                "Integer exceeds the range of SQLite integers (64 bits, signed)"
+            )
         return {"type": "integer", "value": str(value)}
     elif isinstance(value, float):
         if not math.isfinite(value):
             raise ValueError("Only finite floats (not Infinity or NaN) are supported")
         return {"type": "float", "value": value}
     else:
         try:
             data = base64.b64encode(value).decode()
-            return {"type": "blob", "base64": data }
+            return {"type": "blob", "base64": data}
         except TypeError:
             raise TypeError(f"Unsupported value of type {type(value)}")
 
-_MIN_INTEGER = -2**63
-_MAX_INTEGER = 2**63-1
+
+_MIN_INTEGER = -(2**63)
+_MAX_INTEGER = 2**63 - 1
+
 
 def _value_from_proto(value: proto.Value) -> Value:
     if value["type"] == "null":
         return None
     elif value["type"] == "text":
         return str(value["value"])
     elif value["type"] == "integer":
         return int(value["value"])
     elif value["type"] == "float":
         return float(value["value"])
     elif value["type"] == "blob":
         return base64.b64decode(value["base64"] + "====")
     else:
         raise LibsqlError(f"Unknown value type {value['type']!r}", "HRANA_PROTO_ERROR")
-
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/hrana/id_alloc.py` & `libsql_client-0.3.1/libsql_client/hrana/id_alloc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from __future__ import annotations
+
 from typing import Set
 
+
 # An allocator of non-negative integer ids.
 #
 # This clever data structure has these "ideal" properties:
 # - It consumes memory proportional to the number of used ids (which is optimal).
 # - All operations are O(1) time.
-# - The allocated ids are small (with a slight modification, we could always provide the smallest possible
+# - The allocated ids are small (with a slight modification, we could always
+#   provide the smallest possible
 # id).
 class IdAlloc:
     # Set of all allocated ids
     _used_ids: Set[int]
     # Set of all free ids lower than `len(_used_ids)`
     _free_ids: Set[int]
 
@@ -24,17 +28,17 @@
             self._used_ids.add(free_id)
 
             # maintain the invariant of `_free_ids`
             if (len(self._used_ids) - 1) not in self._used_ids:
                 self._free_ids.add(len(self._used_ids) - 1)
             return free_id
 
-        # the `_free_ids` set is empty, so there are no free ids lower than `len(_used_ids)`
-        # this means that `_used_ids` is a set that contains all numbers from 0 to `len(_used_ids) - 1`,
-        # so `len(_used_ids)` is free
+        # the `_free_ids` set is empty, so there are no free ids lower than
+        # `len(_used_ids)` this means that `_used_ids` is a set that contains all
+        # numbers from 0 to `len(_used_ids) - 1`, so `len(_used_ids)` is free
         free_id = len(self._used_ids)
         self._used_ids.add(free_id)
         return free_id
 
     def free(self, used_id: int) -> None:
         self._used_ids.remove(used_id)
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/http.py` & `libsql_client-0.3.1/libsql_client/http.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,56 @@
 from __future__ import annotations
-from typing import Any, List, Optional, Union, cast
-from typing_extensions import TypedDict
-import aiohttp
+
+from typing import Any
+from typing import cast
+from typing import List
+from typing import Optional
 import urllib.parse
 
-from .client import Client, InArgs, InStatement, LibsqlError, Transaction
+import aiohttp
+from typing_extensions import TypedDict
+
+from .client import Client
+from .client import InArgs
+from .client import InStatement
+from .client import LibsqlError
+from .client import Transaction
 from .config import _Config
 from .hrana import proto
-from .hrana.convert import (
-    _stmt_to_proto, _result_set_from_proto,
-    _batch_to_proto, _batch_results_from_proto,
-)
+from .hrana.convert import _batch_results_from_proto
+from .hrana.convert import _batch_to_proto
+from .hrana.convert import _result_set_from_proto
+from .hrana.convert import _stmt_to_proto
 from .result import ResultSet
 
+
 def _create_http_client(config: _Config) -> HttpClient:
     assert config.scheme in ("http", "https")
-    url = urllib.parse.urlunparse((
-        config.scheme, config.authority, config.path,
-        "", "", "",
-    ))
+    if config.scheme == "http" and config.tls:
+        raise LibsqlError(
+            "A 'http:' URL cannot opt into TLS by using ?tls=1", "URL_INVALID"
+        )
+    elif config.scheme == "https" and not config.tls:
+        raise LibsqlError(
+            "A 'https:' URL cannot opt out of TLS by using ?tls=0", "URL_INVALID"
+        )
+
+    url = urllib.parse.urlunparse(
+        (
+            config.scheme,
+            config.authority,
+            config.path,
+            "",
+            "",
+            "",
+        )
+    )
     return HttpClient(url, auth_token=config.auth_token)
 
+
 class HttpClient(Client):
     _session: aiohttp.ClientSession
     _url: str
 
     def __init__(self, url: str, *, auth_token: Optional[str] = None):
         headers = {"authorization": f"Bearer {auth_token}"}
         self._session = aiohttp.ClientSession(headers=headers)
@@ -51,15 +77,16 @@
         response = await self._send("POST", "v1/batch", request)
         proto_res = cast(_BatchResp, response)["result"]
         return _batch_results_from_proto(proto_res, len(stmts))
 
     def transaction(self) -> Transaction:
         raise LibsqlError(
             "The HTTP client does not support transactions. "
-            "Please use a libsql:, ws: or wss: URL, so that the client connects using a WebSocket.",
+            "Please use a libsql:, ws: or wss: URL, so that the client "
+            "connects using a WebSocket.",
             "TRANSACTIONS_NOT_SUPPORTED",
         )
 
     async def close(self) -> None:
         await self._session.close()
 
     @property
@@ -75,27 +102,43 @@
                     if "message" in resp_json:
                         message = resp_json["message"]
                         code = resp_json.get("code") or "UNKNOWN"
                         raise LibsqlError(message, code)
                 elif resp.content_type == "text/plain":
                     resp_text = await resp.text()
                     raise LibsqlError(
-                        f"Server returned HTTP status {resp.status} and error: {resp_text!r}",
+                        "Server returned HTTP status "
+                        f"{resp.status} and error: {resp_text!r}",
                         "SERVER_ERROR",
                     )
-                raise LibsqlError(f"Server returned HTTP status {resp.status}", "SERVER_ERROR")
+                raise LibsqlError(
+                    f"Server returned HTTP status {resp.status}", "SERVER_ERROR"
+                )
 
             return await resp.json()
 
-_ExecuteReq = TypedDict("_ExecuteReq", {
-    "stmt": proto.Stmt,
-})
-_ExecuteResp = TypedDict("_ExecuteResp", {
-    "result": proto.StmtResult,
-})
-
-_BatchReq = TypedDict("_BatchReq", {
-    "batch": proto.Batch,
-})
-_BatchResp = TypedDict("_BatchResp", {
-    "result": proto.BatchResult,
-})
+
+_ExecuteReq = TypedDict(
+    "_ExecuteReq",
+    {
+        "stmt": proto.Stmt,
+    },
+)
+_ExecuteResp = TypedDict(
+    "_ExecuteResp",
+    {
+        "result": proto.StmtResult,
+    },
+)
+
+_BatchReq = TypedDict(
+    "_BatchReq",
+    {
+        "batch": proto.Batch,
+    },
+)
+_BatchResp = TypedDict(
+    "_BatchResp",
+    {
+        "result": proto.BatchResult,
+    },
+)
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/result.py` & `libsql_client-0.3.1/libsql_client/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from __future__ import annotations
+
 from collections.abc import Sequence
-from typing import Dict, Iterator, List, Optional, Tuple, Union, overload
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Optional
+from typing import overload
+from typing import Tuple
+from typing import Union
 
 Value = Union[None, str, int, float, bytes]
 
+
 class ResultSet:
     """Result of an SQL statement.
 
-    The result is composed of columns and rows. Every row is represented as a `Row` object and the length of
+    The result is composed of columns and rows.
+    Every row is represented as a `Row` object and the length of
     every row is equal to the number of columns.
     """
 
     _columns: Tuple[str, ...]
     _rows: List[Row]
     _rows_affected: int
     _last_insert_rowid: Optional[int]
@@ -32,17 +41,20 @@
     def __iter__(self) -> Iterator["Row"]:
         return self._rows.__iter__()
 
     def __len__(self) -> int:
         return len(self._rows)
 
     @overload
-    def __getitem__(self, key: int) -> Row: pass
+    def __getitem__(self, key: int) -> Row:
+        pass
+
     @overload
-    def __getitem__(self, key: slice) -> List[Row]: pass
+    def __getitem__(self, key: slice) -> List[Row]:
+        pass
 
     def __getitem__(self, key: Union[int, slice]) -> Union[Row, List[Row]]:
         return self._rows[key]
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self._columns
@@ -55,14 +67,15 @@
     def rows_affected(self) -> int:
         return self._rows_affected
 
     @property
     def last_insert_rowid(self) -> Optional[int]:
         return self._last_insert_rowid
 
+
 class Row(Sequence):
     """A row returned by an SQL statement.
 
     The row values can be accessed with an index or by name.
     """
 
     _column_idxs: Dict[str, int]
@@ -70,21 +83,28 @@
     __slots__ = ["_column_idxs", "_values"]
 
     def __init__(self, column_idxs: Dict[str, int], values: Tuple[Value, ...]) -> None:
         self._column_idxs = column_idxs
         self._values = values
 
     @overload
-    def __getitem__(self, key: int) -> Value: pass
+    def __getitem__(self, key: int) -> Value:
+        pass
+
     @overload
-    def __getitem__(self, key: str) -> Value: pass
+    def __getitem__(self, key: str) -> Value:
+        pass
+
     @overload
-    def __getitem__(self, key: slice) -> Tuple[Value, ...]: pass
+    def __getitem__(self, key: slice) -> Tuple[Value, ...]:
+        pass
 
-    def __getitem__(self, key: Union[int, str, slice]) -> Union[Value, Tuple[Value, ...]]:
+    def __getitem__(
+        self, key: Union[int, str, slice]
+    ) -> Union[Value, Tuple[Value, ...]]:
         """Access a value by index or by name."""
         tuple_key: Union[int, slice]
         if isinstance(key, str):
             tuple_key = self._column_idxs[key]
         else:
             tuple_key = key
         return self._values[tuple_key]
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/sqlite3.py` & `libsql_client-0.3.1/libsql_client/sqlite3_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 from __future__ import annotations
-from datetime import datetime
-from typing import Any, List, Optional, Tuple, cast
-import asyncio
+
 import math
 import sqlite3
-
-from .client import (
-    Client, InArgs, InStatement, InValue,
-    LibsqlError, Statement, Transaction,
-    _normalize_value,
-)
+from typing import Any
+from typing import cast
+from typing import List
+from typing import Optional
+
+from .client import _normalize_value
+from .client import Client
+from .client import InArgs
+from .client import InStatement
+from .client import InValue
+from .client import LibsqlError
+from .client import Statement
+from .client import Transaction
 from .config import _Config
-from .result import ResultSet, Row, Value
+from .result import ResultSet
+from .result import Row
+
 
 def _create_sqlite3_client(config: _Config) -> Sqlite3Client:
     assert config.scheme == "file"
     if config.authority not in ("", "localhost"):
-        raise LibsqlError(f"Invalid authority in file URL: {config.authority!r}", "URL_INVALID")
+        raise LibsqlError(
+            f"Invalid authority in file URL: {config.authority!r}", "URL_INVALID"
+        )
 
     client = Sqlite3Client(config.path)
     db = client._connect()
     try:
         _execute_stmt(db, "SELECT 1 AS check_that_the_database_can_be_opened")
     finally:
         db.close()
 
     return client
 
+
 class Sqlite3Client(Client):
     _path: str
     _closed: bool
 
     def __init__(self, path: str):
-        self._path = path;
+        self._path = path
         self._closed = False
 
     async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
         db = self._connect()
         try:
             return _execute_stmt(db, stmt, args)
         finally:
@@ -77,14 +87,15 @@
         return sqlite3.connect(
             self._path,
             isolation_level=None,
             check_same_thread=False,
             timeout=0,
         )
 
+
 class Sqlite3Transaction(Transaction):
     database: Optional[sqlite3.Connection]
 
     def __init__(self, database: sqlite3.Connection):
         self.database = database
 
     async def execute(self, stmt: InStatement, args: InArgs = None) -> ResultSet:
@@ -112,21 +123,27 @@
         return self.database is None
 
     def _connection(self) -> sqlite3.Connection:
         if self.database is None:
             raise LibsqlError("The transaction was closed", "TRANSACTION_CLOSED")
         return self.database
 
-def _execute_stmt(db: sqlite3.Connection, in_stmt: InStatement, in_args: InArgs = None) -> ResultSet:
+
+def _execute_stmt(
+    db: sqlite3.Connection, in_stmt: InStatement, in_args: InArgs = None
+) -> ResultSet:
     stmt = Statement.convert(in_stmt, in_args)
     sql_args: Any
     if stmt.args is None:
         sql_args = ()
     elif isinstance(stmt.args, dict):
-        sql_args = {_strip_arg_name(key): _value_to_sql(value) for key, value in stmt.args.items()}
+        sql_args = {
+            _strip_arg_name(key): _value_to_sql(value)
+            for key, value in stmt.args.items()
+        }
     else:
         sql_args = [_value_to_sql(value) for value in stmt.args]
 
     cursor = None
     try:
         cursor = db.execute(stmt.sql, sql_args)
         sql_rows = cursor.fetchall()
@@ -146,16 +163,18 @@
         rows = [Row(column_idxs, sql_row) for sql_row in sql_rows]
         rows_affected = cursor.rowcount
         last_insert_rowid = cursor.lastrowid
         return ResultSet(columns, rows, rows_affected, last_insert_rowid)
     finally:
         cursor.close()
 
+
 def _strip_arg_name(name: str) -> str:
     if len(name) >= 1 and name[0] in (":", "$", "@"):
         return name[1:]
     return name
 
+
 def _value_to_sql(value: InValue) -> Any:
     if isinstance(value, float) and not math.isfinite(value):
         raise ValueError("Only finite floats (not Infinity or NaN) are supported")
     return _normalize_value(value)
```

### Comparing `libsql_client-0.3.0rc0/libsql_client/sync.py` & `libsql_client-0.3.1/libsql_client/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 from __future__ import annotations
-from dataclasses import dataclass
-from typing import Any, Callable, Coroutine, Deque, List, Optional, TypeVar
+
 import asyncio
 import collections
 import concurrent
+from dataclasses import dataclass
 import threading
-
-from .client import Client, InArgs, InStatement, LibsqlError, Transaction
+from typing import Any
+from typing import Callable
+from typing import Coroutine
+from typing import Deque
+from typing import List
+from typing import Optional
+from typing import TypeVar
+
+from .client import Client
+from .client import InArgs
+from .client import InStatement
+from .client import LibsqlError
+from .client import Transaction
 from .create_client import create_client
-from .result import ResultSet, Value
+from .result import ResultSet
 
 T = TypeVar("T")
 
+
 def create_client_sync(*args: Any, **kwargs: Any) -> ClientSync:
     executor = _AsyncExecutor()
     try:
         client: Client = executor.submit_func(lambda: create_client(*args, **kwargs))
         return ClientSync(executor, client)
     except Exception:
         executor.close()
         raise
 
+
 class ClientSync:
     _executor: _AsyncExecutor
     _client: Client
 
     def __init__(self, executor: _AsyncExecutor, client: Client):
         self._executor = executor
         self._client = client
@@ -48,14 +61,15 @@
 
     def __enter__(self) -> ClientSync:
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.close()
 
+
 class TransactionSync:
     _executor: _AsyncExecutor
     _transaction: Transaction
 
     def __init__(self, executor: _AsyncExecutor, transaction: Transaction):
         self._executor = executor
         self._transaction = transaction
@@ -70,27 +84,31 @@
         return self._executor.submit_coro(self._transaction.commit())
 
     def close(self) -> None:
         self._executor.submit_func_unless_closed(self._transaction.close, lambda: None)
 
     @property
     def closed(self) -> bool:
-        return self._executor.submit_func_unless_closed(lambda: self._transaction.closed, lambda: True)
+        return self._executor.submit_func_unless_closed(
+            lambda: self._transaction.closed, lambda: True
+        )
 
     def __enter__(self) -> TransactionSync:
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.close()
 
+
 @dataclass
 class _QueueItem:
     coroutine: Coroutine[Any, Any, Any]
     future: concurrent.futures.Future
 
+
 class _AsyncExecutor:
     _thread: threading.Thread
     _loop: asyncio.AbstractEventLoop
 
     _lock: threading.Lock
     _closed: bool
     _queue: Deque[Optional[_QueueItem]]
@@ -124,15 +142,17 @@
             except Exception as e:
                 item.future.set_exception(e)
 
         with self._lock:
             self._closed = True
             for item in self._queue:
                 if item is not None:
-                    item.future.set_exception(LibsqlError("Client is closed", "CLIENT_CLOSED"))
+                    item.future.set_exception(
+                        LibsqlError("Client is closed", "CLIENT_CLOSED")
+                    )
             self._queue.clear()
 
     async def _dequeue_item(self) -> Optional[_QueueItem]:
         while True:
             with self._lock:
                 if len(self._queue) > 0:
                     return self._queue.popleft()
@@ -142,60 +162,70 @@
             await waker
 
     def _enqueue_item_with_lock(self, item: Optional[_QueueItem]) -> None:
         self._queue.append(item)
         waker, self._waker = self._waker, None
         if waker is not None:
             waker_: asyncio.Future[None] = waker
+
             def resolve_waker() -> None:
                 waker_.set_result(None)
+
             self._loop.call_soon_threadsafe(resolve_waker)
 
     def submit_coro(self, coro: Coroutine[Any, Any, T]) -> T:
         with self._lock:
             if self._closed:
                 raise LibsqlError("Client is closed", "CLIENT_CLOSED")
             fut: concurrent.futures.Future = concurrent.futures.Future()
             self._enqueue_item_with_lock(_QueueItem(coro, fut))
         return fut.result()
 
     def submit_func(self, func: Callable[[], T]) -> T:
         async def coro() -> T:
             return func()
+
         return self.submit_coro(coro())
 
-    def submit_func_unless_closed(self, on_open: Callable[[], T], on_closed: Callable[[], T]) -> T:
+    def submit_func_unless_closed(
+        self, on_open: Callable[[], T], on_closed: Callable[[], T]
+    ) -> T:
         async def on_open_coro() -> T:
             return on_open()
+
         with self._lock:
             if self._closed:
                 return on_closed()
             fut: concurrent.futures.Future = concurrent.futures.Future()
             self._enqueue_item_with_lock(_QueueItem(on_open_coro(), fut))
         return fut.result()
 
-    def close_with_coro(self, coro_func: Callable[[], Coroutine[Any, Any, None]]) -> None:
+    def close_with_coro(
+        self, coro_func: Callable[[], Coroutine[Any, Any, None]]
+    ) -> None:
         with self._lock:
             if self._closed:
                 return
             fut: concurrent.futures.Future = concurrent.futures.Future()
             self._enqueue_item_with_lock(_QueueItem(coro_func(), fut))
             self._enqueue_item_with_lock(None)
         self._thread.join()
         fut.result()
 
     def close(self) -> None:
         async def noop() -> None:
             return None
+
         self.close_with_coro(noop)
 
     def is_closed(self) -> bool:
         with self._lock:
             return self._closed
 
+
 # this is copied from CPython's Lib/asyncio/runners.py
 def _cancel_all_tasks(loop: asyncio.AbstractEventLoop) -> None:
     to_cancel = asyncio.all_tasks(loop)
     if not to_cancel:
         return
 
     for task in to_cancel:
@@ -203,12 +233,14 @@
 
     loop.run_until_complete(asyncio.gather(*to_cancel, return_exceptions=True))
 
     for task in to_cancel:
         if task.cancelled():
             continue
         if task.exception() is not None:
-            loop.call_exception_handler({
-                "message": "unhandled exception during _AsyncExecutor shutdown",
-                "exception": task.exception(),
-                "task": task,
-            })
+            loop.call_exception_handler(
+                {
+                    "message": "unhandled exception during _AsyncExecutor shutdown",
+                    "exception": task.exception(),
+                    "task": task,
+                }
+            )
```

### Comparing `libsql_client-0.3.0rc0/PKG-INFO` & `libsql_client-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: libsql-client
-Version: 0.3.0rc0
+Version: 0.3.1
 Summary: Python SDK for libSQL
 Home-page: https://github.com/libsql/libsql-client-py
 License: MIT
 Author: Gustavo Barbieri
 Author-email: barbieri@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.0,<4.0)
+Requires-Dist: sphinx-press-theme (>=0.8.0,<0.9.0)
 Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Documentation, https://libsql.org/libsql-client-py/
 Project-URL: Repository, https://github.com/libsql/libsql-client-py
 Description-Content-Type: text/markdown
 
 # Python SDK for libSQL
 
@@ -27,14 +29,16 @@
 
 [reference]: https://libsql.org/libsql-client-py/reference.html
 [github]: https://github.com/libsql/libsql-client-py
 [pypi]: https://pypi.org/project/libsql-client/
 
 This is the source repository of the Python SDK for libSQL. You can either connect to a local SQLite database or to a remote libSQL server ([sqld][sqld]).
 
+> **_NOTE:_**  If you want to use libSQL with SQLAlchemy, you should check out the [libSQL dialect](https://github.com/libsql/sqlalchemy-libsql).
+
 [sqld]: https://github.com/libsql/sqld
 
 ## Installation
 
 ```
 pip install libsql-client
 ```
```

