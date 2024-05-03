# Comparing `tmp/revenge-0.21.tar.gz` & `tmp/revenge-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revenge-0.21.tar", last modified: Fri May  3 17:24:07 2024, max compression
+gzip compressed data, was "dist/revenge-0.9.tar", last modified: Tue Aug 20 04:01:42 2019, max compression
```

## Comparing `revenge-0.21.tar` & `revenge-0.9.tar`

### file list

```diff
@@ -1,209 +1,94 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.930709 revenge-0.21/
--rw-rw-r--   0 user      (1001) user      (1001)       88 2024-04-03 20:13:04.000000 revenge-0.21/MANIFEST.in
--rw-r--r--   0 user      (1001) user      (1001)     1478 2024-05-03 17:24:07.930709 revenge-0.21/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     3675 2024-05-03 17:17:59.000000 revenge-0.21/README.md
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.898709 revenge-0.21/revenge/
--rw-rw-r--   0 user      (1001) user      (1001)     3826 2024-04-03 20:13:04.000000 revenge-0.21/revenge/Colorer.py
--rw-rw-r--   0 user      (1001) user      (1001)      478 2024-04-03 20:13:04.000000 revenge-0.21/revenge/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.898709 revenge-0.21/revenge/cli/
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/cli/actions/
--rw-rw-r--   0 user      (1001) user      (1001)      218 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/actions/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3463 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/actions/differential_find.py
--rw-rw-r--   0 user      (1001) user      (1001)     4524 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/actions/find.py
--rw-rw-r--   0 user      (1001) user      (1001)     2999 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/actions/stalker.py
--rw-rw-r--   0 user      (1001) user      (1001)     4166 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/actions/windows_messages.py
--rw-rw-r--   0 user      (1001) user      (1001)     7245 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cli/cli.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/common/
--rw-rw-r--   0 user      (1001) user      (1001)    11424 2024-04-03 20:13:04.000000 revenge-0.21/revenge/common/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    12124 2024-04-03 20:13:04.000000 revenge-0.21/revenge/common/windows_keys_by_id.json
--rw-rw-r--   0 user      (1001) user      (1001)    24925 2024-04-03 20:13:04.000000 revenge-0.21/revenge/common/windows_messages_by_id.json
--rw-rw-r--   0 user      (1001) user      (1001)    24204 2024-04-03 20:13:04.000000 revenge-0.21/revenge/common/windows_messages_by_name.json
--rw-rw-r--   0 user      (1001) user      (1001)      252 2024-04-03 20:13:04.000000 revenge-0.21/revenge/config.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/contexts/
--rw-rw-r--   0 user      (1001) user      (1001)       87 2024-04-03 20:13:04.000000 revenge-0.21/revenge/contexts/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     8564 2024-04-03 20:13:04.000000 revenge-0.21/revenge/contexts/batch.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/cpu/
--rw-rw-r--   0 user      (1001) user      (1001)       90 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/cpu/assembly/
--rw-rw-r--   0 user      (1001) user      (1001)       60 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/assembly/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     5001 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/assembly/instruction.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/cpu/contexts/
--rw-rw-r--   0 user      (1001) user      (1001)     2980 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/contexts/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      268 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/contexts/arm.py
--rw-rw-r--   0 user      (1001) user      (1001)     2909 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/contexts/x64.py
--rw-rw-r--   0 user      (1001) user      (1001)     1311 2024-04-03 20:13:04.000000 revenge-0.21/revenge/cpu/contexts/x86.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.902709 revenge-0.21/revenge/devices/
--rw-rw-r--   0 user      (1001) user      (1001)      998 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/devices/android/
--rw-rw-r--   0 user      (1001) user      (1001)       36 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/android/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     8038 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/android/android.py
--rw-rw-r--   0 user      (1001) user      (1001)      966 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/android/applications.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/devices/local/
--rw-rw-r--   0 user      (1001) user      (1001)     1478 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/local/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/devices/process/
--rw-rw-r--   0 user      (1001) user      (1001)      115 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/process/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     1135 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/process/process.py
--rw-rw-r--   0 user      (1001) user      (1001)     1250 2024-04-03 20:13:04.000000 revenge-0.21/revenge/devices/process/processes.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/engines/
--rw-rw-r--   0 user      (1001) user      (1001)     2262 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/engines/frida/
--rw-rw-r--   0 user      (1001) user      (1001)    11824 2024-05-03 17:17:59.000000 revenge-0.21/revenge/engines/frida/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/engines/frida/devices/
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/devices/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)       88 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/devices/local_device.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.906709 revenge-0.21/revenge/engines/frida/memory/
--rw-rw-r--   0 user      (1001) user      (1001)      305 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/memory/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     2062 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/memory/find.py
--rw-rw-r--   0 user      (1001) user      (1001)      467 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/memory/map.py
--rw-rw-r--   0 user      (1001) user      (1001)     4264 2024-05-03 17:17:59.000000 revenge-0.21/revenge/engines/frida/memory/memory.py
--rw-rw-r--   0 user      (1001) user      (1001)    32341 2024-05-03 17:17:59.000000 revenge-0.21/revenge/engines/frida/memory/memory_bytes.py
--rw-rw-r--   0 user      (1001) user      (1001)     1145 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/memory/memory_range.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/angr/
--rw-rw-r--   0 user      (1001) user      (1001)       23 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/angr/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)       84 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/angr/angr.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/decompiler/
--rw-rw-r--   0 user      (1001) user      (1001)       36 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/decompiler/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      113 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/decompiler/decompiler.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/dwarf/
--rw-rw-r--   0 user      (1001) user      (1001)       88 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/dwarf/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/handles/
--rw-rw-r--   0 user      (1001) user      (1001)       29 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/handles/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      275 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/handles/handles.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/java/
--rw-rw-r--   0 user      (1001) user      (1001)      194 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/java/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      659 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/java/classes.py
--rw-rw-r--   0 user      (1001) user      (1001)     3945 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/java/java.py
--rw-rw-r--   0 user      (1001) user      (1001)    12996 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/java/java_class.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/frida/plugins/radare2/
--rw-rw-r--   0 user      (1001) user      (1001)       29 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/radare2/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)       98 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/frida/plugins/radare2/radare2.py
--rw-rw-r--   0 user      (1001) user      (1001)     7164 2024-05-03 17:17:59.000000 revenge-0.21/revenge/engines/frida/process.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.910709 revenge-0.21/revenge/engines/unicorn/
--rw-rw-r--   0 user      (1001) user      (1001)     1035 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.914709 revenge-0.21/revenge/engines/unicorn/memory/
--rw-rw-r--   0 user      (1001) user      (1001)      315 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/memory/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      217 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/memory/find.py
--rw-rw-r--   0 user      (1001) user      (1001)      189 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/memory/map.py
--rw-rw-r--   0 user      (1001) user      (1001)      599 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/memory/memory.py
--rw-rw-r--   0 user      (1001) user      (1001)     2531 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/memory/memory_bytes.py
--rw-rw-r--   0 user      (1001) user      (1001)      181 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/memory/memory_range.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.914709 revenge-0.21/revenge/engines/unicorn/plugins/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/plugins/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)       85 2024-04-03 20:13:04.000000 revenge-0.21/revenge/engines/unicorn/process.py
--rw-rw-r--   0 user      (1001) user      (1001)      812 2024-04-03 20:13:04.000000 revenge-0.21/revenge/exceptions.py
--rw-rw-r--   0 user      (1001) user      (1001)     4647 2024-04-03 20:13:04.000000 revenge-0.21/revenge/functions.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/js/
--rw-rw-r--   0 user      (1001) user      (1001)      409 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/dispose.js
--rw-rw-r--   0 user      (1001) user      (1001)      188 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/echo.js
--rw-rw-r--   0 user      (1001) user      (1001)      120 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/enumerate_modules.js
--rw-rw-r--   0 user      (1001) user      (1001)      164 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/enumerate_threads.js
--rw-rw-r--   0 user      (1001) user      (1001)      705 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/exception_handler.js
--rw-rw-r--   0 user      (1001) user      (1001)     1455 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/find_in_memory.js
--rw-rw-r--   0 user      (1001) user      (1001)      902 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/generic_suspend_until_true.js
--rw-rw-r--   0 user      (1001) user      (1001)      253 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/get_declared_fields.js
--rw-rw-r--   0 user      (1001) user      (1001)      272 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/get_declared_methods.js
--rw-rw-r--   0 user      (1001) user      (1001)     2830 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/instruction_count.js
--rw-rw-r--   0 user      (1001) user      (1001)      278 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/pause_at.js
--rw-rw-r--   0 user      (1001) user      (1001)      180 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/pause_at2.js
--rw-rw-r--   0 user      (1001) user      (1001)      549 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/replace_function.js
--rw-rw-r--   0 user      (1001) user      (1001)      476 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/resolve_location_address.js
--rw-rw-r--   0 user      (1001) user      (1001)      346 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/rw_everything.js
--rw-rw-r--   0 user      (1001) user      (1001)      563 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/rwx_everything.js
--rw-rw-r--   0 user      (1001) user      (1001)     1072 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/send_batch.js
--rw-rw-r--   0 user      (1001) user      (1001)      981 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/send_repeat.js
--rw-rw-r--   0 user      (1001) user      (1001)     6939 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/stalk.js
--rw-rw-r--   0 user      (1001) user      (1001)     3802 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/telescope.js
--rw-rw-r--   0 user      (1001) user      (1001)     9603 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/timeless.js
--rw-rw-r--   0 user      (1001) user      (1001)      398 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/windows_intercept_message_handler.js
--rw-rw-r--   0 user      (1001) user      (1001)     3134 2024-04-03 20:13:04.000000 revenge-0.21/revenge/js/windows_stalk_message_handlers.js
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/memory/
--rw-rw-r--   0 user      (1001) user      (1001)      213 2024-04-03 20:13:04.000000 revenge-0.21/revenge/memory/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3267 2024-04-03 20:13:04.000000 revenge-0.21/revenge/memory/find.py
--rw-rw-r--   0 user      (1001) user      (1001)      944 2024-04-03 20:13:04.000000 revenge-0.21/revenge/memory/map.py
--rw-rw-r--   0 user      (1001) user      (1001)    11519 2024-04-03 20:13:04.000000 revenge-0.21/revenge/memory/memory.py
--rw-rw-r--   0 user      (1001) user      (1001)    14061 2024-04-03 20:13:04.000000 revenge-0.21/revenge/memory/memory_bytes.py
--rw-rw-r--   0 user      (1001) user      (1001)     3041 2024-04-03 20:13:04.000000 revenge-0.21/revenge/memory/memory_range.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/modules/
--rw-rw-r--   0 user      (1001) user      (1001)      110 2024-04-03 20:13:04.000000 revenge-0.21/revenge/modules/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    10844 2024-04-03 20:13:04.000000 revenge-0.21/revenge/modules/module.py
--rw-rw-r--   0 user      (1001) user      (1001)     7967 2024-04-03 20:13:04.000000 revenge-0.21/revenge/modules/modules.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/native_error/
--rw-rw-r--   0 user      (1001) user      (1001)     2525 2024-04-03 20:13:04.000000 revenge-0.21/revenge/native_error/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     4420 2024-04-03 20:13:04.000000 revenge-0.21/revenge/native_exception.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/parsers/
--rw-rw-r--   0 user      (1001) user      (1001)       21 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/parsers/elf/
--rw-rw-r--   0 user      (1001) user      (1001)       22 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/elf/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     4589 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/elf/elf.py
--rw-rw-r--   0 user      (1001) user      (1001)     2067 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/elf/program_header.py
--rw-rw-r--   0 user      (1001) user      (1001)     1048 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/elf/program_headers.py
--rw-rw-r--   0 user      (1001) user      (1001)     1349 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/elf/section_header.py
--rw-rw-r--   0 user      (1001) user      (1001)     1208 2024-04-03 20:13:04.000000 revenge-0.21/revenge/parsers/elf/section_headers.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.918709 revenge-0.21/revenge/plugins/
--rw-rw-r--   0 user      (1001) user      (1001)      299 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/angr/
--rw-rw-r--   0 user      (1001) user      (1001)       24 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/angr/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     7201 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/angr/angr.py
--rw-rw-r--   0 user      (1001) user      (1001)     5970 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/angr/revenge_target.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/decompiler/
--rw-rw-r--   0 user      (1001) user      (1001)      120 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/decompiler/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     2021 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/decompiler/base.py
--rw-rw-r--   0 user      (1001) user      (1001)     9407 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/decompiler/decompiled.py
--rw-rw-r--   0 user      (1001) user      (1001)     3708 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/decompiler/decompiler.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/dwarf/
--rw-rw-r--   0 user      (1001) user      (1001)       72 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/dwarf/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     8540 2024-05-03 17:17:59.000000 revenge-0.21/revenge/plugins/dwarf/dwarf.py
--rw-rw-r--   0 user      (1001) user      (1001)     3945 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/dwarf/dwarf_decompiler.py
--rw-rw-r--   0 user      (1001) user      (1001)     1027 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/dwarf/dwarf_register_enums.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/handles/
--rw-rw-r--   0 user      (1001) user      (1001)       56 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/handles/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     5682 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/handles/handle.py
--rw-rw-r--   0 user      (1001) user      (1001)     1776 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/handles/handles.py
--rw-rw-r--   0 user      (1001) user      (1001)     3408 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/handles/linux.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/java/
--rw-rw-r--   0 user      (1001) user      (1001)      144 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/java/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     1226 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/java/classes.py
--rw-rw-r--   0 user      (1001) user      (1001)     1934 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/java/java.py
--rw-rw-r--   0 user      (1001) user      (1001)      236 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/java/java_class.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/radare2/
--rw-rw-r--   0 user      (1001) user      (1001)       30 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/radare2/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.922709 revenge-0.21/revenge/plugins/radare2/decompilers/
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/radare2/decompilers/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3721 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/radare2/decompilers/ghidra.py
--rw-rw-r--   0 user      (1001) user      (1001)     9336 2024-04-03 20:13:04.000000 revenge-0.21/revenge/plugins/radare2/radare2.py
--rw-rw-r--   0 user      (1001) user      (1001)    15536 2024-05-03 17:17:59.000000 revenge-0.21/revenge/process.py
--rw-rw-r--   0 user      (1001) user      (1001)     2439 2024-04-03 20:13:04.000000 revenge-0.21/revenge/symbols.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge/techniques/
--rw-rw-r--   0 user      (1001) user      (1001)     4073 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge/techniques/native_instruction_counter/
--rw-rw-r--   0 user      (1001) user      (1001)       87 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/native_instruction_counter/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     1136 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/native_instruction_counter/counter.py
--rw-rw-r--   0 user      (1001) user      (1001)     6251 2024-04-06 03:15:13.000000 revenge-0.21/revenge/techniques/native_instruction_counter/instruction_counter.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge/techniques/native_timeless_tracer/
--rw-rw-r--   0 user      (1001) user      (1001)      210 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/native_timeless_tracer/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3735 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/native_timeless_tracer/timeless_trace.py
--rw-rw-r--   0 user      (1001) user      (1001)     2456 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/native_timeless_tracer/timeless_trace_item.py
--rw-rw-r--   0 user      (1001) user      (1001)     2696 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/native_timeless_tracer/timeless_tracer.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge/techniques/tracer/
--rw-rw-r--   0 user      (1001) user      (1001)      129 2024-04-03 20:13:04.000000 revenge-0.21/revenge/techniques/tracer/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    13875 2024-05-03 17:17:59.000000 revenge-0.21/revenge/techniques/tracer/instruction_tracer.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge/threads/
--rw-rw-r--   0 user      (1001) user      (1001)      110 2024-04-03 20:13:04.000000 revenge-0.21/revenge/threads/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge/threads/create/
--rw-rw-r--   0 user      (1001) user      (1001)      447 2024-04-03 20:13:04.000000 revenge-0.21/revenge/threads/create/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     1269 2024-04-03 20:13:04.000000 revenge-0.21/revenge/threads/create/pthread.py
--rw-rw-r--   0 user      (1001) user      (1001)     5327 2024-04-03 20:13:04.000000 revenge-0.21/revenge/threads/thread.py
--rw-rw-r--   0 user      (1001) user      (1001)     6011 2024-04-03 20:13:04.000000 revenge-0.21/revenge/threads/threads.py
--rw-rw-r--   0 user      (1001) user      (1001)    18423 2024-04-03 20:13:04.000000 revenge-0.21/revenge/types.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-03 17:24:07.926709 revenge-0.21/revenge.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     1478 2024-05-03 17:24:07.000000 revenge-0.21/revenge.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     5551 2024-05-03 17:24:07.000000 revenge-0.21/revenge.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-05-03 17:24:07.000000 revenge-0.21/revenge.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2024-05-03 17:24:07.000000 revenge-0.21/revenge.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)      303 2024-05-03 17:24:07.000000 revenge-0.21/revenge.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        8 2024-05-03 17:24:07.000000 revenge-0.21/revenge.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-05-03 17:24:07.930709 revenge-0.21/setup.cfg
--rwxrwxr-x   0 user      (1001) user      (1001)     1764 2024-05-03 17:17:59.000000 revenge-0.21/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/
+-rwxrwxrwx   0 root         (0) root         (0)       88 2019-08-20 03:59:50.000000 revenge-0.9/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      598 2019-08-20 04:01:42.000000 revenge-0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    15642 2019-08-20 04:00:24.000000 revenge-0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/cli/
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/cli/actions/
+-rwxrwxrwx   0 root         (0) root         (0)     3463 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/actions/differential_find.py
+-rwxrwxrwx   0 root         (0) root         (0)     4524 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/actions/find.py
+-rwxrwxrwx   0 root         (0) root         (0)     2726 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/actions/stalker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4097 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/actions/windows_messages.py
+-rwxrwxrwx   0 root         (0) root         (0)      218 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/actions/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7234 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)        1 2019-08-20 03:59:50.000000 revenge-0.9/revenge/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3826 2019-08-20 03:59:50.000000 revenge-0.9/revenge/Colorer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/common/
+-rwxrwxrwx   0 root         (0) root         (0)    12124 2019-08-20 03:59:50.000000 revenge-0.9/revenge/common/windows_keys_by_id.json
+-rwxrwxrwx   0 root         (0) root         (0)    24925 2019-08-20 03:59:50.000000 revenge-0.9/revenge/common/windows_messages_by_id.json
+-rwxrwxrwx   0 root         (0) root         (0)    24204 2019-08-20 03:59:50.000000 revenge-0.9/revenge/common/windows_messages_by_name.json
+-rwxrwxrwx   0 root         (0) root         (0)     5758 2019-08-20 03:59:50.000000 revenge-0.9/revenge/common/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      252 2019-08-20 03:59:50.000000 revenge-0.9/revenge/config.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/contexts/
+-rwxrwxrwx   0 root         (0) root         (0)     8344 2019-08-20 03:59:50.000000 revenge-0.9/revenge/contexts/batch.py
+-rwxrwxrwx   0 root         (0) root         (0)       87 2019-08-20 03:59:50.000000 revenge-0.9/revenge/contexts/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/device_types/
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/device_types/android/
+-rwxrwxrwx   0 root         (0) root         (0)     7519 2019-08-20 03:59:50.000000 revenge-0.9/revenge/device_types/android/android.py
+-rwxrwxrwx   0 root         (0) root         (0)      966 2019-08-20 03:59:50.000000 revenge-0.9/revenge/device_types/android/applications.py
+-rwxrwxrwx   0 root         (0) root         (0)       36 2019-08-20 03:59:50.000000 revenge-0.9/revenge/device_types/android/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      519 2019-08-20 03:59:50.000000 revenge-0.9/revenge/device_types/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/java/
+-rwxrwxrwx   0 root         (0) root         (0)     1382 2019-08-20 03:59:50.000000 revenge-0.9/revenge/java/classes.py
+-rwxrwxrwx   0 root         (0) root         (0)     5036 2019-08-20 03:59:50.000000 revenge-0.9/revenge/java/java.py
+-rwxrwxrwx   0 root         (0) root         (0)    12924 2019-08-20 03:59:50.000000 revenge-0.9/revenge/java/java_class.py
+-rwxrwxrwx   0 root         (0) root         (0)      144 2019-08-20 03:59:50.000000 revenge-0.9/revenge/java/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/js/
+-rwxrwxrwx   0 root         (0) root         (0)      119 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/enumerate_modules.js
+-rwxrwxrwx   0 root         (0) root         (0)      164 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/enumerate_threads.js
+-rwxrwxrwx   0 root         (0) root         (0)     1787 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/find_in_memory.js
+-rwxrwxrwx   0 root         (0) root         (0)      633 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/generic_suspend_until_true.js
+-rwxrwxrwx   0 root         (0) root         (0)      252 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/get_declared_fields.js
+-rwxrwxrwx   0 root         (0) root         (0)      271 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/get_declared_methods.js
+-rwxrwxrwx   0 root         (0) root         (0)      278 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/pause_at.js
+-rwxrwxrwx   0 root         (0) root         (0)      179 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/pause_at2.js
+-rwxrwxrwx   0 root         (0) root         (0)      339 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/replace_function.js
+-rwxrwxrwx   0 root         (0) root         (0)      399 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/resolve_location_address.js
+-rwxrwxrwx   0 root         (0) root         (0)      572 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/rwx_everything.js
+-rwxrwxrwx   0 root         (0) root         (0)      351 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/rw_everything.js
+-rwxrwxrwx   0 root         (0) root         (0)     7814 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/stalk.js
+-rwxrwxrwx   0 root         (0) root         (0)      395 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/windows_intercept_message_handler.js
+-rwxrwxrwx   0 root         (0) root         (0)     3129 2019-08-20 03:59:50.000000 revenge-0.9/revenge/js/windows_stalk_message_handlers.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/memory/
+-rwxrwxrwx   0 root         (0) root         (0)     4661 2019-08-20 03:59:50.000000 revenge-0.9/revenge/memory/find.py
+-rwxrwxrwx   0 root         (0) root         (0)     1109 2019-08-20 03:59:50.000000 revenge-0.9/revenge/memory/map.py
+-rwxrwxrwx   0 root         (0) root         (0)     7304 2019-08-20 03:59:50.000000 revenge-0.9/revenge/memory/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)    16906 2019-08-20 03:59:50.000000 revenge-0.9/revenge/memory/memory_bytes.py
+-rwxrwxrwx   0 root         (0) root         (0)     2566 2019-08-20 03:59:50.000000 revenge-0.9/revenge/memory/memory_range.py
+-rwxrwxrwx   0 root         (0) root         (0)      213 2019-08-20 03:59:50.000000 revenge-0.9/revenge/memory/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/modules/
+-rwxrwxrwx   0 root         (0) root         (0)     7906 2019-08-20 03:59:50.000000 revenge-0.9/revenge/modules/module.py
+-rwxrwxrwx   0 root         (0) root         (0)     2964 2019-08-20 03:59:50.000000 revenge-0.9/revenge/modules/modules.py
+-rwxrwxrwx   0 root         (0) root         (0)      110 2019-08-20 03:59:50.000000 revenge-0.9/revenge/modules/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4397 2019-08-20 03:59:50.000000 revenge-0.9/revenge/native_exception.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/parsers/
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/parsers/elf/
+-rwxrwxrwx   0 root         (0) root         (0)     4589 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/elf/elf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2067 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/elf/program_header.py
+-rwxrwxrwx   0 root         (0) root         (0)     1048 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/elf/program_headers.py
+-rwxrwxrwx   0 root         (0) root         (0)     1349 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/elf/section_header.py
+-rwxrwxrwx   0 root         (0) root         (0)     1208 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/elf/section_headers.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/elf/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2019-08-20 03:59:50.000000 revenge-0.9/revenge/parsers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    19982 2019-08-20 03:59:50.000000 revenge-0.9/revenge/process.py
+-rwxrwxrwx   0 root         (0) root         (0)     2979 2019-08-20 03:59:50.000000 revenge-0.9/revenge/threads.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/tracer/
+-rwxrwxrwx   0 root         (0) root         (0)     4294 2019-08-20 03:59:50.000000 revenge-0.9/revenge/tracer/assembly_instruction.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge/tracer/contexts/
+-rwxrwxrwx   0 root         (0) root         (0)     3190 2019-08-20 03:59:51.000000 revenge-0.9/revenge/tracer/contexts/x64.py
+-rwxrwxrwx   0 root         (0) root         (0)     1872 2019-08-20 03:59:51.000000 revenge-0.9/revenge/tracer/contexts/x86.py
+-rwxrwxrwx   0 root         (0) root         (0)      567 2019-08-20 03:59:51.000000 revenge-0.9/revenge/tracer/contexts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10962 2019-08-20 03:59:51.000000 revenge-0.9/revenge/tracer/instruction_tracer.py
+-rwxrwxrwx   0 root         (0) root         (0)      512 2019-08-20 03:59:51.000000 revenge-0.9/revenge/tracer/tracer.py
+-rwxrwxrwx   0 root         (0) root         (0)      185 2019-08-20 03:59:50.000000 revenge-0.9/revenge/tracer/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3331 2019-08-20 03:59:51.000000 revenge-0.9/revenge/types.py
+-rwxrwxrwx   0 root         (0) root         (0)      192 2019-08-20 03:59:50.000000 revenge-0.9/revenge/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       50 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      598 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      242 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2235 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2019-08-20 04:01:41.000000 revenge-0.9/revenge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2019-08-20 04:01:42.000000 revenge-0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1623 2019-08-20 03:59:51.000000 revenge-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `revenge-0.21/revenge/Colorer.py` & `revenge-0.9/revenge/Colorer.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/cli/actions/differential_find.py` & `revenge-0.9/revenge/cli/actions/differential_find.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/cli/actions/find.py` & `revenge-0.9/revenge/cli/actions/find.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/cli/actions/stalker.py` & `revenge-0.9/revenge/cli/actions/stalker.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,38 +56,28 @@
 
     def run(self):
         self.action_stalk()
 
     def action_stalk(self):
         """Start the stalker."""
 
-        done = []
-
         def stalk_cb(tid, ti):
             print(ti)
-
-        def on_done(msg, x):
-            done.append(True)
         
-        trace = self._process.techniques.NativeInstructionTracer(
+        trace = self._process.tracer.instructions(
+                threads = self.tid,
                 from_modules = self.from_modules,
                 call = self.call,
                 ret = self.ret,
                 exec = self.exec,
                 block = self.block,
                 compile = self.compile,
                 callback = stalk_cb,
                 )
 
-        trace.apply(self.tid)
-
-        # Figure out when we're done...
-        for bp in ['exit', '_exit']:
-            bp = self._process.memory[bp]
-            bp.breakpoint = False
-            bp.replace_on_message = on_done
-            bp.replace = "function () { send('here'); Thread.sleep(0.5) ; }"
+        # Make sure we're not blocking
+        for addr in list(self._process.memory._active_breakpoints):
+            self._process.memory[addr].breakpoint = False
 
-        self._process.memory[self._process.entrypoint].breakpoint = False
+        while self._process.alive:
+            sleep(0.1)
 
-        # Wait til done
-        while done == []: continue
```

