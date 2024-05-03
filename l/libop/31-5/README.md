# Comparing `tmp/libop-31.tar.gz` & `tmp/libop-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libop-31.tar", last modified: Fri May  3 16:17:51 2024, max compression
+gzip compressed data, was "libop-5.tar", last modified: Sun Dec 31 20:26:04 2023, max compression
```

## Comparing `libop-31.tar` & `libop-5.tar`

### file list

```diff
@@ -1,38 +1,51 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-03 16:17:51.252249 libop-31/
--rw-r--r--   0 bart      (1000) bart      (1001)     4047 2024-05-03 16:17:51.252249 libop-31/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     3513 2024-05-01 12:50:10.000000 libop-31/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-03 16:17:51.252249 libop-31/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3692 2024-05-03 15:26:03.000000 libop-31/bin/op
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-03 16:17:51.252249 libop-31/libop.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     4047 2024-05-03 16:17:51.000000 libop-31/libop.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      540 2024-05-03 16:17:51.000000 libop-31/libop.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-03 16:17:51.000000 libop-31/libop.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        3 2024-05-03 16:17:51.000000 libop-31/libop.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-03 16:17:51.000000 libop-31/libop.egg-info/zip-safe
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-03 16:17:51.252249 libop-31/op/
--rw-r--r--   0 bart      (1000) bart      (1001)       72 2024-05-03 13:32:18.000000 libop-31/op/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      744 2024-05-03 13:32:24.000000 libop-31/op/broker.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6318 2024-05-03 13:52:49.000000 libop-31/op/client.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4049 2024-05-03 13:53:07.000000 libop-31/op/disk.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1445 2024-05-03 13:32:55.000000 libop-31/op/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-03 16:17:51.252249 libop-31/op/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      447 2024-05-02 15:24:09.000000 libop-31/op/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      216 2024-05-02 16:30:37.000000 libop-31/op/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      369 2024-05-03 13:19:38.000000 libop-31/op/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      398 2024-05-03 13:19:55.000000 libop-31/op/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)      706 2024-05-03 13:44:51.000000 libop-31/op/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18737 2024-05-03 13:58:31.000000 libop-31/op/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      674 2024-05-03 13:30:24.000000 libop-31/op/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3528 2024-05-03 13:34:56.000000 libop-31/op/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-03 12:59:45.000000 libop-31/op/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)    10747 2024-05-03 13:28:19.000000 libop-31/op/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1127 2024-05-03 13:30:56.000000 libop-31/op/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      988 2024-05-03 13:29:34.000000 libop-31/op/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5121 2024-05-03 13:30:00.000000 libop-31/op/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6338 2024-05-03 13:33:05.000000 libop-31/op/object.py
--rw-r--r--   0 bart      (1000) bart      (1001)      281 2024-05-03 14:05:38.000000 libop-31/op/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3848 2024-05-03 14:31:34.000000 libop-31/op/thread.py
--rw-r--r--   0 bart      (1000) bart      (1001)      716 2024-05-03 14:01:17.000000 libop-31/op/utility.py
--rw-r--r--   0 bart      (1000) bart      (1001)      828 2024-05-03 14:58:37.000000 libop-31/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-03 16:17:51.252249 libop-31/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      164 2024-05-01 15:00:55.000000 libop-31/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.121652 libop-5/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-12-31 20:26:04.121652 libop-5/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      684 2023-12-31 20:25:48.000000 libop-5/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.117653 libop-5/libop.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      719 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        3 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/zip-safe
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.117653 libop-5/op/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1159 2023-12-31 14:57:27.000000 libop-5/op/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      131 2023-12-31 14:57:27.000000 libop-5/op/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      796 2023-12-31 19:31:40.000000 libop-5/op/brokers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      597 2023-12-31 19:31:09.000000 libop-5/op/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      557 2023-12-31 14:57:27.000000 libop-5/op/collect.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      741 2023-12-31 19:31:36.000000 libop-5/op/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      413 2023-12-31 14:57:27.000000 libop-5/op/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1551 2023-12-31 19:31:28.000000 libop-5/op/excepts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1230 2023-12-31 20:17:14.000000 libop-5/op/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2089 2023-12-31 14:57:27.000000 libop-5/op/locates.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      969 2023-12-31 19:31:46.000000 libop-5/op/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.121652 libop-5/op/mods/
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2023-12-31 20:17:54.000000 libop-5/op/mods/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      200 2023-12-31 14:57:34.000000 libop-5/op/mods/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-12-31 14:57:34.000000 libop-5/op/mods/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      473 2023-12-31 14:57:34.000000 libop-5/op/mods/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      718 2023-12-31 14:57:34.000000 libop-5/op/mods/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16008 2023-12-31 15:00:03.000000 libop-5/op/mods/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      629 2023-12-31 14:57:34.000000 libop-5/op/mods/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3496 2023-12-31 14:57:34.000000 libop-5/op/mods/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16920 2023-12-31 14:57:34.000000 libop-5/op/mods/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      189 2023-12-31 14:57:34.000000 libop-5/op/mods/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      624 2023-12-31 14:57:34.000000 libop-5/op/mods/mre.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      390 2023-12-31 14:57:34.000000 libop-5/op/mods/pwd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2349 2023-12-31 14:57:34.000000 libop-5/op/mods/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6982 2023-12-31 14:57:34.000000 libop-5/op/mods/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2638 2023-12-31 14:57:34.000000 libop-5/op/mods/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1025 2023-12-31 14:57:34.000000 libop-5/op/mods/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      984 2023-12-31 14:57:34.000000 libop-5/op/mods/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1920 2023-12-31 14:57:34.000000 libop-5/op/mods/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2817 2023-12-31 14:57:34.000000 libop-5/op/mods/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5766 2023-12-31 14:57:34.000000 libop-5/op/mods/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5608 2023-12-31 15:00:22.000000 libop-5/op/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6125 2023-12-31 14:57:27.000000 libop-5/op/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4958 2023-12-31 20:22:00.000000 libop-5/op/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2709 2023-12-31 14:57:27.000000 libop-5/op/storage.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2437 2023-12-31 19:31:59.000000 libop-5/op/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)       62 2023-12-31 14:57:27.000000 libop-5/op/utility.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      899 2023-12-31 20:21:50.000000 libop-5/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-12-31 20:26:04.121652 libop-5/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2023-12-31 14:56:01.000000 libop-5/setup.py
```

### Comparing `libop-31/bin/op` & `libop-5/op/runtime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,97 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,W0201,W0212,W0105,W0613,W0406,E0102,W0611,W0718,W0125,E0401
 
 
-"main"
+"runtime"
 
 
 import getpass
