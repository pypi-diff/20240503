# Comparing `tmp/kilter.service-0.2.0.tar.gz` & `tmp/kilter_service-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilter.service-0.2.0.tar", last modified: Mon Jan 30 03:33:06 2023, max compression
+gzip compressed data, was "kilter_service-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kilter.service-0.2.0.tar` & `kilter_service-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    16726 2022-09-20 23:20:59.983151 kilter.service-0.2.0/LICENCE.txt
--rw-r--r--   0        0        0     5310 2022-09-20 23:20:59.985151 kilter.service-0.2.0/README.md
--rw-r--r--   0        0        0      807 2023-01-30 02:33:42.803900 kilter.service-0.2.0/kilter/service/__init__.py
--rw-r--r--   0        0        0        0 2023-01-25 09:49:17.519681 kilter.service-0.2.0/kilter/service/py.typed
--rw-r--r--   0        0        0    11019 2023-01-30 02:33:42.804900 kilter.service-0.2.0/kilter/service/runner.py
--rw-r--r--   0        0        0    16972 2023-01-30 02:33:42.805900 kilter.service-0.2.0/kilter/service/session.py
--rw-r--r--   0        0        0     3378 2023-01-25 09:49:17.519681 kilter.service-0.2.0/kilter/service/util.py
--rw-r--r--   0        0        0     2437 2023-01-30 02:33:42.806900 kilter.service-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6267 1970-01-01 00:00:00.000000 kilter.service-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16726 2024-05-02 00:17:40.054463 kilter_service-0.3.0/LICENCE.txt
+-rw-r--r--   0        0        0     5839 2024-05-02 00:17:40.054463 kilter_service-0.3.0/README.md
+-rw-r--r--   0        0        0      807 2024-05-02 00:55:00.601200 kilter_service-0.3.0/kilter/service/__init__.py
+-rw-r--r--   0        0        0     9599 2024-05-02 00:17:40.058463 kilter_service-0.3.0/kilter/service/options.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:17:40.058463 kilter_service-0.3.0/kilter/service/py.typed
+-rw-r--r--   0        0        0    12841 2024-05-02 00:17:40.058463 kilter_service-0.3.0/kilter/service/runner.py
+-rw-r--r--   0        0        0    17837 2024-05-02 21:35:18.286876 kilter_service-0.3.0/kilter/service/session.py
+-rw-r--r--   0        0        0     3378 2024-05-02 00:17:40.058463 kilter_service-0.3.0/kilter/service/util.py
+-rw-r--r--   0        0        0     2203 2024-05-02 16:44:14.840800 kilter_service-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 kilter_service-0.3.0/PKG-INFO
```

### Comparing `kilter.service-0.2.0/LICENCE.txt` & `kilter_service-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `kilter.service-0.2.0/README.md` & `kilter_service-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,26 @@
 wishes to make use of async/await features.
 
 Use of `libmilter` to implement filters is almost universal as it is a black-box; the 
 on-the-wire protocol used is undocumented and subject to change between versions, which 
 makes writing a third-party parser difficult.
 
 
+Alternatives in the Python Space
+--------------------------------
+
+- [purepythonmilter](https://github.com/gertvdijk/purepythonmilter):
+  A modern and robust implementation for `asyncio`, written purely in statically typed 
+  Python without the need for `libmilter`.
+
+- [python-libmilter](https://github.com/crustymonkey/python-libmilter):
+	Another pure-Python module using threading. Lacks static type annotations and is no longer 
+	actively developed, although still minimally maintained.
+
+
 Usage
 =====
 
 To write filters, create a coroutine function that conforms to `Filter`.  This function 
 takes a `Session` object as its only argument.
 
 `Session` instances have several awaitable methods corresponding to SMTP commands 
@@ -98,30 +110,34 @@
 	async with session.headers as headers:
 		async for header in headers:
 			if header.name.startswith("X-"):
 				remove.append(header)
 
 	# remove the selected headers during the post phase
 	for header in remove:
-		await session.headers.remove(header)
+		await session.headers.delete(header)
+
+	return Accept()
 ```
 
 ```python
 from kilter.service import Session
 from kilter.protocol import Accept
 
 async def strip_x_headers(session: Session) -> Accept:
 	# collect the headers first
 	await session.headers.collect()
 
 	# iterate over collected headers during the post phase, removing the unwanted ones
 	async with session.headers as headers:
 		async for header in headers:
 			if header.name.startswith("X-"):
-				await session.headers.remove(header)
+				await session.headers.delete(header)
+
+	return Accept()
 ```
 
 
 ---
 
 [gitlab-ico]:
   https://img.shields.io/badge/GitLab-code.kodo.org.uk-blue.svg?logo=gitlab
