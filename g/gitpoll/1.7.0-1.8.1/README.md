# Comparing `tmp/gitpoll-1.7.0-py3-none-any.whl.zip` & `tmp/gitpoll-1.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 6605 bytes, number of entries: 14
+Zip file size: 7784 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       32 b- defN 24-Apr-30 16:31 gitpoll/__init__.py
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-30 13:20 gitpoll/args.py
--rw-r--r--  2.0 unx      484 b- defN 24-Apr-30 13:54 gitpoll/config.py
--rw-r--r--  2.0 unx     1436 b- defN 24-Apr-30 16:34 gitpoll/git.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-30 16:34 gitpoll/log.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-30 16:39 gitpoll/main.py
--rw-r--r--  2.0 unx     2049 b- defN 24-Apr-30 16:35 gitpoll/shell.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 16:39 gitpoll/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-30 16:39 gitpoll-1.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1153 b- defN 24-Apr-30 16:39 gitpoll-1.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 16:39 gitpoll-1.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-Apr-30 16:39 gitpoll-1.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-30 16:39 gitpoll-1.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1058 b- defN 24-Apr-30 16:39 gitpoll-1.7.0.dist-info/RECORD
-14 files, 11551 bytes uncompressed, 4865 bytes compressed:  57.9%
+-rw-r--r--  2.0 unx     1527 b- defN 24-May-03 07:39 gitpoll/args.py
+-rw-r--r--  2.0 unx      483 b- defN 24-May-03 07:39 gitpoll/config.py
+-rw-r--r--  2.0 unx      877 b- defN 24-May-03 02:43 gitpoll/git.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-03 02:09 gitpoll/log.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-03 07:37 gitpoll/main.py
+-rw-r--r--  2.0 unx     2072 b- defN 24-May-03 02:17 gitpoll/shell.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-03 08:58 gitpoll/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4576 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1057 b- defN 24-May-03 08:58 gitpoll-1.8.1.dist-info/RECORD
+14 files, 14868 bytes uncompressed, 6044 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: gitpoll/shell.py
 Comment: 
 
 Filename: gitpoll/version.py
 Comment: 
 
-Filename: gitpoll-1.7.0.dist-info/LICENSE
+Filename: gitpoll-1.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: gitpoll-1.7.0.dist-info/METADATA
+Filename: gitpoll-1.8.1.dist-info/METADATA
 Comment: 
 
-Filename: gitpoll-1.7.0.dist-info/WHEEL
+Filename: gitpoll-1.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: gitpoll-1.7.0.dist-info/entry_points.txt
+Filename: gitpoll-1.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: gitpoll-1.7.0.dist-info/top_level.txt
+Filename: gitpoll-1.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gitpoll-1.7.0.dist-info/RECORD
+Filename: gitpoll-1.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitpoll/args.py

```diff
@@ -2,41 +2,58 @@
 import os
 from argparse import ArgumentParser, Namespace
 
 
 def parse_args() -> Namespace:
     """Parse command line arguments for the gitpoll application."""
     parser = ArgumentParser(
-        description="Monitors a Git repository for changes and executes scripts before and after pulling updates."
+        description=(
+            "Monitors a Git repository for changes and executes "
+            + "scripts before and after pulling updates."
+        )
     )
     parser.add_argument(
         "repo_path",
         nargs="?",
         help="Path to the Git repository to monitor.",
         default=os.getcwd(),
         type=str,
     )
     parser.add_argument(
         "-i",
         "--interval",
         type=int,
         help="Interval in seconds to check for changes.",
+        required=False,
+        default=None,
     )
     parser.add_argument(
-        "-f",
+        "-n",
         "--no-pull",
         action="store_true",
         help="Do not pull changes from the repository.",
+        required=False,
     )
     parser.add_argument(
         "-p",
         "--pre-action",
         type=str,
         help="Command or path to the pre-action shell script or command.",
+        required=False,
     )
     parser.add_argument(
         "-P",
         "--post-action",
         type=str,
         help="Command or path to the post-action shell script or command.",
+        required=False,
     )
+    parser.add_argument(
+        '-f',
+        '--force',
+        action='store_true',
+        help='Force execution pre and post actions regardless of changes.',
+        required=False,
+        default=False,
+    )
+
     return parser.parse_args()
```