### Comparing `revenge-0.21/revenge/cli/actions/windows_messages.py` & `revenge-0.9/revenge/cli/actions/windows_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
         self._known_windows_message_handlers = []
 
         def windows_cb(message, data):
             # REMINDER: The JavaScript is filtering out dups. We will only be getting each handler once.
 
             handler_ip = int(message['payload'], 16)
-            handler_module = self._process.modules[handler_ip]
-            if handler_module is not None: handler_module = handler_module.name
+            handler_module = self._process.get_module_by_addr(handler_ip)
             handler_offset = handler_ip - self._process.modules[handler_module]['base']
 
             self._known_windows_message_handlers.append(handler_ip)
 
             # Allow downselection to this module
             if self.include_module == [] or handler_module in self.include_module:
                 print("{: <32}".format("Found Message Handler") + colored(handler_module, 'cyan') + ":" + colorama.Style.BRIGHT + colored(hex(handler_offset), "cyan"))
```

### Comparing `revenge-0.21/revenge/cli/cli.py` & `revenge-0.9/revenge/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,31 +99,31 @@
     return args
 
 def replace_function(process, f):
     """Replace a given function to always return a given value. <module:offset|symbol>?<return_val>"""
     assert type(f) == str, "Unexpected replace function argument type of {}".format(type(f))
 
     location, return_value = f.split("?")
-    replace_location = process.modules.lookup_symbol(location)
+    replace_location = process._resolve_location_string(location)
 
     replace_vars = {
             "FUNCTION_RETURN_VALUE_HERE": return_value,
             "FUNCTION_ADDRESS_HERE": hex(replace_location),
             }
 
-    self.engine.run_script_generic("replace_function.js", replace=replace_vars)
+    self.run_script_generic("replace_function.js", replace=replace_vars)
 
 def main():
     args = parse_args()
 
     process = Process(args.target, resume=args.resume, verbose=args.verbose)
 
     if args.rw_everything:
         print("RW'ing memory areas\t\t... ", end='', flush=True)
-        process.engine.run_script_generic('rw_everything.js', unload=True)
+        process.run_script_generic('rw_everything.js', unload=True)
         cprint('[ DONE ]', 'green')
 
 
     for f in args.replace_function:
         location, return_value = f.split("?")
         mem = process.memory[location]
         mem.replace = int(return_value, 0)
```

### Comparing `revenge-0.21/revenge/common/windows_keys_by_id.json` & `revenge-0.9/revenge/common/windows_keys_by_id.json`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/common/windows_messages_by_id.json` & `revenge-0.9/revenge/common/windows_messages_by_id.json`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/common/windows_messages_by_name.json` & `revenge-0.9/revenge/common/windows_messages_by_name.json`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/contexts/batch.py` & `revenge-0.9/revenge/contexts/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 }}
 
 function flush () {{
     var message = {{
         'return_buffer': return_buffer
     }}
     send(message);
-    // recv('flush', flush);
+    recv('flush', flush);
 }}
 
 function handler (args) {{
     {handler_pre}
 
     args['list'].forEach( function (item) {{
         buffer_return([item, eval(item)]);
@@ -48,34 +48,33 @@
     await sleep(60000);
 }}
 
 function generic_handler(args) {{
     if ( args['type'] == "list" ) {{
         handler(args);
     }}
+    else if ( args['type'] == "flush" ) {{
+        flush();
+    }}
 }}
 
 var recv_list = recv('list', handler);
-//var recv_flush = recv('flush', flush);
+var recv_flush = recv('flush', flush);
 
 // Setting up blocking recv-loop
 // Blocking is sadly needed due to Java implementation...
 
 /*
 var receiver = recv(generic_handler)
 while ( 1 ) {{
     receiver.wait()
     receiver = recv(generic_handler)
 }}
 */
 
-rpc.exports = {{
-    dispose: function () {{ flush(); }},
-    flush: function () {{ flush(); }},
-}}
 
 """
 
 class BatchContext(object):
     def __init__(self, process, send_buffer_size=None, return_buffer_size=None,
             on_message=None, run_script_generic=None, handler_pre=None,
             handler_post=None):
@@ -94,49 +93,48 @@
                 to use for calling? (default: process.run_script_generic)
             handler_pre (str, optional): Something to optionally run before
                 iterating over the strings provided.
             handler_post (str, optional): Something to optionally run after
                 iterating over the strings provided.
 
         Example:
-            .. code-block:: python3
+            with process.BatchContext():
+                for i in range(255):
+                    do_something
 
-                with process.BatchContext():
-                    for i in range(255):
-                        do_something
 
         This Context will simply queue up a bunch of strings, which will be fed
         into the thread and executed sequentially.
         """
 
         self._process = process
         # Queue of things to send
         self.queue = []
         self.send_buffer_size = send_buffer_size or 1024
         self.return_buffer_size = return_buffer_size or 1024
         self.on_message = on_message
         self._script = None
-        self._proxy_run_script_generic = run_script_generic or self._process.engine.run_script_generic
+        self._proxy_run_script_generic = run_script_generic or self._process.run_script_generic
         self._handler_pre = handler_pre or ""
         self._handler_post = handler_post or ""
 
         # How many things do we think the js side is still chewing on rn?
         self._num_pending_complete = 0
 
     def run_script_generic(self, script):
         """Handle calls to the run script generic.
 
         Args:
             script (str): This is the script that will be evaluated by js.
         
-        This should be called from Process.engine.run_script_generic since that will
+        This should be called from Process.run_script_generic since that will
         take care of the pre-processing for this.
 
         IF YOU CALL THIS DIRECTLY, IT'S ON YOU TO MAKE SURE THINGS ARE
-        FORMATTED CORRECTLY! USE Process.engine.run_script_generic INSTEAD!
+        FORMATTED CORRECTLY! USE Process.run_script_generic INSTEAD!
         """
 
         # Process.run_script_generic gets called with this context
         # The script gets resolved and created in full by the run_script_generic
         # method. It then call this. When we're ready to run, we call
         # run_script_generic with NO context, but arguments will be for us.
 
@@ -156,16 +154,15 @@
     def _flush_recieve(self):
         """Force a flush of the receiving buffer back to python."""
 
         if self._script is None:
             logger.error("Cannot find script to tell to flush!")
             return
 
-        #self._script[0].post({"type": "flush"})
-        self._script[0].exports.flush()
+        self._script[0].post({"type": "flush"})
 
     def _send_buffer(self):
         """Handles sending and emptying the buffer.
 
         This assumes that size checks have already been done."""
 
         if self._script is None:
@@ -230,15 +227,15 @@
                 raw=True,
                 unload=False,
                 runtime='v8',
                 timeout=0,
                 on_message=self._context_on_message,
                 )
 
-        self._script = self._process.engine._scripts.pop(0)
+        self._script = self._process._scripts.pop(0)
 
     def _unload_script(self):
         # TODO: This might be called before we're done processing...
         if self._script is None:
             return
 
         self._script[0].unload()
@@ -262,16 +259,15 @@
         while self._num_pending_complete != 0:
             self._flush_recieve()
             sleep(0.1)
 
         # TODO: There's a race condition here where the Frida js has finished
         # processing the things we've sent, but has not finished flushing data
         # back. Sleeping for now, but find a better way...
-        # This should be fixed with the rpc dispose call now...
-        #sleep(0.2)
+        sleep(0.2)
 
         # Done with this script.
         self._unload_script()
 
     def __del__(self):
         self._unload_script()
```

### Comparing `revenge-0.21/revenge/cpu/assembly/instruction.py` & `revenge-0.9/revenge/tracer/assembly_instruction.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
-import re
 from termcolor import cprint, colored
+import re
+
 from prettytable import PrettyTable
 
+from .. import types, common
+
 class AssemblyBlock(object):
     """Represents an assembly block."""
 
     def __init__(self, process, address):
         self._process = process
         self.instructions = []
         self.address = address
@@ -41,75 +44,59 @@
         attrs = ['AssemblyBlock', str(len(self.instructions)), 'instructions']
         return '<' + ' '.join(attrs) + '>'
 
 
 class AssemblyInstruction(object):
     """Represents an assembly instruction."""
 
-    def __init__(self, process, address=None):
+    def __init__(self, process, address):
         """
 
         Args:
             process: Process object
-            address (int, optional): Address for this instruction. Will load
-                from this address.
+            address (int): Address for this instruction. Will load from this address.
         """
 
         self._process = process
         self.address = address
 
-    @classmethod
-    def from_frida_dict(klass, process, d):
-        """Builds this assembly instruction from a frida dictionary, ala Instruction.parse()"""
-        instruction = klass(process)
-        instruction._parse_instruction(d)
-        return instruction
-
-    def _parse_instruction(self, inst):
-        """Given an instruction dict as returned from Frida, parse it into this object."""
+    def _load_from_address(self):
+        inst = self._process.run_script_generic("""send(Instruction.parse({}));""".format(self.address.js), raw=True, unload=True)[0][0]
 
-        self.__address = types.Pointer(common.auto_int(inst['address']))
         self.__address_next = types.Pointer(common.auto_int(inst['next']))
         self.__size = inst['size']
         self.__mnemonic = inst['mnemonic']
         self.__args_str = inst['opStr']
         self.__operands = inst['operands']
         self.__registers_read = inst['regsRead']
         self.__registers_written = inst['regsWritten']
         self.__groups = inst['groups']
 
-    def _load_from_address(self):
-        inst = self._process.engine.run_script_generic("""send(Instruction.parse({}));""".format(self.address.js), raw=True, unload=True)[0][0]
-        self._parse_instruction(inst)
-
     def __str__(self):
         return "{address} {mnemonic: <20}{args}".format(
                     address=colored(hex(self.address), attrs=['bold']) + ":",
                     mnemonic=colored(self.mnemonic, "cyan"),
                     args=colored(self.args_str_resolved, "cyan", attrs=['bold']),
                 )
 
     def __repr__(self):
         attrs = ['AssemblyInstruction', hex(self.address), self.mnemonic, self.args_str]
         return '<' + ' '.join(attrs) + '>'
 
-    def __hash__(self):
-        return hash((self.address, self.args_str))
-
     @property
     def args_str_resolved(self):
         """str: Attempt to resolve addresses in the args str into symbols."""
         s = self.args_str
         
         things = re.findall('0x[0-9a-f]+', s)
         
         for thing in things:
             sym = self._process.modules.lookup_symbol(int(thing,16))
             if sym is not None:
-                s = s.replace(thing, str(sym))
+                s = s.replace(thing, sym)
 
         return s
 
     @property
     def groups(self):
         """list: List of descriptive groups that this instruction belongs to."""
         return self.__groups
@@ -152,14 +139,9 @@
     @property
     def address(self):
         """Pointer: Address where this instruction is located."""
         return self.__address
 
     @address.setter
     def address(self, address):
-        if address is None:
-            self.__address = None
-            return
         self.__address = types.Pointer(common.auto_int(address))
         self._load_from_address()
-
-from ... import types, common
```

### Comparing `revenge-0.21/revenge/cpu/contexts/__init__.py` & `revenge-0.9/revenge/threads.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,106 @@
 
 import logging
-
 logger = logging.getLogger(__name__)
 
-import colorama
+from prettytable import PrettyTable
 
-class CPUContextBase(object):
+from . import common
 
-    __slots__ = ['_process', 'pc', 'sp', '__changed_registers']
+class Thread(object):
 
-    def __init__(self, process, diff=None, **registers):
-        """Represents a CPU context.
-        
-        Args:
-            diff (CPUContext, optional): Build this context as a diff from a
-                previous context
+    def __init__(self, process, info):
+        self._process = process
+        self._info = info
+        self.context = Context(self._process, **self._info['context'])
 
-        Example:
-            CPUContext(process, rax=12, rbx=13, <etc>)
-        """
+    def __repr__(self):
+        attrs = ['Thread', hex(self.id), '@', hex(self.pc), self.state, self.module]
+        if self.trace is not None:
+            attrs.append('tracing')
+        return "<{}>".format(' '.join(attrs))
 
-        self._process = process
-        self.__changed_registers = []
+    def __getattr__(self, elm):
+        return common.auto_int(self._info['context'][elm])
 
-        if not isinstance(diff, (type(None), self.__class__)):
-            raise RevengeInvalidArgumentType("diff must be either None or an instance of {}".format(self.__class__))
+    def __str__(self):
 
-        # Copy over old diff first if need be
-        if diff is not None:
-            for reg in self.REGS:
-                setattr(self, reg, getattr(diff, reg))
+        table = PrettyTable(['attr', 'value'])
 
-        # Generically set any registers we're given
-        for key, val in registers.items():
+        table.add_row(['TID', str(self.id)])
+        table.add_row(["State", self.state])
+        table.add_row(["Module", self.module])
+        table.add_row(["Tracing?", "Yes" if self.trace is not None else "No"])
 
-            if diff:
-                self.changed_registers.append(key)
+        """
+        for reg in self._info['context']:
+            table.add_row([reg, hex(getattr(self, reg))])
+        
+        """
+        table.header = False
+        table.align = "l"
 
-            # If dict, assume it's telescope for now
-            if isinstance(val, dict):
-                setattr(self, key, types.Telescope(self._process, data=val))
-            else:
-                setattr(self, key, common.auto_int(val))
+        return str(table) + '\n' + str(self.context)
 
-    @property
-    def changed_registers(self):
-        """list: What registers were changed with this step?"""
-        return self.__changed_registers
 
-    def __getattr__(self, attr):
-        return eval(self.REGS_ALL[attr])
+    @property
+    def id(self):
+        return self._info['id']
 