+import inspect
 import os
 import pwd
-import readline
 import sys
 import termios
 import time
+import _thread
 
 
-from op.client  import Client, Event, cmnd, init, parse_cmd, scan
-from op.disk    import Workdir, skel
-from op.object  import Default, cdir
-from op.runtime import broker, dte
-from op.utility import debug, enable, errors
+from .clients import Client
+from .command import Command
+from .default import Default
+from .excepts import Error, debug
+from .message import Event
+from .objects import Object
+from .parsers import parse_command, spl
+from .storage import Storage, cdir
+from .threads import launch
+
+
+def __dir__():
+    return (
+        'Cfg',
+        'Console',
+        'cmnd',
+        'daemon',
+        'forever',
+        'main',
+        'privileges',
+        'scan',
+        'wrap',
+        'wrapped'
+    )
+
+
+__all__ = __dir__()
+
+
+Cfg         = Default()
+Cfg.mod     = "cmd,err,mod,mre,pwd,thr"
+Cfg.name    = "op"
+Cfg.version = "5"
+Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Cfg.user    = getpass.getuser()
+Storage.wd  = Cfg.wd
 
 
-from op import modules
-
-
-Cfg             = Default()
-Cfg.dis         = ""
-Cfg.mod         = "cmd,mod"
-Cfg.opts        = ""
-Cfg.name        = __file__.rsplit(os.sep, maxsplit=1)[-1]
-Cfg.version     = "31"
-Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
-
-
-Workdir.workdir = Cfg.wdr
+from . import mods as modules
 
 
 class Console(Client):
 
-    "Console"
-
-    def __init__(self):
-        Client.__init__(self)
-        broker.add(self)
-
     def announce(self, txt):
-        "disable announce."
+        pass
 
     def callback(self, evt):
-        "wait for callback."
         Client.callback(self, evt)
         evt.wait()
 
-    def poll(self):
-        "poll console and create event."
+    def poll(self) -> Event:
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, _channel, txt):
-        "print to console"
+    def say(self, channel, txt):
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
+def cmnd(txt):
+    evn = Event()
+    evn.txt = txt
+    Command.handle(evn)
+    evn.wait()
+    return evn
+
+
 def daemon(pidfile, verbose=False):
-    "switch to background."
-    # pylint: disable=W0212
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
         os._exit(0)
@@ -89,67 +107,101 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
+def forever():
+    while 1:
+        try:
+            time.sleep(1.0)
+        except (KeyboardInterrupt, EOFError):
+            _thread.interrupt_main()
+
+
 def privileges(username):
-    "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
-def wrap(func):
-    "restore console."
+def scan(pkg, modstr, initer=False, wait=True) -> []:
+    mds = []
+    for modname in spl(modstr):
+        module = getattr(pkg, modname, None)
+        if not module:
+            continue
+        for _key, cmd in inspect.getmembers(module, inspect.isfunction):
+            if 'event' in cmd.__code__.co_varnames:
+                Command.add(cmd)
+        for _key, clz in inspect.getmembers(module, inspect.isclass):
+            if not issubclass(clz, Object):
+                continue
+            Storage.add(clz)
+        if initer and "init" in dir(module):
+            module._thr = launch(module.init, name=f"init {modname}")
+            mds.append(module)
+    if wait and initer:
+        for mod in mds:
+            mod._thr.join()
+    return mds
+
+
+def main():
+    Storage.skel()
+    parse_command(Cfg, " ".join(sys.argv[1:]))
+    if "a" in Cfg.opts:
+        Cfg.mod = ",".join(modules.__dir__())
+    if "v" in Cfg.opts:
+        dte = time.ctime(time.time()).replace("  ", " ")
+        debug(f"{Cfg.name.upper()} started {Cfg.opts.upper()} started {dte}")
+    if "d" in Cfg.opts:
+        daemon(Cfg.pidfile)
+        moddir = os.path.join(Storage.wd, "mods")
+        if os.path.exists(moddir) and "m" in Cfg.opts:
+            sys.path.insert(0, os.path.dirname(moddir))
+            import mods
+            if "a" in Cfg.opts:
+                Cfg.mod += "," +  ",".join(mods.__dir__())
+            scan(mods, Cfg.mod, True)
+        privileges(Cfg.user)
+        scan(modules, Cfg.mod, True)
+        forever()
+        return
+    if os.path.exists("mods") and "m" in Cfg.opts:
+        import mods
+        if "a" in Cfg.opts:
+            Cfg.mod += "," +  ",".join(mods.__dir__())
+        scan(mods, Cfg.mod)
+    csl = Console()
+    if "c" in Cfg.opts:
+        scan(modules, Cfg.mod, True, True)
+        csl.start()
+        forever()
+    if Cfg.otxt:
+        scan(modules, Cfg.mod)
+        return cmnd(Cfg.otxt)
+
+
+def wrap(func) -> None:
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
-def main():
-    "main"
-    parse_cmd(Cfg, " ".join(sys.argv[1:]))
-    skel()
-    if "a" in Cfg.opts:
-        Cfg.mod = ",".join(modules.__dir__())
-    if "v" in Cfg.opts:
-        enable(print)
-        debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
-        debug(f"scanned {Cfg.mod}")
-    if "h" in Cfg.opts:
-        print(__doc__)
-    elif "d" in Cfg.opts:
-        Cfg.mod  = ",".join(modules.__dir__())
-        Cfg.user = getpass.getuser()
-        daemon(Cfg.pidfile, "v" in Cfg.opts)
-        scan(modules, Cfg.mod)
-        privileges(Cfg.user)
-        init(modules, Cfg.mod)
-        while 1:
-            time.sleep(1.0)
-    elif "c" in Cfg.opts:
-        scan(modules, Cfg.mod, Cfg.sets.dis)
-        init(modules, Cfg.mod, Cfg.sets.dis)
-        csl = Console()
-        csl.start()
-        while 1:
-            time.sleep(1.0)
-    elif Cfg.otxt:
-        scan(modules, Cfg.mod, Cfg.sets.dis)
-        cmnd(Cfg.otxt, print)
+def wrapped():
+    wrap(main)
+    Error.show()
 
 
 if __name__ == "__main__":