## gitpoll/config.py

```diff
@@ -1,12 +1,12 @@
 # Logging
+import os
+
 LOGGER_FILE = 'gitpoll.log'
 LOGGER_NAME = 'gitpoll'
 MAX_LOG_SIZE = 10 * 1024 * 1024 * 1024  # 10 GB
 MAX_LOG_FILES = 3  # Rotate over three files
-LOGGER_SET_LEVEL = 'INFO'
+LOGGER_SET_LEVEL = 'DEBUG'
 # Optimized log format: Date-Time Level[Logger]Module:Function:Line-Message
 # Example output: 2024-04-30 06:21 - INFO[gitpoll]main:main:22-Checking for changes in the repository.
-LOGGER_FORMAT = (
-    "%(asctime)s %(levelname)s " + "%(module)s:%(funcName)s %(message)s"
-)
+LOGGER_FORMAT = "%(asctime)s %(levelname)s %(module)s:%(funcName)s %(message)s"
 DATE_FORMAT = '%m-%d %H:%M:%S'
```

## gitpoll/git.py

```diff
@@ -1,17 +1,18 @@
 import os
 import subprocess as subproc
-from pyshared import default_repr as def_repr
+from pyshared.python import default_repr as def_repr
 from typing import Union as U, List, Dict, Optional as Opt, Tuple
 from logfunc import logf
 
 from .shell import CmdExec, CmdResult
 
 class GitCmds:
     def __init__(self, repo_path: str):
+        os.chdir(repo_path)
         self.repo_path = repo_path
         self.fetch = CmdExec('git fetch').execute()
         self.local = CmdExec('git rev-parse HEAD').execute()
         self.remote = CmdExec('git rev-parse @{u}').execute()
 
         self.success = (
             self.fetch.code == 0
@@ -24,24 +25,7 @@
 
     def __repr__(self):
         return def_repr(self)
 
     def __str__(self):
         return self.__repr__()
 
-
-# previous non-class version
-# def has_repo_changed(
-#     repo_path: str,
-# ) -> U[bool, Tuple[CmdExec, CmdExec, CmdExec]]:
-#     """Check if the repository has new changes by comparing local and remote heads."""
-#     ...
-#     fetch = CmdExec('git fetch')
-#     local = CmdExec('git rev-parse HEAD')
-#     remote = CmdExec('git rev-parse @{u}')
-#    return git_cmds.changed, (local, remote, fetch)
-
-
-def has_repo_changed(repo_path: str) -> GitCmds:
-    """Check if the repository has new changes by comparing local and remote heads."""
-    os.chdir(repo_path)
-    return GitCmds(repo_path)
```

## gitpoll/main.py