```

### Comparing `kilter.service-0.2.0/kilter/service/__init__.py` & `kilter_service-0.3.0/kilter/service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .runner import Runner
 from .session import END
 from .session import START
 from .session import After
 from .session import Before
 from .session import Session
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 __all__ = [
 	"After",
 	"Before",
 	"END",
 	"ResponseMessage",
 	"Runner",
```

### Comparing `kilter.service-0.2.0/kilter/service/runner.py` & `kilter_service-0.3.0/kilter/service/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,68 +11,69 @@
 `anyio.abc.Listener`, which can be obtained, for instance, from
 `anyio.create_tcp_listener()`.
 """
 
 from __future__ import annotations
 
 import logging
+from collections import defaultdict
 from collections.abc import AsyncGenerator
-from typing import TYPE_CHECKING
 from typing import Final
 from typing import TypeAlias
-from typing import TypeVar
 from warnings import warn
 
 import anyio.abc
 from anyio.streams.stapled import StapledObjectStream
 from async_generator import aclosing
+from typing_extensions import Self
 
 from kilter.protocol.buffer import SimpleBuffer
 from kilter.protocol.core import EditMessage
 from kilter.protocol.core import EventMessage
 from kilter.protocol.core import FilterProtocol
 from kilter.protocol.core import ResponseMessage
 from kilter.protocol.messages import ProtocolFlags
 
+from .options import get_flags
+from .options import get_macros
 from .session import *
 from .util import Broadcast
 from .util import qualname
 
 MessageChannel: TypeAlias = anyio.abc.ObjectStream[Message]
 Sender: TypeAlias = AsyncGenerator[None, ResponseMessage|EditMessage|Negotiate|Skip]
 
 kiB: Final = 2**10
 MiB: Final = 2**20
 
 # TODO: Convert to Union type alias once python/mypy#14242 is fixed
 _VALID_FINAL_RESPONSES: Final = Reject, Discard, Accept, TemporaryFailure, ReplyCode
 _VALID_EVENT_MESSAGE: TypeAlias = Helo | EnvelopeFrom | EnvelopeRecipient | Data | \
 	Unknown | Header | EndOfHeaders | Body | EndOfMessage | Abort
-_DISABLE_PROTOCOL_FLAGS: Final = ProtocolFlags.NO_CONNECT | ProtocolFlags.NO_HELO | \
-	ProtocolFlags.NO_SENDER | ProtocolFlags.NO_RECIPIENT | ProtocolFlags.NO_BODY | \
-	ProtocolFlags.NO_HEADERS | ProtocolFlags.NO_EOH | ProtocolFlags.NO_UNKNOWN | \
-	ProtocolFlags.NO_DATA | ProtocolFlags.NR_CONNECT | ProtocolFlags.NR_HELO | \
-	ProtocolFlags.NR_SENDER | ProtocolFlags.NR_RECIPIENT | ProtocolFlags.NR_DATA | \
-	ProtocolFlags.NR_UNKNOWN | ProtocolFlags.NR_EOH | ProtocolFlags.NR_BODY | \
-	ProtocolFlags.NR_HEADER
 
 _logger = logging.getLogger(__package__)
 
 
 class NegotiationError(Exception):
 	"""
 	An error raised when MTAs are not compatible with the filter
 	"""
 
 
+class _CloseFilter:
+
+	def __init__(self, filtr: Filter):
+		self.filter = filtr
+
+
 class _Broadcast(Broadcast[EventMessage]):
 
 	def __init__(self) -> None:
 		super().__init__()
-		self.task_status: anyio.abc.TaskStatus|None = None
+		self.task_status: anyio.abc.TaskStatus[None]|None = None
 
 	async def shutdown_hook(self) -> None:
 		await self.pre_receive_hook()
 
 	async def pre_receive_hook(self) -> None:
 		if self.task_status is not None:
 			self.task_status.started()
@@ -86,23 +87,23 @@
 	Instances can be used as handlers that can be passed to `anyio.abc.Listener.serve()` or
 	used with any `anyio.abc.ByteStream`.
 	"""
 
 	def __init__(self, *filters: Filter):
 		if len(filters) == 0:  # pragma: no-cover
 			raise TypeError("Runner requires at least one filter to run")
-		self.filters = filters
+		self.filters = list(filters)
 		self.use_skip = True
 
 	async def __call__(self, client: anyio.abc.ByteStream) -> None:
 		"""
 		Return an awaitable that starts and coordinates filters
 		"""
 		buff = SimpleBuffer(1*MiB)
-		proto = FilterProtocol()
+		proto = FilterProtocol(abort_on_unknown=True)
 		sender = _sender(client, proto)
 		macro: Macro|None = None
 		aborted = False
 
 		await sender.asend(None)  # type: ignore # initialise
 
 		async with (
@@ -121,56 +122,95 @@
 					await runner.aclose()
 					return
 				for message in proto.read_from(buff):
 					if __debug__:
 						_logger.debug(f"received: {message}")
 					match message:
 						case Negotiate():
-							await sender.asend(await self._negotiate(message, sender))
+							await sender.asend(await self._negotiate(message))
 						case Macro() as macro:
 							# Note that this Macro will hang around as "macro"; this is for
 							# Connect messages.
 							await runner.set_macros(macro)
 						case Connect():
 							await self._prepare_filters(message, sender, runner)
 							if macro:
 								await runner.set_macros(macro)
-							await sender.asend(await runner.start(True, self.use_skip))
+							needs_response = proto.needs_response(message)
+							match await runner.start(needs_response, True, self.use_skip):
+								case None:
+									assert not needs_response
+								case _CloseFilter() as notif:
+									self.filters.remove(notif.filter)
+								case c_resp if needs_response:
+									assert c_resp is not None and not isinstance(c_resp, _CloseFilter)
+									await sender.asend(c_resp)
+								case c_resp:
+									raise RuntimeError(f"unexpected response: {c_resp}")
 						case Abort():
 							aborted = True
 							await runner.abort(message)
 						case Close():
 							await runner.aclose()
 							return
 						case _:
 							if aborted:
 								aborted = False
-								await runner.start(False, self.use_skip)
-							# TODO: Upgrade and remove ignores once python/mypy#14242 is in
-							# TODO: Should remove assert once kilter.protocol#5 is resolved
-							# Type narrowing should do the job adequately
-							# https://code.kodo.org.uk/kilter/kilter.protocol/-/issues/5
-							assert isinstance(message, _VALID_EVENT_MESSAGE)  # type: ignore[misc,arg-type]
-							await sender.asend(await runner.message_events(message))  # type: ignore[arg-type]
+								await runner.start(True, False, self.use_skip)
+							needs_response = proto.needs_response(message)
+							match await runner.message_events(message, needs_response):
+								case None:
+									assert not needs_response
+								case _CloseFilter() as notif:
+									self.filters.remove(notif.filter)
+								case resp if needs_response:
+									assert resp is not None and not isinstance(resp, _CloseFilter)
+									await sender.asend(resp)
+								case resp:
+									raise RuntimeError(f"unexpected response: {resp}")
 
-	async def _negotiate(self, message: Negotiate, sender: Sender) -> Negotiate:
+	async def _negotiate(self, message: Negotiate) -> Negotiate:
 		_logger.info("Negotiating with MTA")
 
-		# TODO: actually negotiate what the filter wants, not just "everything"
-		actions = set(ActionFlags)  # All actions!
-		if actions != ActionFlags.unpack(message.action_flags):
-			raise NegotiationError("MTA does not accept all actions required by the filter")
-
-		resp = Negotiate(6, 0, 0)
-		resp.protocol_flags = message.protocol_flags & ~_DISABLE_PROTOCOL_FLAGS
-		resp.action_flags = ActionFlags.pack(actions)
+		optmask = ProtocolFlags.NONE
+		options = \
+			ProtocolFlags.SKIP | \
+			ProtocolFlags.NO_HELO | \
+			ProtocolFlags.NO_SENDER | ProtocolFlags.NO_RECIPIENT | \
+			ProtocolFlags.NO_DATA | ProtocolFlags.NO_BODY | \
+			ProtocolFlags.NO_HEADERS | ProtocolFlags.NO_END_OF_HEADERS | \
+			ProtocolFlags.NR_CONNECT | ProtocolFlags.NR_HELO | \
+			ProtocolFlags.NR_SENDER | ProtocolFlags.NR_RECIPIENT | \
+			ProtocolFlags.NR_DATA | ProtocolFlags.NR_BODY | \
+			ProtocolFlags.NR_HEADER | ProtocolFlags.NR_END_OF_HEADERS
+		actions = ActionFlags.NONE
+		macros = defaultdict(set)
+
+		options &= message.protocol_flags  # Remove unoffered initial flags, they are not required
+
+		for filtr in self.filters:
+			flags = get_flags(filtr)
+			optmask |= flags.unset_options
+			options |= flags.set_options
+			actions |= flags.set_actions
+
+			for stage, names in get_macros(filtr).items():
+				macros[stage].update(names)
+
+		options &= ~optmask
+
+		if (missing_actions := actions & ~message.action_flags):
+			raise NegotiationError(f"MTA does not accept {missing_actions}")
 
-		self.use_skip = bool(resp.protocol_flags & ProtocolFlags.SKIP)
+		if (missing_options := options & ~message.protocol_flags):
+			raise NegotiationError(f"MTA does not offer {missing_options}")
 
-		return resp
+		self.use_skip = ProtocolFlags.SKIP in options
+
+		return Negotiate(6, actions, options, dict(macros))
 
 	async def _prepare_filters(
 		self,
 		message: Connect,
 		sender: Sender,
 		runner: _TaskRunner,
 	) -> None:
@@ -178,112 +218,137 @@
 		for fltr in self.filters:
 			session = Session(message, sender, _Broadcast())
 			runner.add_filter(fltr, session)
 
 
 class _TaskRunner:
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="_TaskRunner")
-
 	def __init__(self, tasks: anyio.abc.TaskGroup):
 		self.tasks = tasks
 		self.filters = list[tuple[Filter, Session]]()
-		self.channels = list[MessageChannel]()
+		self.channels = dict[MessageChannel, Filter]()
 
-	async def __aenter__(self: Self) -> Self:
+	async def __aenter__(self) -> Self:
 		return self
 
 	async def __aexit__(self, *_: object) -> None:
 		await self.aclose()
 
 	def add_filter(self, flter: Filter, session: Session, /) -> None:
 		self.filters.append((flter, session))
 
-	async def start(self, first_connect: bool, use_skip: bool) -> ResponseMessage:
+	async def start(
+		self,
+		needs_response: bool,
+		first_connect: bool,
+		use_skip: bool,
+	) -> ResponseMessage|_CloseFilter|None:
 		if self.channels:
 			raise RuntimeError(f"{self} is already running tasks")
 		final: ResponseMessage = Accept()
 		for flter, session in self.filters:
 			lchannel, rchannel = _make_message_channel()
-			self.channels.append(lchannel)
-			match await self.tasks.start(self._runner, flter, session, rchannel, first_connect, use_skip):
+			self.channels[lchannel] = flter
+			match await self.tasks.start(self._runner, flter, session, rchannel, use_skip):
 				case Accept():
-					self.channels.remove(lchannel)
+					del self.channels[lchannel]
 				case Continue():
 					continue
 				case TemporaryFailure() as final:  # replaces final
 					pass
 				case Reject()|Discard()|ReplyCode() as resp:
 					if not first_connect:
 						_logger.warning(
 							f"Ignoring unexpected response from filter after restart: "
 							f"{qualname(flter)} -> {resp}",
 						)
 						continue
+					if not needs_response:
+						_logger.warning(
+							f"Unexpected response from filter {qualname(flter)}",
+						)
+						return _CloseFilter(flter)
 					return resp
 				case _ as arg:  # pragma: no-cover
 					raise TypeError(f"task_status.started called with bad type: {arg!r}")
+		if not needs_response:
+			return None
 		return final if len(self.channels) == 0 else Continue()
 
 	async def set_macros(self, message: Macro) -> None:
 		if self.channels:
 			for channel in self.channels:
 				await channel.send(message)
 		else:
 			for _, session in self.filters:
 				await session.deliver(message)
 
-	async def message_events(self, message: _VALID_EVENT_MESSAGE) -> ResponseMessage|Skip:
+	async def message_events(
+		self,
+		message: _VALID_EVENT_MESSAGE,
+		needs_response: bool,
+	) -> ResponseMessage|Skip|_CloseFilter|None:
 		skip = isinstance(message, Body)
-		for channel in self.channels:
+		for channel in list(self.channels):
 			await channel.send(message)
 			match (await channel.receive()):
 				case Skip():
 					continue
 				case Continue():
 					skip = False
-				case Accept():
-					await channel.aclose()
-					self.channels.remove(channel)
+				case Accept() as resp:
+					flter = await self.close_channel(channel)
+					if len(self.channels) == 0:
+						_logger.info(f"Returning response Accept from {qualname(flter)}")
+						return resp
+					_logger.info(f"Holding response Accept from {qualname(flter)}")
 				case (Reject() | Discard() | TemporaryFailure() | ReplyCode()) as resp:
+					flter = await self.close_channel(channel)
+					if not needs_response:
+						_logger.warning(f"Unexpected response from filter {qualname(flter)}")
+						return _CloseFilter(flter)
+					_logger.info(f"Returning response {type(resp).__name__} from {qualname(flter)}")
 					return resp
-		return (
-			Accept() if len(self.channels) == 0 else
-			Skip() if skip else
-			Continue()
-		)
+		assert len(self.channels) > 0, "Running filters reached zero without a response?!"
+		if not needs_response:
+			return None
+		return Skip() if skip else Continue()
+
+	async def close_channel(self, channel: MessageChannel) -> Filter:
+		await channel.aclose()
+		return self.channels.pop(channel)
 
 	async def abort(self, abort: Abort) -> None:
-		if self.channels:
-			_logger.info("Aborting filters")
+		if not self.channels:
+			return
+		_logger.info("Aborting filters")
 		for channel in self.channels:
 			await channel.send(abort)
 			await channel.receive()
 			await channel.aclose()
-		del self.channels[:]
+		self.channels.clear()
 
 	async def aclose(self) -> None:
-		_logger.info("Closing runners")
+		if self.channels:
+			_logger.info("Closing filters")
 		self.tasks.cancel_scope.cancel()
-		del self.channels[:]
+		self.channels.clear()
 
 	@staticmethod
 	async def _runner(
 		fltr: Filter,
 		session: Session,
 		channel: MessageChannel,
-		first_connect: bool,
 		use_skip: bool, *,
-		task_status: anyio.abc.TaskStatus,
+		task_status: anyio.abc.TaskStatus[ResponseMessage],
 	) -> None:
 		final_resp: ResponseMessage|None = None
 
 		async def _filter_wrap(
-			task_status: anyio.abc.TaskStatus,
+			task_status: anyio.abc.TaskStatus[None],
 		) -> None:
 			nonlocal final_resp
 			async with session:
 				assert isinstance(session.broadcast, _Broadcast)
 				session.broadcast.task_status = task_status
 				try:
 					final_resp = await fltr(session)
@@ -308,20 +373,20 @@
 					return
 				if isinstance(message, Macro):
 					await session.deliver(message)
 					continue
 				# TODO: Upgrade and remove ignores once python/mypy#14242 is in
 				assert isinstance(message, _VALID_EVENT_MESSAGE)  # type: ignore[misc,arg-type]
 				resp = await session.deliver(message)  # type: ignore[arg-type]
-				if final_resp is not None:
-					break  # type: ignore[unreachable]
 				if isinstance(message, Abort):
 					await channel.send(Continue())
 					await channel.aclose()
 					return
+				if final_resp is not None:
+					break  # type: ignore[unreachable]
 				await channel.send(Skip() if use_skip and resp == Skip else Continue())
 			await channel.send(final_resp)
 
 
 def _make_message_channel() -> tuple[MessageChannel, MessageChannel]:
 	lsend, rrecv = anyio.create_memory_object_stream(1, Message)  # type: ignore
 	rsend, lrecv = anyio.create_memory_object_stream(1, Message)  # type: ignore
```

### Comparing `kilter.service-0.2.0/kilter/service/session.py` & `kilter_service-0.3.0/kilter/service/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# Copyright 2022-2023 Dominik Sekotill <dom.sekotill@kodo.org.uk>
+# Copyright 2022-2024 Dominik Sekotill <dom.sekotill@kodo.org.uk>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 Sessions are the kernel of a filter, providing it with an async API to access messages
 """
 
 from __future__ import annotations
 
 from collections.abc import AsyncGenerator
 from collections.abc import AsyncIterator
+from collections.abc import Sequence
 from dataclasses import dataclass
 from enum import Enum
 from ipaddress import IPv4Address
 from ipaddress import IPv6Address
 from pathlib import Path
 from types import TracebackType
-from typing import TYPE_CHECKING
 from typing import AsyncContextManager
 from typing import Literal
 from typing import Protocol
-from typing import TypeVar
 from warnings import warn
 
+from typing_extensions import Self
+
 from ..protocol.core import EditMessage
 from ..protocol.core import EventMessage
 from ..protocol.core import ResponseMessage
 from ..protocol.messages import *
 from . import util
 
 
@@ -39,15 +40,15 @@
 
 
 class Filter(Protocol):
 	"""
 	Filters are callables that accept a `Session` and return a response
 	"""
 
-	async def __call__(self, session: Session) -> ResponseMessage: ...  # noqa: D102
+	async def __call__(self, session: Session, /) -> ResponseMessage: ...  # noqa: D102
 
 
 class Phase(int, Enum):
 	"""
 	Session phases indicate what messages to expect and are impacted by received messages
 
 	Users should not generally need to use these values, however an understanding of the
@@ -143,17 +144,14 @@
 
 
 class Session:
 	"""
 	The kernel of a filter, providing an API for filters to access messages from an MTA
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="Session")
-
 	host: str
 	"""
 	A hostname from a reverse address lookup performed when a client connects
 
 	If no name is found this value defaults to the standard presentation format for
 	`Session.address` surrounded by "[" and "]", e.g. "[192.0.2.100]"
 	"""
@@ -207,15 +205,15 @@
 		self.headers = HeadersAccessor(self, sender)
 		self.body = BodyAccessor(self, sender)
 
 		# Phase checking is a bit fuzzy as a filter may not request every message,
 		# so some phases will be skipped; checks should not try to exactly match a phase.
 		self.phase = Phase.CONNECT
 
-	async def __aenter__(self: Self) -> Self:
+	async def __aenter__(self) -> Self:
 		await self.broadcast.__aenter__()
 		return self
 
 	async def __aexit__(self, *_: object) -> None:
 		await self.broadcast.__aexit__(None, None, None)
 		# on session close, wake up any remaining deliver() awaitables
 		await self.broadcast.shutdown_hook()
@@ -308,14 +306,15 @@
 			)
 		bname = name.encode("utf-8")
 		while self.phase <= Phase.ENVELOPE:
 			message = await self.broadcast.receive()
 			match message:
 				case Unknown():
 					if message.content[:len(bname)] == bname:
+						assert isinstance(message.content, memoryview)
 						return message.content
 				# fake buffers for MAIL and RCPT commands
 				case EnvelopeFrom() if name == "MAIL":
 					vals = [b"MAIL FROM", message.sender, *message.arguments]
 					return memoryview(b" ".join(vals))
 				case EnvelopeRecipient() if name == "RCPT":
 					vals = [b"RCPT TO", message.recipient, *message.arguments]
@@ -369,60 +368,71 @@
 		await self._aiter.aclose()
 
 	async def __aiter(self) -> AsyncGenerator[Header, None]:
 		# yield from cached headers first; allows multiple tasks to access the headers
 		# in an uncoordinated manner; note the broadcaster is locked at this point
 		for header in self._table:
 			yield header
+		seen = set(id(header) for header in self._table)
 		while self.session.phase <= Phase.HEADERS:
 			match (await self.session.broadcast.receive()):
 				case Header() as header:
+					header.freeze()
 					self._table.append(header)
+					seen.add(id(header))
 					try:
 						yield header
 					except GeneratorExit:
 						await self.collect()
 						raise
 				case EndOfHeaders():
 					return
+		# It's possible for collect() to have been called while yielded, in which case the
+		# loop will end. Yield any headers that were stored by collect() but not yet
+		# yielded.
+		for header in self._table:
+			if id(header) not in seen:
+				yield header
 
 	async def collect(self) -> None:
 		"""
 		Collect all headers without producing an iterator
 
 		Calling this method before the `Phase.BODY` phase allows later processing of headers
 		(after the HEADER phase) without the need for an empty loop.
 		"""
 		# note the similarities between this and __aiter; the difference is no mutex or
 		# yields
 		while self.session.phase <= Phase.HEADERS:
 			match (await self.session.broadcast.receive()):
 				case Header() as header:
+					header.freeze()
 					self._table.append(header)
 				case EndOfHeaders():
 					return
 
 	async def delete(self, header: Header) -> None:
 		"""
 		Move onto the `Phase.POST` phase and Instruct the MTA to delete the given header
 		"""
 		await self.collect()
 		await _until_editable(self.session)
-		index = self._table.index(header)
+		index = _index_by_name(self._table, header)
 		await self._editor.asend(ChangeHeader(index, header.name, b""))
-		del self._table[index]
+		self._table.remove(header)
 
 	async def update(self, header: Header, value: bytes) -> None:
 		"""
 		Move onto the `Phase.POST` phase and Instruct the MTA to modify the value of a header
 		"""
 		await self.collect()
 		await _until_editable(self.session)
-		index = self._table.index(header)
+		index = _index_by_name(self._table, header)
 		await self._editor.asend(ChangeHeader(index, header.name, value))
+		index = self._table.index(header)
 		self._table[index].value = value
 
 	async def insert(self, header: Header, position: Position) -> None:
 		"""
 		Move onto the `Phase.POST` phase and instruct the MTA to insert a new header
 
 		The header is inserted at `START`, `END`, or a relative position with `Before` and
@@ -435,34 +445,33 @@
 				index = 0
 			case Position(subject="end"):
 				index = len(self._table)
 			case Before():
 				index = self._table.index(position.subject)
 			case After():  # pragma: no-branch
 				index = self._table.index(position.subject) + 1
+			case _:
+				raise TypeError("Expect a Position")
 		if index >= len(self._table):
 			await self._editor.asend(AddHeader(header.name, header.value))
 			self._table.append(header)
 		else:
-			await self._editor.asend(InsertHeader(index, header.name, header.value))
+			await self._editor.asend(InsertHeader(index + 1, header.name, header.value))
 			self._table.insert(index, header)
 
 
 class HeaderIterator(AsyncGenerator[Header, None]):
 	"""
 	Iterator for headers obtained by using a `HeadersAccessor` as a context manager
 	"""
 
-	if TYPE_CHECKING:
-		Self = TypeVar("Self", bound="HeaderIterator")
-
 	def __init__(self, aiter: AsyncGenerator[Header, None]):
 		self._aiter = aiter
 
-	def __aiter__(self: Self) -> Self:
+	def __aiter__(self) -> Self:
 		return self
 
 	async def __anext__(self) -> Header:  # noqa: D102
 		return await self._aiter.__anext__()
 
 	async def asend(self, value: None = None) -> Header:  # noqa: D102
 		return await self._aiter.__anext__()
@@ -516,20 +525,22 @@
 		self._aiter = None
 
 	async def __aiter(self) -> AsyncGenerator[memoryview, None]:
 		while self.session.phase <= Phase.BODY:
 			match (await self.session.broadcast.receive()):
 				case Body() as body:
 					try:
+						assert isinstance(body.content, memoryview)
 						yield body.content
 					except GeneratorExit:
 						self.skip = True
 						raise
 				case EndOfMessage() as eom:
 					if not self.skip:
+						assert isinstance(eom.content, memoryview)
 						yield eom.content
 
 	async def write(self, chunk: bytes) -> None:
 		"""
 		Request that chunks of a new message body are sent to the MTA
 
 		This method should not be called from within the scope created by using it's
@@ -547,8 +558,22 @@
 
 
 async def _until_editable(session: Session) -> None:
 	if session.phase == Phase.POST:
 		return
 	session.body.skip = True
 	while session.phase < Phase.POST:
-		await session.broadcast.receive()
+		if session.phase == Phase.HEADERS:
+			await session.headers.collect()
+		else:
+			await session.broadcast.receive()
+
+
+def _index_by_name(table: Sequence[Header], needle: Header) -> int:
+	index = 0
+	name = needle.name.lower()
+	for header in table:
+		if header == needle:
+			return index + 1
+		if header.name.lower() == name:
+			index += 1
+	raise ValueError(f"header not found: {needle}")
```

### Comparing `kilter.service-0.2.0/kilter/service/util.py` & `kilter_service-0.3.0/kilter/service/util.py`

 * *Files identical despite different names*

### Comparing `kilter.service-0.2.0/pyproject.toml` & `kilter_service-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,65 @@
 [build-system]
-requires = ["flit_core ~=3.2"]
+requires = ["flit_core ~=3.8"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "kilter.service"
 authors = [
 	{name = "Dom Sekotill", email = "dom.sekotill@kodo.org.uk"},
 ]
 license = {file = "LICENCE.txt"}
 readme = "README.md"
 dynamic = ["version", "description"]
 
-# https://github.com/pypa/flit/issues/476
-requires-python = ">=3.10,<4"
-
+requires-python = "~=3.10"
 dependencies = [
 	"anyio ~=3.0",
 	"async-generator ~=1.2",
-	"kilter.protocol ~=0.2.1",
+	"kilter.protocol ~=0.6.0",
+	"typing-extensions ~=4.0",
 ]
 classifiers = [
 	"Development Status :: 1 - Planning",
 	"Intended Audience :: Telecommunications Industry",
 	"License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 	"Topic :: Communications :: Email :: Filters",
 ]
 
 [project.optional-dependencies]
 tests = [
-	"trio",
+	"trio <0.22",  # Until anyio supports BaseExceptionGroup
 ]
 docs = [
 	"sphinx ~=5.0",
 	"myst-parser",
 	"sphinx-rtd-theme",
 ]
 
 [project.urls]
-Source = "https://code.kodo.org.uk/kilter/kilter.service"
-Documentation = "http://kilter.doc.kodo.org.uk/kilter.service"
+Source = "https://github.com/domsekotill/kilter.service"
+Issues = "https://github.com/domsekotill/kilter.service/issues"
+Documentation = "https://kilter.kodo.org.uk/kilter.service/"
 
 
 [tool.isort]
 force_single_line = true
 known_first_party = "kilter.protocol"
 
 
 [tool.unimport]
-include_star = true
 ignore_init = true
 
 
 [tool.flakeheaven]
 base = "https://code.kodo.org.uk/dom/project-templates/-/raw/main/.flakerules.toml"
-max_line_length = 92
-max_doc_length = 92
-
-[tool.flakeheaven.plugins]
-pycodestyle = ["-E701", "-E226"]
-
-[tool.flakeheaven.exceptions."tests/"]
-flake8-docstrings = ["-D100"]
-
-[tool.flakeheaven.exceptions."README.md"]
-flake8-docstrings = ["-*"]
-
-[tool.flakeheaven.exceptions."doc/*"]
-flake8-docstrings = ["-*"]
 
 
 [tool.mypy]
+python_version = "3.10"
 strict = true
 warn_unused_configs = true
 warn_unreachable = true
 namespace_packages = true
 explicit_package_bases = true
 allow_redefinition = true
 
@@ -85,32 +71,30 @@
 # disallow_any_expr = true
 
 
 [tool.coverage.run]
 data_file = "results/coverage.db"
 branch = true
 source = ["kilter"]
-plugins = [
-	"kodo.plugins.cover_test_context",
-]
 
 [tool.coverage.report]
 precision = 2
 skip_empty = true
 exclude_lines = [
-	"pragma: no-cover",
-	"if .*\\b__name__\\b",
-	"if .*\\bTYPE_CHECKING\\b",
+	"@(abc\\.)abstractmethod",
+	"@overload",
 	"class .*(.*\\bProtocol\\b.*):",
 	"def __repr__",
-	"@overload",
+	"if .*\\bTYPE_CHECKING\\b",
+	"if .*\\b__name__\\b",
+	"pragma: no-cover",
 ]
 partial_branches = [
-	"pragma: no-branch",
 	"if .*\\b__debug__\\b",
+	"pragma: no-branch",
 ]
 
 [tool.coverage.json]
 output = "results/coverage.json"
 show_contexts = true
 
 [tool.coverage.xml]
```

### Comparing `kilter.service-0.2.0/PKG-INFO` & `kilter_service-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: kilter.service
-Version: 0.2.0
+Version: 0.3.0
 Summary: High level, asynchronous framework for writing mail filters
 Author-email: Dom Sekotill <dom.sekotill@kodo.org.uk>
-Requires-Python: >=3.10,<4
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Dist: anyio ~=3.0
 Requires-Dist: async-generator ~=1.2
-Requires-Dist: kilter.protocol ~=0.2.1
+Requires-Dist: kilter.protocol ~=0.6.0
+Requires-Dist: typing-extensions ~=4.0
 Requires-Dist: sphinx ~=5.0 ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
-Requires-Dist: trio ; extra == "tests"
-Project-URL: Documentation, http://kilter.doc.kodo.org.uk/kilter.service
-Project-URL: Source, https://code.kodo.org.uk/kilter/kilter.service
+Requires-Dist: trio <0.22 ; extra == "tests"
+Project-URL: Documentation, https://kilter.kodo.org.uk/kilter.service/
+Project-URL: Issues, https://github.com/domsekotill/kilter.service/issues
+Project-URL: Source, https://github.com/domsekotill/kilter.service
 Provides-Extra: docs
 Provides-Extra: tests
 
 [![gitlab-ico]][gitlab-link]
 [![licence-mpl20]](/LICENCE.txt)
 [![pre-commit-ico]][pre-commit-link]
 [![pipeline-status]][pipeline-report]
@@ -63,14 +65,26 @@
 wishes to make use of async/await features.
 
 Use of `libmilter` to implement filters is almost universal as it is a black-box; the 
 on-the-wire protocol used is undocumented and subject to change between versions, which 
 makes writing a third-party parser difficult.
 
 
+Alternatives in the Python Space
+--------------------------------
+
+- [purepythonmilter](https://github.com/gertvdijk/purepythonmilter):
+  A modern and robust implementation for `asyncio`, written purely in statically typed 
+  Python without the need for `libmilter`.
+
+- [python-libmilter](https://github.com/crustymonkey/python-libmilter):
+	Another pure-Python module using threading. Lacks static type annotations and is no longer 
+	actively developed, although still minimally maintained.
+
+
 Usage
 =====
 
 To write filters, create a coroutine function that conforms to `Filter`.  This function 
 takes a `Session` object as its only argument.
 
 `Session` instances have several awaitable methods corresponding to SMTP commands 
@@ -121,30 +135,34 @@
 	async with session.headers as headers:
 		async for header in headers:
 			if header.name.startswith("X-"):
 				remove.append(header)
 
 	# remove the selected headers during the post phase
 	for header in remove:
-		await session.headers.remove(header)
+		await session.headers.delete(header)
+
+	return Accept()
 ```
 
 ```python
 from kilter.service import Session
 from kilter.protocol import Accept
 
 async def strip_x_headers(session: Session) -> Accept:
 	# collect the headers first
 	await session.headers.collect()
 
 	# iterate over collected headers during the post phase, removing the unwanted ones
 	async with session.headers as headers:
 		async for header in headers:
 			if header.name.startswith("X-"):
-				await session.headers.remove(header)
+				await session.headers.delete(header)
+
+	return Accept()
 ```
 
 
 ---
 
 [gitlab-ico]:
   https://img.shields.io/badge/GitLab-code.kodo.org.uk-blue.svg?logo=gitlab
```