-    readline.redisplay()
-    wrap(main)
-    errors()
+    wrapped()
```

### Comparing `libop-31/libop.egg-info/SOURCES.txt` & `libop-5/libop.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 README.rst
 pyproject.toml
 setup.py
-bin/op
 libop.egg-info/PKG-INFO
 libop.egg-info/SOURCES.txt
 libop.egg-info/dependency_links.txt
 libop.egg-info/top_level.txt
 libop.egg-info/zip-safe
 op/__init__.py
-op/broker.py
-op/client.py
-op/disk.py
+op/__main__.py
+op/brokers.py
+op/clients.py
+op/collect.py
+op/command.py
+op/default.py
+op/excepts.py
 op/handler.py
-op/object.py
+op/locates.py
+op/message.py
+op/objects.py
+op/parsers.py
 op/runtime.py
-op/thread.py
+op/storage.py
+op/threads.py
 op/utility.py
-op/modules/__init__.py
-op/modules/cmd.py
-op/modules/err.py
-op/modules/flt.py
-op/modules/fnd.py
-op/modules/irc.py
-op/modules/log.py
-op/modules/mbx.py
-op/modules/mod.py
-op/modules/rss.py
-op/modules/tdo.py
-op/modules/thr.py
-op/modules/tmr.py
+op/mods/__init__.py
+op/mods/cmd.py
+op/mods/dbg.py
+op/mods/err.py
+op/mods/fnd.py
+op/mods/irc.py
+op/mods/log.py
+op/mods/mbx.py
+op/mods/mdl.py
+op/mods/mod.py
+op/mods/mre.py
+op/mods/pwd.py
+op/mods/req.py
+op/mods/rss.py
+op/mods/rst.py
+op/mods/tdo.py
+op/mods/thr.py
+op/mods/tmr.py
+op/mods/udp.py
+op/mods/wsd.py
```

### Comparing `libop-31/op/client.py` & `libop-5/op/parsers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,141 +1,147 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=W0105
+# pylint: disable=C,R,W0718,W0702
 
 
-"client"
+"parsing text"
 
 
-import inspect
+import datetime
 import os
-import threading
+import re
+import time as ttime
 
 
-from .disk    import scancls
-from .handler import Handler
-from .object  import Default, Object
-from .thread  import later
+from .default import Default
 
 
-class Client(Handler):
-
-    "Client"
-
-    def __init__(self):
-        Handler.__init__(self)
-        self.register("command", command)
-
-    def announce(self, txt):
-        "announce text."
-        self.raw(txt)
-
-    def raw(self, txt):
-        "raw output."
-
-    def say(self, _channel, txt):
-        "say text in a channel."
-        self.raw(txt)
-
-    def show(self, evt):
-        "show results into a channel."
-        for txt in evt.result:
-            self.say(evt.channel, txt)
-
-
-class Command(Object): # pylint: disable=R0903
+def __dir__():
+    return (
+        'NoDate',
+        'fntime',
+        'get_day',
+        'get_hour',
+        'get_time',
+        'laps',
+        'parse_command',
+        'parse_time',
+        'spl',
+        'today',
+        'to_day'
+    )
 
-    "Command"
 
-    cmds = Object()
+__all__ = __dir__()
 
 
-class Event(Default): # pylint: disable=R0902
+bdmonths = [
+    'Bo',
+    'Jan',
+    'Feb',
+    'Mar',
+    'Apr',
+    'May',
+    'Jun',
+    'Jul',
+    'Aug',
+    'Sep',
+    'Oct',
+    'Nov',
+    'Dec'
+]
 
-    "Event"
 
-    def __init__(self):
-        Default.__init__(self)
-        self._thr    = None
-        self._ready  = threading.Event()
-        self.done    = False
-        self.orig    = None
-        self.result  = []
-        self.txt     = ""
-        self.type    = "event"
+year_formats = [
+    "%Y-%m-%d",
+    "%d-%m-%Y",
+    "%d-%m",
+    "%m-%d",
+]
 
-    def ready(self):
-        "event is ready."
-        self._ready.set()
 
-    def reply(self, txt):
-        "add text to the result"
-        self.result.append(txt)
+class NoDate(Exception):
 