-    def __str__(self):
-        table = PrettyTable(["Register", "Value"])
+    @property
+    def state(self):
+        return self._info['state']
 
-        table.align = 'l'
+    @property
+    def pc(self):
+        return int(self._info['context']['pc'],16)
 
-        for reg in self.REGS:
+    @property
+    def module(self):
+        return self._process.get_module_by_addr(self.pc) or "Unknown"
+    
+    @property
+    def trace(self):
+        """Trace or None: Returns Trace object if this thread is currently being traced, otherwise None."""
+        if self.id in self._process.tracer._active_instruction_traces:
+            return self._process.tracer._active_instruction_traces[self.id]
 
-            # Highlight changed registers
-            if reg in self.changed_registers:
-                reg_colored = colorama.Fore.YELLOW + reg + colorama.Style.RESET_ALL
-            else:
-                reg_colored = reg
 
-            thing = getattr(self, reg)
-            
-            if isinstance(thing, types.Telescope):
-                table.add_row([reg_colored, thing.description])
+class Threads(object):
 
-            else:
-                table.add_row([reg_colored, hex(getattr(self, reg))])
+    def __init__(self, process):
+        self._process = process
 
-        return str(table)
+    def __len__(self):
+        return len(self.threads)
 
-    def __hash__(self):
-        # Don't hash as a generator!
-        return hash(tuple(getattr(self, reg) for reg in self.REGS))
+    def __iter__(self):
+        return iter(self.threads)
 
+    def __repr__(self):
+        return "<{} {}>".format(len(self), "Thread" if len(self) == 1 else "Threads")
 
-class CPUContext(object):
-    
-    def __new__(klass, process, *args, **kwargs):
-        """Represents a CPU for this running process."""
+    def __str__(self):
+        table = PrettyTable(['id', 'state', 'pc', 'module', 'Trace'])
 
-        arch = process.arch
+        for thread in self:
+            table.add_row([str(thread.id), thread.state, hex(thread.pc), thread.module, 'Yes' if thread.trace is not None else 'No'])
 
-        if arch == "x64":
-            return X64Context(process, *args, **kwargs)
+        return str(table)
 
-        elif arch == "ia32":
-            return X86Context(process, *args, **kwargs)
+    def __getitem__(self, elm):
 
-        elif arch == "arm":
-            return ARMContext(process, *args, **kwargs)
+        if type(elm) is int:
+            try:
+                return next(thread for thread in self.threads if thread.id == elm)
+            except StopIteration:
+                logger.error("Invalid thread id selected.")
 
         else:
-            logger.error("Currently unsupported architecture of {}".format(arch))
+            logger.error("Not sure how to handle this.")
 
-from prettytable import PrettyTable
-from .x64 import X64Context
-from .x86 import X86Context
-from .arm import ARMContext
-from ... import types, common
+    @property
+    def threads(self):
+        threads = self._process.run_script_generic("""send(Process.enumerateThreadsSync());""", raw=True, unload=True)[0][0]
+        return [Thread(self._process, thread) for thread in threads]
+
+from .tracer.contexts import Context
```

### Comparing `revenge-0.21/revenge/cpu/contexts/x86.py` & `revenge-0.9/revenge/tracer/contexts/x86.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,71 @@
 import logging
 logger = logging.getLogger(__name__)
 
-from . import CPUContextBase
+from termcolor import cprint, colored
+from prettytable import PrettyTable
 
-class X86Context(CPUContextBase):
+from ... import types, common
 
-    REGS = ['eip', 'esp', 'ebp', 'eax', 'ebx', 'ecx', 'edx', 'esi', 'edi']
-    REGS_ALL = {
-        'sp'  : 'self.esp',
-        'bp'  : 'self.ebp',
-        'ip'  : 'self.eip',
-        'eax' : 'self.eax',
-        'ax'  : 'self.eax & 0xffff',
-        'al'  : 'self.eax & 0xff',
-        'ah'  : '(self.eax>>8) & 0xff',
-        'ebx' : 'self.ebx',
-        'bx'  : 'self.ebx & 0xffff',
-        'bl'  : 'self.ebx & 0xff',
-        'bh'  : '(self.ebx>>8) & 0xff',
-        'ecx' : 'self.ecx',
-        'cx'  : 'self.ecx & 0xffff',
-        'cl'  : 'self.ecx & 0xff',
-        'ch'  : '(self.ecx>>8) & 0xff',
-        'edx' : 'self.edx',
-        'dx'  : 'self.edx & 0xffff',
-        'dl'  : 'self.edx & 0xff',
-        'dh'  : '(self.edx>>8) & 0xff',
-        'esi' : 'self.esi',
-        'si'  : 'self.esi & 0xffff',
-        'sil' : 'self.esi & 0xff',
-        'edi' : 'self.edi',
-        'di'  : 'self.edi & 0xffff',
-        'dil' : 'self.edi & 0xff',
-        'ebp' : 'self.ebp',
-        'bp'  : 'self.ebp & 0xffff',
-        'bpl' : 'self.ebp & 0xff',
-        'esp' : 'self.esp',
-        'sp'  : 'self.esp & 0xffff',
-        'spl' : 'self.esp & 0xff',
-        'eip' : 'self.eip',
-    }
+x64_regs = {
+    'sp'  : 'self.esp',
+    'bp'  : 'self.ebp',
+    'ip'  : 'self.eip',
+    'eax' : 'self.eax',
+    'ax'  : 'self.eax & 0xffff',
+    'al'  : 'self.eax & 0xff',
+    'ah'  : '(self.eax>>8) & 0xff',
+    'ebx' : 'self.ebx',
+    'bx'  : 'self.ebx & 0xffff',
+    'bl'  : 'self.ebx & 0xff',
+    'bh'  : '(self.ebx>>8) & 0xff',
+    'ecx' : 'self.ecx',
+    'cx'  : 'self.ecx & 0xffff',
+    'cl'  : 'self.ecx & 0xff',
+    'ch'  : '(self.ecx>>8) & 0xff',
+    'edx' : 'self.edx',
+    'dx'  : 'self.edx & 0xffff',
+    'dl'  : 'self.edx & 0xff',
+    'dh'  : '(self.edx>>8) & 0xff',
+    'esi' : 'self.esi',
+    'si'  : 'self.esi & 0xffff',
+    'sil' : 'self.esi & 0xff',
+    'edi' : 'self.edi',
+    'di'  : 'self.edi & 0xffff',
+    'dil' : 'self.edi & 0xff',
+    'ebp' : 'self.ebp',
+    'bp'  : 'self.ebp & 0xffff',
+    'bpl' : 'self.ebp & 0xff',
+    'esp' : 'self.esp',
+    'sp'  : 'self.esp & 0xffff',
+    'spl' : 'self.esp & 0xff',
+    'eip' : 'self.eip',
+}
 
-    __slots__ = REGS
+class X86Context(object):
 
+    def __init__(self, process, **registers):
+        """Represents a x86 CPU context.
+
+        Example:
+            X86Context(process, eax=12, ebx=13, <etc>)
+        """
+
+        self._process = process
+
+        # Generically set any registers we're given
+        for key, val in registers.items():
+            setattr(self, key, common.auto_int(val))
+
+    def __getattr__(self, attr):
+        return eval(x64_regs[attr])
+
+    def __str__(self):
+        table = PrettyTable(["Register", "Value"])
+        main_regs = ['eip', 'esp', 'ebp', 'eax', 'ebx', 'ecx', 'edx', 'esi', 'edi']
+
+        table.align = 'l'
+
+        for reg in main_regs:
+            table.add_row([reg, hex(getattr(self, reg))])
+
+        return str(table)
```

### Comparing `revenge-0.21/revenge/devices/android/android.py` & `revenge-0.9/revenge/device_types/android/android.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 import frida
 import shlex
 import os
 import subprocess
 from time import sleep
 
 from .. import BaseDevice
-from ... import common
 
 class AndroidDevice(BaseDevice):
-    def __init__(self, engine=None, id=None, type=None, frida_server_release=None):
+    def __init__(self, id=None, type=None, frida_server_release=None):
         """Describes and Android device.
 
         Args:
-            engine (str, optional): What Engine to use? Default: frida
             id (str, optional): Unique ID for this android device
             type (str, optional): Connection type for this device.
             frida_server_release (str, optional): Specify a specific version
                 i.e.: 12.6.11 -- default is latest
 
         Examples:
             AndroidDevice(id="emulator-5554")
             AndroidDevice(type="usb")
         """
-
-        self._engine = engine or 'frida'
         self.id = id
         self._frida_server_release = frida_server_release
         self.type = type.lower()
         self._select_device()
 
         # Make sure we can have root
         self.adb("root")
@@ -104,15 +100,14 @@
         return subprocess.call(["adb", "-s", self.device.id] + command)
 
     def shell(self):
         """Spawn and interact with a shell on the device."""
         self.adb("shell", interactive=True)
 
 
-    @common.retry_on_exception((frida.TransportError,frida.ProcessNotFoundError))
     def spawn(self, application, gated=True, load_symbols=None):
         """Spawn the given application.
 
         Args:
             application (str): Full application name (i.e.: com.android.calculator2)
             gated (bool, optional): If True, pause application immediately on loading
                 This allows hooking prior to program startup.
@@ -134,37 +129,34 @@
         application = application.identifier
         pid = self.device.spawn(application)
 
         if not gated:
             # Sometimes it gates anyway
             self.device.resume(pid)
 
-        return Engine._from_string(self._engine, device=self).Process(pid, load_symbols=load_symbols)
+        return Process(pid, device=self, load_symbols=load_symbols)
 
-    @common.retry_on_exception((frida.TransportError,))
     def attach(self, application, load_symbols=None):
         """Attach to the given application.
 
         Args:
             application (str): Full application name (i.e.: com.android.calculator2) or pid
             load_symbols (list): Only load symbols for the given modules. Same
                 usage as revenge.Process
 
         Returns:
             revenge.Process: Process instantitation for this new process.
         """
         
         if isinstance(application, frida._frida.Application):
             pid = application.pid
-        elif isinstance(application, int):
-            pid = application
         else:
             pid = self.applications[application].pid
 
-        return Engine._from_string(self._engine, device=self).Process(pid, load_symbols=load_symbols)
+        return Process(pid, device=self, load_symbols=load_symbols)
 
     def install(self, package):
         """Install package onto android device.
 
         Args:
             package (str): Path to package to install.
         """
@@ -172,15 +164,15 @@
         package = os.path.abspath(package)
 
         if not os.path.isfile(package):
             logger.error("Cannot find apk to install.")
             return False
 
         # Allow replace by default
-        return self.adb("install -t -r " + package)
+        return self.adb("install -r " + package)
 
     def uninstall(self, application):
         """Uninstall the given application.
         
         Args:
             application (str): Application to uninstall
 
@@ -202,15 +194,15 @@
         return AndroidApplications(self)
 
     @property
     def frida_server_running(self):
         try:
             self.device.enumerate_applications()
             return True
-        except (frida.ServerNotRunningError, frida.InvalidOperationError, frida.ProcessNotFoundError, frida.TransportError):
+        except (frida.ServerNotRunningError, frida.InvalidOperationError):
             return False
 
     @property
     def arch(self):
         """Returns the arch of this android device."""
         try:
             return self.__arch
@@ -232,15 +224,12 @@
         try:
             return self.__version
         except AttributeError:
             p = self.attach(self.device.get_frontmost_application(), load_symbols=[])
             self.__version = p.java.run_script_generic("send(Java.androidVersion)", raw=True, unload=True)[0][0]
             return self.__version
 
-    @property
-    def platform(self):
-        return "linux"
-
 from .applications import AndroidApplications
+from ... import common
 from .. import uname_standard
-from ...engines import Engine
+from ...process import Process
```

### Comparing `revenge-0.21/revenge/devices/android/applications.py` & `revenge-0.9/revenge/device_types/android/applications.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/engines/frida/plugins/java/java.py` & `revenge-0.9/revenge/java/java.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 
 import logging
-LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 import collections
-from .....plugins.java import Java
 
-class FridaJava(Java):
+class Java:
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, process):
         """Handles performing Java related activities."""
-        super().__init__(*args, **kwargs)
-
-        self._JavaClasses = JavaClasses
+        self._process = process
+        
+        # Key = Full path to method that was implemented, Value = str that we implemented with.
+        self._implementations = {}
+
+        # Key: class name, vlaue = list of handles to active objects in memory
+        self._active_handles = collections.defaultdict(lambda: list())
+
+        # Key: Full class name, value = list of dict of reflected info
+        self._cache_reflected_methods = collections.defaultdict(lambda: list())
+        self._cache_reflected_fields = collections.defaultdict(lambda: list())
     
     def run_script_generic(self, script_name, raw=False, main_thread=False, *args, **kwargs):
         """Run the given Java related Frida calls. Simply wraps them in the perform call...
 
         Java Specific:
         Args:
             main_thread (bool, optional): Run this on the main Java thread.
 
-        Calls the Process.engine.run_script_generic as below:
+        Calls the Process.run_script_generic as below:
         """
 
         context = kwargs.get("context", None)
 
         if not raw:
-            script = self._process.engine.load_js(script_name)
+            script = self._process.load_js(script_name)
         else:
             # NOTE: This is meant to transparently convert the java_class and
             # others into the corresponding code. Do not remove str call!
             script = str(script_name)
 
         # If we're outside a context, do the full setup
         if context is None:
@@ -41,53 +48,67 @@
                 script = "Java.scheduleOnMainThread( function () { " + script + "});"
 
             # Wrap up the java call
             script = "Java.perform( function () {" + script + "});"
 
         #kwargs['timeout'] = None
 
-        return self._process.engine.run_script_generic(script, raw=True, *args, **kwargs)
+        return self._process.run_script_generic(script, raw=True, *args, **kwargs)
 
     def find_active_instance(self, klass, invalidate_cache=False):
+        """Look through memory and finds an active instance of the given klass.
+
+        Args:
+            klass (str, JavaClass): The class we want to find already in memory.
+            invalidate_cache (bool, optional): Throw away any current cache.
+                This should normally not be needed.
+
+        Returns:
+            Returns JavaClass instance with approrpiate handle server. This
+            means you can use the object without instantiating it yourself.
+
+        Example:
+            MainActivity = p.java.find_active_class("ooo.defcon2019.quals.veryandroidoso.MainActivity")
+            MainActivity.parse("test")
+        """
 
         if isinstance(klass, JavaClass):
             klass_name = klass._name
             
         elif isinstance(klass, str):
             klass_name = klass
 
         else:
-            LOGGER.error("Invalid klass type of {}".format(type(klass)))
+            logger.error("Invalid klass type of {}".format(type(klass)))
             return
 
+        logger.warn("There's currently a bug in this from frida server version 12.6.12 - current. If this fails to work for you, install server version 12.6.11 via android = revenge.device_types.AndroidDevice(type='usb', frida_server_release='12.6.11')")
+
         if invalidate_cache:
             self._active_handles[klass_name] = []
 
         # Attempt to enumerate active handles if we don't know of any.
         if self._active_handles[klass_name] == []:
-            self._active_handles[klass_name] = self.run_script_generic("var my_list = []; Java.choose('{}', {{onMatch: function (i) {{my_list.push(i); send(i.$h);}}, onComplete: function () {{send('DONE');}}}})".format(klass_name), raw=True, unload=False,onComplete='DONE')[0]
+            self._active_handles[klass_name] = self.run_script_generic("var my_list = []; Java.choose('{}', {{onMatch: function (i) {{my_list.push(i); send(i);}}, onComplete: function () {{send('DONE');}}}})".format(klass_name), raw=True, unload=False,onComplete='DONE')[0]
 
         # If we can't find any instances
         # TODO: Clean-up script if we don't find anything..
         if self._active_handles[klass_name] == []:
-            LOGGER.warn("Couldn't find any active instances of {}!".format(klass_name))
+            logger.warn("Couldn't find any active instances of {}!".format(klass_name))
             return
 
         # Build new instance
-        handle = common.auto_int(self._active_handles[klass_name][0])
+        handle = common.auto_int(self._active_handles[klass_name][0]['$handle'])
         klass = JavaClass(self._process, klass_name, handle=handle)
         return klass
 
     @property
-    def _is_valid(self):
-        try:
-            return self.__is_valid
-        except AttributeError:
-            self.__is_valid = self._process.engine.run_script_generic(r"""send(Java.available)""", raw=True, unload=True)[0][0]
-            return self.__is_valid
+    def classes(self):
+        """JavaClasses: Returns java classes object."""
+        return JavaClasses(self._process)
 
     @property
     def BatchContext(self):
         """Returns a BatchContext class for this jvm.
 
         Example:
             with process.java.BatchContext() as context:
@@ -97,16 +118,16 @@
         """
         return lambda **kwargs: BatchContext(self._process,
                 run_script_generic=self.run_script_generic, 
                 handler_pre = "Java.perform(function () {",
                 handler_post = "});",
                 **kwargs)
 
-from .classes import FridaJavaClasses as JavaClasses
-from .java_class import FridaJavaClass as JavaClass
-from .....engines.frida import FridaEngine
-from .....contexts.batch import BatchContext
-from ..... import common
+from .classes import JavaClasses
+from .java_class import JavaClass
+from ..process import Process
+from ..contexts.batch import BatchContext
+from .. import common
 
 # Fixup docs
-FridaJava.run_script_generic.__doc__ += FridaEngine.run_script_generic.__doc__
-FridaJava.BatchContext.__doc__ += BatchContext.__init__.__doc__
+Java.run_script_generic.__doc__ += Process.run_script_generic.__doc__
+Java.BatchContext.__doc__ += BatchContext.__init__.__doc__
```

### Comparing `revenge-0.21/revenge/engines/frida/plugins/java/java_class.py` & `revenge-0.9/revenge/java/java_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 import logging
-LOGGER = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
-from .....plugins.java import JavaClass
-
-class FridaJavaClass(JavaClass):
+class JavaClass(object):
     _in_init = set()
 
     def __init__(self, process, name=None, prefix=None, handle=None,
             full_description=None, is_method=None, is_field=None,
             implementation_message=None):
         """Represents a Java class.
 
@@ -344,15 +342,15 @@
             raw=True,
             unload=False,
             runtime='v8',
             on_message=self._implementation_message,
             )
         
         # Save it off
-        self._process.java._implementations[str(self)] = [implementation] + self._process.engine._scripts.pop(0)
+        self._process.java._implementations[str(self)] = [implementation] + self._process._scripts.pop(0)
 
     @property
     def _implementation_message(self):
         """callable: Something to get called when 'send' messages are received from implementation."""
         return self.__implemenetation_message
 
     @_implementation_message.setter
@@ -367,10 +365,10 @@
 
 
     @staticmethod
     def _is_safe_method_name(name):
         safe = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_'
         return all(char in safe for char in name)
 
-from ..... import config, common
 
-JavaClass = FridaJavaClass
+from .. import config
+from .. import common
```

### Comparing `revenge-0.21/revenge/engines/frida/process.py` & `revenge-0.9/revenge/modules/module.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,221 +1,267 @@
 
 import logging
+logger = logging.getLogger(__name__)
 
-import frida
+from elftools.elf.elffile import ELFFile
+from termcolor import cprint, colored
+import itertools
+import hashlib
+import os
+import io
+import json
+from fnmatch import fnmatch
+import pefile
 
-from ...process import Process as ProcessBase
-from revenge import common
-from revenge.exceptions import *
+from .. import common, types, config
 
+symbol_cache_path = os.path.join(config.app_dirs.user_cache_dir, 'symbol_cache')
+os.makedirs(symbol_cache_path, exist_ok=True)
 
-class Process(ProcessBase):
+class Module(object):
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, process, name, base, size, path):
+        self._process = process
+        self.name = name
+        self.base = base
+        self.size = size
 
-        self.__frida_process_general_init()
+        self.path = path # Must go last
 
-        if self.device.platform == "linux":
-            self.__frida_process_linux_init()
-        elif self.device.platform == "windows":
-            self.__frida_process_windows_init()
+    def _read_symbols_cache_dict(self, f):
+        """f == file like object
 