```diff
@@ -1,70 +1,71 @@
 #!/usr/bin/env python3
 
 import os
 import time
-
+import sys
+from argparse import ArgumentParser, Namespace
 from .shell import CmdExec
 from .args import parse_args
-from .git import has_repo_changed
+from .git import GitCmds
 from .log import logger
 
 
-def main():
-    args = parse_args()
-    repo_path = (
-        os.path.abspath(args.repo_path) if args.repo_path else os.getcwd()
-    )
-
-    if not os.path.exists(repo_path):
-        logger.error("Repository path '{}' does not exist.".format(repo_path))
-        return 1
-
-    logger.debug('args: {}'.format(args.__dict__))
-
-    while True:
-        logger.debug("Checking for changes in the repository.")
-        logger.debug("Repository path: {} Changing to...".format(repo_path))
-
-        os.chdir(repo_path)  # Change to the repository path
-
-        gitcmds = has_repo_changed(repo_path)
-        if gitcmds.changed:
-            logger.info("Repository has new changes.")
-            pre_action = (
-                args.pre_action
-                if args.pre_action
-                else "echo 'No pre-action configured'"
-            )
-            post_action = (
-                args.post_action
-                if args.post_action
-                else "echo 'No post-action configured'"
-            )
-            logger.debug("Pre-action: {}".format(pre_action))
-            logger.debug("Post-action: {}".format(post_action))
-            logger.debug("Executing pre-action.")
-            pre_cmd = CmdExec(pre_action)
-            logger.debug("Executed pre-action: {}".format(pre_cmd))
+def _log_exit(msg: str, code: int, logfunc: callable):
+    logfunc(msg)
+    sys.exit(code)
+
+
+def _mainloop(pargs: Namespace):
+    try:
+        gitcmds = GitCmds(pargs.repo_path)
+        if gitcmds.changed or pargs.force:
+            logger.debug("Repo Change" if gitcmds.changed else "Force Exec")
+            if pargs.pre_action:
+                logger.debug("Pre-action: {}".format(pargs.pre_action))
+                pre_cmd = CmdExec(pargs.pre_action)
+                logger.info(str(pre_cmd))
 
-            if not args.no_pull:
+            if not pargs.no_pull:
                 logger.info("Pulling changes from the repository.")
                 pull_cmd = CmdExec("git pull")
                 logger.info(str(pull_cmd))
 
-            post_cmd = CmdExec(post_action)
-            logger.info(str(post_cmd))
+            if pargs.post_action:
+                logger.debug("Post-action: {}".format(pargs.post_action))
+                post_cmd = CmdExec(pargs.post_action)
+                logger.info(str(post_cmd))
         else:
             logger.debug("No new changes in the repository.")
 
-        if not args.interval:
-            logger.debug("Monitoring stopped.")
-            return 0
+        if not pargs.interval:
+            _log_exit("Single run completed.", 0, logger.info)
+        else:
+            logger.debug("Sleeping for {} seconds.".format(pargs.interval))
+            time.sleep(pargs.interval)
+    except KeyboardInterrupt:
+        _log_exit("Exiting on keyboard interrupt.", 0, logger.info)
+    except Exception as e:
+        logger.error("Error: {}".format(e), exc_info=True)
+        sys.exit(1)
+
+
+def main():
+    args = parse_args()
+    repo_path = args.repo_path
+
+    if not os.path.exists(repo_path):
+        logger.error("Repository path '{}' does not exist.".format(repo_path))
+        return 1
 
-        logger.debug("Sleeping for {} seconds.".format(args.interval))
-        time.sleep(args.interval)
+    logger.debug("Changing to repository path: {}".format(repo_path))
+    os.chdir(repo_path)
 
-    return 1
+    logger.debug('args: {}'.format(args.__dict__))
+
+    while True:
+        logger.debug("Main loop iteration | ARGS {}".format(args.__dict__))
+        _mainloop(args)
 
 
 if __name__ == "__main__":
     main()
```

## gitpoll/shell.py

```diff
@@ -1,18 +1,18 @@
 import subprocess as subproc
 from subprocess import PIPE
 from typing import Union as U, List, Dict
 import shlex
-from pyshared import default_repr as def_repr
+from pyshared.python import default_repr as def_repr
 from logfunc import logf
 
 from .log import logger
 
 class CmdResult:
-    @logf(use_logger=logger)
+    @logf(level='debug', use_logger=logger)
     def __init__(self, code: int, stdout: str, stderr: str):
         self.code, self.stdout, self.stderr = code, stdout, stderr
 
     def __repr__(self):
         return def_repr(self)
 
     def __str__(self):
@@ -34,15 +34,15 @@
 class CmdExec:
     @logf(level='debug', use_logger=logger)
     def __init__(self, cmd: U[str, List[str]]):
         self.command = shlex.split(cmd) if isinstance(cmd, str) else cmd
         self.code, self.stdout, self.stderr = 0, "", ""
         self.execute()
 
-    @logf(level='info', use_logger=logger)
+    @logf(level='debug', use_logger=logger)
     def execute(self) -> CmdResult:
         try:
             process = subproc.Popen(
                 self.command, stdout=PIPE, stderr=PIPE, universal_newlines=True
             )
             self.stdout, self.stderr = process.communicate()
             self.code = process.returncode
```

## gitpoll/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.7.0'
+__version__ = '1.8.1'
```

## Comparing `gitpoll-1.7.0.dist-info/LICENSE` & `gitpoll-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