-    def wait(self):
-        "wait for event to be ready."
-        if self._thr:
-            self._thr.join()
-        self._ready.wait()
-        return self.result
+    pass
 
 
-def add(func):
-    "add command."
-    setattr(Command.cmds, func.__name__, func)
+def extract_date(daystr):
+    for fmt in year_formats:
+        try:
+            res = ttime.mktime(ttime.strptime(daystr, fmt))
+        except:
+            res = None
+        if res:
+            return res
 
 
-"utilities"
+def fntime(daystr) -> float:
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    timed = ttime.mktime(ttime.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        timed += float('.' + rest)
+    return timed
 
 
-def cmnd(txt, outer):
-    "do a command using the provided output function."
-    clt = Client()
-    clt.raw = outer
-    evn = Event()
-    evn.orig = object.__repr__(clt)
-    evn.txt = txt
-    command(clt, evn)
-    evn.wait()
-    return evn
+def get_day(daystr):
+    try:
+        ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
+        (day, month, yea) = ymdre.groups()
+    except:
+        try:
+            ymre = re.search(r'(\d+)-(\d+)', daystr)
+            (day, month) = ymre.groups()
+            yea = ttime.strftime("%Y", ttime.localtime())
+        except Exception as ex:
+            raise NoDate(daystr) from ex
+    day = int(day)
+    month = int(month)
+    yea = int(yea)
+    date = "%s %s %s" % (day, bdmonths[month], yea)
+    return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
 
 
-def command(bot, evt):
-    "check for and run a command."
-    parse_cmd(evt)
-    func = getattr(Command.cmds, evt.cmd, None)
-    if func:
-        try:
-            func(evt)
-        except Exception as exc: # pylint: disable=W0718
-            later(exc)
-    bot.show(evt)
-    evt.ready()
+def get_hour(daystr):
+    try:
+        hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
+        hours = 60 * 60 * (int(hmsre.group(1)))
+        hoursmin = hours  + int(hmsre.group(2)) * 60
+        hmsres = hoursmin + int(hmsre.group(3))
+    except AttributeError:
+        pass
+    except ValueError:
+        pass
+    try:
+        hmre = re.search(r'(\d+):(\d+)', str(daystr))
+        hours = 60 * 60 * (int(hmre.group(1)))
+        hmsres = hours + int(hmre.group(2)) * 60
+    except AttributeError:
+        return 0
+    except ValueError:
+        return 0
+    return hmsres
 
 
-def init(pkg, modstr, disable=""):
-    "start modules"
-    mds = []
-    for modname in spl(modstr):
-        if skip(modname, disable):
-            continue
-        mod = getattr(pkg, modname, None)
-        if not mod:
-            continue
-        if "init" in dir(mod):
-            try:
-                mod.init()
-                mds.append(mod)
-            except Exception as ex: # pylint: disable=W0718
-                later(ex)
-    return mds
+def get_time(txt):
+    try:
+        target = get_day(txt)
+    except NoDate:
+        target = to_day(today())
+    hour =  get_hour(txt)
+    if hour:
+        target += hour
+    return target
 
 
-def laps(seconds, short=True):
-    "show elapsed time."
+def laps(seconds, short=True) -> str:
     txt = ""
     nsec = float(seconds)
     if nsec < 1:
         return f"{nsec:.2f}s"
     yea = 365*24*60*60
     week = 7*24*60*60
     nday = 24*60*60
@@ -166,21 +172,15 @@
         txt += f"{minutes}m"
     if sec:
         txt += f"{sec}s"
     txt = txt.strip()
     return txt
 
 
-def lsmod(pth):
-    "return list of modules in a directory."
-    return ",".join(sorted([x[:-3] for x in os.listdir(pth) if not x.startswith("__")]))
-
-
-def parse_cmd(obj, txt=None):
-    "parse a string for a command."
+def parse_command(obj, txt=None) -> None:
     args = []
     obj.args    = obj.args or []
     obj.cmd     = obj.cmd or ""
     obj.gets    = obj.gets or Default()
     obj.hasmods = obj.hasmod or False
     obj.index   = None
     obj.mod     = obj.mod or ""
@@ -225,64 +225,55 @@
         obj.txt  = obj.cmd or ""
         obj.rest = " ".join(obj.args)
         obj.txt  = obj.cmd + " " + obj.rest
     else:
         obj.txt = obj.cmd or ""
 
 
-def scancmd(mod) -> None:
-    "scan module for commands."
-    for key, cmd in inspect.getmembers(mod, inspect.isfunction):
-        if key.startswith("cb"):
-            continue
-        if 'event' in cmd.__code__.co_varnames:
-            add(cmd)
-
-
-def scan(pkg, modstr, disable=""):
-    "scan modules for commands and classes"
-    mds = []
-    for modname in spl(modstr):
-        if skip(modname, disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        scancmd(module)
-        scancls(module)
-    return mds
-
-
-def skip(name, skipp):
-    "check for skipping"
-    for skp in spl(skipp):
-        if skp in name:
-            return True
-    return False
+def parse_time(txt):
+    seconds = 0
+    target = 0
+    txt = str(txt)
+    for word in txt.split():
+        if word.startswith("+"):
+            seconds = int(word[1:])
+            return ttime.time() + seconds
+        if word.startswith("-"):
+            seconds = int(word[1:])
+            return ttime.time() - seconds
+    if not target:
+        try:
+            target = get_day(txt)
+        except NoDate:
+            target = to_day(today())
+        hour =  get_hour(txt)
+        if hour:
+            target += hour
+    return target
 
 
-def spl(txt):
-    "split comma separated string into a list."
+def spl(txt) -> []:
     try:
         res = txt.split(',')
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
 
 
-"interface"
+def to_day(daystr):
+    previous = ""
+    line = ""
+    daystr = str(daystr)
+    for word in daystr.split():
+        line = previous + " " + word
+        previous = word
+        try:
+            res = extract_date(line.strip())
+        except ValueError:
+            res = None
+        if res:
+            return res
+        line = ""
 
 
-def __dir__():
-    return (
-        'Client',
-        'Commands',
-        'Event',
-        'add',
-        'cmnd',
-        'command',
-        'lapse',
-        'init',
-        'parse_cmd',
-        'scan',
-        'spl'
-    )
+def today():
+    return str(datetime.datetime.today()).split()[0]
```

### Comparing `libop-31/op/handler.py` & `libop-5/op/handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,62 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=W0105
+# pylint: disable=C,R,W0201,W0212,W0105,W0613,W0406,E0102,W0611,W0718,W0125
 
 
 "handler"
 
 
 import queue
 import threading
 import _thread
 
 
-from .object import Object
-from .thread import launch
+from .objects import Object
+from .threads import launch
 
 
-class Handler:
+def __dir__():
+    return (
+        'Handler',
+   ) 
+
 
-    "Handler"
+__all__ = __dir__()
+
+
+class Handler(Object):
 
     def __init__(self):
+        Object.__init__(self)
         self.cbs      = Object()
         self.queue    = queue.Queue()
         self.stopped  = threading.Event()
-        self.threaded = True
 
-    def callback(self, evt):
-        "call callback based on event type."
+    def callback(self, evt) -> None:
         func = getattr(self.cbs, evt.type, None)
         if not func:
             evt.ready()
             return
-        evt._thr = launch(func, self, evt) # pylint: disable=W0212
+        evt._thr = launch(func, evt)
 
-    def loop(self):
-        "proces events until interrupted."
+    def loop(self) -> None:
         while not self.stopped.is_set():
             try:
-                evt = self.poll()
-                self.callback(evt)
+                self.callback(self.poll())
             except (KeyboardInterrupt, EOFError):
                 _thread.interrupt_main()
 
     def poll(self):
-        "function to return event."
         return self.queue.get()
 
-    def put(self, evt):
-        "put event into the queue."
+    def put(self, evt) -> None:
         self.queue.put_nowait(evt)
 
-    def register(self, typ, cbs):
-        "register callback for a type."
+    def register(self, typ, cbs) -> None:
         setattr(self.cbs, typ, cbs)
 
-    def start(self):
-        "start the event loop."
+    def start(self) -> None:
         launch(self.loop)
 
-    def stop(self):
-        "stop the event loop."
+    def stop(self) -> None:
         self.stopped.set()
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Handler',
-    )
```

### Comparing `libop-31/op/modules/irc.py` & `libop-5/op/mods/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,47 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,E1101,W0105,W0718,W0612,E0611
 
 
 "internet relay chat"
 
 
-import base64
 import os
 import queue
 import socket
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from op.client  import Client, Event, command
-from op.disk    import last, sync, whitelist
-from op.object  import Default, Object, edit, fmt, keys, values
-from op.runtime import broker
-from op.thread  import later, launch
-from op.utility import Debug, debug
+from .. import Default, Object, edit, fmt, keys
+from .. import Client, Command, Error, Event
+from .. import byorig, debug, last, launch, write
 
 
-NAME    = __file__.split(os.sep)[-3]
-saylock = _thread.allocate_lock()
+Error.filter = ["PING", "PONG", "PRIVMSG"]
+
 
+NAME = "op"
 
-Debug.filter = ["PING", "PONG", "PRIVMSG"]
+
+saylock = _thread.allocate_lock()
 
 
 def init():
-    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
     return irc
 
 
-def shutdown():
-    "shutdown irc bot."
-    for bot in values(broker.objs):
-        if "irc" not in str(type(bot)).lower():
-            continue
-        debug(f"IRC stopping {repr(bot)}")
-        bot.state.pongcheck = True
-        bot.state.keeprunning = False
-        bot.events.connected.clear()
-        bot.stop()
-
-
-class Config(Default): # pylint: disable=R0902,R0903
-
-    "Config"
+class Config(Default):
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
@@ -76,21 +61,16 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
-whitelist(Config)
-
-
 class TextWrap(textwrap.TextWrapper):
 
-    "TextWrap"
-
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -98,54 +78,46 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
-    "Output"
-
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
-        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
-        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
-        chanlist = getattr(Output.cache, channel)
-        chanlist.extend(txtlist)
+        Output.cache[channel].extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
-        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
-        "put text to output queue."
-        if channel and channel not in dir(Output.cache):
+        if channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
-        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -160,39 +132,34 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
-        "return size of channel cache."
         if chan in Output.cache:
-            return len(getattr(Output.cache, chan, []))
+            return len(Output.cache.get(chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
-    "IRC"
-
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
-        self.channels = []
         self.events = Default()
         self.events.authed = threading.Event()
         self.events.connected = threading.Event()
         self.events.joined = threading.Event()
         self.events.ready = threading.Event()
+        self.channels = []
         self.sock = None
         self.state = Default()
-        self.state.dostop = False
-        self.state.error = ""
         self.state.keeprunning = False
         self.state.lastline = ""
         self.state.nrconnect = 0
         self.state.nrsend = 0
         self.zelf = ''
         self.register('903', cb_h903)
         self.register('904', cb_h903)
@@ -200,23 +167,20 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
-        broker.add(self)
 
     def announce(self, txt):
-        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
-    def docommand(self, cmd, *args):
-        "send command to server."
+    def command(self, cmd, *args):
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -225,15 +189,14 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
-        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
             debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
@@ -252,113 +215,101 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
-        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
-        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as _ex:
+               ) as ex:
             pass
-        except Exception as ex: # pylint: disable=W0718
-            later(ex)
+        except Exception as ex:
+            Error.errors.append(ex)
 
     def doconnect(self, server, nck, port=6667):
-        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
-                self.state.error = str(ex)
+                self.state.errors = str(ex)
                 debug(str(ex))
             debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
-        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
-            self.docommand('PONG', evt.txt or '')
+            self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.docommand(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
+                self.command(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
             self.zelf = evt.args[-1]
         elif cmd == "376":
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
-            self.state.error = ""
+            self.state.errors = []
             self.events.joined.set()
         elif cmd == '433':
-            self.state.error = txt
+            self.state.errors = txt
             nck = self.cfg.nick + '_'
-            self.docommand('NICK', nck)
+            self.command('NICK', nck)
         return evt
 
     def joinall(self):
-        "join all channels."
         for channel in self.channels:
-            self.docommand('JOIN', channel)
+            self.command('JOIN', channel)
 
     def keep(self):
-        "keep alive."
         while not self.stopped.is_set():
-            if self.state.stopkeep:
-                self.state.stopkeep = False
-                break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
-            self.docommand('PING', self.cfg.server)
+            self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
-        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
-        "parse text into an event."
-        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -412,15 +363,14 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -428,27 +378,26 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                later(ex)
+                Error.add(ex)
                 self.stop()
                 debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
-        "send raw text."
         txt = txt.rstrip()
         debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
@@ -456,214 +405,173 @@
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                later(ex)
+                Error.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        "reconnect to server."
         debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
-        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
-        self.docommand('PRIVMSG', channel, txt)
+        self.command('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
-        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
-        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
-        launch(Client.start, self)
+        Client.start(self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        "stop bot."
-        self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
-        "wait for ready."
         self.events.ready.wait()
 
 
-def cb_auth(bot, evt):
-    "auth callback."
-    bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
+def cb_auth(evt):
+    bot = byorig(evt.orig)
+    bot.command(f'AUTHENTICATE {bot.cfg.password}')
 
 
-def cb_cap(bot, evt):
-    "capabilities callback."
+def cb_cap(evt):
+    bot = byorig(evt.orig)
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
-def cb_error(bot, evt):
-    "error callback."
-    if not bot.state.nrerror:
-        bot.state.nrerror = 0
+def cb_error(evt):
+    bot = byorig(evt.orig)
     bot.state.nrerror += 1
-    bot.state.error = evt.txt
+    bot.state.errors.append(evt.txt)
     debug(evt.txt)
 
 
-def cb_h903(bot, evt):
-    "auth succeded callback."
+def cb_h903(evt):
+    bot = byorig(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_h904(bot, evt):
-    "auth succeded callback."
+def cb_h904(evt):
+    bot = byorig(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_kill(bot, evt):
-    "got killed callback."
+def cb_kill(evt):
+    pass
 
 
-def cb_log(bot, evt):
-    "log callback."
+def cb_log(evt):
+    pass
 
 
-def cb_ready(bot, evt):
-    "bot is ready callback."
-    bot.events.ready.set()
+def cb_ready(evt):
+    bot = byorig(evt.orig)
+    if bot:
+        bot.events.ready.set()
 
 
-def cb_001(bot, evt):
-    "first line received callback."
+def cb_001(evt):
+    bot = byorig(evt.orig)
     bot.logon()
 
 
-def cb_notice(bot, evt):
-    "notice callback."
+def cb_notice(evt):
+    bot = byorig(evt.orig)
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
-        bot.docommand('NOTICE', evt.channel, txt)
+        bot.command('NOTICE', evt.channel, txt)
 
 
-def cb_privmsg(bot, evt):
-    "privmsg callback."
+def cb_privmsg(evt):
+    bot = byorig(evt.orig)
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
         debug(f"command from {evt.origin}: {evt.txt}")
-        command(bot, evt)
+        Command.handle(evt)
 
 
-def cb_quit(bot, evt):
-    "quit callback."
+def cb_quit(evt):
+    bot = byorig(evt.orig)
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
+"commands"
+
+
 def cfg(event):
-    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
                         skip='control,password,realname,sleep,username'.split(",")
                        )
                    )
     else:
         edit(config, event.sets)
-        sync(config, path)
+        write(config, path)
         event.reply('ok')
-
-
-def mre(event):
-    "show from output cache."
-    if not event.channel:
-        event.reply('channel is not set.')
-        return
-    bot = broker.get(event.orig)
-    if 'cache' not in dir(bot):
-        event.reply('bot is missing cache')
-        return
-    if event.channel not in bot.cache:
-        event.reply(f'no output in {event.channel} cache.')
-        return
-    for _x in range(3):
-        txt = bot.gettxt(event.channel)
-        if txt:
-            bot.say(event.channel, txt)
-    size = bot.size(event.channel)
-    event.reply(f'{size} more in cache')
-
-
-def pwd(event):
-    "create a base64 password."
-    if len(event.args) != 2:
-        event.reply('pwd <nick> <password>')
-        return
-    arg1 = event.args[0]
-    arg2 = event.args[1]
-    txt = f'\x00{arg1}\x00{arg2}'
-    enc = txt.encode('ascii')
-    base = base64.b64encode(enc)
-    dcd = base.decode('ascii')
-    event.reply(dcd)
```

### Comparing `libop-31/op/modules/log.py` & `libop-5/op/mods/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0115,C0116,E0402,R0903,E0611
 
 
 "log text"
 
 
 import time
 
 
-from ..client import laps
-from ..disk   import find, fntime, sync
-from ..object import Object
+from .. import Object, find, fntime, laps, write
 
 
-class Log(Object): # pylint: disable=R0903
-
-    "Log"
+class Log(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
 def log(event):
-    "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
-    sync(obj)
+    write(obj)
     event.reply('ok')
```

### Comparing `libop-31/op/modules/mbx.py` & `libop-5/op/mods/mbx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105
+# pylint: disable=C0103,C0209,C0301,C0115,C0116,W0212,R0903
 
 
 "mailbox"
 
 
 import mailbox
 import os
 import time
 
 
-from ..client import laps
-from ..disk   import find, fntime, sync, whitelist
-from ..object import Object, fmt, update
+from .. import Object, find, fmt, fntime, laps, write, update
 
 
-MONTH = {
+bdmonths = ['Bo', 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
+
+
+monthint = {
     'Jan': 1,
     'Feb': 2,
     'Mar': 3,
     'Apr': 4,
     'May': 5,
     'Jun': 6,
     'Jul': 7,
@@ -30,91 +31,84 @@
     'Nov': 11,
     'Dec': 12
 }
 
 
 class Email(Object):
 
-    "Email"
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.text = ""
 
 
-whitelist(Email)
-
-
 def to_date(date):
-    "match date in string." 
     date = date.replace("_", ":")
     res = date.split()
     ddd = ""
     try:
         if "+" in res[3]:
             raise ValueError
         if "-" in res[3]:
             raise ValueError
         int(res[3])
-        ddd = "{:4}-{:#02}-{:#02} {:6}".format(res[3], MONTH[res[2]], int(res[1]), res[4])
+        ddd = "{:4}-{:#02}-{:#02} {:6}".format(res[3], monthint[res[2]], int(res[1]), res[4])
     except (IndexError, KeyError, ValueError) as ex:
         try:
             if "+" in res[4]:
                 raise ValueError from ex
             if "-" in res[4]:
                 raise ValueError from ex
             int(res[4])
-            ddd = "{:4}-{:#02}-{:02} {:6}".format(res[4], MONTH[res[1]], int(res[2]), res[3])
+            ddd = "{:4}-{:#02}-{:02} {:6}".format(res[4], monthint[res[1]], int(res[2]), res[3])
         except (IndexError, KeyError, ValueError):
             try:
-                ddd = "{:4}-{:#02}-{:02} {:6}".format(res[2], MONTH[res[1]], int(res[0]), res[3])
+                ddd = "{:4}-{:#02}-{:02} {:6}".format(res[2], monthint[res[1]], int(res[0]), res[3])
             except (IndexError, KeyError):
                 try:
-                    ddd = "{:4}-{:#02}-{:02}".format(res[2], MONTH[res[1]], int(res[0]))
+                    ddd = "{:4}-{:#02}-{:02}".format(res[2], monthint[res[1]], int(res[0]))
                 except (IndexError, KeyError):
                     try:
-                        ddd = "{:4}-{:#02}".format(res[2], MONTH[res[1]])
+                        ddd = "{:4}-{:#02}".format(res[2], monthint[res[1]])
                     except (IndexError, KeyError):
                         try:
                             ddd = "{:4}".format(res[2])
                         except (IndexError, KeyError):
                             ddd = ""
     return ddd
 
 
 def cor(event):
-    "correspondence"
     if not event.args:
         event.reply("cor <email>")
         return
     nr = -1
     for _fn, email in find("email", {"From": event.args[0]}):
         nr += 1
         txt = ""
         if len(event.args) > 1:
             txt = ",".join(event.args[1:])
         else:
             txt = "From,Subject"
         event.reply("%s %s %s" % (nr, fmt(email, txt, plain=True), laps(time.time() - fntime(email.__stp__))))
 
 
+
 def eml(event):
-    "emnail"
     if not event.args:
         event.reply("eml <searchtxtinemail>")
         return
     nr = -1
     for fn, o in find("email"):
         if event.rest in o.text:
             nr += 1
             event.reply("%s %s %s" % (nr, fmt(o, "From,Subject"), laps(time.time() - fntime(fn))))
 
 
+
 def mbx(event):
-    "mailbox"
     if not event.args:
         return
     fn = os.path.expanduser(event.args[0])
     event.reply("reading from %s" % fn)
     nr = 0
     if os.path.isdir(fn):
         thing = mailbox.Maildir(fn, create=False)
@@ -124,17 +118,17 @@
         return
     try:
         thing.lock()
     except FileNotFoundError:
         pass
     for m in thing:
         o = Email()
-        update(o, m._headers) # pylint: disable=W0212
+        update(o, m._headers)
         o.text = ""
         for payload in m.walk():
             if payload.get_content_type() == 'text/plain':
                 o.text += payload.get_payload()
         o.text = o.text.replace("\\n", "\n")
-        sync(o)
+        write(o)
         nr += 1
     if nr:
         event.reply("ok %s" % nr)
```

### Comparing `libop-31/op/modules/tdo.py` & `libop-5/op/mods/tdo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0115,C0116,R0903,W0105,E0402,E0611
 
 
 "todo list"
 
 
 import time
 
 
-from ..client import laps
-from ..disk   import fntime, find, sync
-from ..object import Object
+from .. import Object, fntime, find, laps, write
 
 
-class NoDate(Exception): # pylint: disable=R0903
+class NoDate(Exception):
 
-    "no matching date"
+    pass
 
 
-class Todo(Object): # pylint: disable=R0903
-
-    "Todo"
+class Todo(Object):
 
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
 
 def dne(event):
-    "flag todo as done."
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
     nmr = 0
     for fnm, obj in find('todo', selector):
         nmr += 1
         obj.__deleted__ = True
-        sync(obj, fnm)
+        write(obj, fnm)
         event.reply('ok')
         break
     if not nmr:
         event.reply("nothing todo")
 
 
 def tdo(event):
-    "add todo."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply("no todo")
         return
     obj = Todo()
     obj.txt = event.rest
-    sync(obj)
+    write(obj)
     event.reply('ok')
```

### Comparing `libop-31/op/modules/thr.py` & `libop-5/op/mods/thr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0116,W0105,E0402,E0401,E0611
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..client import laps
-from ..object import Object, update
+from .. import Object, laps, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
-    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
```

### Comparing `libop-31/op/object.py` & `libop-5/op/objects.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,166 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=W0105
+# pylint: disable=C,R,E0603,E0402,W0401,W0614,W0611,W0622,W0105
 
 
-"clean namespace"
+"a clean namespace"
 
 
+import datetime
 import json
 import os
-import pathlib
-import _thread
+import sys
+import types
 
 
-lock = _thread.allocate_lock()
+def __dir__():
+    return (
+            'Object',
+            'construct',
+            'dump',
+            'dumps',
+            'edit',
+            'fmt',
+            'fqn',
+            'ident',
+            'items',
+            'keys',
+            'load',
+            'loads',
+            'name',
+            'update',
+            'values',
+           )
+
 
+__all__ = __dir__()
 
-class Object: # pylint: disable=R0902
 
-    "Object"
+class Object:
+
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
+    def __repr__(self):
+        return dumps(self)
+
     def __str__(self):
         return str(self.__dict__)
 
 
-class Default(Object): # pylint: disable=R0902,R0903
+"decoder"
+
+
+class ObjectDecoder(json.JSONDecoder):
+
+    def decode(self, s, _w=None):
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
+
+    def raw_decode(self, s, idx=0):
+        return json.JSONDecoder.raw_decode(self, s, idx)
+
+
+def hook(objdict, typ=None) -> Object:
+    if typ:
+        obj = typ()
+    else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw) -> Object:
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw) -> Object:
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+"encoder"
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    def default(self, o) -> str:
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(
+                      o,
+                      (
+                       type(str),
+                       type(True),
+                       type(False),
+                       type(int),
+                       type(float)
+                      )
+                     ):
+            return o
+        try:
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return object.__repr__(o)
+
+    def encode(self, o) -> str:
+        return json.JSONEncoder.encode(self, o)
+
+    def iterencode(
+                   self,
+                   o,
+                   _one_shot=False
+                  ) -> str:
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
+
+
+def dump(*args, **kw) -> None:
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
 
-    "Default"
+def dumps(*args, **kw) -> str:
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
 
-    def __getattr__(self, key):
-        return self.__dict__.get(key, "")
 
+"methods"
 
 
-def construct(obj, *args, **kwargs):
-    "construct an object from provided arguments."
+def construct(obj, *args, **kwargs) -> None:
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
             update(obj, val)
         elif isinstance(val, Object):
             update(obj, vars(val))
     if kwargs:
         update(obj, kwargs)
 
 
-def edit(obj, setter, skip=False):
-    "edit an object from provided dict/dict-like."
+def edit(obj, setter, skip=False) -> None:
     for key, val in items(setter):
         if skip and val == "":
             continue
         try:
             setattr(obj, key, int(val))
             continue
         except ValueError:
@@ -74,16 +174,15 @@
             setattr(obj, key, True)
         elif val in ["False", "false"]:
             setattr(obj, key, False)
         else:
             setattr(obj, key, val)
 
 
-def fmt(obj, args=None, skip=None, plain=False):
-    "format an object to a printable string."
+def fmt(obj, args=None, skip=None, plain=False) -> str:
     if args is None:
         args = keys(obj)
     if skip is None:
         skip = []
     txt = ""
     for key in args:
         if key.startswith("__"):
@@ -94,200 +193,60 @@
         if value is None:
             continue
         if plain:
             txt += f"{value} "
         elif isinstance(value, str) and len(value.split()) >= 2:
             txt += f'{key}="{value}" '
         else:
-            txt += f"{key}={value} "
+            txt += f'{key}={value} '
     return txt.strip()
 
 
-def fqn(obj):
-    "return full qualified name of an object."
+def fqn(obj) -> str:
     kin = str(type(obj)).split()[-1][1:-2]
     if kin == "type":
         kin = obj.__name__
     return kin
 
 
-def items(obj):
-    "return the items of an object."
+def ident(obj) -> str:
+    return os.path.join(
+                        fqn(obj),
+                        os.path.join(*str(datetime.datetime.now()).split())
+                       )
+
+def items(obj) -> []:
     if isinstance(obj, type({})):
         return obj.items()
     return obj.__dict__.items()
 
 
-def keys(obj):
-    "return keys of an object."
+def keys(obj) -> []:
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
-def read(obj, pth):
-    "read an object from file path."
-    with lock:
-        with open(pth, 'r', encoding='utf-8') as ofile:
-            update(obj, load(ofile))
-
-
-def search(obj, selector):
-    "check if object matches provided values."
-    res = False
-    if not selector:
-        return True
-    for key, value in items(selector):
-        val = getattr(obj, key, None)
-        if str(value).lower() in str(val).lower():
-            res = True
-        else:
-            res = False
-            break
-    return res
+def name(obj) -> str:
+    typ = type(obj)
+    if isinstance(typ, types.ModuleType):
+        return obj.__name__
+    if '__self__' in dir(obj):
+        return f'{obj.__self__.__class__.__name__}.{obj.__name__}'
+    if '__class__' in dir(obj) and '__name__' in dir(obj):
+        return f'{obj.__class__.__name__}.{obj.__name__}'
+    if '__class__' in dir(obj):
+        return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
+    if '__name__' in dir(obj):
+        return f'{obj.__class__.__name__}.{obj.__name__}'
+    return None
 
 
-def update(obj, data, empty=True):
-    "update an object."
+def update(obj, data, empty=True) -> None:
     for key, value in items(data):
         if empty and not value:
             continue
         setattr(obj, key, value)
 
 
-def values(obj):
-    "return values of an object."
+def values(obj) -> []:
     return obj.__dict__.values()
-
-
-def write(obj, pth):
-    "write an object to disk."
-    with lock:
-        cdir(os.path.dirname(pth))
-        with open(pth, 'w', encoding='utf-8') as ofile:
-            dump(obj, ofile, indent=4)
-
-
-"decoder"
-
-
-class ObjectDecoder(json.JSONDecoder):
-
-    "ObjectDecoder"
-
-    def __init__(self, *args, **kwargs):
-        json.JSONDecoder.__init__(self, *args, **kwargs)
-
-    def decode(self, s, _w=None):
-        "decoding string to object."
-        val = json.JSONDecoder.decode(self, s)
-        if not val:
-            val = {}
-        return hook(val)
-
-    def raw_decode(self, s, idx=0):
-        "decode partial string to object."
-        return json.JSONDecoder.raw_decode(self, s, idx)
-
-
-def hook(objdict, typ=None):
-    "construct object from dict."
-    if typ:
-        obj = typ()
-    else:
-        obj = Object()
-    construct(obj, objdict)
-    return obj
-
-
-def load(fpt, *args, **kw):
-    "load object from file."
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.load(fpt, *args, **kw)
-
-
-def loads(string, *args, **kw):
-    "load object from string."
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.loads(string, *args, **kw)
-
-
-"encoder"
-
-
-class ObjectEncoder(json.JSONEncoder):
-
-    "ObjectEncoder"
-
-    def __init__(self, *args, **kwargs):
-        json.JSONEncoder.__init__(self, *args, **kwargs)
-
-    def default(self, o):
-        "return stringable value."
-        if isinstance(o, dict):
-            return o.items()
-        if isinstance(o, Object):
-            return vars(o)
-        if isinstance(o, list):
-            return iter(o)
-        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
-            return o
-        try:
-            return json.JSONEncoder.default(self, o)
-        except TypeError:
-            return o.__dict__
-
-    def encode(self, o) -> str:
-        "encode object to string."
-        return json.JSONEncoder.encode(self, o)
-
-    def iterencode(self, o, _one_shot=False):
-        "loop over object to encode to string."
-        return json.JSONEncoder.iterencode(self, o, _one_shot)
-
-
-def dump(*args, **kw):
-    "dump object to file."
-    kw["cls"] = ObjectEncoder
-    return json.dump(*args, **kw)
-
-
-def dumps(*args, **kw):
-    "dump object to string."
-    kw["cls"] = ObjectEncoder
-    return json.dumps(*args, **kw)
-
-
-def cdir(pth):
-    "create directory."
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
-"interface"
-
-
-def __dir__():
-    return (
-        'Object',
-        'Default',
-        'construct',
-        'dump',
-        'dumps',
-        'edit',
-        'fmt',
-        'fqn',
-        'hook',
-        'items',
-        'keys',
-        'load',
-        'loads',
-        'read',
-        'search',
-        'update',
-        'values',
-        'write'
-    )
```

### Comparing `libop-31/pyproject.toml` & `libop-5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 [build-system]
 requires = [
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
+
 [project]
 name = "libop"
 description = "original programmer"
-version = "31"
+version = "5"
 authors = [
-    {name = "Bart Thate",email = "bthate@dds.nl"},
+    {name = "Bart Thate",email = "libbotx@gmail.com"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
+
 [project.urls]
 "home" = "https://pypi.org/project/libop"
-"bugs" = "https://github.com/xobjectz/libop/issues"
-"source" = "https://github.com/xobjectz/libop"
+"bugs" = "https://github.com/botlibx/libop/issues"
+"source" = "https://github.com/botlibx/libop"
 
 
 [tool.setuptools]
-script-files = [
-    'bin/op',
-]
 packages = [
-    "op",
-    "op.modules"
+    'op',
+    'op.mods'
 ]
 zip-safe=true
 
 
 [tool.setuptools.data-files]
 "share/doc/libop" = [
-    "README.rst"
+    "README.rst",
 ]
+
+
+[tool.setuptools.exclude-package-data]
+"*" = [
+       "env*",
+       "html*",
+       "test*"
+      ]
```