-        self.__stdout = b""
-        self.__stderr = b""
-        self._stdout_echo = False
-        self._stderr_echo = False
-        self.engine._frida_device.on('output', self.__fd_cb)
+        Returns either None (if no cache exists) or dict of cache."""
 
-        if "resume" in kwargs and kwargs["resume"]:
-            self.resume()
+        if f is None:
+            return None
 
-    def __handle_process_exception(self, data, msg):
+        assert isinstance(f, io.IOBase), 'Unhandled symbol cache load type of {}'.format(type(f))
 
-        def cleanup():
-            self.memory[wait_for].int8 = 1
+        f.seek(0, 0)
+        h = hashlib.sha256(f.read()).hexdigest()
+        f.seek(0, 0)
 
-        assert data['type'] == 'send', "Unexpected type of " + data['type']
-        assert 'payload' in data, "No payload found in data."
+        this_cache_file = os.path.join(symbol_cache_path, h)
 
-        exception = data['payload']
-        wait_for = common.auto_int(exception['wait_for'])
-        thread_id = exception['thread_id']
+        # Cache miss
+        if not os.path.isfile(this_cache_file):
+            return None
 
-        native_exception = NativeException._from_frida_dict(self, exception, [])
+        # Cache hit
+        with open(this_cache_file, "r") as f:
+            return json.loads(f.read())
 
-        # Append this to the appropriate thread
-        # NOTE: For whatever reason, anything that attempts to interact with frida at this point in execution will hang...
-        self.threads._exceptions[thread_id].append(native_exception)
+    def _load_symbols_cache(self, cache):
+        """Loads symbols previously discovered.
 
-        LOGGER.warning("Caught exception in thread {thread} of type {type} at {at}.\n\tView with process.threads[{thread}].exceptions[-1]".format(
-            thread=thread_id,
-            type=exception['type'],
-            at=exception['address'],
-        ))
+        Args:
+            cache (dict): Dictionary cache to load up.
+        """
 
-        # Make sure this auto-cleans up on exit
-        self._register_cleanup(cleanup)
+        for sym, address in cache.items():
+            if self._process.file_type is "PE" or \
+                    (self.elf is not None and self.elf.type_str == 'DYN'):
+                address = address + self.base
 
-    def __frida_process_general_init(self):
-        """General purpose frida initializations."""
+            self._process.modules._symbol_to_address[self.name][sym] = types.Pointer(address)
+            self._process.modules._address_to_symbol[address] = sym
 
-        if self._ignore_exceptions is not True:
 
-            # TODO: Optionally specify which signals to allow (such as int3)
-            self.engine.run_script_generic("exception_handler.js", unload=False, runtime='v8', on_message=self.__handle_process_exception, timeout=0,
-                                           include_js=["dispose.js", "send_batch.js", "telescope.js", "timeless.js"])
+    def _save_symbols_cache(self, file_io, cache):
+        """Saves symbols into cache to be used later.
 
-            # Register this for cleanup since we need it to be removed first.
-            script = self.engine._scripts.pop(0)
-            self._register_cleanup(lambda: self.engine._unload_script(script[0], allow_exceptions=[frida.InvalidOperationError]))
+        Args:
+            file_io (file like): The base file in full.
+            cache (dict): The symbols we discovered.
+        """
 
-    def __frida_process_windows_init(self):
-        """Setup stuff specifically for Frida process on windows."""
+        file_io.seek(0, 0)
+        h = hashlib.sha256(file_io.read()).hexdigest()
+        file_io.seek(0, 0)
 
-        try:
-            setbuf = self.memory['setbuf']
-        except RevengeSymbolLookupFailure:
-            LOGGER.warning("Couldn't resolve setbuf. Unbuffering of io is disabled.")
-            return
+        this_cache_file = os.path.join(symbol_cache_path, h)
+        with open(this_cache_file, "w") as f:
+            f.write(json.dumps(cache))
+        
 
-        # Windows resolves stdin/out/error using __iob_func
-        try:
-            iob = self.memory['__iob_func']()
-        except RevengeSymbolLookupFailure:
-            LOGGER.warning("Couldn't resolve __iob_func. Unbuffering of io is disabled.")
+    def _load_symbols(self):
+        """Reads in the file for this module and attempts to extract the symbols."""
+
+        # Either we're loading everything or what we're looking at right now __should__ be loaded
+        if self._process._load_symbols is None or any(True for x in self._process._load_symbols if fnmatch(self.name, x)):
+
+            # Clear out old symbols if needed
+            self._process.modules._symbol_to_address[self.name] = {}
+
+            file_io = common.load_file(self._process, self.path)
+            cache = self._read_symbols_cache_dict(file_io)
+
+            if cache is not None:
+                return self._load_symbols_cache(cache)
+        
+            if self._process.file_type == 'ELF':
+                self._load_symbols_elf(file_io)
+            
+            elif self._process.file_type == "PE":
+                self._load_symbols_pe(file_io)
+
+            # TODO: Windows
+            # TODO: Mac
+
+        # If we didn't resolve anything, make sure we noted we tried
+        if self.name not in self._process.modules._symbol_to_address:
+            self._process.modules._symbol_to_address[self.name] = {}
+
+    def _load_symbols_pe(self, pe_io):
+        # TODO: Assuming that this process will work on any system running ELF...
+        print("Loading symbols for {} ... ".format(self.name), end='', flush=True)
+
+        pe = pefile.PE(data=pe_io.read())
+        cache = {}
+
+        # Some PEs don't export anything.
+        if hasattr(pe, "DIRECTORY_ENTRY_EXPORT"):
+            for sym in pe.DIRECTORY_ENTRY_EXPORT.symbols:
+                if sym.name in [b'', None]:
+                    continue
+
+                name = sym.name.decode()
+
+                rel_address = sym.address
+                address = rel_address + self.base
+
+                self._process.modules._symbol_to_address[self.name][name] = types.Pointer(address)
+                self._process.modules._address_to_symbol[address] = name
+                cache[name] = rel_address
+
+        self._save_symbols_cache(pe_io, cache)
+        cprint("[ DONE ]", "green")
+
+    def _load_symbols_elf(self, elf_io):
+        # TODO: Assuming that this process will work on any system running ELF...
+        print("Loading symbols for {} ... ".format(self.name), end='', flush=True)
+
+        if elf_io is None:
+            cprint("[ Failed to load ]", "yellow")
             return
 
-        # Unbuffer stdout
-        setbuf(iob + 0x30, 0)
+        e = ELFFile(elf_io)
+
+        #
+        # Load up any symbols from the file
+        #
+
+        symtab = e.get_section_by_name('.symtab')
+        dynsym = e.get_section_by_name('.dynsym')
+
+        symbols = []
+        cache = {}
+
+        # Sometimes the binary won't have a symbol table
+        if symtab is not None:
+            symbols.append(symtab.iter_symbols())
 
-    def __frida_process_linux_init(self):
-        """Setup stuff specifically for Frida process on linux."""
+        if dynsym is not None:
+            symbols.append(dynsym.iter_symbols())
 
-        stdout = self.memory['stdout']
-        setbuf = self.memory['setbuf']
+        # Pull out symbols
+        for sym in itertools.chain(*symbols):
+            if sym.name == '':
+                continue
 
-        # Unbuffer stdout
-        setbuf(stdout.pointer, 0)
+            address = sym['st_value']
+            rel_address = address
 
-    def __fd_cb(self, pid, fd, data):
-        if pid != self.pid:
+            if self.elf.type_str == 'DYN':
+                address = address + self.base
+
+            self._process.modules._symbol_to_address[self.name][sym.name] = types.Pointer(address)
+            self._process.modules._address_to_symbol[address] = sym.name
+            cache[sym.name] = rel_address
+
+        self._save_symbols_cache(elf_io, cache)
+
+        cprint("[ DONE ]", "green")
+
+    def __repr__(self):
+        attrs = ['Module', self.name, '@', hex(self.base)]
+        return "<{}>".format(' '.join(attrs))
+
+    def __eq__(self, other):
+        return self.name == other.name and self.base == other.base and self.path == other.path and self.size == other.size
+
+    @property
+    def name(self):
+        """str: Module name."""
+        return self.__name
+
+    @name.setter
+    def name(self, name):
+        if type(name) is not str:
+            error = "Name must be string, not {}".format(type(name))
+            logger.error(error)
+            raise Exception(error)
+
+        self.__name = name
+
+    @property
+    def base(self):
+        """int: Base address this module is loaded at."""
+        return self.__base
+
+    @base.setter
+    def base(self, base):
+
+        base = common.auto_int(base)
+
+        if type(base) is int:
+            base = types.Pointer(base)
+
+        self.__base = base
+
+    @property
+    def path(self):
+        """str: Module path."""
+        return self.__path
+
+    @path.setter
+    def path(self, path):
+        if type(path) is not str:
+            error = "Path must be string, not {}".format(type(path))
+            logger.error(error)
+            raise Exception(error)
+
+        self.__path = path
+
+        # Load up the symbols for this file if we haven't already
+        if self.name not in self._process.modules._symbol_to_address:
+            self._load_symbols()
+        
+    @property
+    def size(self):
+        """int: Size of this module."""
+        return self.__size
+
+    @size.setter
+    def size(self, size):
+        self.__size = common.auto_int(size)
+
+    @property
+    def elf(self):
+        """Returns ELF object, if applicable, otherwise None."""
+
+        if self._process.file_type != 'ELF':
             return
 
-        if fd == 1:
-            if self._stdout_echo:
-                print(data.decode('utf-8'), end='', flush=True)
-
-            else:
-                self.__stdout += data
-
-        elif fd == 2:
-            if self._stderr_echo:
-                print(data.decode('utf-8'), end='', flush=True)
-
-            else:
-                self.__stderr += data
-
-        else:
-            LOGGER.warning("Unhandled fd callback: fd == " + hex(fd))
-
-    @common.validate_argument_types(thing=(str, bytes))
-    def stdin(self, thing):
-        thing = common.auto_bytes(thing)
-        self.engine._frida_device.input(self.pid, thing)
-
-    @common.validate_argument_types(n=(int, str, bytes))
-    def stderr(self, n=0):
-
-        if n == 0:
-            ret = self.__stderr
-            self.__stderr = b""
-            return ret
-
-        # String acts as an expect
-        if isinstance(n, (str, bytes)):
-            n = common.auto_bytes(n)
-            # TODO: Might be more efficient to use try/except...
-            while n not in self.__stderr:
-                sleep(0.01)
-            index = self.__stderr.index(n) + len(n)
-            ret = self.__stderr[:index]
-            self.__stderr = self.__stderr[index:]
-            return ret
-
-        else:
-            # n is an int. take that much
-            ret = self.__stderr[:n]
-            self.__stderr = self.__stderr[n:]
-            return ret
-
-    @common.validate_argument_types(n=(int, str, bytes))
-    def stdout(self, n=0):
-
-        if n == 0:
-            ret = self.__stdout
-            self.__stdout = b""
-            return ret
-
-        # String acts as an expect
-        if isinstance(n, (str, bytes)):
-            n = common.auto_bytes(n)
-            # TODO: Might be more efficient to use try/except...
-            while n not in self.__stdout:
-                sleep(0.01)
-            index = self.__stdout.index(n) + len(n)
-            ret = self.__stdout[:index]
-            self.__stdout = self.__stdout[index:]
-            return ret
-
-        else:
-            # n is an int. take that much
-            ret = self.__stdout[:n]
-            self.__stdout = self.__stdout[n:]
-            return ret
-
-    def interactive(self):
-        old_stdout_echo = self._stdout_echo
-        self._stdout_echo = True
-
-        # TODO: Update this so that stdout doesn't clobber stderr and vice vera..
-        old_stderr_echo = self._stderr_echo
-        self._stderr_echo = True
-
-        # Flush out stdout buffer
-        # print(self.stdout('all').decode('utf-8'), end="", flush=True)
-        print(self.stdout().decode('utf-8'), end="", flush=True)
-
-        # TODO: Maybe change this to single char get and send at some point?
-        while True:
-            try:
-                thing = prompt_toolkit.prompt()
-                self.stdin(thing + "\n")
-            except KeyboardInterrupt:
-                break
-
-        self._stdout_echo = old_stdout_echo
-        self._stderr_echo = old_stderr_echo
-
-    def resume(self):
-        threads = list(self.threads)
-
-        if len(self.threads) == 0:
-            return self.engine.resume(self.pid)
-
-        # First, check for suspended threads
-        for thread in threads:
-            if thread.state == "stopped":
-                # Can only resume the entire process for now
-                return self.engine.resume(self.pid)
-
-        # Next, check for revenge breakpoints
-        for thread in threads:
-            if thread.breakpoint:
-                thread.breakpoint = False
-
-
-from time import sleep
-import prompt_toolkit
-from ...native_exception import NativeException
+        try:
+            return self.__elf
+        except AttributeError:
+            self.__elf = ELF(self._process, self)
+            return self.__elf
+
+    @property
+    def symbols(self):
+        """dict: symbol name -> address for this binary."""
+        return self._process.modules._symbol_to_address[self.name]
 
-LOGGER = logging.getLogger(__name__)
+from ..parsers import ELF
```

### Comparing `revenge-0.21/revenge/js/find_in_memory.js` & `revenge-0.9/revenge/js/find_in_memory.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 function memory_scan_match(match) {
 
     if (match.length == 0) {
         return;
     }
 
-    var address = match.address;
-    var size = match.size;
+    var address = match['address'];
+    var size = match['size'];
 
     var d = {
         'address': address,
         'size': size
     };
 
     total_matches.push(d);
@@ -21,15 +21,15 @@
     }
 }
 
 function memory_scan_completed() {
 
     if (total_matches.length > 0) {
         send(total_matches);
-    }
+    };
 
     send('DONE');
 }
 
 // Add downselect to include module here
 var search_space = SEARCH_SPACE_HERE;
 var total_matches = [];
@@ -37,26 +37,35 @@
 
 var base = null;
 var size = null;
 
 setTimeout(function() {
     search_space.forEach(
         function(range) {
-            base = eval(range.base);
-            size = range.size;
-            //protection = Process.getRangeByAddress(base).protection;
+            base = eval(range['base']);
+            size = range['size'];
+            protection = Process.getRangeByAddress(base).protection;
 
-            try {
+            // Protection can actually change between enumerating at the execution of scan. Try to catch that.
+            if (protection == "rw-" || protection == "rwx" || protection == "r-x") {
                 Memory.scanSync(base, size, "SCAN_PATTERN_HERE").forEach(memory_scan_match);
-            } catch {}
+            };
+        });
+
+    memory_scan_completed();
+});
+
+/*
+setTimeout(function () {
+    search_space.enumerateRangesSync('rw').forEach(
+        function (range) {
+            protection = Process.getRangeByAddress(range.base).protection;
 
-            /*
             // Protection can actually change between enumerating at the execution of scan. Try to catch that.
-            if ( protection == "rw-" || protection == "rwx" || protection == "r-x") {
-                try { 
-                    Memory.scanSync(base, size, "SCAN_PATTERN_HERE").forEach( memory_scan_match );
-                } catch {}
-            }*/
+            if ( protection == "rw-" || protection == "rwx" ) {
+                Memory.scanSync(range.base, range.size, "SCAN_PATTERN_HERE").forEach( memory_scan_match );
+            };
         });
 
     memory_scan_completed();
-});
+});
+*/
```

### Comparing `revenge-0.21/revenge/js/stalk.js` & `revenge-0.9/revenge/js/stalk.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,122 +1,163 @@
-/* 
- * Basic stalker
- *
- * requires: dispose.js, batch_send.js
- */
-
-function stalker_is_in_range(ranges, val) {
-    var range;
-    for (var i = 0; i < ranges.length; i++) {
-        range = ranges[i];
-        if (val >= range[0] && val <= range[1])
-            return true;
+//////
+// Borrowed from https://codeshare.frida.re/@mrmacete/stalker-event-parser/
+/////
+
+
+var EV_TYPE_NOTHING = 0;
+var EV_TYPE_CALL = 1;
+var EV_TYPE_RET = 2;
+var EV_TYPE_EXEC = 4;
+var EV_TYPE_BLOCK = 8;
+var EV_TYPE_COMPILE = 16;
+
+var intSize = Process.pointerSize;
+var EV_STRUCT_SIZE = 2 * Process.pointerSize + 2 * intSize;
+
+function parseEvents(blob, callback) {
+    var len = getLen(blob);
+    for (var i = 0; i !== len; i++) {
+        var type = getType(blob, i);
+        switch (type) {
+            case EV_TYPE_CALL:
+                callback(parseCallEvent(blob, i));
+                break;
+            case EV_TYPE_RET:
+                callback(parseRetEvent(blob, i));
+                break;
+            case EV_TYPE_EXEC:
+                callback(parseExecEvent(blob, i));
+                break;
+            case EV_TYPE_BLOCK:
+                callback(parseBlockEvent(blob, i));
+                break;
+            case EV_TYPE_COMPILE:
+                callback(parseCompileEvent(blob, i));
+                break;
+            default:
+                console.log('Unsupported type ' + type);
+                break;
+        }
     }
-    return false;
 }
 
-function stalker_is_in_include_function(include_function, event) {
-    var ip = include_function;
-    var type = event[0];
-    var inside = stalker_is_in_include_function.inside || false;
-    var inside_depth_floor = stalker_is_in_include_function.inside_depth_floor;
-
-    if (type == 'call') {
-        var call_target = ptr(event[2]);
-
-        // We're stepping into this function
-        if (!inside && call_target.compare(ip) == 0) {
-            stalker_is_in_include_function.inside = true;
-            stalker_is_in_include_function.inside_depth_floor = Number(event[3]);
-        }
-    } else if (type == 'ret') {
-        var current_depth = Number(event[3]);
+function getType(blob, idx) {
+    return parseInteger(blob, idx, 0);
+}
 
-        // If we're inside and about to step out
-        if (inside && current_depth == inside_depth_floor + 1) {
-            // Set outside, but still return this as being inside
-            stalker_is_in_include_function.inside = false;
-        }
-    }
+function getLen(blob) {
+    return blob.byteLength / EV_STRUCT_SIZE;
+}
 
-    return inside;
+function parseCallEvent(blob, idx) {
+    return {
+        type: 'call',
+        location: parsePointer(blob, idx, intSize),
+        target: parsePointer(blob, idx, intSize + Process.pointerSize),
+        depth: parseInteger(blob, idx, intSize + 2 * Process.pointerSize)
+    };
 }
 
-// This function handles implicitly adding event depth based on previous depths
-function event_get_depth(event) {
-    var depth = event_get_depth.depth || 0;
+function parseRetEvent(blob, idx) {
+    var ev = parseCallEvent(blob, idx);
+    ev.type = 'ret';
+    return ev;
+}
 
-    if (event[0] == 'call') {
-        depth = Number(event[3]) + 1;
-        event_get_depth.depth = depth;
+function parseExecEvent(blob, idx) {
+    var loc = parsePointer(blob, idx, intSize);
+    return {
+        type: 'exec',
+        location: loc,
+        code: Instruction.parse(loc).toString()
+    };
+}
 
-    } else if (event[0] == 'ret') {
-        depth = Number(event[3]) - 1;
-        event_get_depth.depth = depth;
+function parseBlockEvent(blob, idx) {
+    var begin = parsePointer(blob, idx, intSize);
+    var end = parsePointer(blob, idx, intSize + Process.pointerSize);
+    var i = begin.add(0);
+    var code = [];
+    while (i.compare(end) < 0) {
+        var instr = Instruction.parse(i);
+        code.push(i.toString() + '    ' + instr.toString());
+        i = instr.next;
     }
+    return {
+        type: 'block',
+        begin: begin,
+        end: end,
+        code: code.join('\n')
+    };
+}
 
-    return event_get_depth.depth;
+function parseCompileEvent(blob, idx) {
+    var parsed = parseBlockEvent(blob, idx);
+    parsed.type = 'compile';
+    return parsed;
 }
 
-function stalker_follow(tid) {
-    var module_map = new ModuleMap();
-    var include_from = FROM_MODULES_HERE;
-    var include_function = INCLUDE_FUNCTION_HERE;
-    var exclude_ranges = Array();
-
-    EXCLUDE_RANGES_HERE.forEach(function(item) {
-        exclude_ranges.push(Array(eval(item[0]), eval(item[1])));
-    });
+function parseInteger(blob, idx, offset) {
+    return new Int32Array(blob, idx * EV_STRUCT_SIZE + offset, 1)[0];
+}
 
-    // Unfollow must be called from the source script doing the stalking. Thus, RPC.
-    rpc.exports.unfollow = function() {
-        Stalker.unfollow(tid);
-        Stalker.flush();
-    };
+function parsePointer(blob, idx, offset) {
+    var view = new Uint8Array(blob, idx * EV_STRUCT_SIZE + offset, Process.pointerSize);
+    var stringed = [];
+    for (var i = 0; i < Process.pointerSize; i++) {
+        var x = view[i];
+        var conv = x.toString(16);
+        if (conv.length === 1) {
+            conv = '0' + conv;
+        }
+        stringed.push(conv);
+    }
+    return ptr('0x' + stringed.reverse().join(''));
+}
 
-    // This is automagically called when unloading a script in python
-    dispose_push(function() {
-        Stalker.unfollow(tid);
-    });
+function reverse(arr) {
+    var result = [];
+    for (var i = arr.length - 1; i >= 0; i--) {
+        result.push(arr[i]);
+    }
+    return result;
+}
+
+////
+// Basic stalker
+///
 
-    // TODO: What should this actually be?
-    // also, lower this back down when Stalker starts draining properly again
-    Stalker.queueCapacity = 1048576; // 32768; //65536;
-    //Stalker.queueDrainInterval = 10;
+//var threads = Process.enumerateThreadsSync()
+//for (var i=0; i < threads.length; i++) {
 
+
+function stalker_follow(tid) {
     Stalker.follow(tid, {
         events: {
-            call: STALK_CALL || include_function !== null, // CALL instructions
-            ret: STALK_RET || include_function !== null, // RET instructions
-            exec: STALK_EXEC, // all instructions: not recommended as it's a lot of data
+            call: STALK_CALL, // CALL instructions
+
+            // Other events:
+            ret: STALK_RET, // RET instructions
+            exec: STALK_EXEC, // all instructions: not recommended as it's
+            //                   a lot of data
             block: STALK_BLOCK, // block executed: coarse execution trace
             compile: STALK_COMPILE // block compiled: useful for coverage
         },
 
         onReceive: function(events) {
+            //return send(Stalker.parse(events, {annotate: true, stringify: true}));
+            //send(Stalker.parse(events, {annotate: true, stringify: true}));
 
             var filtered_events = [];
 
             Stalker.parse(events, {
                 annotate: true,
                 stringify: true
             }).forEach(function x(event) {
 
-                var depth = event_get_depth(event);
-
-                // Handle include function
-                if (include_function !== null && !stalker_is_in_include_function(include_function, event)) {
-                    return;
-                }
-
-                // Handle exclude ranges
-                if (stalker_is_in_range(exclude_ranges, ptr(event[1]))) {
-                    return;
-                }
-
                 //
                 // Module filtering
                 //
 
                 var from_module = module_map.findName(ptr(event[1]));
 
                 if (from_module != null) {
@@ -124,76 +165,92 @@
                     // Ignore frida agent calls
                     if (from_module.substring(0, 11) == "frida-agent") {
                         return;
                     }
 
                     // Optionally only include from some modules
                     if (include_from.length > 0 && !include_from.includes(from_module)) {
-                        return;
+                        return
                     }
 
                 }
 
-                var event_dict = {};
+                var event_dict = {}
 
                 if (event[0] == 'call') {
 
-                    event_dict.tid = tid;
-                    event_dict.type = 'call';
-                    event_dict.from_ip = event[1];
-                    event_dict.to_ip = event[2];
-                    event_dict.depth = Number(event[3]);
-                    event_dict.from_module = from_module;
-                    event_dict.to_module = module_map.findName(ptr(event[2]));
+                    var to_module = module_map.findName(ptr(event[2]));
+                    event_dict['tid'] = tid;
+                    event_dict['type'] = 'call';
+                    event_dict['from_ip'] = event[1];
+                    event_dict['to_ip'] = event[2];
+                    event_dict['depth'] = event[3];
+                    event_dict['from_module'] = from_module;
+                    event_dict['to_module'] = to_module;
 
                 } else if (event[0] == 'ret') {
 
-                    event_dict.tid = tid;
-                    event_dict.type = 'ret';
-                    event_dict.from_ip = event[1];
-                    event_dict.to_ip = event[2];
-                    event_dict.depth = Number(event[3]);
-                    event_dict.from_module = from_module;
-                    event_dict.to_module = module_map.findName(ptr(event[2]));
+                    var to_module = module_map.findName(ptr(event[2]));
+                    event_dict['tid'] = tid;
+                    event_dict['type'] = 'ret';
+                    event_dict['from_ip'] = event[1];
+                    event_dict['to_ip'] = event[2];
+                    event_dict['depth'] = event[3];
+                    event_dict['from_module'] = from_module;
+                    event_dict['to_module'] = to_module;
 
                 } else if (event[0] == 'exec') {
 
-                    event_dict.tid = tid;
-                    event_dict.type = 'exec';
-                    event_dict.from_ip = event[1];
-                    event_dict.from_module = from_module;
-                    event_dict.depth = depth;
+                    event_dict['tid'] = tid;
+                    event_dict['type'] = 'exec';
+                    event_dict['from_ip'] = event[1];
+                    event_dict['from_module'] = from_module;
 
                 } else if (event[0] == 'block') {
 
-                    event_dict.tid = tid;
-                    event_dict.type = 'block';
-                    event_dict.from_ip = event[1];
-                    event_dict.to_ip = event[2];
-                    event_dict.from_module = from_module;
-                    event_dict.to_module = module_map.findName(ptr(event[2]));
-                    event_dict.depth = depth;
+                    var to_module = module_map.findName(ptr(event[2]));
+                    event_dict['tid'] = tid;
+                    event_dict['type'] = 'block';
+                    event_dict['from_ip'] = event[1];
+                    event_dict['to_ip'] = event[2];
+                    event_dict['from_module'] = from_module;
+                    event_dict['to_module'] = to_module;
 
                 } else if (event[0] == 'compile') {
 
-                    event_dict.tid = tid;
-                    event_dict.type = 'compile';
-                    event_dict.from_ip = event[1];
-                    event_dict.to_ip = event[2];
-                    event_dict.from_module = from_module;
-                    event_dict.to_module = module_map.findName(ptr(event[2]));
-                    event_dict.depth = depth;
+                    var to_module = module_map.findName(ptr(event[2]));
+                    event_dict['tid'] = tid;
+                    event_dict['type'] = 'compile';
+                    event_dict['from_ip'] = event[1];
+                    event_dict['to_ip'] = event[2];
+                    event_dict['from_module'] = from_module;
+                    event_dict['to_module'] = to_module;
 
                 }
 
-                //filtered_events.push(event_dict);
-                send_batch(event_dict);
+                filtered_events.push(event_dict);
             });
 
-            /*
-            if ( filtered_events.length != 0 ) {
-                send_batch(filtered_events);
-                //send(filtered_events);
-            } */
+            if (filtered_events.length != 0) {
+                send(filtered_events);
+            }
         }
     })
-}
+}
+
+var module_map = new ModuleMap();
+var tid = THREAD_ID_HERE;
+var include_from = FROM_MODULES_HERE;
+
+rpc.exports = {
+    // Unfollow must be called from the source script doing the stalking. Thus, RPC.
+    unfollow: function() {
+        Stalker.unfollow(tid);
+        Stalker.flush();
+    },
+    // This is automagically called when unloading a script in python
+    dispose: function() {
+        Stalker.unfollow(tid);
+    },
+}
+
+stalker_follow(tid);
```

### Comparing `revenge-0.21/revenge/js/windows_stalk_message_handlers.js` & `revenge-0.9/revenge/js/windows_stalk_message_handlers.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
-var GetWindowLongPtrA = new NativeFunction(Module.getExportByName('user32.dll', 'GetWindowLongPtrA'), 'pointer', ['pointer', 'int']);
-var GetWindowLongPtrW = new NativeFunction(Module.getExportByName('user32.dll', 'GetWindowLongPtrW'), 'pointer', ['pointer', 'int']);
-var IsWindowUnicode = new NativeFunction(Module.getExportByName('user32.dll', 'IsWindowUnicode'), 'int', ['pointer']);
+var GetWindowLongPtrA = new NativeFunction(Module.getExportByName('user32.dll', 'GetWindowLongPtrA'), 'pointer', ['pointer', 'int'])
+var GetWindowLongPtrW = new NativeFunction(Module.getExportByName('user32.dll', 'GetWindowLongPtrW'), 'pointer', ['pointer', 'int'])
+var IsWindowUnicode = new NativeFunction(Module.getExportByName('user32.dll', 'IsWindowUnicode'), 'int', ['pointer'])
 
-var known_window_handlers = [];
+var known_window_handlers = []
 
 //
 // General HWND resolver
 // 
 function hwnd_resolver(hwnd) {
 
     // Don't both with null pointer
     if (hwnd == 0) {
-        return;
+        return
     }
 
     var phwnd = ptr(hwnd);
     var phandler = 0;
 
     if (IsWindowUnicode(phwnd)) {
         // Need it as string for the stupid Array check to work.
```

### Comparing `revenge-0.21/revenge/memory/find.py` & `revenge-0.9/revenge/memory/find.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,83 @@
 
 import logging
-
 logger = logging.getLogger(__name__)
 
+import json
+
 from .. import common, types
 import time
 
-
 class MemoryFind(object):
 
-    def __init__(self, engine, thing, ranges=None):
+    def __init__(self, process, thing, ranges=None):
         """Find something in memory.
 
         Args:
