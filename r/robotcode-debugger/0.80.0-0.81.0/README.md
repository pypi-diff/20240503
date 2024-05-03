# Comparing `tmp/robotcode_debugger-0.80.0.tar.gz` & `tmp/robotcode_debugger-0.81.0.tar.gz`

## Comparing `robotcode_debugger-0.80.0.tar` & `robotcode_debugger-0.81.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15859 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/LICENSE.txt
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/README.md
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/pyproject.toml
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/LICENSE.txt
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/README.md
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 robotcode_debugger-0.81.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from typing import Optional, Sequence, Tuple
 
 import click
 
 from robotcode.core.types import ServerMode
 from robotcode.plugin import Application, UnknownError, pass_application
 from robotcode.plugin.click_helper.options import (
@@ -18,27 +17,28 @@
 
 
 @click.command(
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
     add_help_option=True,
 )
 @click.option(
-    "--debug / --no-debug",
+    "--debug/--no-debug",
+    is_flag=True,
     default=True,
     help="Enable/disable debug mode",
     show_default=True,
 )
 @click.option(
     "--stop-on-entry / --no-stop-on-entry",
     is_flag=True,
     help="Breaks into debugger when a robot framework run starts.",
     show_default=True,
 )
 @click.option(
-    "--wait-for-client / --no-wait-for-client",
+    "--wait-for-client/--no-wait-for-client",
     is_flag=True,
     default=True,
     help="Waits until a debug client is connected.",
     show_default=True,
 )
 @click.option(
     "--wait-for-client-timeout",
@@ -51,22 +51,22 @@
     "--configuration-done-timeout",
     type=float,
     default=10,
     help="Timeout to wait for a configuration from client.",
     show_default=True,
 )
 @click.option(
-    "--debugpy / --no-debugpy",
+    "--debugpy/--no-debugpy",
     is_flag=True,
     default=False,
     help="Enable/disable python debugging.",
     show_default=True,
 )
 @click.option(
-    "--debugpy-wait-for-client",
+    "--debugpy-wait-for-client/--no-debugpy-wait-for-client",
     is_flag=True,
     default=True,
     help="Waits for a debugpy client to connect.",
     show_default=False,
 )
 @click.option(
     "--debugpy-port",
@@ -166,36 +166,34 @@
     app.verbose(f"Output timestamps: {output_timestamps}")
     app.verbose(f"Group output: {group_output}")
     app.verbose(f"Stop in entry: {stop_on_entry}")
     app.verbose(f"Robot options and args: {robot_options_and_args}")
 
     try:
         app.exit(
-            asyncio.run(
-                run_debugger(
-                    ctx=ctx,
-                    app=app,
-                    args=list(robot_options_and_args),
-                    mode=mode,
-                    addresses=bind,
-                    port=port if port is not None else DEBUGGER_DEFAULT_PORT,
-                    pipe_name=pipe_name,
-                    debug=debug,
-                    stop_on_entry=stop_on_entry,
-                    wait_for_client=wait_for_client,
-                    wait_for_client_timeout=wait_for_client_timeout,
-                    configuration_done_timeout=configuration_done_timeout,
-                    debugpy=debugpy,
-                    debugpy_wait_for_client=debugpy_wait_for_client,
-                    debugpy_port=debugpy_port,
-                    output_messages=output_messages,
-                    output_log=output_log,
-                    output_timestamps=output_timestamps,
-                    group_output=group_output,
-                )
+            run_debugger(
+                ctx=ctx,
+                app=app,
+                args=list(robot_options_and_args),
+                mode=mode,
+                addresses=bind,
+                port=port if port is not None else DEBUGGER_DEFAULT_PORT,
+                pipe_name=pipe_name,
+                debug=debug,
+                stop_on_entry=stop_on_entry,
+                wait_for_client=wait_for_client,
+                wait_for_client_timeout=wait_for_client_timeout,
+                configuration_done_timeout=configuration_done_timeout,
+                debugpy=debugpy,
+                debugpy_wait_for_client=debugpy_wait_for_client,
+                debugpy_port=debugpy_port,
+                output_messages=output_messages,
+                output_log=output_log,
+                output_timestamps=output_timestamps,
+                group_output=group_output,
             )
         )
 
     except SystemExit:
         raise
     except KeyboardInterrupt:
         app.keyboard_interrupt()
```

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import asyncio
 import inspect
 import json
 import threading
 import traceback
 from collections import OrderedDict
 from typing import (
@@ -138,15 +136,15 @@
             self._logger.exception(e)
             self.send_error(
                 f"Invalid Message: {type(e).__name__}: {e!s} -> {body!s}\n{traceback.format_exc()}",
                 error_message=Message(traceback.format_exc()),
             )
 
     def _handle_messages(self, iterator: Iterator[ProtocolMessage]) -> None:
-        def done(f: asyncio.Future[Any]) -> None:
+        def done(f: "asyncio.Future[Any]") -> None:
             ex = f.exception()
             if ex is not None and not isinstance(ex, asyncio.CancelledError):
                 self._logger.exception(ex, exc_info=ex)
 
         for m in iterator:
             task = asyncio.create_task(self.handle_message(m), name="handle_message")
             task.add_done_callback(done)
@@ -245,23 +243,22 @@
                 result = asyncio.create_task(
                     ensure_coroutine(e.method)(*params[0], **params[1]),
                     name=e.method.__name__,
                 )
 
             self._received_request[message.seq] = result
 
-        def done(t: asyncio.Task[Any]) -> None:
+        def done(t: "asyncio.Task[Any]") -> None:
             try:
                 self.send_response(message.seq, message.command, t.result())
             except asyncio.CancelledError:
                 self._logger.debug(lambda: f"request message {message!r} canceled")
             except (SystemExit, KeyboardInterrupt):
                 raise
             except DebugAdapterRPCErrorException as ex:
-                self._logger.exception(ex)
                 self.send_error(
                     message=ex.message,
                     request_seq=message.seq,
                     command=ex.command or message.command,
                     success=ex.success or False,
                     error_message=ex.error_message,
                 )
@@ -317,15 +314,15 @@
         self.send_message(request)
 
         return result
 
     @_logger.call
     def send_request_async(
         self, request: Request, return_type: Optional[Type[TResult]] = None
-    ) -> asyncio.Future[TResult]:
+    ) -> "asyncio.Future[TResult]":
         return asyncio.wrap_future(self.send_request(request, return_type))
 
     @_logger.call
     def send_event(self, event: Event) -> None:
         self.send_message(event)
 
     @_logger.call
```

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import asyncio
 import functools
 import os
 import threading
-import warnings
+import time
+from concurrent.futures import CancelledError
 from typing import (
     TYPE_CHECKING,
     Callable,
     List,
     Optional,
     Sequence,
     Union,
     cast,
 )
 
 import click
 
-from robotcode.core.async_tools import (
-    run_coroutine_from_thread_async,
-    run_coroutine_in_thread,
-)
+from robotcode.core.concurrent import run_as_debugpy_hidden_task
 from robotcode.core.types import ServerMode, TcpParams
 from robotcode.core.utils.debugpy import (
     enable_debugpy,
     is_debugpy_installed,
     wait_for_debugpy_connected,
 )
 from robotcode.core.utils.logging import LoggingDescriptor
@@ -49,28 +47,30 @@
 def set_server(value: "DebugAdapterServer") -> None:
     with server_lock:
         global _server
         _server = value
 
 
 @_logger.call
-async def wait_for_server(timeout: float = 5) -> "DebugAdapterServer":
-    async def wait() -> None:
-        while get_server() is None:
-            await asyncio.sleep(0.005)
+def wait_for_server(timeout: float = 10) -> "DebugAdapterServer":
 
-    await asyncio.wait_for(wait(), timeout)
+    start_time = time.monotonic()
+    while get_server() is None and time.monotonic() - start_time < timeout:
+        time.sleep(0.005)
 
     result = get_server()
-    assert result is not None
+
+    if result is None:
+        raise RuntimeError("Timeout to get server instance.")
+
     return result
 
 
 @_logger.call
-async def _debug_adapter_server_(
+async def _debug_adapter_server_async(
     on_config_done_callback: Optional[Callable[["DebugAdapterServer"], None]],
     mode: ServerMode,
     addresses: Union[str, Sequence[str], None],
     port: int,
     pipe_name: Optional[str],
 ) -> None:
     from .server import DebugAdapterServer
@@ -85,22 +85,34 @@
     ) as server:
         if on_config_done_callback is not None:
             server.protocol.received_configuration_done_callback = functools.partial(on_config_done_callback, server)
         set_server(server)
         await server.serve()
 
 
+def _debug_adapter_server_(
+    on_config_done_callback: Optional[Callable[["DebugAdapterServer"], None]],
+    mode: ServerMode,
+    addresses: Union[str, Sequence[str], None],
+    port: int,
+    pipe_name: Optional[str],
+) -> None:
+    asyncio.run(_debug_adapter_server_async(on_config_done_callback, mode, addresses, port, pipe_name))
+
+
 DEFAULT_TIMEOUT = 10.0
 
 
 config_done_callback: Optional[Callable[["DebugAdapterServer"], None]] = None
+debugpy_connected = threading.Event()
 
 
 @_logger.call
-async def start_debugpy_async(
+def start_debugpy(
+    app: Application,
     debugpy_port: Optional[int] = None,
     addresses: Union[Sequence[str], str, None] = None,
     wait_for_debugpy_client: bool = False,
     wait_for_client_timeout: float = DEFAULT_TIMEOUT,
 ) -> None:
     port = find_free_port(debugpy_port)
     if port != debugpy_port:
@@ -118,25 +130,30 @@
                         "addresses": addresses,
                         "processId": os.getpid(),
                     },
                 )
             )
 
             if wait_for_debugpy_client:
-                wait_for_debugpy_connected()
+                app.verbose(f"Wait for debugpy incomming connections listening on {addresses}:{port}")
+                if not wait_for_debugpy_connected(wait_for_client_timeout):
+                    app.warning("No debugpy client connected")
+                else:
+                    app.verbose("Debugpy client connected")
+            debugpy_connected.set()
 
         config_done_callback = connect_debugpy
 
 
 @_logger.call
-async def run_debugger(
+def run_debugger(
     ctx: click.Context,
     app: Application,
     args: List[str],
-    mode: str,
+    mode: ServerMode,
     addresses: Union[str, Sequence[str], None],
     port: int,
     pipe_name: Optional[str] = None,
     debug: bool = False,
     stop_on_entry: bool = False,
     wait_for_client: bool = False,
     wait_for_client_timeout: float = DEFAULT_TIMEOUT,
@@ -146,70 +163,60 @@
     debugpy_port: Optional[int] = None,
     output_messages: bool = False,
     output_log: bool = False,
     output_timestamps: bool = False,
     group_output: bool = False,
 ) -> int:
     if debug and debugpy and not is_debugpy_installed():
-        app.warning("Debugpy not installed.")
+        app.warning("Debugpy not installed")
 
     if debug and debugpy:
-        app.verbose("Try to start debugpy session.")
-        await start_debugpy_async(
+        app.verbose("Try to start debugpy session")
+        start_debugpy(
+            app,
             debugpy_port,
             addresses,
             debugpy_wait_for_client,
             wait_for_client_timeout,
         )
 
-    app.verbose("Start robotcode debugger thread.")
-    server_future = run_coroutine_in_thread(
+    app.verbose("Start robotcode debugger thread")
+
+    run_as_debugpy_hidden_task(
         _debug_adapter_server_,
         config_done_callback,
         mode,
         addresses,
         port,
         pipe_name,
     )
 
-    server = await wait_for_server()
+    server = wait_for_server()
+
     exit_code = 255
 
     try:
         if wait_for_client:
-            app.verbose("Wait for incomming connections.")
+            app.verbose("Wait for incomming connections")
             try:
-                await run_coroutine_from_thread_async(
-                    server.protocol.wait_for_client,
-                    wait_for_client_timeout,
-                    loop=server.loop,
-                )
-            except asyncio.CancelledError:
-                pass
-            except asyncio.TimeoutError as e:
-                raise ConnectionError("No incomming connection from a debugger client.") from e
+                server.protocol.wait_for_client(wait_for_client_timeout)
+            except TimeoutError as e:
+                raise ConnectionError("No incomming connection from a debugger client") from e
 
-            await run_coroutine_from_thread_async(server.protocol.wait_for_initialized, loop=server.loop)
+            server.protocol.wait_for_initialized(wait_for_client_timeout)
 
         if wait_for_client:
             app.verbose("Wait for debug configuration.")
             try:
-                await run_coroutine_from_thread_async(
-                    server.protocol.wait_for_configuration_done,
-                    configuration_done_timeout,
-                    loop=server.loop,
-                )
-            except asyncio.CancelledError:
-                pass
-            except asyncio.TimeoutError as e:
-                raise ConnectionError("Timeout to get configuration from client.") from e
+                server.protocol.wait_for_configuration_done(configuration_done_timeout)
+            except TimeoutError as e:
+                raise ConnectionError("Timeout to get configuration from client") from e
 
         if debugpy and debugpy_wait_for_client:
-            app.verbose("Wait for debugpy incomming connections.")
-            wait_for_debugpy_connected()
+            debugpy_connected.wait(wait_for_client_timeout)
 
         args = [
             "--listener",
             "robotcode.debugger.listeners.ListenerV3",
             "--listener",
             "robotcode.debugger.listeners.ListenerV2",
             *args,
@@ -221,56 +228,47 @@
         Debugger.instance().group_output = group_output
         Debugger.instance().output_timestamps = output_timestamps
         Debugger.instance().colored_output = app.colored
         Debugger.instance().debug = debug
         Debugger.instance().set_main_thread(threading.current_thread())
         Debugger.instance().server_loop = server.loop
 
-        app.verbose("Start the debugger instance.")
+        app.verbose("Start the debugger instance")
         Debugger.instance().start()
 
         exit_code = 0
         try:
             from robotcode.runner.cli.robot import robot
 
-            app.verbose("Start robot.")
+            app.verbose("Start robot")
             try:
                 robot_ctx = robot.make_context("robot", args, parent=ctx)
                 robot.invoke(robot_ctx)
             except SystemExit as e:
                 exit_code = cast(int, e.code)
         finally:
             if server.protocol.connected:
-                await run_coroutine_from_thread_async(
-                    server.protocol.send_event_async,
+                server.protocol.send_event(
                     Event(
                         event="robotExited",
                         body={
                             "reportFile": Debugger.instance().robot_report_file,
                             "logFile": Debugger.instance().robot_log_file,
                             "outputFile": Debugger.instance().robot_output_file,
                             "exitCode": exit_code,
                         },
-                    ),
-                    loop=server.loop,
+                    )
                 )
 
-                await run_coroutine_from_thread_async(server.protocol.exit, exit_code, loop=server.loop)
-    except asyncio.CancelledError:
+                server.protocol.exit(exit_code)
+    except CancelledError:
         pass
     finally:
         if server.protocol.connected:
-            await run_coroutine_from_thread_async(server.protocol.terminate, loop=server.loop)
+            server.protocol.terminate()
 
-            try:
-                await run_coroutine_from_thread_async(server.protocol.wait_for_disconnected, loop=server.loop)
-            except asyncio.TimeoutError:
-                warnings.warn("Timeout at disconnect client occurred.")
+            if not server.protocol.wait_for_disconnected():
+                app.warning("Timeout to get disconnected from client")
 
-        server_future.cancel()
-
-        try:
-            await server_future
-        except asyncio.CancelledError:
-            pass
+        server.loop.stop()
 
     return exit_code
```

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import os
+import threading
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
-from robotcode.core import async_tools
+from robotcode.core import concurrent
 from robotcode.core.types import ServerMode, TcpParams
 from robotcode.core.utils.logging import LoggingDescriptor
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.jsonrpc2.server import JsonRPCServer
 
 from .dap_types import (
     AttachRequestArguments,
@@ -55,50 +56,50 @@
 
 class DebugAdapterServerProtocol(DebugAdapterProtocol):
     _logger = LoggingDescriptor()
 
     def __init__(self) -> None:
         super().__init__()
 
-        self._connected_event = async_tools.Event()
-        self._disconnected_event = async_tools.Event()
+        self._connected_event = threading.Event()
+        self._disconnected_event = threading.Event()
         self._connected = False
         self._sigint_signaled = False
 
         self._initialized = False
-        self._initialized_event = async_tools.Event()
+        self._initialized_event = threading.Event()
 
-        self._exited_lock = async_tools.Lock()
+        self._exited_lock = concurrent.RLock()
         self._exited = False
 
-        self._terminated_lock = async_tools.Lock()
+        self._terminated_lock = concurrent.RLock()
         self._terminated = False
 
-        self._received_configuration_done_event = async_tools.Event()
+        self._received_configuration_done_event = threading.Event()
         self._received_configuration_done = False
         self.received_configuration_done_callback: Optional[Callable[[], None]] = None
 
         Debugger.instance().send_event.add(self.on_debugger_send_event)
 
     def on_debugger_send_event(self, sender: Any, event: Event) -> None:
         if self._loop is not None:
             asyncio.run_coroutine_threadsafe(self.send_event_async(event), loop=self._loop)
 
     @property
     def connected(self) -> bool:
         return self._connected
 
     @property
-    async def exited(self) -> bool:
-        async with self._exited_lock:
+    def exited(self) -> bool:
+        with self._exited_lock:
             return self._exited
 
     @property
-    async def terminated(self) -> bool:
-        async with self._terminated_lock:
+    def terminated(self) -> bool:
+        with self._terminated_lock:
             return self._terminated
 
     @_logger.call
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         if self.connected:
             raise ConnectionError("Protocol already connected, only one conntection allowed.")
 
@@ -112,30 +113,32 @@
     def connection_lost(self, exc: Optional[BaseException]) -> None:
         super().connection_lost(exc)
 
         self._connected = False
         self._disconnected_event.set()
 
     @_logger.call
-    async def wait_for_client(self, timeout: float = 5) -> bool:
-        await asyncio.wait_for(self._connected_event.wait(), timeout)
+    def wait_for_client(self, timeout: float = 5) -> bool:
+        if not self._connected_event.wait(timeout):
+            raise TimeoutError("Timeout waiting for client")
 
         return self._connected
 
     @_logger.call
-    async def wait_for_initialized(self, timeout: float = 30) -> bool:
-        await asyncio.wait_for(self._initialized_event.wait(), timeout)
+    def wait_for_initialized(self, timeout: float = 30) -> bool:
+        if not self._initialized_event.wait(timeout):
+            raise TimeoutError("Timeout waiting for client initialization")
 
         return self._initialized
 
     @_logger.call
-    async def wait_for_disconnected(self, timeout: float = 30) -> bool:
-        await asyncio.wait_for(self._disconnected_event.wait(), timeout)
+    def wait_for_disconnected(self, timeout: float = 5) -> bool:
+        self._disconnected_event.wait(timeout)
 
-        return self._connected
+        return not self._connected
 
     @rpc_method(name="initialize", param_type=InitializeRequestArguments)
     async def _initialize(self, arguments: InitializeRequestArguments, *args: Any, **kwargs: Any) -> Capabilities:
         self._initialized = True
 
         if self.loop is not None:
             self.loop.call_soon(self.initialized)
@@ -207,23 +210,23 @@
 
     @_logger.call
     def initialized(self) -> None:
         self.send_event(InitializedEvent())
         self._initialized_event.set()
 
     @_logger.call
-    async def exit(self, exit_code: int) -> None:
-        async with self._exited_lock:
-            await self.send_event_async(ExitedEvent(body=ExitedEventBody(exit_code=exit_code)))
+    def exit(self, exit_code: int) -> None:
+        with self._exited_lock:
+            self.send_event(ExitedEvent(body=ExitedEventBody(exit_code=exit_code)))
             self._exited = True
 
     @_logger.call
-    async def terminate(self) -> None:
-        async with self._terminated_lock:
-            await self.send_event_async(TerminatedEvent())
+    def terminate(self) -> None:
+        with self._terminated_lock:
+            self.send_event(TerminatedEvent())
             self._terminated = True
 
     @rpc_method(name="terminate", param_type=TerminateArguments)
     async def _terminate(
         self,
         arguments: Optional[TerminateArguments] = None,
         *args: Any,
@@ -247,19 +250,15 @@
     @rpc_method(name="disconnect", param_type=DisconnectArguments)
     async def _disconnect(
         self,
         arguments: Optional[DisconnectArguments] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        if (
-            (not (await self.exited) or not (await self.terminated))
-            and arguments is not None
-            and arguments.terminate_debuggee
-        ):
+        if (not (self.exited) or not (self.terminated)) and arguments is not None and arguments.terminate_debuggee:
             os._exit(-1)
         else:
             await self.send_event_async(Event("disconnectRequested"))
             Debugger.instance().attached = False
             Debugger.instance().continue_all()
 
     @rpc_method(name="setBreakpoints", param_type=SetBreakpointsArguments)
@@ -286,16 +285,17 @@
         self._received_configuration_done = True
         self._received_configuration_done_event.set()
 
         if self.received_configuration_done_callback is not None:
             self.received_configuration_done_callback()
 
     @_logger.call
-    async def wait_for_configuration_done(self, timeout: float = 5) -> bool:
-        await asyncio.wait_for(self._received_configuration_done_event.wait(), timeout)
+    def wait_for_configuration_done(self, timeout: float = 5) -> bool:
+        if not self._received_configuration_done_event.wait(timeout):
+            raise TimeoutError("Timeout waiting for configuration done event")
 
         return self._received_configuration_done
 
     @rpc_method(name="continue", param_type=ContinueArguments)
     async def _continue(self, arguments: ContinueArguments, *args: Any, **kwargs: Any) -> ContinueResponseBody:
         Debugger.instance().continue_thread(arguments.thread_id)
         return ContinueResponseBody(all_threads_continued=True)
```

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.81.0/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/.gitignore` & `robotcode_debugger-0.81.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/LICENSE.txt` & `robotcode_debugger-0.81.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/README.md` & `robotcode_debugger-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.80.0/pyproject.toml` & `robotcode_debugger-0.81.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,27 +24,27 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.80.0",
-  "robotcode-runner==0.80.0",
+  "robotcode-jsonrpc2==0.81.0",
+  "robotcode-runner==0.81.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
-Donate = "https://github.com/sponsors/d-biehl"
+Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
 Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
 Issues = "https://github.com/robotcodedev/robotcode/issues"
 Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/debugger/__version__.py"
```

### Comparing `robotcode_debugger-0.80.0/PKG-INFO` & `robotcode_debugger-0.81.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: robotcode-debugger
-Version: 0.80.0
+Version: 0.81.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
-Project-URL: Donate, https://github.com/sponsors/d-biehl
+Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
 License: Apache-2.0
 License-File: LICENSE.txt
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.80.0
-Requires-Dist: robotcode-runner==0.80.0
+Requires-Dist: robotcode-jsonrpc2==0.81.0
+Requires-Dist: robotcode-runner==0.81.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