-            engine: Base engine instantiation
+            process: Base process instantiation
             thing: Some instantiated type to search for from types module
             ranges(list, optional): List of MemoryRange objects to limit the search
                 to. By default, search everything.
         """
-        self._engine = engine
-        self._process = self._engine._process
+        self._process = process
         self.thing = thing
         self.ranges = ranges
 
+        # Loaded script to unload once we're done
+        self._script = None
+
         # Not completed yet
         self.completed = False
 
         # Memory locations we discovered
         self.found = set()
 
+        self._start()
+
     def sleep_until_completed(self):
         """This call sleeps and only returns once the search is completed."""
 
         while not self.completed:
             time.sleep(0.1)
 
-    @common.implement_in_engine()
     def _start(self):
         """Starts the search."""
-        pass
+
+        replace = {
+                "SCAN_PATTERN_HERE": self.search_string,
+                "SEARCH_SPACE_HERE": json.dumps(self._ranges_js),
+                }
+
+        self._process.run_script_generic("find_in_memory.js", replace=replace, unload=False, on_message=self._on_message)
+        self._script = self._process._scripts.pop(0)
+
+    def _on_message(self, m,d):
+        """Catch messages from our search."""
+        payload = m['payload']
+
+        if type(payload) is list:
+            for addr in payload:
+                self.found.add(types.Pointer(common.auto_int(addr['address'])))
+        
+        elif type(payload) is str and payload == 'DONE':
+            self.completed = True
+
+        else:
+            logger.error("Unexpected message: {} {}".format(m,d))
+
+    def __del__(self):
+        # Be sure to unload our script
+        if self._script is not None:
+            self._script[0].unload()
+            self._script = None
 
     def __repr__(self):
         attr = ["MemoryFind"]
         attr += ["found", str(len(self.found))]
-
+        
         if self.completed:
             attr.append("completed")
         else:
             attr.append("running")
 
         return "<{}>".format(' '.join(attr))
 
@@ -66,55 +96,69 @@
         return self.__completed
 
     @completed.setter
     def completed(self, completed):
         assert type(completed) is bool
         self.__completed = completed
 
+        # Clean up our search script when we're done.
+        if completed and self._script is not None:
+            self._script[0].unload()
+            self._script = None
+
     @property
     def search_string(self):
         """The search string for this thing."""
         return self._process.memory._type_to_search_string(self.thing)
 
     @property
     def thing(self):
         """What we're looking for."""
         return self.__thing
 
     @thing.setter
     def thing(self, thing):
-
+        
         if not isinstance(thing, types.all_types):
             error = "Invalid search thing of type {}".format(type(thing))
             logger.error(error)
             raise Exception(error)
 
         self.__thing = thing
 
     @property
+    def _ranges_js(self):
+        """Returns the ranges as a list for insertion into js."""
+        l = []
+        for range in self.ranges:
+            d = {'base': range.base.js, 'size': range.size}
+            l.append(d)
+
+        return l
+
+    @property
     def ranges(self):
         return self.__ranges
 
     @ranges.setter
     def ranges(self, ranges):
-
+        
         if ranges is None:
             # It appears the first time maps gets run, something in the Frida actually changes... Not sure what.
             # Running this here to prime the pump as it were.. Maybe some day figure out wtf is going on.
             # REMINDER: This bug didn't always hit. So pytest may say it's fine when it isn't.
             self._process.memory.maps
             self._process.memory.maps
 
-            ranges = [range for range in self._process.memory.maps if range.readable]
+            ranges = list(self._process.memory.maps)
 
         if type(ranges) is MemoryRange:
             self.__ranges = [ranges]
 
         if type(ranges) not in (list, tuple):
             error = "Invalid range type of {}".format(type(ranges))
             logger.error(error)
             raise Exception(error)
 
         self.__ranges = ranges
 
-
 from . import MemoryRange
```

### Comparing `revenge-0.21/revenge/memory/map.py` & `revenge-0.9/revenge/memory/map.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 logger = logging.getLogger(__name__)
 
 from .. import common, types
 
 class MemoryMap(object):
     """Small wrapper to simply memory map lookups."""
 
-    def __init__(self, engine):
-        self._engine = engine
-        self._process = self._engine._process
+    def __init__(self, process):
+        self._process = process
+
+        ranges = self._process.run_script_generic("""send(Process.enumerateRangesSync(''));""", raw=True, unload=True)[0][0]
+        self._ranges = [MemoryRange(self._process, **range) for range in ranges]
 
     def __iter__(self):
         return self._ranges.__iter__()
 
     def __len__(self):
         return self._ranges.__len__()
 
     def __repr__(self):
         attrs = ['MemoryMap', str(len(self)), 'mapped ranges']
         return "<{}>".format(' '.join(attrs))
 
     def __str__(self):
-        return str(self._engine.memory)
+        return str(self._process.memory)
 
     def __getitem__(self, item):
 
         if isinstance(item, int):
             for range in self:
                 if item >= range.base and item <= range.base + range.size:
                     return range
```

### Comparing `revenge-0.21/revenge/memory/memory_range.py` & `revenge-0.9/revenge/memory/memory_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,28 @@
+
 import logging
 logger = logging.getLogger(__name__)
 
-from .. import common, types, exceptions
+from .. import common, types
 
 class MemoryRange(object):
 
-    def __init__(self, engine, base, size, protection, file=None):
-        self._engine = engine
-        self._process = self._engine._process
+    def __init__(self, process, base, size, protection, file=None):
+        self._process = process
         self.base = base
         self.size = size
         self.protection = protection
         self._file = file
 
-    @common.implement_in_engine()
-    def set_protection(self, read, write, execute):
-        """Sets the protection for this memory page.
-
-        Args:
-            read (bool): Allow read?
-            write (bool): Allow write?
-            execute (bool): Allow execute?
-
-        This will call appropriate mprotect or similar. This can be done
-        implicitly from the .protection property.
-        """
-        pass
-
     def __repr__(self):
         value = ["MemoryRange", hex(self.base), '-', hex(self.base+self.size), self.protection]
         if self.file is not None:
             value.append(self.file + ":" + hex(self.file_offset))
         return '<' + ' '.join(value) + '>'
 
-    def __hash__(self):
-        return hash((self.base, self.size, self.protection, self.file))
 
     @property
     def file(self):
         """str: File backing this memory range, or None."""
         if self._file is None:
             return None
 
@@ -80,19 +64,21 @@
 
         # If we're setting for the first time, assume it's correct
         if not hasattr(self, '_MemoryRange__protection'):
             self.__protection = protection
 
         # Set protection if it's not already this
         elif protection != self.protection:
-            self.set_protection(
-                protection[0] == "r",
-                protection[1] == "w",
-                protection[2] == "x",
-                )
+            self._process.run_script_generic("""Memory.protect({}, {}, '{}')""".format(
+                self.base.js,
+                hex(self.size),
+                protection,
+                ), raw=True, unload=True)
+
+            self.__protection = protection
 
     @property
     def size(self):
         """int: Size for this range."""
         return self.__size
 
     @size.setter
@@ -103,8 +89,7 @@
     def base(self):
         """int: Base address for this range."""
         return self.__base
 
     @base.setter
     def base(self, base):
         self.__base = types.Pointer(common.auto_int(base))
-
```

### Comparing `revenge-0.21/revenge/modules/module.py` & `revenge-0.9/revenge/tracer/instruction_tracer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,380 +1,326 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
-from elftools.elf.elffile import ELFFile
-from termcolor import cprint, colored
-import itertools
-import hashlib
-import os
-import io
+import multiprocessing
+import time
 import json
-from fnmatch import fnmatch
-import pefile
+import collections
+from termcolor import cprint, colored
 
-from .. import common, types, config, symbols
+from prettytable import PrettyTable
 
-symbol_cache_path = os.path.join(config.app_dirs.user_cache_dir, 'symbol_cache')
-os.makedirs(symbol_cache_path, exist_ok=True)
+from .. import types, common
+from ..threads import Thread
 
-class Module(object):
+class TraceItem(object):
 
-    def __init__(self, process, name, base, size, path):
+    def __init__(self, process, item):
         self._process = process
-        self.name = name
-        self.base = base
-        self.size = size
-
-        self.path = path # Must go last
-
-    def _read_symbols_cache_dict(self, f):
-        """f == file like object
-
-        Returns either None (if no cache exists) or dict of cache."""
-
-        if f is None:
-            return None
-
-        assert isinstance(f, io.IOBase), 'Unhandled symbol cache load type of {}'.format(type(f))
-
-        f.seek(0, 0)
-        h = hashlib.sha256(f.read()).hexdigest()
-        f.seek(0, 0)
-
-        this_cache_file = os.path.join(symbol_cache_path, h)
-
-        # Cache miss
-        if not os.path.isfile(this_cache_file):
-            return None
-
-        # Cache hit
-        with open(this_cache_file, "r") as f:
-            return json.loads(f.read())
-
-    def _load_symbols_cache(self, cache):
-        """Loads symbols previously discovered.
-
-        Args:
-            cache (dict): Dictionary cache to load up.
-        """
-
-        #
-        # Symbols
-        #
-
-        for sym, address in cache['symbols'].items():
-            if self._process.file_type == "PE" or \
-                    (self.elf is not None and self.elf.type_str == 'DYN'):
-                address = address + self.base
-
-            sym = symbols.Symbol(self._process, name=sym, address=address)
-            self._process.modules._symbol_to_address[self.name][sym.name] = sym
-            self._process.modules._address_to_symbol[address] = sym
-
-        #
-        # Sections
-        #
-
-        if 'plt_offset' in cache:
-            self.plt = cache['plt_offset']
-
-        #
-        # PLT
-        #
-
-        if 'plt' in cache:
-            for i, sym in enumerate(cache['plt']):
-                addr = self.plt + ((i+1)*0x10)
-                name = 'plt.' + sym
-                sym = symbols.Symbol(self._process, name=name, address=addr)
-                self._process.modules._symbol_to_address[self.name][name] = sym
-                self._process.modules._address_to_symbol[addr] = sym
-
-    def _save_symbols_cache(self, file_io, cache):
-        """Saves symbols into cache to be used later.
-
-        Args:
-            file_io (file like): The base file in full.
-            cache (dict): The symbols we discovered.
-        """
-
-        file_io.seek(0, 0)
-        h = hashlib.sha256(file_io.read()).hexdigest()
-        file_io.seek(0, 0)
-
-        this_cache_file = os.path.join(symbol_cache_path, h)
-        with open(this_cache_file, "w") as f:
-            f.write(json.dumps(cache))
-        
+        self._item = item
+        self.from_ip = None
+        self.from_module = None
+        self.to_ip = None
+        self.to_module = None
+        self.type = None
+        self.depth = None
 
-    def _load_symbols(self):
-        """Reads in the file for this module and attempts to extract the symbols."""
+        self._parse_item(item)
 
-        # Either we're loading everything or what we're looking at right now __should__ be loaded
-        if self._process._load_symbols is None or any(True for x in self._process._load_symbols if fnmatch(self.name, x)):
+    def _parse_item(self, item):
 
-            # Clear out old symbols if needed
-            self._process.modules._symbol_to_address[self.name] = {}
+        # Common
+        self.type = item['type']
+        self.from_ip = types.Pointer(common.auto_int(item['from_ip']))
+        self.from_module = item['from_module']
 
-            file_io = common.load_file(self._process, self.path)
-            cache = self._read_symbols_cache_dict(file_io)
+        if 'to_ip' in item:
+            self.to_ip = types.Pointer(common.auto_int(item['to_ip']))
 
-            if cache is not None:
-                return self._load_symbols_cache(cache)
+        if 'to_module' in item:
+            self.to_module = item['to_module']
 
-            if self._process.file_type == 'ELF':
-                self._load_symbols_elf(file_io)
+        if 'depth' in item:
+            self.depth = common.auto_int(item['depth'])
 
-            elif self._process.file_type == "PE":
-                self._load_symbols_pe(file_io)
+    def __str__(self):
+        s =  colored("{: <10}".format(self.type), attrs=['bold'])
+        from_ip = self.from_symbol or hex(self.from_ip)
 
-            # TODO: Windows
-            # TODO: Mac
+        s += "{: <55}".format(colored(self.from_module,"magenta") + ":" + colored(from_ip, 'magenta', attrs=['bold']))
 
-        # If we didn't resolve anything, make sure we noted we tried
-        if self.name not in self._process.modules._symbol_to_address:
-            self._process.modules._symbol_to_address[self.name] = {}
+        if self.to_ip is not None:
+            to_ip = self.to_symbol or hex(self.to_ip)
+            s += "-> "
+            s += "{: <55}".format(colored(self.to_module, "magenta") + ":" + colored(to_ip, "magenta", attrs=["bold"]))
 
-    def _load_symbols_pe(self, pe_io):
-        # TODO: Assuming that this process will work on any system running ELF...
-        print("Loading symbols for {} ... ".format(self.name), end='', flush=True)
+        if self.depth is not None:
+            s += str(self.depth)
 
-        pe = pefile.PE(data=pe_io.read())
-        cache = {'symbols': {}}
+        return s.strip()
 
-        # Some PEs don't export anything.
-        if hasattr(pe, "DIRECTORY_ENTRY_EXPORT"):
-            for sym in pe.DIRECTORY_ENTRY_EXPORT.symbols:
-                if sym.name in [b'', None]:
-                    continue
-
-                name = sym.name.decode()
-
-                rel_address = sym.address
-                # address = rel_address + self.base
+    def __repr__(self):
+        attrs = ["TraceItem"]
+        attrs.append(hex(self.from_ip))
+        attrs.append(self.type)
 
-                # self._process.modules._symbol_to_address[self.name][name] = types.Pointer(address)
-                # self._process.modules._address_to_symbol[address] = name
-                cache['symbols'][name] = rel_address
+        return "<{}>".format(' '.join(attrs))
 
-        self._save_symbols_cache(pe_io, cache)
-        self._load_symbols_cache(cache)
-        cprint("[ DONE ]", "green")
+    @property
+    def type(self):
+        return self.__type
 
-    def _load_symbols_elf(self, elf_io):
-        # TODO: Assuming that this process will work on any system running ELF...
-        print("Loading symbols for {} ... ".format(self.name), end='', flush=True)
+    @type.setter
+    def type(self, t):
+        assert isinstance(t, (str, type(None))), "Invalid type for type of {}".format(type(t))
 
-        if elf_io is None:
-            cprint("[ Failed to load ]", "yellow")
+        if t is None:
+            self.__type = None
             return
 
-        e = ELFFile(elf_io)
-
-        #
-        # Load up any symbols from the file
-        #
-
-        symtab = e.get_section_by_name('.symtab')
-        dynsym = e.get_section_by_name('.dynsym')
-
-        symbols = []
-        cache = {
-            'symbols': {},
-            'plt': []}
-
-        #
-        # Static Symbols
-        #
-
-        # Sometimes the binary won't have a symbol table
-        if symtab is not None:
-            symbols.append(symtab.iter_symbols())
-
-        if dynsym is not None:
-            symbols.append(dynsym.iter_symbols())
-
-        # Pull out symbols
-        for sym in itertools.chain(*symbols):
-            if sym.name == '':
-                continue
-
-            address = sym['st_value']
-            rel_address = address
+        t = t.lower()
 
-            if self.elf.type_str == 'DYN':
-                address = address + self.base
-
-            cache['symbols'][sym.name] = rel_address
-
-        #
-        # Section offsets
-        #
-
-        plt_section = e.get_section_by_name('.plt')
+        if t not in ['call', 'ret', 'exec', 'block', 'compile']:
+            logger.error("Unhandled traceitem type of {}".format(t))
+            logger.error(str(self._item))
+            return
 
-        if plt_section is not None:
+        self.__type = t
 
-            cache['plt_offset'] = plt_section.header.sh_offset
-            self.plt = cache['plt_offset']
+    @property
+    def from_symbol(self):
+        """Attempts to resolve from_ip into a symbol. If it can, it returns the symbol name. Otherwise it returns None."""
+        return self._process.modules.lookup_symbol(self.from_ip)
+        try:
+            #return self._process.modules._address_to_symbol[self.from_ip]
+            return self._process.modules._address_to_symbol[self.from_ip]
+        except KeyError:
+            return None
 
-            #
-            # PLT/GOT
-            #
+    @property
+    def to_symbol(self):
+        """Attempts to resolve to_ip into a symbol. If it can, it returns the symbol name. Otherwise it returns None."""
+        try:
+            return self._process.modules._address_to_symbol[self.to_ip]
+        except KeyError:
+            return None
 
-            rels = []
 
-            try:
-                rels.append(e.get_section_by_name('.rela.plt').iter_relocations())
-            except AttributeError:
-                pass
+class Trace(object):
+    """Keeps information about a Trace."""
+    
+    def __init__(self, process, tid, script, callback=None):
+        self._process = process
+        self._trace = []
+        self._tid = tid
+        self._script = script
+        self._callback = callback
+
+    def append(self, item):
+        ti = TraceItem(self._process, item)
+        self._trace.append(ti)
+
+        if self._callback is not None:
+            self._callback(self._tid, ti)
+
+    def stop(self):
+        """Stop tracing."""
+
+        if self._script is not None:
+            # TODO: Why the hell is Frida freezing on attempting to unload the stalker script?
+            # Must unfollow a Stalked thread in the SAME CONTEXT IT IS STALKING! Thus the RPC export here.
+            self._script[0].exports.unfollow()
+            # TODO: Add unload back in once it doesn't take forever for it to unload the script...
+            # Until then, calling unfollow and not unloading the script seems to be OK.
+            #time.sleep(1)
+            #self._script[0].unload()
+            self._process.tracer._active_instruction_traces.pop(self._tid)
+            self._script = None
+
+    def wait_for(self, address):
+        """Don't return until the given address is hit in the trace."""
+        address = self._process._resolve_location_string(address)
 
+        # TODO: Optimize this so I don't keep checking the same IPs over and over
+        while True:
             try:
-                rels.append(e.get_section_by_name('.rel.plt').iter_relocations())
-            except AttributeError:
-                pass
-
-            i = 1
-            for s in itertools.chain(*rels):
-                sym_name = dynsym.get_symbol(s.entry.r_info_sym).name
-                got_offset = s.entry.r_offset
+                next(x for x in self._trace if x.from_ip == address)
+                break
+            except StopIteration:
+                continue
+        
+    def __iter__(self):
+        return (x for x in self._trace)
 
-                if self.elf.type_str == 'DYN':
-                    got = self.base + got_offset
-                else:
-                    got = got_offset
+    def __len__(self):
+        return len(self._trace)
 
-                cache['plt'].append(sym_name)
-                cache['symbols']['got.' + sym_name] = got_offset
-                i += 1
+    def __str__(self):
+        return '\n'.join(str(i) for i in self)
 
-        else:
-            logger.warning("Could not find PLT for ELF '{}'".format(self.name))
+    def __repr__(self):
+        attr = ['Trace', 'Thread={}'.format(self._tid)]
+        attr += [str(len(self)), 'items']
 
-        self._save_symbols_cache(elf_io, cache)
-        self._load_symbols_cache(cache)
+        return "<{}>".format(' '.join(attr))
 
-        cprint("[ DONE ]", "green")
+    def __getitem__(self, item):
+        return self._trace.__getitem__(item)
 
-    def __repr__(self):
-        attrs = ['Module', self.name, '@', hex(self.base)]
-        return "<{}>".format(' '.join(attrs))
+class InstructionTracer(object):
 
-    def __eq__(self, other):
-        return self.name == other.name and self.base == other.base and self.path == other.path and self.size == other.size
+    def __init__(self, process, threads=None, from_modules=None, call=False,
+            ret=False, exec=False, block=False, compile=False, callback=None):
+        """
 
-    @property
-    def name(self):
-        """str: Module name."""
-        return self.__name
-
-    @name.setter
-    def name(self, name):
-        if type(name) is not str:
-            error = "Name must be string, not {}".format(type(name))
-            logger.error(error)
-            raise Exception(error)
+        Args:
+            process: Base process instantiation
+            threads (list, optional): What threads to trace. If None, it will trace all threads.
+            from_modules (list, optional): Restrict trace returns to those that start from one of the listed modules.
+            call (bool, optional): Trace calls
+            ret (bool, optional): Trace rets
+            exec (bool, optional): Trace all instructions
+            block (bool, optional): Trace blocks
+            compile (bool, optional): Trace on Frida instruction compile
+            callback (callable, optional): Callable to call with list of new
+                instructions as they come in. First arg will be the thread id.
+        """
 
-        self.__name = name
+        assert callable(callback) or callback is None, "Invalid type for callback of {}".format(type(callback))
 
-    @property
-    def base(self):
-        """int: Base address this module is loaded at."""
-        return self.__base
+        # Santiy check
+        if not any((call, ret, exec, block, compile)):
+            error = "You didn't select any action to trace!"
+            logger.error(error)
+            #raise Exception(error)
 
-    @base.setter
-    def base(self, base):
+        self._process = process
+        self.call= call
+        self.ret = ret
+        self.exec = exec
+        self.block = block
+        self.compile = compile
+        self.threads = threads
+        self._script = {}
+        self._from_modules = from_modules
+        self.callback = callback
+
+        # IMPORTANT: It's important to keep a local pointer to this trace. It's
+        # possible for trace messages to come in after officially stopping the
+        # trace. Using local dict in this way allows this trace to continue to
+        # get information while still being stopped.
+        self.traces = {}
 
-        base = common.auto_int(base)
+        self._start()
 
-        if type(base) is int:
-            base = types.Pointer(base)
+    def _on_message(self, m, d):
+        try:
+            payload = m['payload']
+        except:
+            print(m)
+            raise
+
+        for x in payload:
+            self.traces[x['tid']].append(x)
+
+    def _start(self):
+
+        replace = {
+            "FROM_MODULES_HERE": json.dumps([module.name for module in self._from_modules]),
+            "STALK_CALL": json.dumps(self.call),
+            "STALK_RET": json.dumps(self.ret),
+            "STALK_EXEC": json.dumps(self.exec),
+            "STALK_BLOCK": json.dumps(self.block),
+            "STALK_COMPILE": json.dumps(self.compile),
+        }
+
+        for thread in self.threads:
+            replace['THREAD_ID_HERE'] = str(thread.id)
+            self._process.run_script_generic("stalk.js", replace=replace, unload=False, on_message=self._on_message, runtime='v8')
+            self.traces[thread.id] = Trace(self._process, thread.id, self._process._scripts.pop(0), callback=self.callback)
+            self._process.tracer._active_instruction_traces[thread.id] = self.traces[thread.id]
 
-        self.__base = base
+    def __repr__(self):
+        attrs = ["InstructionTracer"]
+        attrs += [str(len(self.threads)), 'threads']
 
-    @property
-    def path(self):
-        """str: Module path."""
-        return self.__path
-
-    @path.setter
-    def path(self, path):
-        if type(path) is not str:
-            error = "Path must be string, not {}".format(type(path))
-            logger.error(error)
-            raise Exception(error)
+        return "<{}>".format(' '.join(attrs))
 
-        self.__path = path
+    def __iter__(self):
+        return self.traces.values().__iter__()
 
-        # Load up the symbols for this file if we haven't already
-        if self.name not in self._process.modules._symbol_to_address:
-            self._load_symbols()
+    def __str__(self):
+        table = PrettyTable(['tid', 'count'])
 
-    @property
-    def size(self):
-        """int: Size of this module."""
-        return self.__size
-
-    @size.setter
-    def size(self, size):
-        self.__size = common.auto_int(size)
+        for tid, trace in self.traces.items():
+            table.add_row([str(tid), str(len(trace))])
 
-    @property
-    def file(self):
-        """io.BufferReader: Opened file reader to a local copy of this module."""
-        return common.load_file(self._process, self.path)
+        return str(table)
 
     @property
-    def pe(self):
-        """Returns PE object, if applicable, otherwise None."""
+    def threads(self):
+        """list: Threads that are being traced by this object."""
+        return self.__threads
+
+    @threads.setter
+    def threads(self, threads):
+        assert isinstance(threads, (type(None), list, tuple, Thread)), "Invalid threads type of {}".format(type(threads))
 
-        if self._process.file_type != 'PE':
-            return
+        if threads is None:
+            threads = list(self._process.threads)
 
-        try:
-            return self.__pe
-        except AttributeError:
-            self.__pe = pefile.PE(self.file.name)
-            return self.__pe
+        if not isinstance(threads, (list, tuple)):
+            threads = [threads]
 
-    @property
-    def elf(self):
-        """Returns ELF object, if applicable, otherwise None."""
+        else:
+            threads_new = []
+            for thread in threads:
+                if isinstance(thread, Thread):
+                    threads_new.append(thread)
+                elif isinstance(thread, int):
+                    threads_new.append(self._process.threads[thread])
+                else:
+                    raise Exception("Unable to resolve requested thread of type {}".format(type(thread)))
 
-        if self._process.file_type != 'ELF':
-            return
+            threads = threads_new
 
-        try:
-            return self.__elf
-        except AttributeError:
-            self.__elf = ELF(self._process, self)
-            return self.__elf
+        # Make sure the threads aren't already being traced
+        for thread in threads:
+            if thread.id in self._process.tracer._active_instruction_traces:
+                error = "Cannot have more than one trace on the same thread at a time. Stop the existing trace with: process.threads[{}].trace.stop()".format(thread.id)
+                logger.error(error)
+                raise Exception(error)
 
-    @property
-    def symbols(self):
-        """dict: symbol name -> address for this binary."""
-        return self._process.modules._symbol_to_address[self.name]
+        self.__threads = threads
 
     @property
-    def plt(self):
-        """int: Location of PLT for this module. Returns None if not known."""
-        try:
-            return self.symbols['.plt']
-        except KeyError:
-            return None
+    def _from_modules(self):
+        """list,tuple,str,Module,None: What modules to restrict tracing from. Items can be strings (which will resolve) or Module objects."""
+        return self.__from_modules
 
-    @plt.setter
-    def plt(self, address):
+    @_from_modules.setter
+    def _from_modules(self, modules):
 
-        if self._process.file_type == "PE":
-            logger.warn("PLT is not valid for this file type.")
+        assert isinstance(modules, (list, tuple, type(None), str, Module)), "Unsupported type for from_modules of {}".format(type(modules))
+        
+        if modules is None:
+            self.__from_modules = []
             return
+        
+        if not isinstance(modules, (list, tuple)):
+            modules = [modules]
 
-        # Assuming plt needs to be rebased
-        #if self.elf is not None and self.elf.type_str == 'DYN':
-        address = address + self.base
-
-        self.symbols['.plt'] = address
-
+        new_modules = []
+        for module in modules:
+            if isinstance(module, Module):
+                new_modules.append(module)
+            elif isinstance(module, str):
+                new_modules.append(self._process.modules[module])
+            else:
+                error = "Unsupported type for module of {}".format(type(module))
+                logger.error(error)
+                raise Exception(error)
+        
+        self.__from_modules = new_modules
 
-from ..parsers import ELF
+from ..modules import Module
```

### Comparing `revenge-0.21/revenge/modules/modules.py` & `revenge-0.9/revenge/memory/memory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,251 +1,216 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
-import os
-import collections
 from prettytable import PrettyTable
-import datetime
-from fnmatch import fnmatch
-import time
+import binascii
+import operator
+import struct
+
+from .. import common
+from .. import types
 
-from .. import common, types
 
-class Modules(object):
+class Memory(object):
+    """Class to simplify getting and writing things to memory. Behaves like a list.
+    
+    Example:
+        - memory[0x12345].int8 -> Reads a signed 8-bit int from address
+        - memory[0x12345:0x12666] -> Returns byte array from memory
+    """
 
     def __init__(self, process):
         self._process = process
 
-        # key == module name, value == dict of symbol->address
-        self._symbol_to_address = {}
-
-        # key == address, value == symbol
-        self._address_to_symbol = {}
-
-        # key == symbol, value = address (resolved global symbols)
-        self._global_symbol_to_address = {}
-
-        self.__last_update = datetime.datetime(1970,1,1)
-
-    def lookup_offset(self, symbol):
-        """Lookup raw file offset to symbol.
-
-        Returns:
-            tuple: (module_name, offset) or None if cannot resolve
-
-        See examples from modules.lookup_symbol
+        # Keep track of where we've inserted breakpoints
+        # key == address of breakpoint, value == memory location to un-breakpoint it
+        self._active_breakpoints = {}
+
+        # Keep track of what we've allocated.
+        # key == address of allocation, value = script where we allocated it.
+        # NOTE: It's important to keep the script alive until we're done with the alloc or javascript might gc it.
+        self._allocated_memory = {}
+
+        # key == address of replaced function, value = tuple: what it's being replaced with, script so we can unload later
+        self._active_replacements = {}
+
+
+    def alloc(self, size):
+        """Allocate size bytes of memory and get a MemoryBytes object back to use it.
+    
+        Args:
+            size (int): How many bytes to allocate.
         """
+        
+        assert type(size) is int
 
-        # Resolve symbol
-        a = self._process.memory[symbol]
+        pointer = common.auto_int(self._process.run_script_generic("""var p = Memory.alloc(uint64('{}')); send(p);""".format(hex(size)), raw=True, unload=False)[0][0])
+        script = self._process._scripts.pop(0) # We want to hold on to it here
 
-        if a is None:
-            logger.error("lookup_offset: Cannot resolve '{}'.".format(symbol))
-            return
+        self._allocated_memory[pointer] = script
+        return MemoryBytes(self._process, pointer, pointer+size)
 
-        m = self[a.address]
+    def alloc_string(self, s, encoding='latin-1'):
+        """Short-hand to run alloc of appropriate size, then write in the string.
+        
+        Args:
+            s (bytes, str): String to allocate
+            encoding (str, optional): How to encode the string if passed in as type str.
+        """
 
-        if m is None:
-            return None
+        # TODO: Smart guess encoding, linux is usually utf-8, Windows has function call to determine utf-8 vs 16. Mac...?
 
-        return (m.name, a.address - m.base)
+        if type(s) in [types.StringUTF8, types.StringUTF16]:
+            if s.type == 'utf8':
+                encoding = 'utf-8'
+            elif s.type == 'utf16':
+                encoding = 'utf-16'
+            else:
+                logger.error('How did i get here??')
+                return
 
-    def lookup_symbol(self, symbol):
-        """Generically resolve a symbol.
+            s = str(s)
         
-        Examples:
-            resolve_symbol(":strlen") -> returns address of strlen resolved globally.
-            resolve_symbol("strlen") -> equivalent to above
-            resolve_symbol("strlen+0xf") -> strlen offset by 0xf
-            resolve_symbol("a.out:main") -> returns address of main resolved to a.out.
-            resolve_symbol(0x12345) -> returns symbol at that address.
+        if type(s) is str:
+            s = s.encode(encoding)
+            if encoding == 'utf-16':
+                s = s[2:] # Remove BOM
+                s += b'\x00' # Extra null at end of utf-16
         
-        """
-
-        # Resolve address to symbol
-        if isinstance(symbol, int):
-            try:
-                return self._address_to_symbol[symbol]
-            except KeyError:
-                return None
-
-        module, offset, symbol = common.parse_location_string(symbol)
-
-        # Check the caches first
-        if module != "":
-            # First try to resolve with local symbol table
-            try:
-                return self._symbol_to_address[module][symbol] + int(offset, 16)
-            except KeyError:
-                pass
 
-        else:
-            try:
-                return self._global_symbol_to_address[symbol] + int(offset, 16)
-            except KeyError:
-                pass
+        if type(s) is not bytes:
+            logger.error("Invalid string type of {}".format(type(s)))
+            return None
         
-        # Fall back to asking Frida to resolve it
+        # Null terminate
+        s += b'\x00'
 
-        replace_vars = {
-                "FUNCTION_SYMBOL_HERE": symbol,
-                "FUNCTION_MODULE_HERE": module,
-                "FUNCTION_OFFSET_HERE": offset,
-                }
+        mem = self.alloc(len(s))
+        mem.bytes = s
+        return mem
 
-        location_resolved = self._process.engine.run_script_generic("resolve_location_address.js", replace=replace_vars, unload=True)[0]
+    def find(self, *args, **kwargs):
+        """Search for thing in memory. Must be one of the defined types."""
+        return MemoryFind(self._process, *args, **kwargs)
 
-        if location_resolved == []:
-            raise RevengeSymbolLookupFailure("Cannot resolve symbol.")
+    def describe_address(self, address):
+        """Takes in address and attempts to return a better description of what's there."""
 
-        location_resolved = common.auto_int(location_resolved[0])
+        assert isinstance(address, int)
 
-        # Update the caches, but only with the base symbol, not with offset
-        if module == "":
-            self._global_symbol_to_address[symbol] = location_resolved - int(offset,16)
+        desc = ""
+        module = self._process.modules[address]
 
-        return types.Pointer(location_resolved)
+        if module is not None:
+            desc += module.name
 
-    @common.validate_argument_types(library=str)
-    def load_library(self, library):
-        """Dynamically load a library into the program.
+            try:
+                # If we can find a closest function, use that.
+                func_name, func_addr = next((name, addr) for name,addr in sorted(module.symbols.items(), key=operator.itemgetter(1),reverse=True) if address >= addr)
+                desc += ":" + func_name
+                offset = address - func_addr
+
+            except StopIteration:
+                # We did not find a closest function, just offset from module base
+                offset = address - module.base
 
-        Args:
-            library (str): The full path to the library on the process machine
+            if offset != 0:
+                desc += "+" + hex(offset)
 
-        Returns:
-            revenge.modules.Module: RetuRns the new loaded module or None on error.
+        else:
+            desc += hex(address)
 
-        Examples:
-            .. code-block:: python3
+        return desc
 
-                selinux = process.modules.load_library("/lib/x86_64-linux-gnu/libselinux.so.1")
+    def _type_to_search_string(self, thing):
+        """Converts the given object into something relevant that can be fed into a memory search query."""
 
-        This will eventually be implemented across all platforms. For now,
-        it only works on linux platforms.
-        """
+        if not isinstance(thing, types.all_types):
+            logger.error("Please use valid type.")
+            return None
 
-        def load_linux(self, library):
+        endian_str = "<" if self._process.endianness == 'little' else '>'
 
-            dlopen = self._process.memory[':dlopen']
-            dlopen.argument_types = types.Pointer, types.Int32
-            
-            if dlopen is None:
-                logger.error("Unable to locate dlopen. Cannot dynamically load.")
-                return
+        if isinstance(thing, types.StringUTF8):
+            # Normal string
+            return binascii.hexlify(thing.encode('utf-8')).decode()
 
-            # Assuming non-lazy load and exporting symbols for now.
-            out = dlopen(library, 0x102)
+        elif isinstance(thing, types.StringUTF16):
+            # Wide Char String (Windows/UTF16)
+            return binascii.hexlify(thing.encode('utf-16')[2:]).decode()
 
-            # dlopen is reporting an error
-            if out == 0:
-                return False
+        elif isinstance(thing, types.UInt8):
+            return binascii.hexlify(struct.pack(endian_str + "B", thing)).decode()
 
-            self._flush_cache()
-            return self[os.path.basename(library)]
+        elif isinstance(thing, types.Int8):
+            return binascii.hexlify(struct.pack(endian_str + "b", thing)).decode()
 
-        if self._process.device_platform == "linux":
-            return load_linux(self, library)
+        elif isinstance(thing, types.UInt16):
+            return binascii.hexlify(struct.pack(endian_str + "H", thing)).decode()
 
-        else:
-            logger.error("Not yet supported platform for load_library: {}".format(self._process.device_platform))
+        elif isinstance(thing, types.Int16):
+            return binascii.hexlify(struct.pack(endian_str + "h", thing)).decode()
 
-    @common.validate_argument_types(name=str)
-    def _register_plugin(self, plugin, name):
-        """Registers this plugin to be exposed as a module plugin.
+        elif isinstance(thing, types.UInt32):
+            return binascii.hexlify(struct.pack(endian_str + "I", thing)).decode()
 
-        Args:
-            plugin (callable): A class constructor. Must take an argument for
-                the current module
-            name (str): What will this be called?
-        
-        The plugin will be instantiated at most once per module instance, and
-        done only when referenced.
-
-        Examples:
-            .. code-block:: python
-
-                class MyPlugin:
-                    @classmethod
-                    def _modules_plugin(klass, module):
-                        self = klass()
-                        self._module = module
-                        return self
+        elif isinstance(thing, types.Int32):
+            return binascii.hexlify(struct.pack(endian_str + "i", thing)).decode()
 
-                process.modules._register_plugin(MyPlugin._modules_plugin, "myplugin")
+        elif isinstance(thing, types.UInt64):
+            return binascii.hexlify(struct.pack(endian_str + "Q", thing)).decode()
 
-                # This first call will instantiate the plugin
-                process.modules['proc_name'].myplugin
-        """
+        elif isinstance(thing, types.Int64):
+            return binascii.hexlify(struct.pack(endian_str + "q", thing)).decode()
+        
+        else:
+            logger.error("Unexpected type to convert of {}".format(type(thing)))
+            return None
+        
 
-        def getter(self):
-            try:
-                return getattr(self, "__" + name)
-            except AttributeError:
-                setattr(self, "__" + name, plugin(self))
-                return getattr(self, "__" + name)
+    def __getitem__(self, item):
 
-        if not callable(plugin): raise RevengeInvalidArgumentType("plugin must be callable")
+        if type(item) == str:
+            # Assume it's something we need to resolve
+            item = self._process._resolve_location_string(item)
 
-        if name in Module.__dict__:
-            raise RevengeModulePluginAlreadyRegistered("Property name " + name + " is already taken.")
+        if isinstance(item, int):
+            return MemoryBytes(self._process, item)
 
-        # Add the new plugin
-        setattr(Module, name, property(getter, doc=plugin.__doc__))
+        elif type(item) == slice:
 
-    def _flush_cache(self):
-        """Make sure the next time we're hit is a full one."""
-        self.__last_update = datetime.datetime(1970, 1, 1)
+            if item.start is None or item.stop is None or item.step is not None:
+                logger.error("Memory slices must have start and stop and not contain a step option.")
+                return
 
-    def __iter__(self):
-        return self.modules.__iter__()
+            return MemoryBytes(self._process, item.start, item.stop)
 
-    def __len__(self):
-        return len(self.modules)
+        logger.error("Unhandled memory type of {}".format(type(item)))
 
-    def __repr__(self):
-        attrs = ['Modules', str(len(self))]
-        return "<{}>".format(' '.join(attrs))
+    @property
+    def maps(self):
+        """Return a list of memory ranges that are currently allocated."""
+        return MemoryMap(self._process)
 
     def __str__(self):
-        table = PrettyTable(['name', 'base', 'size', 'path'])
-
-        for module in self:
-            table.add_row([module.name, hex(module.base), hex(module.size), module.path])
-
-        table.align['path'] = 'l'
+        
+        table = PrettyTable(['range', 'prot', 'file'])
+        table.header = False
+        table.align = 'l'
+        table.border = False
+
+        for range in self.maps:
+            table.add_row([
+                hex(range.base)[2:] + '-' + hex(range.base+range.size)[2:],
+                range.protection,
+                range.file or '',
+                ])
 
         return str(table)
 
-    def __getitem__(self, item):
-
-        # Resolve module by it's name
-        if isinstance(item, str):
-            return next(mod for mod in self if fnmatch(mod.name, item))
-
-        if isinstance(item, types.Telescope):
-            item = int(item)
-
-        # Resolve module by the address
-        if isinstance(item, int):
-            for mod in self:
-                if item >= mod.base and item <= mod.base + mod.size:
-                    return mod
-            return None
-
-        raise NotImplementedError
-
-    @property
-    def modules(self):
-        """list: Return list of modules."""
-
-        # Time to update the cache
-        if datetime.datetime.now() - self.__last_update > datetime.timedelta(seconds=0.5):
-            mods = self._process.engine.run_script_generic("""send(Process.enumerateModulesSync());""", raw=True, unload=True)[0][0]
-            self.__modules = [Module(self._process, name=mod['name'], base=mod['base'], size=mod['size'], path=mod['path']) for mod in mods]
-            self.__last_update = datetime.datetime.now()
-
-        return self.__modules
+from . import MemoryBytes
+from . import MemoryRange
+from . import MemoryFind
+from . import MemoryMap
 
-from .module import Module
-from ..exceptions import *
+Memory.find.__doc__ = MemoryFind.__init__.__doc__
```

### Comparing `revenge-0.21/revenge/native_exception.py` & `revenge-0.9/revenge/native_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from . import Colorer
 import logging
 
 logger = logging.getLogger(__name__)
 
-import typing
+import frida
 import colorama
 colorama.init()
 
 import os
 from termcolor import cprint, colored
 from prettytable import PrettyTable
 
@@ -29,15 +29,15 @@
              'breakpoint', 'system']
 
     def __init__(self, context, backtrace=None, type=None,
             memory_operation=None, memory_address=None):
         """Represent a native CPU exception.
         
         Args:
-            context: revenge cpu context
+            context: Frida-util cpu context
             backtrace: native backtrace object
             type (str): What type of exception is this.
             memory_operation (str, optional): Type of memory operation
                 (read/write/execute)
             memory_address (int, optional): Address that was accessed when
                 exception occurred.
         """
@@ -91,15 +91,15 @@
 
     @property
     def _process(self):
         return self.context._process
 
     @property
     def type(self):
-        """str: What type of native exception? One of """
+        """str: What type of native exception? See NativeException.TYPES"""
         return self.__type
 
     @type.setter
     def type(self, type):
         type = type.lower()
         assert type in NativeException.TYPES, 'Unexpected native exception type of {}'.format(type)
         self.__type = type
@@ -131,11 +131,9 @@
 
         if isinstance(memory_operation, str):
             memory_operation = memory_operation.lower()
         assert memory_operation in ['read', 'write', 'execute', None], "Unexpected memory_operation of '{}'".format(memory_operation)
         
         self.__memory_operation = memory_operation
 
-from .cpu import CPUContext
+from .tracer.contexts import Context as CPUContext
 from . import common
-
-NativeException.type.__doc__ += ', '.join(NativeException.TYPES)
```

### Comparing `revenge-0.21/revenge/parsers/elf/elf.py` & `revenge-0.9/revenge/parsers/elf/elf.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/parsers/elf/program_header.py` & `revenge-0.9/revenge/parsers/elf/program_header.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/parsers/elf/program_headers.py` & `revenge-0.9/revenge/parsers/elf/program_headers.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/parsers/elf/section_header.py` & `revenge-0.9/revenge/parsers/elf/section_header.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/parsers/elf/section_headers.py` & `revenge-0.9/revenge/parsers/elf/section_headers.py`

 * *Files identical despite different names*

### Comparing `revenge-0.21/revenge/plugins/java/classes.py` & `revenge-0.9/revenge/java/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 from fnmatch import fnmatch
-from ... import common
 
 class JavaClasses(object):
 
     def __init__(self, process):
         """Handles enumerating the loaded Java classes for this JVM."""
         self._process = process
 
@@ -19,26 +18,31 @@
         return self.classes.__iter__()
 
     def __len__(self):
         return len(self.classes)
 
     def __getitem__(self, item):
         if isinstance(item, int):
-            return self._process.engine.plugins.java.JavaClass(self._process, list(self)[item])
+            return JavaClass(self._process, list(self)[item])
 
         elif isinstance(item, str):
-            match = [self._process.engine.plugins.java.JavaClass(self._process, x) for x in self if fnmatch(x, item)]
+            match = [JavaClass(self._process, x) for x in self if fnmatch(x, item)]
             if len(match) > 1:
                 return match
             if match == []:
                 return None
             return match[0]
 
         else:
             logger.error("Unhandled item get of type {}".format(type(item)))
             return
 
     @property
-    @common.implement_in_engine()
     def classes(self):
         """list: The actual list of classes."""
-        pass
+        try:
+            return self.__classes
+        except AttributeError:
+            self.__classes = self._process.java.run_script_generic(r"""send( Java.enumerateLoadedClassesSync() );""", raw=True, unload=True)[0][0]
+            return self.__classes
+
+from .java_class import JavaClass
```

### Comparing `revenge-0.21/revenge/process.py` & `revenge-0.9/revenge/process.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,366 +6,496 @@
 logger = logging.getLogger(__name__)
 
 import frida
 import colorama
 colorama.init()
 
 import os
-import sys
 from termcolor import cprint, colored
 from prettytable import PrettyTable
 import time
 
 import atexit
 import signal
 import json
 import pprint
-import collections
-
-import importlib
-from . import common
+from copy import copy
 
 here = os.path.dirname(os.path.abspath(__file__))
 
-
 class Process(object):
 
     def __init__(self, target, resume=False, verbose=False, load_symbols=None,
-                 envp=None, engine=None, ignore_exceptions=False):
-        """Represents a process.
+            device=None):
+        """
 
         Args:
-            target (str, int, list): File name or pid to attach to. If target
-                is a list, it will be set as argv.
+            target (str, int): File name or pid to attach to.
             resume (bool, optional): Resume the binary if need be after loading?
             verbose (bool, optional): Enable verbose logging
             load_symbols (list, optional): Only load symbols from those modules
                 in the list. Saves some startup time. Can use glob ('libc*')
-            envp (dict, optional): Specify what you want the environment
-                pointer list to look like. Defaults to whatever the current
-                envp is.
-            engine (revenge.engines.Engine): Instantiated Engine for this
-                process
-            ignore_exceptions (bool): Should we not attempt to generically
-                catch process exceptions? Default is False.
-
-        Examples:
-            .. code-block:: python3
-
-                # Kick off ls
-                p = revenge.Process("/bin/ls")
-
-                # Kick off ls for /tmp with custom environment
-                p = revenge.Process(["/bin/ls","/tmp/"], envp={'var1':'thing1'})
-
-                #
-                # Interaction
-                #
-
-                # Write to stdin
-                p.stdin(b"hello\n")
-
-                # Read from stdout
-                p.stdout(16)
-
-                # Read up to expected output in stdout
-                p.stdout("expected")
-
-                # Interact like a shell
-                p.interactive()
+            device (revenge.device_types.*, optional): Define what device
+                to connect to.
         """
 
-        self.__engine = engine
+        # Just variable to ensure we don't garbage collect
+        self._scripts = []
+        # Cache common module addrs
+        self._module_by_addr_cache = {}
+        self.session = None
         self.__file_name = None
         self.__file_type = None
         self.__entrypoint = None
         self._resume_addr = None
         self.__endianness = None
         self.__bits = None
         self._spawn_target = None
         self.verbose = verbose
-        self._envp = envp
+        self.device = device or device_types.LocalDevice()
         self.target = target
-        self._ignore_exceptions = ignore_exceptions
-        self._registered_cleanup = []
 
         if not isinstance(load_symbols, (list, type, type(None))):
             load_symbols = [load_symbols]
         self._load_symbols = load_symbols
 
-        # self.memory = self.engine.memory.Memory(self)
-        self.memory = self.engine.memory
+        self.memory = Memory(self)
         self.threads = Threads(self)
+        self.tracer = Tracer(self)
         self.modules = Modules(self)
-        self.techniques = Techniques(self)
 
         atexit.register(self._at_exit)
-        self.engine.start_session()
-        self._register_plugins()
+        self.start_session()
 
-        # Cache arch right away so we don't have resource locks
-        self.arch
+        if self.run_script_generic(r"""send(Java.available)""", raw=True, unload=True)[0][0]:
+            self.java = Java(self)
 
-        # TODO: move this into frida engine
         # ELF binaries start up in ptrace, which causes some issues, shim at entrypoint so we can remove ptrace
         if self._spawned_pid is not None and self.file_type == 'ELF':
 
-            # Set breakpoint at entry -- Frida changed how it resumes... So can't use entry breakpoint anymore
-            # self.memory[self.entrypoint].breakpoint = True
+            # Set breakpoint at entry
+            self.memory[self.entrypoint_rebased].breakpoint = True
 
             # Set breakpoints at exit calls
             for c in [':exit', ':_exit']:
                 self.memory[c].breakpoint = True
 
-            # Resume to remove ptrace -- Frida changed how it resumes... So can't use entry breakpoint anymore
-            #self.engine.resume(self._spawned_pid)
+            # Resume to remove ptrace
+            self.device.device.resume(self._spawned_pid)
 
-        if self.device.platform == "windows":
-            # Set exit breakpoints
-            for c in ['msvcrt.dll:exit', 'msvcrt.dll:_exit']:
-                self.memory[c].breakpoint = True
+            #time.sleep(0.2)
 
         if self.device_platform == 'linux':
             try:
                 str(self.threads)
             except IndexError:
                 logger.error("Can't enumerate threads. Please check sysctl kernel.yama.ptrace_scope=0 or run as root.")
 
-        """ Handle this at each engine level, not here.
         # Resume file if need be
         if resume:
-            # If we are using a resume variable
-            if self.memory[self.entrypoint].breakpoint:
-                self.memory[self.entrypoint].breakpoint = False
 
+            # If we are using a resume variable
+            if self.memory[self.entrypoint_rebased].breakpoint:
+                self.memory[self.entrypoint_rebased].breakpoint = False
+            
             else:
-                self.engine.resume(self._spawned_pid)
-        """
+                self.device.device.resume(self._spawned_pid)
+
+
+    def pause_at(self, location):
+        """Pause at a given point in execution."""
 
-    def _register_plugins(self):
-        """Figures out which plugins to load and loads them."""
+        pause_location = self._resolve_location_string(location)
+        self.run_script_generic('pause_at2.js', replace={"FUNCTION_ADDRESS_HERE": hex(pause_location)})
+        
+    def _at_exit(self):
+        """Called to clean-up at exit."""
+
+        # TODO: Remove this once pytest fixes their at_exit issue
+        logging.getLogger().setLevel(logging.WARN)
 
-        for plugin_name in dir(self.engine.plugins):
-            if plugin_name.startswith("_"):
-                continue
+        try:
+
+            # Remove breakpoints
+            for addr in copy(self.memory._active_breakpoints):
+                logger.debug("Removing breakpoint: " + hex(addr))
+                self.memory[addr].breakpoint = False
+
+            # Remove function replacements
+            for addr in self.memory._active_replacements:
+                self.memory[addr].replace = None
+
+            # Remove any instruction traces
+            for t in self.threads:
+                if t.trace is not None:
+                    t.trace.stop()
+
+            self.run_script_generic("""Interceptor.detachAll()""", raw=True, unload=True)
+
+            # Unallocate our memory
+            for addr in copy(self.memory._allocated_memory):
+                logger.debug("Unallocating memory: " + hex(addr))
+                self.memory[addr].free()
+
+            # Unload our scripts
+            for script, text in self._scripts:
+                logger.debug("Unloading Script: %s", text)
+
+                try:
+                    script.unload()
+                except frida.InvalidOperationError:
+                    # Already unloaded probably
+                    pass
+
+            logger.debug("Done unloading")
+
+        except (frida.InvalidOperationError, frida.TransportError) as e:
+            # Looks like the program terminated. Possibly finished execution before we finished cleanup.
+            if 'detached' in e.args[0] or 'closed' in e.args[0]:
+                return
 
-            plugin_mod = getattr(self.engine.plugins, plugin_name)
+        # If we spawned it, kill it
+        try:
+            if self._spawned_pid is not None:
+                return self.device.device.kill(self._spawned_pid)
 
-            for item, value in plugin_mod.__dict__.items():
+        except (frida.PermissionDeniedError, frida.ProcessNotFoundError) as e:
+            # This can indicate the process is already dead.
+            try:
+                next(x for x in self.device.device.enumerate_processes() if x.pid == self._spawned_pid)
+                logger.error("Device kill permission error, with process apparently %d still alive.", self._spawned_pid)
+                raise e
+            except StopIteration:
+                return
+
+        # Unload anything we loaded first
+        #for script in self._scripts:
+        #    script.unload()
 
-                if inspect.isclass(value) and issubclass(value, Plugin):
+        try:
 
-                    # Instantiate the plugin
-                    plugin = value(self)
+            # Genericall unstalk everything
+            for thread in self.threads:
+                if thread.trace is not None:
+                    thread.trace.stop()
+                #self.run_script_generic("Stalker.unfollow({tid})".format(tid=thread.id), raw=True, unload=True)
+        
+        except frida.InvalidOperationError:
+            # Session is already detached.
+            pass
 
-                    if plugin._is_valid:
-                        setattr(self, item.lower(), plugin)
+        # Detach our session
+        self.session.detach()
 
-    def quit(self):
-        """Call to quit your session without exiting. Do NOT continue to use this object after.
+    
+    #######################
+    # On Message Handlers #
+    #######################
 
-        If you spawned the process, it will be killed. If you attached to the
-        process, frida will be cleaned out, detatched, and the process should
-        continue normally.
-        """
-        for c in self._registered_cleanup:
-            c()
-        self._at_exit()
-
-    def resume(self):
-        """Resume execution of any current breakpoint hit or suspended thread."""
-        raise NotImplementedError("resume has not been implemented yet in this backend.")
+    def on_message(self, message, data=None):
+        """Generic on message handler."""
+        print("Caught message", message, data)
 
-    def _register_cleanup(self, c):
-        self._registered_cleanup.append(c)
 
-    def _at_exit(self):
-        """Called to clean-up at exit."""
-        self.engine._at_exit()
+    def start_session(self):
+
+        self._spawned_pid = None
+
+        if self._spawn_target is not None:
+            print("Spawning file\t\t\t... ", end='', flush=True)
+            self._spawned_pid = self.device.device.spawn(self._spawn_target)
+            cprint("[ DONE ]", "green")
+
+        print('Attaching to the session\t... ', end='', flush=True)
+
+        try:
+            # Default attach to what we just spawned
+            self.session = self.device.device.attach(self._spawned_pid or self.target)
+        except frida.ProcessNotFoundError:
+            logger.error('Could not find that target process to attach to!')
+            exit(1)
+
+        print(colorama.Fore.GREEN + '[ DONE ]' + colorama.Style.RESET_ALL)
 
     def target_type(self, x):
         # Maybe it's PID
         try:
             return int(x)
 
         # Probably process name
-        except Exception:
+        except:
             return x
 
-    @common.implement_in_engine()
-    def stdout(self, n):
-        """Read n bytes from stdout.
+    def load_js(self, name):
+        with open(os.path.join(here, "js", name), "r") as f:
+            return f.read().strip()
 
-        Args:
-            n (int, str, bytes): Number of bytes to read or string to expect.
-                If no value is given, it's presumed you are trying to read
-                all currently queued output.
+    def get_module_by_addr(self, addr):
 
-        Returns:
-            bytes: Output of stdout
-        """
-        pass
+        addr = common.auto_int(addr)
 
-    @common.implement_in_engine()
-    def stderr(self, n):
-        """Read n bytes from stderr.
+        try:
+            return self._module_by_addr_cache[addr]
+        except:
+            pass
 
+        for module in self.modules:
+            base = module.base
+            size = module.size
+
+            if addr >= base and addr <= base+size:
+                self._module_by_addr_cache[addr] = module.name # Add to cache
+                return module.name
+
+        return None
+
+    def run_script_generic(self, script_name, raw=False, replace=None,
+            unload=False, runtime='duk', on_message=None, timeout=None,
+            context=None, onComplete=None):
+        """Run scripts that don't require anything special.
+        
         Args:
-            n (int, str, bytes): Number of bytes to read or string to expect.
-                If no value is given, it's presumed you are trying to read
-                all currently queued output.
+            script_name (str): What script to load from the js directory
+            raw (bool, optional): Should the script_name actually be considered
+                the script contents?
+            replace (dict, optional): Replace key strings from dictionary with
+                value into script.
+            unload (bool, optional): Auto unload the script. Set to true if the
+                script is fully synchronous.
+            runtime (str, optional): Runtime to use for this script, either
+                'duk' or 'v8'.
+            on_message(callable, optional): Set the on_message handler to this
+                instead.
+            timeout (int, optional): Modify timeout (default is 60 seconds).
+                Note, this will cause the script to run async. 0 == no timeout
+            context (Context, optional): Execute this script under a given
+                context.
+            onComplete (str, optional): If defined, this method will pause
+                until the given onComplete string is returned. Basically
+                allowing run_script_generic to return all things from an async
+                script.
 
         Returns:
-            bytes: Output of stderr
+            tuple: msg, data return from the script
         """
-        pass
 
-    @common.implement_in_engine()
-    def stdin(self, thing):
-        """Write thing to stdin.
 
-        Args:
-            thing (str, bytes): If str, it will be encoded as latin-1.
+        msg = []
+        data = []
 
-        Note: There's no newline auto appended. Remember to add one if you want it.
-        """
-        pass
+        # HACK: Using list for completed to make passing data back from async
+        # function simpler.
+        completed = [] # For use with async scripts
+
+        if not on_message is None and not callable(on_message):
+            logger.error('on_message handler must be callable.')
+            return None
+
+        def on_msg(m, d):
+
+            if m['type'] == 'error':
+                logger.error("Script Run Error: " + pprint.pformat(m['description']))
+                logger.debug(pprint.pformat(m))
+                return
+            
+            # Async is done
+            if onComplete is not None and m['payload'] == onComplete:
+                completed.append(True)
+                return
+
+            logger.debug("on_message: {}".format([m,d]))
+
+            msg.append(m['payload'] if 'payload' in m else None)
+            data.append(d)
+
+        on_message = on_msg if on_message is None else on_message
+
+        if not raw:
+            js = self.load_js(script_name)
+        else:
+            js = script_name
+
+        if replace is not None:
+            assert type(replace) == dict, "Unexpected replace type of {}".format(type(replace))
 
-    @common.implement_in_engine()
-    def interactive(self):
-        """Go interactive. Return back to your shell with ctrl-c."""
-        pass
+            for key, value in replace.items():
+                js = js.replace(key, value)
+
+        if timeout is not None:
+            js = "setTimeout(function() {" + js + "}," + str(timeout) + ")"
+            # Forcing unload to false since we don't know if it's done.
+            unload = False
+
+        # Let context decide when to run this.
+        if context is not None:
+            # Processing is done, let context know.
+            return context.run_script_generic(script_name)
+
+        logger.debug("Running script: %s", js)
+
+        script = self.session.create_script(js, runtime=runtime)
+
+        script.on('message', on_message)
+
+        try:
+            script.load()
+        except:
+            logger.error("Error running script!")
+            script.unload()
+            return
+
+        # If we're async, wait until we're done
+        # This needs to happen before unlink so we ensure we get all messages
+        while onComplete is not None and completed == []:
+            time.sleep(0.01)
+        
+        if unload:
+            script.unload()
+        else:
+            # Inserting instead of appending since earlier scripts need to be unloaded later
+            self._scripts.insert(0, [script, js])
+
+
+        return msg, data
+
+    def _resolve_location_string(self, location):
+        """Take location string and resolve it into an integer address."""
+        #assert type(location) is str, "Invalid call to resolve_location_string with type {}".format(type(location))
+        if isinstance(location, int):
+            return types.Pointer(location)
+
+        return self.modules.lookup_symbol(location)
 
     def __repr__(self):
         attrs = ['Process', self.file_name + ":" + str(self.pid)]
         return '<' + ' '.join(attrs) + '>'
 
     ############
     # Property #
     ############
 
     @property
-    def argv(self):
-        """list: argv for this process instantitation."""
-        return self.__argv
-
-    @argv.setter
-    @common.validate_argument_types(argv=(list, tuple))
-    def argv(self, argv):
-        self.__argv = argv
-
-    @property
     def device_platform(self):
         """Wrapper to discover the device's platform."""
 
-        self.device_platform = self.engine.run_script_generic(r"send(Process.platform)", raw=True, unload=True)[0][0]
+        def message(x, y):
+            self.device_platform = x['payload']
+
+        try:
+            return self.__device_platform
+        except:
+            pass
+
+        js = "send(Process.platform)"
+        script = self.session.create_script(js)
+        script.on('message', message)
+        script.load()
         return self.__device_platform
 
     @device_platform.setter
     def device_platform(self, platform):
         self.__device_platform = platform
 
     @property
     def pid(self):
-        return self.engine.session._impl.pid
+        return self.session._impl.pid
+
+    @property
+    def entrypoint_rebased(self):
+        """Entrypoint as it exists in the current rebased program."""
+        mod = self.modules[self.file_name]
+
+        if self.file_type == 'ELF':
+            if mod.elf.type_str == 'DYN':
+                return types.Pointer(self.entrypoint + mod.base)
+
+        # TODO: Windows?
+        # TODO: Mac?
+
+        return self.entrypoint
 
     @property
     def entrypoint(self):
         """int: Returns the entrypoint for this running program."""
-        mod = self.modules[self.file_name]
 
         if self.__entrypoint is None:
             if self.file_type == 'ELF':
-                self.__entrypoint = self.memory[mod.base + 0x18].pointer
-
-                if mod.elf.type_str == 'DYN':
-                    self.__entrypoint = self.__entrypoint + mod.base
-
-            elif self.file_type == "PE":
-                me = self.modules[self.file_name]
-                self.__entrypoint = me.base + me.pe.OPTIONAL_HEADER.AddressOfEntryPoint
+                self.__entrypoint = int(self.run_script_generic("""send(Memory.readPointer(ptr(Number(Process.getModuleByName('{}').base) + 0x18)))""".format(self.file_name), raw=True, unload=True)[0][0],16)
 
             else:
                 logger.warn('entrypoint not implemented for file of type {}'.format(self.file_type))
                 return None
-
-        # TODO: Mac?
-
+            
         return self.__entrypoint
 
     @property
     def endianness(self):
         """Determine which endianness this binary is. (little, big)"""
 
-        if self.__endianness is not None:
+        if self.__endianness != None:
             return self.__endianness
 
         if self.device_platform == 'windows':
             # TODO: Technically assumption, but like 99% of the time it's right.
             self.__endianness = 'little'
 
         elif self.file_type == 'ELF':
-            endianness = self.engine.run_script_generic("""send(ptr(Number(Process.enumerateModulesSync()[0].base) + 5).readS8())""", raw=True, unload=True)[0][0]
+            endianness = self.run_script_generic("""send(ptr(Number(Process.enumerateModulesSync()[0].base) + 5).readS8())""", raw=True, unload=True)[0][0]
             self.__endianness = 'little' if endianness == 1 else 'big'
 
         else:
             logger.warn("Unhandled endianness check for ({}, {}), assuming little".format(self.file_type, self.device_platform))
 
         return self.__endianness
 
     @property
     def file_type(self):
         """Guesses the file type."""
 
         # TODO: Android processes we attach to can't getModuleByName for their file name...
         # Maybe use "app_process64" instead... Or resolve the first module and go with that..
-        if isinstance(self.device, devices.AndroidDevice):
+        if isinstance(self.device, device_types.AndroidDevice):
             return "ELF"
 
         # TODO: Update this with other formats. PE/COFF/MACHO/etc
         if self.__file_type is None:
-            # Sometimes the file name and module name differ (such as /bin/sh -> dash)
-            # To handle this, we're assuming the core module will always come back first
-            # in the list.
-            me = list(self.modules)[0]
-            b = self.memory[me.base:me.base + 16].bytes
-            if b.startswith(b'\x7fELF'):
+            if self.run_script_generic("""send('bytes', Process.getModuleByName('{}').base.readByteArray(4))""".format(self.file_name), raw=True, unload=True)[1][0] == b'\x7fELF':
                 self.__file_type = 'ELF'
-            elif b.startswith(b'MZ'):
+            elif self.run_script_generic("""send('bytes', Process.getModuleByName('{}').base.readByteArray(2))""".format(self.file_name), raw=True, unload=True)[1][0] == b'MZ':
                 self.__file_type = "PE"
             else:
                 self.__file_type = 'Unknown'
 
         return self.__file_type
 
     @property
     def file_name(self):
-        """str: The base file name."""
+        """The base file name."""
         # TODO: This assumes the base module is always first...
         if self.__file_name is None:
-            self.__file_name = self.engine.run_script_generic("""send(Process.enumerateModulesSync())""", raw=True, unload=True)[0][0][0]['name']
+            self.__file_name = self.run_script_generic("""send(Process.enumerateModulesSync())""", raw=True, unload=True)[0][0][0]['name']
 
         return self.__file_name
 
     @property
     def bits(self):
         """int: How many bits is the CPU?"""
-        if self.__bits is None:
-            self.__bits = self.engine.run_script_generic("""send(Process.pointerSize);""", raw=True, unload=True)[0][0] * 8
-
+        if self.__bits == None:
+            self.__bits = self.run_script_generic("""send(Process.pointerSize);""", raw=True, unload=True)[0][0] * 8
+        
         return self.__bits
 
     @property
     def arch(self):
-        """str: What architecture? (x64, ia32, arm, others?)"""
+        """str: What architecture? (x64, ia32, others?)"""
         try:
             return self.__arch
-        except Exception:
-            known_arch = ['x64', 'ia32', 'arm']
-            arch = self.engine.run_script_generic("""send(Process.arch);""", raw=True, unload=True)[0][0]
+        except:
+            known_arch = ['x64', 'ia32']
+            arch = self.run_script_generic("""send(Process.arch);""", raw=True, unload=True)[0][0]
 
             if arch not in known_arch:
                 raise Exception("Unknown arch returned from Frida: {}".format(arch))
             self.__arch = arch
             return self.__arch
 
     @property
@@ -373,132 +503,108 @@
         """bool: Output extra debugging information."""
         return self.__verbose
 
     @verbose.setter
     def verbose(self, verbose):
         if verbose:
             logging.getLogger().setLevel(logging.DEBUG)
+            #logger.setLevel(logging.DEBUG)
         self.__verbose = verbose
 
     @property
     def target(self):
         """str, int: Target for this session."""
         return self.__target
 
     @target.setter
     def target(self, target):
-
-        # target set will implicitly set argv
-        if isinstance(target, (list, tuple)):
-            self.argv = list(target)
-            target = target[0]
-
-        else:
-            # Place holder until we resolve target
-            self.argv = [target]
-
         # Check if this is a pid
         try:
-            p = next(x for x in self.engine._frida_device.enumerate_processes() if x.pid == common.auto_int(target))
+            p = next(x for x in self.device.device.enumerate_processes() if x.pid == common.auto_int(target))
             target = p.pid
             self.__file_name = p.name
-            self.argv[0] = p.name
 
         except (StopIteration, ValueError):
             pass
 
         if isinstance(target, str):
             full_path = os.path.abspath(target)
             self.__file_name = os.path.basename(full_path)
 
-            # If this string points to an actual file, we will launch it later
             if os.path.isfile(full_path):
                 self._spawn_target = full_path
+            
 
         self.__target = target
 
     @property
     def alive(self):
         """bool: Is this process still alive?"""
         try:
-            next(True for x in self.engine._frida_device.enumerate_processes() if x.pid == self.pid)
+            next(True for x in self.device.device.enumerate_processes() if x.pid == self.pid)
             return True
         except StopIteration:
             return False
 
     @property
     def device(self):
-        """revenge.devices.BaseDevice: What device is this process associated with?"""
-        return self.engine.device
+        """Frida device object for this connection."""
+        return self.__device
 
+    @device.setter
+    def device(self, device):
+        assert isinstance(device, device_types.BaseDevice), "Device must be an instantiation of one of the devices defined in revenge.device_types."
+        self.__device = device
+        """
+        if isinstance(device, device_types.LocalDevice):
+            self.__device = device.device
+
+        elif isinstance(device, device_types.AndroidDevice):
+            self.__device = device.device
+
+        else:
+            error = "Unexpected/unhandled device type of {}".format(type(device))
+            logger.error(error)
+            raise Exception(error)
+        """
+    
     @property
     def BatchContext(self):
         """Returns a BatchContext class for this process.
 
         Example:
-            .. code-block:: python3
-
-                with process.BatchContext() as context:
-                    something(context=context)
+            with process.BatchContext() as context:
+                <stuff>
 
+        BatchContext doc:
         """
         return lambda *args, **kwargs: BatchContext(self, *args, **kwargs)
 
-    @property
-    def _envp(self):
-        """dict: This holds the USER SPECIFIED environment variables. If you
-        do not specify envp, this will be empty but your program will still
-        have the default environment."""
-        return self.__envp
-
-    @_envp.setter
-    @common.validate_argument_types(envp=(dict, type(None)))
-    def _envp(self, envp):
-        self.__envp = envp
-
-    @property
-    def engine(self):
-        """The current engine revenge is using."""
-
-        try:
-            self.__engine._process
-        except AttributeError:
-            self.__engine._process = self
 
-        return self.__engine
-
-
-import inspect
-from . import types, config, devices
+from . import common, types, config, device_types
 from .memory import Memory
 from .threads import Threads
+from .tracer import Tracer
 from .modules import Modules
+from .java import Java
 from .contexts import BatchContext
-from .exceptions import *
-from .techniques import Techniques
-from .plugins import Plugin
-from .engines import Engine
 
 # Doc fixups
 Process.BatchContext.__doc__ += BatchContext.__init__.__doc__
-Process.__doc__ = Process.__init__.__doc__
 
 
 def sigint_handler(sig, frame):
-    sys.exit()
-
+    exit()
 
 signal.signal(signal.SIGINT, sigint_handler)
 
-
 def main():
     signal.signal(signal.SIGINT, sigint_handler)
 
     global process
     process = Process()
 
     while True:
         time.sleep(1)
 
-
 if __name__ == '__main__':
     main()
```

### Comparing `revenge-0.21/setup.py` & `revenge-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 # To use a consistent encoding
-import os
+from codecs import open
+import os, sys, ast
 
 here = os.path.abspath(os.path.dirname(__file__))
-version = '0.21'
+version = '0.9'
 
-# with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+#with open(path.join(here, 'README.md'), encoding='utf-8') as f:
 #    long_description = f.read()
 long_description = "See website for more info."
 
 # Frida 12.6.11 -> https://github.com/frida/frida/issues/986
 
 setup(
     name='revenge',
@@ -27,23 +28,19 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: POSIX :: Linux',
         'Environment :: Console'
     ],
     keywords='frida python3 reversing dbi',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
-    install_requires=['frida==16.2.1', 'prettytable', 'colorama', 'termcolor', 'psutil',
-                      'pyelftools', 'pefile', 'appdirs', 'bs4', 'requests',
-                      'unicorn', 'prompt-toolkit', 'r2pipe', 'pygments'],
+    install_requires=['frida', 'prettytable', 'colorama', 'termcolor', 'psutil', 'pyelftools', 'pefile', 'appdirs', 'bs4', 'requests'],
     extras_require={
-        'dev': ['ipython', 'twine', 'pytest', 'python-coveralls',
-                'coverage==4.5.4', 'pytest-cov', 'pytest-xdist',
-                'sphinxcontrib-napoleon', 'sphinx_rtd_theme',
-                'sphinx-autodoc-typehints', 'pyOpenSSL', 'numpy', 'flake8'],
+        'dev': ['ipython','twine','pytest','python-coveralls','coverage','pytest-cov','pytest-xdist','sphinxcontrib-napoleon', 'sphinx_rtd_theme','sphinx-autodoc-typehints', 'pyOpenSSL', 'numpy'],
     },
     entry_points={
         'console_scripts': [
             'revenge = revenge.cli.cli:main',
         ],
     },
-    include_package_data=True,
+    include_package_data = True,
 )
+
```

